# Comparing `tmp/bw_matchbox-0.5.1.tar.gz` & `tmp/bw_matchbox-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.5.1.tar", last modified: Fri Aug  4 16:46:34 2023, max compression
+gzip compressed data, was "bw_matchbox-0.6.0.tar", last modified: Sun Aug  6 10:01:02 2023, max compression
```

## Comparing `bw_matchbox-0.5.1.tar` & `bw_matchbox-0.6.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.184677 bw_matchbox-0.5.1/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.5.1/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.5.1/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-04 16:46:34.184746 bw_matchbox-0.5.1/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.5.1/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.169986 bw_matchbox-0.5.1/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-04 16:46:03.000000 bw_matchbox-0.5.1/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.5.1/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.168123 bw_matchbox-0.5.1/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.172535 bw_matchbox-0.5.1/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3291 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1891 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     4335 2023-08-04 16:42:28.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     3353 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.172719 bw_matchbox-0.5.1/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.5.1/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.168022 bw_matchbox-0.5.1/bw_matchbox/assets/js/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.173906 bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    25220 2023-08-04 16:42:28.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1272 2023-08-04 16:42:28.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    12861 2023-08-04 16:42:28.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.175637 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3578 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      497 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      993 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4710 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3494 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1128 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4909 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     2523 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3775 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.175941 bw_matchbox-0.5.1/bw_matchbox/assets/js/common/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     5782 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.168065 bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.176256 bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.179949 bw_matchbox-0.5.1/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3937 2023-08-04 16:42:28.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     4442 2023-08-04 13:00:53.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3583 2023-08-04 09:48:51.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.5.1/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.180361 bw_matchbox-0.5.1/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.5.1/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.5.1/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.182348 bw_matchbox-0.5.1/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.5.1/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.5.1/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20822 2023-08-04 13:01:12.000000 bw_matchbox-0.5.1/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.183531 bw_matchbox-0.5.1/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     4974 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-04 16:46:34.000000 bw_matchbox-0.5.1/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 16:46:34.182592 bw_matchbox-0.5.1/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.5.1/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.5.1/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-04 16:46:34.185303 bw_matchbox-0.5.1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.025076 bw_matchbox-0.6.0/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1067 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:01:02.025165 bw_matchbox-0.6.0/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     5337 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.010095 bw_matchbox-0.6.0/bw_matchbox/
+-rw-r--r--   0 cmutel     (501) staff       (20)        6 2023-08-06 10:00:26.000000 bw_matchbox-0.6.0/bw_matchbox/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      215 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007843 bw_matchbox-0.6.0/bw_matchbox/assets/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.011986 bw_matchbox-0.6.0/bw_matchbox/assets/css/
+-rw-r--r--   0 cmutel     (501) staff       (20)     3291 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1891 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4335 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      640 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     1392 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     7618 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 cmutel     (501) staff       (20)     4315 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 cmutel     (501) staff       (20)    11556 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 cmutel     (501) staff       (20)      916 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.012139 bw_matchbox-0.6.0/bw_matchbox/assets/images/
+-rw-r--r--   0 cmutel     (501) staff       (20)    32038 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007731 bw_matchbox-0.6.0/bw_matchbox/assets/js/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.013085 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 cmutel     (501) staff       (20)    25476 2023-08-05 14:34:04.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1272 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 cmutel     (501) staff       (20)    12861 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.014292 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4388 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 cmutel     (501) staff       (20)      885 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1452 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5632 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3447 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     1081 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     4862 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     3321 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     9995 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.014581 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/
+-rw-r--r--   0 cmutel     (501) staff       (20)     5634 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     5782 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.007779 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.015006 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 cmutel     (501) staff       (20)    13286 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 cmutel     (501) staff       (20)     6018 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.020453 bw_matchbox-0.6.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 cmutel     (501) staff       (20)      756 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     3332 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2681 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      461 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 cmutel     (501) staff       (20)       16 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     2666 2023-08-05 06:10:27.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     6969 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      733 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1721 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      734 2023-08-05 07:08:03.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     5175 2023-08-05 19:10:39.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      599 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      412 2023-08-01 11:28:52.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      850 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 cmutel     (501) staff       (20)      947 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 cmutel     (501) staff       (20)     1243 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.020760 bw_matchbox-0.6.0/bw_matchbox/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2692 2023-08-05 18:47:38.000000 bw_matchbox-0.6.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.022516 bw_matchbox-0.6.0/bw_matchbox/data/
+-rw-r--r--   0 cmutel     (501) staff       (20)   123246 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 cmutel     (501) staff       (20)    93862 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 cmutel     (501) staff       (20)   116072 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     1388 2023-08-03 14:06:22.000000 bw_matchbox-0.6.0/bw_matchbox/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    22116 2023-08-06 09:58:28.000000 bw_matchbox-0.6.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.023751 bw_matchbox-0.6.0/bw_matchbox.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     6361 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     4974 2023-08-06 10:01:02.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-07-24 11:26:00.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      167 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       12 2023-08-06 10:01:01.000000 bw_matchbox-0.6.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-08-06 10:01:02.022717 bw_matchbox-0.6.0/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1145 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/docs/conf.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-07-24 11:16:50.000000 bw_matchbox-0.6.0/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1900 2023-08-06 10:01:02.025626 bw_matchbox-0.6.0/setup.cfg
```

### Comparing `bw_matchbox-0.5.1/LICENSE` & `bw_matchbox-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/PKG-INFO` & `bw_matchbox-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.5.1
+Version: 0.6.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
@@ -84,15 +84,15 @@
 To use `bw_matchbox`, you need to do the following:
 
 ### Create a configuration file
 
 Configuration is done via a `toml` file. See [`config_example.toml`](https://github.com/cauldron/bw_matchbox/blob/main/config_example.toml) for the structure of this file. It needs to provide the following:
 
 * `[users]` section: Authentication, via a set of usernames and passwords
-* `changes_file`: Location of the file where we will save your matching selections.
+* `output_dir`: Location of the directory where output files will be written. Must be writable.
 * `directories`: (Optional) Location of existing [randonneur](https://github.com/cmutel/randonneur) matching files to use, if any.
 
 The easiest way to set this up is with:
 
 ```console
 matchbox setup
 ```
```

### Comparing `bw_matchbox-0.5.1/README.md` & `bw_matchbox-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 To use `bw_matchbox`, you need to do the following:
 
 ### Create a configuration file
 
 Configuration is done via a `toml` file. See [`config_example.toml`](https://github.com/cauldron/bw_matchbox/blob/main/config_example.toml) for the structure of this file. It needs to provide the following:
 
 * `[users]` section: Authentication, via a set of usernames and passwords
-* `changes_file`: Location of the file where we will save your matching selections.
+* `output_dir`: Location of the directory where output files will be written. Must be writable.
 * `directories`: (Optional) Location of existing [randonneur](https://github.com/cmutel/randonneur) matching files to use, if any.
 
 The easiest way to set this up is with:
 
 ```console
 matchbox setup
 ```
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/processes-list.css`

 * *Files 20% similar despite different names*

```diff
@@ -10,38 +10,69 @@
 
 /* Header */
 .processes-list .page-header h1 {
   font-size: 200%;
 }
 
 /* Empty state: hode some elements... */
-/* .processes-list.empty .page-filters, */
-/* UNUSED: .processes-list.empty .table-pagination, */
 .processes-list.empty .processes-list-table {
   display: none;
 }
+.processes-list.loading .processes-list-table-empty,
+.processes-list:not(.empty) .processes-list-table-empty {
+  display: none;
+}
+.processes-list .processes-list-table-empty {
+  padding: 10px;
+  margin: 10px auto;
+  text-align: center;
+  opacity: 0.5;
+}
 
 /* Loading state: disable some elements... */
 .processes-list > * {
   transition: all var(--common-animation-time);
 }
 .processes-list.loading .page-search,
 .processes-list.loading .page-filters,
-/* UNUSED: .processes-list.loading .table-pagination, */
 .processes-list.loading .bottom-actions-links {
   opacity: 0.5;
   pointer-events: none;
 }
 .processes-list.loading .bottom-actions-links {
   opacity: 0;
 }
 
+/* Top radio groups... */
+.processes-list .page-filters {
+  line-height: 1;
+}
+.processes-list .page-filters > span,
+.processes-list .page-filters > span > span {
+  display: inline-block;
+  margin-right: 10px;
+}
+.processes-list .page-filters .radio-group-item {
+  white-space: nowrap;
+}
+.processes-list .page-filters .radio-group-item-disabled {
+  opacity: 0.5;
+  pointer-events: none;
+}
+.processes-list .page-filters .radio-group-item > label {
+  font-weight: normal;
+}
+.processes-list.has-search .radio-group.order-by {
+  pointer-events: none;
+  opacity: 0.5;
+}
+
 /* Table */
 .processes-list-table {
-  margin-bottom: 0;
+  margin: 20px 0;
 }
 .processes-list-table tr td:last-child div > .button {
   display: block;
   width: 100%;
   margin-bottom: 0;
 }
 
@@ -96,38 +127,43 @@
  *   text-decoration: underline;
  * }
  */
 
 /* Bottom actions */
 .processes-list .bottom-actions {
   position: relative;
-  min-height: 80px;
+  margin: 10px 0;
+  min-height: 40px;
   text-align: center;
   display: flex;
   justify-content: center;
   align-items: center;
   align-content: center;
 }
 /* Action links... */
 .processes-list .bottom-actions-links {
   transition: all var(--common-animation-time);
 }
-.processes-list .bottom-actions-links a {
+.processes-list .bottom-actions-links > * {
   display: none;
-  color: var(-layout-theme-primary-color-dark1);
-  cursor: pointer;
   margin: 0 10px;
 }
+.processes-list .bottom-actions-links > a {
+  color: var(--layout-theme-primary-color-dark1);
+  cursor: pointer;
+}
 .processes-list .bottom-actions-links a + a::before {
-  display: inline-block;
+  /* display: inline-block; */
 }
 .processes-list .bottom-actions-links a:hover {
   text-decoration: underline;
 }
 /* Show 'Reload' (after error) button if error... */
 .processes-list.error .bottom-actions-links a#action-clear-and-reload,
 /* Show 'Load more' button for all 'order by' values except for 'random'... */
-.processes-list:not(.order-random, .error) .bottom-actions-links a#action-load-more,
+.processes-list.has-more-data.has-search:not(.error) .bottom-actions-links a#action-load-more,
+.processes-list.has-more-data:not(.order-random, .error) .bottom-actions-links a#action-load-more,
+.processes-list:not(.has-more-data, .empty, .error) .bottom-actions-links span#show-total-records-number,
 /* Show 'Refresh' button for 'random' 'order by' value... */
-.processes-list.order-random:not(.error) .bottom-actions-links a#action-reload-random {
+.processes-list.order-random:not(.error, .has-search) .bottom-actions-links a#action-reload-random {
   display: inline-block;
 }
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.6.0/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.6.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -62,14 +62,15 @@
             // Methods...
 
             shiftRowHandler(event, row, row_id) {
                 CompareRowClick.disableRowClickHandler();
                 // Add row from source to target array
                 event.preventDefault();
                 row.parentElement.parentElement.classList.add('shift-right');
+                document.getElementById('replace-with-target-arrow').style.display = 'none';
                 const {
                     source_data,
                     target_data
                 } = this.sharedData;
                 const obj = source_data.find((item) => item.row_id == row_id);
                 // Creating new object with unique (?) row_id
                 const newObj = {
@@ -413,27 +414,30 @@
                     if (obj.row_id == rowId) {
                         this.comment += `* Removed exchange of ${obj.amount} ${obj.unit} ${obj.name} from ${obj.location}.\n`;
                         arr.splice(index, 1);
                         return true;
                     }
                     return false;
                 }
+                document.getElementById('replace-with-target-arrow').style.display = 'none';
                 target_data.filter(removeValue);
                 this.buildTable('target-table', target_data, true);
             },
 
             expandRowHandler(element) {
                 const {
                     target_data
                 } = this.sharedData;
                 CompareRowClick.disableRowClickHandler();
                 const elInputId = element.getAttribute('input_id');
                 const elAmount = element.getAttribute('amount');
                 const url = '/expand/' + elInputId + '/' + elAmount + '/';
                 const node = target_data.find((item) => item.input_id == elInputId);
+
+                document.getElementById('replace-with-target-arrow').style.display = 'none';
                 /* console.log('[CompareCore:expandRowHandler]', {
                  *   elInputId,
                  *   elAmount,
                  *   url,
                  *   node,
                  * })
                  */
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -32,35 +32,57 @@
          * - Add fallback for 'Reload' (reload last data chunk) if error occured.
          */
 
         // NOTE: Don't forget to call `startAllModules` for all the used modules...
         const allModulesList = [
             ProcessesListConstants,
             ProcessesListData,
-            ProcessesListDataRender,
             ProcessesListNodes,
-            // ProcessesListPagination, // UNUSED: Using incremental data loading
             ProcessesListStates,
             ProcessesListSearch,
+            ProcessesListDataRender,
             ProcessesListDataLoad,
         ];
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesList = {
+            // Proxy handlers...
+
             /** Update value of 'order by' parameter from user */
             onOrderByChange(target) {
                 // TODO: Move to Handlers module?
                 const {
                     value
                 } = target;
                 ProcessesListStates.setOrderBy(value);
                 ProcessesListDataLoad.loadData();
             },
 
+            /** Update value of 'filterBy' parameter from user */
+            onFilterByChange(target) {
+                // TODO: Move to Handlers module?
+                const {
+                    value
+                } = target;
+                ProcessesListStates.setFilterBy(value);
+                ProcessesListDataLoad.loadData();
+            },
+
+            /** Update value of 'userDb' parameter from user */
+            onUserDbChange(target) {
+                // TODO: Move to Handlers module?
+                const {
+                    value
+                } = target;
+                ProcessesListStates.setUserDb(value);
+                ProcessesListDataLoad.loadData();
+            },
+
+            // Data methods...
+
             /** clearAndReloadData -- Reload entire data (clear and load only first chunk)
              */
             clearAndReloadData() {
                 ProcessesListStates.clearData();
                 ProcessesListDataLoad.loadData();
             },
 
@@ -78,28 +100,29 @@
             },
 
             /** Get all the parameters passed in the url query */
             fetchUrlParams() {
                 // Get & store the database value form the url query...
                 const urlParams = CommonHelpers.parseQuery(window.location.search);
                 const {
-                    database,
-                    q: searchValue
+                    // database, // UNUSED: #41: Using `databases` and `userDb`
+                    q: searchValue,
                 } = urlParams;
-                // Get database from url or from server-passed data...
-                ProcessesListData.database = database || ProcessesListData.sharedParams.database;
+                /* // UNUSED: Get database from url or from server-passed data... (Used only for `searchUrl` requests.)
+                 * ProcessesListData.database = database || ProcessesListData.sharedParams.database;
+                 */
                 ProcessesListData.searchValue = searchValue || '';
             },
 
             /** startAllModules -- Start all the modules
              */
             startAllModules() {
                 // Start all the modules...
                 allModulesList.forEach((module) => {
-                    if (typeof module.start === 'function') {
+                    if (module && typeof module.start === 'function') {
                         try {
                             module.start();
                             /* // Alternate option: Delayed start...
                              * setTimeout(module.start.bind(module), 0);
                              */
                         } catch (error) {
                             // eslint-disable-next-line no-console
@@ -113,17 +136,22 @@
                         }
                     }
                 });
             },
 
             /** Start entrypoint */
             start(sharedParams) {
+                // Save shared data for future use...
                 ProcessesListData.sharedParams = sharedParams;
+                // Fetch url query parameters...
                 this.fetchUrlParams();
+                // Initialize all the modules...
                 this.startAllModules();
+                // Load data...
+                ProcessesListDataLoad.loadData();
             },
         };
 
         // Provide module...
         provide(ProcessesList);
     },
 );
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -19,52 +19,75 @@
     ) {
         // Define module...
 
         /** @descr Dynamic data loading support
          */
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesListDataLoad = {
+            __id: 'ProcessesListDataLoad',
+
             /** Load next/current (?) data chunk
              * @param {object} [opts] - Options.
              * @param {boolean} [opts.update] - Update current data chunk.
              */
-            loadData(_opts = true) {
+            loadData( /* opts = {} */ ) {
+                const {
+                    currentPage,
+                    orderBy,
+                    filterBy,
+                    userDb,
+                    searchValue,
+                    sharedParams,
+                    hasSearch
+                } =
+                ProcessesListData;
+                const {
+                    databases,
+                    // database, // UNUSED: #41: Using `databases` and `userDb`.
+                } = sharedParams;
                 const {
                     pageSize,
-                    processesApiUrl: urlBase
+                    processesApiUrl: urlBase,
+                    useDebug,
+                    defaultOrderBy,
+                    defaultFilterBy,
                 } = ProcessesListConstants;
-                const {
-                    currentPage,
-                    database,
-                    orderBy
-                } = ProcessesListData;
+                const userDbValue = databases[userDb]; // Could it be empty? Eg, to use: `|| database`
                 const offset = currentPage * pageSize; // TODO!
                 const params = {
-                    database,
-                    order_by: orderBy,
+                    search: searchValue, // TODO: Should the `order_by` parameter be disabled if the `search` parameter has used?
+                    database: userDbValue, // useDebug ? database : userDb || defaultUserDb,
+                    order_by: !hasSearch && orderBy !== defaultOrderBy ? orderBy : '',
+                    filter: filterBy !== defaultFilterBy ? filterBy : '',
                     offset,
                     limit: pageSize,
                 };
                 const urlQuery = CommonHelpers.makeQuery(params, {
                     addQuestionSymbol: true
                 });
                 const url = urlBase + urlQuery;
-                /* console.log('[ProcessesListDataLoad:loadData]: start', {
-                 *   url,
-                 *   params,
-                 *   urlQuery,
-                 *   urlBase,
-                 *   currentPage,
-                 *   pageSize,
-                 *   offset,
-                 *   orderBy,
-                 * });
-                 */
+                // DEBUG: Using temporarily while working with requests (issues #41, #45, etc)...
+                console.log('[ProcessesListDataLoad:loadData]: start', {
+                    searchValue,
+                    databases,
+                    userDbValue,
+                    useDebug,
+                    userDb,
+                    // database, // UNUSED: #41: Using `databases` and `userDb`.
+                    url,
+                    params,
+                    urlQuery,
+                    urlBase,
+                    currentPage,
+                    pageSize,
+                    offset,
+                    orderBy,
+                    filterBy,
+                });
                 ProcessesListStates.setLoading(true);
                 fetch(url)
                     .then((res) => {
                         const {
                             ok,
                             status,
                             statusText
@@ -95,40 +118,37 @@
                             data,
                             total_records: totalRecords
                         } = json;
                         const hasData = Array.isArray(data) && !!data.length;
                         const loadedRecords = hasData ? data.length : 0;
                         const currentRecords = offset + loadedRecords;
                         const hasMoreData = hasData && currentRecords < totalRecords;
-                        /* console.log('[ProcessesListDataLoad:loadData]: start', {
-                         *   hasMoreData,
-                         *   currentRecords,
+                        const availableCount = hasMoreData ? totalRecords - currentRecords : 0;
+                        /* console.log('[ProcessesListDataLoad:loadData]: success', {
+                         *   availableCount,
                          *   totalRecords,
+                         *   hasData,
                          *   loadedRecords,
-                         *   offset,
-                         *   url,
-                         *   params,
-                         *   urlQuery,
-                         *   urlBase,
-                         *   currentPage,
-                         *   pageSize,
-                         *   orderBy,
-                         *   json,
+                         *   currentRecords,
+                         *   hasMoreData,
+                         *   data,
                          * });
                          */
                         // Update total records number...
-                        ProcessesListData.totalRecords = totalRecords;
+                        // ProcessesListData.totalRecords = totalRecords;
+                        ProcessesListStates.setTotalRecordsCount(totalRecords);
                         // Append data to current table...
-                        // TODO: Use `opts.update` to update last data chunk.
+                        // TODO: Use `opts.update` to update (replace rows) last loaded data set.
                         ProcessesListDataRender.renderTableData(data, {
                             append: true
                         });
                         ProcessesListStates.setError(undefined); // Clear the error: all is ok
                         ProcessesListStates.setHasData(ProcessesListData.hasData || hasData); // Update 'has data' flag
                         ProcessesListStates.setHasMoreData(hasMoreData); // Update 'has more data' flag
+                        ProcessesListStates.updateAvailableRecordsInfo(availableCount);
                     })
                     .catch((error) => {
                         // eslint-disable-next-line no-console
                         console.error('[ProcessesListDataLoad:loadData]: error (catched)', {
                             error,
                             url,
                             params,
@@ -142,18 +162,13 @@
                     })
                     .finally(() => {
                         ProcessesListStates.setLoading(false);
                         // Update all the page dynamic elements?
                         ProcessesListStates.updatePage();
                     });
             },
-
-            /** Load first portion of data to display */
-            start() {
-                this.loadData();
-            },
         };
 
         // Provide module...
         provide(ProcessesListDataLoad);
     },
 );
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,14 @@
     ) {
         // Define module...
 
         /** @descr Render table content.
          */
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesListDataRender = {
             clearTableData() {
                 const tBodyNode = ProcessesListNodes.getTBodyNode();
                 tBodyNode.replaceChildren();
             },
 
             renderDataRow(rowData) {
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,14 @@
          *
          * TODO:
          *   - Cache found nodes?
          *   - Throw error if node not found?
          */
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesListNodes = {
             getSearchBarNode() {
                 const node = document.getElementById('query_string');
                 return node;
             },
 
             getTBodyNode() {
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,14 @@
          * Sample of pagination node in html:
          * ```
          *   <div class="table-pagination"></div>
          * ```
          */
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesListPagination = {
             // TODO: `ProcessesListPagination` should be exposed to global scope or `onNavigationClick` should be proxied.
             renderNavigationLink(id, text) {
                 return `<a pagination-id="${id}" class="link" onClick="ProcessesListPagination.onNavigationClick(this)">${text}</a>`;
             },
 
             renderNavigationText(text) {
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,63 +1,78 @@
 modules.define(
     'ProcessesListSearch',
     [
         // Required modules...
         'CommonHelpers',
         'ProcessesListData',
+        'ProcessesListDataLoad',
         'ProcessesListNodes',
+        'ProcessesListStates',
     ],
     function provide_ProcessesListSearch(
         provide,
         // Resolved modules...
         CommonHelpers,
         ProcessesListData,
+        ProcessesListDataLoad,
         ProcessesListNodes,
+        ProcessesListStates,
     ) {
         // Define module...
 
         /** @descr Search bar support
          */
 
         // global module variable
-        // eslint-disable-next-line no-unused-vars
         const ProcessesListSearch = {
-            /** Go to the search page (TODO: to refactor?) */
+            __id: 'ProcessesListSearch',
+
+            /* [>* UNUSED (old approach): Go to the search page (TODO: to refactor?) <]
+             * doSearchRedirect() {
+             *   const { database } = ProcessesListData;
+             *   const { searchUrl } = ProcessesListData.sharedParams;
+             *   const searchBar = ProcessesListNodes.getSearchBarNode();
+             *   const searchValue = searchBar && searchBar.value;
+             *   // TODO: pare search value with previous (if exists)?
+             *   if (searchValue !== ProcessesListData.searchValue) {
+             *     ProcessesListData.searchValue = searchValue; // Useless due to following redirect
+             *     // If searchValue is empty, then go to index (processes-list, root) page, else -- to the search page...
+             *     const urlParams = {
+             *       database,
+             *       q: searchValue,
+             *     };
+             *     const urlQuery = CommonHelpers.makeQuery(urlParams, { addQuestionSymbol: true });
+             *     const urlBase = searchValue ? searchUrl : '/';
+             *     const url = urlBase + urlQuery;
+             *     [> console.log('[ProcessesListSearch:doSearch]', {
+             *      *   url,
+             *      *   urlQuery,
+             *      *   urlParams,
+             *      *   urlBase,
+             *      *   searchValue,
+             *      *   searchUrl,
+             *      * });
+             *      <]
+             *     location.assign(url);
+             *   }
+             *   return false;
+             * },
+             */
+
+            /** Apply search */
             doSearch() {
-                const {
-                    database
-                } = ProcessesListData;
-                const {
-                    searchUrl
-                } = ProcessesListData.sharedParams;
                 const searchBar = ProcessesListNodes.getSearchBarNode();
-                const searchValue = searchBar && searchBar.value;
-                // TODO: pare search value with previous (if exists)?
+                const searchValue = searchBar.value;
+                // If value had changed...
                 if (searchValue !== ProcessesListData.searchValue) {
+                    const hasSearch = !!searchValue;
+                    ProcessesListStates.setHasSearch(hasSearch);
                     ProcessesListData.searchValue = searchValue; // Useless due to following redirect
-                    // If searchValue is empty, then go to index (processes-list, root) page, else -- to the search page...
-                    const urlParams = {
-                        database,
-                        q: searchValue,
-                    };
-                    const urlQuery = CommonHelpers.makeQuery(urlParams, {
-                        addQuestionSymbol: true
-                    });
-                    const urlBase = searchValue ? searchUrl : '/';
-                    const url = urlBase + urlQuery;
-                    /* console.log('[ProcessesListSearch:doSearch]', {
-                     *   url,
-                     *   urlQuery,
-                     *   urlParams,
-                     *   urlBase,
-                     *   searchValue,
-                     *   searchUrl,
-                     * });
-                     */
-                    location.assign(url);
+                    ProcessesListStates.clearData();
+                    ProcessesListDataLoad.loadData();
                 }
                 return false;
             },
 
             searchKeyHandler(event) {
                 if (event.key === 'Enter') {
                     this.doSearch();
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-0.6.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/compare.html`

 * *Files 22% similar despite different names*

```diff
@@ -39,63 +39,42 @@
     <div class="column one-half">
       <h3><a href="{{ url_for('process_detail', id=source_node.id) }}">{{ source_node.name }}</a></h3>
       <table class="fixed-table fixed-table-active compare-table" id="source-table" width="100%">
       </table>
     </div>
     <div class="column one-half">
       <h3><a href="{{ url_for('process_detail', id=target_node.id) }}">{{ target_node.name }}</a>
-      <span onclick="CompareCore.replaceWithTargetHandler(this)"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
+      <span onclick="CompareCore.replaceWithTargetHandler(this)" id="replace-with-target-arrow"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
       <table class="fixed-table fixed-table-active compare-table" id="target-table" width="100%">
       </table>
     </div>
   </div>
 </div>
 
 <script>
   modules.require('CompareCore', (CompareCore) => {
-    /* // Enable debug mode...
-     * const useDebug = true;
-     * // TODO: Expose it to global scope?
-     */
-
     // Global variables for compare tables feature (via global variable `sharedData`)...
     const sharedData = {
       source_data: {{ source_data_json|safe }}, // TDataRecord[]
       target_data: {{ target_data_json|safe }}, // TDataRecord[]
       target_node: {{ target_json|safe}},
       source_id: {{ source_node.id }},
       target_id: {{ target_node.id }},
       target_name: '{{ target_node.name|safe }}',
       source_node_unit: '{{source_node.unit}}',
       source_node_location: '{{source_node.location}}',
+      /* XXX: Probably these labels should be added in `index.html`? Is it required here?
+       * // TODO: Remove when #41 is closed
+       * // Not used anyway?
+       * source_db_label: '{{ source }}',
+       * target_db_label: '{{ target }}',
+       * proxy_db_label: '{{ proxy }}',
+       */
     };
 
-    /* // DEBUG: Crop data table to easier debugging...
-     * if (useDebug) {
-     *   sharedData.source_data.length = 2;
-     *   sharedData.target_data.length = 2;
-     * }
-     */
-
-    /* // DEBUG: Emulate pre-collapsed elements data...
-     * if (useDebug) {
-     *   // Link first columns...
-     *   const collapsedGroupId = 'Collapsed-0-abcdef'
-     *   sharedData.source_data[0].collapsed = true
-     *   sharedData.source_data[0]['collapsed-group'] = collapsedGroupId;
-     *   sharedData.target_data[0].collapsed = true
-     *   sharedData.target_data[0]['collapsed-group'] = collapsedGroupId;
-     *   console.log('DEBUG: Emulate pre-collapsed elements data', {
-     *     source_data: sharedData.source_data,
-     *     target_data: sharedData.target_data,
-     *   });
-     *   debugger;
-     * }
-     */
-
     // Export to global scope (to access from generated html code handlers).
     window.CompareCore = CompareCore;
 
     // Start core module...
     CompareCore.start(sharedData);
   });
 </script>
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/databases.html`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,26 @@
           <select class="u-full-width" id="source" name="source">
             {% for d in databases %}
             <option value="{{ d }}">{{ d }}</option>
             {% endfor %}
           </select>
         </div>
         <div class="five columns">
-          <label for="source">Target database</label>
+          <label for="target">Target database</label>
           <select class="u-full-width" id="target" name="target">
             {% for d in databases %}
             <option value="{{ d }}">{{ d }}</option>
             {% endfor %}
           </select>
         </div>
         <div class="two columns">
+<!--
           <label id="use_proxy_toggle" for="use_proxy">Use proxy</label>
           <input type="checkbox" onclick="showProxySection(this,'proxy-row')" name="use-proxy" checked>
+-->
         </div>
       </div>
       <div class="row">
         <div id="proxy-row">
           <div class="five columns">
             <label for="proxy-existing">Use existing database for proxy, or...</label>
             <select class="u-full-width" id="proxy-existing" name="proxy-existing">
@@ -47,24 +49,25 @@
         </div>
       </div>
     </form>
   </div>
 </div>
 
 <script>
-function showProxySection(checkbox, section_div) {
-   if( checkbox.checked == true ) {
-      document.getElementById(section_div).style.display = "block";
-   } else {
-      document.getElementById(section_div).style.display = "none";
-   }
-};
+// function showProxySection(checkbox, section_div) {
+//    if( checkbox.checked == true ) {
+//       document.getElementById(section_div).style.display = "block";
+//    } else {
+//       document.getElementById(section_div).style.display = "none";
+//    }
+// };
 
 // var select_cache = "";
 
+// Greys out "Use existing database" values to show that a new database will be used
 document.getElementById("proxy-new").addEventListener("keyup", function() {
   var db_select = document.getElementById("proxy-existing");
   if (this.value.trim().length) {
     // select_cache = db_select.value;
     // db_select.value = "None";
     db_select.style.opacity = 0.3;
   } else {
```

#### html2text {}

```diff
@@ -3,14 +3,13 @@
 ****** Select Source and Target Databases ******
 {% for d in databases %}
 {{ d }}
 {% endfor %}
 {% for d in databases %}
 {{ d }}
 {% endfor %}
-Use proxy *
 {% for d in databases %}
 {{ d }}
 {% endfor %}
 Create a new database [proxy-new           ]
 Save changes [Submit]
  {% include 'footer.html' %}
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/navigation.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 <div class="row" style="margin-top: 5%">
     <div class="two columns"><a href="{{ url_for('index') }}">home</a></div>
     <div class="two columns"><a href="{{ url_for('select_matching_files') }}">Input files ({{ file_number or 0}})</a></div>
     <div class="two columns">User: {{ user }}</div>
-    <div class="two columns">Editing: {{ changes_file }}</div>
-    <div class="four columns">Proxy: {{ proxy or "None" }}</div>
+    <div class="six columns">Proxy: {{ proxy or "None" }}</div>
 </div>
 <div class="row">
     {% if project %}<div class="four columns">Project: {{ project }} | <a href="{{ url_for('select_project') }}">Change</a></div>{% endif %}
     {% if source %}<div class="four columns">Source DB: {{ source }}</div>
     <div class="four columns">Target DB: {{ target }} | <a href="{{ url_for('select_databases') }}">Change</a></div>{% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 home
 Input_files_({{_file_number_or_0}})
 User: {{ user }}
-Editing: {{ changes_file }}
 Proxy: {{ proxy or "None" }}
 {% if project %}
 Project: {{ project }} | Change
 {% endif %} {% if source %}
 Source DB: {{ source }}
 Target DB: {{ target }} | Change
 {% endif %}
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.6.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.6.0/bw_matchbox/bin/matchbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """bw_matchbox scripts.
 
 Usage:
-  matchbox setup
+  matchbox setup [<output_dir>]
   matchbox example_project [<project_name>]
   matchbox webapp <config> [--port=<port>] [--localhost]
 
 Options:
   -h --help     Show this screen.
   --version     Show version.
 
 """
-import datetime
-import json
 from pathlib import Path
 
 import bw2data as bd
 import bw2io as bi
 from docopt import docopt
 
 from bw_matchbox.webapp import configure_app, matchbox_app
@@ -25,15 +23,15 @@
 CWD = Path.cwd()
 
 CONFIG_TEMPLATE = """[users]
 johnny = "mnemonic"
 
 [files]
 directories = []
-changes_file = "{}"
+output_dir = "{}"
 """
 
 CHANGES_TEMPLATE = {
     "name": "<change-this-please>",
     "licenses": [
         {
             "name": "CC BY 4.0",
@@ -56,33 +54,29 @@
     "delete": [],
     "disaggregate": [],
     "replace": [],
     "update": [],
 }
 
 
-def create_setup_files(filename, changesfile):
+def create_setup_files(filename, output_dir):
     if not filename.lower().endswith(".toml"):
         filename += ".toml"
-    if not changesfile.lower().endswith(".json"):
-        changesfile += ".json"
-    with open(CWD / filename, "w") as f:
-        f.write(CONFIG_TEMPLATE.format(CWD / changesfile))
+    with open(CWD / filename, "w", newline="\n") as f:
+        data = CONFIG_TEMPLATE.format(str(output_dir).replace('\\', '/'))
+        f.write(data)
         print("Created config file {}".format(CWD / filename))
-    with open(CWD / changesfile, "w") as f:
-        CHANGES_TEMPLATE["created"] = datetime.datetime.now().isoformat()
-        json.dump(CHANGES_TEMPLATE, f, ensure_ascii=False, indent=2)
-        print("Created changes file {}".format(CWD / changesfile))
 
 
 def main():
     args = docopt(__doc__, version="bw_matchbox app 1.0")
 
     if args["setup"]:
-        create_setup_files("config.toml", "changes.json")
+        output_dir = args["<output_dir>"] or CWD
+        create_setup_files("config.toml", Path(output_dir).resolve())
     elif args["example_project"]:
         name = args["<project_name>"] or "matchbox-example"
         bi.install_project("USEEIO-1.1", name)
         bd.projects.set_current(name)
         bd.Database("USEEIO-1.1").copy("USEEIO-copy")
         print(
             f"Create project {name}. Make sure to select `USEEIO-1.1` for one "
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.6.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/data/dare.json` & `bw_matchbox-0.6.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/utils.py` & `bw_matchbox-0.6.0/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/bw_matchbox/webapp.py` & `bw_matchbox-0.6.0/bw_matchbox/webapp.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import string
 import uuid
 from pathlib import Path
 
 import bw2data as bd
 import flask
 import tomli
+import whoosh
 from bw2data.backends import ActivityDataset as AD
 from flask_httpauth import HTTPBasicAuth
 from peewee import fn
 from werkzeug.security import check_password_hash, generate_password_hash
 
 from .utils import name_close_enough, similar_location
 
@@ -49,19 +50,21 @@
         # double `\\`).
         raise ValueError("Invalid or unreadable config file")
 
     app.config["mb_users"] = {
         user: generate_password_hash(password)
         for user, password in config["users"].items()
     }
-    app.config["mb_changes_file"] = config["files"]["changes_file"]
-    try:
-        json.load(open(app.config["mb_changes_file"], "rb"))
-    except:
-        raise ValueError("Can't read changes file")
+    app.config["mb_output_dir"] = Path(config["files"]["output_dir"])
+    if not (
+        app.config["mb_output_dir"].is_dir()
+        and os.access(app.config["mb_output_dir"], os.W_OK)
+    ):
+        raise ValueError("`output_dir` is invalid")
+
     return app
 
 
 def get_context():
     project = flask.request.cookies.get("project")
     if not project:
         return flask.redirect(flask.url_for("select_project"))
@@ -105,15 +108,14 @@
     else:
         resp = flask.make_response(
             flask.render_template(
                 "project.html",
                 file_number=sum(1 for obj in files if obj["enabled"]),
                 projects=[o for o in bd.projects],
                 user=auth.current_user(),
-                changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
             )
         )
         resp.delete_cookie("project")
         resp.delete_cookie("source")
         resp.delete_cookie("target")
         return resp
 
@@ -127,40 +129,36 @@
     bd.projects.set_current(project)
 
     files = get_files()
 
     if flask.request.method == "POST":
         source = flask.request.form["source"]
         target = flask.request.form["target"]
-        use_proxy = "use-proxy" in flask.request.form
         proxy_existing = flask.request.form["proxy-existing"]
         proxy_new = flask.request.form["proxy-new"].strip()
+
         if source != target:
             resp = flask.make_response(flask.redirect(flask.url_for("index")))
             resp.set_cookie("source", source)
             resp.set_cookie("target", target)
 
-            if use_proxy:
-                if proxy_new:
-                    bd.Database(proxy_new).register()
-                    resp.set_cookie("proxy", proxy_new)
-                else:
-                    resp.set_cookie("proxy", proxy_existing)
+            if proxy_new:
+                bd.Database(proxy_new).register()
+                resp.set_cookie("proxy", proxy_new)
             else:
-                resp.set_cookie("proxy", "")
+                resp.set_cookie("proxy", proxy_existing)
 
             return resp
 
     resp = flask.make_response(
         flask.render_template(
             "databases.html",
             project=project,
             file_number=sum(1 for obj in files if obj["enabled"]),
             user=auth.current_user(),
-            changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
             databases=bd.databases,
         )
     )
     resp.delete_cookie("source")
     resp.delete_cookie("target")
     return resp
 
@@ -206,15 +204,14 @@
             files=files_formatted,
             file_number=sum(1 for obj in files if obj["enabled"]),
             project=proj,
             proxy=proxy,
             source=s,
             target=t,
             user=auth.current_user(),
-            changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         )
     )
     resp.set_cookie("files", json.dumps(files))
     return resp
 
 
 @matchbox_app.route("/", methods=["GET"])
@@ -237,122 +234,138 @@
         target=t,
         file_number=sum(1 for obj in files if obj["enabled"]),
         table_data=[obj for obj, _ in zip(bd.Database(s), range(50))],
         query_string="",
         database=s,
         proxy=proxy,
         user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
     )
 
 
+def apply_filter_to_qs(qs, filter_arg):
+    if filter_arg == "unmatched":
+        return [node for node in qs if not node.data.get("matched")]
+    else:
+        return [node for node in qs if node.data.get(filter_arg)]
+
+
+def apply_limit_offset(qs, limit, offset):
+    if offset:
+        qs = qs[offset:]
+    if limit:
+        qs = qs[:limit]
+    return qs
+
+
+def maybe_int(value):
+    if value in (None, ""):
+        return None
+    else:
+        return int(value)
+
+
 @matchbox_app.route("/processes", methods=["GET"])
 @auth.login_required
 def processes():
     """API Endpoint to get process data for dynamic table population.
 
     GET args:
 
     * database (str): Name of database to draw processes from. Defaults to source
-                      database (stored in cookie) if not given.
-    * order_by (str): Parameter to sort by. Random if not provided. Valid parameters:
+                    database (stored in cookie) if not given.
+    * limit (int): Number of results to return
+    * order_by (str, optional): Parameter to sort by. Random if not provided.
+                    Valid parameters:
         * name (will be used 99% of the time)
         * location
         * product (short name for reference product)
-    * offset (int): Offset from beginning of sorted values. Zero-indexed.
+    * offset (int, optional): Offset from beginning of sorted values. Zero-indexed.
                     Only used if sorting.
-    * limit (int): Number of results to return
+    * filter (string, optional): Optional attribute filter. Should be one of
+                    `matched`, `unmatched`, or `waitlist`.
+    * search (string, optional): Optional parameter to pass to search index.
+                    Note that this overrides `order_by`.
 
     Response data format (JSON):
 
     ```
         [
             {
                 'details_url': 'URL for `process_detail` page for this activity',
                 'match_url': 'URL for `match` page for this activity',
                 'matched': 'Boolean. Whether or not process is already matched.',
+                'waitlist': 'Boolean. Whether or not process has attribute `waitlist`.',
                 'id': 'Integer process ID',
                 'name': 'Process name',
                 'location': 'Process location',
                 'unit': 'Unit of reference product',
             }
         ]
     ```
     """
     context = get_context()
     proj, s, t, proxy = context
     bd.projects.set_current(proj)
 
     database_label = flask.request.args.get("database") or s
-    qs = AD.select().where(AD.database == database_label)
-
-    total_records = qs.count()
-
-    order_by = flask.request.args.get("order_by")
-    if order_by and order_by in ("name", "location", "product"):
-        qs = qs.order_by(getattr(AD, order_by))
+    limit = maybe_int(flask.request.args.get("limit"))
+    offset = maybe_int(flask.request.args.get("offset"))
+    filter_arg = flask.request.args.get("filter")
+
+    search_query = flask.request.args.get("search")
+    if search_query:
+        # Override default very small search limit
+        qs = [
+            x._document
+            for x in bd.Database(database_label).search(search_query, limit=1000)
+        ]
+        if filter_arg:
+            qs = apply_filter_to_qs(qs, filter_arg)
+        total_records = len(qs)
+        qs = apply_limit_offset(qs, limit, offset)
     else:
-        qs = qs.order_by(fn.Random())
-
-    offset = flask.request.args.get("offset")
-    if offset:
-        qs = qs.offset(int(offset))
+        qs = AD.select().where(AD.database == database_label)
 
-    limit = flask.request.args.get("limit")
-    if limit:
-        qs = qs.limit(int(limit))
-    else:
-        qs = qs.limit(50)
+        order_by = flask.request.args.get("order_by")
+        if order_by and order_by in ("name", "location", "product"):
+            qs = qs.order_by(getattr(AD, order_by))
+        else:
+            qs = qs.order_by(fn.Random())
+
+        if not filter_arg:
+            total_records = qs.count()
+
+            if offset:
+                qs = qs.offset(offset)
+            if limit:
+                qs = qs.limit(limit)
+        else:
+            qs = apply_filter_to_qs(qs, filter_arg)
+            total_records = len(qs)
+            qs = apply_limit_offset(qs, limit, offset)
 
     payload = {
         "total_records": total_records,
         "data": [
             {
                 "details_url": flask.url_for("process_detail", id=obj.id),
                 "match_url": flask.url_for("match", source=obj.id),
                 "matched": bool(obj.data.get("matched")),
+                "waitlist": bool(obj.data.get("waitlist")),
                 "id": obj.id,
                 "name": obj.name,
                 "location": obj.location,
                 "unit": obj.data["unit"],
             }
             for obj in qs
         ],
     }
     return flask.jsonify(payload)
 
 
-@matchbox_app.route("/unmatched", methods=["GET"])
-@auth.login_required
-def unmatched():
-    context = get_context()
-    if isinstance(context, flask.Response):
-        return context
-    proj, s, t, proxy = context
-
-    files = get_files()
-
-    bd.projects.set_current(proj)
-    return flask.render_template(
-        "index.html",
-        title="Unmatched Processes",
-        unmatched_link=False,
-        project=proj,
-        proxy=proxy,
-        source=s,
-        target=t,
-        file_number=sum(1 for obj in files if obj["enabled"]),
-        table_data=[obj for obj, _ in zip(bd.Database(s), range(50))],
-        query_string="",
-        database=s,
-        user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
-    )
-
-
 # @matchbox_app.route("/match-status", methods=["GET"])
 # @auth.login_required
 # def match_status():
 #     crud = {}
 #     status = {}
 #     failed = []
 
@@ -392,23 +405,24 @@
     proj, s, t, proxy = context
 
     files = get_files()
     bd.projects.set_current(proj)
 
     q = flask.request.args.get("q")
     embed = flask.request.args.get("e")
+    search_db = flask.request.args.get("database")
+
     if embed:
         source = bd.get_activity(id=int(flask.request.args.get("source")))
         return flask.render_template(
             "search-embedded.html",
             source=source,
-            table_data=bd.Database(t).search(q, limit=100),
+            table_data=bd.Database(search_db or t).search(q, limit=100),
         )
     else:
-        search_db = flask.request.args.get("database")
         return flask.render_template(
             "index.html",
             project=proj,
             source=s,
             target=t,
             file_number=sum(1 for obj in files if obj["enabled"]),
             proxy=proxy,
@@ -429,61 +443,94 @@
     node = bd.get_node(id=id)
 
     attr = flask.request.args.get("attr")
     value = flask.request.args.get("value")
 
     if attr is None or value is None:
         flask.abort(400)
-    if attr in ("highlighted", "matched"):
+    if attr in ("highlighted", "matched", "no_match_needed"):
         if value not in ("0", "1"):
             flask.abort(400)
         value = {"0": False, "1": True}[value]
 
     node[attr] = value
-    node.save()
+
+    try:
+        node.save()
+    except whoosh.index.LockError:
+        # MAIN_WRITELOCK not being released. Can ignore as we don't
+        # change anything that is in the index anyway.
+        pass
     return ""
 
 
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
+    proxy_node = bd.get_node(id=node["proxy_id"]) if node.get("proxy_id") else None
+
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
+        authors=",".join(
+            [obj.get("name", "Unknown") for obj in node.get("authors", [])]
+        ),
         project=proj,
         proxy=proxy,
+        proxy_node=proxy_node,
         source=s,
         target=t,
         file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         same_name_count=same_name_count,
         same_name=same_name,
         technosphere=technosphere,
         biosphere=biosphere,
         show_matching=False,
     )
 
 
+@matchbox_app.route("/multi-match/<id>", methods=["GET"])
+@auth.login_required
+def multi_match(id):
+    context = get_context()
+    proj, s, t, proxy = context
+    bd.projects.set_current(proj)
+
+    node = bd.get_node(id=id)
+    node["matched"] = True
+    node["no_match_needed"] = True
+    node.save()
+
+    for ds in AD.select().where(
+        AD.name == node["name"], AD.database == node["database"], AD.id != node.id
+    ):
+        if not ds.data.get("matched"):
+            ds.data["matched"] = True
+            ds.data["no_match_needed"] = True
+            ds.save()
+    return ""
+
+
 @matchbox_app.route("/match/<source>", methods=["GET"])
 @auth.login_required
 def match(source):
     context = get_context()
     if isinstance(context, flask.Response):
         return context
     proj, s, t, proxy = context
@@ -500,15 +547,14 @@
         ds=node,
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
         file_number=sum(1 for obj in files if obj["enabled"]),
         user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         query_string=node["name"] + " " + node.get("location", ""),
         matches=matches,
     )
 
 
 def check_similar(node, candidates):
     for index, candidate in enumerate(candidates):
@@ -587,15 +633,14 @@
         title="Database Comparison Page",
         project=proj,
         proxy=proxy,
         source=s,
         target=t,
         target_json=json.dumps(target_itself),
         user=auth.current_user(),
-        changes_file=Path(matchbox_app.config["mb_changes_file"]).name,
         file_number=sum(1 for obj in files if obj["enabled"]),
         source_node=source,
         source_data_json=json.dumps(source_technosphere),
         target_node=target,
         target_data_json=json.dumps(target_technosphere),
     )
 
@@ -660,10 +705,11 @@
         process.new_edge(
             type="technosphere",
             input=bd.get_activity(id=exc["input_id"]),
             amount=exc["amount"],
         ).save()
 
     source["matched"] = True
+    source["proxy_id"] = process.id
     source.save()
 
     return flask.redirect(flask.url_for("process_detail", id=process.id))
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.6.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.5.1
+Version: 0.6.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
@@ -84,15 +84,15 @@
 To use `bw_matchbox`, you need to do the following:
 
 ### Create a configuration file
 
 Configuration is done via a `toml` file. See [`config_example.toml`](https://github.com/cauldron/bw_matchbox/blob/main/config_example.toml) for the structure of this file. It needs to provide the following:
 
 * `[users]` section: Authentication, via a set of usernames and passwords
-* `changes_file`: Location of the file where we will save your matching selections.
+* `output_dir`: Location of the directory where output files will be written. Must be writable.
 * `directories`: (Optional) Location of existing [randonneur](https://github.com/cmutel/randonneur) matching files to use, if any.
 
 The easiest way to set this up is with:
 
 ```console
 matchbox setup
 ```
```

### Comparing `bw_matchbox-0.5.1/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.6.0/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/docs/conf.py` & `bw_matchbox-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.5.1/setup.cfg` & `bw_matchbox-0.6.0/setup.cfg`

 * *Files identical despite different names*

