# Comparing `tmp/bw_matchbox-0.6.1.tar.gz` & `tmp/bw_matchbox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.6.1.tar", last modified: Sun Aug  6 10:30:24 2023, max compression
+gzip compressed data, was "bw_matchbox-0.7.0.tar", last modified: Sun Aug  6 19:19:27 2023, max compression
```

## Comparing `bw_matchbox-0.6.1.tar` & `bw_matchbox-0.7.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.511582 bw_matchbox-0.6.1/
--rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:30:24.511665 bw_matchbox-0.6.1/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.496254 bw_matchbox-0.6.1/bw_matchbox/
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-06 10:30:01.000000 bw_matchbox-0.6.1/bw_matchbox/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493945 bw_matchbox-0.6.1/bw_matchbox/assets/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.498870 bw_matchbox-0.6.1/bw_matchbox/assets/css/
--rw-r--r--   0 cmutel     (501) staff       (20)     3291 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1891 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/common.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4335 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.499148 bw_matchbox-0.6.1/bw_matchbox/assets/images/
--rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493803 bw_matchbox-0.6.1/bw_matchbox/assets/js/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.500245 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 cmutel     (501) staff       (20)    25476 2023-08-05 14:34:04.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 cmutel     (501) staff       (20)    12861 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.502152 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.502713 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/
--rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 cmutel     (501) staff       (20)     5782 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.493867 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.503318 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.506745 bw_matchbox-0.6.1/bw_matchbox/assets/templates/
--rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 cmutel     (501) staff       (20)     3332 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1721 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 cmutel     (501) staff       (20)     5354 2023-08-06 10:07:44.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.507046 bw_matchbox-0.6.1/bw_matchbox/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/bin/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-0.6.1/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.508693 bw_matchbox-0.6.1/bw_matchbox/data/
--rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/bw_matchbox/data/dare.json
--rw-r--r--   0 cmutel     (501) staff       (20)     1388 2023-08-03 14:06:22.000000 bw_matchbox-0.6.1/bw_matchbox/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)    22460 2023-08-06 10:28:58.000000 bw_matchbox-0.6.1/bw_matchbox/webapp.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.510336 bw_matchbox-0.6.1/bw_matchbox.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     4974 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-06 10:30:24.000000 bw_matchbox-0.6.1/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:30:24.508836 bw_matchbox-0.6.1/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-0.6.1/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-06 10:30:24.512129 bw_matchbox-0.6.1/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.326846 bw_matchbox-0.7.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.7.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.7.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 19:19:27.326906 bw_matchbox-0.7.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5337 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.312123 bw_matchbox-0.7.0/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-06 19:19:05.000000 bw_matchbox-0.7.0/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310431 bw_matchbox-0.7.0/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.314892 bw_matchbox-0.7.0/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3297 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1922 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4256 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4315 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.315126 bw_matchbox-0.7.0/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310326 bw_matchbox-0.7.0/bw_matchbox/assets/js/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.316336 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20330 2023-08-06 19:03:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6194 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    12879 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.317723 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4388 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      885 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1452 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5632 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3447 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1081 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4862 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3321 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9995 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.318071 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5781 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.310372 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.318408 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.321997 bw_matchbox-0.7.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3880 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2681 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6969 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      734 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5932 2023-08-06 18:58:22.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.7.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.322398 bw_matchbox-0.7.0/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.7.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2692 2023-08-05 17:26:08.000000 bw_matchbox-0.7.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.324551 bw_matchbox-0.7.0/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.7.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2155 2023-08-06 18:22:10.000000 bw_matchbox-0.7.0/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    22926 2023-08-06 19:01:25.000000 bw_matchbox-0.7.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.325754 bw_matchbox-0.7.0/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6361 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5090 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-06 19:19:27.000000 bw_matchbox-0.7.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-06 19:19:27.324798 bw_matchbox-0.7.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.7.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.7.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-06 19:19:27.327275 bw_matchbox-0.7.0/setup.cfg
```

### Comparing `bw_matchbox-0.6.1/LICENSE` & `bw_matchbox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/PKG-INFO` & `bw_matchbox-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.6.1
+Version: 0.7.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.6.1/README.md` & `bw_matchbox-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/common-modal.css`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   display: flex;
   justify-content: center;
   align-items: center;
   align-content: center;
   /* By default is hidden and inactive, see `show` state below */
   pointer-events: none;
   opacity: 0;
-  transition: all var(--common-animation-time);
+  transition: all var(--common-effect-time) ease-out;
   /* Emulate show effect */
   margin-top: -100px;
   margin-bottom: 100px;
 }
 .common-modal-wrapper .common-modal.show {
   opacity: 1;
   pointer-events: all;
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/common.css`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   /* Primary colors for hovered elements */
   --layout-theme-primary-color-dark1: #1eaedb; /* aks rgb(30,174,219) */
   --layout-theme-primary-color-dark2: #0fa0ce; /* aks gb(15,160,206) */
   /* Error color */
   --layout-theme-error-color: #c33;
   /* Animations */
   --common-animation-time: 250ms;
