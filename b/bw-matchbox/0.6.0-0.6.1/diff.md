# Comparing `tmp/bw_matchbox-0.6.0.tar.gz` & `tmp/bw_matchbox-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.6.0.tar", last modified: Sun Aug  6 10:01:02 2023, max compression
+gzip compressed data, was "bw_matchbox-0.6.1.tar", last modified: Sun Aug  6 10:30:24 2023, max compression
```

## Comparing `bw_matchbox-0.6.0.tar` & `bw_matchbox-0.6.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.025076 bw_matchbox-0.6.0/
--rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:01:02.025165 bw_matchbox-0.6.0/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.010095 bw_matchbox-0.6.0/bw_matchbox/
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-06 10:00:26.000000 bw_matchbox-0.6.0/bw_matchbox/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007843 bw_matchbox-0.6.0/bw_matchbox/assets/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.011986 bw_matchbox-0.6.0/bw_matchbox/assets/css/
--rw-r--r--   0 cmutel     (501) staff       (20)     3291 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1891 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/common.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4335 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.012139 bw_matchbox-0.6.0/bw_matchbox/assets/images/
--rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007731 bw_matchbox-0.6.0/bw_matchbox/assets/js/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.013085 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 cmutel     (501) staff       (20)    25476 2023-08-05 14:34:04.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 cmutel     (501) staff       (20)    12861 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.014292 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.014581 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/
--rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5782 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007779 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.015006 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.020453 bw_matchbox-0.6.0/bw_matchbox/assets/templates/
--rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3332 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1721 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 cmutel     (501) staff       (20)     5175 2023-08-05 19:10:39.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.020760 bw_matchbox-0.6.0/bw_matchbox/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-0.6.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.022516 bw_matchbox-0.6.0/bw_matchbox/data/
--rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/data/dare.json
--rw-r--r--   0 cmutel     (501) staff       (20)     1388 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)    22116 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.023751 bw_matchbox-0.6.0/bw_matchbox.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     4974 2023-08-06 10:01:02.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.022717 bw_matchbox-0.6.0/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-06 10:01:02.025626 bw_matchbox-0.6.0/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.511582 bw_matchbox-0.6.1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:30:24.511665 bw_matchbox-0.6.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.496254 bw_matchbox-0.6.1/bw_matchbox/
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-06 10:30:01.000000 bw_matchbox-0.6.1/bw_matchbox/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493945 bw_matchbox-0.6.1/bw_matchbox/assets/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.498870 bw_matchbox-0.6.1/bw_matchbox/assets/css/
+-rw-r--r--   0 cmutel     (501) staff       (20)     3291 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1891 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4335 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.499148 bw_matchbox-0.6.1/bw_matchbox/assets/images/
+-rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493803 bw_matchbox-0.6.1/bw_matchbox/assets/js/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.500245 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 cmutel     (501) staff       (20)    25476 2023-08-05 14:34:04.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    12861 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.502152 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.502713 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/
+-rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5782 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493867 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.503318 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.506745 bw_matchbox-0.6.1/bw_matchbox/assets/templates/
+-rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3332 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1721 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     5354 2023-08-06 10:07:44.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.507046 bw_matchbox-0.6.1/bw_matchbox/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-0.6.1/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.508693 bw_matchbox-0.6.1/bw_matchbox/data/
+-rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/data/dare.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     1388 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    22460 2023-08-06 10:28:58.000000 bw_matchbox-0.6.1/bw_matchbox/webapp.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.510336 bw_matchbox-0.6.1/bw_matchbox.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     4974 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.508836 bw_matchbox-0.6.1/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-06 10:30:24.512129 bw_matchbox-0.6.1/setup.cfg
```

### Comparing `bw_matchbox-0.6.0/LICENSE` & `bw_matchbox-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/PKG-INFO` & `bw_matchbox-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.6.0
+Version: 0.6.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.6.0/README.md` & `bw_matchbox-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.6.1/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.6.1/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/process_detail.html`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
           <li>Comment: {{ds.comment }}</li>
           {% if same_name_count %}
               <li>Datasets with same name: {{ same_name_count }}: {% for obj in same_name %}<a href="{{ url_for('process_detail', id=obj.id) }}">{% if obj.data.matched %}<i class="fa-solid fa-check"></i> {% endif %}{{obj.location}}</a> {% endfor %}</li>
           {% endif %}
           {% if proxy_node %}
               <li>Proxy: <a href="{{ url_for('process_detail', id=proxy_node.id) }}">{{ proxy_node }}</a></li>
           {% endif %}
+          {% if reference_node %}
+              <li>Proxy for: <a href="{{ url_for('process_detail', id=reference_node.id) }}">{{ reference_node }}</a></li>
+          {% endif %}
 
       </ul>
       <h2>Technosphere Inputs</h2>
       <table width="100%">
         <tr>
           <th>Amount</th>
           <th>Name</th>
```

