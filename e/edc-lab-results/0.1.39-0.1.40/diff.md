# Comparing `tmp/edc-lab-results-0.1.39.tar.gz` & `tmp/edc-lab-results-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-lab-results-0.1.39.tar", last modified: Tue Aug  1 04:34:50 2023, max compression
+gzip compressed data, was "edc-lab-results-0.1.40.tar", last modified: Sun Aug  6 20:57:15 2023, max compression
```

## Comparing `edc-lab-results-0.1.39.tar` & `edc-lab-results-0.1.40.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.491017 edc-lab-results-0.1.39/
--rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.477632 edc-lab-results-0.1.39/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.481223 edc-lab-results-0.1.39/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 19:25:16.000000 edc-lab-results-0.1.39/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-25 20:27:10.000000 edc-lab-results-0.1.39/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-08-01 04:34:50.491112 edc-lab-results-0.1.39/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      733 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-09 19:25:16.000000 edc-lab-results-0.1.39/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.482847 edc-lab-results-0.1.39/edc_lab_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3809 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.484120 edc-lab-results-0.1.39/edc_lab_results/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-10-26 16:30:10.000000 edc-lab-results-0.1.39/edc_lab_results/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-10-26 16:30:10.000000 edc-lab-results-0.1.39/edc_lab_results/admin/blood_results_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1867 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1002 2022-07-27 02:24:23.000000 edc-lab-results-0.1.39/edc_lab_results/calculate_missing.py
--rw-r--r--   0 erikvw     (501) staff       (20)      504 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3813 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/fieldsets.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.485011 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      251 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      836 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3990 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.487670 edc-lab-results-0.1.39/edc_lab_results/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)     1189 2022-08-15 00:51:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4343 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/blood_result_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/electrolytes_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4420 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbc_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1749 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbg_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1748 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/glucose_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/hba1c_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/insulin_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3107 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/lft_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1723 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/lipid_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      426 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/proteinuria_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-08-15 00:51:30.000000 edc-lab-results-0.1.39/edc_lab_results/model_mixins/rft_model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.489058 edc-lab-results-0.1.39/edc_lab_results/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.490395 edc-lab-results-0.1.39/edc_lab_results/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1367 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      683 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2039 2023-04-20 21:10:15.000000 edc-lab-results-0.1.39/edc_lab_results/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2708 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.490891 edc-lab-results-0.1.39/edc_lab_results/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4466 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_blood_result.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7389 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-07 00:31:57.000000 edc-lab-results-0.1.39/edc_lab_results/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2104 2022-09-30 01:31:16.000000 edc-lab-results-0.1.39/edc_lab_results/tests/visit_schedule.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-01 04:34:50.483584 edc-lab-results-0.1.39/edc_lab_results.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1644 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2465 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 00:14:15.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-08-01 04:34:50.000000 edc-lab-results-0.1.39/edc_lab_results.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1776 2023-05-24 17:18:30.000000 edc-lab-results-0.1.39/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2217 2023-08-01 04:34:43.000000 edc-lab-results-0.1.39/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1210 2023-08-01 04:34:50.491441 edc-lab-results-0.1.39/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.997637 edc-lab-results-0.1.40/
+-rw-r--r--   0 erikvw     (501) staff       (20)       76 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.984400 edc-lab-results-0.1.40/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.988566 edc-lab-results-0.1.40/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1927 2023-08-06 20:57:08.000000 edc-lab-results-0.1.40/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 17:18:30.000000 edc-lab-results-0.1.40/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-09 19:25:16.000000 edc-lab-results-0.1.40/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-25 20:27:10.000000 edc-lab-results-0.1.40/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     6946 2023-08-06 20:57:15.997729 edc-lab-results-0.1.40/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     6086 2023-08-06 20:57:08.000000 edc-lab-results-0.1.40/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-09 19:25:16.000000 edc-lab-results-0.1.40/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.990035 edc-lab-results-0.1.40/edc_lab_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3809 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.991402 edc-lab-results-0.1.40/edc_lab_results/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2022-10-26 16:30:10.000000 edc-lab-results-0.1.40/edc_lab_results/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-10-26 16:30:10.000000 edc-lab-results-0.1.40/edc_lab_results/admin/blood_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/admin/reportable_results_modeladmin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1002 2022-07-27 02:24:23.000000 edc-lab-results-0.1.40/edc_lab_results/calculate_missing.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      504 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3813 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/fieldsets.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.992308 edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      251 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      836 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3990 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      437 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/blood_results_glu_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.994518 edc-lab-results-0.1.40/edc_lab_results/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1189 2022-08-15 00:51:30.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4343 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/blood_result_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      955 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/electrolytes_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4420 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/fbc_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1749 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/fbg_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/glucose_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/hba1c_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1140 2023-05-24 17:18:30.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/insulin_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3107 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/lft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1723 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/lipid_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      426 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/proteinuria_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2022-08-15 00:51:30.000000 edc-lab-results-0.1.40/edc_lab_results/model_mixins/rft_model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.995840 edc-lab-results-0.1.40/edc_lab_results/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.997007 edc-lab-results-0.1.40/edc_lab_results/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1367 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      683 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2039 2023-04-20 21:10:15.000000 edc-lab-results-0.1.40/edc_lab_results/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2708 2023-08-01 04:34:43.000000 edc-lab-results-0.1.40/edc_lab_results/tests/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.997415 edc-lab-results-0.1.40/edc_lab_results/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4466 2023-08-01 04:34:43.000000 edc-lab-results-0.1.40/edc_lab_results/tests/tests/test_blood_result.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7389 2023-08-01 04:34:43.000000 edc-lab-results-0.1.40/edc_lab_results/tests/tests/test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      261 2022-05-07 00:31:57.000000 edc-lab-results-0.1.40/edc_lab_results/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2104 2022-09-30 01:31:16.000000 edc-lab-results-0.1.40/edc_lab_results/tests/visit_schedule.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-08-06 20:57:15.990787 edc-lab-results-0.1.40/edc_lab_results.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     6946 2023-08-06 20:57:15.000000 edc-lab-results-0.1.40/edc_lab_results.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2465 2023-08-06 20:57:15.000000 edc-lab-results-0.1.40/edc_lab_results.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-08-06 20:57:15.000000 edc-lab-results-0.1.40/edc_lab_results.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 00:14:15.000000 edc-lab-results-0.1.40/edc_lab_results.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       16 2023-08-06 20:57:15.000000 edc-lab-results-0.1.40/edc_lab_results.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1737 2023-08-06 20:57:08.000000 edc-lab-results-0.1.40/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2217 2023-08-01 04:34:43.000000 edc-lab-results-0.1.40/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1170 2023-08-06 20:57:15.998029 edc-lab-results-0.1.40/setup.cfg
```

### Comparing `edc-lab-results-0.1.39/.github/workflows/build.yml` & `edc-lab-results-0.1.40/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,16 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.11']
         django-version: ['4.1', '4.2', 'dev']