+  --common-effect-time: 500ms;
 }
 
 /* Basic layout */
 
 /* Issue #7: Widen default Skeleton page width */
 
 .container {
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/compare.css`

 * *Files 7% similar despite different names*

```diff
@@ -118,45 +118,50 @@
   transition: all var(--common-animation-time) ease;
 }
 .compare-table tr.collapsed-handler td:hover {
   background-color: var(--compare-selected-bg-color2);
 }
 
 /* Modal customizations for `set-number-modal`: inner layout with inner scrolls */
-.common-modal-content#set-number-modal .common-modal-content-wrapper {
+#set-number-modal .common-modal-content-wrapper {
   /* Made wrapper clipping */
   display: flex;
 }
-.common-modal-content#set-number-modal .common-modal-content-wrapper > div {
+#set-number-modal .common-modal-content-wrapper > div {
   /* Both inner columns are scrollable */
   overflow: auto;
   padding: 20px;
   flex: 1;
   width: 50%;
 }
-.common-modal-content#set-number-modal .common-modal-content-wrapper > div > *:last-child {
+#set-number-modal .common-modal-content-wrapper > div > *:last-child {
   margin-bottom: 0;
 }
 
 /* Adjust 'edit number' modal table columns widths */
-.common-modal-content#set-number-modal #edit-number-table th:last-child {
+#set-number-modal #edit-number-table th:last-child {
   width: 50px;
 }
-.common-modal-content#set-number-modal #edit-number-table th:first-child {
+#set-number-modal #edit-number-table th:first-child {
   width: 80px;
 }
 /* Adjust 'edit number' modal content styles */
-.common-modal-content#set-number-modal .strong {
+#set-number-modal .strong {
   margin: 5px 0;
 }
 
 /* Adjust 'proxy-dialog-modal' modal content styles */
-.common-modal-content#proxy-dialog-modal #proxy-table th:first-child {
+#proxy-dialog-modal #proxy-table th:first-child {
   width: 50%;
 }
-.common-modal-content#proxy-dialog-modal #proxy-table th:nth-child(2) {
+#proxy-dialog-modal #proxy-table th:nth-child(2) {
   width: 7em;
 }
-.common-modal-content#proxy-dialog-modal #proxy-table td:last-child div textarea {
+#proxy-dialog-modal #proxy-table td:last-child div textarea {
   display: block;
   width: 100%;
 }
