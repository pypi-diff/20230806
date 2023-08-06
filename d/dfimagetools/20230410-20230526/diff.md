# Comparing `tmp/dfimagetools-20230410.tar.gz` & `tmp/dfimagetools-20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfimagetools-20230410.tar", last modified: Mon Apr 10 08:01:47 2023, max compression
+gzip compressed data, was "dfimagetools-20230526.tar", last modified: Fri May 26 06:07:46 2023, max compression
```

## Comparing `dfimagetools-20230410.tar` & `dfimagetools-20230526.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.392297 dfimagetools-20230410/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.172296 dfimagetools-20230410/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.304297 dfimagetools-20230410/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3653 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-04-10 06:21:28.000000 dfimagetools-20230410/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22101 2023-04-10 06:21:27.000000 dfimagetools-20230410/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-04-30 13:22:39.000000 dfimagetools-20230410/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-04-30 13:22:39.000000 dfimagetools-20230410/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-04-30 13:22:39.000000 dfimagetools-20230410/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20230410/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20230410/MANIFEST.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20230410/MANIFEST.test_data.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-10 08:01:47.392297 dfimagetools-20230410/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20230410/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-04-10 06:21:28.000000 dfimagetools-20230410/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.173296 dfimagetools-20230410/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.305297 dfimagetools-20230410/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.306296 dfimagetools-20230410/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-04-10 08:00:49.000000 dfimagetools-20230410/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20230410/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1798 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/dfimagetools-tools.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20230410/config/dpkg/python3-dfimagetools.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-04-10 06:21:28.000000 dfimagetools-20230410/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.306296 dfimagetools-20230410/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20230410/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.307297 dfimagetools-20230410/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20230410/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5687 2022-09-03 04:58:03.000000 dfimagetools-20230410/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.308297 dfimagetools-20230410/dfimagetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      110 2023-04-10 08:00:49.000000 dfimagetools-20230410/dfimagetools/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/artifact_filters.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9053 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/bodyfile.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/data_stream_writer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/environment_variables.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6866 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/file_entry_lister.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2022-09-03 04:58:03.000000 dfimagetools-20230410/dfimagetools/helpers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11121 2022-10-02 12:20:49.000000 dfimagetools-20230410/dfimagetools/path_resolver.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4304 2022-12-26 19:18:50.000000 dfimagetools-20230410/dfimagetools/recursive_hasher.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2022-04-30 13:22:39.000000 dfimagetools-20230410/dfimagetools/resources.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2861 2022-12-26 04:50:18.000000 dfimagetools-20230410/dfimagetools/source_analyzer.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-04-30 13:22:39.000000 dfimagetools-20230410/dfimagetools/windows_registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.309296 dfimagetools-20230410/dfimagetools.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2023-04-10 08:01:47.000000 dfimagetools-20230410/dfimagetools.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      834 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-04-10 08:01:46.000000 dfimagetools-20230410/dfimagetools.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20230410/dfimagetools.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.317297 dfimagetools-20230410/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-04-10 06:21:28.000000 dfimagetools-20230410/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-04-10 06:21:38.000000 dfimagetools-20230410/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.317297 dfimagetools-20230410/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2022-12-18 20:43:00.000000 dfimagetools-20230410/docs/sources/Bodyfile-format.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.348296 dfimagetools-20230410/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-04-09 20:52:07.000000 dfimagetools-20230410/docs/sources/api/dfimagetools.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.375296 dfimagetools-20230410/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2022-11-21 19:36:05.000000 dfimagetools-20230410/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      902 2023-04-10 08:00:49.000000 dfimagetools-20230410/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-02 12:20:49.000000 dfimagetools-20230410/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-04-10 08:01:47.393297 dfimagetools-20230410/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6828 2023-04-10 06:21:28.000000 dfimagetools-20230410/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 18:36:28.000000 dfimagetools-20230410/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 06:21:27.000000 dfimagetools-20230410/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.376297 dfimagetools-20230410/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230410/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/artifact_filters.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20230410/tests/bodyfile.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/environment_variables.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20230410/tests/file_entry_lister.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2022-04-30 13:22:39.000000 dfimagetools-20230410/tests/path_resover.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      655 2022-12-23 10:46:53.000000 dfimagetools-20230410/tests/source_analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2022-10-02 12:20:49.000000 dfimagetools-20230410/tests/test_lib.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.391296 dfimagetools-20230410/tools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20230410/tools/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8865 2022-10-02 12:20:49.000000 dfimagetools-20230410/tools/extract_data_streams.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8136 2022-12-18 20:43:00.000000 dfimagetools-20230410/tools/list_file_entries.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-10-02 12:20:49.000000 dfimagetools-20230410/tools/map_extents.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4465 2022-12-26 19:18:50.000000 dfimagetools-20230410/tools/recursive_hasher.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3866 2022-12-25 20:20:03.000000 dfimagetools-20230410/tools/source_analyzer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2023-04-10 06:21:28.000000 dfimagetools-20230410/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-10 08:01:47.392297 dfimagetools-20230410/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230410/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-04-10 06:21:28.000000 dfimagetools-20230410/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-04-10 06:21:28.000000 dfimagetools-20230410/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2022-04-30 13:22:18.000000 dfimagetools-20230410/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.767302 dfimagetools-20230526/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.650302 dfimagetools-20230526/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.726302 dfimagetools-20230526/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3687 2023-05-25 04:37:23.000000 dfimagetools-20230526/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2023-05-25 04:37:23.000000 dfimagetools-20230526/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5838 2023-05-25 04:37:23.000000 dfimagetools-20230526/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23200 2023-05-25 04:37:23.000000 dfimagetools-20230526/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-04-30 13:22:39.000000 dfimagetools-20230526/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      479 2022-04-30 13:22:39.000000 dfimagetools-20230526/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      292 2022-04-30 13:22:39.000000 dfimagetools-20230526/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2021-10-31 13:10:45.000000 dfimagetools-20230526/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      608 2022-01-29 19:59:40.000000 dfimagetools-20230526/MANIFEST.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-01-29 19:59:40.000000 dfimagetools-20230526/MANIFEST.test_data.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-05-26 06:07:46.767302 dfimagetools-20230526/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-12-26 07:38:07.000000 dfimagetools-20230526/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-24 04:36:16.000000 dfimagetools-20230526/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.650302 dfimagetools-20230526/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.738302 dfimagetools-20230526/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-05-25 04:37:23.000000 dfimagetools-20230526/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-24 04:36:16.000000 dfimagetools-20230526/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-24 04:36:16.000000 dfimagetools-20230526/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.740302 dfimagetools-20230526/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-05-26 05:29:23.000000 dfimagetools-20230526/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       23 2021-12-23 07:30:27.000000 dfimagetools-20230526/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-24 04:36:16.000000 dfimagetools-20230526/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-25 04:37:23.000000 dfimagetools-20230526/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      976 2021-12-26 07:38:07.000000 dfimagetools-20230526/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2021-12-26 07:38:07.000000 dfimagetools-20230526/config/dpkg/dfimagetools-tools.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      105 2021-12-26 07:38:07.000000 dfimagetools-20230526/config/dpkg/python3-dfimagetools.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-24 04:36:16.000000 dfimagetools-20230526/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.740302 dfimagetools-20230526/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2021-12-23 07:30:27.000000 dfimagetools-20230526/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.741302 dfimagetools-20230526/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      229 2021-12-21 12:01:47.000000 dfimagetools-20230526/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5865 2023-05-25 04:37:23.000000 dfimagetools-20230526/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.745302 dfimagetools-20230526/dfimagetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      110 2023-05-26 05:29:23.000000 dfimagetools-20230526/dfimagetools/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2022-10-02 12:20:49.000000 dfimagetools-20230526/dfimagetools/artifact_filters.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9053 2022-10-02 12:20:49.000000 dfimagetools-20230526/dfimagetools/bodyfile.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2022-10-02 12:20:49.000000 dfimagetools-20230526/dfimagetools/data_stream_writer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-10-02 12:20:49.000000 dfimagetools-20230526/dfimagetools/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3493 2023-04-16 06:53:17.000000 dfimagetools-20230526/dfimagetools/environment_variables.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6916 2023-05-25 04:41:19.000000 dfimagetools-20230526/dfimagetools/file_entry_lister.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-05-25 04:37:23.000000 dfimagetools-20230526/dfimagetools/helpers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11121 2022-10-02 12:20:49.000000 dfimagetools-20230526/dfimagetools/path_resolver.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4304 2022-12-26 19:18:50.000000 dfimagetools-20230526/dfimagetools/recursive_hasher.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2362 2023-04-16 06:53:17.000000 dfimagetools-20230526/dfimagetools/resources.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2861 2022-12-26 04:50:18.000000 dfimagetools-20230526/dfimagetools/source_analyzer.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2022-04-30 13:22:39.000000 dfimagetools-20230526/dfimagetools/windows_registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.746302 dfimagetools-20230526/dfimagetools.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2023-05-26 06:07:45.000000 dfimagetools-20230526/dfimagetools.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2023-05-26 06:07:46.000000 dfimagetools-20230526/dfimagetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-26 06:07:45.000000 dfimagetools-20230526/dfimagetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      860 2023-05-26 06:07:45.000000 dfimagetools-20230526/dfimagetools.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       13 2023-05-26 06:07:45.000000 dfimagetools-20230526/dfimagetools.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      388 2021-12-26 07:38:07.000000 dfimagetools-20230526/dfimagetools.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.747302 dfimagetools-20230526/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2023-05-24 04:36:22.000000 dfimagetools-20230526/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      528 2022-11-21 19:36:05.000000 dfimagetools-20230526/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-24 04:36:22.000000 dfimagetools-20230526/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.748302 dfimagetools-20230526/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2022-12-18 20:43:00.000000 dfimagetools-20230526/docs/sources/Bodyfile-format.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.749302 dfimagetools-20230526/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2023-04-09 20:52:07.000000 dfimagetools-20230526/docs/sources/api/dfimagetools.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       73 2022-11-21 19:36:05.000000 dfimagetools-20230526/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.749302 dfimagetools-20230526/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1693 2022-11-21 19:36:05.000000 dfimagetools-20230526/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      296 2022-11-21 19:36:05.000000 dfimagetools-20230526/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      930 2023-05-25 04:37:23.000000 dfimagetools-20230526/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-10-02 12:20:49.000000 dfimagetools-20230526/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1490 2023-05-26 06:07:46.768302 dfimagetools-20230526/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6828 2023-05-24 04:36:16.000000 dfimagetools-20230526/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 18:36:28.000000 dfimagetools-20230526/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-24 04:36:16.000000 dfimagetools-20230526/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.753302 dfimagetools-20230526/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230526/tests/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7807 2023-04-16 06:53:17.000000 dfimagetools-20230526/tests/artifact_filters.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4034 2022-01-29 19:59:40.000000 dfimagetools-20230526/tests/bodyfile.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2291 2022-04-30 13:22:39.000000 dfimagetools-20230526/tests/environment_variables.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3293 2022-01-29 19:59:40.000000 dfimagetools-20230526/tests/file_entry_lister.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11717 2023-04-16 06:53:17.000000 dfimagetools-20230526/tests/path_resover.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      655 2022-12-23 10:46:53.000000 dfimagetools-20230526/tests/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2022-10-02 12:20:49.000000 dfimagetools-20230526/tests/test_lib.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.765302 dfimagetools-20230526/tools/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       57 2021-12-21 09:32:11.000000 dfimagetools-20230526/tools/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8865 2022-10-02 12:20:49.000000 dfimagetools-20230526/tools/extract_data_streams.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     8136 2022-12-18 20:43:00.000000 dfimagetools-20230526/tools/list_file_entries.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5100 2022-10-02 12:20:49.000000 dfimagetools-20230526/tools/map_extents.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4465 2022-12-26 19:18:50.000000 dfimagetools-20230526/tools/recursive_hasher.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3866 2022-12-25 20:20:03.000000 dfimagetools-20230526/tools/source_analyzer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2023-05-24 17:58:01.000000 dfimagetools-20230526/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-26 06:07:46.767302 dfimagetools-20230526/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-12-21 09:32:11.000000 dfimagetools-20230526/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-24 04:36:16.000000 dfimagetools-20230526/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-24 04:36:16.000000 dfimagetools-20230526/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      655 2022-04-30 13:22:18.000000 dfimagetools-20230526/utils/update_release.sh
```

### Comparing `dfimagetools-20230410/.github/workflows/test_docker.yml` & `dfimagetools-20230526/.github/workflows/test_docker.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['37']
+        version: ['38']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools
+        dnf install -y @development-tools python3 python3-devel libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-pyyaml python3-setuptools
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
@@ -41,28 +41,28 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
+        apt-get install -y build-essential python3 python3-dev libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
```

### Comparing `dfimagetools-20230410/.github/workflows/test_docs.yml` & `dfimagetools-20230526/.github/workflows/test_docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -32,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
+        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv libbde-python3 libcreg-python3 libewf-python3 libfsapfs-python3 libfsext-python3 libfsfat-python3 libfshfs-python3 libfsntfs-python3 libfsxfs-python3 libfvde-python3 libfwnt-python3 libluksde-python3 libmodi-python3 libphdi-python3 libqcow-python3 libregf-python3 libsigscan-python3 libsmdev-python3 libsmraw-python3 libvhdi-python3 libvmdk-python3 libvsapm-python3 libvsgpt-python3 libvshadow-python3 libvslvm-python3 python3-artifacts python3-cffi-backend python3-cryptography python3-dfdatetime python3-dfvfs python3-dfwinreg python3-distutils python3-dtfabric python3-idna python3-pip python3-pytsk3 python3-pyxattr python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfimagetools-20230410/.pylintrc` & `dfimagetools-20230526/.pylintrc`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# Pylint 2.14.x configuration file
+# Pylint 2.17.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
 [MAIN]
 
 # Analyse import fallback blocks. This can be used to support both Python 2 and
 # 3 compatible code, which means that the block might have code that exists
 # only in one or another interpreter, leading to false positives when analysed.
 analyse-fallback-blocks=no
 
+# Clear in-memory caches upon conclusion of linting. Useful if running pylint
+# in a server-like mode.
+clear-cache-post-run=no
+
 # Load and enable all available extensions. Use --list-extensions to see a list
 # all available extensions.
 #enable-all-extensions=
 
 # In error mode, messages with a category besides ERROR or FATAL are
 # suppressed, and no reports are done by default. Error mode is compatible with
 # disabling specific errors.
@@ -21,44 +25,46 @@
 # Always return a 0 (non-error) status code, even if lint errors are found.
 # This is primarily useful in continuous integration scripts.
 #exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
-extension-pkg-allow-list=pybde,pycreg,pyewf,pyfsapfs,pyfsext,pyfshfs,pyfsntfs,pyfsxfs,pyfvde,pyfwnt,pyluksde,pymodi,pyphdi,pyqcow,pyregf,pysigscan,pysmdev,pysmraw,pytsk3,pyvhdi,pyvmdk,pyvsgpt,pyvshadow,pyvslvm,xattr
+extension-pkg-allow-list=pybde,pycreg,pyewf,pyfsapfs,pyfsext,pyfsfat,pyfshfs,pyfsntfs,pyfsxfs,pyfvde,pyfwnt,pyluksde,pymodi,pyphdi,pyqcow,pyregf,pysigscan,pysmdev,pysmraw,pytsk3,pyvhdi,pyvmdk,pyvsapm,pyvsgpt,pyvshadow,pyvslvm,xattr
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code. (This is an alternative name to extension-pkg-allow-list
 # for backward compatibility.)
 extension-pkg-whitelist=
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
-# Specify a score threshold to be exceeded before program exits with error.
+# Specify a score threshold under which the program will exit with error.
 fail-under=10
 
 # Interpret the stdin as a python script, whose filename needs to be passed as
 # the module_or_package argument.
 #from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the ignore-list. The
-# regex matches against paths and can be in Posix or Windows format.
+# Add files or directories matching the regular expressions patterns to the
+# ignore-list. The regex matches against paths and can be in Posix or Windows
+# format. Because '\\' represents the directory delimiter on Windows systems,
+# it can't be used as an escape character.
 ignore-paths=
 
-# Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths. The default value ignores Emacs file
-# locks
+# Files or directories matching the regular expression patterns are skipped.
+# The regex matches against base names, not paths. The default value ignores
+# Emacs file locks
 ignore-patterns=^\.#
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
 ignored-modules=
@@ -89,249 +95,32 @@
 # the version used to run pylint.
 py-version=3.11
 
 # Discover python modules and packages in the file system subtree.
 # recursive=no
 recursive=yes
 
+# Add paths to the list of the source roots. Supports globbing patterns. The
+# source root is an absolute path or a path relative to the current working
+# directory used to determine a package namespace for modules located under the
+# source root.
+source-roots=
+
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
 # In verbose mode, extra non-checker-related info will be displayed.
 #verbose=
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'fatal', 'error', 'warning', 'refactor',
-# 'convention', and 'info' which contain the number of messages in each
-# category, as well as 'statement' which is the total number of statements
-# analyzed. This score is used by the global evaluation report (RP0004).
-evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-#output-format=
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-# score=yes
-score=no
-
-
-[MESSAGES CONTROL]
-
-# Only show warnings with the listed confidence levels. Leave empty to show
-# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
-# UNDEFINED.
-confidence=HIGH,
-           CONTROL_FLOW,
-           INFERENCE,
-           INFERENCE_FAILURE,
-           UNDEFINED
-
-# Disable the message, report, category or checker with the given id(s). You
-# can either give multiple identifiers separated by comma (,) or put this
-# option multiple times (only on the command line, not in the configuration
-# file where it should appear only once). You can also use "--disable=all" to
-# disable everything first and then re-enable specific checks. For example, if
-# you want to run only the similarities checker, you can use "--disable=all
-# --enable=similarities". If you want to run only the classes checker, but have
-# no Warning level messages displayed, use "--disable=all --enable=classes
-# --disable=W".
-disable=assignment-from-none,
-        bad-inline-option,
-        consider-using-f-string,
-        deprecated-pragma,
-        duplicate-code,
-        file-ignored,
-        fixme,
-        locally-disabled,
-        logging-format-interpolation,
-        logging-fstring-interpolation,
-        missing-param-doc,
-        raise-missing-from,
-        raw-checker-failed,
-        super-with-arguments,
-        suppressed-message,
-        too-few-public-methods,
-        too-many-ancestors,
-        too-many-boolean-expressions,
-        too-many-branches,
-        too-many-instance-attributes,
-        too-many-lines,
-        too-many-locals,
-        too-many-nested-blocks,
-        too-many-public-methods,
-        too-many-return-statements,
-        too-many-statements,
-        unsubscriptable-object,
-        useless-object-inheritance,
-        useless-suppression
-
-# Enable the message, report, category or checker with the given id(s). You can
-# either give multiple identifier separated by comma (,) or put this option
-# multiple time (only on the command line, not in the configuration file where
-# it should appear only once). See also the "--disable" option for examples.
-enable=c-extension-no-member
-
-
-[VARIABLES]
-
-# List of additional names supposed to be defined in builtins. Remember that
-# you should avoid defining new builtins when possible.
-additional-builtins=
-
-# Tells whether unused global variables should be treated as a violation.
-allow-global-unused-variables=yes
-
-# List of names allowed to shadow builtins
-allowed-redefined-builtins=
-
-# List of strings which can identify a callback function by name. A callback
-# name must start or end with one of those strings.
-callbacks=cb_,
-          _cb
-
-# A regular expression matching the name of dummy variables (i.e. expected to
-# not be used).
-dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
-
-# Argument names that match this expression will be ignored. Default to name
-# with leading underscore.
-ignored-argument-names=_.*|^ignored_|^unused_
-
-# Tells whether we should check for unused import in __init__ files.
-init-import=no
-
-# List of qualified module names which can have objects that can redefine
-# builtins.
-redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
-
-
-[TYPECHECK]
-
-# List of decorators that produce context managers, such as
-# contextlib.contextmanager. Add to this list to register other decorators that
-# produce valid context managers.
-contextmanager-decorators=contextlib.contextmanager
-
-# List of members which are set dynamically and missed by pylint inference
-# system, and so shouldn't trigger E1101 when accessed. Python regular
-# expressions are accepted.
-generated-members=
-
-# Tells whether to warn about missing members when the owner of the attribute
-# is inferred to be None.
-ignore-none=yes
-
-# This flag controls whether pylint should warn about no-member and similar
-# checks whenever an opaque object is returned when inferring. The inference
-# can return multiple potential results while evaluating a Python object, but
-# some branches might not be evaluated, which results in partial inference. In
-# that case, it might be useful to still emit no-member and other checks for
-# the rest of the inferred objects.
-ignore-on-opaque-inference=yes
-
-# List of symbolic message names to ignore for Mixin members.
-ignored-checks-for-mixins=no-member,
-                          not-async-context-manager,
-                          not-context-manager,
-                          attribute-defined-outside-init
-
-# List of class names for which member attributes should not be checked (useful
-# for classes with dynamically set attributes). This supports the use of
-# qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
-
-# Show a hint with possible names when a member name was not found. The aspect
-# of finding the hint is based on edit distance.
-missing-member-hint=yes
-
-# The minimum edit distance a name should have in order to be considered a
-# similar match for a missing member name.
-missing-member-hint-distance=1
-
-# The total number of similar names that should be taken in consideration when
-# showing a hint for a missing member.
-missing-member-max-choices=1
-
-# Regex pattern to define which classes are considered mixins.
-mixin-class-rgx=.*[Mm]ixin
-
-# List of decorators that change the signature of a decorated function.
-signature-mutators=
-
-
-[LOGGING]
-
-# The type of string formatting that logging methods do. `old` means using %
-# formatting, `new` is for `{}` formatting.
-logging-format-style=old
-
-# Logging modules to check that the string format arguments are in logging
-# function parameter format.
-logging-modules=logging
-
-
-[DESIGN]
-
-# List of regular expressions of class ancestor names to ignore when counting
-# public methods (see R0903)
-exclude-too-few-public-methods=
-
-# List of qualified class names to ignore when counting class parents (see
-# R0901)
-ignored-parents=
-
-# Maximum number of arguments for function / method.
-# max-args=5
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
 # naming-style. If left empty, argument names will be checked with the set
@@ -456,70 +245,102 @@
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 # These decorators are taken in consideration only for invalid-name.
 property-classes=abc.abstractproperty
 
+# Regular expression matching correct type alias names. If left empty, type
+# alias names will be checked with the set naming style.
+#typealias-rgx=
+
 # Regular expression matching correct type variable names. If left empty, type
 # variable names will be checked with the set naming style.
 #typevar-rgx=
 
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
 # naming-style. If left empty, variable names will be checked with the set
 # naming style.
 #variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
-[EXCEPTIONS]
-
-# Exceptions that will emit a warning when caught.
-overgeneral-exceptions=BaseException,
-                       Exception
-
-
 [CLASSES]
 
 # Warn about protected attribute access inside special methods
 check-protected-access-in-special-methods=no
 
 # List of method names used to declare (i.e. assign) instance attributes.
 defining-attr-methods=__init__,
                       __new__,
                       setUp,
+                      asyncSetUp,
                       __post_init__
 
 # List of member names, which should be excluded from the protected access
 # warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
+exclude-protected=_asdict,_fields,_replace,_source,_make,os._exit
 
 # List of valid names for the first argument in a class method.
 valid-classmethod-first-arg=cls
 
 # List of valid names for the first argument in a metaclass class method.
+# valid-metaclass-classmethod-first-arg=mcs
 valid-metaclass-classmethod-first-arg=cls
 
 
-[MISCELLANEOUS]
+[DESIGN]
 
-# List of note tags to take in consideration, separated by a comma.
-notes=FIXME,
-      XXX,
-      TODO
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
 
-# Regular expression of note tags to take in consideration.
-notes-rgx=
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=builtins.BaseException,builtins.Exception
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -546,14 +367,196 @@
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
 
 
+[IMPORTS]
+
+# List of modules that can be imported at any level, not just the top level
+# one.
+allow-any-import-level=
+
+# Allow explicit reexports by alias from a package __init__.
+allow-reexport-from-package=no
+
+# Allow wildcard imports from modules that define __all__.
+allow-wildcard-with-all=no
+
+# Deprecated modules which should not be used, separated by a comma.
+deprecated-modules=
+
+# Output a graph (.gv or any supported image format) of external dependencies
+# to the given file (report RP0402 must not be disabled).
+ext-import-graph=
+
+# Output a graph (.gv or any supported image format) of all (i.e. internal and
+# external) dependencies to the given file (report RP0402 must not be
+# disabled).
+import-graph=
+
+# Output a graph (.gv or any supported image format) of internal dependencies
+# to the given file (report RP0402 must not be disabled).
+int-import-graph=
+
+# Force import order to recognize a module as part of the standard
+# compatibility libraries.
+known-standard-library=
+
+# Force import order to recognize a module as part of a third party library.
+known-third-party=enchant
+
+# Couples of modules and preferred modules, separated by a comma.
+preferred-modules=
+
+
+[LOGGING]
+
+# The type of string formatting that logging methods do. `old` means using %
+# formatting, `new` is for `{}` formatting.
+logging-format-style=old
+
+# Logging modules to check that the string format arguments are in logging
+# function parameter format.
+logging-modules=logging
+
+
+[MESSAGES CONTROL]
+
+# Only show warnings with the listed confidence levels. Leave empty to show
+# all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
+# UNDEFINED.
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
+
+# Disable the message, report, category or checker with the given id(s). You
+# can either give multiple identifiers separated by comma (,) or put this
+# option multiple times (only on the command line, not in the configuration
+# file where it should appear only once). You can also use "--disable=all" to
+# disable everything first and then re-enable specific checks. For example, if
+# you want to run only the similarities checker, you can use "--disable=all
+# --enable=similarities". If you want to run only the classes checker, but have
+# no Warning level messages displayed, use "--disable=all --enable=classes
+# --disable=W".
+disable=assignment-from-none,
+        bad-inline-option,
+        consider-using-f-string,
+        deprecated-pragma,
+        duplicate-code,
+        file-ignored,
+        fixme,
+        locally-disabled,
+        logging-format-interpolation,
+        logging-fstring-interpolation,
+        missing-param-doc,
+        raise-missing-from,
+        raw-checker-failed,
+        super-with-arguments,
+        suppressed-message,
+        too-few-public-methods,
+        too-many-ancestors,
+        too-many-boolean-expressions,
+        too-many-branches,
+        too-many-instance-attributes,
+        too-many-lines,
+        too-many-locals,
+        too-many-nested-blocks,
+        too-many-public-methods,
+        too-many-return-statements,
+        too-many-statements,
+        unsubscriptable-object,
+        useless-object-inheritance,
+        useless-suppression,
+        use-symbolic-message-instead
+
+# Enable the message, report, category or checker with the given id(s). You can
+# either give multiple identifier separated by comma (,) or put this option
+# multiple time (only on the command line, not in the configuration file where
+# it should appear only once). See also the "--disable" option for examples.
+enable=c-extension-no-member
+
+
+[METHOD_ARGS]
+
+# List of qualified names (i.e., library.method) which require a timeout
+# parameter e.g. 'requests.api.get,requests.api.post'
+timeout-methods=requests.api.delete,requests.api.get,requests.api.head,requests.api.options,requests.api.patch,requests.api.post,requests.api.put,requests.api.request
+
+
+[MISCELLANEOUS]
+
+# List of note tags to take in consideration, separated by a comma.
+notes=FIXME,
+      XXX,
+      TODO
+
+# Regular expression of note tags to take in consideration.
+notes-rgx=
+
+
+[REFACTORING]
+
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
+
+[SIMILARITIES]
+
+# Comments are removed from the similarity computation
+ignore-comments=yes
+
+# Docstrings are removed from the similarity computation
+ignore-docstrings=yes
+
+# Imports are removed from the similarity computation
+ignore-imports=yes
+
+# Signatures are removed from the similarity computation
+ignore-signatures=yes
+
+# Minimum lines number of a similarity.
+min-similarity-lines=4
+
+
 [SPELLING]
 
 # Limits count of emitted suggestions for spelling mistakes.
 max-spelling-suggestions=4
 
 # Spelling dictionary name. Available dictionaries: en_AG (hunspell), en_AU
 # (hunspell), en_BS (hunspell), en_BW (hunspell), en_BZ (hunspell), en_CA
@@ -575,82 +578,102 @@
 spelling-private-dict-file=
 
 # Tells whether to store unknown words to the private dictionary (see the
 # --spelling-private-dict-file option) instead of raising a message.
 spelling-store-unknown-words=no
 
 
-[SIMILARITIES]
-
-# Comments are removed from the similarity computation
-ignore-comments=yes
-
-# Docstrings are removed from the similarity computation
-ignore-docstrings=yes
-
-# Imports are removed from the similarity computation
-ignore-imports=yes
-
-# Signatures are removed from the similarity computation
-ignore-signatures=yes
-
-# Minimum lines number of a similarity.
-min-similarity-lines=4
-
-
 [STRING]
 
 # This flag controls whether inconsistent-quotes generates a warning when the
 # character used as a quote delimiter is used inconsistently within a module.
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[IMPORTS]
+[TYPECHECK]
 
-# List of modules that can be imported at any level, not just the top level
-# one.
-allow-any-import-level=
+# List of decorators that produce context managers, such as
+# contextlib.contextmanager. Add to this list to register other decorators that
+# produce valid context managers.
+contextmanager-decorators=contextlib.contextmanager
 
-# Allow wildcard imports from modules that define __all__.
-allow-wildcard-with-all=no
+# List of members which are set dynamically and missed by pylint inference
+# system, and so shouldn't trigger E1101 when accessed. Python regular
+# expressions are accepted.
+generated-members=
 
-# Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=
+# Tells whether to warn about missing members when the owner of the attribute
+# is inferred to be None.
+ignore-none=yes
 
-# Output a graph (.gv or any supported image format) of external dependencies
-# to the given file (report RP0402 must not be disabled).
-ext-import-graph=
+# This flag controls whether pylint should warn about no-member and similar
+# checks whenever an opaque object is returned when inferring. The inference
+# can return multiple potential results while evaluating a Python object, but
+# some branches might not be evaluated, which results in partial inference. In
+# that case, it might be useful to still emit no-member and other checks for
+# the rest of the inferred objects.
+ignore-on-opaque-inference=yes
 
-# Output a graph (.gv or any supported image format) of all (i.e. internal and
-# external) dependencies to the given file (report RP0402 must not be
-# disabled).
-import-graph=
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
 
-# Output a graph (.gv or any supported image format) of internal dependencies
-# to the given file (report RP0402 must not be disabled).
-int-import-graph=
+# List of class names for which member attributes should not be checked (useful
+# for classes with dynamically set attributes). This supports the use of
+# qualified names.
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
-# Force import order to recognize a module as part of the standard
-# compatibility libraries.
-known-standard-library=
+# Show a hint with possible names when a member name was not found. The aspect
+# of finding the hint is based on edit distance.
+missing-member-hint=yes
 
-# Force import order to recognize a module as part of a third party library.
-known-third-party=enchant
+# The minimum edit distance a name should have in order to be considered a
+# similar match for a missing member name.
+missing-member-hint-distance=1
 
-# Couples of modules and preferred modules, separated by a comma.
-preferred-modules=
+# The total number of similar names that should be taken in consideration when
+# showing a hint for a missing member.
+missing-member-max-choices=1
 
+# Regex pattern to define which classes are considered mixins.
+mixin-class-rgx=.*[Mm]ixin
 
-[REFACTORING]
+# List of decorators that change the signature of a decorated function.
+signature-mutators=
 
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
 
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
+[VARIABLES]
+
+# List of additional names supposed to be defined in builtins. Remember that
+# you should avoid defining new builtins when possible.
+additional-builtins=
+
+# Tells whether unused global variables should be treated as a violation.
+allow-global-unused-variables=yes
+
+# List of names allowed to shadow builtins
+allowed-redefined-builtins=
+
+# List of strings which can identify a callback function by name. A callback
+# name must start or end with one of those strings.
+callbacks=cb_,
+          _cb
+
+# A regular expression matching the name of dummy variables (i.e. expected to
+# not be used).
+dummy-variables-rgx=_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_
+
+# Argument names that match this expression will be ignored.
+ignored-argument-names=_.*|^ignored_|^unused_
+
+# Tells whether we should check for unused import in __init__ files.
+init-import=no
+
+# List of qualified module names which can have objects that can redefine
+# builtins.
+redefining-builtins-modules=six.moves,past.builtins,future.builtins,builtins,io
```