-        exclude:
-          - python-version: '3.10'
-            django-version: 'dev'
     services:
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
```

### Comparing `edc-lab-results-0.1.39/.gitignore` & `edc-lab-results-0.1.40/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/.pre-commit-config.yaml` & `edc-lab-results-0.1.40/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/LICENSE` & `edc-lab-results-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/action_items.py` & `edc-lab-results-0.1.40/edc_lab_results/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/admin/reportable_results_modeladmin_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/admin/reportable_results_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/calculate_missing.py` & `edc-lab-results-0.1.40/edc_lab_results/calculate_missing.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/fieldsets.py` & `edc-lab-results-0.1.40/edc_lab_results/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/blood_results_fbg_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/form_validator_mixins/blood_results_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/__init__.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/blood_result_model_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/blood_result_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/electrolytes_model_mixins.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/electrolytes_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbc_model_mixins.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/fbc_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/fbg_model_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/fbg_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/glucose_model_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/glucose_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/hba1c_model_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/hba1c_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/insulin_model_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/insulin_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/lft_model_mixins.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/lft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/lipid_model_mixins.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/lipid_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/model_mixins/rft_model_mixins.py` & `edc-lab-results-0.1.40/edc_lab_results/model_mixins/rft_model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-local-private.pem` & `edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/etc/user-rsa-restricted-private.pem` & `edc-lab-results-0.1.40/edc_lab_results/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/forms.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/lab_profiles.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/models.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/test_case_mixin.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_blood_result.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/tests/test_blood_result.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/tests/test_form.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results/tests/visit_schedule.py` & `edc-lab-results-0.1.40/edc_lab_results/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/edc_lab_results.egg-info/SOURCES.txt` & `edc-lab-results-0.1.40/edc_lab_results.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/pyproject.toml` & `edc-lab-results-0.1.40/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -32,23 +32,21 @@
   "if TYPE_CHECKING:",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310}-dj{41,42},
     py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.10: py310
     3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
     4.1: dj41
     4.2: dj42, lint
     dev: djdev
```

### Comparing `edc-lab-results-0.1.39/runtests.py` & `edc-lab-results-0.1.40/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-lab-results-0.1.39/setup.cfg` & `edc-lab-results-0.1.40/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.10
+python_requires = >=3.11
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	examples*
```

