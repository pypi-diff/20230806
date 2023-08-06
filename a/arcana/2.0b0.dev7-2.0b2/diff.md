# Comparing `tmp/arcana-2.0b0.dev7.tar.gz` & `tmp/arcana-2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcana-2.0b0.dev7.tar", last modified: Mon Aug 22 07:43:27 2022, max compression
+gzip compressed data, was "arcana-2.0b2.tar", last modified: Tue Dec 20 07:01:11 2022, max compression
```

## Comparing `arcana-2.0b0.dev7.tar` & `arcana-2.0b2.tar`

### file list

```diff
@@ -1,111 +1,77 @@
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.763745 arcana-2.0b0.dev7/
--rw-r--r--   0 tclose     (501) staff       (20)    16577 2021-10-07 03:50:02.000000 arcana-2.0b0.dev7/LICENSE
--rw-r--r--   0 tclose     (501) staff       (20)      134 2022-03-28 05:52:30.000000 arcana-2.0b0.dev7/MANIFEST.in
--rw-r--r--   0 tclose     (501) staff       (20)     4378 2022-08-22 07:43:27.764206 arcana-2.0b0.dev7/PKG-INFO
--rw-r--r--   0 tclose     (501) staff       (20)     2879 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/README.rst
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.765658 arcana-2.0b0.dev7/arcana/
--rw-r--r--   0 tclose     (501) staff       (20)     1085 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/__about__.py
--rw-r--r--   0 tclose     (501) staff       (20)      976 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)      502 2022-08-22 07:43:27.765771 arcana-2.0b0.dev7/arcana/_version.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.719278 arcana-2.0b0.dev7/arcana/cli/
--rw-r--r--   0 tclose     (501) staff       (20)      165 2022-05-13 06:55:43.000000 arcana-2.0b0.dev7/arcana/cli/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     4878 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/cli/apply.py
--rw-r--r--   0 tclose     (501) staff       (20)     8809 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/cli/dataset.py
--rw-r--r--   0 tclose     (501) staff       (20)    26903 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/cli/deploy.py
--rw-r--r--   0 tclose     (501) staff       (20)     3510 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/cli/derive.py
--rw-r--r--   0 tclose     (501) staff       (20)     3495 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/cli/store.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.722744 arcana-2.0b0.dev7/arcana/core/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-03-28 05:52:30.000000 arcana-2.0b0.dev7/arcana/core/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    32920 2022-08-22 06:22:22.000000 arcana-2.0b0.dev7/arcana/core/analysis.py
--rw-r--r--   0 tclose     (501) staff       (20)     3781 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/core/cli.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.736104 arcana-2.0b0.dev7/arcana/core/data/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-13 06:55:43.000000 arcana-2.0b0.dev7/arcana/core/data/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     9518 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/data/column.py
--rw-r--r--   0 tclose     (501) staff       (20)    37499 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/data/format.py
--rw-r--r--   0 tclose     (501) staff       (20)    11546 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/data/row.py
--rw-r--r--   0 tclose     (501) staff       (20)    32373 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/data/set.py
--rw-r--r--   0 tclose     (501) staff       (20)     5694 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/core/data/space.py
--rw-r--r--   0 tclose     (501) staff       (20)    13521 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/data/store.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.737741 arcana-2.0b0.dev7/arcana/core/deploy/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-18 01:16:26.000000 arcana-2.0b0.dev7/arcana/core/deploy/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    17553 2022-08-22 07:39:49.000000 arcana-2.0b0.dev7/arcana/core/deploy/build.py
--rw-r--r--   0 tclose     (501) staff       (20)     5464 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/core/deploy/docs.py
--rw-r--r--   0 tclose     (501) staff       (20)     9898 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/core/deploy/utils.py
--rw-r--r--   0 tclose     (501) staff       (20)     4544 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/enum.py
--rw-r--r--   0 tclose     (501) staff       (20)     7137 2022-08-22 06:22:22.000000 arcana-2.0b0.dev7/arcana/core/mark.py
--rw-r--r--   0 tclose     (501) staff       (20)    25403 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/pipeline.py
--rw-r--r--   0 tclose     (501) staff       (20)    30846 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/core/utils.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.738340 arcana-2.0b0.dev7/arcana/data/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-03-28 05:52:30.000000 arcana-2.0b0.dev7/arcana/data/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.740110 arcana-2.0b0.dev7/arcana/data/formats/
--rw-r--r--   0 tclose     (501) staff       (20)       46 2022-05-13 06:55:43.000000 arcana-2.0b0.dev7/arcana/data/formats/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     2863 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/formats/common.py
--rw-r--r--   0 tclose     (501) staff       (20)    16501 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/formats/medimage.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.742079 arcana-2.0b0.dev7/arcana/data/spaces/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-13 06:55:43.000000 arcana-2.0b0.dev7/arcana/data/spaces/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)      272 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/data/spaces/common.py
--rw-r--r--   0 tclose     (501) staff       (20)     1246 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/data/spaces/medimage.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.742622 arcana-2.0b0.dev7/arcana/data/stores/
--rw-r--r--   0 tclose     (501) staff       (20)        1 2022-05-13 06:55:43.000000 arcana-2.0b0.dev7/arcana/data/stores/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.744131 arcana-2.0b0.dev7/arcana/data/stores/bids/
--rw-r--r--   0 tclose     (501) staff       (20)       61 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/data/stores/bids/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    10043 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/stores/bids/dataset.py
--rw-r--r--   0 tclose     (501) staff       (20)     7433 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/stores/bids/structure.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.745143 arcana-2.0b0.dev7/arcana/data/stores/common/
--rw-r--r--   0 tclose     (501) staff       (20)       36 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/data/stores/common/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    12439 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/stores/common/file_system.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.745599 arcana-2.0b0.dev7/arcana/data/stores/medimage/
--rw-r--r--   0 tclose     (501) staff       (20)       58 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/data/stores/medimage/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.747645 arcana-2.0b0.dev7/arcana/data/stores/medimage/xnat/
--rw-r--r--   0 tclose     (501) staff       (20)       48 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/data/stores/medimage/xnat/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    28419 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/stores/medimage/xnat/api.py
--rw-r--r--   0 tclose     (501) staff       (20)     6451 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/data/stores/medimage/xnat/cs.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.748077 arcana-2.0b0.dev7/arcana/deploy/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-18 01:16:26.000000 arcana-2.0b0.dev7/arcana/deploy/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.748980 arcana-2.0b0.dev7/arcana/deploy/medimage/
--rw-r--r--   0 tclose     (501) staff       (20)       64 2022-05-18 01:16:26.000000 arcana-2.0b0.dev7/arcana/deploy/medimage/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    22885 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/deploy/medimage/xnat.py
--rw-r--r--   0 tclose     (501) staff       (20)     4254 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/exceptions.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.749847 arcana-2.0b0.dev7/arcana/tasks/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-03-28 05:52:30.000000 arcana-2.0b0.dev7/arcana/tasks/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.750679 arcana-2.0b0.dev7/arcana/tasks/bids/
--rw-r--r--   0 tclose     (501) staff       (20)       26 2022-05-18 01:16:26.000000 arcana-2.0b0.dev7/arcana/tasks/bids/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)    15156 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/tasks/bids/app.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.752130 arcana-2.0b0.dev7/arcana/tasks/common/
--rw-r--r--   0 tclose     (501) staff       (20)       70 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/tasks/common/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     5208 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/tasks/common/archive.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.752830 arcana-2.0b0.dev7/arcana/tasks/common/tests/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/tasks/common/tests/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     2258 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/tasks/common/tests/test_archive.py
--rw-r--r--   0 tclose     (501) staff       (20)     1054 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/tasks/common/utils.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.755463 arcana-2.0b0.dev7/arcana/test/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/test/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     4731 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/test/datasets.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.758000 arcana-2.0b0.dev7/arcana/test/fixtures/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-13 06:55:44.000000 arcana-2.0b0.dev7/arcana/test/fixtures/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     4754 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/bids.py
--rw-r--r--   0 tclose     (501) staff       (20)     7553 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/common.py
--rw-r--r--   0 tclose     (501) staff       (20)      913 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/core.py
--rw-r--r--   0 tclose     (501) staff       (20)     3773 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/docs.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.759417 arcana-2.0b0.dev7/arcana/test/fixtures/medimage/
--rw-r--r--   0 tclose     (501) staff       (20)      375 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/medimage/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     1074 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/fixtures/medimage/dicom.py
--rw-r--r--   0 tclose     (501) staff       (20)     7745 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/test/fixtures/medimage/xnat.py
--rw-r--r--   0 tclose     (501) staff       (20)     1328 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/formats.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.760685 arcana-2.0b0.dev7/arcana/test/stores/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-18 01:16:32.000000 arcana-2.0b0.dev7/arcana/test/stores/__init__.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.762493 arcana-2.0b0.dev7/arcana/test/stores/medimage/
--rw-r--r--   0 tclose     (501) staff       (20)        0 2022-05-18 01:16:32.000000 arcana-2.0b0.dev7/arcana/test/stores/medimage/__init__.py
--rw-r--r--   0 tclose     (501) staff       (20)     8991 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/test/stores/medimage/xnat.py
--rw-r--r--   0 tclose     (501) staff       (20)     5415 2022-08-18 23:39:33.000000 arcana-2.0b0.dev7/arcana/test/tasks.py
--rw-r--r--   0 tclose     (501) staff       (20)      299 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/arcana/test/utils.py
-drwxr-xr-x   0 tclose     (501) staff       (20)        0 2022-08-22 07:43:27.714969 arcana-2.0b0.dev7/arcana.egg-info/
--rw-r--r--   0 tclose     (501) staff       (20)     4378 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/PKG-INFO
--rw-r--r--   0 tclose     (501) staff       (20)     2325 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/SOURCES.txt
--rw-r--r--   0 tclose     (501) staff       (20)        1 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/dependency_links.txt
--rw-r--r--   0 tclose     (501) staff       (20)       96 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/entry_points.txt
--rw-r--r--   0 tclose     (501) staff       (20)      386 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/requires.txt
--rw-r--r--   0 tclose     (501) staff       (20)        7 2022-08-22 07:43:27.000000 arcana-2.0b0.dev7/arcana.egg-info/top_level.txt
--rw-r--r--   0 tclose     (501) staff       (20)      496 2022-08-22 07:43:27.765226 arcana-2.0b0.dev7/setup.cfg
--rw-r--r--   0 tclose     (501) staff       (20)     1829 2022-08-04 03:59:21.000000 arcana-2.0b0.dev7/setup.py
--rw-r--r--   0 tclose     (501) staff       (20)    80044 2022-08-02 21:24:53.000000 arcana-2.0b0.dev7/versioneer.py
+-rw-r--r--   0        0        0    16577 2022-12-20 07:00:29.697791 arcana-2.0b2/LICENSE
+-rw-r--r--   0        0        0     2905 2022-12-20 07:00:29.697791 arcana-2.0b2/README.rst
+-rw-r--r--   0        0        0     1114 2022-12-20 07:00:29.697791 arcana-2.0b2/arcana/__init__.py
+-rw-r--r--   0        0        0      157 2022-12-20 07:01:11.615013 arcana-2.0b2/arcana/_version.py
+-rw-r--r--   0        0        0      257 2022-12-20 07:00:29.697791 arcana-2.0b2/arcana/common/__init__.py
+-rw-r--r--   0        0        0       60 2022-12-20 07:00:29.697791 arcana-2.0b2/arcana/common/analysis/__init__.py
+-rw-r--r--   0        0        0       99 2022-12-20 07:00:29.697791 arcana-2.0b2/arcana/common/analysis/tasks/__init__.py
+-rw-r--r--   0        0        0     5213 2022-12-20 07:00:29.697791 arcana-2.0b2/arcana/common/analysis/tasks/archive.py
+-rw-r--r--   0        0        0    10849 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/analysis/tasks/shell.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/analysis/tasks/tests/__init__.py
+-rw-r--r--   0        0        0     2288 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/analysis/tasks/tests/test_archive.py
+-rw-r--r--   0        0        0     1054 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/analysis/tasks/tests/test_shell.py
+-rw-r--r--   0        0        0     1057 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/analysis/tasks/utils.py
+-rw-r--r--   0        0        0      348 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/data/__init__.py
+-rw-r--r--   0        0        0    13099 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/data/file_system.py
+-rw-r--r--   0        0        0     2909 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/data/formats.py
+-rw-r--r--   0        0        0      272 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/data/spaces.py
+-rw-r--r--   0        0        0     3282 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/common/data/tests/test_file_system.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/__init__.py
+-rw-r--r--   0        0        0    18286 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/make.py
+-rw-r--r--   0        0        0     5840 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/mark.py
+-rw-r--r--   0        0        0    28005 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/pipeline.py
+-rw-r--r--   0        0        0     4903 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/salience.py
+-rw-r--r--   0        0        0    19482 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/spec.py
+-rw-r--r--   0        0        0    51640 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/tests/test_analysis.py
+-rw-r--r--   0        0        0     2469 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/analysis/tests/test_pipeline.py
+-rw-r--r--   0        0        0      160 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/__init__.py
+-rw-r--r--   0        0        0     4970 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/apply.py
+-rw-r--r--   0        0        0      602 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/base.py
+-rw-r--r--   0        0        0     8839 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/dataset.py
+-rw-r--r--   0        0        0    20258 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/deploy.py
+-rw-r--r--   0        0        0     3479 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/derive.py
+-rw-r--r--   0        0        0     3511 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/store.py
+-rw-r--r--   0        0        0     1699 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/tests/test_cli_apply.py
+-rw-r--r--   0        0        0     4163 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/tests/test_cli_dataset.py
+-rw-r--r--   0        0        0    12665 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/tests/test_cli_deploy.py
+-rw-r--r--   0        0        0     1942 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/tests/test_cli_derive.py
+-rw-r--r--   0        0        0     4436 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/__init__.py
+-rw-r--r--   0        0        0     9432 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/column.py
+-rw-r--r--   0        0        0    11592 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/row.py
+-rw-r--r--   0        0        0    35502 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/set.py
+-rw-r--r--   0        0        0     6053 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/space.py
+-rw-r--r--   0        0        0    14103 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/store.py
+-rw-r--r--   0        0        0      737 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/tests/test_data_column.py
+-rw-r--r--   0        0        0      124 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/tests/test_data_store.py
+-rw-r--r--   0        0        0     1246 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/tests/test_dataset.py
+-rw-r--r--   0        0        0      105 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/type/__init__.py
+-rw-r--r--   0        0        0    25574 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/type/base.py
+-rw-r--r--   0        0        0     2980 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/type/directory.py
+-rw-r--r--   0        0        0      418 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/type/field.py
+-rw-r--r--   0        0        0    10470 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/data/type/file.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/__init__.py
+-rw-r--r--   0        0        0       35 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/command/__init__.py
+-rw-r--r--   0        0        0    18669 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/command/base.py
+-rw-r--r--   0        0        0     7905 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/command/components.py
+-rw-r--r--   0        0        0     7074 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/command/entrypoint_opts.py
+-rw-r--r--   0        0        0     9511 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/command/tests/test_deploy_command.py
+-rw-r--r--   0        0        0       88 2022-12-20 07:00:29.701791 arcana-2.0b2/arcana/core/deploy/image/__init__.py
+-rw-r--r--   0        0        0    19408 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/deploy/image/app.py
+-rw-r--r--   0        0        0    18555 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/deploy/image/base.py
+-rw-r--r--   0        0        0    11519 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/deploy/image/components.py
+-rw-r--r--   0        0        0     1178 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/deploy/image/metapackage.py
+-rw-r--r--   0        0        0     6841 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/deploy/tests/test_licenses.py
+-rw-r--r--   0        0        0        0 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/__init__.py
+-rw-r--r--   0        0        0    15764 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/misc.py
+-rw-r--r--   0        0        0     4902 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/packaging.py
+-rw-r--r--   0        0        0    19384 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/serialize.py
+-rw-r--r--   0        0        0      299 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/testing/__init__.py
+-rw-r--r--   0        0        0    11225 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/testing/data.py
+-rw-r--r--   0        0        0     6652 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/testing/tasks.py
+-rw-r--r--   0        0        0     1095 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/core/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     4316 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/exceptions.py
+-rw-r--r--   0        0        0      224 2022-12-20 07:00:29.705791 arcana-2.0b2/arcana/mark.py
+-rw-r--r--   0        0        0     2292 2022-12-20 07:00:29.805792 arcana-2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5173 1970-01-01 00:00:00.000000 arcana-2.0b2/PKG-INFO
```

### Comparing `arcana-2.0b0.dev7/LICENSE` & `arcana-2.0b2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,8 @@
     No term or condition of this Public License will be waived and no failure to comply consented to unless expressly agreed to by the Licensor.
     Nothing in this Public License constitutes or may be interpreted as a limitation upon, or waiver of, any privileges and immunities that apply to the Licensor or You, including from the legal processes of any jurisdiction or authority.
 
 Creative Commons is not a party to its public licenses. Notwithstanding, Creative Commons may elect to apply one of its public licenses to material it publishes and in those instances will be considered the “Licensor.” The text of the Creative Commons public licenses is dedicated to the public domain under the CC0 Public Domain Dedication. Except for the limited purpose of indicating that material is shared under a Creative Commons public license or as otherwise permitted by the Creative Commons policies published at creativecommons.org/policies, Creative Commons does not authorize the use of the trademark “Creative Commons” or any other trademark or logo of Creative Commons without its prior written consent including, without limitation, in connection with any unauthorized modifications to any of its public licenses or any other arrangements, understandings, or agreements concerning use of licensed material. For the avoidance of doubt, this paragraph does not form part of the public licenses.
 
 Creative Commons may be contacted at creativecommons.org.
 
-Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations. 
+Additional languages available: العربية, čeština, Deutsch, Ελληνικά, Español, euskara, suomeksi, français, hrvatski, Bahasa Indonesia, italiano, 日本語, 한국어, Lietuvių, latviski, te reo Māori, Nederlands, norsk, polski, português, română, русский, Slovenščina, svenska, Türkçe, українська, 中文, 華語. Please read the FAQ for more information about official translations.
```

### Comparing `arcana-2.0b0.dev7/README.rst` & `arcana-2.0b2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .. image:: https://readthedocs.org/projects/arcana/badge/?version=latest
   :target: http://arcana.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 
 
 Abstraction of Repository-Centric ANAlysis (Arcana_) is Python framework
 for "repository-centric" analyses of study groups (e.g. NeuroImaging
-studies) built on Pydra_.
+studies) built on the Pydra_ dataflow engine.
 
 Arcana_ interacts closely with a data store (e.g. XNAT repository or BIDS dataset),
 storing intermediate outputs, along with the parameters used to derive them,
 for reuse by subsequent analyses.
 
 Analysis workflows are constructed and executed using the Pydra_
 package, and can either be run locally or submitted to HPC
@@ -36,15 +36,15 @@
 Detailed documentation on Arcana can be found at https://arcana.readthedocs.io
 
 Quick Installation
 ------------------
 
 Arcana can be installed for Python 3 using *pip*::
 
-    $ pip3 install arcana
+    $ pip3 install arcana>=2.0b
 
 .. _Arcana: http://arcana.readthedocs.io
 .. _Pydra: http://pydra.readthedocs.io
 .. _XNAT: http://xnat.org
 .. _BIDS: http://bids.neuroimaging.io/
 .. _`Environment Modules`: http://modules.sourceforge.net
```

### Comparing `arcana-2.0b0.dev7/arcana/__init__.py` & `arcana-2.0b2/arcana/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,17 +13,22 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from ._version import get_versions
+PACKAGE_NAME = "arcana"
+CODE_URL = f"https://github.com/australian-imaging-service/{PACKAGE_NAME}"
 
-__version__ = get_versions()["version"]
-del get_versions
-from .__about__ import __authors__
-from .core.data.set import Dataset
-from .core.data.store import DataStore
+__authors__ = [("Thomas G. Close", "tom.g.close@gmail.com")]
+
+from ._version import __version__
+
+from pydra import set_input_validator
+
+set_input_validator(True)
+# from .core.data.set import Dataset
+# from .core.data.store import DataStore
 
 # Should be set explicitly in all FSL interfaces, but this squashes the warning
 # os.environ['FSLOUTPUTTYPE'] = 'NIFTI_GZ'
```

### Comparing `arcana-2.0b0.dev7/arcana/cli/apply.py` & `arcana-2.0b2/arcana/core/cli/apply.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-from inspect import Arguments
 import click
+import typing as ty
 from arcana.core.data.set import Dataset
-from arcana.core.cli import cli
-from arcana.core.utils import resolve_class, parse_value
+from pydra.engine.core import TaskBase
+from arcana.core.utils.serialize import ClassResolver, parse_value
+from arcana.core.data.type.base import DataType
+from .base import cli
 
 
 @cli.group()
 def apply():
     pass
 
 
 @apply.command(
     name="pipeline",
     help="""Apply a Pydra workflow to a dataset as a pipeline between
 two columns
 
-DATASET_ID_STR string containing the nickname of the data store, the ID of the dataset
+DATASET_LOCATOR string containing the nickname of the data store, the ID of the dataset
 (e.g. XNAT project ID or file-system directory) and the dataset's name in the
-format <STORE-NICKNAME>//<DATASET-ID>:<DATASET-NAME>
+format <store-nickname>//<dataset-id>[@<dataset-name>]
 
 PIPELINE_NAME is the name of the pipeline
 
 WORKFLOW_LOCATION is the location to a Pydra workflow on the Python system path,
 <MODULE>:<WORKFLOW>""",
 )
-@click.argument("dataset_id_str")
+@click.argument("dataset_locator")
 @click.argument("pipeline_name")
 @click.argument("workflow_location")
 @click.option(
     "--input",
     "-i",
     nargs=3,
     default=(),
-    metavar="<col-name> <pydra-field> <required-format>",
+    metavar="<col-name> <pydra-field> <required-datatype>",
     multiple=True,
     type=str,
     help=(
         "the link between a column and an input of the workflow. "
         "The required format is the location (<module-path>:<class>) of the format "
         "expected by the workflow"
     ),
 )
 @click.option(
     "--output",
     "-o",
     nargs=3,
     default=(),
-    metavar="<col-name> <pydra-field> <produced-format>",
+    metavar="<col-name> <pydra-field> <produced-datatype>",
     multiple=True,
     type=str,
     help=(
         "the link between an output of the workflow and a sink column. "
-        "The produced format is the location (<module-path>:<class>) of the format "
+        "The produced datatype is the location (<module-path>:<class>) of the datatype "
         "produced by the workflow"
     ),
 )
 @click.option(
     "--parameter",
     "-p",
     nargs=2,
@@ -66,83 +68,83 @@
     help=("a fixed parameter of the workflow to set when applying it"),
 )
 @click.option(
     "--source",
     "-s",
     nargs=3,
     default=(),
-    metavar="<col-name> <pydra-field> <required-format>",
+    metavar="<col-name> <pydra-field> <required-datatype>",
     multiple=True,
     type=str,
     help=(
         "add a source to the dataset and link it to an input of the workflow "
         "in a single step. The source column must be able to be specified by its "
-        "path alone and be already in the format required by the workflow"
+        "path alone and be already in the datatype required by the workflow"
     ),
 )
 @click.option(
     "--sink",
     "-k",
     nargs=3,
     default=(),
-    metavar="<col-name> <pydra-field> <produced-format>",
+    metavar="<col-name> <pydra-field> <produced-datatype>",
     multiple=True,
     type=str,
     help=(
         "add a sink to the dataset and link it to an output of the workflow "
-        "in a single step. The sink column be in the same format as produced "
+        "in a single step. The sink column be in the same datatype as produced "
         "by the workflow"
     ),
 )
 @click.option(
-    "--row_frequency",
+    "--row-frequency",
     "-f",
     default=None,
     type=str,
     help=(
-        "the row_frequency of the rows the pipeline will be executed over, i.e. "
+        "the row-frequency of the rows the pipeline will be executed over, i.e. "
         "will it be run once per-session, per-subject or per whole dataset, "
-        "by default the highest row_frequency rows (e.g. per-session)"
+        "by default the highest row-frequency rows (e.g. per-session)"
     ),
 )
 @click.option(
     "--overwrite/--no-overwrite",
     default=False,
     help=("whether to overwrite previous pipelines"),
 )
 def apply_pipeline(
-    dataset_id_str,
+    dataset_locator,
     pipeline_name,
     workflow_location,
     input,
     output,
     parameter,
     source,
     sink,
     row_frequency,
     overwrite,
 ):
 
-    dataset = Dataset.load(dataset_id_str)
-    workflow = resolve_class(workflow_location)(
-        name="workflow", **{n: parse_value(v) for n, v in parameter}
-    )
+    dataset = Dataset.load(dataset_locator)
+    workflow = ClassResolver(TaskBase, alternative_types=[ty.Callable])(
+        workflow_location
+    )(name="workflow", **{n: parse_value(v) for n, v in parameter})
 
     inputs = parse_col_option(input)
     outputs = parse_col_option(output)
     sources = parse_col_option(source)
     sinks = parse_col_option(sink)
 
-    for col_name, pydra_field, format in sources:
-        dataset.add_source(col_name, format)
-        inputs.append((col_name, pydra_field, format))
-
-    for col_name, pydra_field, format in sinks:
-        dataset.add_sink(col_name, format)
-        outputs.append((col_name, pydra_field, format))
+    for col_name, field, datatype in sources:
+        dataset.add_source(col_name, datatype)
+        inputs.append((col_name, field, datatype))
+
+    for col_name, field, datatype in sinks:
+        dataset.add_sink(col_name, datatype)
+        outputs.append((col_name, field, datatype))
 
     dataset.apply_pipeline(
         pipeline_name,
         workflow,
         inputs,
         outputs,
         row_frequency=row_frequency,
@@ -178,10 +180,8 @@
     ),
 )
 def apply_bids_app():
     raise NotImplementedError
 
 
 def parse_col_option(option):
-    return [
-        (c, p, resolve_class(f, prefixes=["arcana.data.formats"])) for c, p, f in option
-    ]
+    return [(c, p, ClassResolver(DataType)(f)) for c, p, f in option]
```

### Comparing `arcana-2.0b0.dev7/arcana/cli/dataset.py` & `arcana-2.0b2/arcana/core/cli/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from __future__ import annotations
 import click
-from arcana.core.cli import cli
+from .base import cli
 from arcana.core.data.set import Dataset
 from arcana.core.data.store import DataStore
-from arcana.core.utils import resolve_class
-
-
-XNAT_CACHE_DIR = "xnat-cache"
+from arcana.core.data.space import DataSpace
+from arcana.core.data.type.base import DataType
+from arcana.core.utils.serialize import ClassResolver
 
 
 @cli.group()
 def dataset():
     pass
 
 
@@ -18,15 +18,15 @@
     help=(
         """Define the tree structure and IDs to include in a
 dataset. Where possible, the definition file is saved inside the dataset for
 use by multiple users, if not possible it is stored in the ~/.arcana directory.
 
 ID_STR string containing the nick-name of the store, the ID of the dataset
 (e.g. XNAT project ID or file-system directory) and the dataset's name in the
-format <NICKNAME>//DATASET_ID:DATASET_NAME
+format <store-nickname>//<dataset-id>[@<dataset-name>]
 
 HIERARCHY the data frequencies that are present in the data tree. For some
 store types this is fixed (e.g. XNAT-> subject > session) but for more flexible
 (e.g. FileSystem), which dimension each layer of sub-directories corresponds to
 can be arbitrarily specified. dimensions"""
     ),
 )
@@ -46,30 +46,30 @@
     nargs=2,
     default=(),
     metavar="<freq-id>",
     multiple=True,
     type=str,
     help=(
         "The rows to include in the dataset. First value is the "
-        "row_frequency of the ID (e.g. 'group', 'subject', 'session') "
+        "row-frequency of the ID (e.g. 'group', 'subject', 'session') "
         "followed by the IDs to be included in the dataset. "
         "If the second arg contains '/' then it is interpreted as "
         "the path to a text file containing a list of IDs"
     ),
 )
 @click.option(
     "--exclude",
     nargs=2,
     default=(),
     metavar="<freq-id>",
     multiple=True,
     type=str,
     help=(
         "The rows to exclude from the dataset. First value is the "
-        "row_frequency of the ID (e.g. 'group', 'subject', 'session') "
+        "row-frequency of the ID (e.g. 'group', 'subject', 'session') "
         "followed by the IDs to be included in the dataset. "
         "If the second arg contains '/' then it is interpreted as "
         "the path to a text file containing a list of IDs"
     ),
 )
 @click.option(
     "--space",
@@ -78,15 +78,15 @@
         "The enum that specifies the data dimensions of the dataset. "
         "Defaults to `Clinical`, which "
         "consists of the typical dataset>group>subject>session "
         "data tree used in medimage trials/studies"
     ),
 )
 @click.option(
-    "--id_inference",
+    "--id-inference",
     nargs=2,
     metavar="<source-regex>",
     multiple=True,
     help="""Specifies how IDs of row frequencies that not explicitly
 provided are inferred from the IDs that are. For example, given a set
 of subject IDs that are a combination of the ID of the group that they belong
 to + their member IDs (i.e. matched test/controls have same member ID), e.g.
@@ -94,29 +94,29 @@
 CONTROL01, CONTROL02, CONTROL03, ... and TEST01, TEST02, TEST03
 
 the group ID can be extracted by providing the ID to source it from
 (i.e. subject) and a regular expression (in Python regex syntax:
 https://docs.python.org/3/library/re.html) with a named
 groups corresponding to the inferred IDs
 
---id_inference subject '(?P<group>[A-Z]+)(?P<member>[0-9]+)'
+--id-inference subject '(?P<group>[A-Z]+)(?P<member>[0-9]+)'
 
 """,
 )
 def define(id_str, hierarchy, include, exclude, space, id_inference):
 
     store_name, id, name = Dataset.parse_id_str(id_str)
 
     if not hierarchy:
         hierarchy = None
 
     store = DataStore.load(store_name)
 
     if space:
-        space = resolve_class(space, ["arcana.data.spaces"])
+        space = ClassResolver(DataSpace)(space)
 
     dataset = store.new_dataset(
         id,
         hierarchy=hierarchy,
         space=space,
         id_inference=id_inference,
         include=include,
@@ -138,46 +138,43 @@
 @click.argument("dataset_path")
 @click.argument("new_name")
 def copy(dataset_path, new_name):
     dataset = Dataset.load(dataset_path)
     dataset.save(new_name)
 
 
-def optional_args(names, args):
-    kwargs = {}
+# def optional_args(names, args):
+#     kwargs = {}
 
 
 @dataset.command(
     name="add-source",
     help="""Adds a source column to a dataset. A source column
 selects comparable items along a dimension of the dataset to serve as
 an input to pipelines and analyses.
 
-Arguments
----------
-dataset_path
-    The path to the dataset including store and dataset name (where
-    applicable), e.g. central-xnat//MYXNATPROJECT:pass_t1w_qc
-name
-    The name the source will be referenced by
-format
-    The data type of the column. Can be a field (int|float|str|bool),
-    field array (list[int|float|str|bool]) or "file-group"
-    (file, file+header/side-cars or directory)
+DATASET_PATH: The path to the dataset including store and dataset name
+(where applicable), e.g. central-xnat//MYXNATPROJECT:pass_t1w_qc
+
+NAME: The name the source will be referenced by
+
+FORMAT: The data type of the column. Can be a field (int|float|str|bool),
+field array (list[int|float|str|bool]) or
+"file-group" (file, file+header/side-cars or directory)
 """,
 )
 @click.argument("dataset_path")
 @click.argument("name")
-@click.argument("format")
+@click.argument("datatype")
 @click.option(
-    "--row_frequency",
+    "--row-frequency",
     "-f",
     metavar="<dimension>",
     help=(
-        "The row_frequency that items appear in the dataset (e.g. per "
+        "The row-frequency that items appear in the dataset (e.g. per "
         "'session', 'subject', 'timepoint', 'group', 'dataset' for "
         "medimage:Clinical data dimensions"
     ),
     show_default="highest",
 )
 @click.option(
     "--path",
@@ -221,21 +218,21 @@
     help=(
         "Match on specific header value. This option is only valid for "
         "select formats that the implement the 'header_val()' method "
         "(e.g. medimage:dicom)."
     ),
 )
 def add_source(
-    dataset_path, name, format, row_frequency, path, order, quality, is_regex, header
+    dataset_path, name, datatype, row_frequency, path, order, quality, is_regex, header
 ):
     dataset = Dataset.load(dataset_path)
     dataset.add_source(
         name=name,
         path=path,
-        format=resolve_class(format, prefixes=["arcana.data.formats"]),
+        datatype=ClassResolver(DataType)(datatype),
         row_frequency=row_frequency,
         quality_threshold=quality,
         order=order,
         header_vals=dict(header),
         is_regex=is_regex,
     )
     dataset.save()
@@ -249,29 +246,29 @@
 Arguments
 ---------
 dataset_path
     The path to the dataset including store and dataset name (where
     applicable), e.g. central-xnat//MYXNATPROJECT:pass_t1w_qc
 name
     The name the source will be referenced by
-format
+datatype
     The data type of the column. Can be a field (int|float|str|bool),
     field array (list[int|float|str|bool]) or "file-group"
     (file, file+header/side-cars or directory)
 """,
 )
 @click.argument("dataset_path")
 @click.argument("name")
-@click.argument("format")
+@click.argument("datatype")
 @click.option(
-    "--row_frequency",
+    "--row-frequency",
     "-f",
     metavar="<dimension>",
     help=(
-        "The row_frequency that items appear in the dataset (e.g. per "
+        "The row-frequency that items appear in the dataset (e.g. per "
         "'session', 'subject', 'timepoint', 'group', 'dataset' for "
         "medimage:Clinical data dimensions"
     ),
     show_default="highest",
 )
 @click.option(
     "--path",
@@ -285,20 +282,20 @@
     "--salience",
     "-s",
     help=(
         "The salience of the column, i.e. whether it will show up on "
         "'arcana derive menu'"
     ),
 )
-def add_sink(dataset_path, name, format, row_frequency, path, salience):
+def add_sink(dataset_path, name, datatype, row_frequency, path, salience):
     dataset = Dataset.load(dataset_path)
     dataset.add_sink(
         name=name,
         path=path,
-        format=resolve_class(format, prefixes=["arcana.data.formats"]),
+        datatype=ClassResolver(DataType)(datatype),
         row_frequency=row_frequency,
         salience=salience,
     )
     dataset.save()
 
 
 @dataset.command(
```

### Comparing `arcana-2.0b0.dev7/arcana/cli/deploy.py` & `arcana-2.0b2/arcana/core/cli/deploy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,93 @@
 import logging
 import sys
 import shutil
-import json
 from pathlib import Path
+import json
+import typing as ty
+from traceback import format_exc
+import tempfile
 import click
 import docker
 import docker.errors
-import tempfile
-from collections import defaultdict
-import shlex
-from traceback import format_exc
-from arcana import __version__
-from arcana.core.cli import cli
-from arcana.core.pipeline import Input as PipelineInput, Output as PipelineOutput
-from arcana.core.utils import resolve_class, parse_value, show_workflow_errors
-from arcana.core.deploy.utils import (
-    load_yaml_spec,
-    walk_spec_paths,
-    DOCKER_HUB,
-    extract_file_from_docker_image,
-    compare_specs,
-)
-from arcana.core.deploy.docs import create_doc
-from arcana.core.deploy.build import SPEC_PATH as spec_path_in_docker
-from arcana.core.utils import package_from_module, pydra_asdict
-from arcana.core.data.row import DataRow
-from arcana.deploy.medimage.xnat import build_xnat_cs_image
+from pydra.engine.core import TaskBase
+from arcana.core.utils.serialize import (
+    package_from_module,
+    pydra_asdict,
+    ClassResolver,
+)
+from arcana.core.deploy.image import Metapackage, App
+
+# from arcana.deploy.xnat.image import XnatCSImage
+from arcana.exceptions import ArcanaBuildError
 from arcana.core.data.set import Dataset
 from arcana.core.data.store import DataStore
-from arcana.exceptions import ArcanaBuildError, ArcanaUsageError
-
+from arcana.core.utils.misc import extract_file_from_docker_image, DOCKER_HUB
+from .base import cli
+from arcana.core.deploy.command import entrypoint_opts
 
 logger = logging.getLogger("arcana")
 
 
 @cli.group()
 def deploy():
     pass
 
 
-@deploy.group()
-def xnat():
-    pass
-
-
-@xnat.command(
-    help="""Build a wrapper image specified in a module
+@deploy.command(
+    name="make-app",
+    help="""Construct and build a dockerfile/apptainer-file for containing a pipeline
 
-SPEC_PATH is the file system path to the specification to build, or directory
+SPEC_ROOT is the file system path to the specification to build, or directory
 containing multiple specifications
 
-DOCKER_ORG is the Docker organisation the images should belong to"""
+TARGET is the type of image to build, e.g. arcana.deploy.xnat:XnatCSImage
+the target should resolve to a class deriviing from arcana.core.deploy.App.
+If it is located under the `arcana.deploy`, then that prefix can be dropped, e.g.
+common:App
+""",
 )
-@click.argument("spec_path", type=click.Path(exists=True, path_type=Path))
-@click.argument("docker_org", type=str)
+@click.argument("spec_root", type=click.Path(exists=True, path_type=Path))
+@click.argument("target", type=str)
 @click.option(
     "--registry",
-    "docker_registry",
     default=DOCKER_HUB,
     help="The Docker registry to deploy the pipeline to",
 )
 @click.option(
-    "--build_dir",
+    "--build-dir",
     default=None,
-    type=click.Path(exists=True, path_type=Path),
+    type=click.Path(path_type=Path),
     help=(
         "Specify the directory to build the Docker image in. "
         "Defaults to `.build` in the directory containing the "
         "YAML specification"
     ),
 )
 @click.option(
+    "--release",
+    default=None,
+    nargs=2,
+    metavar="<release-name> <release-version>",
+    type=str,
+    help=("Name of the release for the package as a whole (i.e. for all pipelines)"),
+)
+@click.option(
+    "--tag-latest/--dont-tag-latest",
+    default=False,
+    type=bool,
+    help='whether to tag the release as the "latest" or not',
+)
+@click.option(
+    "--save-manifest",
+    default=None,
+    type=click.Path(writable=True),
+    help="File path at which to save the build manifest",
+)
+@click.option(
     "--logfile",
     default=None,
     type=click.Path(path_type=Path),
     help="Log output to file instead of stdout",
 )
 @click.option("--loglevel", default="info", help="The level to display logs at")
 @click.option(
@@ -83,15 +96,15 @@
     default=False,
     help=(
         "Use locally installed Python packages, instead of pulling "
         "them down from PyPI"
     ),
 )
 @click.option(
-    "--install_extras",
+    "--install-extras",
     type=str,
     default=None,
     help=(
         "Install extras to use when installing Arcana inside the "
         "container image. Typically only used in tests to provide "
         "'test' extra"
     ),
@@ -114,18 +127,34 @@
 @click.option(
     "--generate-only/--build",
     type=bool,
     default=False,
     help="Just create the build directory and dockerfile",
 )
 @click.option(
-    "--license-dir",
-    type=click.Path(exists=True, path_type=Path),
-    default=None,
-    help="Directory containing licences required to build the images",
+    "--license",
+    type=(str, click.Path(exists=True, path_type=Path)),
+    default=(),
+    nargs=2,
+    metavar="<license-name> <path-to-license-file>",
+    multiple=True,
+    help=(
+        "Licenses provided at build time to be stored in the image (instead of "
+        "downloaded at runtime)"
+    ),
+)
+@click.option(
+    "--license-to-download",
+    type=str,
+    default=(),
+    multiple=True,
+    help=(
+        "Specify licenses that are not provided at runtime and instead downloaded "
+        "from the data store at runtime in order to satisfy their conditions"
+    ),
 )
 @click.option(
     "--check-registry/--dont-check-registry",
     type=bool,
     default=False,
     help=(
         "Check the registry to see if an existing image with the "
@@ -135,265 +164,363 @@
 )
 @click.option(
     "--push/--dont-push",
     type=bool,
     default=False,
     help=("push built images to registry"),
 )
-def build(
-    spec_path,
-    docker_org,
-    docker_registry,
+@click.option(
+    "--clean-up/--dont-clean-up",
+    type=bool,
+    default=False,
+    help=(
+        "Remove built images after they are pushed to the registry (requires --push)"
+    ),
+)
+def make_app(
+    target,
+    spec_root,
+    registry,
+    release,
+    tag_latest,
+    save_manifest,
     logfile,
     loglevel,
-    build_dir,
+    build_dir: Path,
     use_local_packages,
     install_extras,
     raise_errors,
     generate_only,
     use_test_config,
-    license_dir,
+    license,
+    license_to_download,
     check_registry,
     push,
+    clean_up,
 ):
 
-    if isinstance(spec_path, bytes):  # FIXME: This shouldn't be necessary
-        spec_path = Path(spec_path.decode("utf-8"))
+    if clean_up and not push:
+        raise ValueError("'--clean-up' flag requires '--push'")
+
+    if tag_latest and not release:
+        raise ValueError("'--tag-latest' flag requires '--release'")
+
+    if isinstance(spec_root, bytes):  # FIXME: This shouldn't be necessary
+        spec_root = Path(spec_root.decode("utf-8"))
     if isinstance(build_dir, bytes):  # FIXME: This shouldn't be necessary
         build_dir = Path(build_dir.decode("utf-8"))
-    if isinstance(license_dir, bytes):  # FIXME: This shouldn't be necessary
-        license_dir = Path(license_dir.decode("utf-8"))
-
-    if install_extras:
-        install_extras = install_extras.split(",")
-    else:
-        install_extras = []
 
-    logging.basicConfig(filename=logfile, level=getattr(logging, loglevel.upper()))
+    if build_dir is None:
+        build_dir = spec_root / ".build"
 
-    temp_dir = tempfile.mkdtemp()
+    if not build_dir.exists():
+        build_dir.mkdir()
 
-    errors = False
-    for spath in walk_spec_paths(spec_path):
+    install_extras = install_extras.split(",") if install_extras else []
 
-        logging.info("Building '%s' image", spath)
-        spec = load_yaml_spec(spath, base_dir=spec_path)
+    logging.basicConfig(filename=logfile, level=getattr(logging, loglevel.upper()))
 
-        # Make image tag
-        pkg_name = spath.stem.lower()
-        tag = ".".join(spath.relative_to(spec_path).parent.parts + (pkg_name,))
+    temp_dir = tempfile.mkdtemp()
 
-        image_version = str(spec.pop("pkg_version"))
-        if "wrapper_version" in spec:
-            image_version += f"-{spec.pop('wrapper_version')}"
+    target_cls = ClassResolver(App)(target)
 
-        image_tag = f"{docker_org}/{tag}:{image_version}"
-        if docker_registry != DOCKER_HUB:
-            image_tag = docker_registry.lower() + "/" + image_tag
+    dc = docker.from_env()
 
-        if build_dir is None:
-            image_build_dir = spath.parent / ".build" / spath.stem
-        else:
-            image_build_dir = build_dir
-            if spath != spec_path:
-                image_build_dir /= spath.parent.relative_to(spec_path)
-            image_build_dir /= spath.stem
-
-        image_build_dir.mkdir(exist_ok=True, parents=True)
-
-        # Update the spec to remove '_' prefixed keys and add in build params
-        spec = {k: v for k, v in spec.items() if not k.startswith("_")}
-        spec.update(
-            {
-                "image_tag": image_tag,
-                "docker_registry": docker_registry,
-                "use_local_packages": use_local_packages,
-                "arcana_install_extras": install_extras,
-                "test_config": use_test_config,
-            }
+    license_paths = {}
+    for lic_name, lic_src in license:
+        if isinstance(lic_src, bytes):  # FIXME: This shouldn't be necessary
+            lic_src = Path(lic_src.decode("utf-8"))
+        license_paths[lic_name] = lic_src
+
+    # Load image specifications from YAML files stored in directory tree
+
+    # Don't error if the modules the task, data stores, data types, etc...
+    # aren't present in the build environment
+    # FIXME: need to test for this
+    with ClassResolver.FALLBACK_TO_STR:
+        image_specs = target_cls.load_tree(
+            spec_root,
+            registry=registry,
+            license_paths=license_paths,
+            licenses_to_download=set(license_to_download),
         )
 
-        # Check the target registry to see a) if an image with the same tag
-        # already exists and b) whether it was built with the same specs
-        if check_registry:
+    # Check the target registry to see a) if the images with the same tag
+    # already exists and b) whether it was built with the same specs
+    if check_registry:
+
+        conflicting = {}
+        to_build = []
+        for image_spec in image_specs:
+
             extracted_dir = extract_file_from_docker_image(
-                image_tag, spec_path_in_docker
+                image_spec.reference, image_spec.SPEC_PATH
             )
-            if extracted_dir is not None:
+            if extracted_dir is None:
                 logger.info(
-                    f"Comparing build spec with that of existing image {image_tag}"
+                    f"Did not find existing image matching {image_spec.reference}"
                 )
-                built_spec = load_yaml_spec(
-                    extracted_dir / Path(spec_path_in_docker).name
+                changelog = None
+            else:
+                logger.info(
+                    f"Comparing build spec with that of existing image {image_spec.reference}"
                 )
-                if diff := compare_specs(built_spec, spec, check_version=True):
-                    msg = (
-                        f"Spec for '{image_tag}' doesn't match the one that was "
-                        "used to build the image already in the registry (skipping):\n\n"
-                        + str(diff.pretty())
-                    )
-                    if raise_errors:
-                        raise ArcanaBuildError(msg)
-                    else:
-                        logger.error(msg)
-                    continue
-                else:
-                    logger.info(
-                        "Skipping '%s' build as identical image already "
-                        "exists in registry"
-                    )
-                    continue
+                built_spec = image_spec.load(
+                    extracted_dir / Path(image_spec.SPEC_PATH).name
+                )
+
+                changelog = image_spec.compare_specs(built_spec, check_version=True)
+
+            if changelog is None:
+                to_build.append(image_spec)
+            elif not changelog:
+                logger.info(
+                    "Skipping '%s' build as identical image already "
+                    "exists in registry"
+                )
+            else:
+                conflicting[image_spec.reference] = changelog
+
+        if conflicting:
+            msg = ""
+            for tag, changelog in conflicting.items():
+                msg += (
+                    f"spec for '{tag}' doesn't match the one that was "
+                    "used to build the image already in the registry:\n\n"
+                    + str(changelog.pretty())
+                    + "\n\n\n"
+                )
+
+            raise ArcanaBuildError(msg)
+
+        image_specs = to_build
+
+    if release or save_manifest:
+        manifest = {
+            "package": spec_root.stem,
+            "images": [],
+        }
+        if release:
+            manifest["release"] = ":".join(release)
+
+    errors = False
+
+    for image_spec in image_specs:
+        spec_build_dir = (
+            build_dir / image_spec.loaded_from.relative_to(spec_root)
+        ).with_suffix("")
+        if spec_build_dir.exists():
+            shutil.rmtree(spec_build_dir)
+        spec_build_dir.mkdir(parents=True)
         try:
-            build_xnat_cs_image(
-                build_dir=image_build_dir,
+            image_spec.make(
+                build_dir=spec_build_dir,
+                use_test_config=use_test_config,
+                use_local_packages=use_local_packages,
                 generate_only=generate_only,
-                license_dir=license_dir,
-                **spec,
             )
         except Exception:
             if raise_errors:
                 raise
-            logger.error("Could not build %s pipeline:\n%s", image_tag, format_exc())
+            logger.error(
+                "Could not build %s pipeline:\n%s", image_spec.reference, format_exc()
+            )
             errors = True
             continue
         else:
-            click.echo(image_tag)
-            logger.info("Successfully built %s pipeline", image_tag)
+            click.echo(image_spec.reference)
+            logger.info("Successfully built %s pipeline", image_spec.reference)
 
         if push:
-            dc = docker.from_env()
             try:
-                dc.api.push(image_tag)
-            except Exception as e:
+                dc.api.push(image_spec.reference)
+            except Exception:
                 if raise_errors:
                     raise
-                logger.error(f"Could not push '%s':\n\n%s", image_tag, format_exc())
+                logger.error(
+                    "Could not push '%s':\n\n%s", image_spec.reference, format_exc()
+                )
                 errors = True
             else:
-                logger.info("Successfully pushed '%s' to registry", image_tag)
+                logger.info(
+                    "Successfully pushed '%s' to registry", image_spec.reference
+                )
+            if clean_up:
+                dc.api.remove_image(image_spec.reference)
+                dc.containers.prune()
+                dc.images.prune(filters={"dangling": False})
+                dc.api.remove_image(image_spec.base_image)
+                dc.images.prune(filters={"dangling": False})
+                logger.info(
+                    "Removed '%s' and pruned dangling images to free up disk space",
+                    image_spec.reference,
+                )
+
+        if release or save_manifest:
+            manifest["images"].append(
+                {
+                    "name": image_spec.path,
+                    "version": image_spec.tag,
+                }
+            )
+    if release:
+        metapkg = Metapackage(
+            name=release[0],
+            version=release[1],
+            org=spec_root.stem,
+            manifest=manifest,
+        )
+        metapkg.make(use_local_packages=use_local_packages)
+        if push:
+            try:
+                dc.api.push(metapkg.reference)
+            except Exception:
+                if raise_errors:
+                    raise
+                logger.error(
+                    "Could not push release metapackage '%s':\n\n%s",
+                    metapkg.reference,
+                    format_exc(),
+                )
+                errors = True
+            else:
+                logger.info(
+                    "Successfully pushed release metapackage '%s' to registry",
+                    metapkg.reference,
+                )
+
+            if tag_latest:
+                # Also push release to "latest" tag
+                image = dc.images.get(metapkg.reference)
+                latest_tag = metapkg.path + ":latest"
+                image.reference(latest_tag)
+
+                try:
+                    dc.api.push(latest_tag)
+                except Exception:
+                    if raise_errors:
+                        raise
+                    logger.error(
+                        "Could not push latest tag for release metapackage '%s':\n\n%s",
+                        metapkg.path,
+                        format_exc(),
+                    )
+                    errors = True
+                else:
+                    logger.info(
+                        (
+                            "Successfully pushed latest tag for release metapackage '%s' "
+                            "to registry"
+                        ),
+                        metapkg.path,
+                    )
+        if save_manifest:
+            with open(save_manifest, "w") as f:
+                json.dump(manifest, f, indent="    ")
 
     shutil.rmtree(temp_dir)
     if errors:
         sys.exit(1)
 
 
 @deploy.command(
     name="list-images",
     help="""Walk through the specification paths and list tags of the images
 that will be build from them.
 
-SPEC_PATH is the file system path to the specification to build, or directory
+SPEC_ROOT is the file system path to the specification to build, or directory
 containing multiple specifications
 
 DOCKER_ORG is the Docker organisation the images should belong to""",
 )
-@click.argument("spec_path", type=click.Path(exists=True, path_type=Path))
-@click.argument("docker_org", type=str)
+@click.argument("spec_root", type=click.Path(exists=True, path_type=Path))
 @click.option(
     "--registry",
-    "docker_registry",
     default=None,
     help="The Docker registry to deploy the pipeline to",
 )
-def list_images(spec_path, docker_org, docker_registry):
+def list_images(spec_root, registry):
 
-    if isinstance(spec_path, bytes):  # FIXME: This shouldn't be necessary
-        spec_path = Path(spec_path.decode("utf-8"))
+    if isinstance(spec_root, bytes):  # FIXME: This shouldn't be necessary
+        spec_root = Path(spec_root.decode("utf-8"))
 
-    for spath in walk_spec_paths(spec_path):
-        spec = load_yaml_spec(spath, base_dir=spec_path)
-
-        # Make image tag
-        pkg_name = spath.stem.lower()
-        tag = ".".join(spath.relative_to(spec_path).parent.parts + (pkg_name,))
-        image_version = str(spec.pop("pkg_version"))
-        if "wrapper_version" in spec:
-            image_version += f"-{spec.pop('wrapper_version')}"
-        image_tag = f"{docker_org}/{tag}:{image_version}"
-        if docker_registry is not None:
-            image_tag = docker_registry.lower().rstrip("/") + "/" + image_tag
-        else:
-            docker_registry = DOCKER_HUB
-        click.echo(image_tag)
+    for image_spec in App.load_tree(spec_root, registry=registry):
+        click.echo(image_spec.reference)
 
 
-@deploy.command(
-    name="test",
-    help="""Test container images defined by YAML
-specs
-
-Arguments
----------
-module_path
-    The file system path to the module to build""",
-)
-@click.argument("spec_path", type=click.Path(exists=True, path_type=Path))
-def test(spec_path):
-    # FIXME: Workaround for click 7.x, which improperly handles path_type
-    if type(spec_path) is bytes:
-        spec_path = Path(spec_path.decode("utf-8"))
+# @deploy.command(
+#     name="test",
+#     help="""Test container images defined by YAML
+# specs
+
+# Arguments
+# ---------
+# module_path
+#     The file system path to the module to build""",
+# )
+# @click.argument("spec_path", type=click.Path(exists=True, path_type=Path))
+# def test(spec_path):
+#     # FIXME: Workaround for click 7.x, which improperly handles path_type
+#     if type(spec_path) is bytes:
+#         spec_path = Path(spec_path.decode("utf-8"))
 
-    raise NotImplementedError
+#     raise NotImplementedError
 
 
 @deploy.command(
-    name="docs",
+    name="make-docs",
     help="""Build docs for one or more yaml wrappers
 
-SPEC_PATH is the path of a YAML spec file or directory containing one or more such files.
+SPEC_ROOT is the path of a YAML spec file or directory containing one or more such files.
 
 The generated documentation will be saved to OUTPUT.
 """,
 )
-@click.argument("spec_path", type=click.Path(exists=True, path_type=Path))
+@click.argument("spec_root", type=click.Path(exists=True, path_type=Path))
 @click.argument("output", type=click.Path(path_type=Path))
 @click.option(
-    "--root", type=click.Path(exists=True, path_type=Path), default=Path.cwd()
+    "--registry",
+    default=DOCKER_HUB,
+    help="The Docker registry to deploy the pipeline to",
 )
 @click.option("--flatten/--no-flatten", default=False)
 @click.option("--loglevel", default="warning", help="The level to display logs at")
-def build_docs(spec_path, output, root, flatten, loglevel):
+def make_docs(spec_root, output, registry, flatten, loglevel):
     # FIXME: Workaround for click 7.x, which improperly handles path_type
-    if type(spec_path) is bytes:
-        spec_path = Path(spec_path.decode("utf-8"))
+    if type(spec_root) is bytes:
+        spec_root = Path(spec_root.decode("utf-8"))
     if type(output) is bytes:
         output = Path(output.decode("utf-8"))
 
     logging.basicConfig(level=getattr(logging, loglevel.upper()))
 
     output.mkdir(parents=True, exist_ok=True)
 
-    for spath in walk_spec_paths(spec_path):
-        spec = load_yaml_spec(spath, base_dir=spec_path)
-        mod_name = spec["_module_name"]
+    with ClassResolver.FALLBACK_TO_STR:
+        image_specs = App.load_tree(spec_root, registry=registry)
 
-        try:
-            src_file = spath.absolute().relative_to(root)
-        except ValueError:
-            logger.warning(
-                f"build_docs: {spath.absolute().as_posix()!r} does not lie "
-                f"within {root.as_posix()!r}, do you need to specify --root?"
-            )
-            src_file = spath.absolute()
+    for image_spec in image_specs:
 
-        create_doc(spec, output, mod_name, src_file=src_file, flatten=flatten)
-        logging.info("Successfully created docs for %s", mod_name)
+        image_spec.autodoc(output, flatten=flatten)
+        logging.info("Successfully created docs for %s", image_spec.path)
 
 
 @deploy.command(
     name="required-packages",
-    help="""Detect the Python packages required to run the 
+    help="""Detect the Python packages required to run the
 specified workflows and return them and their versions""",
 )
 @click.argument("task_locations", nargs=-1)
 def required_packages(task_locations):
 
     required_modules = set()
     for task_location in task_locations:
-        workflow = resolve_class(task_location)
+        workflow = ClassResolver(TaskBase, alternative_types=[ty.Callable])(
+            task_location
+        )
         pydra_asdict(workflow, required_modules)
 
     for pkg in package_from_module(required_modules):
         click.echo(f"{pkg.key}=={pkg.version}")
 
 
 @deploy.command(
@@ -414,399 +541,112 @@
     executable = image_attrs["Entrypoint"]
     if executable is None:
         executable = image_attrs["Cmd"]
 
     click.echo(executable)
 
 
-@click.command(
-    name="run-arcana-pipeline",
-    help="""Defines a new dataset, applies and launches a pipeline
-in a single command. Given the complexity of combining all these steps in one
-CLI, it isn't recommended to use this command manually, it is typically used
-by automatically generated code when deploying a pipeline within a container image.
-
-Not all options are be used when defining datasets, however, the
-'--dataset_name <NAME>' option can be provided to use an existing dataset
-definition.
+@deploy.command(
+    help="""Displays the changelogs found in the release manifest of a deployment build
 
-DATASET_ID_STR string containing the nickname of the data store, the ID of the
-dataset (e.g. XNAT project ID or file-system directory) and the dataset's name
-in the format <STORE-NICKNAME>//<DATASET-ID>:<DATASET-NAME>
+MANIFEST_JSON is a JSON file containing a list of container images built in the release
+and the commands present in them"""
+)
+@click.argument("manifest_json", type=click.File())
+@click.argument("images", nargs=-1)
+def changelog(manifest_json):
 
-PIPELINE_NAME is the name of the pipeline
+    manifest = json.load(manifest_json)
 
-WORKFLOW_LOCATION is the location to a Pydra workflow on the Python system path.
-It can be omitted if PIPELINE_NAME matches an existing pipeline
+    for entry in manifest["images"]:
+        click.echo(
+            f"{entry['name']} [{entry['version']}] changes "
+            f"from {entry['previous_version']}:\n{entry['changelog']}"
+        )
+
+
+@deploy.command(
+    name="install-license",
+    help="""Installs a license within a store (i.e. site-wide) or dataset (project-specific)
+for use in a deployment pipeline
+
+LICENSE_NAME the name of the license to upload. Must match the name of the license specified
+in the deployment specification
+
+SOURCE_FILE path to the license file to upload
+
+INSTALL_LOCATIONS a list of installation locations, which are either the "nickname" of a
+store (as saved by `arcana store add`) or the ID of a dataset in form
+<store-nickname>//<dataset-id>[@<dataset-name>], where the dataset ID
+is either the location of the root directory (for file-system based stores) or the
+project ID for managed data repositories.
 """,
 )
-@click.argument("dataset_id_str")
-@click.argument("pipeline_name")
-@click.argument("task_location")
-@click.option(
-    "--parameter",
-    "-p",
-    nargs=2,
-    default=(),
-    metavar="<name> <value>",
-    multiple=True,
-    type=str,
-    help=("free parameters of the workflow to be passed by the pipeline user"),
-)
-@click.option(
-    "--input",
-    nargs=5,
-    default=(),
-    metavar="<col-name> <col-format> <match-criteria> <pydra-field> <format>",
-    multiple=True,
-    type=str,
-    help=(
-        "link an input of the task/workflow to a column of the dataset, adding a source"
-        "column matched by the name/path of the column if it isn't already present. "
-        "Automatically generated source columns must be able to be specified by their "
-        "path alone and be already in the format required by the task/workflow"
-    ),
-)
-@click.option(
-    "--output",
-    nargs=5,
-    default=(),
-    metavar="<col-name> <col-format> <output-path> <pydra-field> <format>",
-    multiple=True,
-    type=str,
-    help=(
-        "add a sink to the dataset and link it to an output of the task/workflow "
-        "in a single step. The sink column be in the same format as produced "
-        "by the task/workflow"
-    ),
-)
-@click.option(
-    "--row_frequency",
-    "-f",
-    default=None,
-    type=str,
-    help=(
-        "the row_frequency of the rows the pipeline will be executed over, i.e. "
-        "will it be run once per-session, per-subject or per whole dataset, "
-        "by default the highest row_frequency rows (e.g. per-session)"
-    ),
-)
-@click.option(
-    "--ids", default=None, type=str, help="List of IDs to restrict the pipeline to"
-)
-@click.option(
-    "--work",
-    "-w",
-    "work_dir",
-    default=None,
-    help=(
-        "The location of the directory where the working files "
-        "created during the pipeline execution will be stored"
-    ),
-)
-@click.option(
-    "--plugin",
-    default="cf",
-    help=("The Pydra plugin with which to process the task/workflow"),
-)
-@click.option(
-    "--loglevel",
-    type=str,
-    default="info",
-    help=("The level of detail logging information is presented"),
-)
-@click.option(
-    "--dataset_hierarchy", type=str, default=None, help="Comma-separated hierarchy"
-)
-@click.option(
-    "--dataset_space", type=str, default=None, help="The data space of the dataset"
-)
-@click.option("--dataset_name", type=str, default=None, help="The name of the dataset")
-@click.option(
-    "--single-row",
-    type=str,
-    default=None,
-    help=(
-        "Restrict the dataset created to a single row (to avoid issues with "
-        "unrelated rows that aren't being processed). Comma-separated list "
-        "of IDs for each layer of the hierarchy (passed to `Dataset.add_leaf`)"
-    ),
-)
-@click.option(
-    "--overwrite/--no-overwrite",
-    type=bool,
-    help=("Whether to overwrite the saved pipeline with the same name, if present"),
-)
+@click.argument("license_name")
+@click.argument("source_file", type=click.Path(exists=True, path_type=Path))
+@click.argument("install_locations", nargs=-1)
 @click.option(
-    "--configuration",
-    nargs=2,
-    default=(),
-    metavar="<name> <value>",
-    multiple=True,
-    type=str,
-    help=(
-        "configuration args of the task/workflow. Differ from parameters in that they is passed to the "
-        "task/workflow at initialisation (and can therefore help specify its inputs) not as inputs. Values "
-        "can be any valid JSON (including basic types)."
-    ),
-)
-@click.option(
-    "--export-work",
+    "--logfile",
     default=None,
-    type=click.Path(exists=False, path_type=Path),
-    help="Export the work directory to another location after the task/workflow exits",
-)
-@click.option(
-    "--raise-errors/--catch-errors",
-    type=bool,
-    default=False,
-    help="raise exceptions instead of capturing them to suppress call stack",
-)
-@click.option(
-    "--keep-running-on-errors/--exit-on-errors",
-    type=bool,
-    default=False,
-    help=(
-        "Keep the the pipeline running in infinite loop on error (will need "
-        "to be manually killed). Can be useful in situations where the "
-        "enclosing container will be removed on completion and you need to "
-        "be able to 'exec' into the container to debug."
-    ),
+    type=click.Path(path_type=Path),
+    help="Log output to file instead of stdout",
 )
-def run_pipeline(
-    dataset_id_str,
-    pipeline_name,
-    task_location,
-    parameter,
-    input,
-    output,
-    row_frequency,
-    overwrite,
-    work_dir,
-    plugin,
-    loglevel,
-    dataset_name,
-    dataset_space,
-    dataset_hierarchy,
-    ids,
-    configuration,
-    single_row,
-    export_work,
-    raise_errors,
-    keep_running_on_errors,
-):
+@click.option("--loglevel", default="info", help="The level to display logs at")
+def install_license(install_locations, license_name, source_file, logfile, loglevel):
 
-    if type(export_work) is bytes:
-        export_work = Path(export_work.decode("utf-8"))
+    logging.basicConfig(filename=logfile, level=getattr(logging, loglevel.upper()))
 
-    if loglevel != "none":
-        logging.basicConfig(stream=sys.stdout, level=getattr(logging, loglevel.upper()))
+    if isinstance(source_file, bytes):  # FIXME: This shouldn't be necessary
+        source_file = Path(source_file.decode("utf-8"))
 
-    if work_dir is None:
-        work_dir = tempfile.mkdtemp()
-    work_dir = Path(work_dir)
-    work_dir.mkdir(parents=True, exist_ok=True)
-
-    store_cache_dir = work_dir / "store-cache"
-    pipeline_cache_dir = work_dir / "pydra"
-
-    try:
-        dataset = Dataset.load(dataset_id_str)
-    except KeyError:
-
-        store_name, id, name = Dataset.parse_id_str(dataset_id_str)
-
-        if dataset_name is not None:
-            name = dataset_name
-
-        if dataset_hierarchy is None or dataset_space is None:
-            raise RuntimeError(
-                f"If the dataset ID string ('{dataset_id_str}') doesn't "
-                "reference an existing dataset '--dataset_hierarchy' and "
-                "'--dataset_space' must be provided"
-            )
+    if not install_locations:
+        install_locations = ["file"]
 
-        store = DataStore.load(store_name, cache_dir=store_cache_dir)
-        space = resolve_class(dataset_space, ["arcana.data.spaces"])
-        hierarchy = dataset_hierarchy.split(",")
-
-        dataset = store.new_dataset(id, hierarchy=hierarchy, space=space)
-
-    if single_row is not None:
-        # Adds a single row to the dataset (i.e. skips a full scan)
-        dataset.add_leaf(single_row.split(","))
-
-    def extract_qualifiers_from_path(user_input: str):
-        """Extracts out "qualifiers" from the user-inputted paths. These are
-        in the form 'path kw1=val1 kw2=val2...
-
-        Parameters
-        ----------
-        col_name : str
-            name of the column the
-        user_input : str
-            The path expression + qualifying keyword args to extract
-
-        Returns
-        -------
-        path : str
-            the path expression stripped of qualifiers
-        qualifiers : defaultdict[dict]
-            the extracted qualifiers
-        """
-        qualifiers = defaultdict(dict)
-        if "=" in user_input:  # Treat user input as containing qualifiers
-            parts = shlex.split(user_input)
-            path = parts[0]
-            for part in parts[1:]:
-                try:
-                    full_name, val = part.split("=", maxsplit=1)
-                except ValueError as e:
-                    e.args = ((e.args[0] + f" attempting to split '{part}' by '='"),)
-                    raise e
-                try:
-                    ns, name = full_name.split(".", maxsplit=1)
-                except ValueError as e:
-                    e.args = (
-                        (e.args[0] + f" attempting to split '{full_name}' by '.'"),
-                    )
-                    raise e
-                qualifiers[ns][name] = val
-        else:
-            path = user_input
-        return path, qualifiers
-
-    pipeline_inputs = []
-    converter_args = {}  # Arguments passed to converter
-    for col_name, col_format_name, match_criteria, pydra_field, format_name in input:
-        col_format = resolve_class(col_format_name, prefixes=["arcana.data.formats"])
-        format = resolve_class(format_name, prefixes=["arcana.data.formats"])
-        if not match_criteria and format != DataRow:
-            logger.warning(
-                f"Skipping '{col_name}' source column as no input was provided"
-            )
-            continue
-        pipeline_inputs.append(PipelineInput(col_name, pydra_field, format))
-        if DataRow in (col_format, format):
-            if (col_format, format) != (DataRow, DataRow):
-                raise ArcanaUsageError(
-                    "Cannot convert to/from built-in data type `DataRow`: "
-                    f"col_format={col_format}, format={format}"
-                )
-            logger.info(
-                f"No column added for '{col_name}' column as it uses built-in "
-                "type `arcana.core.data.row.DataRow`"
-            )
-            continue
-        path, qualifiers = extract_qualifiers_from_path(match_criteria)
-        source_kwargs = qualifiers.pop("criteria", {})
-        converter_args[col_name] = qualifiers.pop("converter", {})
-        if qualifiers:
-            raise ArcanaUsageError(
-                "Unrecognised qualifier namespaces extracted from path for "
-                f"{col_name} (expected ['criteria', 'converter']): {qualifiers}"
-            )
-        if col_name in dataset.columns:
-            column = dataset[col_name]
-            logger.info(f"Found existing source column {column}")
+    for install_loc in install_locations:
+        if "//" in install_loc:
+            dataset = Dataset.load(install_loc)
+            store_name, _, _ = Dataset.parse_id_str(install_loc)
+            msg = f"for '{dataset.name}' dataset on {store_name} store"
         else:
-            logger.info(f"Adding new source column '{col_name}'")
-            dataset.add_source(
-                name=col_name,
-                format=col_format,
-                path=path,
-                is_regex=True,
-                **source_kwargs,
-            )
+            store = DataStore.load(install_loc)
+            dataset = store.site_licenses_dataset()
+            if dataset is None:
+                raise ValueError(
+                    f"{install_loc} store doesn't support the installation of site-wide "
+                    "licenses, please specify a dataset to install it for"
+                )
+            msg = f"site-wide on {install_loc} store"
 
-    logger.debug("Pipeline inputs: %s", pipeline_inputs)
+        dataset.install_license(license_name, source_file)
+        logger.info("Successfully installed '%s' license %s", license_name, msg)
 
-    pipeline_outputs = []
-    for col_name, col_format_name, path_expr, pydra_field, format_name in output:
-        format = resolve_class(format_name, prefixes=["arcana.data.formats"])
-        col_format = resolve_class(col_format_name, prefixes=["arcana.data.formats"])
-        pipeline_outputs.append(PipelineOutput(col_name, pydra_field, format))
-        path, qualifiers = extract_qualifiers_from_path(path_expr)
-        converter_args[col_name] = qualifiers.pop("converter", {})
-        if qualifiers:
-            raise ArcanaUsageError(
-                "Unrecognised qualifier namespaces extracted from path for "
-                f"{col_name} (expected ['criteria', 'converter']): {qualifiers}"
-            )
-        if col_name in dataset.columns:
-            column = dataset[col_name]
-            if not column.is_sink:
-                raise ArcanaUsageError(
-                    "Output column name '{col_name}' shadows existing source column"
-                )
-            logger.info(f"Found existing sink column {column}")
-        else:
-            logger.info(f"Adding new source column '{col_name}'")
-            dataset.add_sink(name=col_name, format=col_format, path=path)
 
-    logger.debug("Pipeline outputs: %s", pipeline_outputs)
+@deploy.command(
+    name="pipeline-entrypoint",
+    help="""Loads/creates a dataset, then applies and launches a pipeline
+in a single command. To be used within the command configuration of an XNAT
+Container Service ready Docker image.
 
-    kwargs = {n: parse_value(v) for n, v in configuration}
-    if "name" not in kwargs:
-        kwargs["name"] = "workflow_to_run"
-
-    task = resolve_class(task_location)(**kwargs)
-
-    for pname, pval in parameter:
-        if pval != "":
-            setattr(task.inputs, pname, parse_value(pval))
-
-    if pipeline_name in dataset.pipelines and not overwrite:
-        pipeline = dataset.pipelines[pipeline_name]
-        if task != pipeline.workflow:
-            raise RuntimeError(
-                f"A pipeline named '{pipeline_name}' has already been applied to "
-                "which differs from one specified. Please use '--overwrite' option "
-                "if this is intentional"
-            )
-    else:
-        pipeline = dataset.apply_pipeline(
-            pipeline_name,
-            task,
-            inputs=pipeline_inputs,
-            outputs=pipeline_outputs,
-            row_frequency=row_frequency,
-            overwrite=overwrite,
-            converter_args=converter_args,
-        )
+DATASET_LOCATOR string containing the nickname of the data store, the ID of the
+dataset (e.g. XNAT project ID or file-system directory) and the dataset's name
+in the format <store-nickname>//<dataset-id>[@<dataset-name>]
 
-    # Instantiate the Pydra workflow
-    wf = pipeline(cache_dir=pipeline_cache_dir)
+""",
+)
+@click.argument("dataset_locator")
+@entrypoint_opts.data_columns
+@entrypoint_opts.parameterisation
+@entrypoint_opts.execution
+@entrypoint_opts.dataset_config
+@entrypoint_opts.debugging
+def pipeline_entrypoint(
+    dataset_locator,
+    spec_path,
+    **kwargs,
+):
 
-    if ids is not None:
-        ids = ids.split(",")
+    image_spec = App.load(spec_path)
 
-    # execute the workflow
-    try:
-        result = wf(ids=ids, plugin=plugin)
-    except Exception:
-        msg = show_workflow_errors(pipeline_cache_dir, omit_nodes=["per_node", wf.name])
-        logger.error("Pipeline failed with errors for the following nodes:\n\n%s", msg)
-        if raise_errors or not msg:
-            raise
-        else:
-            errors = True
-    else:
-        logger.info(
-            "Pipeline %s ran successfully for the following data rows:\n%s",
-            pipeline_name,
-            "\n".join(result.output.processed),
-        )
-        errors = False
-    finally:
-        if export_work:
-            logger.info("Exporting work directory to '%s'", export_work)
-            export_work.mkdir(parents=True, exist_ok=True)
-            shutil.copytree(pipeline_cache_dir, export_work / "pydra")
-    # Abort at the end after the working directory can be copied back to the
-    # host so that XNAT knows there was an error
-    if errors:
-        if keep_running_on_errors:
-            while True:
-                pass
-        else:
-            sys.exit(1)
+    image_spec.command.execute(
+        dataset_locator,
+        **kwargs,
+    )
```

### Comparing `arcana-2.0b0.dev7/arcana/cli/derive.py` & `arcana-2.0b2/arcana/core/cli/derive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from pathlib import Path
 import logging
 import cloudpickle as cp
 import click
-from arcana import __version__
-from arcana.core.cli import cli
 from arcana.core.data.set import Dataset
-from arcana.core.utils import set_loggers
-
+from arcana.core.utils.misc import set_loggers
+from .base import cli
 
 logger = logging.getLogger("arcana")
 
 
 @cli.group()
 def derive():
     pass
 
 
 @derive.command(
     name="column",
     help="""Derive data for a data sink column and
 all prerequisite columns.
 
-DATASET_ID_STR string containing the nickname of the data store, the ID of the dataset
+DATASET_LOCATOR string containing the nickname of the data store, the ID of the dataset
 (e.g. XNAT project ID or file-system directory) and the dataset's name in the
-format <STORE-NICKNAME>//<DATASET-ID>:<DATASET-NAME>
+format <store-nickname>//<dataset-id>[@<dataset-name>]
 
 COLUMNS are the names of the sink columns to derive""",
 )
-@click.argument("dataset_id_str")
+@click.argument("dataset_locator")
 @click.argument("columns", nargs=-1)
 @click.option(
     "--work",
     "-w",
     default=None,
     help=(
         "The location of the directory where the working files "
@@ -45,27 +43,27 @@
 )
 @click.option(
     "--loglevel",
     type=str,
     default="info",
     help=("The level of detail logging information is presented"),
 )
-def derive_column(dataset_id_str, columns, work, plugin, loglevel):
+def derive_column(dataset_locator, columns, work, plugin, loglevel):
 
     logging.basicConfig(level=getattr(logging, loglevel.upper()))
 
     if work is not None:
         work_dir = Path(work)
         store_cache = work_dir / "store-cache"
         pipeline_cache = work_dir / "pipeline-cache"
     else:
         store_cache = None
         pipeline_cache = None
 
-    dataset = Dataset.load(dataset_id_str, cache_dir=store_cache)
+    dataset = Dataset.load(dataset_locator, cache_dir=store_cache)
 
     set_loggers(loglevel)
 
     dataset.derive(*columns, cache_dir=pipeline_cache, plugin=plugin)
 
     columns_str = "', '".join(columns)
     logger.info(f"Derived data for '{columns_str}' column(s) successfully")
```

### Comparing `arcana-2.0b0.dev7/arcana/cli/store.py` & `arcana-2.0b2/arcana/core/cli/store.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from inspect import Arguments
 from operator import itemgetter
 import click
-from arcana.core.utils import resolve_class
 from arcana.core.data.store import DataStore
-from arcana.core.cli import cli
-from arcana.core.utils import get_home_dir, class_location
+from arcana.core.utils.serialize import ClassResolver
+from arcana.core.utils.misc import get_home_dir
+from .base import cli
 
 
 @cli.group()
 def store():
     pass
 
 
@@ -18,15 +17,15 @@
 
 Arguments
 ---------
 nickname
     The name given to the store for reference in other commands
 type
     The storage class and the module it is defined in, e.g.
-    `arcana.data.store.medimage:Xnat`
+    `arcana.data.store.xnat:Xnat`
 location
     The location of the store, e.g. server address
 *varargs
     Parameters that are specific to the 'type' of storage class to be added
 """
 )
 @click.argument("nickname")
@@ -48,15 +47,16 @@
     "-c",
     default=None,
     help="The location of a cache dir to download local copies of remote data",
 )
 def add(nickname, type, location, varargs, cache, user, password):
     if cache is None:
         cache = get_home_dir() / "cache" / nickname
-    store_cls = resolve_class(type, ["arcana.data.stores"])
+        cache.mkdir(parents=True, exist_ok=True)
+    store_cls = ClassResolver(DataStore)(type)
     store = store_cls(location, *varargs, cache_dir=cache, user=user, password=password)
     store.save(nickname)
 
 
 @store.command(
     help="""
 Gives a data store saved in the config file ('~/.arcana/stores.yaml') a new
@@ -113,14 +113,14 @@
     store.save(nickname)
 
 
 @store.command(help="""List available stores that have been saved""")
 def ls():
     click.echo("Built-in stores\n---------------")
     for name, store in sorted(DataStore.singletons().items(), key=itemgetter(0)):
-        click.echo(f"{name} - {class_location(store)}")
+        click.echo(f"{name} - {ClassResolver.tostr(store, strip_prefix=False)}")
     click.echo("\nSaved stores\n-------------")
     for name, entry in DataStore.load_saved_entries().items():
         store_class = entry.pop("class")
         click.echo(f"{name} - {store_class[1:-1]}")
         for key, val in sorted(entry.items(), key=itemgetter(0)):
             click.echo(f"    {key}: {val}")
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/column.py` & `arcana-2.0b2/arcana/core/data/column.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 import re
 import typing as ty
 import attrs
 from operator import attrgetter
 from attrs.converters import optional
 
 # from arcana.core.data.row import DataRow
-from arcana.core.utils import class_location
+from arcana.core.utils.serialize import ClassResolver
 from arcana.exceptions import ArcanaDataMatchError
-from ..enum import DataQuality, ColumnSalience
+from ..analysis.salience import DataQuality, ColumnSalience
 from .space import DataSpace
 
 
+ItemType = ty.TypeVar("ItemType")
+
+
 @attrs.define
-class DataColumn(metaclass=ABCMeta):
+class DataColumn(ty.Generic[ItemType], metaclass=ABCMeta):
 
     name: str = attrs.field()
     path: str = attrs.field()
-    format = attrs.field()
+    datatype = attrs.field()
     row_frequency: DataSpace = attrs.field()
     dataset = attrs.field(
         default=None, metadata={"asdict": False}, eq=False, hash=False, repr=False
     )
 
     def __iter__(self):
         return (n[self.name] for n in self.dataset.rows(self.row_frequency))
 
-    def __getitem__(self, id):
+    def __getitem__(self, id) -> ItemType:
         return self.dataset.row(id=id, row_frequency=self.row_frequency)[self.name]
 
     def __len__(self):
         return len(list(self.dataset.rows(self.row_frequency)))
 
     @property
     def ids(self):
@@ -44,15 +47,15 @@
         Parameters
         ----------
         row: DataRow
             the row to match the item from
 
         Returns
         -------
-        DataItem
+        DataType
             the data item that matches the criteria/path
 
         Raises
         ------
         ArcanaDataMatchError
             if none or multiple items match the criteria/path of the column
             within the row
@@ -73,15 +76,15 @@
 
     Parameters
     ----------
     path : str
         A regex name_path to match the file_group names with. Must match
         one and only one file_group per <row_frequency>. If None, the name
         is used instead.
-    format : type
+    datatype : type
         File format that data will be
     row_frequency : DataSpace
         The row_frequency of the file-group within the dataset tree, e.g. per
         'session', 'subject', 'timepoint', 'group', 'dataset'
     quality_threshold : DataQuality
         The acceptable quality (or above) that should be considered. Data items
         will be considered missing
@@ -116,23 +119,21 @@
     def match(self, row):
         criteria = [
             (match_path, self.path if not self.is_regex else None),
             (match_path_regex, self.path if self.is_regex else None),
             (match_quality, self.quality_threshold),
             (match_header_vals, self.header_vals),
         ]
-        # Get all items that match the data format of the source
-        matches = row.resolved(self.format)
+        # Get all items that match the data type of the source
+        matches = row.resolved(self.datatype)
         if not matches:
-            format_str = class_location(
-                self.format, strip_prefix="arcana.data.formats."
-            )
             msg = (
-                f"Did not find any items matching data format "
-                f"{format_str} in '{row.id}' {self.row_frequency} for the "
+                f"Did not find any items matching data datatype "
+                f"{ClassResolver.tostr(self.datatype)} in '{row.id}' "
+                f"{self.row_frequency} for the "
                 f"'{self.name}' column, found unresolved items:"
             )
             for item in sorted(row.unresolved, key=attrgetter("path")):
                 msg += (
                     f"\n    {item.path}: paths="
                     + ",".join(p.name for p in item.file_paths)
                     + ((", uris=" + ",".join(item.uris.keys())) if item.uris else "")
@@ -165,28 +166,27 @@
                 "Found multiple matches " + self._error_msg(row, matches)
             )
         else:
             match = matches[0]
         return match
 
     def _error_msg(self, row, matches):
-        format_str = class_location(self.format, strip_prefix="arcana.data.formats.")
         return (
-            f" attempting to select a {format_str} item for the '{row.id}' "
-            f"{row.frequency} in the '{self.name}' column, found:"
+            f" attempting to select {ClassResolver.tostr(self.datatype)} item for "
+            f"the '{row.id}' {row.frequency} in the '{self.name}' column, found:"
             + self._format_matches(matches)
             + self._format_criteria()
         )
 
     def _format_criteria(self):
-        format_str = class_location(self.format, strip_prefix="arcana.data.formats.")
         return (
-            f"\n\n    criteria: path='{self.path}', is_regex={self.is_regex}, "
-            + f"format={format_str}, quality_threshold='{self.quality_threshold}', "
-            + f"header_vals={self.header_vals}, order={self.order}"
+            f"\n\n    criteria: {self.path}', is_regex={self.is_regex}, "
+            f"datatype={ClassResolver.tostr(self.datatype)}, "
+            f"quality_threshold='{self.quality_threshold}', "
+            f"header_vals={self.header_vals}, order={self.order}"
         )
 
     def _format_matches(self, matches):
         out_str = ""
         for match in sorted(matches, key=attrgetter("path")):
             out_str += "\n    "
             if match.order:
@@ -225,16 +225,16 @@
     processing pipeline.
 
     Parameters
     ----------
     path : str
         The path to the relative location the corresponding data items will be
         stored within the rows of the data tree.
-    format : type
-        The file format or data type used to store the corresponding items
+    datatype : type
+        The file datatype or data type used to store the corresponding items
         in the store dataset.
     row_frequency : DataSpace
         The row_frequency of the file-group within the dataset tree, e.g. per
         'session', 'subject', 'timepoint', 'group', 'dataset'
     salience : Salience
         The salience of the specified file-group, i.e. whether it would be
         typically of interest for publication outputs or whether it is just
@@ -249,18 +249,18 @@
         converter=lambda s: ColumnSalience[str(s)] if s is not None else None,
     )
     pipeline_name: str = attrs.field(default=None)
 
     is_sink = True
 
     def match(self, row):
-        matches = [i for i in row.resolved(self.format) if i.path == self.path]
+        matches = [i for i in row.resolved(self.datatype) if i.path == self.path]
         if not matches:
-            # Return a placeholder data item that can be set
-            return self.format(path=self.path, row=row, exists=False)
+            # Return a placeholder data item th.datatypebe set
+            return self.datatype(path=self.path, row=row, exists=False)
         elif len(matches) > 1:
             raise ArcanaDataMatchError(
                 "Found multiple matches " + self._error_msg(row, matches)
             )
         return matches[0]
 
     def derive(self, ids=None):
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/format.py` & `arcana-2.0b2/arcana/core/data/type/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-import os
-import os.path as op
+from __future__ import annotations
 from pathlib import Path
 import typing as ty
-from itertools import chain
 from copy import copy
 import hashlib
 import logging
-import shutil
 from abc import ABCMeta, abstractmethod
 import attrs
 from attrs.converters import optional
 from pydra.engine.core import LazyField, Workflow
-from arcana.core.utils import class_location, parse_value, func_task, path2varname
-from arcana.core.mark import CONVERTER_ANNOT
+from arcana.core.utils.misc import (
+    func_task,
+    path2varname,
+    classproperty,
+    CONVERTER_ANNOTATIONS,
+    HASH_CHUNK_SIZE,
+)
 from arcana.exceptions import (
     ArcanaUsageError,
     ArcanaNameError,
     ArcanaDataNotDerivedYetError,
     ArcanaFileFormatError,
     ArcanaFormatConversionError,
 )
-from ..enum import DataQuality
+from ...analysis.salience import DataQuality  # @ignore reshadowedImports
+
+
+if ty.TYPE_CHECKING:
+    from arcana.core.data.row import DataRow
+
+
+def absolute_path(path):
+    return Path(path).absolute()
+
+
+def absolute_paths_dict(dct):
+    return {n: absolute_path(p) for n, p in dict(dct).items()}
 
 
 logger = logging.getLogger("arcana")
 
 
 @attrs.define
-class DataItem(metaclass=ABCMeta):
+class DataType(metaclass=ABCMeta):
     """
-    A representation of a file_group within the dataset.
+    A representation of an atomic data item within a dataset. Subclassed to define
+    different data file/directory formats and fields
 
     Parameters
     ----------
     name_path : str
         The name_path to the relative location of the file group, i.e. excluding
         information about which row in the data tree it belongs to
     order : int | None
@@ -55,15 +70,17 @@
 
     path: str = attrs.field()
     uri: str = attrs.field(default=None)
     order: int = attrs.field(default=None)
     quality: DataQuality = attrs.field(default=DataQuality.usable)
     exists: bool = attrs.field(default=True)
     provenance: ty.Dict[str, ty.Any] = attrs.field(default=None)
-    row = attrs.field(default=None)
+    row: DataRow = attrs.field(default=None)
+
+    DEFAULT_PACKAGE = "arcana.data.types"
 
     @abstractmethod
     def get(self, assume_exists=False):
         """Pulls data from the store (if remote) and caches locally
 
         Parameters
         ----------
@@ -81,14 +98,25 @@
         Parameters
         ----------
         value : ty.Any
             The value to update
         """
         raise NotImplementedError
 
+    @classproperty
+    def desc(cls):
+        """Descriptive name that can be overridden in subclasses
+
+        Returns
+        -------
+        _type_
+            _description_
+        """
+        return cls.__name__.lower()
+
     @property
     def recorded_checksums(self):
         if self.provenance is None:
             return None
         else:
             return self.provenance.outputs[self.name_path]
 
@@ -116,107 +144,17 @@
                 f"Cannot 'get' {self} as it is not part of a dataset"
             )
 
     @classmethod
     def class_name(cls):
         return cls.__name__.lower()
 
-    @classmethod
-    def location(cls, relative=True):
-        """Returns the location of the format class definition
-
-        Parameters
-        ----------
-        relative : bool, optional
-            return the module location relative to `arcana.data.formats`,
-            if applicable, by default True
-
-        Returns
-        -------
-        str
-            the location of the class format in <module-path>:<class-name>
-        """
-        loc = class_location(cls)
-        if relative and loc.startswith("arcana.data.formats."):
-            loc = loc[len("arcana.data.formats.") :]
-        return loc
-
-
-@attrs.define
-class Field(DataItem):
-    """
-    A representation of a value field in the dataset.
-
-    Parameters
-    ----------
-    name_path : str
-        The name_path to the relative location of the field, i.e. excluding
-        information about which row in the data tree it belongs to
-    derived : bool
-        Whether or not the value belongs in the derived session or not
-    row : DataRow
-        The data row that the field belongs to
-    exists : bool
-        Whether the field exists or is just a placeholder for a sink
-    provenance : Provenance | None
-        The provenance for the pipeline that generated the field,
-        if applicable
-    """
-
-    value: int or float or str = attrs.field(converter=parse_value, default=None)
-
-    def get(self, assume_exists=False):
-        if not assume_exists:
-            self._check_exists()
-        self._check_part_of_row()
-        self.value = self.row.dataset.store.get_field_value(self)
-
-    def put(self, value):
-        self._check_part_of_row()
-        self.row.dataset.store.put_field_value(self, self.format(value))
-        self.exists = True
-
-    def __int__(self):
-        return int(self.value)
-
-    def __float__(self):
-        return float(self.value)
-
-    def __str__(self):
-        if self.format.__args__:  # Sequence type
-            val = "[" + ",".join(self._to_str(v) for v in self.value) + "]"
-        else:
-            val = self._to_str(self.value)
-        return val
-
-    def _to_str(self, val):
-        if self.format is str:
-            val = '"{}"'.format(val)
-        else:
-            val = str(val)
-        return val
-
-    def get_checksums(self):
-        """
-        For duck-typing with file_groups in checksum management. Instead of a
-        checksum, just the value of the field is used
-        """
-        return self.value
-
-
-def absolute_path(path):
-    return Path(path).absolute()
-
-
-def absolute_paths_dict(dct):
-    return {n: absolute_path(p) for n, p in dict(dct).items()}
-
 
 @attrs.define
-class FileGroup(DataItem, metaclass=ABCMeta):
+class FileGroup(DataType, metaclass=ABCMeta):
     """
     A representation of a file_group within the dataset.
 
     Parameters
     ----------
     name_path : str
         The name_path to the relative location of the file group, i.e. excluding
@@ -242,22 +180,22 @@
         Additional files in the file_group. Keys should match corresponding
         side_cars dictionary in format.
     checksums : ty.Dict[str, str]
         A checksums of all files within the file_group in a dictionary sorted
         bys relative file name_paths
     """
 
+    ext = None  # to be overridden by file-format specific classes
+
     fs_path: str = attrs.field(default=None, converter=optional(absolute_path))
     _checksums: ty.Dict[str, str] = attrs.field(default=None, repr=False, init=False)
     # Alternative names for the file format, empty by default overridden in
     # sub-classes where necessary
     alternative_names = ()
 
-    HASH_CHUNK_SIZE = 2**20  # 1MB in calc. checksums to avoid mem. issues
-
     @fs_path.validator
     def validate_fs_path(self, _, fs_path):
         if fs_path is not None:
             if not fs_path.exists:
                 raise ArcanaUsageError(
                     "Attempting to set a path that doesn't exist " f"({fs_path})"
                 )
@@ -268,14 +206,15 @@
                 )
 
     def get(self, assume_exists=False):
         if assume_exists:
             self.exists = True
         self._check_part_of_row()
         fs_paths = self.row.dataset.store.get_file_group_paths(self)
+        self.exists = True
         self.set_fs_paths(fs_paths)
         self.validate_file_paths()
 
     def put(self, *fs_paths):
         self._check_part_of_row()
         fs_paths = [Path(p) for p in fs_paths]
         dir_paths = list(p for p in fs_paths if p.is_dir())
@@ -284,20 +223,21 @@
             raise ArcanaFileFormatError(
                 f"Cannot put more than one directory, {dir_paths_str}, as part "
                 f"of the same file group {self}"
             )
         # Make a copy of the file-group to validate the local paths and auto-gen
         # any defaults before they are pushed to the store
         cpy = copy(self)
+        cpy.exists = True
         cpy.set_fs_paths(fs_paths)
         cache_paths = self.row.dataset.store.put_file_group_paths(self, cpy.fs_paths)
         # Set the paths to the cached files
+        self.exists = True
         self.set_fs_paths(cache_paths)
         self.validate_file_paths()
-        self.exists = True
         # Save provenance
         if self.provenance:
             self.row.dataset.store.put_provenance(self)
 
     @property
     def fs_paths(self):
         """All base paths (i.e. not nested within directories) in the file group"""
@@ -329,15 +269,15 @@
         ----------
         name : str
             Name to match
 
         Returns
         -------
         bool
-            whether or not the name matches the format
+            whether or not the name matches the datatype
         """
         return name.lower() in [
             n.lower() for n in (cls.class_name(),) + cls.alternative_names
         ]
 
     @property
     def value(self):
@@ -362,15 +302,15 @@
         self._check_exists()
         checksums = {}
         for fpath in self.all_file_paths():
             fhash = hashlib.md5()
             with open(fpath, "rb") as f:
                 # Calculate hash in chunks so we don't run out of memory for
                 # large files.
-                for chunk in iter(lambda: f.read(self.HASH_CHUNK_SIZE), b""):
+                for chunk in iter(lambda: f.read(HASH_CHUNK_SIZE), b""):
                     fhash.update(chunk)
             checksums[fpath] = fhash.hexdigest()
         checksums = self.generalise_checksum_keys(checksums)
         return checksums
 
     def contents_equal(self, other, **kwargs):
         """
@@ -386,45 +326,45 @@
         """
         self._check_exists()
         other._check_exists()
         return self.checksums[self.fs_path.name] == other.checksums[other.fs_path.name]
 
     @classmethod
     def resolve(cls, unresolved):
-        """Resolve file group loaded from a repository to the specific format
+        """Resolve file group loaded from a repository to the specific datatype
 
         Parameters
         ----------
         unresolved : UnresolvedFileGroup
             A file group loaded from a repository that has not been resolved to
-            a specific format yet
+            a specific datatype yet
 
         Returns
         -------
         FileGroup
             The resolved file-group object
 
         Raises
         ------
         ArcanaUnresolvableFormatException
             If there doesn't exist a unique resolution from the unresolved file
-            group to the given format, then an ArcanaFileFormatError should be
+            group to the given datatype, then an ArcanaFileFormatError should be
             raised
         """
-        # Perform matching based on resource names in multi-format
+        # Perform matching based on resource names in multi-datatype
         # file-group
         if unresolved.uris is not None:
             item = None
             for format_name, uri in unresolved.uris.items():
                 if cls.matches_format_name(format_name):
                     item = cls(uri=uri, **unresolved.item_kwargs)
             if item is None:
                 raise ArcanaFileFormatError(
                     f"Could not file a matching resource in {unresolved.path} for"
-                    f" the given format ({cls.class_name()}), found "
+                    f" the given datatype ({cls.class_name()}), found "
                     "('{}')".format("', '".join(unresolved.uris))
                 )
         else:
             item = cls(**unresolved.item_kwargs)
             item.set_fs_paths(unresolved.file_paths)
         return item
 
@@ -489,27 +429,30 @@
 
         Raises
         ------
         ArcanaFileFormatError
             When no paths match or more than one path matches the given extension"""
         if ext is None:
             ext = cls.ext
-        matches = [str(p) for p in paths if str(p).endswith("." + ext)]
+        if ext:
+            matches = [str(p) for p in paths if str(p).endswith("." + ext)]
+        else:
+            matches = paths
         if not matches:
             paths_str = ", ".join(str(p) for p in paths)
             raise ArcanaFileFormatError(
                 f"No matching files with '{ext}' extension found in "
                 f"file group {paths_str}"
             )
         elif len(matches) > 1:
-            matches_str = ", ".join(matches)
+            matches_str = ", ".join(str(p) for p in matches)
             raise ArcanaFileFormatError(
                 f"Multiple files with '{ext}' extension found in : {matches_str}"
             )
-        return matches[0]
+        return str(matches[0])
 
     def validate_file_paths(self):
         attrs.validate(self)
         self.exists = True
 
     def _check_paths_exist(self, fs_paths: ty.List[Path]):
         if missing := [p for p in fs_paths if not p or not Path(p).exists()]:
@@ -525,20 +468,20 @@
                         msg += (
                             f"\n\nFiles in the directory '{str(fs_path.parent)}' are:\n"
                         )
                         msg += "\n".join(str(p) for p in fs_path.parent.iterdir())
             raise ArcanaFileFormatError(msg)
 
     def convert_to(self, to_format, **kwargs):
-        """Convert the FileGroup to a new format
+        """Convert the FileGroup to a new datatype
 
         Parameters
         ----------
         to_format : type
-            the file-group format to convert to
+            the file-group datatype to convert to
         **kwargs
             args to pass to the conversion process
 
         Returns
         -------
         FileGroup
             the converted file-group
@@ -574,15 +517,15 @@
         wf = Workflow(name=name, input_spec=["to_convert"])
 
         # Get row to extract paths from file-group lazy field
         wf.add(
             func_task(
                 access_paths,
                 in_fields=[("from_format", type), ("file_group", from_format)],
-                out_fields=[(i, str) for i in from_format.fs_names()],
+                out_fields=[(i, Path) for i in from_format.fs_names()],
                 # name='extract',
                 from_format=from_format,
                 file_group=wf.lzin.to_convert,
             )
         )
 
         # Aggregate converter inputs and combine with fixed keyword args
@@ -606,75 +549,80 @@
 
         logger.debug("Paths to encapsulate are:\n%s", to_encapsulate)
 
         wf.add(
             func_task(
                 encapsulate_paths,
                 in_fields=[("to_format", type), ("to_convert", from_format)]
-                + [(o, str) for o in cls.fs_names()],
+                + [(o, ty.Union[str, Path]) for o in cls.fs_names()],
                 out_fields=[("converted", cls)],
                 # name='encapsulate',
                 to_format=cls,
                 to_convert=wf.lzin.to_convert,
                 **to_encapsulate,
             )
         )
 
         wf.set_output(("converted", wf.encapsulate_paths.lzout.converted))
 
         return wf
 
     @classmethod
     def find_converter(cls, from_format):
-        """Selects the converter method from the given format. Will select the
+        """Selects the converter method from the given datatype. Will select the
         most specific conversion.
 
         Parameters
         ----------
         from_format : type
-            The format type to convert from
+            The datatype type to convert from
 
         Returns
         -------
-        function
-            The bound method that adds rows to a given workflow
+        function or NoneType
+            The bound method that adds rows to a given workflow if conversion is required
+            and None if no conversion is required
 
         Raises
         ------
         ArcanaFormatConversionError
             _description_
         """
+        if from_format is cls or issubclass(from_format, cls):
+            return None  # No conversion is required
         converter = None
         for attr_name in dir(cls):
             meth = getattr(cls, attr_name)
             try:
-                converts_from = meth.__annotations__[CONVERTER_ANNOT]
+                converts_from = meth.__annotations__[CONVERTER_ANNOTATIONS]
             except (AttributeError, KeyError):
                 pass
             else:
                 if from_format is converts_from or issubclass(
                     from_format, converts_from
                 ):
                     if converter:
-                        prev_converts_from = converter.__annotations__[CONVERTER_ANNOT]
+                        prev_converts_from = converter.__annotations__[
+                            CONVERTER_ANNOTATIONS
+                        ]
                         if issubclass(converts_from, prev_converts_from):
                             converter = meth
                         elif not issubclass(prev_converts_from, converts_from):
                             raise ArcanaFormatConversionError(
                                 f"Ambiguous converters between {from_format} "
                                 f"and {cls}: {converter} and {meth}. Please "
                                 f"define a specific converter from {from_format} "
                                 f"(i.e. instead of from {prev_converts_from} "
                                 f"and {converts_from} respectively)"
                             )
                     else:
                         converter = meth
-        if not converter:
+        if converter is None:
             raise ArcanaFormatConversionError(
-                f"No converters defined between {from_format} and {cls}"
+                f"No datatype converters are defined from {from_format} to {cls}"
             )
         return converter
 
     def generalise_checksum_keys(
         self, checksums: ty.Dict[str, str], base_path: Path = None
     ):
         """Generalises the paths used for the file paths in a checksum dictionary
@@ -737,355 +685,66 @@
     )
     file_group = to_format(to_convert.path + "_" + to_format.class_name())
     file_group.set_fs_paths(fs_paths.values())
     return file_group
 
 
 @attrs.define
-class BaseFile(FileGroup):
-
-    is_dir = False
-
-    def set_fs_paths(self, fs_paths: ty.List[Path]):
-        self._check_paths_exist(fs_paths)
-        self.fs_path = absolute_path(self.matches_ext(*fs_paths))
-
-    def all_file_paths(self):
-        """The paths of all nested files within the file-group"""
-        if self.fs_path is None:
-            raise ArcanaUsageError(
-                f"Attempting to access file paths of {self} before they are set"
-            )
-        return self.fs_paths
-
-    def copy_to(self, fs_path: str or Path, symlink: bool = False):
-        """Copies the file-group to the new path, with auxiliary files saved
-        alongside the primary-file path.
-
-        Parameters
-        ----------
-        path : str
-            Path to save the file-group to excluding file extensions
-        symlink : bool
-            Use symbolic links instead of copying files to new location
-
-        Returns
-        -------
-        BaseFile
-            A copy of the file object at the new file system path
-        """
-        if symlink:
-            copy_file = os.symlink
-        else:
-            copy_file = shutil.copyfile
-        dest_path = Path(str(fs_path) + "." + self.ext)
-        copy_file(self.fs_path, dest_path)
-        cpy = copy(self)
-        cpy.set_fs_paths([dest_path])
-        return cpy
-
-    @classmethod
-    def copy_ext(cls, old_path, new_path):
-        """Copy extension from the old path to the new path, ensuring that all
-        of the extension is used (e.g. 'nii.gz' instead of 'gz')
-
-        Parameters
-        ----------
-        old_path: Path or str
-            The path from which to copy the extension from
-        new_path: Path or str
-            The path to append the extension to
-
-        Returns
-        -------
-        Path
-            The new path with the copied extension
-        """
-        if not cls.matches_ext(old_path):
-            raise ArcanaFileFormatError(
-                f"Extension of old path ('{str(old_path)}') does not match that "
-                f"of file, '{cls.ext}'"
-            )
-        return Path(new_path).with_suffix("." + cls.ext)
-
-    @classmethod
-    def all_exts(cls):
-        return [cls.ext]
-
-
-@attrs.define
-class WithSideCars(BaseFile):
-    """Base class for file-groups with a primary file and several header or
-    side car files
+class Field(DataType):
     """
+    A representation of a value field in the dataset.
 
-    side_cars: ty.Dict[str, str] = attrs.field(converter=optional(absolute_paths_dict))
-
-    @side_cars.default
-    def default_side_cars(self):
-        if self.fs_path is None:
-            return {}
-        return self.default_side_car_paths(self.fs_path)
-
-    @side_cars.validator
-    def validate_side_cars(self, _, side_cars):
-        if side_cars is not None:
-            if self.fs_path is None:
-                raise ArcanaUsageError(
-                    "Auxiliary files can only be provided to a FileGroup "
-                    f"of '{self.path}' ({side_cars}) if the local path is "
-                    "as well"
-                )
-            if set(self.side_car_exts) != set(side_cars.keys()):
-                raise ArcanaUsageError(
-                    "Keys of provided auxiliary files ('{}') don't match "
-                    "format ('{}')".format(
-                        "', '".join(side_cars.keys()), "', '".join(self.side_car_exts)
-                    )
-                )
-            missing_side_cars = [f for f in side_cars.values() if not op.exists(f)]
-            if missing_side_cars:
-                raise ArcanaUsageError(
-                    f"Attempting to set paths of auxiliary files for {self} "
-                    "that don't exist ('{}')".format("', '".join(missing_side_cars))
-                )
-
-    @classmethod
-    def fs_names(cls):
-        """Return names for each top-level file-system path in the file group,
-        used when generating Pydra task interfaces.
+    Parameters
+    ----------
+    name_path : str
+        The name_path to the relative location of the field, i.e. excluding
+        information about which row in the data tree it belongs to
+    derived : bool
+        Whether or not the value belongs in the derived session or not
+    row : DataRow
+        The data row that the field belongs to
+    exists : bool
+        Whether the field exists or is just a placeholder for a sink
+    provenance : Provenance | None
+        The provenance for the pipeline that generated the field,
+        if applicable
+    """
 
-        Returns
-        -------
-        tuple[str]
-            sequence of names for top-level file-system paths in the file group"""
-        return super().fs_names() + cls.side_car_exts
+    value: ty.Any = None
 
-    def set_fs_paths(self, paths: ty.List[Path]):
-        super().set_fs_paths(paths)
-        to_assign = set(Path(p) for p in paths)
-        to_assign.remove(self.fs_path)
-        # Begin with default side_car paths and override if provided
-        self.side_cars = self.default_side_car_paths(self.fs_path)
-        for sc_ext in self.side_car_exts:
-            try:
-                matched = self.side_cars[sc_ext] = absolute_path(
-                    self.matches_ext(*paths, ext=sc_ext)
-                )
-            except ArcanaFileFormatError:
-                pass  # fallback to default
-            else:
-                to_assign.remove(matched)
+    def get(self, assume_exists=False):
+        if not assume_exists:
+            self._check_exists()
+        self._check_part_of_row()
+        self.value = self.row.dataset.store.get_field_value(self)
 
-    @property
-    def fs_paths(self):
-        return chain(super().fs_paths, self.side_cars.values())
+    def put(self, value):
+        self._check_part_of_row()
+        self.row.dataset.store.put_field_value(self, self.format(value))
+        self.exists = True
 
-    def side_car(self, name):
-        return self.side_cars[name]
+    def __int__(self):
+        return int(self.value)
 
-    def copy_to(self, fs_path: str or Path, symlink: bool = False):
-        """Copies the file-group to the new path, with auxiliary files saved
-        alongside the primary-file path.
+    def __float__(self):
+        return float(self.value)
 
-        Parameters
-        ----------
-        fs_path : str or Path
-            Path to save the file-group to excluding file extensions
-        symlink : bool
-            Use symbolic links instead of copying files to new location
-        """
-        if symlink:
-            copy_file = os.symlink
+    def __str__(self):
+        if self.datatype.__args__:  # Sequence type
+            val = "[" + ",".join(self._to_str(v) for v in self.value) + "]"
         else:
-            copy_file = shutil.copyfile
-        dest_path = Path(str(fs_path) + "." + self.ext)
-        copy_file(self.fs_path, dest_path)
-        dest_side_cars = self.default_side_car_paths(dest_path)
-        for sc_ext, sc_path in self.side_cars.items():
-            copy_file(sc_path, dest_side_cars[sc_ext])
-        cpy = copy(self)
-        cpy.set_fs_paths([dest_path] + list(dest_side_cars.values()))
-        return cpy
-
-    @classmethod
-    def default_side_car_paths(cls, primary_path):
-        """
-        Get the default paths for auxiliary files relative to the path of the
-        primary file, i.e. the same name as the primary path with a different
-        extension
-
-        Parameters
-        ----------
-        primary_path : str
-            Path to the primary file in the file_group
-
-        Returns
-        -------
-        aux_paths : ty.Dict[str, str]
-            A dictionary of auxiliary file names and default paths
-        """
-
-        return {
-            e: Path(str(primary_path)[: -len(cls.ext)] + e) for e in cls.side_car_exts
-        }
-
-    @classmethod
-    def copy_ext(cls, old_path, new_path):
-        """Copy extension from the old path to the new path, ensuring that all
-        of the extension is used (e.g. 'nii.gz' instead of 'gz'). If the old
-        path extension doesn't match the primary path, the methods loops through
-        all side-car extensions and selects the longest matching.
+            val = self._to_str(self.value)
+        return val
 
-        Parameters
-        ----------
-        old_path: Path or str
-            The path from which to copy the extension from
-        new_path: Path or str
-            The path to append the extension to
+    def _to_str(self, val):
+        if self.datatype is str:
+            val = '"{}"'.format(val)
+        else:
+            val = str(val)
+        return val
 
-        Returns
-        -------
-        Path
-            The new path with the copied extension
+    def get_checksums(self):
         """
-        try:
-            # Check to see if the path it matches the primary path extension
-            return super().copy_ext(old_path, new_path)
-        except ArcanaFileFormatError:
-            pass
-        matches = []
-        for ext in cls.side_car_exts:
-            try:
-                cls.matches_ext(old_path, ext=ext)
-            except ArcanaFileFormatError:
-                pass
-            else:
-                matches.append(ext)
-        if not matches:
-            sc_exts_str = "', '".join(cls.side_car_exts)
-            raise ArcanaFileFormatError(
-                f"Extension of old path ('{str(old_path)}') does not match any "
-                f" in {cls}: '{cls.ext}', {sc_exts_str}"
-            )
-        longest_match = max(matches, key=len)
-        return Path(new_path).with_suffix("." + longest_match)
-
-    def generalise_checksum_keys(
-        self, checksums: ty.Dict[str, str], base_path: Path = None
-    ):
-        """Generalises the paths used for the file paths in a checksum dictionary
-        so that they are the same irrespective of that the top-level file-system
-        paths are
-
-        Parameters
-        ----------
-        checksums: dict[str, str]
-            The checksum dict mapping relative file paths to checksums
-
-        Returns
-        -------
-        dict[str, str]
-            The checksum dict with file paths generalised"""
-        if base_path is None:
-            base_path = self.fs_path
-        generalised = {}
-        fs_name_dict = {
-            self.matches_ext(*checksums.keys(), ext=e): e for e in self.side_car_exts
-        }
-        mapped_exts = list(fs_name_dict.values())
-        duplicates = set([e for e in mapped_exts if mapped_exts.count(e) > 1])
-        if duplicates:
-            raise ArcanaUsageError(
-                f"Multiple files with same extensions found in {self}: "
-                + ", ".join(str(k) for k in checksums.keys())
-            )
-        for key, chksum in checksums.items():
-            try:
-                rel_key = fs_name_dict[str(key)]
-            except KeyError:
-                try:
-                    rel_key = Path(key).relative_to(base_path)
-                except ValueError:
-                    continue  # skip these files
-            generalised[str(rel_key)] = chksum
-        return generalised
-
-    @classmethod
-    def all_exts(cls):
-        return [cls.ext] + list(cls.side_car_exts)
-
-
-@attrs.define
-class BaseDirectory(FileGroup):
-
-    is_dir = True
-    content_types = ()  # By default, don't check contents for any types
-
-    def set_fs_paths(self, fs_paths: ty.List[Path]):
-        self._check_paths_exist(fs_paths)
-        matches = [p for p in fs_paths if Path(p).is_dir() and self.contents_match(p)]
-        types_str = ", ".join(t.__name__ for t in self.content_types)
-        if not matches:
-            raise ArcanaFileFormatError(
-                f"No matching directories with contents matching {types_str}"
-            )
-        elif len(matches) > 1:
-            matches_str = ", ".join(str(m) for m in matches)
-            raise ArcanaFileFormatError(
-                f"Multiple directories with contents matching {types_str}: "
-                f"{matches_str}"
-            )
-        self.fs_path = absolute_path(matches[0])
-
-    @classmethod
-    def contents_match(cls, path: Path):
-        from arcana.core.data.row import UnresolvedFileGroup
-
-        path = Path(path)  # Ensure a Path object not a string
-        contents = UnresolvedFileGroup.from_paths(path, path.iterdir())
-        for content_type in cls.content_types:
-            resolved = False
-            for unresolved in contents:
-                try:
-                    content_type.resolve(unresolved)
-                except ArcanaFileFormatError:
-                    pass
-                else:
-                    resolved = True
-                    break
-            if not resolved:
-                return False
-        return True
-
-    def all_file_paths(self):
-        "Iterates through all files in the group and returns their file paths"
-        if self.fs_path is None:
-            raise ArcanaUsageError(
-                f"Attempting to access file paths of {self} before they are set"
-            )
-        return chain(
-            *(
-                (Path(root) / f for f in files)
-                for root, _, files in os.walk(self.fs_path)
-            )
-        )
-
-    def copy_to(self, fs_path: str, symlink: bool = False):
-        """Copies the file-group to the new path, with auxiliary files saved
-        alongside the primary-file path.
-
-        Parameters
-        ----------
-        fs_path : str
-            Path to save the file-group to excluding file extensions
-        symlink : bool
-            Use symbolic links instead of copying files to new location
+        For duck-typing with file_groups in checksum management. Instead of a
+        checksum, just the value of the field is used
         """
-        if symlink:
-            copy_dir = os.symlink
-        else:
-            copy_dir = shutil.copytree
-        copy_dir(self.fs_path, fs_path)
-        cpy = copy(self)
-        cpy.set_fs_paths([fs_path])
-        return cpy
+        return self.value
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/row.py` & `arcana-2.0b2/arcana/core/data/row.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from abc import ABCMeta
 import arcana.core.data.set
 from arcana.exceptions import (
     ArcanaNameError,
     ArcanaWrongFrequencyError,
     ArcanaFileFormatError,
 )
-from .format import DataItem
-from ..enum import DataQuality
+from .type.base import DataType
+from ..analysis.salience import DataQuality
 from .space import DataSpace
 
 
 @attrs.define(auto_detect=True)
 class DataRow:
     """A "row" in a dataset "frame" where file-groups and fields can be placed, e.g.
     a session or subject.
@@ -46,15 +46,15 @@
         Parameters
         ----------
         column_name : str
             Name of a selected column in the dataset
 
         Returns
         -------
-        DataItem
+        DataType
             The item matching the provided name specified by the column name
         """
         if column_name in self._items:
             return self._items[column_name]
         else:
             try:
                 spec = self.dataset[column_name]
@@ -116,15 +116,15 @@
         Parameters
         ----------
         column_name : str
             Name of a selected column in the dataset
 
         Returns
         -------
-        Sequence[DataItem]
+        Sequence[DataType]
             The item matching the provided name specified by the column name
             if the column is of matching or ancestor frequency, or list of
             items if a descendent or unrelated frequency.
         """
         try:
             return [self[column_name]]
         except ArcanaWrongFrequencyError:
@@ -140,27 +140,27 @@
     @property
     def unresolved(self):
         if self._unresolved is None:
             self._unresolved = []
             self.dataset.store.find_items(self)
         return self._unresolved
 
-    def resolved(self, format):
+    def resolved(self, datatype):
         """
-        Items in the row that are able to be resolved to the given format
+        Items in the row that are able to be resolved to the given datatype
 
         Parameters
         ----------
-        format : type
-            The file format or type to reolve the item to
+        datatype : type
+            The file datatype or type to reolve the item to
         """
         matches = []
         for potential in self.unresolved:
             try:
-                matches.append(format.resolve(potential))
+                matches.append(datatype.resolve(potential))
             except ArcanaFileFormatError:
                 pass
         return matches
 
     @property
     def ids_tuple(self):
         return self.dataset.ids_tuple(self.ids)
@@ -175,15 +175,15 @@
             self._unresolved = []
         self._unresolved.append(
             UnresolvedField(path=path, row=self, value=value, **kwargs)
         )
 
 
 @attrs.define
-class UnresolvedDataItem(metaclass=ABCMeta):
+class UnresolvedDataType(metaclass=ABCMeta):
     """A file-group stored in, potentially multiple, unknown file formats.
     File formats are resolved by providing a list of candidates to the
     'resolve' method
 
     Parameters
     ----------
     path : str
@@ -202,15 +202,15 @@
     """
 
     path: str = attrs.field(default=None)
     row: DataRow = attrs.field(default=None)
     order: int = attrs.field(default=None)
     quality: DataQuality = attrs.field(default=DataQuality.usable)
     provenance: ty.Dict[str, ty.Any] = attrs.field(default=None)
-    _matched: ty.Dict[str, DataItem] = attrs.field(factory=dict, init=False)
+    _matched: ty.Dict[str, DataType] = attrs.field(factory=dict, init=False)
 
     @property
     def item_kwargs(self):
         return {
             "path": self.path,
             "order": self.order,
             "row": self.row,
@@ -222,15 +222,15 @@
     "Convert all file paths to absolute real paths"
     if file_paths:
         file_paths = [Path(p).absolute() for p in file_paths]
     return file_paths
 
 
 @attrs.define
-class UnresolvedFileGroup(UnresolvedDataItem):
+class UnresolvedFileGroup(UnresolvedDataType):
     """A file-group stored in, potentially multiple, unknown file formats.
     File formats are resolved by providing a list of candidates to the
     'resolve' method
 
     Parameters
     ----------
     name_path : str
@@ -247,17 +247,17 @@
         The provenance for the pipeline that generated the file-group,
         if applicable
     row : DataRow
         The data row that the field belongs to
     file_paths : Sequence[str] | None
         Path to the file-group in the local cache
     uris : Dict[str, str] | None
-        For stores where the name of the file format is saved with the
+        For stores where the name of the file datatype is saved with the
         data (i.e. XNAT), the name of the resource enables straightforward
-        format identification. It is stored here along with URIs corresponding
+        datatype identification. It is stored here along with URIs corresponding
         to each resource
     """
 
     file_paths: ty.Sequence[Path] = attrs.field(factory=list, converter=normalise_paths)
     uris: ty.Dict[str] = attrs.field(default=None)
 
     @classmethod
@@ -270,15 +270,15 @@
             # Add all possible stems
             for i in range(len(relpath.suffixes)):
                 groups["".join([path_stem] + relpath.suffixes[: (i + 1)])].append(path)
         return [cls(path=p, file_paths=g, **kwargs) for p, g in groups.items()]
 
 
 @attrs.define
-class UnresolvedField(UnresolvedDataItem):
+class UnresolvedField(UnresolvedDataType):
     """A file-group stored in, potentially multiple, unknown file formats.
     File formats are resolved by providing a list of candidates to the
     'resolve' method
 
     Parameters
     ----------
     path : str
@@ -301,26 +301,26 @@
         The data row that the field belongs to
     """
 
     value: ty.Union[
         float, int, str, ty.List[float], ty.List[int], ty.List[str]
     ] = attrs.field(default=None)
 
-    # def _resolve(self, format):
+    # def _resolve(self, datatype):
     #     try:
-    #         if format._name == 'Sequence':
-    #             if len(format.__args__) > 1:
+    #         if datatype._name == 'Sequence':
+    #             if len(datatype.__args__) > 1:
     #                 raise ArcanaUsageError(
     #                     f"Sequence formats with more than one arg "
-    #                     "are not supported ({format})")
-    #             subtype = format.__args__[0]
+    #                     "are not supported ({datatype})")
+    #             subtype = datatype.__args__[0]
     #             value = [subtype(v)
     #                         for v in self.value[1:-1].split(',')]
     #         else:
-    #             value = format(self.value)
+    #             value = datatype(self.value)
     #     except ValueError as e:
     #         raise ArcanaUnresolvableFormatException(
     #                 f"Could not convert value of {self} ({self.value}) "
-    #                 f"to format {format}") from e
+    #                 f"to datatype {datatype}") from e
     #     else:
-    #         item = DataItem(value=value, **self.item_kwargs)
+    #         item = DataType(value=value, **self.item_kwargs)
     #     return item
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/set.py` & `arcana-2.0b2/arcana/core/data/set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 import logging
 import typing as ty
 from pathlib import Path
 from itertools import chain
 import re
+import shutil
 import attrs
 import attrs.filters
 from attrs.converters import default_if_none
+from arcana.core.utils.serialize import asdict
 from arcana.exceptions import (
+    ArcanaLicenseNotFoundError,
     ArcanaNameError,
     ArcanaDataTreeConstructionError,
     ArcanaUsageError,
     ArcanaBadlyFormattedIDError,
     ArcanaWrongDataSpaceError,
 )
-from arcana.core.utils import asdict
 from .space import DataSpace
 from .column import DataColumn, DataSink, DataSource
 from . import store as datastore
-
 from .row import DataRow
 
+if ty.TYPE_CHECKING:
+    from ..deploy.image.components import License
 
 logger = logging.getLogger("arcana")
 
 
 @attrs.define
 class Dataset:
     """
@@ -105,16 +108,19 @@
     workflows : Dict[str, pydra.Workflow]
         Workflows that have been applied to the dataset to generate sink
     access_args: ty.Dict[str, Any]
         Repository specific args used to control the way the dataset is accessed
     """
 
     DEFAULT_NAME = "default"
+    LICENSES_PATH = (
+        "LICENSES"  # The resource that project-specifc licenses are expected
+    )
 
-    id: str = attrs.field(converter=str)
+    id: str = attrs.field(converter=str, metadata={"asdict": False})
     store: datastore.DataStore = attrs.field()
     hierarchy: ty.List[DataSpace] = attrs.field()
     space: DataSpace = attrs.field(default=None)
     id_inference: ty.List[ty.Tuple[DataSpace, str]] = attrs.field(
         factory=dict, converter=default_if_none(factory=dict)
     )
     include: ty.List[ty.Tuple[DataSpace, str or list[str]]] = attrs.field(
@@ -170,16 +176,15 @@
     ):
         """Loads a dataset from an store/ID/name string, as used in the CLI
 
         Parameters
         ----------
         id: str
             either the ID of a dataset if `store` keyword arg is provided or a
-            "dataset ID string" in the format
-            <STORE-NICKNAME>//<DATASET-ID>:<DATASET-NAME>
+            "dataset ID string" in the format <store-nickname>//<dataset-id>[@<dataset-name>]
         store: DataStore, optional
             the store to load the dataset. If not provided the provided ID
             is interpreted as an ID string
         name: str, optional
             the name of the dataset within the project/directory
             (e.g. 'test', 'training'). Used to specify a subset of data rows
             to work with, within a greater project
@@ -206,32 +211,30 @@
             raise ArcanaUsageError(
                 f"Data hierarchy of {wrong_freq} column specs do(es) not match"
                 f" that of dataset {self.space}"
             )
 
     @exclude.validator
     def exclude_validator(self, _, exclude):
-        both = [
-            f
-            for f in self.include
-            if (self.include[f] is not None and exclude[f] is not None)
-        ]
+        include_freqs = set(f for f, i in self.include if i is not None)
+        exclude_freqs = set(f for f, i in exclude if i is not None)
+        both = include_freqs & exclude_freqs
         if both:
             raise ArcanaUsageError(
                 "Cannot provide both 'include' and 'exclude' arguments "
                 "for frequencies ('{}') to Dataset".format("', '".join(both))
             )
 
     @hierarchy.validator
     def hierarchy_validator(self, _, hierarchy):
         if not hierarchy:
             raise ArcanaUsageError(f"hierarchy provided to {self} cannot be empty")
 
-        not_valid = [f for f in hierarchy if f not in self.space.__members__]
         space = type(hierarchy[0]) if self.space is None else self.space
+        not_valid = [f for f in hierarchy if f not in self.space.__members__]
         if space is str:
             raise ArcanaUsageError(
                 "Either the data space of the set needs to be provided "
                 "separately, or the hierarchy must be provided as members of "
                 "a single data space, not strings"
             )
         try:
@@ -242,15 +245,15 @@
                     ", ".join(not_valid), self.space
                 )
             )
         # Check that all data frequencies are "covered" by the hierarchy and
         # each subsequent
         covered = self.space(0)
         for i, layer in enumerate(hierarchy):
-            diff = layer - covered
+            diff = (layer ^ covered) & layer
             if not diff:
                 raise ArcanaUsageError(
                     f"{layer} does not add any additional basis layers to "
                     f"previous layers {hierarchy[i:]}"
                 )
             covered |= layer
         if covered != max(self.space):
@@ -299,68 +302,68 @@
         self._root = DataRow({self.root_freq: None}, self.root_freq, self)
 
     def refresh(self):
         """Refresh the dataset rows"""
         self._root = None
 
     def add_source(
-        self, name, format, path=None, row_frequency=None, overwrite=False, **kwargs
+        self, name, datatype, path=None, row_frequency=None, overwrite=False, **kwargs
     ):
         """Specify a data source in the dataset, which can then be referenced
         when connecting workflow inputs.
 
         Parameters
         ----------
         name : str
             The name used to reference the dataset "column" for the
             source
-        format : type
-            The file-format (for file-groups) or format (for fields)
+        datatype : type
+            The file-format (for file-groups) or datatype (for fields)
             that the source will be stored in within the dataset
         path : str, default `name`
             The location of the source within the dataset
         row_frequency : DataSpace, default self.leaf_freq
             The row_frequency of the source within the dataset
         overwrite : bool
             Whether to overwrite existing columns
         **kwargs : ty.Dict[str, Any]
             Additional kwargs to pass to DataSource.__init__
         """
         row_frequency = self._parse_freq(row_frequency)
         if path is None:
             path = name
-        source = DataSource(name, path, format, row_frequency, dataset=self, **kwargs)
+        source = DataSource(name, path, datatype, row_frequency, dataset=self, **kwargs)
         self._add_spec(name, source, overwrite)
         return source
 
     def add_sink(
-        self, name, format, path=None, row_frequency=None, overwrite=False, **kwargs
+        self, name, datatype, path=None, row_frequency=None, overwrite=False, **kwargs
     ):
         """Specify a data source in the dataset, which can then be referenced
         when connecting workflow inputs.
 
         Parameters
         ----------
         name : str
             The name used to reference the dataset "column" for the
             sink
-        format : type
-            The file-format (for file-groups) or format (for fields)
+        datatype : type
+            The file-format (for file-groups) or datatype (for fields)
             that the sink will be stored in within the dataset
         path : str, default `name`
             The location of the sink within the dataset
         row_frequency : DataSpace, default self.leaf_freq
             The row_frequency of the sink within the dataset
         overwrite : bool
             Whether to overwrite an existing sink
         """
         row_frequency = self._parse_freq(row_frequency)
         if path is None:
             path = name
-        sink = DataSink(name, path, format, row_frequency, dataset=self, **kwargs)
+        sink = DataSink(name, path, datatype, row_frequency, dataset=self, **kwargs)
         self._add_spec(name, sink, overwrite)
         return sink
 
     def _add_spec(self, name, spec, overwrite):
         if name in self.columns:
             if overwrite:
                 logger.info(
@@ -566,15 +569,15 @@
                 for regex in regexes:
                     match = re.match(regex, label)
                     if match is None:
                         raise ArcanaBadlyFormattedIDError(
                             f"{layer} label '{label}', does not match ID inference"
                             f" pattern '{regex}'"
                         )
-                    new_freqs = layer - (layer & row_frequency)
+                    new_freqs = (layer ^ row_frequency) & layer
                     for target_freq, target_id in match.groupdict().items():
                         target_freq = self.space[target_freq]
                         if (target_freq & new_freqs) != target_freq:
                             raise ArcanaUsageError(
                                 f"Inferred ID target, {target_freq}, is not a "
                                 f"data row_frequency added by layer {layer}"
                             )
@@ -627,16 +630,18 @@
                 f"ID clash ({row.id}) between rows inserted into data " "tree"
             )
         row_dict[row.id] = row
         # Insert root row
         # Insert parent rows if not already present and link them with
         # inserted row
         for parent_freq, parent_id in row.ids.items():
-            diff_freq = row.frequency - (parent_freq & row.frequency)
-            if diff_freq and parent_freq:  # Don't need to insert root row again
+            if not parent_freq:
+                continue  # Don't need to insert root row again
+            diff_freq = (row.frequency ^ parent_freq) & row.frequency
+            if diff_freq:
                 # logger.debug(f'Linking parent {parent_freq}: {parent_id}')
                 try:
                     parent_row = self.row(parent_freq, parent_id)
                 except ArcanaNameError:
                     # logger.debug(
                     #     f'Parent {parent_freq}:{parent_id} not found, adding')
                     parent_ids = {
@@ -674,18 +679,18 @@
 
         Parameters
         ----------
         name : str
             name of the pipeline
         workflow : pydra.Workflow
             pydra workflow to connect to the dataset as a pipeline
-        inputs : list[arcana.core.pipeline.Input or tuple[str, str, type] or tuple[str, str]]
-            List of inputs to the pipeline (see `arcana.core.pipeline.Pipeline.Input`)
-        outputs : list[arcana.core.pipeline.Output or tuple[str, str, type] or tuple[str, str]]
-            List of outputs of the pipeline (see `arcana.core.pipeline.Pipeline.Output`)
+        inputs : list[arcana.core.analysis.pipeline.Input or tuple[str, str, type] or tuple[str, str]]
+            List of inputs to the pipeline (see `arcana.core.analysis.pipeline.Pipeline.PipelineInput`)
+        outputs : list[arcana.core.analysis.pipeline.Output or tuple[str, str, type] or tuple[str, str]]
+            List of outputs of the pipeline (see `arcana.core.analysis.pipeline.Pipeline.PipelineOutput`)
         row_frequency : str, optional
             the frequency of the data rows the pipeline will be executed over, i.e.
             will it be run once per-session, per-subject or per whole dataset,
             by default the highest row frequency (e.g. per-session for Clinical)
         overwrite : bool, optional
             overwrite connections to previously connected sinks, by default False
         converter_args : dict[str, dict]
@@ -698,52 +703,50 @@
             the pipeline added to the dataset
 
         Raises
         ------
         ArcanaUsageError
             if overwrite is false and
         """
-        from arcana.core.pipeline import Pipeline, Input, Output
+        from arcana.core.analysis.pipeline import Pipeline
 
         row_frequency = self._parse_freq(row_frequency)
 
-        def parsed_conns(lst, conn_type):
-            parsed = []
-            for spec in lst:
-                if isinstance(spec, conn_type):
-                    parsed.append(spec)
-                elif len(spec) == 3:
-                    parsed.append(conn_type(*spec))
-                else:
-                    col_name, pydra_field = spec
-                    parsed.append(
-                        conn_type(col_name, pydra_field, self[col_name].format)
-                    )
-            return parsed
+        # def parsed_conns(lst, conn_type):
+        #     parsed = []
+        #     for spec in lst:
+        #         if isinstance(spec, conn_type):
+        #             parsed.append(spec)
+        #         elif len(spec) == 3:
+        #             parsed.append(conn_type(*spec))
+        #         else:
+        #             col_name, field = spec
+        #             parsed.append(conn_type(col_name, field, self[col_name].datatype))
+        #     return parsed
 
         pipeline = Pipeline(
             name=name,
             dataset=self,
             row_frequency=row_frequency,
             workflow=workflow,
-            inputs=parsed_conns(inputs, Input),
-            outputs=parsed_conns(outputs, Output),
+            inputs=inputs,
+            outputs=outputs,
             converter_args=converter_args,
         )
         for outpt in pipeline.outputs:
-            sink = self[outpt.col_name]
+            sink = self[outpt.name]
             if sink.pipeline_name is not None:
                 if overwrite:
                     logger.info(
-                        f"Overwriting pipeline of sink '{outpt.col_name}' "
+                        f"Overwriting pipeline of sink '{outpt.name}' "
                         f"{sink.pipeline_name} with {name}"
                     )
                 else:
                     raise ArcanaUsageError(
-                        f"Attempting to overwrite pipeline of '{outpt.col_name}' "
+                        f"Attempting to overwrite pipeline of '{outpt.name}' "
                         f"sink ({sink.pipeline_name}) with {name}. Use "
                         f"'overwrite' option if this is desired"
                     )
             sink.pipeline_name = pipeline.name
         self.pipelines[name] = pipeline
 
         return pipeline
@@ -757,18 +760,18 @@
             Names of the columns corresponding to the items to derive
         ids : Iterable[str]
             The IDs of the data rows in each column to derive
         cache_dir
 
         Returns
         -------
-        Sequence[List[DataItem]]
+        Sequence[List[DataType]]
             The derived columns
         """
-        from arcana.core.pipeline import Pipeline
+        from arcana.core.analysis.pipeline import Pipeline
 
         sinks = [self[s] for s in set(sink_names)]
         for pipeline, _ in Pipeline.stack(*sinks):
             # Execute pipelines in stack
             # FIXME: Should combine the pipelines into a single workflow and
             # dilate the IDs that need to be run when summarising over different
             # data axes
@@ -800,21 +803,99 @@
     @classmethod
     def parse_id_str(cls, id):
         parts = id.split("//")
         if len(parts) == 1:  # No store definition, default to file system
             store_name = "file"
         else:
             store_name, id = parts
-        parts = id.split("::")
+        parts = id.split("@")
         if len(parts) == 1:
             name = cls.DEFAULT_NAME
         else:
             id, name = parts
         return store_name, id, name
 
+    def download_licenses(self, licenses: list[License]):
+        """Install licenses from project-specific location in data store and
+        install them at the destination location
+
+        Parameters
+        ----------
+        licenses : list[License]
+            the list of licenses stored in the dataset or in a site-wide location that
+            need to be downloaded to the local file-system before a pipeline is run
+
+        Raises
+        ------
+        ArcanaLicenseNotFoundError
+            raised if the license of the given name isn't present in the project-specific
+            location to retrieve
+        """
+
+        site_licenses_dataset = self.store.site_licenses_dataset()
+
+        for lic in licenses:
+
+            license_file = self._get_license_file(lic.name)
+
+            try:
+                lic_fs_path = license_file.fs_paths[0]
+            except ArcanaUsageError:
+                missing = False
+                if site_licenses_dataset is not None:
+                    license_file = self._get_license_file(
+                        lic.name, dataset=site_licenses_dataset
+                    )
+                    try:
+                        lic_fs_path = license_file.fs_paths[0]
+                    except ArcanaUsageError:
+                        missing = True
+                else:
+                    missing = True
+                if missing:
+                    msg = (
+                        f"Did not find a license corresponding to '{lic.name}' at "
+                        f"{License.column_name(lic.name)} in {self}"
+                    )
+                    if site_licenses_dataset:
+                        msg += f" or {site_licenses_dataset}"
+                    raise ArcanaLicenseNotFoundError(
+                        lic.name,
+                        msg,
+                    )
+            shutil.copyfile(lic_fs_path, lic.destination)
+
+    def install_license(self, name, source_file):
+        """Store project-specific license in dataset
+
+        Parameters
+        ----------
+        name : str
+            name of the license to install
+        source_file : Path
+            path to the license file to install
+        """
+        license_file = self._get_license_file(name)
+        license_file.put(source_file)
+
+    def _get_license_file(self, lic_name, dataset=None):
+        import arcana.common.data.formats
+        import arcana.core.deploy.image.components
+
+        if dataset is None:
+            dataset = self
+        license_column = DataSink(
+            f"{lic_name}_license",
+            arcana.core.deploy.image.components.License.column_path(lic_name),
+            arcana.common.data.formats.File,
+            row_frequency=self.root_freq,
+            dataset=dataset,
+        )
+        return license_column.match(dataset.root)
+
 
 @attrs.define
 class SplitDataset:
     """A dataset created by combining multiple datasets into a conglomerate
 
     Parameters
     ----------
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/space.py` & `arcana-2.0b2/arcana/core/data/space.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as ty
 import re
-from operator import __or__
 from enum import Enum
-from arcana.core.utils import class_location, resolve_class
+from arcana.core.utils.serialize import ClassResolver
+from arcana.core.utils.misc import classproperty
 
 
 class DataSpace(Enum):
     """
     Base class for all "data space" enums. DataSpace enums specify
     the relationships between rows of a dataset.
 
@@ -121,26 +121,23 @@
 
     def __or__(self, other):
         return type(self)(self.value | other.value)
 
     def __invert__(self):
         return type(self)(~self.value)
 
-    def __add__(self, other):
-        return type(self)(self.value + other.value)
-
-    def __sub__(self, other):
-        return type(self)(self.value - other.value)
-
     def __hash__(self):
         return self.value
 
     def __bool__(self):
         return bool(self.value)
 
+    def bin(self):
+        return bin(self.value)
+
     @classmethod
     def union(cls, freqs: ty.Sequence[Enum]):
         "Returns the union between data row_frequency values"
         union = cls(0)
         for f in freqs:
             union |= f
         return union
@@ -165,13 +162,25 @@
         -------
         bool
             True if self is parent of child
         """
         return ((self & child) == self) and (child != self or if_match)
 
     def tostr(self):
-        return f"{class_location(self)}[{str(self)}]"
+        return f"{ClassResolver.tostr(self, strip_prefix=False)}[{str(self)}]"
 
     @classmethod
     def fromstr(cls, s):
-        class_loc, val = re.match(r"(.*)\[([^\]]+)\]", s).groups()
-        return resolve_class(class_loc)[val]
+        match = re.match(r"(.*)\[([^\]]+)\]", s)
+        if match is None:
+            raise ValueError(
+                f"'{s}' is not a string of the format <data-space-enum>[<value>]"
+            )
+        class_loc, val = match.groups()
+        space = ClassResolver(cls)(class_loc)
+        return space[val] if not isinstance(space, str) else s
+
+    @classproperty
+    def DEFAULT_PACKAGE(cls):
+        """Cannot be a regular class attribute because then DataSpace won't be able to
+        be extended"""
+        return "arcana.data.spaces"
```

### Comparing `arcana-2.0b0.dev7/arcana/core/data/store.py` & `arcana-2.0b2/arcana/core/data/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
+from __future__ import annotations
 import logging
 from abc import abstractmethod, ABCMeta
-import inspect
 from pathlib import Path
 import attrs
 import typing as ty
 import yaml
-from arcana.core.utils import (
-    get_config_file_path,
-    list_subclasses,
-    resolve_class,
-    class_location,
+from arcana.core.utils.serialize import (
     asdict,
     fromdict,
 )
+import arcana
+from arcana.core.utils.misc import get_config_file_path
+from arcana.core.utils.packaging import list_subclasses
 from arcana.exceptions import ArcanaUsageError, ArcanaNameError
 
 DS = ty.TypeVar("DS", bound="DataStore")
 
 logger = logging.getLogger("arcana")
 
 
@@ -30,14 +29,16 @@
 
     _connection_depth = attrs.field(
         default=0, init=False, hash=False, repr=False, eq=False
     )
 
     CONFIG_NAME = "stores"
 
+    DEFAULT_PACKAGE = "arcana.data.stores"
+
     @abstractmethod
     def find_rows(self, dataset):
         """
         Find all data rows for a dataset in the store and populate the
         Dataset object using its `add_row` method.
 
         Parameters
@@ -169,26 +170,26 @@
 
     @abstractmethod
     def put_provenance(self, item, provenance: ty.Dict[str, ty.Any]):
         """Stores provenance information for a given data item in the store
 
         Parameters
         ----------
-        item: DataItem
+        item: DataType
             The item to store the provenance data for
         provenance: dict[str, Any]
             The provenance data to store"""
 
     @abstractmethod
     def get_provenance(self, item) -> ty.Dict[str, ty.Any]:
         """Stores provenance information for a given data item in the store
 
         Parameters
         ----------
-        item: DataItem
+        item: DataType
             The item to store the provenance data for
 
         Returns
         -------
         provenance: dict[str, Any] or None
             The provenance data stored in the repository for the data item.
             None if no provenance data has been stored"""
@@ -245,14 +246,18 @@
         with self:
             entries[name] = self.asdict()
         self.save_entries(entries, config_path=config_path)
 
     def asdict(self, **kwargs):
         return asdict(self, **kwargs)
 
+    def site_licenses_dataset(self):
+        """Can be overridden by subclasses to provide a dataset to hold site-wide licenses"""
+        return None
+
     @classmethod
     def load(cls: ty.Type[DS], name: str, config_path: Path = None, **kwargs) -> DS:
         """Loads a DataStore from that has been saved in the configuration file.
         If no entry is saved under that name, then it searches for DataStore
         sub-classes with aliases matching `name` and checks whether they can
         be initialised without any parameters.
 
@@ -284,15 +289,15 @@
                 return cls.singletons()[name]
             except KeyError:
                 raise ArcanaNameError(
                     name, f"No saved data store or built-in type matches '{name}'"
                 )
         else:
             entry.update(kwargs)
-            store = fromdict(entry)
+            store = fromdict(entry)  # Would be good to use a class resolver here
         return store
 
     @classmethod
     def remove(cls, name: str, config_path: Path = None):
         """Removes the entry saved under 'name' in the config file
 
         Parameters
@@ -319,30 +324,38 @@
             The hierarchy of the dataset
         space : EnumMeta
             The DataSpace enum that defines the frequencies (e.g.
             per-session, per-subject,...) present in the dataset.
         **kwargs:
             Keyword args passed on to the Dataset init method
         """
+        from .space import DataSpace
+
         if not hierarchy:
-            try:
-                hierarchy = self.DEFAULT_HIERARCHY
-            except AttributeError as e:
-                raise ArcanaUsageError(
-                    "'hierarchy' kwarg must be specified for datasets in "
-                    f"{type(self)} stores"
-                ) from e
+            if space:
+                hierarchy = [max(space)]
+            else:
+                try:
+                    hierarchy = self.DEFAULT_HIERARCHY
+                except AttributeError as e:
+                    raise ArcanaUsageError(
+                        "'hierarchy' kwarg must be specified for datasets in "
+                        f"{type(self)} stores"
+                    ) from e
         if not space:
-            try:
-                space = self.DEFAULT_SPACE
-            except AttributeError as e:
-                raise ArcanaUsageError(
-                    "'space' kwarg must be specified for datasets in "
-                    f"{type(self)} stores"
-                ) from e
+            if hierarchy and isinstance(hierarchy[0], DataSpace):
+                space = type(hierarchy[0])
+            else:
+                try:
+                    space = self.DEFAULT_SPACE
+                except AttributeError as e:
+                    raise ArcanaUsageError(
+                        "'space' kwarg must be specified for datasets in "
+                        f"{type(self)} stores"
+                    ) from e
         from arcana.core.data.set import (
             Dataset,
         )  # avoid circular imports it is imported here rather than at the top of the file
 
         dataset = Dataset(id, store=self, space=space, hierarchy=hierarchy, **kwargs)
         return dataset
 
@@ -352,29 +365,28 @@
         )  # avoid circular imports it is imported here rather than at the top of the file
 
         if name is None:
             name = Dataset.DEFAULT_NAME
         dct = self.load_dataset_definition(id, name)
         if dct is None:
             raise KeyError(f"Did not find a dataset '{id}::{name}'")
-        return fromdict(dct, name=name, store=self)
+        return fromdict(dct, id=id, name=name, store=self)
 
     @classmethod
     def singletons(cls):
-        """Returns stores in a dictionary indexed by their aliases, for which there only needs to be a single instance"""
+        """Returns stores in a dictionary indexed by their aliases, for which there
+        only needs to be a single instance"""
         try:
             return cls._singletons
         except AttributeError:
             pass
         # If not saved in the configuration file search for sub-classes
         # whose alias matches `name` and can be initialised without params
-        import arcana.data.stores
-
         cls._singletons = {}
-        for store_cls in list_subclasses(arcana.data.stores, DataStore):
+        for store_cls in list_subclasses(arcana, DataStore):
             try:
                 cls._singletons[store_cls.get_alias()] = store_cls()
             except Exception:
                 pass
         return cls._singletons
 
     @classmethod
```

### Comparing `arcana-2.0b0.dev7/arcana/core/deploy/build.py` & `arcana-2.0b2/arcana/core/deploy/image/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,522 +1,517 @@
+from __future__ import annotations
 import typing as ty
-from pathlib import Path
+
+# import hashlib
+from pathlib import PurePath, Path
 import json
 import tempfile
 import logging
+from copy import copy
 import shutil
-from natsort import natsorted
+from inspect import isclass, isfunction
+from build import ProjectBuilder
+import attrs
 import docker
-import yaml
 from neurodocker.reproenv import DockerRenderer
 from arcana import __version__
-from arcana.__about__ import PACKAGE_NAME, python_versions
+from arcana import PACKAGE_NAME
+from arcana.core.utils.serialize import (
+    ClassResolver,
+    ObjectConverter,
+)
+from arcana.core.utils.misc import (
+    DOCKER_HUB,
+)
+from arcana.core.data.space import DataSpace
 from arcana.exceptions import ArcanaBuildError
-from .utils import PipSpec, local_package_location
-
+from .components import Packages, BaseImage, PipPackage, CondaPackage
 
 logger = logging.getLogger("arcana")
 
-DEFAULT_BASE_IMAGE = "ubuntu:kinetic"
-PYTHON_PACKAGE_DIR = "python-packages"
-
-CONDA_ENV = "arcana"
-
-SPEC_PATH = "/arcana-spec.yaml"
-
-
-def build_docker_image(image_tag: str, build_dir: Path = None, **kwargs):
-    """Executes the full build workflow, from generating the Dockerfile to
-    calling Docker to build it
 
-    Parameters
-    ----------
-    image_tag : str
-        _description_
-    build_dir : Path, optional
-        _description_, by default None
+@attrs.define(kw_only=True)
+class ArcanaImage:
     """
-    if build_dir is None:
-        build_dir = tempfile.mkdtemp()
-    build_dir = Path(build_dir)
-
-    dockerfile = construct_dockerfile(build_dir, **kwargs)
-
-    dockerfile_build(dockerfile, build_dir, image_tag)
-
-
-def construct_dockerfile(
-    build_dir: Path,
-    base_image: str = DEFAULT_BASE_IMAGE,
-    python_packages: ty.Iterable[
-        PipSpec or ty.Dict[str, str] or ty.Tuple[str, str]
-    ] = None,
-    system_packages: ty.Iterable[ty.Iterable[ty.Tuple[str, str]]] = None,
-    package_templates: ty.Iterable[ty.Dict[str, str]] = None,
-    labels: ty.Dict[str, str] = None,
-    package_manager: str = "apt",
-    arcana_install_extras: ty.Iterable[str] = (),
-    readme: str = None,
-    use_local_packages: bool = False,
-    pypi_fallback: bool = False,
-    license_dir: Path = None,
-    licenses: ty.Iterable[ty.Dict[str, str]] = (),
-    spec: dict = None,
-) -> DockerRenderer:
-    """Constructs a dockerfile that wraps a with dependencies
-
-    Parameters
-    ----------
-    build_dir : Path
-        Path to the directory the Dockerfile will be written into copy any local
-        files to
-    base_image : str, optional
-        The base image to build from
-    python_packages:  Iterable[PipSpec or dict[str, str] or tuple[str, str]], optional
-        Name and version of the Python PyPI packages to add to the image (in
-        addition to Arcana itself)
-    system_packages: Iterable[str], optional
-        Name and version of operating system packages (see Neurodocker) to add
-        to the image
+    Base class with Arcana installed within it from which all container image
+    specifications can inherit from
+
+    name : str
+        name of the package/pipeline
+    version : str
+        version of the package/pipeline
+    build_iteration : str
+        will be appended to the tag of the built images. Used to specify that the build
+        specification has been updated but the underlying software is the same
+    org : str
+        the organisation the image will be tagged within
+    base_image : arcana.core.deploy.image.components.BaseImage, optional
+        the base image to build from
+    packages : arcana.core.deploy.image.components.Packages
+        System (OS), PyPI, Conda and Neurodocker packages/templates to be installed
+        in the image
     package_templates : Iterable[dict[str, str]]
         Neurodocker package installation templates to be installed inside the image. A
         dictionary containing the 'name' and 'version' of the template along
         with any additional keyword arguments required by the template
-    labels : ty.Dict[str, str], optional
-        labels to be added to the image
-    arcana_install_extras : Iterable[str], optional
-        Extras for the Arcana package that need to be installed into the
-        dockerfile (e.g. tests)
+    registry : str, optional
+        the container registry the image is to be installed at
     readme : str, optional
-        Description of the container to put in a README
-    use_local_packages: bool, optional
-        Use the python package versions that are installed within the
-        current environment, i.e. instead of pulling from PyPI. Useful during
-        development and testing
-    pypi_fallback : bool, optional
-        whether to fallback to packages installed on PyPI when versions of
-        local packages don't match installed
-    license_dir : Path, optional
-        path to the directory containing the licence files to copy into the
-        image
-    licenses : list[dict[str, str]], optional
-        specification of licenses to install inside docker image. Each dict
-        should contain 'source' and 'destination' items.
-    spec : dict, optional
-        the specification used to generate the image to be saved inside it for
-        future reference
-
-    Returns
-    -------
-    DockerRenderer
-        Neurodocker Docker renderer to construct dockerfile from
+        text to include in the image README file
+    labels : dict[str, str]
     """
-    if python_packages is None:
-        python_packages = []
-    else:
-        python_packages = [
-            (
-                PipSpec(p)
-                if isinstance(p, str)
-                else (
-                    PipSpec(**p)
-                    if isinstance(p, dict)
-                    else (PipSpec(*p) if not isinstance(p, PipSpec) else p)
-                )
-            )
-            for p in python_packages
-        ]
-
-    if not build_dir.is_dir():
-        raise ArcanaBuildError(f"Build dir '{str(build_dir)}' is not a valid directory")
-
-    dockerfile = DockerRenderer(package_manager).from_(base_image)
-    dockerfile.install(["git", "ssh-client", "vim"])
-
-    if system_packages is not None:
-        install_system_packages(dockerfile, system_packages)
 
-    if package_templates is not None:
-        install_package_templates(dockerfile, package_templates)
-
-    install_python(
-        dockerfile,
-        python_packages,
-        build_dir,
-        use_local_packages=use_local_packages,
-        pypi_fallback=pypi_fallback,
+    name: str
+    version: str = attrs.field(converter=str)
+    build_iteration: str = None
+    base_image: BaseImage = attrs.field(
+        default=BaseImage(), converter=ObjectConverter(BaseImage)
     )
-
-    # Arcana is installed separately from the other Python packages, partly so
-    # the dependency Docker layer can be cached in dev and partly so it can be
-    # treated differently if required in the future
-    install_arcana(
-        dockerfile,
-        build_dir,
-        install_extras=arcana_install_extras,
-        use_local_package=use_local_packages,
+    packages: Packages = attrs.field(
+        default=Packages(), converter=ObjectConverter(Packages)
     )
-
-    if licenses and license_dir is None:
-        raise ArcanaBuildError(
-            "'--license_dir' input must be provided for specifications "
-            f"including 'licenses' items ({licenses})"
+    org: str = None
+    registry: str = DOCKER_HUB
+    readme: str = None
+    labels: dict[str, str] = None
+
+    @property
+    def reference(self):
+        return f"{self.path}:{self.tag}"
+
+    @property
+    def tag(self):
+        return (
+            f"{self.version}-{self.build_iteration}"
+            if self.build_iteration
+            else self.version
         )
 
-    install_licenses(dockerfile, licenses, license_dir, build_dir)
-
-    if readme:
-        insert_readme(dockerfile, readme, build_dir)
-
-    if spec:
-        insert_spec(dockerfile, spec, build_dir)
+    @property
+    def path(self):
+        prefix = self.registry + "/" if self.registry != DOCKER_HUB else ""
+        org_str = self.org + "/" if self.org else ""
+        return (prefix + org_str + self.name).lower()
+
+    def make(
+        self,
+        build_dir: Path = None,
+        generate_only: bool = False,
+        **kwargs,
+    ):
+        """Makes the container image from the spec: generates the Dockerfile and then
+        builds it.
+
+        Parameters
+        ----------
+        build_dir : Path, optional
+            _description_, by default None
+        """
+
+        if build_dir is None:
+            build_dir = tempfile.mkdtemp()
+        build_dir = Path(build_dir)
+        if build_dir.exists():
+            shutil.rmtree(build_dir)
+        build_dir.mkdir()
+
+        dockerfile = self.construct_dockerfile(build_dir, **kwargs)
+
+        if not generate_only:
+            self.build(dockerfile, build_dir, image_tag=self.reference)
+
+    def construct_dockerfile(
+        self,
+        build_dir: Path,
+        use_local_packages: bool = False,
+        pypi_fallback: bool = False,
+        arcana_install_extras: ty.List[str] = (),
+        **kwargs,
+    ) -> DockerRenderer:
+        """Constructs a dockerfile that wraps a with dependencies
+
+        Parameters
+        ----------
+        build_dir : Path
+            Path to the directory the Dockerfile will be written into copy any local
+            files to
+        use_local_packages: bool, optional
+            Use the python package versions that are installed within the
+            current environment, i.e. instead of pulling from PyPI. Useful during
+            development and testing
+        pypi_fallback : bool, optional
+            whether to fallback to packages installed on PyPI when versions of
+            local packages don't match installed
+        arcana_install_extras : Iterable[str], optional
+            Extras for the Arcana package that need to be installed into the
+            dockerfile (e.g. tests)
+        readme : str, optional
+            Description of the container to put in a README
+        labels : ty.Dict[str, str], optional
+            labels to be added to the image
+
+        Returns
+        -------
+        DockerRenderer
+            Neurodocker Docker renderer to construct dockerfile from
+        """
 
-    if labels:
-        # dockerfile.label(labels)
-        dockerfile._parts.append(
-            "LABEL "
-            + " \\\n      ".join(f"{k}={json.dumps(v)}" for k, v in labels.items())
-        )
+        if not build_dir.is_dir():
+            raise ArcanaBuildError(
+                f"Build dir '{str(build_dir)}' is not a valid directory"
+            )
 
-    return dockerfile
+        dockerfile = self.init_dockerfile()
 
+        self.install_system_packages(dockerfile)
 
-def dockerfile_build(dockerfile: DockerRenderer, build_dir: Path, image_tag: str):
-    """Builds the dockerfile in the specified build directory
+        self.install_package_templates(dockerfile)
 
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        Neurodocker renderer to build
-    build_dir : Path
-        path of the build directory
-    image_tag : str
-        Docker image tag to assign to the built image
-    """
-
-    # Save generated dockerfile to file
-    out_file = build_dir / "Dockerfile"
-    out_file.parent.mkdir(exist_ok=True, parents=True)
-    with open(str(out_file), "w") as f:
-        f.write(dockerfile.render())
-    logger.info("Dockerfile for '%s' generated at %s", image_tag, str(out_file))
-
-    dc = docker.from_env()
-    try:
-        dc.images.build(path=str(build_dir), tag=image_tag)
-    except docker.errors.BuildError as e:
-        build_log = "\n".join(ln.get("stream", "") for ln in e.build_log)
-        raise RuntimeError(
-            f"Building '{image_tag}' from '{str(build_dir)}/Dockerfile' "
-            f"failed with the following errors:\n\n{build_log}"
+        self.install_python(
+            dockerfile,
+            build_dir,
+            use_local_packages=use_local_packages,
+            pypi_fallback=pypi_fallback,
         )
-    logging.info("Successfully built docker image %s", image_tag)
-
-
-def install_python(
-    dockerfile: DockerRenderer,
-    packages: ty.Iterable[PipSpec],
-    build_dir: Path,
-    use_local_packages: bool = False,
-    pypi_fallback: bool = False,
-):
-    """Generate Neurodocker instructions to install an appropriate version of
-    Python and the required Python packages
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    packages : ty.Iterable[PipSpec]
-        the python packages (with optional extras) that need to be installed
-    build_dir : Path
-        the path to the build directory
-    arcana_install_extras : Iterable[str]
-        Optional extras (i.e. as defined in "extras_require" in setup.py) required
-        for the arcana package
-    use_local_packages: bool, optional
-        Use the python package versions that are installed within the
-        current environment, i.e. instead of defaulting to the release from PyPI.
-        Useful during development and testing
-    pypi_fallback : bool, optional
-        Whether to fall back to PyPI version when local version doesn't match
-        requested
-
-    Returns
-    -------
-    list[list[str, list[str, str]]]
-        neurodocker instructions to install python and required packages
-    """
 
-    # # Split out and merge any extras specifications (e.g. "arcana[test]")
-    # between dependencies of the same package
-    # Add arcana dependency
-    packages = PipSpec.unique(packages, remove_arcana=True)
-
-    dockerfile.add_registered_template(
-        "miniconda",
-        version="latest",
-        env_name=CONDA_ENV,
-        env_exists=False,
-        conda_install=" ".join(
-            ["python=" + natsorted(python_versions)[-1], "numpy", "traits"]
-        ),
-        pip_install=" ".join(
-            pip_spec2str(p, dockerfile, build_dir, use_local_packages, pypi_fallback)
-            for p in packages
-        ),
-    )
+        # Arcana is installed separately from the other Python packages, partly so
+        # the dependency Docker layer can be cached in dev and partly so it can be
+        # treated differently if required in potential subclasses
+        self.install_arcana(
+            dockerfile,
+            build_dir,
+            install_extras=arcana_install_extras,
+            use_local_package=use_local_packages,
+        )
 
+        self.write_readme(dockerfile, build_dir)
 
-def install_arcana(
-    dockerfile: DockerRenderer,
-    build_dir: Path,
-    install_extras: ty.Iterable = (),
-    use_local_package: bool = False,
-):
-    """Install the Arcana Python package into the Dockerfile
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the Neurdocker renderer
-    build_dir : Path
-        the directory the Docker image is built from
-    install_extras : list[str]
-        list of "install extras" (options) to specify when installing Arcana
-        (e.g. 'test')
-    use_local_package : bool
-        Use local installation of arcana
-    """
-    pip_str = pip_spec2str(
-        PipSpec(PACKAGE_NAME, extras=install_extras),
-        dockerfile,
-        build_dir,
-        use_local_packages=use_local_package,
-        pypi_fallback=False,
-    )
-    dockerfile.run(
-        f'bash -c "source activate {CONDA_ENV} \\\n'
-        f'&& python -m pip install --pre --no-cache-dir {pip_str}"'
-    )
+        self.add_labels(dockerfile)
 
+        return dockerfile
 
-def install_system_packages(dockerfile: DockerRenderer, packages: ty.Iterable[str]):
-    """Generate Neurodocker instructions to install systems packages in dockerfile
+    @classmethod
+    def build(cls, dockerfile: DockerRenderer, build_dir: Path, image_tag: str):
+        """Builds the dockerfile in the specified build directory
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            Neurodocker renderer to build
+        build_dir : Path
+            path of the build directory
+        image_tag : str
+            Docker image tag to assign to the built image
+        """
+
+        # Save generated dockerfile to file
+        out_file = build_dir / "Dockerfile"
+        out_file.parent.mkdir(exist_ok=True, parents=True)
+        with open(str(out_file), "w") as f:
+            f.write(dockerfile.render())
+        logger.info("Dockerfile for '%s' generated at %s", image_tag, str(out_file))
+
+        dc = docker.from_env()
+        try:
+            dc.images.build(path=str(build_dir), tag=image_tag)
+        except docker.errors.BuildError as e:
+            build_log = "\n".join(ln.get("stream", "") for ln in e.build_log)
+            raise RuntimeError(
+                f"Building '{image_tag}' from '{str(build_dir)}/Dockerfile' "
+                f"failed with the following errors:\n\n{build_log}"
+            )
+        logging.info("Successfully built docker image %s", image_tag)
 
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    system_packages : Iterable[str]
-        the packages to install on the operating system
-    """
-    dockerfile.install(packages)
+    def init_dockerfile(self):
+        dockerfile = DockerRenderer(self.base_image.package_manager).from_(
+            self.base_image.reference
+        )
+        return dockerfile
 
+    def add_labels(self, dockerfile, labels=None):
+        if labels is None:
+            labels = self.labels
+        if labels:
+            dockerfile.labels({k: json.dumps(v).strip('"') for k, v in labels.items()})
+
+    def install_python(
+        self,
+        dockerfile: DockerRenderer,
+        build_dir: Path,
+        use_local_packages: bool = False,
+        pypi_fallback: bool = False,
+    ):
+        """Generate Neurodocker instructions to install an appropriate version of
+        Python and the required Python packages
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        build_dir : Path
+            the path to the build directory
+        arcana_install_extras : Iterable[str]
+            Optional extras (i.e. as defined in "extras_require" in setup.py) required
+            for the arcana package
+        use_local_packages: bool, optional
+            Use the python package versions that are installed within the
+            current environment, i.e. instead of defaulting to the release from PyPI.
+            Useful during development and testing
+        pypi_fallback : bool, optional
+            Whether to fall back to PyPI version when local version doesn't match
+            requested
+
+        Returns
+        -------
+        list[list[str, list[str, str]]]
+            neurodocker instructions to install python and required packages
+        """
+
+        pip_strs = []
+        for pip_spec in self.packages.pip:
+            if use_local_packages:
+                pip_spec = pip_spec.local_package_location(pypi_fallback=pypi_fallback)
+            pip_strs.append(self.pip_spec2str(pip_spec, dockerfile, build_dir))
+
+        conda_pkg_names = set(p.name for p in self.packages.conda)
+        conda_strs = []
+        if "python" not in conda_pkg_names:
+            conda_strs.append("python")
+        for pkg_name in CondaPackage.REQUIRED:
+            if pkg_name not in conda_pkg_names:
+                conda_strs.append(pkg_name)
+
+        conda_strs.extend(
+            f"{p.name}={p.version}" if p.version is not None else p.name
+            for p in self.packages.conda
+        )
 
-def install_package_templates(
-    dockerfile: DockerRenderer, package_templates: ty.Iterable[ty.Dict[str, str]]
-):
-    """Install custom packages from Neurodocker package_templates
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    package_templates : Iterable[dict[str, str]]
-        Neurodocker installation package_templates to be installed inside the image. A
-        dictionary containing the 'name' and 'version' of the template along
-        with any additional keyword arguments required by the template
-    """
+        dockerfile.add_registered_template(
+            "miniconda",
+            version="latest",
+            env_name=self.CONDA_ENV,
+            env_exists=False,
+            conda_install=" ".join(conda_strs),
+            pip_install=" ".join(pip_strs),
+        )
 
-    for kwds in package_templates:
-        dockerfile.add_registered_template(kwds.pop("name"), **kwds)
+    def install_system_packages(self, dockerfile: DockerRenderer):
+        """Generate Neurodocker instructions to install systems packages in dockerfile
 
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        system_packages : Iterable[str]
+            the packages to install on the operating system
+        """
+        pkg_strs = [
+            f"{p.name}={p.version}" if p.version else p.name
+            for p in self.packages.system
+        ]
+        dockerfile.install(pkg_strs)
 
-def install_licenses(
-    dockerfile: DockerRenderer,
-    licenses: ty.List[ty.Dict[str, str]],
-    license_dir: Path,
-    build_dir: Path,
-):
-    """Generate Neurodocker instructions to install README file inside the docker
-    image
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    description : str
-        a description of what the pipeline does, to be inserted in a README file
-        in the Docker image
-    build_dir : Path
-        path to build dir
-    """
-    if not licenses:
-        return
-    # Copy licenses into build directory
-    license_build_dir = build_dir / "licenses"
-    shutil.copytree(license_dir, license_build_dir, dirs_exist_ok=True)
-    for spec in licenses:
-        src = license_build_dir / spec["source"]
-        dockerfile.copy(
-            source=[str(src.relative_to(build_dir))], destination=spec["destination"]
+    def install_package_templates(
+        self,
+        dockerfile: DockerRenderer,
+    ):
+        """Install custom packages from Neurodocker package_templates
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        package_templates : Iterable[dict[str, str]]
+            Neurodocker installation package_templates to be installed inside the image. A
+            dictionary containing the 'name' and 'version' of the template along
+            with any additional keyword arguments required by the template
+        """
+        for template in self.packages.neurodocker:
+            kwds = attrs.asdict(template)
+            kwds = copy(
+                kwds
+            )  # so we can pop the name and leave the original dictionary intact
+            dockerfile.add_registered_template(kwds.pop("name"), **kwds)
+
+    def install_arcana(
+        self,
+        dockerfile: DockerRenderer,
+        build_dir: Path,
+        install_extras: ty.Iterable = (),
+        use_local_package: bool = False,
+    ):
+        """Install the Arcana Python package into the Dockerfile
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the Neurdocker renderer
+        build_dir : Path
+            the directory the Docker image is built from
+        install_extras : list[str]
+            list of "install extras" (options) to specify when installing Arcana
+            (e.g. 'test')
+        use_local_package : bool
+            Use local installation of arcana
+        """
+        arcana_pip_spec = PipPackage(PACKAGE_NAME, extras=install_extras)
+        if use_local_package:
+            arcana_pip_spec = arcana_pip_spec.local_package_location()
+        pip_str = self.pip_spec2str(
+            arcana_pip_spec,
+            dockerfile,
+            build_dir,
+        )
+        dockerfile.run(
+            f'bash -c "source activate {self.CONDA_ENV} \\\n'
+            f'&& python -m pip install --pre --no-cache-dir {pip_str}"'
         )
 
-
-def insert_readme(dockerfile: DockerRenderer, description, build_dir):
-    """Generate Neurodocker instructions to install README file inside the docker
-    image
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    description : str
-        a description of what the pipeline does, to be inserted in a README file
-        in the Docker image
-    build_dir : Path
-        path to build dir
-    """
-    if description is None:
-        description = ""
-    else:
-        description = "\n" + description + "\n"
-    with open(build_dir / "README.md", "w") as f:
-        f.write(DOCKERFILE_README_TEMPLATE.format(__version__, description))
-    dockerfile.copy(source=["./README.md"], destination="/README.md")
-
-
-def insert_spec(dockerfile: DockerRenderer, spec, build_dir):
-    """Generate Neurodocker instructions to install README file inside the docker
-    image
-
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        the neurodocker renderer to append the install instructions to
-    spec : dict
-        the specification used to build the image
-    build_dir : Path
-        path to build dir
-    """
-    with open(build_dir / "arcana-spec.yaml", "w") as f:
-        yaml.dump(spec, f)
-    dockerfile.copy(source=["./arcana-spec.yaml"], destination=SPEC_PATH)
-
-
-def pip_spec2str(
-    pip_spec: PipSpec,
-    dockerfile: DockerRenderer,
-    build_dir: Path,
-    use_local_packages: bool,
-    pypi_fallback: bool,
-) -> str:
-    """Generates a string to be passed to `pip` in order to install a package
-    from a "pip specification" object
-
-    Parameters
-    ----------
-    pip_spec : PipSpec
-        specification of the package to install
-    dockerfile : DockerRenderer
-        Neurodocker Docker renderer object used to generate the Dockerfile
-    build_dir : Path
-        path to the directory the Docker image will be built in
-    use_local_packages : bool
-        whether to prefer local version of package (instead of PyPI version)
-
-    Returns
-    -------
-    str
-        string to be passed to `pip` installer
-    """
-    # Copy the local development versions of Python dependencies into the
-    # docker image if present, instead of relying on the PyPI version,
-    # which might be missing local changes and bugfixes (particularly in testing)
-    if use_local_packages:
-        pip_spec = local_package_location(pip_spec, pypi_fallback=pypi_fallback)
-    if pip_spec.file_path:
-        if pip_spec.version or pip_spec.url:
-            raise ArcanaBuildError(
-                "Cannot specify a package by `file_path`, `version` and/or " "`url`"
+    @classmethod
+    def pip_spec2str(
+        cls,
+        pip_spec: PipPackage,
+        dockerfile: DockerRenderer,
+        build_dir: Path,
+    ) -> str:
+        """Generates a string to be passed to `pip` in order to install a package
+        from a "pip specification" object
+
+        Parameters
+        ----------
+        pip_spec : PipPackage
+            specification of the package to install
+        dockerfile : DockerRenderer
+            Neurodocker Docker renderer object used to generate the Dockerfile
+        build_dir : Path
+            path to the directory the Docker image will be built in
+
+        Returns
+        -------
+        str
+            string to be passed to `pip` installer
+        """
+        # Copy the local development versions of Python dependencies into the
+        # docker image if present, instead of relying on the PyPI version,
+        # which might be missing local changes and bugfixes (particularly in testing)
+        # if use_local_packages:
+        #     pip_spec = pip_spec.local_package_location(pypi_fallback=pypi_fallback)
+        if pip_spec.file_path:
+            if pip_spec.version or pip_spec.url:
+                raise ArcanaBuildError(
+                    "Cannot specify a package by `file_path`, `version` and/or " "`url`"
+                )
+            # pkg_build_path = cls.copy_sdist_into_build_dir(
+            #     pip_spec.file_path, build_dir
+            # )
+            # Create a source distribution tarball to be installed within the docker
+            # image
+            sdist_dir = build_dir / cls.PYTHON_PACKAGE_DIR
+            builder = ProjectBuilder(pip_spec.file_path)
+            pkg_build_path = Path(builder.build("sdist", sdist_dir))
+            pip_str = "/" + cls.PYTHON_PACKAGE_DIR + "/" + pkg_build_path.name
+            dockerfile.copy(
+                source=[str(pkg_build_path.relative_to(build_dir))], destination=pip_str
             )
-        pkg_build_path = copy_package_into_build_dir(
-            pip_spec.name, pip_spec.file_path, build_dir
-        )
-        pip_str = "/" + PYTHON_PACKAGE_DIR + "/" + pip_spec.name
-        dockerfile.copy(
-            source=[str(pkg_build_path.relative_to(build_dir))], destination=pip_str
-        )
-    elif pip_spec.url:
+        elif pip_spec.url:
+            if pip_spec.version:
+                raise ArcanaBuildError(
+                    "Cannot specify a package by `url` and `version`"
+                )
+            pip_str = pip_spec.url
+        else:
+            pip_str = pip_spec.name
+        if pip_spec.extras:
+            pip_str += "[" + ",".join(pip_spec.extras) + "]"
         if pip_spec.version:
-            raise ArcanaBuildError("Cannot specify a package by `url` and `version`")
-        pip_str = pip_spec.url
-    else:
-        pip_str = pip_spec.name
-    if pip_spec.extras:
-        pip_str += "[" + ",".join(pip_spec.extras) + "]"
-    if pip_spec.version:
-        pip_str += "==" + pip_spec.version
-    return pip_str
-
-
-def copy_package_into_build_dir(
-    package_name: str, local_installation: Path, build_dir: Path
-):
-    """Copies a local installation of a package into the build directory
-
-    Parameters
-    ----------
-    package_name : str
-        the name of the package (how it will be called in the docker image)
-    local_installation : Path
-        path to the local installation
-    build_dir : Path
-        path to the build directory
-    """
-    pkg_build_path = build_dir / PYTHON_PACKAGE_DIR / package_name
-    if pkg_build_path.exists():
-        shutil.rmtree(pkg_build_path)
-    # Copy source tree into build dir minus any cache files and paths
-    # included in the gitignore
-    patterns_to_ignore = list(PATTERNS_TO_NOT_COPY_INTO_BUILD)
-    ignore_paths = [Path(p) for p in PATHS_TO_NOT_COPY_INTO_BUILD]
-    if (local_installation / ".gitignore").exists():
-        with open(local_installation / ".gitignore") as f:
-            gitignore = f.read().splitlines()
-        patterns_to_ignore.extend(p for p in gitignore if not p.startswith("/"))
-        ignore_paths.extend(Path(p[1:]) for p in gitignore if p.startswith("/"))
-    patterns_to_ignore.append(
-        "conftest.py"
-    )  # confuses pytest if nested within build dirs
-    ignore_patterns = shutil.ignore_patterns(*patterns_to_ignore)
-
-    def ignore_paths_and_patterns(directory, contents):
-        to_ignore = ignore_patterns(directory, contents)
-        to_ignore.update(c for c in contents if Path(directory) / c in ignore_paths)
-        return to_ignore
+            pip_str += "==" + pip_spec.version
+        return pip_str
 
-    shutil.copytree(
-        local_installation, pkg_build_path, ignore=ignore_paths_and_patterns
-    )
-    return pkg_build_path
+    # @classmethod
+    # def copy_sdist_into_build_dir(cls, local_installation: Path, build_dir: Path):
+    #     """Create a source distribution from a locally installed "editable" python package
+    #     and copy it into the build dir so it can be installed in the Docker image
+
+    #     Parameters
+    #     ----------
+    #     package_name : str
+    #         the name of the package (how it will be called in the docker image)
+    #     local_installation : Path
+    #         path to the local installation
+    #     build_dir : Path
+    #         path to the build directory
+
+    #     Returns
+    #     -------
+    #     Path
+    #         the path to the source distribution within the build directory
+    #     """
+    #     sdist_dir = build_dir / cls.PYTHON_PACKAGE_DIR
+    #     built = build_package(local_installation, sdist_dir, ["sdist"])
+    #     return sdist_dir / built[0]
 
+    def write_readme(self, dockerfile: DockerRenderer, build_dir):
+        """Generate Neurodocker instructions to install README file inside the docker
+        image
 
-DOCKERFILE_README_TEMPLATE = """
-    The following Docker image was generated by arcana v{} to enable the
-    commands to be run in the XNAT container service. See
-    https://raw.githubusercontent.com/Australian-Imaging-Service/arcana/main/LICENSE
-    for licence.
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        description : str
+            a description of what the pipeline does, to be inserted in a README file
+            in the Docker image
+        build_dir : Path
+            path to build dir
+        """
+        with open(build_dir / "README.md", "w") as f:
+            f.write(self.DOCKERFILE_README_TEMPLATE.format(__version__, self.readme))
+        dockerfile.copy(source=["./README.md"], destination="/README.md")
+
+    def asdict(self):
+        """Return a serialized version of the pipeline image specification that can be
+        written to file"""
+
+        def filter(attr, value):
+            return not isinstance(value, type(self)) and attr.metadata.get(
+                "asdict", True
+            )
 
-    {}
+        def serializer(_, attr, value):
+            if attr is not None and "serializer" in attr.metadata:
+                value = attr.metadata["serializer"](
+                    value,
+                    value_serializer=serializer,
+                    filter=filter,
+                )
+            elif isinstance(value, DataSpace):
+                if hasattr(self, "command") and self.command.DATA_SPACE:
+                    value = str(value)
+                else:
+                    value = value.tostr()
+            elif isinstance(value, PurePath):
+                # TODO: need better handling of saving checksums
+                # if value.exists():
+                #     fhash = hashlib.md5()
+                #     with open(value, "rb") as f:
+                #         # Calculate hash in chunks so we don't run out of memory for
+                #         # large files.
+                #         for chunk in iter(lambda: f.read(HASH_CHUNK_SIZE), b""):
+                #             fhash.update(chunk)
+                #     value = "checksum:" + fhash.hexdigest()
+                # else:
+                value = str(value)
+            elif isclass(value) or isfunction(value):
+                value = ClassResolver.tostr(value, strip_prefix=False)
+            return value
+
+        return attrs.asdict(self, value_serializer=serializer, filter=filter)
+
+    DOCKERFILE_README_TEMPLATE = """
+        The following Docker image was generated by Arcana v{} (https://arcana.readthedocs.io)
 
-    """
+        {}
 
-PATHS_TO_NOT_COPY_INTO_BUILD = "debug-build"
-PATTERNS_TO_NOT_COPY_INTO_BUILD = (
-    "conftest.py",
-    "*.pyc",
-    "__pycache__",
-    ".pytest_cache",
-    "tests",
-)
+        """
+
+    PYTHON_PACKAGE_DIR = "python-packages"
+    CONDA_ENV = "arcana"
```

### Comparing `arcana-2.0b0.dev7/arcana/core/mark.py` & `arcana-2.0b2/arcana/core/analysis/mark.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,78 @@
-from copy import copy
-import attrs
-from .analysis import _UnresolvedOp, make_analysis_class, _InheritedFrom, _MappedFrom
-from .enum import ColumnSalience, ParameterSalience, CheckSalience
-from arcana.exceptions import ArcanaDesignError
-
-
-PIPELINE_ANNOT = "__arcana_pipeline__"
-CONVERTER_ANNOT = "__arcana_converter__"
-SWICTH_ANNOT = "__arcana_switch__"
-CHECK_ANNOT = "__arcana_check__"
-
-ATTR_TYPE = "__arcana_type__"
+from __future__ import annotations
+from types import MemberDescriptorType
+from .spec import (
+    _UnresolvedOp,
+    _Inherited,
+    _MappedFrom,
+    ColumnSpec,
+    Parameter,
+    SubanalysisSpec,
+)
+from .make import make
+from .salience import ColumnSalience, ParameterSalience, CheckSalience
+from ..utils.misc import (
+    SWICTH_ANNOTATIONS,
+    CHECK_ANNOTATIONS,
+    PIPELINE_ANNOTATIONS,
+    CONVERTER_ANNOTATIONS,
+)
 
 
 def analysis(space: type):
     """Designate a class to be an analysis class
 
     Parameters
     ----------
     space : type (subclass of DataSpace)
         The data space the analysis operates on, see"""
 
-    def decorator(cls):
-        return make_analysis_class(cls, space)
+    def decorator(klass):
+        return make(klass, space)
 
     return decorator
 
 
 def column(
-    desc, row_frequency=None, salience=ColumnSalience.supplementary, metadata=None
+    desc,
+    row_frequency=None,
+    salience=ColumnSalience.supplementary,
+    metadata=None,
 ):
-    if metadata is None:
-        metadata = {}
-    else:
-        metadata = copy(metadata)
-    metadata.update(
-        {
-            ATTR_TYPE: "column",
-            "desc": desc,
-            "row_frequency": row_frequency,
-            "salience": salience,
-        }
-    )
-    return attrs.field(
-        default=None,
+    return ColumnSpec(
+        desc=desc,
+        row_frequency=row_frequency,
+        salience=salience,
         metadata=metadata,
     )
 
 
 def parameter(
     desc,
     default=None,
     choices=None,
     lower_bound=None,
     upper_bound=None,
     salience=ParameterSalience.recommended,
     metadata=None,
 ):
-    if choices is not None:
-        if upper_bound is not None or lower_bound is not None:
-            raise ArcanaDesignError(
-                f"Cannot specify lower ({lower_bound}) or upper ({lower_bound}) bound "
-                f"in conjunction with 'choices' arg ({choices})"
-            )
-    if metadata is None:
-        metadata = {}
-    else:
-        metadata = copy(metadata)
-    metadata.update(
-        {
-            ATTR_TYPE: "parameter",
-            "desc": desc,
-            "salience": salience,
-            "choices": choices,
-            "lower_bound": lower_bound,
-            "upper_bound": upper_bound,
-        }
-    )
-    return attrs.field(
+    return Parameter(
+        desc=desc,
         default=default,
-        validator=_parameter_validator,
+        choices=choices,
+        lower_bound=lower_bound,
+        upper_bound=upper_bound,
+        salience=salience,
         metadata=metadata,
     )
 
 
-def subanalysis(desc, **mappings):
-
-    return attrs.field(
-        metadata={
-            ATTR_TYPE: "subanalysis",
-            "desc": desc,
-            "mappings": tuple(mappings.items()),
-        },
-        init=False,
+def subanalysis(desc, metadata=None, **mappings):
+    return SubanalysisSpec(
+        desc=desc, mappings=tuple(mappings.items()), metadata=metadata
     )
 
 
 def pipeline(*outputs, condition=None, switch=None):
     """Decorate a instance method that adds nodes to an existing Pydra workflow
 
     Parameters
@@ -110,15 +86,15 @@
         name of a "switch" method in the analysis class, which selects nodes to be run
         with this pipeline instead of the default. If a tuple, then the first element
         is the switch name and the second is the return value it should match (the
         return value should be boolean otherwise)
     """
 
     def decorator(meth):
-        anots = meth.__annotations__[PIPELINE_ANNOT] = {}
+        anots = meth.__annotations__[PIPELINE_ANNOTATIONS] = {}
         anots["outputs"] = outputs
         anots["condition"] = condition
         anots["switch"] = switch.__name__ if switch is not None else None
         return meth
 
     return decorator
 
@@ -129,57 +105,53 @@
 
     Parameters
     ----------
     in_task : bool
         whether to wrap the switch in its own task or whether it adds its own nodes
         explicitly"""
     anot = meth.__annotations__
-    anot[SWICTH_ANNOT] = True
+    anot[SWICTH_ANNOTATIONS] = True
     return meth
 
 
 def check(column, salience=CheckSalience.prudent):
     """Decorate a method, which adds a quality control check to be run against a column"""
 
     def decorator(meth):
-        meth.__annotations__[CHECK_ANNOT] = {"column": column, "salience": salience}
-        return meth
-
-    return decorator
-
-
-def converter(output_format):
-    def decorator(meth):
-        anot = meth.__annotations__
-        anot[CONVERTER_ANNOT] = output_format
+        meth.__annotations__[CHECK_ANNOTATIONS] = {
+            "column": column,
+            "salience": salience,
+        }
         return meth
 
     return decorator
 
 
-def inherited_from(base_class, **to_overwrite):
+def inherit(ref: MemberDescriptorType = None, **to_overwrite):
     """Used to explicitly inherit a column or attribute from a base class so it can be
     used in a sub class. This explicit inheritance is enforced when the column/parameter
     is referenced in the base class in order to make the code more readable (i.e. so
     other developers can track where columns/parameters are defined)
 
     Parameters
     ----------
-    base_class : type
-        the base class to inherit the column/parameter from. The name will be matched
-        to the name of the column/parameter in the base class
+    ref : MemberDescriptorType, optional
+        a reference to the field that is being inherited from. Note that it is not
+        actually used for anything, the field to be inherited is determined by scanning
+        the method-resolution order for matching names, but it can make the code more
+        readable by linking the inherited attribute with its initial definition.
     **to_overwrite:
         any attributes to override from the inherited column/parameter
     """
     if "row_frequency" in to_overwrite:
         raise ValueError("Cannot overwrite row_frequency when inheriting")
-    return _InheritedFrom(base_class, to_overwrite)
+    return _Inherited(to_overwrite)
 
 
-def mapped_from(subanalysis_name, column_name, **to_overwrite):
+def map_from(subanalysis_name, column_name, **to_overwrite):
     """Used to explicitly inherit a column or attribute from a base class so it can be
     used in a sub class. This explicit inheritance is enforced when the column/parameter
     is referenced in the base class in order to make the code more readable (i.e. so
     other developers can track where columns/parameters are defined)
 
     Parameters
     ----------
@@ -208,25 +180,14 @@
         (
             column,
             in_format,
         ),
     )
 
 
-def _parameter_validator(_, attr, val):
-    if attr.metadata["choices"] is not None:
-        choices = attr.metadata["choices"]
-        if val not in choices:
-            raise ValueError(
-                f"{val} is not a valid value for '{attr.name}' parameter: {choices}"
-            )
-    else:
-        lower_bound = attr.metadata.get("lower_bound")
-        upper_bound = attr.metadata.get("upper_bound")
-        if not (
-            (lower_bound is None or val >= lower_bound)
-            and (upper_bound is None or val <= upper_bound)
-        ):
-            raise ValueError(
-                f"Value of '{attr.name}' ({val}) is not within the specified bounds: "
-                f"{lower_bound} - {upper_bound}"
-            )
+def converter(output_format):
+    def decorator(meth):
+        anot = meth.__annotations__
+        anot[CONVERTER_ANNOTATIONS] = output_format
+        return meth
+
+    return decorator
```

### Comparing `arcana-2.0b0.dev7/arcana/core/pipeline.py` & `arcana-2.0b2/arcana/core/analysis/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,139 +1,205 @@
 from __future__ import annotations
 import attrs
 import typing as ty
 from collections import OrderedDict
 from pathlib import Path
-from dataclasses import dataclass
 import logging
 from copy import copy, deepcopy
-from collections.abc import Iterable
 import attrs.converters
 import pydra.mark
 from pydra.engine.core import Workflow
 from arcana.exceptions import (
     ArcanaNameError,
     ArcanaUsageError,
     ArcanaDesignError,
     ArcanaPipelinesStackError,
     ArcanaOutputNotProducedException,
     ArcanaDataMatchError,
+    ArcanaFormatConversionError,
 )
-from .data.format import DataItem, FileGroup, Field
+from ..data.type.base import DataType, FileGroup, Field
 import arcana.core.data.set
 import arcana.core.data.row
-from .data.space import DataSpace
-from .utils import (
+from ..data.space import DataSpace
+from ..utils.misc import (
     func_task,
+    pydra_eq,
+    path2varname,
+    add_exc_note,
+)
+from ..utils.serialize import (
     asdict,
     fromdict,
     pydra_asdict,
     pydra_fromdict,
-    pydra_eq,
-    path2varname,
+    ClassResolver,
+    ObjectListConverter,
 )
 
+
 logger = logging.getLogger("arcana")
 
 
-@dataclass
-class Input:
-    col_name: str
-    pydra_field: str
-    required_format: type
+@attrs.define
+class PipelineField:
+    """Defines an input to a pipeline
 
+    Parameters
+    ----------
+    name : str
+        Name of the input and how it will be referred to in UI
+    field : str, optional
+        the name of the pydra input field to connect to, defaults to name
+    datatype : type, optional
+        the type of the items to be passed to the input, arcana.data.types.common.File by default
+    """
 
-@dataclass
-class Output:
-    col_name: str
-    pydra_field: str
-    produced_format: type
+    name: str
+    field: str = attrs.field()
+    datatype: type = attrs.field(
+        default=None,
+        converter=ClassResolver(
+            DataType,
+            allow_none=True,
+            alternative_types=[arcana.core.data.row.DataRow],
+        ),
+    )
+
+    @field.default
+    def field_default(self):
+        return self.name
+
+
+logger = logging.getLogger("arcana")
 
 
 @attrs.define
 class Pipeline:
     """A thin wrapper around a Pydra workflow to link it to sources and sinks
     within a dataset
 
     Parameters
     ----------
+    name : str
+        the name of the pipeline, used to differentiate it from others
     row_frequency : DataSpace, optional
         The row_frequency of the pipeline, i.e. the row_frequency of the
         derivatvies within the dataset, e.g. per-session, per-subject, etc,
         by default None
     workflow : Workflow
         The pydra workflow that performs the actual analysis
     inputs : Sequence[ty.Union[str, ty.Tuple[str, type]]]
         List of column names (i.e. either data sources or sinks) to be
         connected to the inputs of the pipeline. If the pipelines requires
-        the input to be in a format to the source, then it can be specified
+        the input to be in a datatype to the source, then it can be specified
         in a tuple (NAME, FORMAT)
     outputs : Sequence[ty.Union[str, ty.Tuple[str, type]]]
         List of sink names to be connected to the outputs of the pipeline
-        If the input to be in a specific format, then it can be provided in
+        If the input to be in a specific datatype, then it can be provided in
         a tuple (NAME, FORMAT)
     converter_args : dict[str, dict]
         keyword arguments passed on to the converter to control how the
         conversion is performed.
     dataset : Dataset
         the dataset the pipeline has been applied to
     """
 
     name: str = attrs.field()
     row_frequency: DataSpace = attrs.field()
     workflow: Workflow = attrs.field(eq=attrs.cmp_using(pydra_eq))
-    inputs: ty.List[Input] = attrs.field(
-        converter=lambda lst: [Input(*i) if isinstance(i, Iterable) else i for i in lst]
+    inputs: list[PipelineField] = attrs.field(
+        converter=ObjectListConverter(PipelineField)
     )
-    outputs: ty.List[Output] = attrs.field(
-        converter=lambda lst: [
-            Output(*o) if isinstance(o, Iterable) else o for o in lst
-        ]
+    outputs: list[PipelineField] = attrs.field(
+        converter=ObjectListConverter(PipelineField)
     )
     converter_args: ty.Dict[str, dict] = attrs.field(
         factory=dict, converter=attrs.converters.default_if_none(factory=dict)
     )
     dataset: arcana.core.data.set.Dataset = attrs.field(
         metadata={"asdict": False}, default=None, eq=False, hash=False
     )
 
+    def __attrs_post_init__(self):
+        for field in self.inputs + self.outputs:
+            if field.datatype is None:
+                field.datatype = self.dataset[field.name].datatype
+
     @inputs.validator
-    def inputs_validator(self, _, inpt):
-        if inpt.format == arcana.core.data.row.DataRow:  # special case
-            return
-        column = self.dataset.column[inpt.col_name]
-        inpt.required_format.find_converter(column.format)
-        if inpt.pydra_field not in self.workflow.input_names:
-            raise ArcanaNameError(
-                f"{inpt.pydra_field} is not in the input spec of '{self.name}' "
-                f"pipeline: " + "', '".join(self.workflow.input_names)
-            )
+    def inputs_validator(self, _, inputs: list[PipelineField]):
+        for inpt in inputs:
+            if inpt.datatype is arcana.core.data.row.DataRow:  # special case
+                continue
+            if self.dataset:
+                column = self.dataset[inpt.name]
+                # Check that a converter can be found if required
+                if inpt.datatype:
+                    try:
+                        inpt.datatype.find_converter(column.datatype)
+                    except ArcanaFormatConversionError as e:
+                        msg = (
+                            f"required to in conversion of '{inpt.name}' input "
+                            f"to '{self.name}' pipeline"
+                        )
+                        add_exc_note(e, msg)
+                        raise
+            elif inpt.datatype is None:
+                raise ValueError(
+                    f"Datatype must be explicitly set for {inpt.name} in unbound Pipeline"
+                )
+            if inpt.field not in self.workflow.input_names:
+                raise ArcanaNameError(
+                    inpt.field,
+                    f"{inpt.field} is not in the input spec of '{self.name}' "
+                    f"pipeline: " + "', '".join(self.workflow.input_names),
+                )
 
     @outputs.validator
-    def outputs_validator(self, _, outpt):
-        column = self.dataset.column[outpt.col_name]
-        if column.row_frequency != self.row_frequency:
-            raise ArcanaUsageError(
-                f"Pipeline row_frequency ('{str(self.row_frequency)}') doesn't match "
-                f"that of '{outpt.col_name}' output ('{str(self.row_frequency)}')"
-            )
-        column.format.find_converter(outpt.produced_format)
-        if outpt.pydra_field not in self.workflow.output_names:
-            raise ArcanaNameError(
-                f"{outpt.pydra_field} is not in the output spec of '{self.name}' "
-                f"pipeline: " + "', '".join(self.workflow.output_names)
-            )
+    def outputs_validator(self, _, outputs: list[PipelineField]):
+        for outpt in outputs:
+            if self.dataset:
+                column = self.dataset[outpt.name]
+                if column.row_frequency != self.row_frequency:
+                    raise ArcanaUsageError(
+                        f"Pipeline row_frequency ('{str(self.row_frequency)}') doesn't match "
+                        f"that of '{outpt.name}' output ('{str(self.row_frequency)}')"
+                    )
+                # Check that a converter can be found if required
+                if outpt.datatype:
+                    try:
+                        column.datatype.find_converter(outpt.datatype)
+                    except ArcanaFormatConversionError as e:
+                        msg = (
+                            f"required to in conversion of '{outpt.name}' output "
+                            f"from '{self.name}' pipeline"
+                        )
+                        add_exc_note(e, msg)
+                        raise
+            elif outpt.datatype is None:
+                raise ValueError(
+                    f"Datatype must be explicitly set for {outpt.name} in unbound Pipeline"
+                )
+            if outpt.field not in self.workflow.output_names:
+                raise ArcanaNameError(
+                    f"{outpt.field} is not in the output spec of '{self.name}' "
+                    f"pipeline: " + "', '".join(self.workflow.output_names)
+                )
 
     @property
     def input_varnames(self):
-        return [path2varname(i.col_name) for i in self.inputs]
+        return [
+            i.name for i in self.inputs
+        ]  # [path2varname(i.name) for i in self.inputs]
 
     @property
     def output_varnames(self):
-        return [path2varname(o.col_name) for o in self.outputs]
+        return [
+            o.name for o in self.outputs
+        ]  # [path2varname(o.name) for o in self.outputs]
 
     # parameterisation = self.get_parameterisation(kwargs)
     # self.wf.to_process.inputs.parameterisation = parameterisation
     # self.wf.per_node.source.inputs.parameterisation = parameterisation
 
     def __call__(self, **kwargs):
         """
@@ -185,70 +251,72 @@
 
         # Automatically output interface for source node to include sourced
         # columns
         source_out_dct = {}
         for inpt in self.inputs:
             # If the row frequency of the column is not a parent of the pipeline
             # then the input will be a sequence of all the child rows
-            if inpt.required_format is arcana.core.data.row.DataRow:
+            if inpt.datatype is arcana.core.data.row.DataRow:
                 dtype = arcana.core.data.row.DataRow
-            elif self.dataset[inpt.col_name].row_frequency.is_parent(
-                self.row_frequency, if_match=True
-            ):
-                dtype = inpt.required_format
             else:
-                dtype = ty.Sequence[inpt.required_format]
-            source_out_dct[inpt.col_name] = dtype
+                dtype = self.dataset[inpt.name].datatype
+                # If the row frequency of the source column is higher than the frequency
+                # of the pipeline, then the related elements of the source column are
+                # collected into a list and passed to the pipeline
+                if not self.dataset[inpt.name].row_frequency.is_parent(
+                    self.row_frequency, if_match=True
+                ):
+                    dtype = list[dtype]
+            source_out_dct[inpt.name] = dtype
         source_out_dct["provenance_"] = ty.Dict[str, ty.Any]
 
         wf.per_row.add(
             func_task(
                 source_items,
                 in_fields=[
                     ("dataset", arcana.core.data.set.Dataset),
                     ("row_frequency", DataSpace),
                     ("id", str),
-                    ("inputs", ty.Sequence[Input]),
+                    ("inputs", ty.List[PipelineField]),
                     ("parameterisation", ty.Dict[str, ty.Any]),
                 ],
                 out_fields=list(source_out_dct.items()),
                 name="source",
                 dataset=self.dataset,
                 row_frequency=self.row_frequency,
                 inputs=self.inputs,
                 id=wf.per_row.lzin.id,
             )
         )
 
         # Set the inputs
         sourced = {
-            i.col_name: getattr(wf.per_row.source.lzout, i.col_name)
-            for i in self.inputs
+            i.name: getattr(wf.per_row.source.lzout, i.name) for i in self.inputs
         }
 
-        # Do input format conversions if required
+        # Do input datatype conversions if required
         for inpt in self.inputs:
-            if inpt.required_format == arcana.core.data.row.DataRow:
+            if inpt.datatype == arcana.core.data.row.DataRow:
                 continue
-            stored_format = self.dataset[inpt.col_name].format
+            stored_format = self.dataset[inpt.name].datatype
             if not (
-                inpt.required_format is stored_format
-                or issubclass(stored_format, inpt.required_format)
+                inpt.datatype is stored_format
+                or issubclass(stored_format, inpt.datatype)
             ):
                 logger.info(
                     "Adding implicit conversion for input '%s' " "from %s to %s",
-                    inpt.col_name,
+                    inpt.name,
                     stored_format.class_name(),
-                    inpt.required_format.class_name(),
+                    inpt.datatype.class_name(),
                 )
-                source_name = inpt.col_name
-                converter = inpt.required_format.converter_task(
+                source_name = inpt.name
+                converter = inpt.datatype.converter_task(
                     stored_format,
                     name=f"{source_name}_input_converter",
-                    **self.converter_args.get(inpt.col_name, {}),
+                    **self.converter_args.get(inpt.name, {}),
                 )
                 converter.inputs.to_convert = sourced.pop(source_name)
                 if issubclass(source_out_dct[source_name], ty.Sequence):
                     # Iterate over all items in the sequence and convert them
                     # separately
                     converter.split("to_convert")
                 # Insert converter
@@ -257,76 +325,79 @@
                 sourced[source_name] = converter.lzout.converted
 
         # Create identity row to accept connections from user-defined rows
         # via `set_output` method
         wf.per_row.add(
             func_task(
                 access_paths_and_values,
-                in_fields=[(i.col_name, DataItem) for i in self.inputs],
-                out_fields=[(i.col_name, ty.Any) for i in self.inputs],
+                in_fields=[
+                    (i.name, ty.Union[DataType, arcana.core.data.row.DataRow])
+                    for i in self.inputs
+                ],
+                out_fields=[(i.name, ty.Any) for i in self.inputs],
                 name="input_interface",
                 **sourced,
             )
         )
 
         # Add the "inner" workflow of the pipeline that actually performs the
         # analysis/processing
         wf.per_row.add(deepcopy(self.workflow))
         # Make connections to "inner" workflow
         for inpt in self.inputs:
             setattr(
                 getattr(wf.per_row, self.workflow.name).inputs,
-                inpt.pydra_field,
-                getattr(wf.per_row.input_interface.lzout, inpt.col_name),
+                inpt.field,
+                getattr(wf.per_row.input_interface.lzout, inpt.name),
             )
 
         # Creates a row to accept values from user-defined rows and
-        # encapsulate them into DataItems
+        # encapsulate them into DataTypes
         wf.per_row.add(
             func_task(
                 encapsulate_paths_and_values,
-                in_fields=[("outputs", ty.Dict[str, type])]
-                + [(o, ty.Any) for o in self.output_varnames],
-                out_fields=[(o, DataItem) for o in self.output_varnames],
+                in_fields=[("outputs", ty.List[PipelineField])]
+                + [(o.name, ty.Union[str, Path]) for o in self.outputs],
+                out_fields=[(o.name, DataType) for o in self.outputs],
                 name="output_interface",
                 outputs=self.outputs,
                 **{
-                    o.col_name: getattr(
-                        getattr(wf.per_row, self.workflow.name).lzout, o.pydra_field
+                    o.name: getattr(
+                        getattr(wf.per_row, self.workflow.name).lzout, o.field
                     )
                     for o in self.outputs
                 },
             )
         )
 
-        # Set format converters where required
+        # Set datatype converters where required
         to_sink = {
             o: getattr(wf.per_row.output_interface.lzout, o)
             for o in self.output_varnames
         }
 
-        # Do output format conversions if required
+        # Do output datatype conversions if required
         for outpt in self.outputs:
-            stored_format = self.dataset[outpt.col_name].format
+            stored_format = self.dataset[outpt.name].datatype
             if not (
-                outpt.produced_format is stored_format
-                or issubclass(outpt.produced_format, stored_format)
+                outpt.datatype is stored_format
+                or issubclass(outpt.datatype, stored_format)
             ):
                 logger.info(
                     "Adding implicit conversion for output '%s' " "from %s to %s",
-                    outpt.col_name,
-                    outpt.produced_format.class_name(),
+                    outpt.name,
+                    outpt.datatype.class_name(),
                     stored_format.class_name(),
                 )
                 # Insert converter
-                sink_name = path2varname(outpt.col_name)
+                sink_name = path2varname(outpt.name)
                 converter = stored_format.converter_task(
-                    outpt.produced_format,
+                    outpt.datatype,
                     name=f"{sink_name}_output_converter",
-                    **self.converter_args.get(outpt.col_name, {}),
+                    **self.converter_args.get(outpt.name, {}),
                 )
                 converter.inputs.to_convert = to_sink.pop(sink_name)
                 wf.per_row.add(converter)
                 # Map converter output to workflow output
                 to_sink[sink_name] = converter.lzout.converted
 
         # Can't use a decorated function as we need to allow for dynamic
@@ -337,15 +408,15 @@
                 in_fields=(
                     [
                         ("dataset", arcana.core.data.set.Dataset),
                         ("row_frequency", DataSpace),
                         ("id", str),
                         ("provenance", ty.Dict[str, ty.Any]),
                     ]
-                    + [(s, DataItem) for s in to_sink]
+                    + [(s, DataType) for s in to_sink]
                 ),
                 out_fields=[("id", str)],
                 name="sink",
                 dataset=self.dataset,
                 row_frequency=self.row_frequency,
                 id=wf.per_row.lzin.id,
                 provenance=wf.per_row.source.lzout.provenance_,
@@ -448,15 +519,15 @@
                 to_produce.append(sink)
             else:
                 to_produce = []
             # Add the pipeline to the stack
             stack[pipeline.name] = pipeline, to_produce
             # Recursively add all the pipeline's prerequisite pipelines to the stack
             for inpt in pipeline.inputs:
-                inpt_column = sink.dataset[inpt.col_name]
+                inpt_column = sink.dataset[inpt.name]
                 if inpt_column.is_sink:
                     try:
                         push_pipeline_on_stack(
                             inpt_column,
                             downstream=[(pipeline, to_produce)] + downstream,
                         )
                     except ArcanaPipelinesStackError as e:
@@ -482,45 +553,42 @@
 
 def split_side_car_suffix(name):
     """Splits the basename from a side car sufix (as combined by `append_side_car_suffix`"""
     return name.split("__o__")
 
 
 @pydra.mark.task
-@pydra.mark.annotate(
-    {
-        "dataset": arcana.core.data.set.Dataset,
-        "row_frequency": DataSpace,
-        "outputs": ty.Sequence[str],
-        "requested_ids": ty.Sequence[str] or None,
-        "parameterisation": ty.Dict[str, ty.Any],
-        "return": {"ids": ty.List[str], "cant_process": ty.List[str]},
-    }
-)
-def to_process(dataset, row_frequency, outputs, requested_ids, parameterisation):
+@pydra.mark.annotate({"return": {"ids": ty.List[str], "cant_process": ty.List[str]}})
+def to_process(
+    dataset: arcana.core.data.set.Dataset,
+    row_frequency: DataSpace,
+    outputs: ty.List[PipelineField],
+    requested_ids: ty.Union[list[str], None],
+    parameterisation: dict[str, ty.Any],
+):
     if requested_ids is None:
         requested_ids = dataset.row_ids(row_frequency)
     ids = []
     cant_process = []
     for row in dataset.rows(row_frequency, ids=requested_ids):
         # TODO: Should check provenance of existing rows to see if it matches
-        not_exist = [not row[o.col_name].exists for o in outputs]
+        not_exist = [not row[o.name].exists for o in outputs]
         if all(not_exist):
             ids.append(row.id)
         elif any(not_exist):
             cant_process.append(row.id)
     logger.debug("Found %s ids to process, and can't process %s", ids, cant_process)
     return ids, cant_process
 
 
 def source_items(
     dataset: arcana.core.data.set.Dataset,
     row_frequency: DataSpace,
     id: str,
-    inputs: ty.List[Input],
+    inputs: ty.List[PipelineField],
     parameterisation: dict,
 ):
     """Selects the items from the dataset corresponding to the input
     sources and retrieves them from the store to a cache on
     the host
 
     Parameters
@@ -537,23 +605,23 @@
     logger.debug("Sourcing %s", inputs)
     provenance = copy(parameterisation)
     sourced = []
     row = dataset.row(row_frequency, id)
     with dataset.store:
         missing_inputs = {}
         for inpt in inputs:
-            # If the required format is of type DataRow then provide the whole
+            # If the required datatype is of type DataRow then provide the whole
             # row to the pipeline input
-            if inpt.required_format == arcana.core.data.row.DataRow:
+            if inpt.datatype == arcana.core.data.row.DataRow:
                 sourced.append(row)
                 continue
             try:
-                item = row[inpt.col_name]
+                item = row[inpt.name]
             except ArcanaDataMatchError as e:
-                missing_inputs[inpt.col_name] = str(e)
+                missing_inputs[inpt.name] = str(e)
             else:
                 item.get()  # download to host if required
                 sourced.append(item)
         if missing_inputs:
             raise ArcanaDataMatchError("\n\n" + "\n\n".join(missing_inputs.values()))
     return tuple(sourced) + (provenance,)
 
@@ -567,15 +635,15 @@
         the dataset to source the data from
     row_frequency : DataSpace
         the frequency of the row to source the data from
     id : str
         the ID of the row to source from
     provenance : dict
         provenance information to be stored alongside the generated data
-    **to_sink : dict[str, DataItem]
+    **to_sink : dict[str, DataType]
         data items to be stored in the data store
     """
     logger.debug("Sinking %s", to_sink)
     row = dataset.row(row_frequency, id)
     with dataset.store:
         for outpt_name, output in to_sink.items():
             row_item = row[outpt_name]
@@ -601,19 +669,19 @@
 
 def encapsulate_paths_and_values(outputs, **kwargs):
     """Copies files into the CWD renaming so the basenames match
     except for extensions"""
     logger.debug("Encapsulating %s into %s", kwargs, outputs)
     items = []
     for outpt in outputs:
-        val = kwargs[outpt.col_name]
-        if issubclass(outpt.produced_format, FileGroup):
-            obj = outpt.produced_format.from_fs_path(val)
+        val = kwargs[outpt.name]
+        if issubclass(outpt.datatype, FileGroup):
+            obj = outpt.datatype.from_fs_path(val)
         else:
-            obj = outpt.produced_format(val)
+            obj = outpt.datatype(val)
         items.append(obj)
     if len(items) > 1:
         return tuple(items)
     elif items:
         return items[0]
     else:
         return None
@@ -628,28 +696,28 @@
 #     constrained to the name_paths passed to the 'include' kwarg, with the
 #     exception of sub-name_paths passed to the 'exclude' kwarg
 
 #     Parameters
 #     ----------
 #     other : Provenance
 #         The provenance object to compare against
-#     include : ty.List[ty.List[str]] | None
+#     include : list[list[str]] | None
 #         Paths in the provenance to include in the match. If None all are
 #         incluced
-#     exclude : ty.List[ty.List[str]] | None
+#     exclude : list[list[str]] | None
 #         Paths in the provenance to exclude from the match. In None all are
 #         excluded
 #     """
 #     if include is not None:
 #         include_res = [self._gen_prov_path_regex(p) for p in include]
 #     if exclude is not None:
 #         exclude_res = [self._gen_prov_path_regex(p) for p in exclude]
 #     diff = DeepDiff(self._prov, other._prov, ignore_order=True)
 #     # Create regular expressions for the include and exclude name_paths in
-#     # the format that deepdiff uses for nested dictionary/lists
+#     # the datatype that deepdiff uses for nested dictionary/lists
 
 #     def include_change(change):
 #         if include is None:
 #             included = True
 #         else:
 #             included = any(rx.match(change) for rx in include_res)
 #         if included and exclude is not None:
```

### Comparing `arcana-2.0b0.dev7/arcana/data/formats/common.py` & `arcana-2.0b2/arcana/common/data/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from abc import ABCMeta
 import zipfile
-from arcana.core.data.format import FileGroup, BaseFile, BaseDirectory
-from arcana.core.mark import converter
-from arcana.tasks.common.archive import create_tar, extract_tar, create_zip, extract_zip
+from arcana.core.data.type.base import FileGroup
+from arcana.core.data.type import BaseFile, BaseDirectory
+from arcana.mark import converter
+from arcana.common.analysis.tasks.archive import (
+    create_tar,
+    extract_tar,
+    create_zip,
+    extract_zip,
+)
 
 
 # Compressed formats
 class Zip(BaseFile):
     ext = "zip"
 
     @classmethod
@@ -65,17 +71,14 @@
     @converter(TarGz)
     def untargz(cls, fs_path):
         node = extract_tar(in_file=fs_path)
         return node, node.lzout.out_file
 
 
 class Directory(BaseDirectory):
-
-    ext = ""
-
     @classmethod
     @converter(Zip)
     def unzip(cls, fs_path):
         node = extract_zip(in_file=fs_path)
         return node, node.lzout.out_file
 
     @classmethod
```

### Comparing `arcana-2.0b0.dev7/arcana/data/stores/common/file_system.py` & `arcana-2.0b2/arcana/common/data/file_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 import logging
 import json
 import attrs
 import yaml
 from fasteners import InterProcessLock
 from arcana.exceptions import ArcanaMissingDataException, ArcanaUsageError
 from arcana.core.data.set import Dataset
-from arcana.data.spaces.medimage import Clinical, DataSpace
+
+# from arcana.data.spaces.medimage import Clinical, DataSpace
 from arcana.core.data.store import DataStore
-from arcana.core.data.format import FileGroup
+from arcana.core.data.type.base import FileGroup
+from arcana.core.utils.misc import get_home_dir
+from arcana.common.data.spaces import Samples
 
 
 logger = logging.getLogger("arcana")
 
 
 # Matches directory names used for summary rows with dunder beginning and
 # end (e.g. '__visit_01__') and hidden directories (i.e. starting with '.' or
@@ -45,14 +48,15 @@
     alias = "file"
     PROV_SUFFIX = ".prov"
     FIELDS_FNAME = "__fields__.json"
     LOCK_SUFFIX = ".lock"
     PROV_KEY = "__provenance__"
     VALUE_KEY = "__value__"
     METADATA_DIR = ".arcana"
+    SITE_LICENSES_DIR = "site-licenses"
 
     def new_dataset(self, id, *args, **kwargs):
         if not Path(id).exists():
             raise ArcanaUsageError(f"Path to dataset root '{id}'' does not exist")
         return super().new_dataset(id, *args, **kwargs)
 
     def save_dataset_definition(self, dataset_id, definition, name):
@@ -97,17 +101,17 @@
         """
         self.cast_value(self.get_field_val(field))
 
     def cast_value(self, val, field):
         if isinstance(val, dict):
             val = val[self.VALUE_KEY]
         if field.array:
-            val = [field.format(v) for v in val]
+            val = [field.datatype(v) for v in val]
         else:
-            val = field.format(val)
+            val = field.datatype(val)
         return val
 
     def put_file_group_paths(self, file_group: FileGroup, fs_paths: ty.List[Path]):
         """
         Inserts or updates a file_group in the store
         """
         stem_path = self.file_group_stem_path(file_group)
@@ -252,15 +256,15 @@
         for layer in row.dataset.hierarchy:
             if not (layer.is_parent(row.frequency) or layer == row.frequency):
                 break
             path /= row.ids[layer]
             accounted_freq |= layer
         # If not "leaf row" then
         if row.frequency != max(row.dataset.space):
-            unaccounted_freq = row.frequency - (row.frequency & accounted_freq)
+            unaccounted_freq = (row.frequency ^ accounted_freq) & row.frequency
             unaccounted_id = row.ids[unaccounted_freq]
             if unaccounted_id is None:
                 path /= f"__{unaccounted_freq}__"
             elif isinstance(unaccounted_id, str):
                 path /= f"__{unaccounted_freq}_{unaccounted_id}__"
             else:
                 path /= f"__{unaccounted_freq}_" + "_".join(unaccounted_id) + "__"
@@ -275,43 +279,54 @@
 
     def fields_json_path(self, field):
         return self.root_dir(field.row) / self.row_path(field.row) / self.FIELDS_FNAME
 
     def prov_json_path(self, file_group):
         return self.file_group_path(file_group) + self.PROV_SUFFX
 
-    def get_provenance(self, item):
-        if item.is_file_group:
-            prov = self._get_file_group_provenance(item)
-        else:
-            prov = self._get_field_provenance(item)
-        return prov
-
-    def _get_file_group_provenance(self, file_group):
-        if file_group.fs_path is not None:
-            prov_path = self.prov_json_path(file_group)
-            if prov_path.exists():
-                with open(prov_path) as f:
-                    provenance = json.load(f)
-            else:
-                provenance = {}
-        else:
-            provenance = None
-        return provenance
-
-    def _get_field_provenance(self, field):
-        """
-        Loads the fields provenance from the JSON dictionary
-        """
-        val_dct = self.get_field_val(field)
-        if isinstance(val_dct, dict):
-            prov = val_dct.get(self.PROV_KEY)
-        else:
-            prov = None
-        return prov
+    def site_licenses_dataset(self):
+        """Provide a place to store hold site-wide licenses"""
+        dataset_root = get_home_dir() / self.SITE_LICENSES_DIR
+        if not dataset_root.exists():
+            dataset_root.mkdir(parents=True)
+        try:
+            dataset = self.load_dataset(dataset_root)
+        except KeyError:
+            dataset = self.new_dataset(dataset_root, space=Samples)
+        return dataset
+
+    # def get_provenance(self, item):
+    #     if item.is_file_group:
+    #         prov = self._get_file_group_provenance(item)
+    #     else:
+    #         prov = self._get_field_provenance(item)
+    #     return prov
+
+    # def _get_file_group_provenance(self, file_group):
+    #     if file_group.fs_path is not None:
+    #         prov_path = self.prov_json_path(file_group)
+    #         if prov_path.exists():
+    #             with open(prov_path) as f:
+    #                 provenance = json.load(f)
+    #         else:
+    #             provenance = {}
+    #     else:
+    #         provenance = None
+    #     return provenance
+
+    # def _get_field_provenance(self, field):
+    #     """
+    #     Loads the fields provenance from the JSON dictionary
+    #     """
+    #     val_dct = self.get_field_val(field)
+    #     if isinstance(val_dct, dict):
+    #         prov = val_dct.get(self.PROV_KEY)
+    #     else:
+    #         prov = None
+    #     return prov
 
     def get_field_val(self, field):
         """
         Load fields JSON, locking to prevent read/write conflicts
         Would be better if only checked if locked to allow
         concurrent reads but not possible with multi-process
         locks (in my understanding at least).
@@ -333,25 +348,25 @@
             except AttributeError:
                 pass
             raise ArcanaMissingDataException(
                 "{} does not exist in the local store {}".format(field.name, self)
             )
 
 
-def single_dataset(
-    path: str, tree_dimensions: DataSpace = Clinical, **kwargs
-) -> Dataset:
-    """
-    Creates a Dataset from a file system path to a directory
-
-    Parameters
-    ----------
-    path : str
-        Path to directory containing the dataset
-    tree_dimensions : type
-        The enum class that defines the directory tree dimensions of the
-        stores
-    """
-
-    return FileSystem(op.join(path, ".."), **kwargs).dataset(
-        op.basename(path), tree_dimensions
-    )
+# def single_dataset(
+#     path: str, tree_dimensions: DataSpace = Clinical, **kwargs
+# ) -> Dataset:
+#     """
+#     Creates a Dataset from a file system path to a directory
+
+#     Parameters
+#     ----------
+#     path : str
+#         Path to directory containing the dataset
+#     tree_dimensions : type
+#         The enum class that defines the directory tree dimensions of the
+#         stores
+#     """
+
+#     return FileSystem(op.join(path, ".."), **kwargs).dataset(
+#         op.basename(path), tree_dimensions
+#     )
```

### Comparing `arcana-2.0b0.dev7/arcana/deploy/medimage/xnat.py` & `arcana-2.0b2/arcana/core/deploy/image/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,636 +1,549 @@
-import sys
-import re
+from __future__ import annotations
 import typing as ty
 from pathlib import Path
-import tempfile
-import inspect
-import json
-from attr import NOTHING
-from dataclasses import dataclass
+from itertools import chain
+import re
+import logging
+import shlex
+import shutil
+import attrs
+import yaml
+from urllib.parse import urlparse
+from deepdiff import DeepDiff
 from neurodocker.reproenv import DockerRenderer
 from arcana import __version__
-from arcana.core.data.format import FileGroup
-import arcana.data.formats.common
-from arcana.data.spaces.medimage import Clinical
-from arcana.data.stores.medimage import XnatViaCS
-import arcana.core.data.row
-from arcana.core.deploy.build import construct_dockerfile, dockerfile_build, CONDA_ENV
-from arcana.core.deploy.utils import DOCKER_HUB
-from arcana.core.utils import resolve_class, class_location, path2varname
-from arcana.core.data.store import DataStore
-from arcana.exceptions import ArcanaUsageError
-
-
-def path2xnatname(path):
-    return re.sub(r"[^a-zA-Z0-9_]+", "_", path)
-
-
-IN_DOCKER_ARCANA_HOME_DIR = "/arcana-home"
-
-
-def build_xnat_cs_image(
-    image_tag: str,
-    commands: ty.List[ty.Dict[str, ty.Any]],
-    authors: ty.List[ty.Tuple[str, str]],
-    info_url: str,
-    docker_registry: str = DOCKER_HUB,
-    build_dir: Path = None,
-    test_config: bool = False,
-    generate_only: bool = False,
-    pkg_version: str = None,  # Ignored here, just included to allow specs to be passed directly as kwargs
-    wrapper_version: str = None,  # ditto
-    **kwargs,
-):
-    """Creates a Docker image containing one or more XNAT commands ready
-    to be installed in XNAT's container service plugin
+from arcana.core.utils.serialize import (
+    ObjectConverter,
+    ObjectListConverter,
+    ClassResolver,
+)
+from arcana.core.data.type import BaseDirectory
+from ..command.base import ContainerCommand
+from .base import ArcanaImage
+from .components import ContainerAuthor, License, KnownIssue
+
+
+logger = logging.getLogger("arcana")
+
+
+@attrs.define(kw_only=True)
+class App(ArcanaImage):
+    """A container image that contains a command with specific inputs and outputs to run.
 
     Parameters
     ----------
-    image_tag : str
-        Tag to name the built Docker image with
-    commands: dict[str, Any]
-        List of command specifications (in dicts) to be installed on the
-        image, see `generate_xnat_command` for valid args (dictionary keys).
-    authors : list[str]
-        Names and emails of the maintainers of the wrapper pipeline
+    name : str
+        name of the package/pipeline
+    version : str
+        version of the package/pipeline
+    org : str
+        the organisation the image will be tagged within
+    base_image : BaseImage, optional
+        the base image to build from
+    packages : Packages, optional
+        the package manager used to install system packages (should match OS on base image)
+    registry : str, optional
+        the container registry the image is to be installed at
     info_url : str
-        The URL of the package website explaining the analysis software
-        and what it does
-    docker_registry : str
-        The Docker registry the image will be uploaded to
-    wrapper_version : str
-        The version of the wrapper specific to the pkg version. It will be
-        appended to the package version, e.g. 0.16.2 -> 0.16.2--1
-    build_dir : Path
-        the directory to build the docker image within, i.e. where to write
-        Dockerfile and supporting files to be copied within the image
-    test_config : bool
-        whether to create the container so that it will work with the test
-        XNAT configuration (i.e. hard-coding the XNAT server IP)
-    pkg_version : str, optional
-        ignored by function, just included to allow specs to be passed directly
-        as kwargs **specs
-    wrapper_version : str, optional
-        ignored by function, just included to allow specs to be passed directly
-        as kwargs as **specs
-    **kwargs:
-        Passed on to `construct_dockerfile` method
-
-    Returns
-    -------
-    DockerRenderer
-        the Neurodocker renderer
-    Path
-        path to build directory
+        the url of a documentation page describing the package
+    authors : list[ContainerAuthor]
+        list of authors of the package
+    description : str
+        single line description to be when referring to the pipeline in UIs
+    command : ContainerCommand
+        description of the command that is to be run within the image
+    licenses : list[dict[str, str]], optional
+        specification of licenses required by the commands in the container. Each dict
+        should contain the 'name' of the license and the 'destination' it should be
+        installed inside the container.
+    build_iteration : str, optional
+        version of the specification relative to the package version, i.e. if the package
+        version hasn't been updated but the specification has been altered, the spec
+        version should be updated (otherwise builds will fail). The spec version should
+        reset to "0" if the package version is updated.
+    long_description : str
+        Multi-line description of the pipeline used in documentation
+    known_issues : dict
+        Any known issues with the pipeline. To be used in auto-doc generation
+    loaded_from : Path
+        the file the spec was loaded from, if applicable
     """
-    # Save a snapshot of the arguments to this function in a dict to save
-    # within the built image
-    ARGS_TO_IGNORE = [
-        "kwargs",
-        "build_dir",
-        "generate_only",
-        "license_dir",
-        "pkg_version",
-        "wrapper_version",
-    ]
-    spec = {k: v for k, v in kwargs.items() if k not in ARGS_TO_IGNORE}
-    for argname in inspect.signature(build_xnat_cs_image).parameters:
-        if argname not in ARGS_TO_IGNORE:
-            spec[argname] = locals()[argname]
-    spec["arcana_version"] = __version__
-
-    if build_dir is None:
-        build_dir = tempfile.mkdtemp()
-    build_dir = Path(build_dir)
 
-    xnat_commands = []
-    for cmd_spec in commands:
+    SPEC_PATH = "/arcana-spec.yaml"
+    IN_DOCKER_ARCANA_HOME_DIR = "/arcana-home"
+
+    DEFAULT_PACKAGE = "arcana.deploy"
+
+    info_url: str = attrs.field()
+    authors: ty.List[ContainerAuthor] = attrs.field(
+        converter=ObjectListConverter(ContainerAuthor),
+        metadata={"serializer": ObjectListConverter.asdict},
+    )
+    description: str
+    command: ContainerCommand = attrs.field(converter=ObjectConverter(ContainerCommand))
+    licenses: list[License] = attrs.field(
+        factory=dict,
+        converter=ObjectListConverter(License),
+        metadata={"serializer": ObjectListConverter.asdict},
+    )
+    known_issues: list[KnownIssue] = attrs.field(
+        factory=list,
+        converter=ObjectListConverter(KnownIssue),
+        metadata={"serializer": ObjectListConverter.asdict},
+    )
+    long_description: str = ""
+    loaded_from: Path = attrs.field(default=None, metadata={"asdict": False})
+    arcana_version: str = __version__
+
+    def __attrs_post_init__(self):
+
+        # Set back-references to this image in the command spec
+        self.command.image = self
+
+    @info_url.validator
+    def info_url_validator(self, _, info_url):
+        parsed = urlparse(info_url)
+        if not parsed.scheme or not parsed.netloc:
+            raise ValueError(
+                f"Could not parse info url '{info_url}', please include URL scheme"
+            )
 
-        if "info_url" not in cmd_spec:
-            cmd_spec["info_url"] = info_url
+    def add_entrypoint(self, dockerfile: DockerRenderer, build_dir: Path):
 
-        xnat_cmd = generate_xnat_cs_command(
-            image_tag=image_tag, registry=docker_registry, **cmd_spec
+        command_line = (
+            self.command.activate_conda_cmd() + "arcana deploy pipeline-entrypoint"
         )
 
-        xnat_commands.append(xnat_cmd)
+        dockerfile.entrypoint(shlex.split(command_line))
 
-    # Convert XNAT command label into string that can by placed inside the
-    # Docker label
-    command_label = json.dumps(xnat_commands).replace("$", r"\$")
-
-    dockerfile = construct_dockerfile(
-        build_dir,
-        labels={"org.nrg.commands": command_label, "maintainer": authors[0]},
-        spec=spec,
-        **kwargs,
-    )
+    def construct_dockerfile(self, build_dir: Path, **kwargs) -> DockerRenderer:
+        """Constructs a dockerfile that wraps a with dependencies
 
-    # Copy the generated XNAT commands inside the container for ease of reference
-    copy_command_ref(dockerfile, xnat_commands, build_dir)
+        Parameters
+        ----------
+        build_dir : Path
+            Path to the directory the Dockerfile will be written into copy any local
+            files to
+        **kwargs
+            Passed onto the ArcanaImage.construct_dockerfile() method
+
+        Returns
+        -------
+        DockerRenderer
+            Neurodocker Docker renderer to construct dockerfile from
+        """
+
+        dockerfile = super().construct_dockerfile(build_dir, **kwargs)
+
+        self.install_licenses(
+            dockerfile,
+            build_dir,
+        )
 
-    save_store_config(dockerfile, build_dir, test_config=test_config)
+        self.insert_spec(dockerfile, build_dir)
 
-    if not generate_only:
-        dockerfile_build(dockerfile, build_dir, image_tag)
+        self.add_entrypoint(dockerfile, build_dir)
 
-    return dockerfile, build_dir
-
-
-def generate_xnat_cs_command(
-    name: str,
-    pydra_task: str,
-    image_tag: str,
-    inputs,
-    outputs,
-    description: str,
-    version: str,
-    info_url: str,
-    parameters=None,
-    configuration=None,
-    row_frequency="session",
-    registry=DOCKER_HUB,
-    long_description: str = None,
-):
-    """Constructs the XNAT CS "command" JSON config, which specifies how XNAT
-    should handle the containerised pipeline
+        return dockerfile
 
-    Parameters
-    ----------
-    name : str
-        Name of the container service pipeline
-    pydra_task
-        The module path and name (separated by ':') to the Pydra task, or function
-        that returns a Pydra Workflow, to execute, e.g. arcana.tasks.bids:bids_app
-    image_tag : str
-        Name + version of the Docker image to be created
-    inputs : ty.List[ty.Union[InputArg, tuple]]
-        Inputs to be provided to the container (pydra_field, format, name, row_frequency).
-        'pydra_field' and 'format' will be passed to "inputs" arg of the Dataset.pipeline() method,
-        'row_frequency' to the Dataset.add_source() method and 'name' is displayed in the XNAT
-        UI
-    outputs : ty.List[ty.Union[OutputArg, tuple]]
-        Outputs to extract from the container (pydra_field, format, output_path).
-        'pydra_field' and 'format' will be passed as "outputs" arg the Dataset.pipeline() method,
-        'output_path' determines the path the output will saved in the XNAT data tree.
-    description : str
-        User-facing description of the pipeline
-    version : str
-        Version string for the wrapped pipeline
-    info_url : str
-        URI explaining in detail what the pipeline does
-    parameters : ty.List[str]
-        Parameters to be exposed in the CS command
-    row_frequency : str
-        Frequency of the pipeline to generate (can be either 'dataset' or 'session' currently)
-    registry : str
-        URI of the Docker registry to upload the image to
-    configuration : dict[str, Any]
-        Fixed arguments passed to the workflow at initialisation. Can be used to specify
-        the input fields of the workflow/task
-    long_description : str
-        A long description of the pipeline, used in documentation and ignored
-        here. Only included in the signature so that an error isn't thrown when
-        it is encountered.
-
-    Returns
-    -------
-    dict
-        JSON that can be used
-
-    Raises
-    ------
-    ArcanaUsageError
-        [description]
-    """
-    if parameters is None:
-        parameters = []
-    if configuration is None:
-        configuration = {}
-    if isinstance(row_frequency, str):
-        row_frequency = Clinical[row_frequency]
-    if row_frequency not in VALID_FREQUENCIES:
-        raise ArcanaUsageError(
-            f"'{row_frequency}'' is not a valid option ('"
-            + "', '".join(VALID_FREQUENCIES)
-            + "')"
-        )
+    def install_licenses(
+        self,
+        dockerfile: DockerRenderer,
+        build_dir: Path,
+    ):
+        """Generate Neurodocker instructions to install licenses within the container
+        image
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        build_dir : Path
+            path to build dir
+        """
+        # Copy licenses into build directory
+        license_build_dir = build_dir / "licenses"
+        license_build_dir.mkdir()
+        for lic in self.licenses:
+            if lic.store_in_image:
+                if lic.source:
+                    build_path = license_build_dir / lic.name
+                    shutil.copyfile(lic.source, build_path)
+                    dockerfile.copy(
+                        source=[str(build_path.relative_to(build_dir))],
+                        destination=str(lic.destination),
+                    )
+                else:
+                    logger.warning(
+                        "License file for '%s' was not provided, will attempt to download "
+                        "from '%s' dataset-level column or site-wide license dataset at "
+                        "runtime",
+                        lic.name,
+                        lic.column_name(lic.name),
+                    )
+
+    def insert_spec(self, dockerfile: DockerRenderer, build_dir):
+        """Generate Neurodocker instructions to save the specification inside the built
+        image to be used when running the command and comparing against future builds
+
+        Parameters
+        ----------
+        dockerfile : DockerRenderer
+            the neurodocker renderer to append the install instructions to
+        spec : dict
+            the specification used to build the image
+        build_dir : Path
+            path to build dir
+        """
+        self.save(build_dir / "arcana-spec.yaml")
+        dockerfile.copy(source=["./arcana-spec.yaml"], destination=self.SPEC_PATH)
+
+    def save(self, yml_path: Path):
+        """Saves the specification to a YAML file that can be loaded again
+
+        Parameters
+        ----------
+        yml_path : Path
+            path to file to save the spec to
+        """
+        yml_dct = self.asdict()
+        yml_dct["type"] = ClassResolver.tostr(self, strip_prefix=False)
+        with open(yml_path, "w") as f:
+            yaml.dump(yml_dct, f)
+
+    @classmethod
+    def load(
+        cls,
+        yml: ty.Union[Path, dict],
+        root_dir: Path = None,
+        license_paths: dict[str, Path] = None,
+        licenses_to_download: set[str] = None,
+        **kwargs,
+    ):
+        """Loads a deploy-build specification from a YAML file
 
-    # Convert tuples to appropriate dataclasses for inputs, outputs and parameters
-    def parse_specs(args, klass):
-        parsed_args = []
-        for arg in args:
-            if isinstance(arg, klass):
-                parsed = arg
-            elif isinstance(arg, dict):
-                parsed = klass(**arg)
-            else:
-                parsed = klass(*arg)
-            if not parsed.format is arcana.core.data.row.DataRow:
-                parsed_args.append(parsed)
-        return parsed_args
-
-    inputs = parse_specs(inputs, InputArg)
-    outputs = parse_specs(outputs, OutputArg)
-
-    parsed_params = []
-    for param in parameters:
-        if isinstance(param, ParamArg):
-            parsed = param
-        elif isinstance(param, str):
-            parsed = ParamArg(pydra_field=param)
-        else:
-            parsed = ParamArg(**param)
-        parsed_params.append(parsed)
-    parameters = parsed_params
-
-    # JSON to define all inputs and parameters to the pipelines
-    inputs_json = []
-
-    # Add task inputs to inputs JSON specification
-    input_args = []
-    for inpt in inputs:
-        replacement_key = f"[{inpt.pydra_field.upper()}_INPUT]"
-        if issubclass(inpt.format, FileGroup):
-            desc = f"Match resource [SCAN_TYPE]: {inpt.description} "
-            input_type = "string"
+        Parameters
+        ----------
+        yml : Path or dict
+            path to the YAML file to load or loaded dictionary
+        root_dir : Path, optional
+            path to the root directory from which a tree of specs are being loaded from.
+            The name of the root directory is taken to be the organisation the image
+            belongs to, and all nested directories above the YAML file will be joined by
+            '.' and prepended to the name of the loaded spec.
+        license_paths : dict[str, Path], optional
+            Licenses that are provided at build time to be included in the image.
+        licenses_to_download : set[str], optional
+            Licenses that are to be downloaded at runtime. If `license_paths` is not
+            None (i.e. how to access required licenses are to be specified) then required
+            licenses that are not in license_paths need to be explicitly listed in
+            `licenses_to_download` otherwise an error is raised
+        **kwargs
+            additional keyword arguments that override/augment the values loaded from
+            the spec file
+
+        Returns
+        -------
+        Self
+            The loaded spec object
+        """
+
+        if isinstance(yml, str):
+            yml = Path(yml)
+        if isinstance(yml, Path):
+            yml_dict = cls._load_yaml(yml)
+            if type(yml_dict) is not dict:
+                raise ValueError(f"{yml!r} didn't contain a dict!")
+
+            if "name" not in yml_dict:
+                if root_dir is not None:
+                    yml_dict["name"] = ".".join(
+                        yml.relative_to(root_dir).parent.parts + (yml.stem,)
+                    )
+                else:
+                    yml_dict["name"] = yml.stem
+
+            if "org" not in yml_dict:
+                if root_dir is not None:
+                    yml_dict["org"] = root_dir.name
+                else:
+                    yml_dict["org"] = None
+
+            yml_dict["loaded_from"] = yml.absolute()
         else:
-            desc = (
-                f"Match field ({inpt.format.dtype}) [FIELD_NAME]: {inpt.description} "
-            )
-            input_type = COMMAND_INPUT_TYPES.get(inpt.format, "string")
-        inputs_json.append(
-            {
-                "name": path2xnatname(inpt.name),
-                "description": desc,
-                "type": input_type,
-                "default-value": inpt.path,
-                "required": False,
-                "user-settable": True,
-                "replacement-key": replacement_key,
-            }
-        )
-        input_args.append(
-            f"--input {inpt.name} {inpt.stored_format.location()} '{replacement_key}' {inpt.pydra_field} {inpt.format.location()} "
-        )
+            yml_dict = yml
 
-    # Add parameters as additional inputs to inputs JSON specification
-    param_args = []
-    for param in parameters:
-        desc = f"Parameter ({param.type}): " + param.description
-
-        replacement_key = f"[{param.pydra_field.upper()}_PARAM]"
-
-        inputs_json.append(
-            {
-                "name": param.name,
-                "description": desc,
-                "type": COMMAND_INPUT_TYPES.get(param.type, "string"),
-                "default-value": (param.default if param.default else ""),
-                "required": param.required,
-                "user-settable": True,
-                "replacement-key": replacement_key,
-            }
-        )
-        param_args.append(f"--parameter {param.pydra_field} '{replacement_key}' ")
+        yml_dict.pop("type", None)  # Remove "type" from dict if present
 
-    # Set up output handlers and arguments
-    outputs_json = []
-    output_handlers = []
-    output_args = []
-    for output in outputs:
-        label = output.path.split("/")[0]
-        out_fname = output.path + ("." + output.format.ext if output.format.ext else "")
-        # Set the path to the
-        outputs_json.append(
-            {
-                "name": output.name,
-                "description": f"{output.pydra_field} ({output.format.location()})",
-                "required": True,
-                "mount": "out",
-                "path": out_fname,
-                "glob": None,
-            }
-        )
-        output_handlers.append(
-            {
-                "name": f"{output.name}-resource",
-                "accepts-command-output": output.name,
-                "via-wrapup-command": None,
-                "as-a-child-of": "SESSION",
-                "type": "Resource",
-                "label": label,
-                "format": output.format.class_name(),
-            }
-        )
-        output_args.append(
-            f"--output {output.name} {output.stored_format.location()} '{output.path}' {output.pydra_field} {output.format.location()} "
-        )
+        # Override/augment loaded values from spec
+        yml_dict.update(kwargs)
 
-    # Set up fixed arguments used to configure the workflow at initialisation
-    config_args = []
-    for cname, cvalue in configuration.items():
-        cvalue_json = json.dumps(cvalue)  # .replace('"', '\\"')
-        config_args.append(f"--configuration {cname} '{cvalue_json}' ")
-
-    # Add input for dataset name
-    FLAGS_KEY = "#ARCANA_FLAGS#"
-    inputs_json.append(
-        {
-            "name": "Arcana_flags",
-            "description": "Flags passed to `run-arcana-pipeline` command",
-            "type": "string",
-            "default-value": (
-                "--plugin cf "
-                "--work /wl "  # NB: work dir moved inside container due to file-locking issue on some mounted volumes (see https://github.com/tox-dev/py-filelock/issues/147)
-                "--dataset_name default "
-                "--loglevel info "
-                f"--export-work {XnatViaCS.WORK_MOUNT}"
-            ),
-            "required": False,
-            "user-settable": True,
-            "replacement-key": FLAGS_KEY,
-        }
-    )
+        image = cls(**yml_dict)
 
-    input_args_str = " ".join(input_args)
-    output_args_str = " ".join(output_args)
-    param_args_str = " ".join(param_args)
-    config_args_str = " ".join(config_args)
-
-    cmdline = (
-        f"conda run --no-capture-output -n {CONDA_ENV} "  # activate conda
-        f"run-arcana-pipeline xnat-cs//[PROJECT_ID] {name} {pydra_task} "  # run pydra task in Arcana
-        + input_args_str
-        + output_args_str
-        + param_args_str
-        + config_args_str
-        + FLAGS_KEY
-        + " "
-        + f"--dataset_space medimage:Clinical "
-        f"--dataset_hierarchy subject,session "
-        "--single-row [SUBJECT_LABEL],[SESSION_LABEL] "
-        f"--row_frequency {row_frequency} "
-    )  # pass XNAT API details
-    # TODO: add option for whether to overwrite existing pipeline
-
-    # Create Project input that can be passed to the command line, which will
-    # be populated by inputs derived from the XNAT object passed to the pipeline
-    inputs_json.append(
-        {
-            "name": "PROJECT_ID",
-            "description": "Project ID",
-            "type": "string",
-            "required": True,
-            "user-settable": False,
-            "replacement-key": "[PROJECT_ID]",
+        # Explicitly override directive in loaded spec to store license in the image
+
+        if license_paths is not None:
+            for lic in image.licenses:
+                if lic.name in licenses_to_download:
+                    lic.store_in_image = False
+                if lic.store_in_image:
+                    try:
+                        lic.source = license_paths[lic.name]
+                    except KeyError:
+                        raise RuntimeError(
+                            f"{lic.name} license has not been provided when it is "
+                            "specified to be stored in the image"
+                        )
+
+        return image
+
+    @classmethod
+    def _load_yaml(cls, yaml_file: ty.Union[Path, str]):
+        def yaml_join(loader, node):
+            seq = loader.construct_sequence(node)
+            return "".join([str(i) for i in seq])
+
+        # Add special constructors to handle joins and concatenations within the YAML
+        yaml.SafeLoader.add_constructor(tag="!join", constructor=yaml_join)
+        with open(yaml_file, "r") as f:
+            dct = yaml.load(f, Loader=yaml.SafeLoader)
+        return dct
+
+    @classmethod
+    def load_tree(cls, root_dir: Path, **kwargs) -> list:
+        """Walk the given directory structure and load all specs found within it
+
+        Parameters
+        ----------
+        root_dir : Path
+            path to the base directory
+        """
+        if root_dir.is_file():
+            return [cls.load(root_dir, **kwargs)]
+        specs = []
+        for path in chain(root_dir.rglob("*.yml"), root_dir.rglob("*.yaml")):
+            if not any(p.startswith(".") for p in path.parts):
+
+                logging.info("Found container image specification file '%s'", path)
+                specs.append(cls.load(path, root_dir=root_dir, **kwargs))
+
+        return specs
+
+    def autodoc(self, doc_dir, flatten: bool):
+        header = {
+            "title": self.name,
+            "weight": 10,
         }
-    )
 
-    # Access session via Container service args and derive
-    if row_frequency == Clinical.session:
-        # Set the object the pipeline is to be run against
-        context = ["xnat:imageSessionData"]
-        # Create Session input that  can be passed to the command line, which
-        # will be populated by inputs derived from the XNAT session object
-        # passed to the pipeline.
-        inputs_json.extend(
-            [
-                {
-                    "name": "SESSION_LABEL",
-                    "description": "Imaging session label",
-                    "type": "string",
-                    "required": True,
-                    "user-settable": False,
-                    "replacement-key": "[SESSION_LABEL]",
-                },
-                {
-                    "name": "SUBJECT_LABEL",
-                    "description": "Subject label",
-                    "type": "string",
-                    "required": True,
-                    "user-settable": False,
-                    "replacement-key": "[SUBJECT_LABEL]",
-                },
-            ]
-        )
-        # Add specific session to process to command line args
-        cmdline += " --ids [SESSION_LABEL] "
-        # Access the session XNAT object passed to the pipeline
-        external_inputs = [
-            {
-                "name": "SESSION",
-                "description": "Imaging session",
-                "type": "Session",
-                "source": None,
-                "default-value": None,
-                "required": True,
-                "replacement-key": None,
-                "sensitive": None,
-                "provides-value-for-command-input": None,
-                "provides-files-for-command-mount": "in",
-                "via-setup-command": None,
-                "user-settable": False,
-                "load-children": True,
-            }
-        ]
-        # Access to project ID and session label from session XNAT object
-        derived_inputs = [
-            {
-                "name": "__SESSION_LABEL__",
-                "type": "string",
-                "derived-from-wrapper-input": "SESSION",
-                "derived-from-xnat-object-property": "label",
-                "provides-value-for-command-input": "SESSION_LABEL",
-                "user-settable": False,
-            },
-            {
-                "name": "__SUBJECT_ID__",
-                "type": "string",
-                "derived-from-wrapper-input": "SESSION",
-                "derived-from-xnat-object-property": "subject-id",
-                "provides-value-for-command-input": "SUBJECT_LABEL",
-                "user-settable": False,
-            },
-            {
-                "name": "__PROJECT_ID__",
-                "type": "string",
-                "derived-from-wrapper-input": "SESSION",
-                "derived-from-xnat-object-property": "project-id",
-                "provides-value-for-command-input": "PROJECT_ID",
-                "user-settable": False,
-            },
-        ]
-
-    else:
-        raise NotImplementedError(
-            "Wrapper currently only supports session-level pipelines"
-        )
+        if self.loaded_from:
+            header["source_file"] = str(self.loaded_from)
 
-    # Generate the complete configuration JSON
-    xnat_command = {
-        "name": name,
-        "description": description,
-        "label": name,
-        "version": version,
-        "schema-version": "1.0",
-        "image": image_tag,
-        "index": registry,
-        "type": "docker",
-        "command-line": cmdline,
-        "override-entrypoint": True,
-        "mounts": [
-            {"name": "in", "writable": False, "path": str(XnatViaCS.INPUT_MOUNT)},
-            {"name": "out", "writable": True, "path": str(XnatViaCS.OUTPUT_MOUNT)},
-            {  # Saves the Pydra-cache directory outside of the container for easier debugging
-                "name": "work",
-                "writable": True,
-                "path": str(XnatViaCS.WORK_MOUNT),
-            },
-        ],
-        "ports": {},
-        "inputs": inputs_json,
-        "outputs": outputs_json,
-        "xnat": [
-            {
-                "name": name,
-                "description": description,
-                "contexts": context,
-                "external-inputs": external_inputs,
-                "derived-inputs": derived_inputs,
-                "output-handlers": output_handlers,
-            }
-        ],
-    }
+        if flatten:
+            out_dir = doc_dir
+        else:
+            assert isinstance(doc_dir, Path)
 
-    if info_url:
-        xnat_command["info-url"] = info_url
+            out_dir = doc_dir.joinpath(*self.name.split(".")[:-1])
 
-    return xnat_command
+            assert doc_dir in out_dir.parents or out_dir == doc_dir
 
+            out_dir.mkdir(parents=True, exist_ok=True)
 
-def copy_command_ref(dockerfile: DockerRenderer, xnat_commands, build_dir):
-    """Generate Neurodocker instructions to copy a version of the XNAT commands
-    into the image for reference
+        with open(f"{out_dir}/{self.name}.md", "w") as f:
+            f.write("---\n")
+            yaml.dump(header, f)
+            f.write("\n---\n\n")
 
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        Neurodocker renderer to build
-    xnat_commands : list[dict]
-        XNAT command JSONs to copy into the Dockerfile for reference
-    build_dir : Path
-        path to build directory
-    """
-    # Copy command JSON inside dockerfile for ease of reference
-    cmds_dir = build_dir / "xnat_commands"
-    cmds_dir.mkdir(exist_ok=True)
-    for cmd in xnat_commands:
-        fname = cmd.get("name", "command") + ".json"
-        with open(cmds_dir / fname, "w") as f:
-            json.dump(cmd, f, indent="    ")
-    dockerfile.copy(source=["./xnat_commands"], destination="/xnat_commands")
+            f.write("## Package Info\n")
+            tbl_info = MarkdownTable(f, "Key", "Value")
+            tbl_info.write_row("Name", self.name)
+            tbl_info.write_row("App version", self.version)
+            tbl_info.write_row(
+                "Build iteration", self.build_iteration if self.build_iteration else "0"
+            )
+            tbl_info.write_row("Base image", escaped_md(self.base_image.reference))
+            tbl_info.write_row(
+                "Maintainer", f"{self.authors[0].name} ({self.authors[0].email})"
+            )
+            tbl_info.write_row("Info URL", self.info_url)
+            tbl_info.write_row("Short description", self.description)
+            for known_issue in self.known_issues:
+                tbl_info.write_row("Known issues", known_issue.url)
+
+            short_desc = self.long_description or self.description
+            f.write(f"\n{short_desc}\n\n")
+
+            if self.licenses:
+                f.write("### Required licenses\n")
+
+                tbl_lic = MarkdownTable(f, "Name", "URL", "Description")
+                for lic in self.licenses:
+                    tbl_lic.write_row(
+                        lic.name,
+                        escaped_md(lic.info_url),
+                        lic.description.strip(),
+                    )
+
+                f.write("\n")
+
+            f.write("## Command\n")
+
+            tbl_cmd = MarkdownTable(f, "Key", "Value")
+
+            # if self.command.configuration is not None:
+            #     config = self.command.configuration
+            #     # configuration keys are variable depending on the workflow class
+            tbl_cmd.write_row("Task", ClassResolver.tostr(self.command.task))
+            freq_name = (
+                self.command.row_frequency.name
+                if not isinstance(self.command.row_frequency, str)
+                else re.match(r".*\[(\w+)\]", self.command.row_frequency).group(1)
+            )
+            tbl_cmd.write_row("Operates on", freq_name)
 
+            f.write("#### Inputs\n")
+            tbl_inputs = MarkdownTable(
+                f, "Name", "Data type", "Stored data type default", "Description"
+            )
+            if self.command.inputs is not None:
+                for inpt in self.command.inputs:
+                    tbl_inputs.write_row(
+                        escaped_md(inpt.name),
+                        self._data_format_html(inpt.datatype),
+                        self._data_format_html(inpt.default_column.datatype),
+                        inpt.help_string,
+                    )
+                f.write("\n")
+
+            f.write("#### Outputs\n")
+            tbl_outputs = MarkdownTable(
+                f, "Name", "Data type", "Stored data type default", "Description"
+            )
+            if self.command.outputs is not None:
+                for outpt in self.command.outputs:
+                    tbl_outputs.write_row(
+                        escaped_md(outpt.name),
+                        self._data_format_html(outpt.datatype),
+                        self._data_format_html(outpt.default_column.datatype),
+                        outpt.help_string,
+                    )
+                f.write("\n")
+
+            if self.command.parameters is not None:
+                f.write("#### Parameters\n")
+                tbl_params = MarkdownTable(f, "Name", "Data type", "Description")
+                for param in self.command.parameters:
+                    tbl_params.write_row(
+                        escaped_md(param.name),
+                        escaped_md(ClassResolver.tostr(param.datatype)),
+                        param.help_string,
+                    )
+                f.write("\n")
+
+    def compare_specs(self, other, check_version=True):
+        """Compares two build specs against each other and returns the difference
+
+        Parameters
+        ----------
+        s1 : dict
+            first spec
+        s2 : dict
+            second spec
+        check_version : bool
+            check the arcana version used to generate the specs
+
+        Returns
+        -------
+        DeepDiff
+            the difference between the specs
+        """
+
+        sdict = self.asdict()
+        odict = other.asdict()
+
+        def prep(s):
+            dct = {
+                k: v
+                for k, v in s.items()
+                if (not k.startswith("_") and (v or isinstance(v, bool)))
+            }
+            if check_version:
+                if "arcana_version" not in dct:
+                    dct["arcana_version"] = __version__
+            else:
+                del dct["arcana_version"]
+            return dct
 
-def save_store_config(dockerfile: DockerRenderer, build_dir: Path, test_config=False):
-    """Save a configuration for a XnatViaCS store.
+        diff = DeepDiff(prep(sdict), prep(odict), ignore_order=True)
+        return diff
 
-    Parameters
-    ----------
-    dockerfile : DockerRenderer
-        Neurodocker renderer to build
-    build_dir : Path
-        the build directory to save supporting files
-    test_config : bool
-        whether the target XNAT is using the local test configuration, in which
-        case the server location will be hard-coded rather than rely on the
-        XNAT_HOST environment variable passed to the container by the XNAT CS
-    """
-    xnat_cs_store_entry = {"class": "<" + class_location(XnatViaCS) + ">"}
-    if test_config:
-        if sys.platform == "linux":
-            ip_address = "172.17.0.1"  # Linux + GH Actions
+    # @classmethod
+    # def load_in_image(cls, spec_path: Path = SPEC_PATH):
+    #     yml_dct = cls._load_yaml(spec_path)
+    #     klass = ClassResolver(cls)(yml_dct.pop("type"))
+    #     return klass.load(yml_dct)
+
+    @classmethod
+    def _data_format_html(cls, datatype):
+
+        if isinstance(datatype, str):
+            module, name = datatype.split(":")
+            name = name.lower()
+            text = f"{name} (from '{module}' extension)"
         else:
-            ip_address = "host.docker.internal"  # Mac/Windows local debug
-        xnat_cs_store_entry["server"] = "http://" + ip_address + ":8080"
-    DataStore.save_entries(
-        {"xnat-cs": xnat_cs_store_entry}, config_path=build_dir / "stores.yaml"
-    )
-    dockerfile.run(command="mkdir -p /root/.arcana")
-    dockerfile.run(command=f"mkdir -p {str(XnatViaCS.CACHE_DIR)}")
-    dockerfile.copy(
-        source=["./stores.yaml"], destination=IN_DOCKER_ARCANA_HOME_DIR + "/stores.yaml"
-    )
-    dockerfile.env(ARCANA_HOME=IN_DOCKER_ARCANA_HOME_DIR)
+            if ext := getattr(datatype, "ext", None):
+                text = f"{datatype.desc} (`.{ext}`)"
+            elif getattr(datatype, "is_dir", None) and datatype is not BaseDirectory:
+                text = f"{datatype.desc} (directory)"
+            else:
+                text = datatype.desc
 
+            name = datatype.__name__.lower()
 
-@dataclass
-class InputArg:
-    name: str  # How the input will be referred to in the XNAT dialog, defaults to the pydra_field name
-    path: str = None
-    format: type = arcana.data.formats.common.File
-    pydra_field: str = None  # Must match the name of the Pydra task input
-    row_frequency: Clinical = Clinical.session
-    description: str = ""  # description of the input
-    stored_format: type = None  # the format the input is stored in the data store in
-
-    def __post_init__(self):
-        if self.path is None:
-            self.path = self.name
-        if self.pydra_field is None:
-            self.pydra_field = self.name
-        if self.stored_format is None:
-            self.stored_format = self.format
-        if isinstance(self.format, str):
-            self.format = resolve_class(self.format, prefixes=["arcana.data.formats"])
-        if isinstance(self.stored_format, str):
-            self.stored_format = resolve_class(
-                self.stored_format, prefixes=["arcana.data.formats"]
-            )
+        return (
+            f'<span data-toggle="tooltip" data-placement="bottom" title="{name}" '
+            f'aria-label="{name}">{text}</span>'
+        )
 
+    DOCKERFILE_README_TEMPLATE = """
+        The following Docker image was generated by Arcana v{} to enable the
+        commands to be run in the XNAT container service. See
+        https://raw.githubusercontent.com/Australian-Imaging-Service/arcana/main/LICENSE
+        for licence.
 
-@dataclass
-class OutputArg:
-    name: str
-    path: str = None  # The path the output is stored at in XNAT
-    format: type = arcana.data.formats.common.File
-    pydra_field: str = (
-        None  # Must match the name of the Pydra task output, defaults to the path
-    )
-    stored_format: type = (
-        None  # the format the output is to be stored in the data store in
-    )
+        {}
 
-    def __post_init__(self):
-        if self.path is None:
-            self.path = self.name
-        if self.pydra_field is None:
-            self.pydra_field = self.name
-        if self.stored_format is None:
-            self.stored_format = self.format
-        if isinstance(self.format, str):
-            self.format = resolve_class(self.format, prefixes=["arcana.data.formats"])
-        if isinstance(self.stored_format, str):
-            self.stored_format = resolve_class(
-                self.stored_format, prefixes=["arcana.data.formats"]
-            )
+        """
 
 
-@dataclass
-class ParamArg:
-    name: str  # How the input will be referred to in the XNAT dialog, defaults to pydra_field name
-    type: type = str
-    pydra_field: str = None  # Name of parameter to expose in Pydra task
-    required: bool = False
-    default: str = None
-    description: str = ""  # description of the parameter
+class MarkdownTable:
+    def __init__(self, f, *headers: str) -> None:
+        self.headers = tuple(headers)
 
-    def __post_init__(self):
-        if self.pydra_field is None:
-            self.pydra_field = path2varname(self.name)
+        self.f = f
+        self._write_header()
 
+    def _write_header(self):
+        self.write_row(*self.headers)
+        self.write_row(*("-" * len(x) for x in self.headers))
 
-COMMAND_INPUT_TYPES = {bool: "bool", str: "string", int: "number", float: "number"}
+    def write_row(self, *cols: str):
+        cols = list(cols)
+        if len(cols) > len(self.headers):
+            raise ValueError(
+                f"More entries in row ({len(cols)} than columns ({len(self.headers)})"
+            )
+
+        # pad empty column entries if there's not enough
+        cols += [""] * (len(self.headers) - len(cols))
+
+        # TODO handle new lines in col
+        self.f.write(
+            "|" + "|".join(str(col).replace("|", "\\|") for col in cols) + "|\n"
+        )
 
 
-VALID_FREQUENCIES = (Clinical.session, Clinical.dataset)
+def escaped_md(value: str) -> str:
+    if not value:
+        return ""
+    return f"`{value}`"
```

### Comparing `arcana-2.0b0.dev7/arcana/exceptions.py` & `arcana-2.0b2/arcana/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
     pass
 
 
 class ArcanaFileFormatError(ArcanaError):
     pass
 
 
+class ArcanaLicenseNotFoundError(ArcanaNameError):
+    pass
+
+
 class ArcanaUnresolvableFormatException(ArcanaException):
     pass
 
 
 class ArcanaFileGroupNotCachedException(ArcanaException):
     pass
```

### Comparing `arcana-2.0b0.dev7/arcana/tasks/common/archive.py` & `arcana-2.0b2/arcana/common/analysis/tasks/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import tempfile
 import tarfile
 import zipfile
 from pathlib import Path
 import attrs
 from pydra import mark
 from pydra.engine.specs import MultiInputObj, MultiOutputObj, File, Directory
-from arcana.core.utils import set_cwd
+from arcana.core.utils.misc import set_cwd
 from arcana.exceptions import ArcanaUsageError
 
 
 TAR_COMPRESSION_TYPES = ["", "gz", "bz2", "xz"]
 
 
 @mark.task
@@ -26,15 +26,15 @@
                 "help_string": (
                     "The type of compression applied to tar file, "
                     "', '".join(TAR_COMPRESSION_TYPES)
                 ),
                 "allowed_values": list(TAR_COMPRESSION_TYPES),
             },
         ),
-        "format": str,
+        "format": int,
         "ignore_zeros": bool,
         "return": {"out_file": File},
     }
 )
 def create_tar(
     in_file,
     out_file=None,
```

### Comparing `arcana-2.0b0.dev7/arcana/tasks/common/tests/test_archive.py` & `arcana-2.0b2/arcana/common/analysis/tasks/tests/test_archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import os.path
 import tempfile
 import shutil
 import filecmp
 import pytest
-from arcana.tasks.common.archive import create_tar, extract_tar, create_zip, extract_zip
+from arcana.common.analysis.tasks.archive import (
+    create_tar,
+    extract_tar,
+    create_zip,
+    extract_zip,
+)
 
 
 TEST_DIR = "__test__"
 
 
 @pytest.fixture(scope="module")
 def base_dir():
```

### Comparing `arcana-2.0b0.dev7/arcana/tasks/common/utils.py` & `arcana-2.0b2/arcana/common/analysis/tasks/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import typing as ty
 import json
 from pydra import mark
 from pydra.engine.core import File
 from pydra.engine.specs import BaseSpec, SpecInfo
 from pydra.engine.task import FunctionTask
-from arcana.core.data.format import DataItem, FileGroup
+from arcana.core.data.type.base import DataType, FileGroup
 from arcana.core.data.row import DataRow
 
 
 def identity(**fields):
     return fields
 
 
 def identity_task(task_name, fields):
     task = FunctionTask(
         identity,
         input_spec=SpecInfo(
             name=f"{task_name}Inputs",
             bases=(BaseSpec,),
-            fields=[(s, DataItem) for s in fields],
+            fields=[(s, DataType) for s in fields],
         ),
         output_spec=SpecInfo(
             name=f"{task_name}Outputs", bases=(BaseSpec,), fields=[("row", DataRow)]
         ),
     )
     return task
```

### Comparing `arcana-2.0b0.dev7/arcana/test/tasks.py` & `arcana-2.0b2/arcana/core/utils/testing/tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -217,7 +217,41 @@
     with open(in_file) as f:
         contents = f.read()
     try:
         float(contents.strip())
     except ValueError:
         return False
     return True
+
+
+@mark.task
+def check_license(expected_license_path: str, expected_license_contents: Path) -> Path:
+    """Checks the `expected_license_path` to see if there is a file with the same contents
+    as that of `expected_license_contents`
+
+    Parameters
+    ----------
+    expected_license_path : Path
+        path to the expected license file
+    expected_license_contents : Path
+        path containing the contents expected in the expected license file
+
+    Returns
+    -------
+    Path
+        passes through the expected license file so the task can be connected back to the
+        dataset
+    """
+    expected_license_path = Path(expected_license_path)
+    expected_license_contents = Path(expected_license_contents)
+    with open(expected_license_contents) as f:
+        expected_contents = f.read()
+    if not expected_license_path.exists():
+        raise Exception(f"Did not find license file at {expected_license_path}")
+    with open(expected_license_path) as f:
+        actual_contents = f.read()
+    if expected_contents != actual_contents:
+        raise Exception(
+            f'License contents "{actual_contents}" did not match '
+            f'expected "{expected_contents}"'
+        )
+    return expected_license_contents
```