### Comparing `dfimagetools-20230410/LICENSE` & `dfimagetools-20230526/LICENSE`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/MANIFEST.in` & `dfimagetools-20230526/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/MANIFEST.test_data.in` & `dfimagetools-20230526/MANIFEST.test_data.in`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/PKG-INFO` & `dfimagetools-20230526/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20230410
+Version: 20230526
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfimagetools-20230410/appveyor.yml` & `dfimagetools-20230526/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/config/appveyor/install.ps1` & `dfimagetools-20230526/config/appveyor/install.ps1`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
-$Dependencies = "PyYAML artifacts cffi cryptography dfdatetime dfvfs dfwinreg dtfabric idna libbde libcreg libewf libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libregf libsigscan libsmdev libsmraw libvhdi libvmdk libvsgpt libvshadow libvslvm pytsk3 xattr"
+$Dependencies = "PyYAML artifacts cffi cryptography dfdatetime dfvfs dfwinreg dtfabric idna libbde libcreg libewf libfsapfs libfsext libfsfat libfshfs libfsntfs libfsxfs libfvde libfwnt libluksde libmodi libphdi libqcow libregf libsigscan libsmdev libsmraw libvhdi libvmdk libvsapm libvsgpt libvshadow libvslvm pytsk3 xattr"
 
 If ($Dependencies.Length -gt 0)
 {
 	$Dependencies = ${Dependencies} -split " "
 
-	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1 | %{ '$_' }"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
 	Write-Host (${Output} | Out-String)
 
 	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
 	{
 		$Track = "stable"
 	}
 	Else
 	{
 		$Track = $env:APPVEYOR_REPO_BRANCH
 	}
 	New-Item -ItemType "directory" -Name "dependencies"
 
 	$env:PYTHONPATH = "..\l2tdevtools"
 
-	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
 	Write-Host (${Output} | Out-String)
 }
```

