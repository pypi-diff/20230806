# Comparing `tmp/edc-pdutils-0.3.8.tar.gz` & `tmp/edc-pdutils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-pdutils-0.3.8.tar", last modified: Wed Jul  6 06:48:09 2022, max compression
+gzip compressed data, was "edc-pdutils-0.3.9.tar", last modified: Fri Aug 19 15:02:51 2022, max compression
```

## Comparing `edc-pdutils-0.3.8.tar` & `edc-pdutils-0.3.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.524839 edc-pdutils-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       94 2020-03-04 23:15:19.000000 edc-pdutils-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.506229 edc-pdutils-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.509411 edc-pdutils-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-pdutils-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1406 2022-06-23 21:54:26.000000 edc-pdutils-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-23 21:54:26.000000 edc-pdutils-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     3924 2022-07-06 06:48:09.524960 edc-pdutils-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3086 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.511677 edc-pdutils-0.3.8/edc_pdutils/
--rw-r--r--   0 erikvw     (501) staff       (20)      744 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2021-05-16 19:48:26.000000 edc-pdutils-0.3.8/edc_pdutils/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      141 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.512898 edc-pdutils-0.3.8/edc_pdutils/column_handlers/
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/column_handlers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      527 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/column_handlers/column_apply.py
--rw-r--r--   0 erikvw     (501) staff       (20)      685 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/column_handlers/column_map.py
--rw-r--r--   0 erikvw     (501) staff       (20)      203 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2971 2022-07-06 06:42:34.000000 edc-pdutils-0.3.8/edc_pdutils/database.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.514222 edc-pdutils-0.3.8/edc_pdutils/df_exporters/
--rw-r--r--   0 erikvw     (501) staff       (20)      324 2020-10-06 17:42:55.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3219 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_crf_inline_tables_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1048 2020-10-06 17:42:55.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_crf_tables_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5488 2021-05-16 19:48:26.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)      921 2021-05-16 18:35:37.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_model_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)      791 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_noncrf_tables_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4319 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/df_exporters/tables_exporter.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.514824 edc-pdutils-0.3.8/edc_pdutils/df_handlers/
--rw-r--r--   0 erikvw     (501) staff       (20)      123 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/df_handlers/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2901 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_handlers/crf_df_handler.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2005 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_handlers/df_handler.py
--rw-r--r--   0 erikvw     (501) staff       (20)      823 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_handlers/non_crf_df_handler.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2308 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/df_handlers/registered_subject_df_handler.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.515303 edc-pdutils-0.3.8/edc_pdutils/dialects/
--rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/dialects/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3311 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/dialects/crf_dialect.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2637 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/dialects/mysql_dialect.py
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/dialects/rs_dialect.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1667 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)       77 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/mappings.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.515741 edc-pdutils-0.3.8/edc_pdutils/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    12259 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      549 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/migrations/0002_auto_20180921_2242.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.517768 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/
--rw-r--r--   0 erikvw     (501) staff       (20)      229 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      160 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9908 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/model_to_dataframe.py
--rw-r--r--   0 erikvw     (501) staff       (20)      326 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/subject_model_to_dataframe.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4981 2022-06-23 21:54:26.000000 edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/value_getter.py
--rw-r--r--   0 erikvw     (501) staff       (20)      160 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2997 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/site.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.518412 edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/
--rw-r--r--   0 erikvw     (501) staff       (20)       76 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      930 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      739 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/table_to_dataframe.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.519605 edc-pdutils-0.3.8/edc_pdutils/tables/
--rw-r--r--   0 erikvw     (501) staff       (20)      120 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/tables/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3195 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/aliquot.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1552 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2319 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/crf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2388 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/requisition.py
--rw-r--r--   0 erikvw     (501) staff       (20)      878 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/table.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tables/visit.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.521661 edc-pdutils-0.3.8/edc_pdutils/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.522871 edc-pdutils-0.3.8/edc_pdutils/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1866 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/tests/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     3337 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.523646 edc-pdutils-0.3.8/edc_pdutils/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2637 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_crf_tables_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1341 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_dialects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1646 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_non_crf_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1268 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_site_handlers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2296 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_table_exporter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2669 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/edc_pdutils/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.524692 edc-pdutils-0.3.8/edc_pdutils/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)      244 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/utils/datetime_to_date.py
--rw-r--r--   0 erikvw     (501) staff       (20)      638 2020-03-04 23:14:02.000000 edc-pdutils-0.3.8/edc_pdutils/utils/decrypt.py
--rw-r--r--   0 erikvw     (501) staff       (20)      717 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/utils/identity256.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1662 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/utils/missing_subject_identifiers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2021-03-01 03:55:57.000000 edc-pdutils-0.3.8/edc_pdutils/utils/undash.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-06 06:48:09.512535 edc-pdutils-0.3.8/edc_pdutils.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     3924 2022-07-06 06:48:09.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3172 2022-07-06 06:48:09.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-06 06:48:09.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:15:19.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-07-06 06:48:09.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       12 2022-07-06 06:48:09.000000 edc-pdutils-0.3.8/edc_pdutils.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1583 2022-06-23 21:54:26.000000 edc-pdutils-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1906 2022-07-06 06:47:52.000000 edc-pdutils-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1167 2022-07-06 06:48:09.525302 edc-pdutils-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.040902 edc-pdutils-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       94 2020-03-04 23:15:19.000000 edc-pdutils-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.023807 edc-pdutils-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.026865 edc-pdutils-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-19 02:12:43.000000 edc-pdutils-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1406 2022-06-23 21:54:26.000000 edc-pdutils-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-23 21:54:26.000000 edc-pdutils-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     3924 2022-08-19 15:02:51.041017 edc-pdutils-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3086 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-19 15:02:43.000000 edc-pdutils-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.029193 edc-pdutils-0.3.9/edc_pdutils/
+-rw-r--r--   0 erikvw     (501) staff       (20)      744 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2021-05-16 19:48:26.000000 edc-pdutils-0.3.9/edc_pdutils/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      141 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.030420 edc-pdutils-0.3.9/edc_pdutils/column_handlers/
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/column_handlers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      527 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/column_handlers/column_apply.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      685 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/column_handlers/column_map.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      203 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2971 2022-07-06 06:42:34.000000 edc-pdutils-0.3.9/edc_pdutils/database.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.031614 edc-pdutils-0.3.9/edc_pdutils/df_exporters/
+-rw-r--r--   0 erikvw     (501) staff       (20)      324 2020-10-06 17:42:55.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3219 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_crf_inline_tables_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1048 2020-10-06 17:42:55.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_crf_tables_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5488 2021-05-16 19:48:26.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      921 2021-05-16 18:35:37.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_model_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      791 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_noncrf_tables_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4319 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/df_exporters/tables_exporter.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.032433 edc-pdutils-0.3.9/edc_pdutils/df_handlers/
+-rw-r--r--   0 erikvw     (501) staff       (20)      123 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/df_handlers/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2901 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_handlers/crf_df_handler.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2005 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_handlers/df_handler.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      823 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_handlers/non_crf_df_handler.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2308 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/df_handlers/registered_subject_df_handler.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.033037 edc-pdutils-0.3.9/edc_pdutils/dialects/
+-rw-r--r--   0 erikvw     (501) staff       (20)      110 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/dialects/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3311 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/dialects/crf_dialect.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2637 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/dialects/mysql_dialect.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/dialects/rs_dialect.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1667 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       77 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/mappings.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.033454 edc-pdutils-0.3.9/edc_pdutils/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    12259 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      549 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/migrations/0002_auto_20180921_2242.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.035460 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/
+-rw-r--r--   0 erikvw     (501) staff       (20)      229 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      160 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9912 2022-08-19 15:02:43.000000 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/model_to_dataframe.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      326 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/subject_model_to_dataframe.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4981 2022-06-23 21:54:26.000000 edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/value_getter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      160 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2997 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/site.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.036047 edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/
+-rw-r--r--   0 erikvw     (501) staff       (20)       76 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      930 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      739 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/table_to_dataframe.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.037128 edc-pdutils-0.3.9/edc_pdutils/tables/
+-rw-r--r--   0 erikvw     (501) staff       (20)      120 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/tables/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3195 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/aliquot.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1552 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2319 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/crf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2388 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/requisition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      878 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/table.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tables/visit.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.037856 edc-pdutils-0.3.9/edc_pdutils/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.039237 edc-pdutils-0.3.9/edc_pdutils/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-07-15 04:03:23.000000 edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1866 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/tests/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     3337 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.039938 edc-pdutils-0.3.9/edc_pdutils/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2637 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_crf_tables_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1341 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_dialects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1646 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_non_crf_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1268 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_site_handlers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2296 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_table_exporter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2669 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/edc_pdutils/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.040782 edc-pdutils-0.3.9/edc_pdutils/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)      244 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/utils/datetime_to_date.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      638 2020-03-04 23:14:02.000000 edc-pdutils-0.3.9/edc_pdutils/utils/decrypt.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      717 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/utils/identity256.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1662 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/utils/missing_subject_identifiers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2021-03-01 03:55:57.000000 edc-pdutils-0.3.9/edc_pdutils/utils/undash.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-19 15:02:51.030049 edc-pdutils-0.3.9/edc_pdutils.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3924 2022-08-19 15:02:50.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3172 2022-08-19 15:02:51.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-19 15:02:50.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:15:19.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-19 15:02:50.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       12 2022-08-19 15:02:50.000000 edc-pdutils-0.3.9/edc_pdutils.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1583 2022-06-23 21:54:26.000000 edc-pdutils-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1906 2022-07-06 06:47:52.000000 edc-pdutils-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1167 2022-08-19 15:02:51.041339 edc-pdutils-0.3.9/setup.cfg
```

### Comparing `edc-pdutils-0.3.8/.github/workflows/build.yml` & `edc-pdutils-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/.gitignore` & `edc-pdutils-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/LICENSE` & `edc-pdutils-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/PKG-INFO` & `edc-pdutils-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pdutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Use pandas with clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pdutils
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc pandas,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-pdutils-0.3.8/README.rst` & `edc-pdutils-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/__init__.py` & `edc-pdutils-0.3.9/edc_pdutils/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/column_handlers/column_apply.py` & `edc-pdutils-0.3.9/edc_pdutils/column_handlers/column_apply.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/column_handlers/column_map.py` & `edc-pdutils-0.3.9/edc_pdutils/column_handlers/column_map.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/database.py` & `edc-pdutils-0.3.9/edc_pdutils/database.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_crf_inline_tables_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_crf_inline_tables_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_crf_tables_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_crf_tables_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_model_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_model_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/csv_noncrf_tables_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/csv_noncrf_tables_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_exporters/tables_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/df_exporters/tables_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_handlers/crf_df_handler.py` & `edc-pdutils-0.3.9/edc_pdutils/df_handlers/crf_df_handler.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_handlers/df_handler.py` & `edc-pdutils-0.3.9/edc_pdutils/df_handlers/df_handler.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_handlers/non_crf_df_handler.py` & `edc-pdutils-0.3.9/edc_pdutils/df_handlers/non_crf_df_handler.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/df_handlers/registered_subject_df_handler.py` & `edc-pdutils-0.3.9/edc_pdutils/df_handlers/registered_subject_df_handler.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/dialects/crf_dialect.py` & `edc-pdutils-0.3.9/edc_pdutils/dialects/crf_dialect.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/dialects/mysql_dialect.py` & `edc-pdutils-0.3.9/edc_pdutils/dialects/mysql_dialect.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/dialects/rs_dialect.py` & `edc-pdutils-0.3.9/edc_pdutils/dialects/rs_dialect.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/helper.py` & `edc-pdutils-0.3.9/edc_pdutils/helper.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/migrations/0001_initial.py` & `edc-pdutils-0.3.9/edc_pdutils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/migrations/0002_auto_20180921_2242.py` & `edc-pdutils-0.3.9/edc_pdutils/migrations/0002_auto_20180921_2242.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/model_to_dataframe.py` & `edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/model_to_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,19 @@
                         col for col in self.columns if col not in self.encrypted_columns
                     ]
                     queryset = self.queryset.values_list(*columns).filter(**self.query_filter)
                     self._dataframe = pd.DataFrame(list(queryset), columns=columns)
                 self.merge_dataframe_with_pivoted_m2ms()
                 self._dataframe.rename(columns=self.columns, inplace=True)
                 self._dataframe.fillna(value=np.nan, inplace=True)