+#proxy-dialog-modal #match-type-select {
+  max-width: 250px;
+  overflow: hidden;
+  text-overflow: ellipsis;
+}
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.7.0/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.7.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,28 @@
 modules.define(
     'CompareCore',
     [
         // Required modules...
         'CommonHelpers',
         'CommonModal',
+        'CompareProxyDialogModal',
         'CompareRowClick',
         'CompareRowsHelpers',
     ],
     function provide_CompareCore(
         provide,
         // Resolved modules...
         CommonHelpers,
         CommonModal,
+        CompareProxyDialogModal,
         CompareRowClick,
         CompareRowsHelpers,
     ) {
         /* Compare tables feature code (via global variable `CompareCore`).
          *
-         * Mouse handler methods are used:
-         * - CompareRowsHelpers.clickRowHandler -- Click on regular row to select or collapse selected rows.
-         * - CompareRowsHelpers.clickUncollapseRowHandler -- Click on collapsed row handler to uncollapse.
-         * - CompareRowClick.disableRowClickHandler -- To disable row click effect (if we have some nested interactive elements).
-         * - CompareCore.removeRowHandler
-         * - CompareCore.expandRowHandler
-         * - CompareCore.editNumberHandler
-         * - CompareCore.shiftRowHandler
-         * - CompareCore.replaceAmountRowHandler
-         * - CompareCore.setNumberHandler
-         * - CompareCore.setNewNumberHandler
-         * - CompareCore.resetNumberHandler
-         * - CompareCore.rescaleAmountHandler
-         * - CompareCore.replaceWithTargetHandler
-         *
          * Data table record types:
          *
          * interface TDataRecord {
          *   amount: number; // 7.135225509515751e-9
          *   amount_display: string; // "7.1e-09"
          *   input_id: number; // 633
          *   location: string; // "United States"
@@ -52,17 +39,14 @@
         const CompareCore = {
             // External data...
             sharedData: undefined, // Initializing in `CompareCore.start` from `bw_matchbox/assets/templates/compare.html`
 
             // Counter for making unique records (see `replaceWithTargetHandler`)
             targetNodesCounter: 0,
 
-            // Local data: construct comment field for the `set-number-modal` modal dialog...
-            comment: '',
-
             // Methods...
 
             shiftRowHandler(event, row, row_id) {
                 CompareRowClick.disableRowClickHandler();
                 // Add row from source to target array
                 event.preventDefault();
                 row.parentElement.parentElement.classList.add('shift-right');
@@ -76,15 +60,15 @@
                 const newObj = {
                     ...obj,
                     row_id: 'source-' + obj.row_id
                 };
                 target_data.push(newObj);
                 this.sortTable(target_data);
                 this.buildTable('target-table', target_data, true);
-                this.comment += `* Added source exchange of ${obj.amount} ${obj.unit} ${obj.name} in ${obj.location}.\n`;
+                this.sharedData.comment += `* Added source exchange of ${obj.amount} ${obj.unit} ${obj.name} in ${obj.location}.\n`;
                 row.parentElement.innerHTML = `<i class="fa-solid fa-check"></i>`;
             },
 
             buildRow(data, is_target) {
                 const {
                     collapsedRows
                 } = CompareRowsHelpers;
@@ -102,35 +86,21 @@
                 const rowKind = is_target ? 'target' : 'source';
                 const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
                 if (collapsed && !collapsedRows[collapsedId] && collapsedRows[collapsedId] !== false) {
                     const otherRowKind = !is_target ? 'target' : 'source';
                     const otherTableDataKey = otherRowKind + '_data';
                     const otherTableData = this.sharedData[otherTableDataKey];
                     const collapsedGroupId = data['collapsed-group'];
-                    /* // ORIGONAL BUG: Don't use indices as row_id's!
-                     * const otherRowId = otherTableData.findIndex(
-                     *   (other) => other['collapsed-group'] === collapsedGroupId,
-                     * );
-                     */
                     const otherRowData = otherTableData.find(
                         (other) => other['collapsed-group'] === collapsedGroupId,
                     );
                     if (!otherRowData) {
                         throw new Error('Cannot find other collapsed record');
                     }
                     const otherRowId = otherRowData.row_id;
-                    /* console.log('[CompareCore:buildRow] check', {
-                     *   otherRowId,
-                     *   otherRowKind,
-                     *   otherTableDataKey,
-                     *   otherTableData,
-                     *   collapsedGroupId,
-                     *   otherRowData,
-                     * });
-                     */
                     const otherCollapsedId = CompareRowsHelpers.getCollapsedId(otherRowKind, otherRowId);
                     collapsedRows[collapsedId] = {
                         rowKind,
                         rowId,
                         pairId: otherRowId,
                         // rowEl, // OBSOLETE: Avoid of use it.
                     };
@@ -251,141 +221,14 @@
             ${rowsList.join('')}
           </tbody>
         `;
                 document.getElementById(table_id).innerHTML = header + content;
                 CompareRowsHelpers.updateCollapsedState();
             },
 
-            createOneToOneProxyFunc(event) {
-                event.preventDefault();
-
-                const submission_data = {
-                    exchanges: [{
-                        input_id: this.sharedData.target_id,
-                        amount: 1.0
-                    }],
-                    source: this.sharedData.source_id,
-                    comment: 'One-to-one proxy',
-                    name: 'Proxy for ' +
-                        this.sharedData.target_name
-                        .replace('Market group for ', '')
-                        .replace('market group for ', '')
-                        .replace('Market for ', '')
-                        .replace('market for ', '')
-                        .trim(),
-                };
-                const url = '/create-proxy/';
-                fetch(url, {
-                    method: 'POST',
-                    redirect: 'follow',
-                    headers: {
-                        'Content-Type': 'application/json'
-                    },
-                    body: JSON.stringify(submission_data),
-                }).then((response) => {
-                    if (response.redirected) {
-                        window.location.href = response.url;
-                    }
-                });
-            },
-
-            createProxyFunc(event) {
-                event.preventDefault();
-                const {
-                    target_name,
-                    // comment,
-                    source_node_unit,
-                    source_node_location,
-                    target_data,
-                    source_id,
-                } = this.sharedData;
-                const {
-                    comment
-                } = this;
-                const name =
-                    'Proxy for ' +
-                    target_name
-                    .replace('Market group for ', '')
-                    .replace('market group for ', '')
-                    .replace('Market for ', '')
-                    .replace('market for ', '')
-                    .trim();
-
-                const begin = `
-          <form>
-            <input class="u-full-width" type="text" id="proxy-name" name="proxy-name" value="${name}">
-            <label for="proxy-comment">Comment</label>
-            <textarea class="u-full-width" id="proxy-comment" name="proxy-comment">${comment}</textarea>
-            <p><button class="button-primary" id="create-proxy-submit-button">Create Proxy Process</button>
-            | Unit: ${source_node_unit}
-            | Location: ${source_node_location}</p>
-            <table id="proxy-table" class="fixed-table" width="100%">
-              <thead>
-                <tr>
-                  <th>Name</th>
-                  <th>Amount</th>
-                  <th>Comment</th>
-                </tr>
-              </thead>
-              <tbody>
-        `;
-
-                const rows = target_data.map(function(item, _index) {
-                    return `
-              <tr input_id=${item.input_id}>
-                <td><div>${item.name}</div></td>
-                <td><div>${item.amount_display}</div></td>
-                <td><div><textarea type="text" id="proxy-name-${item.input_id}" name="proxy-name-${item.input_id}"></textarea></div></td>
-              </tr>
-          `;
-                });
-
-                const end = `
-              </tbody>
-            </table>
-          </form>
-        `;
-
-                const title = 'Proxy name';
-                const content = begin + rows.join('') + end;
-
-                CommonModal.setModalContentId('proxy-dialog-modal')
-                    .setTitle(title)
-                    .setModalContentOptions({
-                        scrollable: true,
-                        padded: true,
-                    })
-                    .setContent(content)
-                    .showModal();
-
-                const submit = document.getElementById('create-proxy-submit-button');
-                submit.addEventListener('click', async (e) => {
-                    e.preventDefault();
-                    const submission_data = {
-                        exchanges: target_data,
-                        source: source_id,
-                        comment: document.getElementById('proxy-comment').value,
-                        name: document.getElementById('proxy-name').value,
-                    };
-                    const url = '/create-proxy/';
-                    fetch(url, {
-                        method: 'POST',
-                        redirect: 'follow',
-                        headers: {
-                            'Content-Type': 'application/json'
-                        },
-                        body: JSON.stringify(submission_data),
-                    }).then((response) => {
-                        if (response.redirected) {
-                            window.location.href = response.url;
-                        }
-                    });
-                });
-            },
-
             replaceWithTargetHandler(elem) {
                 CompareRowClick.disableRowClickHandler();
                 const {
                     target_node,
                     target_data
                 } = this.sharedData;
                 // Trying to make unique row_id...
@@ -393,30 +236,30 @@
                 const newNode = {
                     ...target_node,
                     row_id: 'replaced-' + uniqueCounter
                 };
                 target_data.push(newNode);
                 // TODO: Is it required to create (update?) unique row_id
                 target_data.splice(0, target_data.length - 1);
-                this.comment += `* Collapsed input exchanges to target node\n`;
+                this.sharedData.comment += `* Collapsed input exchanges to target node\n`;
                 // TODO: Is sorting required here?
                 this.buildTable('target-table', target_data, true);
                 elem.innerHTML = '';
             },
 
             removeRowHandler(element) {
                 CompareRowClick.disableRowClickHandler();
                 const rowId = element.closest('td').getAttribute('row_id');
                 const {
                     target_data
                 } = this.sharedData;
 
                 function removeValue(obj, index, arr) {
                     if (obj.row_id == rowId) {
-                        this.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
+                        this.sharedData.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
                         arr.splice(index, 1);
                         return true;
                     }
                     return false;
                 }
                 document.getElementById('replace-with-target-arrow').style.display = 'none';
                 target_data.filter(removeValue);
@@ -430,22 +273,15 @@
                 CompareRowClick.disableRowClickHandler();
                 const elInputId = element.getAttribute('input_id');
                 const elAmount = element.getAttribute('amount');
                 const url = '/expand/' + elInputId + '/' + elAmount + '/';
                 const node = target_data.find((item) => item.input_id == elInputId);
 
                 document.getElementById('replace-with-target-arrow').style.display = 'none';
-                /* console.log('[CompareCore:expandRowHandler]', {
-                 *   elInputId,
-                 *   elAmount,
-                 *   url,
-                 *   node,
-                 * })
-                 */
-                this.comment += `* Expanded process inputs of ${node.amount} ${node.unit} from ${node.name} in ${node.location}.\n`;
+                this.sharedData.comment += `* Expanded process inputs of ${node.amount} ${node.unit} from ${node.name} in ${node.location}.\n`;
                 fetch(url)
                     .then((response) => {
                         if (!response.ok) {
                             throw new Error(`HTTP error ${response.status}`);
                         }
                         return response.json();
                     })
@@ -470,15 +306,15 @@
 
             replaceAmountRowHandler(elem, target_id) {
                 CompareRowClick.disableRowClickHandler();
                 const s = this.sharedData.source_data.find(
                     (item) => item.row_id == elem.getAttribute('source_id'),
                 );
                 const t = this.sharedData.target_data.find((item) => item.row_id == target_id);
-                this.comment += `* Used source database amount ${s.amount} ${s.unit} from ${s.name} in ${s.location} instead of ${t.amount} ${t.unit} from ${t.name} in ${t.location}.\n`;
+                this.sharedData.comment += `* Used source database amount ${s.amount} ${s.unit} from ${s.name} in ${s.location} instead of ${t.amount} ${t.unit} from ${t.name} in ${t.location}.\n`;
                 document.getElementById('number-current-amount').innerText = elem.getAttribute('amount');
             },
 
             rescaleAmountHandler(event) {
                 event.preventDefault();
                 const {
                     target
@@ -486,30 +322,30 @@
                 const formRootElem = target.closest('.set-number-modal-form');
                 const rowId = formRootElem.getAttribute('row_id');
                 CompareRowClick.disableRowClickHandler();
                 const t = this.sharedData.target_data.find((item) => item.row_id == rowId);
                 const scale = Number(document.getElementById('rescale_number').value);
                 const node = document.getElementById('number-current-amount');
                 if (scale != 1) {
-                    this.comment += `* Rescaled amount ${t.amount} ${t.unit} from ${t.name} in ${t.location} by ${scale}.\n`;
+                    this.sharedData.comment += `* Rescaled amount ${t.amount} ${t.unit} from ${t.name} in ${t.location} by ${scale}.\n`;
                 }
                 node.innerText = Number(node.innerText) * scale;
             },
 
             setNewNumberHandler(event) {
                 event.preventDefault();
                 const {
                     target
                 } = event;
                 const formRootElem = target.closest('.set-number-modal-form');
                 const rowId = formRootElem.getAttribute('row_id');
                 CompareRowClick.disableRowClickHandler();
                 const t = this.sharedData.target_data.find((item) => item.row_id == rowId);
                 const new_value = document.getElementById('new_number').value;
-                this.comment += `* Set manual exchange value of ${new_value} instead of ${t.amount} ${t.unit} for ${t.name} in ${t.location}.\n`;
+                this.sharedData.comment += `* Set manual exchange value of ${new_value} instead of ${t.amount} ${t.unit} for ${t.name} in ${t.location}.\n`;
                 document.getElementById('number-current-amount').innerText = new_value;
             },
 
             setNumberHandler(event) {
                 event.preventDefault();
                 const {
                     target
@@ -660,14 +496,15 @@
             /** start -- Initialize compare feature (entry point)
              * @param {object} sharedData -- See initialization in `bw_matchbox/assets/templates/compare.html`
              */
             start(sharedData) {
                 // Save public data...
                 this.sharedData = sharedData;
                 CompareRowsHelpers.sharedData = sharedData;
+                CompareProxyDialogModal.sharedData = sharedData;
 
                 const {
                     source_data,
                     target_data
                 } = this.sharedData;
 
                 // console.log('[CompareCore:start] sharedData', sharedData);
@@ -681,18 +518,26 @@
                 // Create tables...
                 this.buildTable('source-table', source_data, false);
                 this.buildTable('target-table', target_data, true);
 
                 // Button handlers...
                 document
                     .getElementById('save-mapping-button')
-                    .addEventListener('click', this.createProxyFunc.bind(this), false);
+                    .addEventListener(
+                        'click',
+                        CompareProxyDialogModal.openProxyDialogModal.bind(CompareProxyDialogModal),
+                        false,
+                    );
                 document
                     .getElementById('one-to-one')
-                    .addEventListener('click', this.createOneToOneProxyFunc.bind(this), false);
+                    .addEventListener(
+                        'click',
+                        CompareProxyDialogModal.createOneToOneProxyFunc.bind(CompareProxyDialogModal),
+                        false,
+                    );
 
                 const expandAll = document.getElementById('expand-all-collapsed');
                 expandAll.addEventListener(
                     'click',
                     CompareRowsHelpers.expandAllCollapsedRows.bind(CompareRowsHelpers),
                 );
             },
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -22,18 +22,19 @@
          *   rowEl: TRowEl;
          *   rowId: TRowId;
          * };
          * interface TCollapsedRow extends TSelectedRow { pairId: TRowId };
          */
 
         // Define module...
-
         const CompareRowsHelpers = {
+            // Shared Data...
+            sharedData: undefined, // Initializing in `CompareCore.start` from `bw_matchbox/assets/templates/compare.html`
+
             // Data...
-            sharedData: undefined, // Initializing in `CompareCore.initCompare` from `bw_matchbox/assets/templates/compare.html`
             rowColumnsCount: 5, // Number of columns in a table row (ATTENTION: It could be changed)...
             selectedFirst: undefined, // <undefined | TSelectedRow>
             collapsedRows: {}, // Record<TRowId, TCollapsedRow> -- Hash of collapsed row
 
             // Methods...
 
             getRootNode() {
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
         // Resolved modules...
         CommonHelpers,
     ) {
         // Define module...
 
         const CommonModal = {
             /** Initialized flag (see `inited` method) */
-            initied: false,
+            inited: false,
 
             /** getModalNode -- Get root modal node
              * @return {HTMLElement|undefined}
              */
             getModalNode() {
                 const modal = document.getElementById('common-modal');
                 // TODO: Cache?
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-0.7.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/compare.html`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {% include 'common-modal.html' %}
 
 {# Module-specific dependencies... #}
 
 <link rel="stylesheet" href="{{ url_for('static', filename='css/compare.css') }}">
 
 <script src="{{ url_for('static', filename='js/Compare/CompareRowsHelpers.js') }}"></script>
+<script src="{{ url_for('static', filename='js/Compare/CompareProxyDialogModal.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareRowClick.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareCore.js') }}"></script>
 
 {# Core js module:
   - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`)
 #}
 
@@ -36,20 +37,22 @@
     <button class="button-primary" id="expand-all-collapsed" onClick="">Expand all collapsed rows</button>
   </div>
   <div class="row compare-tables">
     <div class="column one-half">
       <h3><a href="{{ url_for('process_detail', id=source_node.id) }}">{{ source_node.name }}</a></h3>
       <table class="fixed-table fixed-table-active compare-table" id="source-table" width="100%">
       </table>
+      <p>{{ source_biosphere_number }} biosphere exchanges</p>
     </div>
     <div class="column one-half">
       <h3><a href="{{ url_for('process_detail', id=target_node.id) }}">{{ target_node.name }}</a>
       <span onclick="CompareCore.replaceWithTargetHandler(this)" id="replace-with-target-arrow"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
       <table class="fixed-table fixed-table-active compare-table" id="target-table" width="100%">
       </table>
+      <p>{{ target_biosphere_number }} biosphere exchanges</p>
     </div>
   </div>
 </div>
 
 <script>
   modules.require('CompareCore', (CompareCore) => {
     // Global variables for compare tables feature (via global variable `sharedData`)...
@@ -58,20 +61,27 @@
       target_data: {{ target_data_json|safe }}, // TDataRecord[]
       target_node: {{ target_json|safe}},
       source_id: {{ source_node.id }},
       target_id: {{ target_node.id }},
       target_name: '{{ target_node.name|safe }}',
       source_node_unit: '{{source_node.unit}}',
       source_node_location: '{{source_node.location}}',
-      /* XXX: Probably these labels should be added in `index.html`? Is it required here?
-       * // TODO: Remove when #41 is closed
-       * // Not used anyway?
-       * source_db_label: '{{ source }}',
-       * target_db_label: '{{ target }}',
-       * proxy_db_label: '{{ proxy }}',
+      match_types: {{ match_types|safe }},
+      match_type_default: '3',
+      comment: '', // Shared comments accumulator
+      /* // #52: match_types sample:
+       * {
+       *   '1': 'No direct match available',
+       *   '2': 'Direct match with near-identical data',
+       *   '3': 'Match with updated data',
+       *   '4': 'Match with updated data and adding source transport',
+       *   '5': 'Match with market and replace or remove transport',
+       *   '6': 'Match with market and replace or remove transport and loss factor',
+       *   '7': 'Equivalent datasets after modification',
+       * }
        */
     };
 
     // Export to global scope (to access from generated html code handlers).
     window.CompareCore = CompareCore;
 
     // Start core module...
```

#### html2text {}

```diff
@@ -7,9 +7,11 @@
 %}{{ source_node.location }} | {{ target_node.location }}{% endif %} ***
 *** Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{
 { source_node.unit }} | {{ target_node.unit }}{% endif %} ***
 {% if proxy and proxy != "None" %}Create Proxy 1-to-1 Proxy{% else %}Save{%
 endif %}
 Expand all collapsed rows
 **** {{_source_node.name_}} ****
+{{ source_biosphere_number }} biosphere exchanges
 {{_target_node.name_}}
+{{ target_biosphere_number }} biosphere exchanges
  {% include 'footer.html' %}
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/process_detail.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 {% include 'header.html' %}
 <div class="container">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="column">
       <h1>{{ ds.name }}
         {% if ds.database == source %}
+          <button onclick="markWaitlist(this)" style="vertical-align: middle" class="button-primary" id="mark-waitlist">Waitlist</button>
           {% if not ds.matched %}<button onclick="markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">No match needed</button>
           {% if same_name_count %}<button onclick="markAllMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-multi-match">Mark all matched</button>{% endif %}
-          <a style="vertical-align: middle" id="match-button" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% elif ds.no_match_needed %}<button id="match-button" style="vertical-align: middle">No match needed</button>{% else %}<button id="match-button" style="vertical-align: middle">Matched</button>{% endif %}
+          <a style="vertical-align: middle" id="match-button" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% elif ds.match_type == "1" %}<button id="match-button" style="vertical-align: middle">No match needed</button>{% else %}<button id="match-button" style="vertical-align: middle">Matched</button>{% endif %}
         {% endif %}
       </h1>
       <ul>
           <li>Database: {{ ds.database }}</li>
           <li>Location: {{ ds.location }}</li>
           <li>Unit: {{ ds.unit }}</li>
           <li>ID: {{ ds.id }}</li>
@@ -24,14 +25,17 @@
           {% endif %}
           {% if proxy_node %}
               <li>Proxy: <a href="{{ url_for('process_detail', id=proxy_node.id) }}">{{ proxy_node }}</a></li>
           {% endif %}
           {% if reference_node %}
               <li>Proxy for: <a href="{{ url_for('process_detail', id=reference_node.id) }}">{{ reference_node }}</a></li>
           {% endif %}
+          {% if match_type %}
+              <li>Match type: {{ match_type }}</li>
+          {% endif %}
 
       </ul>
       <h2>Technosphere Inputs</h2>
       <table width="100%">
         <tr>
           <th>Amount</th>
           <th>Name</th>
@@ -90,16 +94,27 @@
       {% endif %}
       </table>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
+function markWaitlist (button) {
+  var url = "{{ url_for('add_attribute', id=ds.id, attr='waitlist', value='1')|safe }}";
+  fetch(url).then((response) => {
+    if (!response.ok) {
+        throw new Error(`HTTP error ${response.status}`);
+    };
+    button.innerText = "Waitlisted";
+    button.classList.remove("button-primary");
+  });
+};
+
 function markMatched (button) {
-  fetch("{{ url_for('add_attribute', id=ds.id, attr='no_match_needed', value='1')|safe }}");
+  fetch("{{ url_for('add_attribute', id=ds.id, attr='match_type', value='1')|safe }}");
   var url = "{{ url_for('add_attribute', id=ds.id, attr='matched', value='1')|safe }}";
   fetch(url).then((response) => {
     if (!response.ok) {
         throw new Error(`HTTP error ${response.status}`);
     };
     button.innerText = "Matched";
     button.classList.remove("button-primary");
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% include 'header.html' %}
 {% include 'navigation.html' %}
-****** {{ ds.name }} {% if ds.database == source %} {% if not ds.matched %}No
-match needed {% if same_name_count %}Mark all matched{% endif %} Match{% elif
-ds.no_match_needed %}No match needed{% else %}Matched{% endif %} {% endif %}
-******
+****** {{ ds.name }} {% if ds.database == source %} Waitlist {% if not
+ds.matched %}No match needed {% if same_name_count %}Mark all matched{% endif
+%} Match{% elif ds.match_type == "1" %}No match needed{% else %}Matched{% endif
+%} {% endif %} ******
     * Database: {{ ds.database }}
     * Location: {{ ds.location }}
     * Unit: {{ ds.unit }}
     * ID: {{ ds.id }}
     * Production amount: {{ ds['production amount'] }}
     * Reference product: {{ ds['reference product'] }}
     * Authors: {{ authors }}
@@ -17,14 +17,16 @@
       %}
       {%_if_obj.data.matched_%}_{%_endif_%}{{obj.location}}
        {% endfor %}
     * {% endif %} {% if proxy_node %}
     * Proxy: {{_proxy_node_}}
     * {% endif %} {% if reference_node %}
     * Proxy for: {{_reference_node_}}
+    * {% endif %} {% if match_type %}
+    * Match type: {{ match_type }}
     * {% endif %}
 ***** Technosphere Inputs *****
 Amount        Name              Location              Unit              Matched     Action
                                                                                     {% if row.matched
                                                                                     %}
                                                                                     Compare
                                                                                     {{ row.match.name
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.7.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.7.0/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.7.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/data/dare.json` & `bw_matchbox-0.7.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/bw_matchbox/webapp.py` & `bw_matchbox-0.7.0/bw_matchbox/webapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import tomli
 import whoosh
 from bw2data.backends import ActivityDataset as AD
 from flask_httpauth import HTTPBasicAuth
 from peewee import fn
 from werkzeug.security import check_password_hash, generate_password_hash
 
-from .utils import name_close_enough, similar_location
+from .utils import get_match_types, name_close_enough, similar_location
 
 BASE_DIR = Path(__file__).resolve().parent
 DATA_DIR = BASE_DIR / "data"
 
 matchbox_app = flask.Flask(
     "matchbox_app",
     static_folder=BASE_DIR / "assets",
@@ -57,14 +57,16 @@
     app.config["mb_output_dir"] = Path(config["files"]["output_dir"])
     if not (
         app.config["mb_output_dir"].is_dir()
         and os.access(app.config["mb_output_dir"], os.W_OK)
     ):
         raise ValueError("`output_dir` is invalid")
 
+    app.config["mb_match_types"] = get_match_types(app.config["mb_output_dir"])
+
     return app
 
 
 def get_context():
     project = flask.request.cookies.get("project")
     if not project:
         return flask.redirect(flask.url_for("select_project"))
@@ -443,15 +445,15 @@
     node = bd.get_node(id=id)
 
     attr = flask.request.args.get("attr")
     value = flask.request.args.get("value")
 
     if attr is None or value is None:
         flask.abort(400)
-    if attr in ("highlighted", "matched", "no_match_needed"):
+    if attr in ("waitlist", "matched"):
         if value not in ("0", "1"):
             flask.abort(400)
         value = {"0": False, "1": True}[value]
 
     node[attr] = value
 
     try:
@@ -463,32 +465,34 @@
     return ""
 
 
 def get_authors(authors):
     if not authors:
         return "Unknown"
     elif isinstance(authors, list):
-        return ",".join({obj.get("name", "Unknown") for obj in authors})
+        return ", ".join({obj.get("name", "Unknown") for obj in authors})
     else:
-        return ",".join({obj.get("name", "Unknown") for obj in authors.values()})
+        return ", ".join({obj.get("name", "Unknown") for obj in authors.values()})
 
 
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
-    reference_node = bd.get_node(id=node["original_id"]) if node.get("original_id") else None
+    reference_node = (
+        bd.get_node(id=node["original_id"]) if node.get("original_id") else None
+    )
 
     same_name = AD.select().where(
         AD.name == node["name"], AD.database == node["database"], AD.id != node.id
     )
     same_name_count = same_name.count()
     technosphere = sorted(node.technosphere(), key=lambda x: x.input["name"])
     biosphere = sorted(node.biosphere(), key=lambda x: x.input["name"])
@@ -507,35 +511,38 @@
         file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
         same_name_count=same_name_count,
         same_name=same_name,
         technosphere=technosphere,
         biosphere=biosphere,
         show_matching=False,
+        match_type=matchbox_app.config["mb_match_types"].get(node.get("match_type")),
     )
 
 
 @matchbox_app.route("/multi-match/<id>", methods=["GET"])
 @auth.login_required
 def multi_match(id):
     context = get_context()
     proj, s, t, proxy = context
     bd.projects.set_current(proj)
 
     node = bd.get_node(id=id)
     node["matched"] = True
-    node["no_match_needed"] = True
+    node["match_type"] = "1"
+    node["waitlist"] = False
     node.save()
 
     for ds in AD.select().where(
         AD.name == node["name"], AD.database == node["database"], AD.id != node.id
     ):
         if not ds.data.get("matched"):
             ds.data["matched"] = True
-            ds.data["no_match_needed"] = True
+            ds.data["match_type"] = "1"
+            ds.data["waitlist"] = False
             ds.save()
     return ""
 
 
 @matchbox_app.route("/match/<source>", methods=["GET"])
 @auth.login_required
 def match(source):
@@ -645,16 +652,19 @@
         source=s,
         target=t,
         target_json=json.dumps(target_itself),
         user=auth.current_user(),
         file_number=sum(1 for obj in files if obj["enabled"]),
         source_node=source,
         source_data_json=json.dumps(source_technosphere),
+        source_biosphere_number=len(source.biosphere()),
         target_node=target,
         target_data_json=json.dumps(target_technosphere),
+        target_biosphere_number=len(target.biosphere()),
+        match_types=matchbox_app.config["mb_match_types"],
     )
 
 
 @matchbox_app.route("/expand/<id>/<scale>/", methods=["GET"])
 @auth.login_required
 def expand(id, scale):
     context = get_context()
@@ -686,26 +696,26 @@
 
 
 @matchbox_app.route("/create-proxy/", methods=["POST"])
 @auth.login_required
 def create_proxy():
     content = flask.request.get_json()
     proj, s, t, proxy = get_context()
-    # files = get_files()
     bd.projects.set_current(proj)
 
     source = bd.get_activity(id=content["source"])
     process = bd.Database(proxy).new_activity(
         name=content["name"],
         code=uuid.uuid4().hex,
         comment=content["comment"],
         unit=source["unit"],
         location=source["location"],
         original_name=source["name"],
         original_id=source.id,
+        match_type=content.get("match_type", "0"),
         **{"reference product": source.get("reference product")}
     )
     process.save()
 
     source_rp = source.rp_exchange()
     process.new_edge(
         input=process, amount=source_rp["amount"], type="production"
@@ -714,11 +724,12 @@
         process.new_edge(
             type="technosphere",
             input=bd.get_activity(id=exc["input_id"]),
             amount=exc["amount"],
         ).save()
 
     source["matched"] = True
+    source["waitlist"] = False
     source["proxy_id"] = process.id
     source.save()
 
     return flask.redirect(flask.url_for("process_detail", id=process.id))
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.7.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.6.1
+Version: 0.7.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.6.1/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.7.0/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ./bw_matchbox/assets/css/fixed-table.css
 ./bw_matchbox/assets/css/normalize.css
 ./bw_matchbox/assets/css/processes-list.css
 ./bw_matchbox/assets/css/skeleton.css
 ./bw_matchbox/assets/css/tooltip.css
 ./bw_matchbox/assets/images/favicon.ico
 ./bw_matchbox/assets/js/Compare/CompareCore.js
+./bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
 ./bw_matchbox/assets/js/Compare/CompareRowClick.js
 ./bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
@@ -71,14 +72,15 @@
 bw_matchbox/assets/css/fixed-table.css
 bw_matchbox/assets/css/normalize.css
 bw_matchbox/assets/css/processes-list.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
 bw_matchbox/assets/js/Compare/CompareCore.js
+bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
 bw_matchbox/assets/js/Compare/CompareRowClick.js
 bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
 bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
```

### Comparing `bw_matchbox-0.6.1/docs/conf.py` & `bw_matchbox-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.6.1/setup.cfg` & `bw_matchbox-0.7.0/setup.cfg`

 * *Files identical despite different names*