### Comparing `dfimagetools-20230410/config/appveyor/runtests.sh` & `dfimagetools-20230526/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/config/dpkg/control` & `dfimagetools-20230526/config/dpkg/control`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Build-Depends: debhelper (>= 9), dh-python, python3-all (>= 3.6~), python3-setuptools
 Standards-Version: 4.1.4
 X-Python3-Version: >= 3.6
 Homepage: https://github.com/log2timeline/dfimagetools
 
 Package: python3-dfimagetools
 Architecture: all
-Depends: libbde-python3 (>= 20220121), libcreg-python3 (>= 20200725), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220816), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libregf-python3 (>= 20201002), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-artifacts (>= 20220219), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20220816), python3-dfvfs (>= 20220831), python3-dfwinreg (>= 20211207), python3-dtfabric (>= 20220219), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
+Depends: libbde-python3 (>= 20220121), libcreg-python3 (>= 20200725), libewf-python3 (>= 20131210), libfsapfs-python3 (>= 20220709), libfsext-python3 (>= 20220829), libfsfat-python3 (>= 20220925), libfshfs-python3 (>= 20220831), libfsntfs-python3 (>= 20211229), libfsxfs-python3 (>= 20220829), libfvde-python3 (>= 20220121), libfwnt-python3 (>= 20210717), libluksde-python3 (>= 20220121), libmodi-python3 (>= 20210405), libphdi-python3 (>= 20220228), libqcow-python3 (>= 20201213), libregf-python3 (>= 20201002), libsigscan-python3 (>= 20191221), libsmdev-python3 (>= 20140529), libsmraw-python3 (>= 20140612), libvhdi-python3 (>= 20201014), libvmdk-python3 (>= 20140421), libvsapm-python3 (>= 20230506), libvsgpt-python3 (>= 20211115), libvshadow-python3 (>= 20160109), libvslvm-python3 (>= 20160109), python3-artifacts (>= 20220219), python3-cffi-backend (>= 1.9.1), python3-cryptography (>= 2.0.2), python3-dfdatetime (>= 20221112), python3-dfvfs (>= 20220831), python3-dfwinreg (>= 20211207), python3-dtfabric (>= 20220219), python3-idna (>= 2.5), python3-pytsk3 (>= 20210419), python3-pyxattr (>= 0.7.2), python3-yaml (>= 3.10), ${misc:Depends}
 Description: Python 3 module of dfImageTools
  Collection of tools to process storage media images.
 
 Package: dfimagetools-tools
 Architecture: all
 Depends: python3-dfimagetools (>= ${binary:Version}), ${misc:Depends}
 Description: Tools of dfImageTools
