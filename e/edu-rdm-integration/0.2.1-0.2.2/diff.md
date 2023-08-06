# Comparing `tmp/edu-rdm-integration-0.2.1.tar.gz` & `tmp/edu-rdm-integration-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu-rdm-integration-0.2.1.tar", last modified: Sat Aug  5 19:51:45 2023, max compression
+gzip compressed data, was "edu-rdm-integration-0.2.2.tar", last modified: Sun Aug  6 10:05:10 2023, max compression
```

## Comparing `edu-rdm-integration-0.2.1.tar` & `edu-rdm-integration-0.2.2.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.740099 edu-rdm-integration-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     4066 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.1/CHANGELOG.md
--rwxr-xr-x   0 root         (0) root         (0)     5358 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3458 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      175 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    16257 2023-08-05 19:51:45.741099 edu-rdm-integration-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11460 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.657099 edu-rdm-integration-0.2.1/requirements/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.661099 edu-rdm-integration-0.2.1/requirements/dependencies/
--rw-r--r--   0 root         (0) root         (0)       89 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/requirements/dependencies/development_packages.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/dependencies/external_packages.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/requirements/dependencies/internal_packages.txt
--rw-r--r--   0 root         (0) root         (0)      372 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.1/requirements/dependencies/internal_sources.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/dependencies/production_packages.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/requirements/dependencies/system_packages.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/dependencies/testing_packages.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/development.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/production.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/requirements/stage.txt
--rw-r--r--   0 root         (0) root         (0)      471 2023-08-05 19:51:45.742099 edu-rdm-integration-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2842 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.647099 edu-rdm-integration-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.672099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/
--rw-r--r--   0 root         (0) root         (0)       72 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.690099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      363 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/apps.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/caches.py
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/consts.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/enums.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/errors.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/functions.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/helpers.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/managers.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/presenters.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/receivers.py
--rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/results.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/runners.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/strategies.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/strings.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/tests.py
--rw-r--r--   0 root         (0) root         (0)      496 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/validators.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/app_settings.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.691099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.694099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1310 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/caches.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/functions.py
--rw-r--r--   0 root         (0) root         (0)     5219 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/managers.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.695099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.709099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7212 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/caches.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/consts.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/enums.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/errors.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/functions.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/managers.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/results.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/runners.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/strings.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/tests.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/validators.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/strategies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.709099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.718099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
--rw-r--r--   0 root         (0) root         (0)     7423 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/strategies.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/consts.py
--rw-r--r--   0 root         (0) root         (0)     9117 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/entities.py
--rw-r--r--   0 root         (0) root         (0)     4876 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.720099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.734099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/caches.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/consts.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/enums.py
--rw-r--r--   0 root         (0) root         (0)      291 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/errors.py
--rw-r--r--   0 root         (0) root         (0)    11664 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/functions.py
--rw-r--r--   0 root         (0) root         (0)     3076 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5665 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/managers.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/presenters.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/requests.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/results.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/runners.py
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/strings.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/tests.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/validators.py
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/consts.py
--rw-r--r--   0 root         (0) root         (0)     6718 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/strategies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.736099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.738099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/commands/collect_models_data.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/commands/export_entities_data.py
--rw-r--r--   0 root         (0) root         (0)    19777 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/general.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/generators.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.740099 edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/
--rw-r--r--   0 root         (0) root         (0)    18718 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19850 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/models.py
--rw-r--r--   0 root         (0) root         (0)     6806 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/storages.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 19:51:45.674099 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16257 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5790 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      172 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.781885 edu-rdm-integration-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     4468 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/CHANGELOG.md
+-rwxr-xr-x   0 root         (0) root         (0)     5358 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      175 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16659 2023-08-06 10:05:10.781885 edu-rdm-integration-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-08-05 19:51:37.000000 edu-rdm-integration-0.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.726885 edu-rdm-integration-0.2.2/requirements/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.730885 edu-rdm-integration-0.2.2/requirements/dependencies/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.2/requirements/dependencies/development_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/dependencies/external_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/requirements/dependencies/internal_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      372 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.2/requirements/dependencies/internal_sources.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/dependencies/production_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.2/requirements/dependencies/system_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/dependencies/testing_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/development.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/production.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/requirements/stage.txt
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-06 10:05:10.783886 edu-rdm-integration-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.717886 edu-rdm-integration-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.735885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.747886 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/caches.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/enums.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/managers.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/receivers.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/results.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/runners.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/tests.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/validators.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.748885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.750886 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5219 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.751886 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.759885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/strategies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.760886 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.767886 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)     7423 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/consts.py
+-rw-r--r--   0 root         (0) root         (0)     9117 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/entities.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.768885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.776885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)    11755 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-08-06 10:05:01.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/requests.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/consts.py
+-rw-r--r--   0 root         (0) root         (0)     6718 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/strategies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.778885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.779885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/commands/collect_models_data.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/commands/export_entities_data.py
+-rw-r--r--   0 root         (0) root         (0)    19777 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/general.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/generators.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.781885 edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19850 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/models.py
+-rw-r--r--   0 root         (0) root         (0)     6806 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/storages.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 10:05:10.738885 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16659 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5790 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 19:51:45.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      173 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-06 10:05:10.000000 edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/top_level.txt
```

### Comparing `edu-rdm-integration-0.2.1/CHANGELOG.md` & `edu-rdm-integration-0.2.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,24 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.2.2] - 2023-08-06
+
+Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+### Добавлено
+
+- [EDUSCHL-19920](https://jira.bars.group/browse/EDUSCHL-19920)
+  PATCH Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+
 ## [0.2.1] - 2023-08-05
  
 Восстановление сборки пакета после ухода с poetry.
  
 ### Добавлено
  
 ### Изменено
```

### Comparing `edu-rdm-integration-0.2.1/CONDUCT.md` & `edu-rdm-integration-0.2.2/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/LICENSE` & `edu-rdm-integration-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/PKG-INFO` & `edu-rdm-integration-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 0.2.1
+Version: 0.2.2
 Summary: Интеграция с Региональной витриной данных
 Home-page: 
 Download-URL: 
 Author: BARS Group
 Author-email: bars@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -203,14 +203,24 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.2.2] - 2023-08-06