-                for column in list(
-                    self._dataframe.select_dtypes(include=["datetime64[ns, UTC]"]).columns
-                ):
-                    # TODO: causes deprecation warning
-                    self._dataframe[column] = self._dataframe[column].astype("datetime64[ns]")
+                # TODO: causes deprecation warning (commented out)
+                # for column in list(
+                #     self._dataframe.select_dtypes(include=["datetime64[ns, UTC]"]).columns
+                # ):
+                #     self._dataframe[column] = self._dataframe[column].astype()
                 for column in list(self._dataframe.select_dtypes(include=["O"]).columns):
                     self._dataframe[column] = self._dataframe[column].astype(str)
                 if self.drop_sys_columns:
                     self._dataframe = self._dataframe.drop(self.edc_sys_columns, axis=1)
         return self._dataframe
 
     def merge_dataframe_with_pivoted_m2ms(self):
```

### Comparing `edc-pdutils-0.3.8/edc_pdutils/model_to_dataframe/value_getter.py` & `edc-pdutils-0.3.9/edc_pdutils/model_to_dataframe/value_getter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/site.py` & `edc-pdutils-0.3.9/edc_pdutils/site.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/helper.py` & `edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/helper.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/table_to_dataframe/table_to_dataframe.py` & `edc-pdutils-0.3.9/edc_pdutils/table_to_dataframe/table_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/aliquot.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/aliquot.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/consent.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/consent.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/crf.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/crf.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/requisition.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/requisition.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/table.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/table.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tables/visit.py` & `edc-pdutils-0.3.9/edc_pdutils/tables/visit.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-local-private.pem` & `edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/etc/user-rsa-restricted-private.pem` & `edc-pdutils-0.3.9/edc_pdutils/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/helper.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/helper.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/models.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_crf_tables_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_crf_tables_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_dialects.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_dialects.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_non_crf_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_non_crf_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_site_handlers.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_site_handlers.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/tests/test_table_exporter.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/tests/test_table_exporter.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/tests/visit_schedule.py` & `edc-pdutils-0.3.9/edc_pdutils/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/utils/decrypt.py` & `edc-pdutils-0.3.9/edc_pdutils/utils/decrypt.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/utils/identity256.py` & `edc-pdutils-0.3.9/edc_pdutils/utils/identity256.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils/utils/missing_subject_identifiers.py` & `edc-pdutils-0.3.9/edc_pdutils/utils/missing_subject_identifiers.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/edc_pdutils.egg-info/PKG-INFO` & `edc-pdutils-0.3.9/edc_pdutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pdutils
-Version: 0.3.8
+Version: 0.3.9
 Summary: Use pandas with clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-pdutils
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc pandas,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-pdutils-0.3.8/edc_pdutils.egg-info/SOURCES.txt` & `edc-pdutils-0.3.9/edc_pdutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/pyproject.toml` & `edc-pdutils-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/runtests.py` & `edc-pdutils-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-pdutils-0.3.8/setup.cfg` & `edc-pdutils-0.3.9/setup.cfg`

 * *Files identical despite different names*