```

### Comparing `dfimagetools-20230410/config/dpkg/copyright` & `dfimagetools-20230526/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dependencies.ini` & `dfimagetools-20230526/dependencies.ini`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dpkg_name: python3-cryptography
 minimum_version: 2.0.2
 rpm_name: python3-cryptography
 version_property: __version__
 
 [dfdatetime]
 dpkg_name: python3-dfdatetime
-minimum_version: 20220816
+minimum_version: 20221112
 rpm_name: python3-dfdatetime
 version_property: __version__
 
 [dfvfs]
 dpkg_name: python3-dfvfs
 minimum_version: 20220831
 rpm_name: python3-dfvfs
@@ -88,15 +88,15 @@
 pypi_name: libfsext-python
 rpm_name: libfsext-python3
 version_property: get_version()
 
 [pyfsfat]
 dpkg_name: libfsfat-python3
 l2tbinaries_name: libfsfat
-minimum_version: 20220816
+minimum_version: 20220925
 pypi_name: libfsfat-python
 rpm_name: libfsfat-python3
 version_property: get_version()
 
 [pyfshfs]
 dpkg_name: libfshfs-python3
 l2tbinaries_name: libfshfs
@@ -219,14 +219,22 @@
 dpkg_name: libvmdk-python3
 l2tbinaries_name: libvmdk
 minimum_version: 20140421
 pypi_name: libvmdk-python
 rpm_name: libvmdk-python3
 version_property: get_version()
 
+[pyvsapm]
+dpkg_name: libvsapm-python3
+l2tbinaries_name: libvsapm
+minimum_version: 20230506
+pypi_name: libvsapm-python
+rpm_name: libvsapm-python3
+version_property: get_version()
+
 [pyvsgpt]
 dpkg_name: libvsgpt-python3
 l2tbinaries_name: libvsgpt
 minimum_version: 20211115
 pypi_name: libvsgpt-python
 rpm_name: libvsgpt-python3
 version_property: get_version()
```