+
+Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+### Добавлено
+
+- [EDUSCHL-19920](https://jira.bars.group/browse/EDUSCHL-19920)
+  PATCH Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+
 ## [0.2.1] - 2023-08-05
  
 Восстановление сборки пакета после ухода с poetry.
  
 ### Добавлено
  
 ### Изменено
```

### Comparing `edu-rdm-integration-0.2.1/README.md` & `edu-rdm-integration-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/setup.py` & `edu-rdm-integration-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     find_packages,
     setup,
 )
 
 
 PROJECT = 'edu_rdm_integration'
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 current_dir_path = Path().resolve()
 
 
 #  Получение полного описания
 with open(str(current_dir_path / 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/caches.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/functions.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/helpers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/managers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/receivers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/receivers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/results.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/runners.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/adapters/strategies.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/adapters/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/app_settings.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/app_settings.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/apps.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/apps.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/caches.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/functions.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/managers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/base/runners.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/caches.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/functions.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/helpers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/managers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/results.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/runners.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/base/validators.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/calculated/strategies.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/calculated/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/results.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/collect_data/non_calculated/strategies.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/collect_data/non_calculated/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/consts.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/consts.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/entities.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/entities.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/enums.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/enums.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/caches.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/functions.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from edu_rdm_integration.consts import (
     LOGS_DELIMITER,
 )
 from edu_rdm_integration.enums import (
     FileUploadStatusEnum,
 )
 from edu_rdm_integration.export_data.base.consts import (
+    OPERATIONS_URLS_MAP,
     OPERATIONS_METHODS_MAP,
 )
 from edu_rdm_integration.export_data.base.errors import (
     BaseExportDataError,
 )
 from edu_rdm_integration.export_data.base.helpers import (
     BaseExportDataFunctionHelper,
@@ -245,14 +246,15 @@
                 method = OPERATIONS_METHODS_MAP.get(operation)
                 file_path = Path.joinpath(Path(settings.MEDIA_ROOT), relative_file_path)
 
                 request = RegionalDataMartEntityRequest(
                     datamart_name=settings.RDM_UPLOADER_CLIENT_DATAMART_NAME,
                     table_name=self.first_entity.key.lower(),
                     method=method,
+                    operation=OPERATIONS_URLS_MAP.get(operation),
                     parameters={},
                     headers={
                         'Content-Type': 'text/csv',
                     },
                     files=[],
                     data=file_path.open('rb').read(),
                 )
```

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/helpers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/managers.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/requests.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """
     Запрос на отправку данных сущности.
     """
 
     datamart_name: str
     table_name: str
     method: str
+    operation: str
     headers: dict
     parameters: dict = Field(default_factory=dict)
     files: list = Field(default_factory=list)
     data: Any = None
 
     def get_method(self):
         """
@@ -37,15 +38,15 @@
         """
         return self.method
 
     def get_url(self):
         """
         Получение сформированного URL.
         """
-        return f'/v2/datamarts/{self.datamart_name}/tables/{self.table_name}/upload'
+        return f'/v2/datamarts/{self.datamart_name}/tables/{self.table_name}/{self.operation}'
 
     def get_headers(self) -> dict:
         """
         Возвращает заголовки запроса.
         """
         return self.headers
```

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/results.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/results.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/runners.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/base/validators.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/export_data/strategies.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/export_data/strategies.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/general.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/general.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/management/generators.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/management/generators.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/0001_initial.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/models.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/models.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/storages.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/storages.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration/utils.py` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration/utils.py`

 * *Files identical despite different names*

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/PKG-INFO` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 0.2.1
+Version: 0.2.2
 Summary: Интеграция с Региональной витриной данных
 Home-page: 
 Download-URL: 
 Author: BARS Group
 Author-email: bars@bars.group
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
@@ -203,14 +203,24 @@
   MAJOR Название задачи или изменения.
  
 ### Изменено
  
 ### Исправлено
 
 
+## [0.2.2] - 2023-08-06
+
+Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+### Добавлено
+
+- [EDUSCHL-19920](https://jira.bars.group/browse/EDUSCHL-19920)
+  PATCH Для API РВД добавлена поддержка параметра типа операции для загрузки данных.
+
+
 ## [0.2.1] - 2023-08-05
  
 Восстановление сборки пакета после ухода с poetry.
  
 ### Добавлено
  
 ### Изменено
```

### Comparing `edu-rdm-integration-0.2.1/src/edu_rdm_integration.egg-info/SOURCES.txt` & `edu-rdm-integration-0.2.2/src/edu_rdm_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