#### html2text {}

```diff
@@ -15,14 +15,16 @@
     * {% if same_name_count %}
     * Datasets with same name: {{ same_name_count }}: {% for obj in same_name
       %}
       {%_if_obj.data.matched_%}_{%_endif_%}{{obj.location}}
        {% endfor %}
     * {% endif %} {% if proxy_node %}
     * Proxy: {{_proxy_node_}}
+    * {% endif %} {% if reference_node %}
+    * Proxy for: {{_reference_node_}}
     * {% endif %}
 ***** Technosphere Inputs *****
 Amount        Name              Location              Unit              Matched     Action
                                                                                     {% if row.matched
                                                                                     %}
                                                                                     Compare
                                                                                     {{ row.match.name
```

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.6.1/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.6.1/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/data/dare.json` & `bw_matchbox-0.6.1/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/utils.py` & `bw_matchbox-0.6.1/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/bw_matchbox/webapp.py` & `bw_matchbox-0.6.1/bw_matchbox/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,44 +459,53 @@
     except whoosh.index.LockError:
         # MAIN_WRITELOCK not being released. Can ignore as we don't
         # change anything that is in the index anyway.
         pass
     return ""
 
 
+def get_authors(authors):
+    if not authors:
+        return "Unknown"
+    elif isinstance(authors, list):
+        return ",".join({obj.get("name", "Unknown") for obj in authors})
+    else:
+        return ",".join({obj.get("name", "Unknown") for obj in authors.values()})
+
+
 @matchbox_app.route("/process/<id>", methods=["GET"])
 @auth.login_required
 def process_detail(id):
     context = get_context()
     if isinstance(context, flask.Response):
         return context
     proj, s, t, proxy = context
     files = get_files()
     bd.projects.set_current(proj)
 
     node = bd.get_node(id=id)
     proxy_node = bd.get_node(id=node["proxy_id"]) if node.get("proxy_id") else None
+    reference_node = bd.get_node(id=node["original_id"]) if node.get("original_id") else None
 
     same_name = AD.select().where(
         AD.name == node["name"], AD.database == node["database"], AD.id != node.id
     )
     same_name_count = same_name.count()
     technosphere = sorted(node.technosphere(), key=lambda x: x.input["name"])
     biosphere = sorted(node.biosphere(), key=lambda x: x.input["name"])
 
     return flask.render_template(
         "process_detail.html",
         title="bw_matchbox Detail Page",
         ds=node,
-        authors=",".join(
-            [obj.get("name", "Unknown") for obj in node.get("authors", [])]
-        ),
+        authors=get_authors(node.get("authors")),
         project=proj,
         proxy=proxy,
         proxy_node=proxy_node,
+        reference_node=reference_node,
         source=s,
         target=t,
         file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
         same_name_count=same_name_count,
         same_name=same_name,
         technosphere=technosphere,
```

### Comparing `bw_matchbox-0.6.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.6.1/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.6.0
+Version: 0.6.1
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.6.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.6.1/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/docs/conf.py` & `bw_matchbox-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.0/setup.cfg` & `bw_matchbox-0.6.1/setup.cfg`

 * *Files identical despite different names*