### Comparing `dfimagetools-20230410/dfimagetools/artifact_filters.py` & `dfimagetools-20230526/dfimagetools/artifact_filters.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/bodyfile.py` & `dfimagetools-20230526/dfimagetools/bodyfile.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/data_stream_writer.py` & `dfimagetools-20230526/dfimagetools/data_stream_writer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/decorators.py` & `dfimagetools-20230526/dfimagetools/decorators.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/environment_variables.py` & `dfimagetools-20230526/dfimagetools/environment_variables.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/file_entry_lister.py` & `dfimagetools-20230526/dfimagetools/file_entry_lister.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,45 +39,47 @@
 
     Args:
       base_path_specs (list[dfvfs.PathSpec]): source path specification.
 
     Returns:
       list[str]: path segments.
     """
-    if not base_path_spec.HasParent() or not base_path_spec.parent:
+    if not base_path_spec:
       return ['']
 
-    if base_path_spec.parent.type_indicator in (
+    path_segments = self._GetBasePathSegments(base_path_spec.parent)
+
+    if base_path_spec.type_indicator in (
         dfvfs_definitions.TYPE_INDICATOR_APFS_CONTAINER,
         dfvfs_definitions.TYPE_INDICATOR_GPT,
         dfvfs_definitions.TYPE_INDICATOR_LVM):
       volume_system = dfvfs_volume_system_factory.Factory.NewVolumeSystem(
-          base_path_spec.parent.type_indicator)
-      volume_system.Open(base_path_spec.parent)
+          base_path_spec.type_indicator)
+      volume_system.Open(base_path_spec)
 
-      volume = volume_system.GetVolumeByIdentifier(
-          base_path_spec.parent.location[1:])
+      volume = volume_system.GetVolumeByIdentifier(base_path_spec.location[1:])
 
-      if base_path_spec.parent.type_indicator == (
-          dfvfs_definitions.TYPE_INDICATOR_GPT):
+      if base_path_spec.type_indicator == dfvfs_definitions.TYPE_INDICATOR_GPT:
         volume_identifier_prefix = 'gpt'
       else:
         volume_identifier_prefix = volume_system.VOLUME_IDENTIFIER_PREFIX
 
       volume_identifier = volume.GetAttribute('identifier')
 
       volume_path_segment = (
           f'{volume_identifier_prefix:s}{{{volume_identifier.value:s}}}')
-      return ['', volume_path_segment]
+      path_segments.append(volume_path_segment)
+      return path_segments
 
-    if base_path_spec.parent.type_indicator == (
+    if base_path_spec.type_indicator == (
         dfvfs_definitions.TYPE_INDICATOR_TSK_PARTITION):
-      return base_path_spec.parent.location.split('/')
+      path_segments.append(base_path_spec.location[1:])
+      return path_segments
 
-    return ['']
+    return path_segments
 
   def _GetPathSpecificationString(self, path_spec):
     """Retrieves a printable string representation of the path specification.
 
     Args:
       path_spec (dfvfs.PathSpec): path specification.
 
@@ -159,15 +161,15 @@
         path_specification_string = self._GetPathSpecificationString(
             base_path_spec)
         logging.warning(''.join([
             'Unable to open base path specification:\n',
             path_specification_string]))
         return
 
-      base_path_segments = self._GetBasePathSegments(base_path_spec)
+      base_path_segments = self._GetBasePathSegments(base_path_spec.parent)
       for result in self._ListFileEntry(
           file_system, file_entry, base_path_segments):
         yield result
 
   def ListFileEntriesWithFindSpecs(self, base_path_specs, find_specs):
     """Lists file entries in the base path specifications.
 
@@ -185,15 +187,15 @@
 
       if dfvfs_path_spec_factory.Factory.IsSystemLevelTypeIndicator(
           base_path_spec.type_indicator):
         mount_point = base_path_spec
       else:
         mount_point = base_path_spec.parent
 
-      base_path_segments = self._GetBasePathSegments(base_path_spec)
+      base_path_segments = self._GetBasePathSegments(base_path_spec.parent)
 
       searcher = file_system_searcher.FileSystemSearcher(
           file_system, mount_point)
       for path_spec in searcher.Find(find_specs=find_specs):
         file_entry = dfvfs_resolver.Resolver.OpenFileEntry(path_spec)
         path_segments = file_system.SplitPath(path_spec.location)
```

### Comparing `dfimagetools-20230410/dfimagetools/helpers.py` & `dfimagetools-20230526/dfimagetools/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 def SetDFVFSBackEnd(back_end):
   """Sets the dfVFS back-end.
 
   Args:
     back_end (str): dfVFS back-end.
   """
-  if back_end == 'EXT':
+  if back_end == 'APM':
+    dfvfs_definitions.PREFERRED_APM_BACK_END = (
+        dfvfs_definitions.TYPE_INDICATOR_APM)
+
+  elif back_end == 'EXT':
     dfvfs_definitions.PREFERRED_EXT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_EXT)
 
   elif back_end == 'FAT':
     dfvfs_definitions.PREFERRED_FAT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_FAT)
 
@@ -27,15 +31,17 @@
         dfvfs_definitions.TYPE_INDICATOR_HFS)
 
   elif back_end == 'NTFS':
     dfvfs_definitions.PREFERRED_NTFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_NTFS)
 
   elif back_end == 'TSK':
-    dfvfs_definitions.PREFERRED_EXT_BACK_END = (
+    dfvfs_definitions.PREFERRED_APM_BACK_END = (
+        dfvfs_definitions.TYPE_INDICATOR_TSK)
+    dfvfs_definitions.PREFERRED_APM_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
     dfvfs_definitions.PREFERRED_FAT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
     dfvfs_definitions.PREFERRED_GPT_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK_PARTITION)
     dfvfs_definitions.PREFERRED_HFS_BACK_END = (
         dfvfs_definitions.TYPE_INDICATOR_TSK)
```

### Comparing `dfimagetools-20230410/dfimagetools/path_resolver.py` & `dfimagetools-20230526/dfimagetools/path_resolver.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/recursive_hasher.py` & `dfimagetools-20230526/dfimagetools/recursive_hasher.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/resources.py` & `dfimagetools-20230526/dfimagetools/resources.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/source_analyzer.py` & `dfimagetools-20230526/dfimagetools/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools/windows_registry.py` & `dfimagetools-20230526/dfimagetools/windows_registry.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools.egg-info/PKG-INFO` & `dfimagetools-20230526/dfimagetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfimagetools
-Version: 20230410
+Version: 20230526
 Summary: Storage media image tools
 Home-page: https://github.com/log2timeline/dfimagetools
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `dfimagetools-20230410/dfimagetools.egg-info/SOURCES.txt` & `dfimagetools-20230526/dfimagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/dfimagetools.egg-info/requires.txt` & `dfimagetools-20230526/dfimagetools.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 pip>=7.0.0
 PyYAML>=3.10
 artifacts>=20220219
 cffi>=1.9.1
 cryptography>=2.0.2
-dfdatetime>=20220816
+dfdatetime>=20221112
 dfvfs>=20220831
 dfwinreg>=20211207
 dtfabric>=20220219
 libbde-python>=20220121
 libcreg-python>=20200725
 libewf-python>=20131210
 libfsapfs-python>=20220709
 libfsext-python>=20220829
-libfsfat-python>=20220816
+libfsfat-python>=20220925
 libfshfs-python>=20220831
 libfsntfs-python>=20211229
 libfsxfs-python>=20220829
 libfvde-python>=20220121
 libfwnt-python>=20210717
 libluksde-python>=20220121
 libmodi-python>=20210405
@@ -24,14 +24,15 @@
 libqcow-python>=20201213
 libregf-python>=20201002
 libsigscan-python>=20191221
 libsmdev-python>=20140529
 libsmraw-python>=20140612
 libvhdi-python>=20201014
 libvmdk-python>=20140421
+libvsapm-python>=20230506
 libvsgpt-python>=20211115
 libvshadow-python>=20160109
 libvslvm-python>=20160109
 pytsk3>=20210419
 
 [:platform_system != "Windows"]
 pyxattr>=0.7.2
```

### Comparing `dfimagetools-20230410/docs/conf.py` & `dfimagetools-20230526/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/docs/index.rst` & `dfimagetools-20230526/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/docs/sources/Bodyfile-format.md` & `dfimagetools-20230526/docs/sources/Bodyfile-format.md`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/docs/sources/api/dfimagetools.rst` & `dfimagetools-20230526/docs/sources/api/dfimagetools.rst`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/docs/sources/user/Installation-instructions.md` & `dfimagetools-20230526/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/requirements.txt` & `dfimagetools-20230526/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 pip >= 7.0.0
 PyYAML >= 3.10
 artifacts >= 20220219
 cffi >= 1.9.1
 cryptography >= 2.0.2
-dfdatetime >= 20220816
+dfdatetime >= 20221112
 dfvfs >= 20220831
 dfwinreg >= 20211207
 dtfabric >= 20220219
 libbde-python >= 20220121
 libcreg-python >= 20200725
 libewf-python >= 20131210
 libfsapfs-python >= 20220709
 libfsext-python >= 20220829
-libfsfat-python >= 20220816
+libfsfat-python >= 20220925
 libfshfs-python >= 20220831
 libfsntfs-python >= 20211229
 libfsxfs-python >= 20220829
 libfvde-python >= 20220121
 libfwnt-python >= 20210717
 libluksde-python >= 20220121
 libmodi-python >= 20210405
@@ -24,12 +24,13 @@
 libqcow-python >= 20201213
 libregf-python >= 20201002
 libsigscan-python >= 20191221
 libsmdev-python >= 20140529
 libsmraw-python >= 20140612
 libvhdi-python >= 20201014
 libvmdk-python >= 20140421
+libvsapm-python >= 20230506
 libvsgpt-python >= 20211115
 libvshadow-python >= 20160109
 libvslvm-python >= 20160109
 pytsk3 >= 20210419
 pyxattr >= 0.7.2 ; platform_system != "Windows"
```

### Comparing `dfimagetools-20230410/run_tests.py` & `dfimagetools-20230526/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/setup.cfg` & `dfimagetools-20230526/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	README
 build_requires = python3-setuptools
 requires = libbde-python3 >= 20220121
 	libcreg-python3 >= 20200725
 	libewf-python3 >= 20131210
 	libfsapfs-python3 >= 20220709
 	libfsext-python3 >= 20220829
-	libfsfat-python3 >= 20220816
+	libfsfat-python3 >= 20220925
 	libfshfs-python3 >= 20220831
 	libfsntfs-python3 >= 20211229
 	libfsxfs-python3 >= 20220829
 	libfvde-python3 >= 20220121
 	libfwnt-python3 >= 20210717
 	libluksde-python3 >= 20220121
 	libmodi-python3 >= 20210405
@@ -34,21 +34,22 @@
 	libqcow-python3 >= 20201213
 	libregf-python3 >= 20201002
 	libsigscan-python3 >= 20191221
 	libsmdev-python3 >= 20140529
 	libsmraw-python3 >= 20140612
 	libvhdi-python3 >= 20201014
 	libvmdk-python3 >= 20140421
+	libvsapm-python3 >= 20230506
 	libvsgpt-python3 >= 20211115
 	libvshadow-python3 >= 20160109
 	libvslvm-python3 >= 20160109
 	python3-artifacts >= 20220219
 	python3-cffi >= 1.9.1
 	python3-cryptography >= 2.0.2
-	python3-dfdatetime >= 20220816
+	python3-dfdatetime >= 20221112
 	python3-dfvfs >= 20220831
 	python3-dfwinreg >= 20211207
 	python3-dtfabric >= 20220219
 	python3-idna >= 2.5
 	python3-pytsk3 >= 20210419
 	python3-pyxattr >= 0.7.2
 	python3-pyyaml >= 3.10
```

### Comparing `dfimagetools-20230410/setup.py` & `dfimagetools-20230526/setup.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/artifact_filters.py` & `dfimagetools-20230526/tests/artifact_filters.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/bodyfile.py` & `dfimagetools-20230526/tests/bodyfile.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/environment_variables.py` & `dfimagetools-20230526/tests/environment_variables.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/file_entry_lister.py` & `dfimagetools-20230526/tests/file_entry_lister.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/path_resover.py` & `dfimagetools-20230526/tests/path_resover.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/source_analyzer.py` & `dfimagetools-20230526/tests/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tests/test_lib.py` & `dfimagetools-20230526/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tools/extract_data_streams.py` & `dfimagetools-20230526/tools/extract_data_streams.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tools/list_file_entries.py` & `dfimagetools-20230526/tools/list_file_entries.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tools/map_extents.py` & `dfimagetools-20230526/tools/map_extents.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tools/recursive_hasher.py` & `dfimagetools-20230526/tools/recursive_hasher.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tools/source_analyzer.py` & `dfimagetools-20230526/tools/source_analyzer.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/tox.ini` & `dfimagetools-20230526/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -14,31 +14,15 @@
     -rrequirements.txt
     -rtest_requirements.txt
     coverage: coverage
 commands =
     py3{7,8,9,10,11}: ./run_tests.py
     coverage: coverage erase
     coverage: coverage run --source=dfimagetools --omit="*_test*,*__init__*,*test_lib*" run_tests.py
-
-[testenv:codecov]
-skip_install = True
-passenv =
-    CFLAGS
-    CPPFLAGS
-    GITHUB_ACTION
-    GITHUB_HEAD_REF
-    GITHUB_REF
-    GITHUB_REPOSITORY
-    GITHUB_RUN_ID
-    GITHUB_SHA
-    LDFLAGS
-deps =
-    codecov < 2.1.10
-commands =
-    codecov
+    coverage: coverage xml
 
 [testenv:docs]
 usedevelop = True
 deps =
     -rdocs/requirements.txt
 commands =
     sphinx-build -b html -d build/doctrees docs dist/docs
@@ -52,15 +36,15 @@
     CPPFLAGS
     LDFLAGS
 setenv =
     PYTHONPATH = {toxinidir}
 deps =
     -rrequirements.txt
     -rtest_requirements.txt
-    pylint >= 2.14.0, < 2.15.0
+    pylint >= 2.17.0, < 2.18.0
     yamllint >= 1.26.0
 commands =
     pylint --version
     yamllint -v
     # Ignore setup.py for now due to:
     # setup.py:15:0: E0001: Cannot import 'distutils.command.bdist_msi' due to
     # syntax error 'expected an indented block (<unknown>, line 347)' (syntax-error)
```

### Comparing `dfimagetools-20230410/utils/dependencies.py` & `dfimagetools-20230526/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfimagetools-20230410/utils/update_release.sh` & `dfimagetools-20230526/utils/update_release.sh`

 * *Files identical despite different names*

