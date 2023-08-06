# Comparing `tmp/lamindb_setup-0.49.4.tar.gz` & `tmp/lamindb_setup-0.49.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.49.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.49.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.49.4.tar` & `lamindb_setup-0.49.5.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.4/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.4/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.4/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.4/README.md
--rw-r--r--   0        0        0    59511 2023-08-04 10:39:57.261622 lamindb_setup-0.49.4/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.4/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.4/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.4/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.4/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.4/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.4/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.4/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.4/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.4/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.4/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.4/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.4/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.4/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.4/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.49.4/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.4/lamin-project.yaml
--rw-r--r--   0        0        0     2758 2023-08-04 10:39:34.709811 lamindb_setup-0.49.4/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5704 2023-07-31 17:31:23.899228 lamindb_setup-0.49.4/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.49.4/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.49.4/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.49.4/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.4/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.4/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.49.4/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6602 2023-07-25 01:43:24.440143 lamindb_setup-0.49.4/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1413 2023-07-24 10:02:47.316262 lamindb_setup-0.49.4/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.49.4/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.49.4/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.4/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.49.4/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.4/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.4/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.4/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.49.4/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.4/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.4/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.49.4/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.4/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.49.4/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.4/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.4/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0    11249 2023-08-02 03:33:18.382713 lamindb_setup-0.49.4/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.4/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.4/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.49.4/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.4/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.4/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-07-18 04:17:11.571437 lamindb_setup-0.49.4/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.4/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.4/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.49.4/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4862 2023-08-03 12:06:57.634858 lamindb_setup-0.49.4/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2734 2023-07-31 17:31:23.900624 lamindb_setup-0.49.4/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.4/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.4/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.4/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.4/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.4/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    33450 2023-07-25 01:43:38.325656 lamindb_setup-0.49.4/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.4/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.4/lnschema-core/README.md
--rw-r--r--   0        0        0      447 2023-07-25 01:43:38.325792 lamindb_setup-0.49.4/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.4/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
--rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
--rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
--rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
--rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
--rw-r--r--   0        0        0     3585 2023-07-25 01:43:38.326104 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.4/lnschema-core/lnschema_core/mocks.py
--rw-r--r--   0        0        0    64949 2023-07-31 11:23:10.578935 lamindb_setup-0.49.4/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.4/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.4/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.4/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.4/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.4/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.4/noxfile.py
--rw-r--r--   0        0        0     1169 2023-08-04 10:32:33.588209 lamindb_setup-0.49.4/pyproject.toml
--rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.4/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.4/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.4/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.4/tests/test_bionty.py
--rw-r--r--   0        0        0     4936 2023-08-03 09:23:05.337238 lamindb_setup-0.49.4/tests/test_init_instance.py
--rw-r--r--   0        0        0     2207 2023-07-25 01:43:24.442039 lamindb_setup-0.49.4/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.4/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-24 10:02:47.316450 lamindb_setup-0.49.4/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.4/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.4/tests/test_signup.py
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 lamindb_setup-0.49.4/PKG-INFO
+-rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.5/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.5/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.5/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.5/README.md
+-rw-r--r--   0        0        0    59839 2023-08-06 21:15:15.938006 lamindb_setup-0.49.5/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.5/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.5/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.5/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.5/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.5/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.5/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.5/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.5/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.5/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.5/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.5/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.5/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.5/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.5/docs/reference.md
+-rw-r--r--   0        0        0      364 2023-08-06 21:14:34.989760 lamindb_setup-0.49.5/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.5/lamin-project.yaml
+-rw-r--r--   0        0        0     2758 2023-08-06 21:14:50.504187 lamindb_setup-0.49.5/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5704 2023-07-31 17:31:23.899228 lamindb_setup-0.49.5/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2072 2023-08-06 21:14:34.990057 lamindb_setup-0.49.5/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      849 2023-08-06 21:14:34.990237 lamindb_setup-0.49.5/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2014 2023-08-06 21:14:34.990409 lamindb_setup-0.49.5/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.5/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.5/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7475 2023-08-06 21:14:34.990684 lamindb_setup-0.49.5/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6601 2023-08-06 21:14:34.990879 lamindb_setup-0.49.5/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1417 2023-08-06 21:14:34.991033 lamindb_setup-0.49.5/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1685 2023-08-06 21:14:34.991186 lamindb_setup-0.49.5/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      782 2023-08-06 21:14:34.991331 lamindb_setup-0.49.5/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.5/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2188 2023-08-06 21:14:34.991491 lamindb_setup-0.49.5/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.5/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.5/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.5/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3497 2023-08-06 21:14:34.991664 lamindb_setup-0.49.5/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.5/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.5/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5998 2023-08-06 21:14:34.991847 lamindb_setup-0.49.5/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.5/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10928 2023-08-06 21:14:34.992038 lamindb_setup-0.49.5/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.5/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0    11248 2023-08-06 21:14:34.992292 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9340 2023-08-06 21:14:34.992512 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2317 2023-08-06 21:14:34.992697 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.5/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2174 2023-08-06 21:14:34.992898 lamindb_setup-0.49.5/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4867 2023-08-05 09:44:28.020872 lamindb_setup-0.49.5/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2734 2023-07-31 17:31:23.900624 lamindb_setup-0.49.5/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.5/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.5/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.5/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    36103 2023-08-06 12:24:47.608810 lamindb_setup-0.49.5/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.5/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.5/lnschema-core/README.md
+-rw-r--r--   0        0        0      508 2023-08-06 12:24:47.608958 lamindb_setup-0.49.5/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.5/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
+-rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
+-rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
+-rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
+-rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
+-rw-r--r--   0        0        0     6285 2023-08-06 12:24:47.609237 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
+-rw-r--r--   0        0        0     2985 2023-08-06 12:24:47.609326 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py
+-rw-r--r--   0        0        0      393 2023-08-06 12:24:47.609390 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0014_rename_ref_field_featureset_registry.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.5/lnschema-core/lnschema_core/mocks.py
+-rw-r--r--   0        0        0    71611 2023-08-06 12:24:47.609755 lamindb_setup-0.49.5/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.5/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.5/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.5/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.5/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.5/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.5/noxfile.py
+-rw-r--r--   0        0        0     1168 2023-08-06 21:14:34.993101 lamindb_setup-0.49.5/pyproject.toml
+-rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.5/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.5/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.5/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.5/tests/test_bionty.py
+-rw-r--r--   0        0        0     4936 2023-08-03 09:23:05.337238 lamindb_setup-0.49.5/tests/test_init_instance.py
+-rw-r--r--   0        0        0     2207 2023-07-25 01:43:24.442039 lamindb_setup-0.49.5/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.5/tests/test_login.py
+-rw-r--r--   0        0        0      457 2023-07-24 10:02:47.316450 lamindb_setup-0.49.5/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.5/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.5/tests/test_signup.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 lamindb_setup-0.49.5/PKG-INFO
```

### Comparing `lamindb_setup-0.49.4/.github/workflows/build.yml` & `lamindb_setup-0.49.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/.gitignore` & `lamindb_setup-0.49.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/.pre-commit-config.yaml` & `lamindb_setup-0.49.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/LICENSE` & `lamindb_setup-0.49.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/changelog.md` & `lamindb_setup-0.49.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Replace `lamin_logger` with `lamin_utils` | [454](https://github.com/laminlabs/lamindb-setup/pull/454) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 | 0.49.5
+🚚 Rename `ORM` to `Registry` | [453](https://github.com/laminlabs/lamindb-setup/pull/453) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-05 |
 ⬇️ Upper bound external dependencies | [452](https://github.com/laminlabs/lamindb-setup/pull/452) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.49.4
 🎨 Add `.record` property to `StorageSettings` | [451](https://github.com/laminlabs/lamindb-setup/pull/451) | [falexwolf](https://github.com/falexwolf) | 2023-08-03 | 0.49.3
 ✅ Fix init-instance test for sqlite instance | [450](https://github.com/laminlabs/lamindb-setup/pull/450) | [bpenteado](https://github.com/bpenteado) | 2023-08-02 |
 🎨 Fix `init-instance` anti-patterns and expand tests | [449](https://github.com/laminlabs/lamindb-setup/pull/449) | [bpenteado](https://github.com/bpenteado) | 2023-08-01 |
 ✨ Propagate kwargs through synchronization functions | [448](https://github.com/laminlabs/lamindb-setup/pull/448) | [Koncopd](https://github.com/Koncopd) | 2023-07-31 | 0.49.2
 🐛 Fix local variable 'db_dsn' referenced before assignment | [447](https://github.com/laminlabs/lamindb-setup/pull/447) | [fredericenard](https://github.com/fredericenard) | 2023-07-30 |
 🚸 Show help by default and add --version | [446](https://github.com/laminlabs/lamindb-setup/pull/446) | [Zethson](https://github.com/Zethson) | 2023-07-30 |
```

### Comparing `lamindb_setup-0.49.4/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.49.5/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/faq/multi-session.ipynb` & `lamindb_setup-0.49.5/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.49.5/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.49.5/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.49.5/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.49.5/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.49.5/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.49.5/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/docs/guide/setup-user.md` & `lamindb_setup-0.49.5/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/__init__.py` & `lamindb_setup-0.49.5/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.49.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.49.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/__main__.py` & `lamindb_setup-0.49.5/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.49.5/lamindb_setup/_check_instance_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._init_instance import reload_schema_modules
 from ._silence_loggers import silence_loggers
 from .dev._settings_store import current_instance_settings_file
 
 _INSTANCE_NOT_SETUP_WARNING = """\
 You haven't yet setup an instance: Please call `ln.setup.init()` or `ln.setup.load()`
@@ -30,15 +30,15 @@
                 if not IS_SETUP:
                     setup_django(isettings)
                     reload_schema_modules(isettings)
                     # only now we can import lamindb
                     import lamindb as ln
 
                     logger.success(
-                        f"Loaded instance: {isettings.identifier} (lamindb"
+                        f"loaded instance: {isettings.identifier} (lamindb"
                         f" {ln.__version__})"
                     )
                 return True
             else:
                 return IS_SETUP
         except Exception:
             # user will get more detailed traceback once they run the CLI
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_close.py` & `lamindb_setup-0.49.5/lamindb_setup/_close.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings import settings
 from .dev._settings_store import current_instance_settings_file
 from .dev._setup_bionty_sources import delete_bionty_sources_yaml
 
 
 def close(mute: bool = False) -> None:
@@ -11,14 +11,15 @@
     Returns `None` if succeeds, otherwise an exception is raised.
     """
     if current_instance_settings_file().exists():
         instance = settings.instance.identifier
         try:
             settings.instance._update_cloud_sqlite_file()
         except FileNotFoundError:
-            logger.warning("Did not find local cache file")
+            logger.warning("did not find local cache file")
         current_instance_settings_file().unlink()
         delete_bionty_sources_yaml()
-        logger.success(f"Closed instance: {instance}")
+        if not mute:
+            logger.success(f"closed instance: {instance}")
     else:
         if not mute:
-            logger.info("No instance loaded")
+            logger.info("no instance loaded")
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_delete.py` & `lamindb_setup-0.49.5/lamindb_setup/_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import shutil
 from pathlib import Path
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._close import close
 from ._settings import settings
 from .dev._settings_load import load_instance_settings
 from .dev._settings_store import instance_settings_file
 
 
 def delete(instance_name: str):
     """Delete an instance."""
     instance_identifier = f"{settings.user.handle}/{instance_name}"
-    logger.info(f"Deleting instance {instance_identifier}")
+    logger.info(f"deleting instance {instance_identifier}")
     settings_file = instance_settings_file(instance_name, settings.user.handle)
     if not settings_file.exists():
         logger.warning(
             "Could not delete as instance settings do not exist locally. Did you"
             " provide a wrong instance name? Could you try loading it?"
         )
         return None
     isettings = load_instance_settings(settings_file)
 
     delete_settings(settings_file)
     if settings._instance_exists:
         if instance_identifier == settings.instance.identifier:
-            close()  # close() does further operations, unlocking...
+            close(mute=True)  # close() does further operations, unlocking...
             settings._instance_settings = None
     delete_cache(isettings.storage.cache_dir)
     if isettings.dialect == "sqlite":
         if isettings._sqlite_file.exists():
             isettings._sqlite_file.unlink()
             logger.info("    deleted '.lndb' sqlite file")
         else:
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_docstrings.py` & `lamindb_setup-0.49.5/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_init_instance.py` & `lamindb_setup-0.49.5/lamindb_setup/_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import sys
 from pathlib import Path
 from typing import Optional, Union
 
-from lamin_logger import logger
+from lamin_utils import logger
 from pydantic import PostgresDsn
 
 from lamindb_setup.dev.upath import UPath
 
 from ._close import close as close_instance
 from ._docstrings import instance_description as description
 from ._settings import settings
@@ -27,15 +27,15 @@
             root=ssettings.root_as_str,
             type=ssettings.type,
             region=ssettings.region,
             created_by_id=settings.user.id,
         ),
     )
     if created:
-        logger.success(f"Saved: {storage}")
+        logger.success(f"saved: {storage}")
 
 
 def register_user_and_storage(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
     from lnschema_core.models import User
 
@@ -45,15 +45,15 @@
             defaults=dict(
                 handle=usettings.handle,
                 name=usettings.name,
                 email=usettings.email,
             ),
         )
         if created:
-            logger.success(f"Saved: {user}")
+            logger.success(f"saved: {user}")
         register_storage(isettings.storage)
     except OperationalError as error:
         logger.warning(f"Instance seems not set up ({error})")
 
 
 def reload_schema_modules(isettings: InstanceSettings):
     schema_names = ["core"] + list(isettings.schema)
@@ -71,15 +71,15 @@
     if "lamindb" in sys.modules:
         import lamindb
 
         importlib.reload(lamindb)
     else:
         # only log if we're outside lamindb
         # lamindb itself logs upon import!
-        logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
+        logger.success(f"loaded instance: {isettings.owner}/{isettings.name}")
 
 
 ERROR_SQLITE_CACHE = """
 Your cached local SQLite file exists, while your cloud SQLite file ({}) doesn't.
 Either delete your cache ({}) or add it back to the cloud (if delete was accidental).
 """
 
@@ -168,43 +168,43 @@
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Registering instance on hub failed:\n{result}")
         logger.success(
-            f"Registered instance on hub: https://lamin.ai/{owner}/{name_str}"
+            f"registered instance on hub: https://lamin.ai/{owner}/{name_str}"
         )
 
     if _test:
         isettings._persist()
         return None
 
     silence_loggers()
 
     also_init_bionty = True
     if isettings._is_db_setup(mute=True)[0]:
         logger.warning(
-            "Your instance DB already has content, but we couldn't find settings,"
+            "your instance DB already has content, but couldn't find settings,"
             " proceeding with setup"
         )
         # do not write the bionty tables again
         also_init_bionty = False
     load_from_isettings(isettings, init=True, also_init_bionty=also_init_bionty)
     if isettings._is_cloud_sqlite:
         isettings._cloud_sqlite_locker.lock()
         logger.warning(
-            "Locked the instance. To unlock and push changes to the cloud SQLite file,"
-            " call: lamin close"
+            "locked instance (to unlock and push changes to the cloud SQLite file,"
+            " call: lamin close)"
         )
     if not isettings.is_remote:
         verbosity = logger._verbosity
-        logger.set_verbosity(3)
+        logger.set_verbosity(4)
         logger.hint(
-            "Did not register local instance on hub (if you want to, call `lamin"
+            "did not register local instance on hub (if you want, call `lamin"
             " register`)"
         )
         logger.set_verbosity(verbosity)
     return None
 
 
 def load_from_isettings(
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_load_instance.py` & `lamindb_setup-0.49.5/lamindb_setup/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Optional, Union
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from lamindb_setup.dev.upath import UPath
 
 from ._close import close as close_instance
 from ._init_instance import load_from_isettings
 from ._settings import InstanceSettings, settings
 from ._silence_loggers import silence_loggers
@@ -65,15 +65,15 @@
             storage_region=storage_result["region"],
             db=instance_result["db"],
             schema=instance_result["schema_str"],
         )
     else:
         settings_file = instance_settings_file(name, owner)
         if settings_file.exists():
-            logger.info(f"Found cached instance metadata: {settings_file}")
+            logger.info(f"found cached instance metadata: {settings_file}")
             isettings = load_instance_settings(settings_file)
         else:
             if _log_error_message:
                 raise RuntimeError(
                     f"Instance {owner}/{name} neither loadable from hub nor local"
                     " cache. Check whether instance exists and you have access:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_migrate.py` & `lamindb_setup-0.49.5/lamindb_setup/_migrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._check_instance_setup import check_instance_setup
 from ._settings import settings
 from .dev._django import setup_django
 
 
 class migrate:
@@ -29,15 +29,15 @@
         """Deploy a migration."""
         if check_instance_setup():
             raise RuntimeError("Restart Python session to migrate or use CLI!")
         setup_django(settings.instance, deploy_migrations=True)
 
     @classmethod
     def check(cls) -> bool:
-        """Check whether ORM definitions are in sync with migrations."""
+        """Check whether Registry definitions are in sync with migrations."""
         from django.core.management import call_command
 
         setup_django(settings.instance)
         try:
             call_command("makemigrations", check_changes=True)
         except SystemExit:
             logger.error(
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_notebook.py` & `lamindb_setup-0.49.5/lamindb_setup/_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 
 def track(notebook_path: str, pypackage: Optional[str] = None):
     try:
         from nbproject.dev import initialize_metadata, read_notebook, write_notebook
         from nbproject.dev._initialize import nbproject_id
     except ImportError:
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_register_instance.py` & `lamindb_setup-0.49.5/lamindb_setup/_register_instance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings import settings
 
 
 def register():
     """Register an instance on the hub."""
     from .dev._hub_core import init_instance as init_instance_hub
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_schema.py` & `lamindb_setup-0.49.5/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_set.py` & `lamindb_setup-0.49.5/lamindb_setup/_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Union
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from lamindb_setup.dev.upath import UPath
 
 from ._init_instance import register_user_and_storage
 from ._settings import settings
 from .dev import deprecated
 from .dev._settings_instance import InstanceSettings
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_settings.py` & `lamindb_setup-0.49.5/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_setup_user.py` & `lamindb_setup-0.49.5/lamindb_setup/_setup_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Union
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings import settings
 from .dev._settings_load import load_or_create_user_settings, load_user_settings
 from .dev._settings_save import save_user_settings
 from .dev._settings_store import user_settings_file_email, user_settings_file_handle
 
 
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
     from .dev._hub_core import sign_up_hub
 
     response = sign_up_hub(email)
     if response == "handle-exists":  # handle already exists
-        logger.error("The handle already exists. Please choose a different one.")
+        logger.error("The handle already exists: please choose a different one")
         return "handle-exists"
     if response == "user-exists":  # user already exists
-        logger.error("User already exists! Please login instead: `lamin login`.")
+        logger.error("User already exists! Please login instead: `lamin login`")
         return "user-exists"
     user_settings = load_or_create_user_settings()
     user_settings.email = email
     save_user_settings(user_settings)
     user_settings.password = response
     save_user_settings(user_settings)
     return None  # user needs to confirm email now
@@ -88,17 +88,17 @@
     if response == "could-not-login":
         return response
     elif response == "complete-signup":
         return response
     else:
         user_id, user_handle, user_name, access_token = response
     if handle is None:
-        logger.success(f"Logged in with handle {user_handle} and id {user_id}")
+        logger.success(f"logged in with handle {user_handle} and id {user_id}")
     else:
-        logger.success(f"Logged in with email {user_settings.email} and id {user_id}")
+        logger.success(f"logged in with email {user_settings.email} and id {user_id}")
     user_settings.id = user_id
     user_settings.handle = user_handle
     user_settings.name = user_name
     user_settings.access_token = access_token
     save_user_settings(user_settings)
 
     settings._user_settings = None
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.49.5/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Optional, Union
 
 import fsspec
 from dateutil.parser import isoparse  # type: ignore
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings_instance import InstanceSettings
 from .upath import UPath, infer_filesystem
 
 EXPIRATION_TIME = 7 * 24 * 60 * 60  # 1 week
 
 MAX_MSG_COUNTER = 100  # print the msg after this number of iterations
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_django.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_django.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 import builtins
 import os
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings_instance import InstanceSettings
 
 IS_RUN_FROM_IPYTHON = getattr(builtins, "__IPYTHON__", False)
 IS_SETUP = False
 
 
@@ -108,15 +108,15 @@
     # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
             except Exception as e:
                 logger.warning(f"Failed to execute: {stmt} because of {e}")
-    logger.success("Created legacy migration preparations")
+    logger.success("created legacy migration preparations")
     return True
 
 
 def insert_legacy_data(isettings: InstanceSettings):
     import sqlalchemy as sa
 
     engine = sa.create_engine(isettings.db)
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import Optional, Tuple, Union
 from uuid import UUID, uuid4
 
-from lamin_logger import logger
+from lamin_utils import logger
 from postgrest.exceptions import APIError
 
 from ._hub_client import connect_hub, connect_hub_with_auth, get_lamin_site_base_url
 from ._hub_crud import (
     sb_insert_collaborator,
     sb_insert_db_user,
     sb_insert_instance,
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Literal, Optional, Set, Tuple, Union
 
-from lamin_logger import logger
+from lamin_utils import logger
 
 from ._settings_save import save_instance_settings
 from ._settings_store import current_instance_settings_file, instance_settings_file
 from ._storage import StorageSettings
 from .upath import UPath
 
 # leave commented out until we understand more how to deal with
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import shutil
 from pathlib import Path
 
-from lamin_logger import logger
+from lamin_utils import logger
 from pydantic import BaseSettings
 
 
 def get_settings_dir():
     settings_dir = Path.home() / ".lamin"
     settings_dir.mkdir(parents=True, exist_ok=True)
     # deal with legacy settings directory
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_setup_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 from types import ModuleType
 
 from importlib_metadata import requires as importlib_requires
 from importlib_metadata import version as get_pip_version
-from lamin_logger import logger
+from lamin_utils import logger
 from packaging.requirements import Requirement
 
 from ._django import setup_django
 from ._settings_instance import InstanceSettings
 
 
 def get_schema_module_name(schema_name):
@@ -55,9 +55,9 @@
 
     schema_names = ["core"] + list(isettings.schema)
     msg = ""
     for schema_name in schema_names:
         module = check_schema_version_and_import(schema_name)
         msg += f"{schema_name}=={module.__version__} "
     if init:
-        logger.info(f"Creating schemas: {msg}")
+        logger.info(f"creating schemas: {msg}")
     return msg, schema_names
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             root_path = root.resolve()
         elif isinstance(root, str):
             root_path = Storage._str_to_path(root)
         else:
             raise ValueError("root should be of type Union[str, Path, UPath].")
         self._root = root_path
         self._region = region
-        # would prefer to type below as ORM, but need to think through import order
+        # would prefer to type below as Registry, but need to think through import order
         self._record: Optional[Any] = None
 
     @staticmethod
     def _str_to_path(storage: str) -> Union[Path, UPath]:
         if storage.startswith("s3://"):
             # for new buckets there could be problems if the region is not specified
             storage_root = UPath(storage, cache_regions=True)
```

### Comparing `lamindb_setup-0.49.4/lamindb_setup/dev/upath.py` & `lamindb_setup-0.49.5/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.49.5/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/.gitignore` & `lamindb_setup-0.49.5/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.49.5/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.49.5/lnschema-core/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🚚 Remove reference ORM from Label and add it to Feature, add slot to FeatureSet link models | [238](https://github.com/laminlabs/lnschema-core/pull/238) | [falexwolf](https://github.com/falexwolf) | 2023-07-24 |
+🚚 Rename `ref_field` to `registry` | [256](https://github.com/laminlabs/lnschema-core/pull/256) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 |
+♻️ Add `Data` base class for `File` & `Dataset` | [255](https://github.com/laminlabs/lnschema-core/pull/255) | [falexwolf](https://github.com/falexwolf) | 2023-08-05 |
+🚚 Rename ORM to Registry | [254](https://github.com/laminlabs/lnschema-core/pull/254) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-05 |
+🚚 Type Link ORMs with `LinkORM` | [253](https://github.com/laminlabs/lnschema-core/pull/253) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.43.3
+🚚 Rename select to filter | [252](https://github.com/laminlabs/lnschema-core/pull/252) | [falexwolf](https://github.com/falexwolf) | 2023-07-31 | 0.43.0
+🚚 Rename `Feature.label_orms` to `Feature.registries` | [251](https://github.com/laminlabs/lnschema-core/pull/251) | [falexwolf](https://github.com/falexwolf) | 2023-07-31 |
+♻️ Aggregate ref_field, ref_orm, ref_schema into ref_field | [250](https://github.com/laminlabs/lnschema-core/pull/250) | [falexwolf](https://github.com/falexwolf) | 2023-07-31 |
+🚚 Move feature foreign key from Label to link model | [249](https://github.com/laminlabs/lnschema-core/pull/249) | [falexwolf](https://github.com/falexwolf) | 2023-07-31 |
+🚚 Allow multiple label ORMs in feature | [247](https://github.com/laminlabs/lnschema-core/pull/247) | [falexwolf](https://github.com/falexwolf) | 2023-07-29 |
+🚑️ Hash can be null | [246](https://github.com/laminlabs/lnschema-core/pull/246) | [falexwolf](https://github.com/falexwolf) | 2023-07-26 |
+📝 Add signatures to remaining ORMs | [245](https://github.com/laminlabs/lnschema-core/pull/245) | [falexwolf](https://github.com/falexwolf) | 2023-07-26 | 0.42.1
+🚚 Add field `hash` to `FeatureSet` | [244](https://github.com/laminlabs/lnschema-core/pull/244) | [falexwolf](https://github.com/falexwolf) | 2023-07-26 |
+🚸 Type-annotate `FeatureManager` | [243](https://github.com/laminlabs/lnschema-core/pull/243) | [falexwolf](https://github.com/falexwolf) | 2023-07-26 |
+🚚 Rename `featureset_id` to `feature_set_id` in `FeatureSetFile` link table | [242](https://github.com/laminlabs/lnschema-core/pull/242) | [falexwolf](https://github.com/falexwolf) | 2023-07-26 |
+🚚 Add `Modality` | [240](https://github.com/laminlabs/lnschema-core/pull/240) | [falexwolf](https://github.com/falexwolf) | 2023-07-25 |
+🚚 Add `File.accessor` | [239](https://github.com/laminlabs/lnschema-core/pull/239) | [falexwolf](https://github.com/falexwolf) | 2023-07-25 |
+🚚 Remove reference Registry from Label and add it to Feature, add slot to FeatureSet link models | [238](https://github.com/laminlabs/lnschema-core/pull/238) | [falexwolf](https://github.com/falexwolf) | 2023-07-24 | 0.41.0
 📝 Updated view_parents signature | [237](https://github.com/laminlabs/lnschema-core/pull/237) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-23 | 0.40.1
 🚚 More comprehensive `Label` and `FeatureSet` fields | [236](https://github.com/laminlabs/lnschema-core/pull/236) | [falexwolf](https://github.com/falexwolf) | 2023-07-23 |
 🚚 Integrate `Category` and `Tag` into `Label` | [235](https://github.com/laminlabs/lnschema-core/pull/235) | [falexwolf](https://github.com/falexwolf) | 2023-07-22 |
 🚚 Add `description` and `parents` to `Tag`, delete `Project`, replace `Run.name` with `Run.reference_type`, `Run.inputs` as `File.input_of` | [233](https://github.com/laminlabs/lnschema-core/pull/233) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 🚚 Add categories to file and dataset | [232](https://github.com/laminlabs/lnschema-core/pull/232) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 💄 Improve docstring | [231](https://github.com/laminlabs/lnschema-core/pull/231) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-20 | 0.39.0
 🚚 Rename `FeatureValue` to `Category` | [230](https://github.com/laminlabs/lnschema-core/pull/230) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
@@ -23,15 +39,15 @@
 🚚 Move `QuerySet` to lamindb | [220](https://github.com/laminlabs/lnschema-core/pull/220) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 |
 ✨ Allow for annotate in `.df()` | [219](https://github.com/laminlabs/lnschema-core/pull/219) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 |
 🚚 Rename `File.name` to `File.description` | [218](https://github.com/laminlabs/lnschema-core/pull/218) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 | 0.38.0
 🚚 Update `Feature` and `FeatureSet` | [217](https://github.com/laminlabs/lnschema-core/pull/217) | [falexwolf](https://github.com/falexwolf) | 2023-07-01 |
 💄 Prettify dataframe display | [216](https://github.com/laminlabs/lnschema-core/pull/216) | [falexwolf](https://github.com/falexwolf) | 2023-06-30 |
 📝 Fix docs | [215](https://github.com/laminlabs/lnschema-core/pull/215) | [falexwolf](https://github.com/falexwolf) | 2023-06-30 | 0.37.0
 🚚 Move `File` docstrings and signatures | [214](https://github.com/laminlabs/lnschema-core/pull/214) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
-🚚 Rename `BaseORM` to `ORM`, move `ORM` signatures here | [213](https://github.com/laminlabs/lnschema-core/pull/213) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
+🚚 Rename `BaseORM` to `Registry`, move `Registry` signatures here | [213](https://github.com/laminlabs/lnschema-core/pull/213) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
 ✨ Add `Dataset` & `Feature` ORMs | [212](https://github.com/laminlabs/lnschema-core/pull/212) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 | 0.37a1
 💄 Denoise display of timestamps | [211](https://github.com/laminlabs/lnschema-core/pull/211) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 |
 🎨 Auto-manage `RunInput` relationship | [210](https://github.com/laminlabs/lnschema-core/pull/210) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 | 0.36.1
 🚚 Repurpose `Folder` to `Tag` | [209](https://github.com/laminlabs/lnschema-core/pull/209) | [falexwolf](https://github.com/falexwolf) | 2023-06-22 | 0.36.0
 🚚 Move `BaseORM.__init__` to lamindb | [208](https://github.com/laminlabs/lnschema-core/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 | 0.35.10
 🚚 Expand field length `short_name` in transform | [207](https://github.com/laminlabs/lnschema-core/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 |
 🔥 Remove `Lookup` | [206](https://github.com/laminlabs/lnschema-core/pull/206) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.35.9
@@ -79,21 +95,21 @@
 🐛 Fix `.replace()` for key != None | [156](https://github.com/laminlabs/lnschema-core/pull/156) | [falexwolf](https://github.com/falexwolf) | 2023-04-13 | 0.32.2
 🎨 Set `Transform` id upon insert, update `Transform` default | [154](https://github.com/laminlabs/lnschema-core/pull/154) | [falexwolf](https://github.com/falexwolf) | 2023-04-12 | 0.32.1
 🚚 Add app type | [155](https://github.com/laminlabs/lnschema-core/pull/155) | [falexwolf](https://github.com/falexwolf) | 2023-04-12 |
 🩹 Fix name check in replace | [153](https://github.com/laminlabs/lnschema-core/pull/153) | [Koncopd](https://github.com/Koncopd) | 2023-04-10 |
 ✨ Overwrite key in replace if needed | [152](https://github.com/laminlabs/lnschema-core/pull/152) | [Koncopd](https://github.com/Koncopd) | 2023-04-10 |
 🚸 Use full filename to populate `File.name`, introduce `File.key` and `Folder.key` | [150](https://github.com/laminlabs/lnschema-core/pull/150) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 | 0.32.0
 ✨ Add `File.replace()` and `File.stage()` | [149](https://github.com/laminlabs/lnschema-core/pull/149) | [Koncopd](https://github.com/Koncopd) | 2023-04-03 | 0.31.0
-♻️ Refactor ORM defintions | [148](https://github.com/laminlabs/lnschema-core/pull/148) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.30.0
+♻️ Refactor Registry defintions | [148](https://github.com/laminlabs/lnschema-core/pull/148) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.30.0
 🚚 Add `reference` to `Transform` | [147](https://github.com/laminlabs/lnschema-core/pull/147) | [falexwolf](https://github.com/falexwolf) | 2023-03-25 | 0.30rc5
 💚 Add weak backward compat | [commit](https://github.com/laminlabs/lnschema-core/commit/aa5ce2c272f0d9f14d7fa36a1298705c8ae6dda2) | [falexwolf](https://github.com/falexwolf) | 2023-03-24 | 0.30rc4
 🚚 Rename `DObject` to `File` and `DFolder` to `Folder` | [146](https://github.com/laminlabs/lnschema-core/pull/146) | [falexwolf](https://github.com/falexwolf) | 2023-03-24 | 0.30rc3
 🎨 Simplify `Run` | [145](https://github.com/laminlabs/lnschema-core/pull/145) | [falexwolf](https://github.com/falexwolf) | 2023-03-23 |
 🏗️ Combine `Notebook` and `Pipeline` into `Transform` | [144](https://github.com/laminlabs/lnschema-core/pull/144) | [falexwolf](https://github.com/falexwolf) | 2023-03-23 | 0.30rc2
-🔥 Remove Usage ORM | [143](https://github.com/laminlabs/lnschema-core/pull/143) | [falexwolf](https://github.com/falexwolf) | 2023-03-22 | 0.30rc1
+🔥 Remove Usage Registry | [143](https://github.com/laminlabs/lnschema-core/pull/143) | [falexwolf](https://github.com/falexwolf) | 2023-03-22 | 0.30rc1
 ⬆️ typeguard<3.0.0 and update lamindb | [141](https://github.com/laminlabs/lnschema-core/pull/141) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-15 | 0.29.7
 🚑 Fix __name__ of reltype | [137](https://github.com/laminlabs/lnschema-core/pull/137) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 | 0.29.6
 📝 Fix docs reference | [commit](https://github.com/laminlabs/lnschema-core/commit/e5b7d5d0bc7180e7c145f5ad7eac75db5928fde5) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 | 0.29.5
 🚸 Be smart about `global_context` and `load_latest` | [136](https://github.com/laminlabs/lnschema-core/pull/136) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 | 0.29.4
 🚚 Rename ref to reference, added backward compat for features_ref | [135](https://github.com/laminlabs/lnschema-core/pull/135) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-14 | 0.29.3
 ✨ Implement ln.Features | [134](https://github.com/laminlabs/lnschema-core/pull/134) | [sunnyosun](https://github.com/sunnyosun) | 2023-03-14 | 0.29.3rc1
 🚚 Move track_run logic here | [133](https://github.com/laminlabs/lnschema-core/pull/133) | [falexwolf](https://github.com/falexwolf) | 2023-03-13 | 0.29.2
@@ -118,22 +134,22 @@
 🚚 Add column `external_id` to `Run` | [109](https://github.com/laminlabs/lnschema-core/pull/109) | [falexwolf](https://github.com/falexwolf) | 2023-02-14 | 0.27.0
 🔧 Ensure all id lengths are multiples of 4 | [108](https://github.com/laminlabs/lnschema-core/pull/108) | [falexwolf](https://github.com/falexwolf) | 2023-02-14 |
 🚚 Move `storage` table back to `core` module | [89](https://github.com/laminlabs/lnschema-core/pull/89) | [falexwolf](https://github.com/falexwolf) | 2023-02-14 | 0.26.1
 🔥 Remove migration files | [107](https://github.com/laminlabs/lnschema-core/pull/107) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-14 | 0.26.0
 ⬆️ Upgrade and rename `lndb_setup` to `lndb` (v0.32.0) | [105](https://github.com/laminlabs/lnschema-core/pull/105) | [bpenteado](https://github.com/bpenteado) | 2023-02-13 | 0.25.12
 🚚 Rename `track_runin` to `is_run_input` | [104](https://github.com/laminlabs/lnschema-core/pull/104) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-13 | 0.25.11
 ✨ Added track_runin to DObject.load() | [103](https://github.com/laminlabs/lnschema-core/pull/103) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-13 | 0.25.10
-💄 Fix ORM preview message | [102](https://github.com/laminlabs/lnschema-core/pull/102) | [bpenteado](https://github.com/bpenteado) | 2023-02-07 |
-🚸 Introduce ORM relationship previews | [101](https://github.com/laminlabs/lnschema-core/pull/101) | [bpenteado](https://github.com/bpenteado) | 2023-02-07 |
+💄 Fix Registry preview message | [102](https://github.com/laminlabs/lnschema-core/pull/102) | [bpenteado](https://github.com/bpenteado) | 2023-02-07 |
+🚸 Introduce Registry relationship previews | [101](https://github.com/laminlabs/lnschema-core/pull/101) | [bpenteado](https://github.com/bpenteado) | 2023-02-07 |
 🚚 Rename `DSet` to `DFolder` | [100](https://github.com/laminlabs/lnschema-core/pull/100) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-07 | 0.25.9
-🔥  Disable ORM relationship preview | [99](https://github.com/laminlabs/lnschema-core/pull/99) | [bpenteado](https://github.com/bpenteado) | 2023-02-02 | 0.25.8
+🔥  Disable Registry relationship preview | [99](https://github.com/laminlabs/lnschema-core/pull/99) | [bpenteado](https://github.com/bpenteado) | 2023-02-02 | 0.25.8
 🐛 Fix assigning _cloud_filepath | [98](https://github.com/laminlabs/lnschema-core/pull/98) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-02 | 0.25.7
 ✨ Added _filekey to DObject for custom file keys | [97](https://github.com/laminlabs/lnschema-core/pull/97) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-02 | 0.25.6
 ✨ Added _cloud_filepath private attribute | [96](https://github.com/laminlabs/lnschema-core/pull/96) | [sunnyosun](https://github.com/sunnyosun) | 2023-02-02 | 0.25.5
-✨ Add rich string representation for ORM classes | [95](https://github.com/laminlabs/lnschema-core/pull/95) | [bpenteado](https://github.com/bpenteado) | 2023-01-31 | 0.25.4
+✨ Add rich string representation for Registry classes | [95](https://github.com/laminlabs/lnschema-core/pull/95) | [bpenteado](https://github.com/bpenteado) | 2023-01-31 | 0.25.4
 🚸 Auto populate fk constrained fields from `Relationship`s | [94](https://github.com/laminlabs/lnschema-core/pull/94) | [bpenteado](https://github.com/bpenteado) | 2023-01-26 | 0.25.3
 🐛 Fix strict type checking for relationships | [93](https://github.com/laminlabs/lnschema-core/pull/93) | [bpenteado](https://github.com/bpenteado) | 2023-01-24 | 0.25.2
 🩹 Fix error message in `Relationship` type checking | [92](https://github.com/laminlabs/lnschema-core/pull/92) | [bpenteado](https://github.com/bpenteado) | 2023-01-23 | 0.25.1
 ✨ Enable data validation with pydantic | [91](https://github.com/laminlabs/lnschema-core/pull/91) | [bpenteado](https://github.com/bpenteado) | 2023-01-20 | 0.25.0
 🩹 Fix `_dbconfig` | [90](https://github.com/laminlabs/lnschema-core/pull/90) | [falexwolf](https://github.com/falexwolf) | 2023-01-16 | 0.24.1
 👷 Extend CI to py3.8-3.10 | [88](https://github.com/laminlabs/lnschema-core/pull/88) | [sunnyosun](https://github.com/sunnyosun) | 2023-01-12 |
 🚚 Add `title` field to `Notebook` | [87](https://github.com/laminlabs/lnschema-core/pull/87) | [falexwolf](https://github.com/falexwolf) | 2023-01-09 | 0.24.0
```

### Comparing `lamindb_setup-0.49.4/lnschema-core/LICENSE` & `lamindb_setup-0.49.5/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,77 @@
-# Generated by Django 4.2.2 on 2023-07-24 16:50
+# Generated by Django 4.2.2 on 2023-07-28 13:22
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("lnschema_core", "0011_label_remove_tag_created_by_remove_tag_parents_and_more"),
+        ("lnschema_core", "0012_remove_label_ref_id_remove_label_ref_orm_and_more"),
     ]
 
     operations = [
         migrations.RemoveField(
-            model_name="label",
-            name="ref_id",
-        ),
-        migrations.RemoveField(
-            model_name="label",
-            name="ref_orm",
+            model_name="feature",
+            name="labels_orm",
         ),
         migrations.RemoveField(
-            model_name="label",
-            name="ref_schema",
-        ),
-        migrations.AddField(
             model_name="feature",
-            name="labels_orm",
-            field=models.CharField(db_index=True, default=None, max_length=40, null=True),
+            name="labels_schema",
         ),
         migrations.AddField(
             model_name="feature",
-            name="labels_schema",
-            field=models.CharField(db_index=True, default=None, max_length=40, null=True),
+            name="registries",
+            field=models.CharField(db_index=True, default=None, max_length=128, null=True),
         ),
-        migrations.CreateModel(
-            name="FileFeatureSet",
-            fields=[
-                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
-                ("slot", models.CharField(default=None, max_length=40, null=True)),
-                ("featureset", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.featureset")),
-                ("file", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.file")),
-            ],
-            options={
-                "unique_together": {("file", "featureset")},
-            },
+        migrations.AlterUniqueTogether(
+            name="label",
+            unique_together=set(),
         ),
         migrations.CreateModel(
-            name="DatasetFeatureSet",
+            name="FileLabel",
             fields=[
                 ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
-                ("slot", models.CharField(default=None, max_length=50, null=True)),
-                ("dataset", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.dataset")),
-                ("featureset", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.featureset")),
+                ("feature", models.ForeignKey(default=None, null=True, on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.feature")),
+                ("file", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.file")),
+                ("label", models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to="lnschema_core.label")),
             ],
             options={
-                "unique_together": {("dataset", "featureset")},
+                "unique_together": {("file", "label")},
             },
         ),
-        migrations.RunSQL("CREATE TABLE lnschema_core_filefeatureset_tmp (id BIGINT, file_id TEXT, featureset_id TEXT)"),
-        migrations.RunSQL("INSERT INTO lnschema_core_filefeatureset_tmp (id, file_id, featureset_id) SELECT id, file_id, featureset_id from lnschema_core_file_feature_sets"),
+        migrations.RunSQL("CREATE TABLE lnschema_core_filelabel_tmp (id BIGINT, file_id TEXT, label_id TEXT)"),
+        migrations.RunSQL("INSERT INTO lnschema_core_filelabel_tmp (id, file_id, label_id) SELECT id, file_id, label_id from lnschema_core_file_labels"),
         migrations.RemoveField(
             model_name="file",
-            name="feature_sets",
+            name="labels",
+        ),
+        migrations.AddField(
+            model_name="file",
+            name="labels",
+            field=models.ManyToManyField(related_name="files", through="lnschema_core.FileLabel", to="lnschema_core.label"),
+        ),
+        migrations.RunSQL("INSERT INTO lnschema_core_filelabel (id, file_id, label_id) SELECT id, file_id, label_id from lnschema_core_filelabel_tmp"),
+        migrations.RunSQL("DROP TABLE lnschema_core_filelabel_tmp"),
+        migrations.RemoveField(
+            model_name="label",
+            name="feature",
         ),
         migrations.RemoveField(
-            model_name="dataset",
-            name="feature_sets",
+            model_name="featureset",
+            name="ref_field",
         ),
-        migrations.AddField(
-            model_name="dataset",
-            name="feature_sets",
-            field=models.ManyToManyField(related_name="datasets", through="lnschema_core.DatasetFeatureSet", to="lnschema_core.featureset"),
+        migrations.RenameField(
+            model_name="featureset",
+            old_name="ref_orm",
+            new_name="ref_field",
         ),
-        migrations.AddField(
-            model_name="file",
-            name="feature_sets",
-            field=models.ManyToManyField(related_name="files", through="lnschema_core.FileFeatureSet", to="lnschema_core.featureset"),
+        migrations.RemoveField(
+            model_name="featureset",
+            name="ref_schema",
+        ),
+        migrations.AlterField(
+            model_name="featureset",
+            name="ref_field",
+            field=models.CharField(db_index=True, max_length=128),
         ),
-        migrations.RunSQL("INSERT INTO lnschema_core_filefeatureset (id, file_id, featureset_id) SELECT id, file_id, featureset_id from lnschema_core_filefeatureset_tmp"),
-        migrations.RunSQL("DROP TABLE lnschema_core_filefeatureset_tmp"),
     ]
```

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,49 +14,54 @@
     Union,
     overload,
 )
 
 from django.db import models
 from django.db.models import CASCADE, PROTECT
 from django.db.models.query_utils import DeferredAttribute as Field
+from lamindb_setup import _check_instance_setup
 from upath import UPath
 
 from lnschema_core.mocks import AnnDataAccessor, BackedAccessor, QuerySet
 from lnschema_core.types import AnnDataLike, DataLike, ListLike, PathLike, StrField
 
 from .ids import base62_8, base62_12, base62_20
 from .types import TransformType
 from .users import current_user_id
 
-if TYPE_CHECKING:
+_INSTANCE_SETUP = _check_instance_setup()
+
+if TYPE_CHECKING or _INSTANCE_SETUP:
     import pandas as pd
+    from lamindb.dev import FeatureManager
+
 
 IPYTHON = getattr(builtins, "__IPYTHON__", False)
 TRANSFORM_TYPE_DEFAULT = TransformType.notebook if IPYTHON else TransformType.pipeline
 
 
-class ORM(models.Model):
-    """LaminDB's base ORM.
+class Registry(models.Model):
+    """LaminDB's base Registry.
 
     Is based on django.db.models.Model.
 
-    Why does LaminDB call it `ORM` and not `Model`? The term "ORM" can't lead to
+    Why does LaminDB call it `Registry` and not `Model`? The term "Registry" can't lead to
     confusion with statistical, machine learning or biological models.
     """
 
     def add_synonym(
         self,
         synonym: Union[str, ListLike],
         force: bool = False,
         save: Optional[bool] = None,
     ):
         """Add synonyms to a record.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.remove_synonym`
+            :meth:`~lamindb.dev.Registry.remove_synonym`
                 Remove synonyms
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.CellType.from_bionty(name="T cell").save()
             >>> lookup = lb.CellType.lookup()
             >>> record = lookup.t_cell
@@ -68,15 +73,15 @@
         """
         pass
 
     def remove_synonym(self, synonym: Union[str, ListLike]):
         """Remove synonyms from a record.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.add_synonym`
+            :meth:`~lamindb.dev.Registry.add_synonym`
                 Add synonyms
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.CellType.from_bionty(name="T cell").save()
             >>> lookup = lb.CellType.lookup()
             >>> record = lookup.t_cell
@@ -88,17 +93,17 @@
         pass
 
     def describe(self):
         """Rich representation of a record with relationships.
 
         Examples:
             >>> ln.File(ln.dev.datasets.file_jpg_paradisi05(), description="paradisi05").save()
-            >>> file = ln.File.select(description="paradisi05").one()
+            >>> file = ln.File.filter(description="paradisi05").one()
             >>> ln.save(ln.Label.from_values(["image", "benchmark", "example"], field="name"))
-            >>> labels = ln.Label.select(name__in = ["image", "benchmark", "example"]).all()
+            >>> labels = ln.Label.filter(name__in = ["image", "benchmark", "example"]).all()
             >>> file.labels.set(labels)
             >>> file.describe()
             File(id=jb7BY5UJoQVGMUOKiLcn, key=None, suffix=.jpg, description=paradisi05, size=29358, hash=r4tnqmKI_SjrkdLzpuWp4g, hash_type=md5, created_at=2023-07-19 15:48:26.485889+00:00, updated_at=2023-07-19 16:43:17.792241+00:00) # noqa
             ...
             One/Many-to-One:
                 🔗 storage: Storage(id=Zl2q0vQB, root=/home/runner/work/lamindb/lamindb/docs/guide/mydata, type=local, updated_at=2023-07-19 14:18:21, created_by_id=DzTjkKse)
                 🔗 transform: None
@@ -119,69 +124,67 @@
 
         Notes:
             For more info, see tutorial: :doc:`/guide/data-lineage`.
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.Tissue.from_bionty(name="subsegmental bronchus").save()
-            >>> record = lb.Tissue.select(name="respiratory tube").one()
+            >>> record = lb.Tissue.filter(name="respiratory tube").one()
             >>> record.view_parents()
             >>> tissue.view_parents(with_children=True)
         """
         pass
 
     def set_abbr(self, value: str):
         """Set value for abbr field and add to synonyms.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.add_synonym`
+            :meth:`~lamindb.dev.Registry.add_synonym`
                 Add synonyms
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.ExperimentalFactor.from_bionty(name="single-cell RNA sequencing").save()
-            >>> scrna = lb.ExperimentalFactor.select(name="single-cell RNA sequencing").one()
+            >>> scrna = lb.ExperimentalFactor.filter(name="single-cell RNA sequencing").one()
             >>> scrna.abbr
             None
             >>> scrna.synonyms
             'single-cell RNA-seq|single-cell transcriptome sequencing|scRNA-seq|single cell RNA sequencing'
             >>> scrna.set_abbr("scRNA")
             >>> scrna.abbr
             'scRNA'
             >>> scrna.synonyms
             'scRNA|single-cell RNA-seq|single cell RNA sequencing|single-cell transcriptome sequencing|scRNA-seq'
             >>> scrna.save()
         """
         pass
 
     @classmethod
-    def from_values(cls, identifiers: ListLike, field: StrField, **kwargs) -> List["ORM"]:
+    def from_values(cls, values: ListLike, field: StrField, **kwargs) -> List["Registry"]:
         """Parse values for an identifier (a name, an id, etc.) and create records.
 
         This method helps avoid problems around duplication of entries,
         violation of idempotency, and performance when creating records in bulk.
 
         Args:
-            identifiers: ``ListLike`` A list of values for an identifier, e.g.
-                ``["name1", "name2"]``.
-            field: ``StrField`` An ``ORM`` field to look up, e.g., ``lb.CellMarker.name``.
-            **kwargs: Can contain ``species``. Either ``"human"``, ``"mouse"``, or any other
-                `name` of `Bionty.Species`. If ``None``, will use default species in
-                bionty for each entity.
+            values: `ListLike` A list of values for an identifier, e.g.
+                `["name1", "name2"]`.
+            field: `StrField` An ``Registry`` field to look up, e.g., `lb.CellMarker.name`.
+            **kwargs: Additional conditions for creation of records, e.g., `species="human"`.
 
         Returns:
             A list of records.
 
-        For every ``value`` in a list-like of identifiers and a given `ORM.field`,
+        For every `value` in a list-like of identifiers and a given `Registry.field`,
         this function performs:
 
         1. It checks whether the value already exists in the database
-           (``ORM.select(field=value)``). If so, it adds the queried record to
+           (``Registry.filter(field=value)``). If so, it adds the queried record to
            the returned list and skips step 2. Otherwise, proceed with 2.
-        2. If the ``ORM`` is from ``lnschema_bionty``, it checks whether there is an
+        2. If the ``Registry`` is from ``lnschema_bionty``, it checks whether there is an
            exact match in the underlying ontology (``Bionty.inspect(value, field)``).
            If so, it creates a record from Bionty and adds it to the returned list.
            Otherwise, it creates a record that populates a single field using `value`
            and adds the record to the returned list.
 
         Notes:
             For more info, see tutorial: :doc:`/biology/registries`.
@@ -254,15 +257,15 @@
 
         Returns:
             - A Dictionary of "mapped" and "unmapped" identifiers
             - If `return_df`: A DataFrame indexed by identifiers with a boolean `__mapped__`
                 column that indicates compliance with the identifiers.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.map_synonyms`
+            :meth:`~lamindb.dev.Registry.map_synonyms`
                 Standardize synonyms
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.settings.species = "human"
             >>> gene_synonyms = ["A1CF", "A1BG", "FANCD1", "FANCD20"]
             >>> ln.save(lb.Gene.from_values(gene_synonyms, field="symbol"))
@@ -284,15 +287,15 @@
                 look up the values for. Defaults to first string field.
 
         Returns:
             A `NamedTuple` of lookup information of the field values with a
             dictionary converter.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.search`
+            :meth:`~lamindb.dev.Registry.search`
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.settings.species = "human"
             >>> lb.Gene.from_bionty(symbol="ADGB-DT").save()
             >>> lookup = lb.Gene.lookup()
             >>> lookup.adgb_dt
@@ -335,31 +338,31 @@
 
         Returns:
             If `return_mapper` is `False`: a list of standardized names. Otherwise,
             a dictionary of mapped values with mappable synonyms as keys and
             standardized names as values.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.add_synonym`
+            :meth:`~lamindb.dev.Registry.add_synonym`
                 Add synonyms
-            :meth:`~lamindb.dev.ORM.remove_synonym`
+            :meth:`~lamindb.dev.Registry.remove_synonym`
                 Remove synonyms
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> lb.settings.species = "human"
             >>> gene_synonyms = ["A1CF", "A1BG", "FANCD1", "FANCD20"]
             >>> ln.save(lb.Gene.from_values(gene_synonyms, field="symbol"))
             >>> standardized_names = lb.Gene.map_synonyms(gene_synonyms)
             >>> standardized_names
             ['A1CF', 'A1BG', 'BRCA2', 'FANCD20']
         """
 
     @classmethod
-    def select(cls, **expressions) -> QuerySet:
+    def filter(cls, **expressions) -> QuerySet:
         """Query records.
 
         Args:
             expressions: Fields and values passed as Django query expressions.
 
         Returns:
             A :class:`~lamindb.dev.QuerySet`.
@@ -368,21 +371,21 @@
             `django queries <https://docs.djangoproject.com/en/4.2/topics/db/queries/>`__
 
         Notes:
             For more info, see tutorial: :doc:`/guide/select`.
 
         Examples:
             >>> ln.Label(name="my label").save()
-            >>> label = ln.Label.select(name="my label").one()
+            >>> label = ln.Label.filter(name="my label").one()
             >>> label
             Label(id=TMn5Zuju, name=my label, updated_at=2023-07-19 18:24:49, created_by_id=DzTjkKse)
         """
-        from lamindb._select import select
+        from lamindb._filter import filter
 
-        return select(cls, **expressions)
+        return filter(cls, **expressions)
 
     @classmethod
     def search(
         cls,
         string: str,
         *,
         field: Optional[StrField] = None,
@@ -403,15 +406,15 @@
                 column is available. If `None`, is ignored.
 
         Returns:
             A sorted `DataFrame` of search results with a score in column `__ratio__`.
             If `return_queryset` is `True`, a sorted QuerySet.
 
         See Also:
-            :meth:`~lamindb.dev.ORM.lookup`
+            :meth:`~lamindb.dev.Registry.lookup`
 
         Examples:
             >>> ln.save(ln.Label.from_values(["Label1", "Label2", "Label3"], field="name"))
             >>> ln.Label.search("Label2")
                         id   __ratio__
             name
             Label2  o3FY3c5n  100.000000
@@ -420,48 +423,59 @@
         """
         pass
 
     class Meta:
         abstract = True
 
 
+class Data:
+    """Base class for :class`~lamdindb.File` & :class`~lamdindb.Dataset`."""
+
+    @property
+    def features(self) -> "FeatureManager":
+        """Feature manager (:class:`~lamindb.dev.FeatureManager`)."""
+        pass
+
+
 # -------------------------------------------------------------------------------------
-# A note on required fields at the ORM level
+# A note on required fields at the Registry level
 #
 # As Django does most of its validation on the Form-level, it doesn't offer functionality
-# for validating the integrity of an ORM object upon instantation (similar to pydantic)
+# for validating the integrity of an Registry object upon instantation (similar to pydantic)
 #
 # For required fields, we define them as commonly done on the SQL level together
-# with a validator in ORM (validate_required_fields)
+# with a validator in Registry (validate_required_fields)
 #
 # This goes against the Django convention, but goes with the SQLModel convention
 # (Optional fields can be null on the SQL level, non-optional fields cannot)
 #
 # Due to Django's convention where CharField has pre-configured (null=False, default=""), marking
 # a required field necessitates passing `default=None`. Without the validator it would trigger
 # an error at the SQL-level, with it, it triggers it at instantiation
 
 # -------------------------------------------------------------------------------------
-# A note on class and instance methods of core ORM
+# A note on class and instance methods of core Registry
 #
 # All of these are defined and tested within lamindb, in files starting with _{orm_name}.py
 
 
-class User(ORM):
-    """Users.
+class User(Registry):
+    """User registry: humans and bots.
+
+    Is auto-managed. No need to create records.
 
     All data in this table is synched from the cloud user account to ensure a
     universal user identity, valid across DB instances and email & handle
     changes.
 
     Examples:
 
         Query a user by handle:
 
-        >>> user = ln.User.select(handle="testuser1").one()
+        >>> user = ln.User.filter(handle="testuser1").one()
         >>> user
         User(id=DzTjkKse, handle=testuser1, email=testuser1@lamin.ai, name=Test User1, updated_at=2023-07-10 18:37:26)
     """
 
     id = models.CharField(max_length=8, primary_key=True, default=None)
     """Universal id, valid across DB instances."""
     handle = models.CharField(max_length=30, unique=True, db_index=True, default=None)
@@ -471,17 +485,42 @@
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Name (optional)."""  # has to match hub specification, where it's also optional
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
 
+    @overload
+    def __init__(
+        self,
+        handle: str,
+        email: str,
+        name: Optional[str],
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        super(User, self).__init__(*args, **kwargs)
 
-class Storage(ORM):
-    """Storage locations: S3 or GCP buckets or local storage locations.
+
+class Storage(Registry):
+    """Storage locations: S3/GCP buckets or local directories.
+
+    Is auto-managed, no need to create objects.
 
     See Also:
         :attr:`~lamindb.dev.Settings.storage`
 
     Examples:
 
         Configure the default storage location upon initiation of a LaminDB instance:
@@ -512,24 +551,56 @@
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_storages")
     """Creator of record, a :class:`~lamindb.User`."""
 
+    @overload
+    def __init__(
+        self,
+        root: str,
+        type: str,
+        region: Optional[str],
+    ):
+        ...
 
-class Transform(ORM):
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        super(Storage, self).__init__(*args, **kwargs)
+
+
+class Transform(Registry):
     """Transforms of files & datasets.
 
     Pipelines, workflows, notebooks, app-based transformations.
 
     A pipeline is versioned software that transforms data.
     This can be anything from typical workflow tools (Nextflow, Snakemake,
     Prefect, Apache Airflow, etc.) to simple (versioned) scripts.
 
+    Args:
+        name: `str` A name.
+        short_name: `Optional[str] = None` A description.
+        version: `Optional[str] = "0"` A :class:`~lamindb.Transform` record or its name.
+        type: `Optional[TransformType] = None` Either `'notebook'`, `'pipeline'`
+            or `'app'`. If `None`, defaults to `'notebook'` within a notebook (IPython
+            environment), and to `'pipeline'` outside of it.
+        reference: `Optional[str] = None` A reference like a URL.
+
     See Also:
         :meth:`lamindb.track`
             Track global Transform & Run for a notebook or pipeline.
         :class:`~lamindb.Run`
             Executions of the transform.
 
     Notes:
@@ -552,18 +623,17 @@
 
     id = models.CharField(max_length=14, db_index=True, primary_key=True, default=None)
     """Universal id, composed of stem_id and version suffix."""
     name = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Transform name or title, a pipeline name, notebook title, etc..
     """
     short_name = models.CharField(max_length=128, db_index=True, null=True, default=None)
-    """A short name.
-    """
+    """A short name (optional)."""
     stem_id = models.CharField(max_length=12, default=base62_12, db_index=True)
-    """Stem of id, identifying transform up to version."""
+    """Stem of id, identifying the transform up to version (auto-managed)."""
     version = models.CharField(max_length=10, default="0", db_index=True)
     """Version, defaults to `"0"`.
 
     Use this to label different versions of the same pipeline, notebook, etc.
 
     Consider using `semantic versioning <https://semver.org>`__
     with `Python versioning <https://peps.python.org/pep-0440/>`__.
@@ -594,82 +664,141 @@
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_transforms")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         unique_together = (("stem_id", "version"),)
 
+    @overload
+    def __init__(
+        self,
+        name: str,
+        short_name: Optional[str] = None,
+        version: Optional[str] = "0",
+        type: Optional[TransformType] = None,
+        reference: Optional[str] = None,
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
 
-class Run(ORM):
-    """Runs of transforms (:class:`~lamindb.Transform`).
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        super(Transform, self).__init__(*args, **kwargs)
 
-    Typically, a run has inputs and outputs:
 
-    - References to outputs are stored in :class:`~lamindb.File` in the `run` field.
-      This is possible as every given file has a unique run that created it. Any
-      given `Run` can output multiple `files`: `run.outputs`.
-    - References to inputs are stored in the :class:`~lamindb.File` in the
-      `input_of` field. Any `file` might serve as an input for multiple `runs`.
-      Similarly, any `run` might have many `files` as inputs: `run.inputs`.
+class Run(Registry):
+    """Runs of transforms.
+
+    Args:
+        reference: `str` A name.
+        reference_type: `str` A description.
+        transform: `Transform` A :class:`~lamindb.Transform` record or its name.
 
     See Also:
         :meth:`lamindb.track`
             Track global Transform & Run for a notebook or pipeline.
         :class:`~lamindb.Transform`
             Transformations that runs execute.
 
     Notes:
-        For more info, see tutorial: :doc:`/guide/data-lineage`.
+        See guide: :doc:`/guide/data-lineage`.
+
+        Typically, a run has inputs and outputs:
+
+            - References to outputs are stored in :class:`~lamindb.File` in the `run` field.
+              This is possible as every given file has a unique run that created it. Any
+              given `Run` can output multiple `files`: `run.outputs`.
+            - References to inputs are stored in the :class:`~lamindb.File` in the
+              `input_of` field. Any `file` might serve as an input for multiple `runs`.
+              Similarly, any `run` might have many `files` as inputs: `run.inputs`.
 
     Examples:
 
         Track a pipeline run:
 
         >>> ln.Transform(name="Cell Ranger", version="7.2.0", type="pipeline").save()
-        >>> transform = ln.Transform.select(name="Cell Ranger", version="7.2.0").one()
+        >>> transform = ln.Transform.filter(name="Cell Ranger", version="7.2.0").one()
         >>> transform
         Transform(id=JhiujsLlbTKLIt, name=Cell Ranger, stem_id=JhiujsLlbTKL, version=7.2.0, type=pipeline, created_by_id=DzTjkKse)
         >>> ln.track(transform)
         💬 Loaded: Transform(id=ceHkZMaiHFdoB6, name=Cell Ranger, stem_id=ceHkZMaiHFdo, version=7.2.0, type=pipeline, updated_at=2023-07-10 18:37:19, created_by_id=DzTjkKse)
         ✅ Saved: Run(id=RcpWIKC8cF74Pn3RUJ1W, run_at=2023-07-10 18:37:19, transform_id=ceHkZMaiHFdoB6, created_by_id=DzTjkKse)
-        >>> ln.context.run
+        >>> ln.dev.context.run
         Run(id=RcpWIKC8cF74Pn3RUJ1W, run_at=2023-07-10 18:37:19, transform_id=ceHkZMaiHFdoB6, created_by_id=DzTjkKse)
 
         Track a notebook run:
 
         >>> ln.track()
         ✅ Saved: Transform(id=1LCd8kco9lZUBg, name=Track data lineage / provenance, short_name=02-data-lineage, stem_id=1LCd8kco9lZU, version=0, type=notebook, updated_at=2023-07-10 18:37:19, created_by_id=DzTjkKse) # noqa
         ✅ Saved: Run(id=pHgVICV9DxBaV6BAuKJl, run_at=2023-07-10 18:37:19, transform_id=1LCd8kco9lZUBg, created_by_id=DzTjkKse)
-        >>> ln.context.run
+        >>> ln.dev.context.run
         Run(id=pHgVICV9DxBaV6BAuKJl, run_at=2023-07-10 18:37:19, transform_id=1LCd8kco9lZUBg, created_by_id=DzTjkKse)
     """
 
     id = models.CharField(max_length=20, default=base62_20, primary_key=True)
     """Universal id, valid across DB instances."""
-    reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """A reference like a URL or external ID (such as from a workflow manager)."""
-    reference_type = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """Type of reference, e.g., a workflow manager execution ID."""
     transform = models.ForeignKey(Transform, CASCADE, related_name="runs")
     """The transform :class:`~lamindb.Transform` that is being run."""
-    # input_files on File
-    # output_files on File
-    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
-    """Time of creation of record."""
     run_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of run execution."""
     created_by = models.ForeignKey(User, CASCADE, default=current_user_id, related_name="created_runs")
     """Creator of record, a :class:`~lamindb.User`."""
+    # input_files on File
+    # output_files on File
+    reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """A reference like a URL or external ID (such as from a workflow manager)."""
+    reference_type = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """Type of reference, e.g., a workflow manager execution ID."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
 
+    @overload
+    def __init__(
+        self,
+        reference: str,
+        reference_type: str,
+        transform: Transform,
+    ):
+        ...
 
-class Label(ORM):
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        super(Run, self).__init__(*args, **kwargs)
+
+
+class Label(Registry):
     """Labels for files & datasets.
 
-    A label can be used to annotate a file or dataset as a whole. For instance,
-    with "Project 1", "curated", or "Iris flower".
+    Args:
+        name: `str` A name.
+        description: `str` A description.
+        feature: `Optional[Union["Feature", str]]` A :class:`~lamindb.Feature`
+            record or its name.
+
+    A label can be used to annotate a file or dataset as a whole: "Project 1",
+    "curated", or "Iris flower".
 
     In some cases, a label is measured only within a part of a file or dataset.
     Then, a :class:`~lamindb.Feature` qualifies the measurement and slot for the
     label measurements (typically, a column name). For instance, the dataset
     might contain measurements across 2 species of the Iris flower: "setosa" &
     "versicolor".
 
@@ -680,141 +809,226 @@
         :mod:`lnschema_bionty` to label files & datasets.
 
         If you work with biological samples, likely, the only sustainable way of
         tracking metadata, is to create a custom schema module.
 
     See Also:
         :meth:`lamindb.Feature`
-            Qualifiers for measurements in files & datasets.
+            Dimensions of measurement for files & datasets.
 
     Examples:
 
         Create a new label:
 
         >>> label = ln.Label(name="ML output")
         >>> label.save()
         >>> label
         Label(id=gelGp2P6, name=ML output, created_by_id=DzTjkKse)
 
         Label a file:
 
-        >>> label = ln.Label.select(name="ML output").one()
+        >>> label = ln.Label.filter(name="ML output").one()
         >>> label
         Label(id=gelGp2P6, name=ML output, created_by_id=DzTjkKse)
         >>> file = ln.File("./myfile.csv")
         >>> file.save()
         >>> file
         File(id=MveGmGJImYY5qBwmr0j0, suffix=.csv, size=4, hash=CY9rzUYh03PK3k6DJie09g, hash_type=md5, updated_at=2023-07-19 13:47:59, storage_id=597Sgod0, created_by_id=DzTjkKse) # noqa
         >>> file.labels.add(label)
         >>> file.labels.list("name")
         ['ML output']
 
         Group labels:
 
         >>> ln.Label(name="Project 1").save()
-        >>> project1 = ln.Label.select(name="Project 1").one()
+        >>> project1 = ln.Label.filter(name="Project 1").one()
         >>> ln.Label(name="is_project").save()
-        >>> is_project = ln.Label.select(name="is_project").one()
+        >>> is_project = ln.Label.filter(name="is_project").one()
         >>> project1.parents.add(is_project)
 
         Query by label:
 
-        >>> ln.File.select(labels=project).first()
+        >>> ln.File.filter(labels=project).first()
         File(id=MveGmGJImYY5qBwmr0j0, suffix=.csv, size=4, hash=CY9rzUYh03PK3k6DJie09g, hash_type=md5, updated_at=2023-07-19 13:47:59, storage_id=597Sgod0, created_by_id=DzTjkKse) # noqa
     """
 
     id = models.CharField(max_length=8, default=base62_8, primary_key=True)
     """A universal random id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, unique=True, default=None)
     """Name or title of label (required)."""
     description = models.TextField(null=True, default=None)
     """A description (optional)."""
     parents = models.ManyToManyField("self", symmetrical=False, related_name="children")
     """Parent labels, useful to hierarchically group labels (optional)."""
-    feature = models.ForeignKey("Feature", CASCADE, related_name="labels", null=True, default=None)
-    """The feature in which the label is sampled (optional)."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_labels")
     """Creator of record, a :class:`~lamindb.User`."""
 
-    class Meta:
-        unique_together = (("name", "feature"),)
+    @overload
+    def __init__(
+        self,
+        name: str,
+        description: str,
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        pass
 
 
-class Feature(ORM):
-    """Qualifiers for measurements in files & datasets.
+class Modality(Registry):
+    """Measurement types of features.
+
+    .. note::
+
+        This will soon borrow readout-related records from the experimental factor
+        ontology, see :class:`~lnschema_bionty.ExperimentalFactor`.
+
+    Args:
+        name: `str` A name.
+        ontology_id: `Optional[str]` A public ontology ID.
+        abbr: `Optional[str]` An abbreviation.
+        description: `Optional[str]` A description.
+    """
+
+    id = models.CharField(max_length=8, default=base62_8, primary_key=True)
+    """Universal id, valid across DB instances."""
+    name = models.CharField(max_length=256, db_index=True)
+    """Name of the modality (required)."""
+    ontology_id = models.CharField(max_length=32, db_index=True, null=True, default=None)
+    """Ontology ID of the modality."""
+    abbr = models.CharField(max_length=32, db_index=True, unique=True, null=True, default=None)
+    """A unique abbreviation for the modality (optional)."""
+    synonyms = models.TextField(null=True, default=None)
+    """Bar-separated (|) synonyms that correspond to this modality."""
+    description = models.TextField(null=True, default=None)
+    """Description."""
+    molecule = models.TextField(null=True, default=None, db_index=True)
+    """Molecular experimental factor, parsed from EFO."""
+    instrument = models.TextField(null=True, default=None, db_index=True)
+    """Instrument used to measure, parsed from EFO."""
+    measurement = models.TextField(null=True, default=None, db_index=True)
+    """Phenotypic experimental factor, parsed from EFO."""
+    parents = models.ManyToManyField("self", symmetrical=False, related_name="children")
+    """Parents."""
+    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    """Time of creation of record."""
+    updated_at = models.DateTimeField(auto_now=True, db_index=True)
+    """Time of last update to record."""
+    created_by = models.ForeignKey(
+        User,
+        models.PROTECT,
+        default=current_user_id,
+        related_name="created_modalities",
+    )
+    """Creator of record, a :class:`~lamindb.User`."""
+
+    @overload
+    def __init__(
+        self,
+        name: str,
+        ontology_id: str,
+        abbr: Optional[str],
+        description: Optional[str],
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        super(Modality, self).__init__(*args, **kwargs)
+
+
+class Feature(Registry):
+    """Dimensions of measurements in files & datasets.
 
     See Also:
         :meth:`~lamindb.Feature.from_df`
             Create feature records from DataFrame.
+        :attr:`lamindb.File.features`
+            Manage feature annotations of files.
         :meth:`lamindb.Label`
             Labels for files & datasets.
 
     Args:
         name: `str` Name of the feature, typically, a column name.
-        type: `str` Simple type ("float", "int", "str", "categorical"). If
-            "categorical", consider managing categories with
-            :class:`~lamindb.Label`.
-        unit: `Optional[str] = None` Unit of measure, ideally SI (`m`, `s`, `kg`, etc.) or 'normalized' etc.
+        type: `str` Simple type ("float", "int", "str", "category").
+        unit: `Optional[str] = None` Unit of measure, ideally SI (`"m"`, `"s"`, `"kg"`, etc.) or `"normalized"` etc.
         description: `Optional[str] = None` A description.
         synonyms: `Optional[str] = None` Bar-separated synonyms.
 
     .. note::
 
         *Features* and *labels* are two ways of using entities to structure & categorize data:
 
         1. a feature qualifies *which entity* is measured as part of a *joint* measurement
         2. a label *is* a measured value of an entity
 
     Notes:
 
-        - :doc:`/biology/scrna`
-        - :doc:`/biology/flow`
-
         For more control, you can use :mod:`lnschema_bionty` ORMs to manage
         common basic biological entities like genes, proteins & cell markers
         involved in expression/count measurements.
 
         Similarly, you can define custom ORMs to manage high-level derived
         features like gene sets, malignancy, etc.
 
     Examples:
 
         >>> df = pd.DataFrame({"feat1": [1, 2], "feat2": [3.1, 4.2], "feat3": ["cond1", "cond2"]})
         >>> features = ln.Feature.from_df(df)
         >>> features.save()
         >>> # the information from the DataFrame is now available in the Feature table
-        >>> ln.Feature.select().df()
+        >>> ln.Feature.filter().df()
         id    name    type
          a   feat1     int
          b   feat2   float
          c   feat3     str
 
     """
 
     id = models.CharField(max_length=12, default=base62_12, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, default=None)
     """Name of feature (required)."""
     type = models.CharField(max_length=64, db_index=True, default=None)
     """Simple type ("float", "int", "str", "category").
 
-    If "category", consider managing categories with :class:`~lamindb.Label` or another label ORM.
+    If "category", consider managing categories with :class:`~lamindb.Label` or
+    another Registry for managing labels.
     """
     unit = models.CharField(max_length=30, db_index=True, null=True, default=None)
-    """Unit of measure, ideally SI (`m`, `s`, `kg`, etc.) or 'normalized' etc. (optional)"""
+    """Unit of measure, ideally SI (`m`, `s`, `kg`, etc.) or 'normalized' etc. (optional)."""
     description = models.TextField(db_index=True, null=True, default=None)
     """A description."""
-    labels_orm = models.CharField(max_length=40, db_index=True, default=None, null=True)
-    """ORM providing the vocabulary for labels, e.g., :class:`lnschema_bionty.CellLine` (optional)."""
-    labels_schema = models.CharField(max_length=40, db_index=True, default=None, null=True)
-    """Schema of the ORM (optional)."""
+    registries = models.CharField(max_length=128, db_index=True, default=None, null=True)
+    """ORMs that provide identifiers for labels, bar-separated (|) (optional)."""
     synonyms = models.TextField(null=True, default=None)
     """Bar-separated (|) synonyms (optional)."""
     feature_sets = models.ManyToManyField("FeatureSet", related_name="features")
     """Feature sets linked to this feature."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
@@ -856,53 +1070,46 @@
         pass
 
     def save(self, *args, **kwargs) -> None:
         """Save."""
         pass
 
 
-class FeatureSet(ORM):
+class FeatureSet(Registry):
     """Jointly measured sets of features.
 
     See Also:
         :meth:`~lamindb.FeatureSet.from_values`
             Create from values.
         :meth:`~lamindb.FeatureSet.from_df`
             Create from dataframe columns.
+        :class:`~lamindb.Modality`
+            Type of measurement.
 
     Note:
 
         Feature sets are useful as you might have millions of data batches
         that measure the same features: all of them link against the same
         feature set. If instead, you'd link against single features (say, genes),
         you'd face exploding link tables.
 
         A `feature_set` is identified by the hash of feature identifiers.
 
     Args:
-        features: `Iterable[ORM]` An iterable of :class:`~lamindb.Feature`
-            records to hash, e.g., `[Feature(...), Feature(...)]. Is turned into
+        features: `Iterable[Registry]` An iterable of :class:`~lamindb.Feature`
+            records to hash, e.g., `[Feature(...), Feature(...)]`. Is turned into
             a set upon instantiation. If you'd like to pass values, use
             :meth:`~lamindb.FeatureSet.from_values` or
             :meth:`~lamindb.FeatureSet.from_df`.
-        ref_field: `Optional[str] = "id"` The field providing the identifier to
-            hash.
         type: `Optional[Union[Type, str]] = None` The simple type. Defaults to
-            `None` if reference ORM is :class:`~lamindb.Feature`, defaults to
+            `None` if reference Registry is :class:`~lamindb.Feature`, defaults to
             `"float"` otherwise.
-        readout: Optional[str]: `Optional[str] = None` An abbreviation for
-            the readout measured for each feature, ideally from,
-            :mod:`lnschema_bionty.ExperimentalFactor.abbr`.
+        modality: `Optional[str] = None` A name or id for :class:`~lamindb.Modality`.
         name: `Optional[str] = None` A name.
 
-    Notes:
-
-        - :doc:`/biology/scrna`
-        - :doc:`/biology/flow`
-
     Examples:
 
         >>> df = pd.DataFrame({"feat1": [1, 2], "feat2": [3.1, 4.2], "feat3": ["cond1", "cond2"]})
         >>> feature_set = ln.FeatureSet.from_df(df)
 
         >>> features = ln.Feature.from_values(["feat1", "feat2"], type=float)
         >>> ln.FeatureSet(features)
@@ -919,40 +1126,37 @@
     id = models.CharField(max_length=20, primary_key=True, default=None)
     """A universal id (hash of the set of feature identifiers)."""
     name = models.CharField(max_length=128, null=True, default=None)
     """A name (optional)."""
     n = models.IntegerField()
     """Number of features in the set."""
     type = models.CharField(max_length=64, null=True, default=None)
-    """Simple type, e.g., "str", "int". Is `None` for :class:`~lamindb.Feature` (optional)."""
-    readout = models.CharField(max_length=64, null=True, default=None)
-    """The readout type, e.g., "RNA", "Protein", etc.
-
-    Consider using :mod:`lnschema_bionty.ExperimentalFactor.abbr`.
-    """
-    ref_field = models.CharField(max_length=64, db_index=True)
-    """Field of ORM that was hashed."""
-    ref_orm = models.CharField(max_length=64, db_index=True)
-    """The reference ORM for feature identifiers."""
-    ref_schema = models.CharField(max_length=64, db_index=True)
-    """The schema where the reference ORM is defined."""
+    """Simple type, e.g., "str", "int". Is `None` for :class:`~lamindb.Feature` (optional).
+
+    For :class:`~lamindb.Feature`, types are expected to be in-homogeneous and defined on a per-feature level.
+    """
+    modality = models.ForeignKey(Modality, PROTECT, null=True, default=None)
+    """The measurement modality, e.g., "RNA", "Protein", "Gene Module", "pathway" (:class:`~lamindb.Modality`)."""
+    registry = models.CharField(max_length=128, db_index=True)
+    """The registry that stores & validated the features `'bionty.Gene'`."""
+    hash = models.CharField(max_length=20, default=None, db_index=True, null=True)
+    """The hash of the set."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
-    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_featuresets")
+    created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_feature_sets")
     """Creator of record, a :class:`~lamindb.User`."""
 
     @overload
     def __init__(
         self,
-        features: Iterable[ORM],
-        ref_field: Optional[str] = None,
+        features: Iterable[Registry],
         type: Optional[Union[Type, str]] = None,
-        readout: Optional[str] = None,
+        modality: Optional[str] = None,
         name: Optional[str] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
@@ -963,28 +1167,28 @@
     def __init__(
         self,
         *args,
         **kwargs,
     ):
         pass
 
-    @classmethod  # type:ignore
-    def from_values(cls, values: ListLike, field: Field = Feature.name, type: Optional[Union[Type, str]] = None, name: Optional[str] = None, readout: Optional[str] = None, **kwargs) -> "FeatureSet":  # type: ignore  # noqa
-        """Create feature set from identifier values.
+    @classmethod
+    def from_values(  # type: ignore
+        cls, values: ListLike, field: Field = Feature.name, type: Optional[Union[Type, str]] = None, name: Optional[str] = None, modality: Optional[str] = None, **kwargs
+    ) -> Optional["FeatureSet"]:
+        """Create feature set for validated features.
 
         Args:
             values: ``ListLike`` A list of identifiers, like feature names or ids.
-            field: ``Field = Feature.name`` The field of a reference ORM to
+            field: ``Field = Feature.name`` The field of a reference Registry to
                 map values.
             type: `Optional[Union[Type, str]] = None` The simple type. Defaults to
-                `None` if reference ORM is :class:`~lamindb.Feature`, defaults to
+                `None` if reference registry is :class:`~lamindb.Feature`, defaults to
                 `"float"` otherwise.
-            readout: Optional[str]: `Optional[str] = None` An abbreviation for
-                the readout measured for each feature, ideally from,
-                :mod:`lnschema_bionty.ExperimentalFactor.abbr`.
+            modality: `Optional[str] = None` A name or id for :class:`~lamindb.Modality`.
             name: `Optional[str] = None` A name.
             **kwargs: Can contain ``species`` or other context to interpret values.
 
         Examples:
 
             >>> features = ["feat1", "feat2"]
             >>> feature_set = ln.FeatureSet.from_values(features)
@@ -995,70 +1199,66 @@
         pass
 
     @classmethod
     def from_df(
         cls,
         df: "pd.DataFrame",
         name: Optional[str] = None,
-    ) -> "FeatureSet":
-        """Create Feature records for columns."""
+    ) -> Optional["FeatureSet"]:
+        """Create feature set for validated features."""
         pass
 
     def save(self, *args, **kwargs) -> None:
         """Save."""
+        pass
 
 
-class File(ORM):
-    """Batches of data stored as files and objects.
+class File(Registry, Data):
+    """File registry: data batches.
 
     Args:
-        data: `Union[PathLike, DataLike]` A file path or an in-memory data
-            object (`DataFrame`, `AnnData`) to serialize. Can be a cloud path, e.g.,
-            `"s3://my-bucket/my_samples/my_file.fcs"`.
-        key: `Optional[str] = None` A storage key: a relative filepath within the
-            current default storage, e.g., `"my_samples/my_file.fcs"`.
-        name: `Optional[str] = None` A description.
-        run: `Optional[Run] = None` The run that created the file, gets auto-linked
-            if `ln.track()` was called.
-
-    Track where files come from by passing the generating :class:`~lamindb.Run`.
-
-    Often, files store jointly measured features: track them with
-    :class:`~lamindb.FeatureSet`.
-
-    If files have corresponding representations in storage and memory, LaminDB
-    makes some configurable default choices (e.g., serialize a `DataFrame` as a
-    `.parquet` file).
+        data: `Union[PathLike, DataLike]` A file path or a data
+            object (`DataFrame`, `AnnData`) to serialize. Can be a cloud path,
+            e.g., `"s3://my-bucket/myfolder/myfile.fcs"`.
+        key: `Optional[str] = None` The desired storage key: a relative filepath
+            within the a storage location, e.g., `"myfolder/myfile.fcs"`. If
+            `None`, gets auto-populated for data in the cloud.
+        description: `Optional[str] = None` A description.
+        run: `Optional[Run] = None` The run that created the file. If `None`,
+            gets auto-linked if you generated a run context with :meth:`~lamindb.track`.
 
-    .. admonition:: Formats in storage & their API access
+    .. admonition:: Typical formats in storage & their API accessors
 
-        Listed are typical `suffix` values & in memory data objects.
+        Listed are typical values for :attr:`~lamindb.File.suffix` & :attr:`~lamindb.File.accessor`.
 
         - Table: `.csv`, `.tsv`, `.parquet`, `.ipc` ⟷ `DataFrame`, `pyarrow.Table`
         - Annotated matrix: `.h5ad`, `.h5mu`, `.zrad` ⟷ `AnnData`, `MuData`
         - Image: `.jpg`, `.png` ⟷ `np.ndarray`, ...
         - Arrays: HDF5 group, zarr group, TileDB store ⟷ HDF5, zarr, TileDB loaders
         - Fastq: `.fastq` ⟷ /
         - VCF: `.vcf` ⟷ /
         - QC: `.html` ⟷ /
 
+        LaminDB makes some default choices (e.g., serialize a `DataFrame` as a
+        `.parquet` file).
+
     Note:
         In some cases, e.g. for zarr-based storage, a `File` object is stored as
         many small objects in what appears to be a "folder" in storage.
 
     See Also:
         :meth:`lamindb.File.from_df`
             Create a file object from `DataFrame` and track features.
         :meth:`lamindb.File.from_anndata`
             Create a file object from `AnnData` and track features.
         :meth:`lamindb.File.from_dir`
             Bulk create file objects from a directory.
 
     Notes:
-        For more info, see tutorial: :doc:`/guide/tutorial1`.
+        For more info, see tutorial: :doc:`/tutorial1`.
 
     Examples:
 
         Track a file from a local filepath:
 
         >>> filepath = ln.dev.datasets.file_mini_csv()
         >>> filepath
@@ -1087,14 +1287,19 @@
     """Storage key, the relative path within the storage location."""
     suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """File suffix.
 
     This is a file extension if the `file` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
     """
+    accessor = models.CharField(max_length=64, db_index=True, null=True, default=None)
+    """Default backed or memory accessor, e.g., DataFrame, AnnData.
+
+    Soon, also: SOMA, MuData, zarr.Group, tiledb.Array, etc.
+    """
     description = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """A description."""
     size = models.BigIntegerField(null=True, db_index=True)
     """Size in bytes.
 
     Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
     """
@@ -1105,15 +1310,15 @@
     """
     hash_type = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """Type of hash."""
     feature_sets = models.ManyToManyField(FeatureSet, related_name="files", through="FileFeatureSet")
     """The feature sets measured in the file (see :class:`~lamindb.FeatureSet`)."""
     transform = models.ForeignKey(Transform, PROTECT, related_name="files", null=True, default=None)
     """:class:`~lamindb.Transform` whose run created the `file`."""
-    labels = models.ManyToManyField(Label, related_name="files")
+    labels = models.ManyToManyField(Label, through="FileLabel", related_name="files")
     """:class:`~lamindb.File` records in label."""
     run = models.ForeignKey(Run, PROTECT, related_name="output_files", null=True, default=None)
     """:class:`~lamindb.Run` that created the `file`."""
     input_of = models.ManyToManyField(Run, related_name="input_files")
     """Runs that use this file as an input."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
@@ -1126,16 +1331,16 @@
         unique_together = (("storage", "key"),)
 
     @overload
     def __init__(
         self,
         data: Union[PathLike, DataLike],
         key: Optional[str] = None,
+        description: Optional[str] = None,
         run: Optional[Run] = None,
-        name: Optional[str] = None,
     ):
         ...
 
     @overload
     def __init__(
         self,
         *db_args,
@@ -1163,15 +1368,15 @@
         See Also:
             :meth:`lamindb.Dataset`
                 Track datasets.
             :class:`lamindb.Feature`
                 Track features.
 
         Notes:
-            For more info, see tutorial: :doc:`/guide/tutorial1`.
+            For more info, see tutorial: :doc:`/tutorial1`.
 
         Examples:
             >>> df = ln.dev.datasets.df_iris_in_meter_batch1()
             >>> df.head()
               sepal_length sepal_width petal_length petal_width iris_species_code
             0        0.051       0.035        0.014       0.002                 0
             1        0.049       0.030        0.014       0.002                 0
@@ -1206,15 +1411,15 @@
             :meth:`lamindb.Dataset`
                 Track datasets.
             :class:`lamindb.Feature`
                 Track features.
 
         Notes:
 
-            For more info, see tutorial: :doc:`/guide/tutorial1`.
+            For more info, see tutorial: :doc:`/tutorial1`.
 
         Examples:
             >>> import lnschema_bionty as lb
             lb.settings.species = "human"
             ✅ Set species: Species(id=uHJU, name=human, taxon_id=9606, scientific_name=homo_sapiens, updated_at=2023-07-19 14:45:17, bionty_source_id=t317, created_by_id=DzTjkKse) # noqa
             >>> adata = ln.dev.datasets.anndata_with_obs()
             >>> adata
@@ -1234,20 +1439,28 @@
         """
         pass
 
     @classmethod
     def from_dir(
         cls,
         path: PathLike,
+        key: Optional[str] = None,
         *,
         run: Optional[Run] = None,
-        storage_root: Optional[PathLike] = None,
     ) -> List["File"]:
         """Create a list of file objects from a directory.
 
+        Args:
+            path: `PathLike` Source path of folder.
+            key: `Optional[str]` Key for storage destination. If `None` and
+                directory is in a registered location, an inferred `key` will
+                reflect the relative position. If `None` and directory is outside
+                of a registered storage location, the inferred key defaults to `path.name`.
+            run: `Run` A `Run` object.
+
         Examples:
             >>> dir_path = ln.dev.datasets.generate_cell_ranger_files("sample_001", ln.settings.storage)
             >>> dir_path.name
             'sample_001'
             >>> files = ln.File.from_dir(dir_path)
             💡 using storage prefix = sample_001/
             💬 → 15 files
@@ -1293,42 +1506,43 @@
         Notes:
             For more info, see tutorial: :doc:`/guide/stream`.
 
         Examples:
 
             Read AnnData in backed mode from cloud:
 
-            >>> file = ln.File.select(key="lndb-storage/pbmc68k.h5ad").one()
+            >>> file = ln.File.filter(key="lndb-storage/pbmc68k.h5ad").one()
             >>> file.backed()
             AnnData object with n_obs × n_vars = 70 × 765 backed at 's3://lamindb-ci/lndb-storage/pbmc68k.h5ad'
                 obs: ['cell_type', 'index', 'louvain', 'n_genes', 'percent_mito']
                 obsm: ['X_pca', 'X_umap']
                 obsp: ['connectivities', 'distances']
                 uns: ['louvain', 'louvain_colors', 'neighbors', 'pca']
                 var: ['highly_variable', 'index', 'n_counts']
                 varm: ['PCs']
         """
         pass
 
     @classmethod
     def tree(
         cls,
-        prefix: Optional[str] = None,
+        path: Optional[PathLike] = None,
         *,
         level: int = -1,
         limit_to_directories: bool = False,
         length_limit: int = 1000,
-    ):
-        """Given a prefix, print a visual tree structure of files.
+    ) -> None:
+        """Print a visual tree structure of files & directories.
 
         Examples:
             >>> dir_path = ln.dev.datasets.generate_cell_ranger_files("sample_001", ln.settings.storage)
             >>> dir_path.name
             'sample_001'
             >>> ln.File.tree(dir_path)
+            3 subdirectories, 15 files
             sample_001
             ├── web_summary.html
             ├── metrics_summary.csv
             ├── molecule_info.h5
             ├── filtered_feature_bc_matrix
             │   ├── features.tsv.gz
             │   ├── barcodes.tsv.gz
@@ -1340,35 +1554,33 @@
             │   ├── barcodes.tsv.gz
             │   └── matrix.mtx.gz
             ├── possorted_genome_bam.bam.bai
             ├── cloupe.cloupe
             ├── possorted_genome_bam.bam
             ├── filtered_feature_bc_matrix.h5
             └── raw_feature_bc_matrix.h5
-            ...
-            3 directories, 15 files
         """
         pass
 
     def path(self) -> Union[Path, UPath]:
         """Path in storage.
 
         Examples:
 
             File in cloud storage:
 
             >>> ln.File("s3://lamindb-ci/lndb-storage/pbmc68k.h5ad").save()
-            >>> file = ln.File.select(key="lndb-storage/pbmc68k.h5ad").one()
+            >>> file = ln.File.filter(key="lndb-storage/pbmc68k.h5ad").one()
             >>> file.path()
             S3Path('s3://lamindb-ci/lndb-storage/pbmc68k.h5ad')
 
             File in local storage:
 
             >>> ln.File("./myfile.csv", description="myfile").save()
-            >>> file = ln.File.select(description="myfile").one()
+            >>> file = ln.File.filter(description="myfile").one()
             >>> file.path()
             PosixPath('/home/runner/work/lamindb/lamindb/docs/guide/mydata/myfile.csv')
         """
         pass
 
     def load(self, is_run_input: Optional[bool] = None, stream: bool = False) -> DataLike:
         """Slabele and load to memory.
@@ -1376,40 +1588,40 @@
         Returns in-memory representation if possible, e.g., an `AnnData` object for an `h5ad` file.
 
         Examples:
 
             Load as a `DataFrame`:
 
             >>> ln.File.from_df(ln.dev.datasets.df_iris_in_meter_batch1(), description="iris").save()
-            >>> file = ln.File.select(description="iris").one()
+            >>> file = ln.File.filter(description="iris").one()
             >>> file.load().head()
             sepal_length sepal_width petal_length petal_width iris_species_code
             0        0.051       0.035        0.014       0.002                 0
             1        0.049       0.030        0.014       0.002                 0
             2        0.047       0.032        0.013       0.002                 0
             3        0.046       0.031        0.015       0.002                 0
             4        0.050       0.036        0.014       0.002                 0
 
             Load as an `AnnData`:
 
             >>> ln.File("s3://lamindb-ci/lndb-storage/pbmc68k.h5ad").save()
-            >>> file = ln.File.select(key="lndb-storage/pbmc68k.h5ad").one()
+            >>> file = ln.File.filter(key="lndb-storage/pbmc68k.h5ad").one()
             >>> file.load()
             AnnData object with n_obs × n_vars = 70 × 765
                 obs: 'cell_type', 'n_genes', 'percent_mito', 'louvain'
                 var: 'n_counts', 'highly_variable'
                 uns: 'louvain', 'louvain_colors', 'neighbors', 'pca'
                 obsm: 'X_pca', 'X_umap'
                 varm: 'PCs'
                 obsp: 'connectivities', 'distances'
 
             Fall back to :meth:`~lamindb.File.stage` if no in-memory representation is configured:
 
             >>> ln.File(ln.dev.datasets.file_jpg_paradisi05(), description="paradisi05").save()
-            >>> file = ln.File.select(description="paradisi05").one()
+            >>> file = ln.File.filter(description="paradisi05").one()
             >>> file.load()
             PosixPath('/home/runner/work/lamindb/lamindb/docs/guide/mydata/.lamindb/jb7BY5UJoQVGMUOKiLcn.jpg')
         """
         pass
 
     def stage(self, is_run_input: Optional[bool] = None) -> Path:
         """Update cache from cloud storage if outdated.
@@ -1417,15 +1629,15 @@
         Returns a path to a locally cached on-disk object (say, a `.jpg` file).
 
         Examples:
 
             Sync file from cloud and returns the local path of the cache:
 
             >>> ln.File("s3://lamindb-ci/lndb-storage/pbmc68k.h5ad").save()
-            >>> file = ln.File.select(key="lndb-storage/pbmc68k.h5ad").one()
+            >>> file = ln.File.filter(key="lndb-storage/pbmc68k.h5ad").one()
             >>> file.stage()
             PosixPath('/home/runner/work/Caches/lamindb/lamindb-ci/lndb-storage/pbmc68k.h5ad')
         """
         pass
 
     def delete(self, storage: Optional[bool] = None) -> None:
         """Delete file, optionally from storage.
@@ -1449,29 +1661,35 @@
             >>> file = ln.File("./myfile.csv", key="myfile.csv")
             💡 File will be copied to storage upon `save()` using storage key = myfile.csv
             >>> file.save()
             💡 storing file 2fO9kSKVXFXYoLccExOY with key myfile.csv
         """
         pass
 
-    @property
-    def features(self):
-        """Feature manager (:class:`~lamindb.dev.FeatureManager`)."""
-        from lamindb._feature_manager import FeatureManager
 
-        return FeatureManager(self)
+class Dataset(Registry, Data):
+    """Dataset registry: collections of data batches.
+
+    .. warning::
+
+        The `Dataset` registry builds on all other registries and might change
+        in the future.
 
+        What's not going to change is that a dataset can both be stored in a
+        single file and sharded across several files.
 
-class Dataset(ORM):
-    """Datasets.
+    Args:
+        data: `DataLike` A data object (`DataFrame`, `AnnData`) to store.
+        name: `str` A name.
+        description: `Optional[str] = None` A description.
 
     Datasets are measurements of features (aka observations of variables).
 
     1. A feature can be a “high-level” feature with meaning: a labelled
-       column in a DataFrame with an entry in :class:`~lamindb.Feature` or another ORM.
+       column in a DataFrame with an entry in :class:`~lamindb.Feature` or another Registry.
        Examples: gene id, protein id, phenotype name, temperature,
        concentration, treatment label, treatment id, etc.
     2. In other cases, a feature might be a “low-level” feature without semantic
        meaning. Examples: pixels, single letters in sequences, etc.
 
     LaminDB typically stores datasets as one or multiple files (`.files`), either as
 
@@ -1485,15 +1703,15 @@
     One might also store a dataset in a SQL table or view, but this is *not* yet
     supported by LaminDB.
 
     See Also:
         :class:`~lamindb.File`
 
     Notes:
-        For more info, see tutorial: :doc:`/guide/tutorial1`.
+        For more info, see tutorial: :doc:`/tutorial1`.
 
     Examples:
         >>> df = ln.dev.datasets.df_iris_in_meter_batch1()
         >>> df.head()
           sepal_length sepal_width petal_length petal_width iris_species_code
         0        0.051       0.035        0.014       0.002                 0
         1        0.049       0.030        0.014       0.002                 0
@@ -1526,50 +1744,98 @@
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of run execution."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_datasets")
     """Creator of record, a :class:`~lamindb.User`."""
 
+    @overload
+    def __init__(
+        self,
+        data: Any,
+        name: str,
+        description: Optional[str] = None,
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
 
-class FileFeatureSet(ORM):
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        pass
+
+
+class LinkORM:
+    pass
+
+
+class FileFeatureSet(Registry, LinkORM):
     file = models.ForeignKey(File, on_delete=models.CASCADE)
-    featureset = models.ForeignKey(FeatureSet, on_delete=models.CASCADE)
+    feature_set = models.ForeignKey(FeatureSet, on_delete=models.CASCADE)
     slot = models.CharField(max_length=40, null=True, default=None)
 
     class Meta:
-        unique_together = ("file", "featureset")
+        unique_together = ("file", "feature_set")
 
 
-class DatasetFeatureSet(ORM):
+class DatasetFeatureSet(Registry, LinkORM):
     dataset = models.ForeignKey(Dataset, on_delete=models.CASCADE)
-    featureset = models.ForeignKey(FeatureSet, on_delete=models.CASCADE)
+    feature_set = models.ForeignKey(FeatureSet, on_delete=models.CASCADE)
     slot = models.CharField(max_length=50, null=True, default=None)
 
     class Meta:
-        unique_together = ("dataset", "featureset")
+        unique_together = ("dataset", "feature_set")
+
+
+class FileLabel(Registry, LinkORM):
+    file = models.ForeignKey(File, on_delete=models.CASCADE)
+    label = models.ForeignKey(Label, on_delete=models.CASCADE)
+    feature = models.ForeignKey(Feature, CASCADE, null=True, default=None)
+
+    class Meta:
+        unique_together = ("file", "label")
 
 
 # -------------------------------------------------------------------------------------
 # Low-level logic needed in lamindb-setup
 
 # Below is needed within lnschema-core because lamindb-setup already performs
 # some logging
 
 
-def format_datetime(dt: Union[datetime, Any]) -> str:
-    if not isinstance(dt, datetime):
-        return dt
+def format_field_value(value: Union[datetime, str, Any]) -> Any:
+    if isinstance(value, datetime):
+        return value.strftime("%Y-%m-%d %H:%M:%S")
+    elif isinstance(value, str):
+        return f"'{value}'"
     else:
-        return dt.strftime("%Y-%m-%d %H:%M:%S")
+        return value
 
 
-def __repr__(self: ORM) -> str:
+def __repr__(self: Registry) -> str:
     field_names = [field.name for field in self._meta.fields if (not isinstance(field, models.ForeignKey) and field.name != "created_at")]
     field_names += [f"{field.name}_id" for field in self._meta.fields if isinstance(field, models.ForeignKey)]
-    fields_str = {k: format_datetime(getattr(self, k)) for k in field_names if hasattr(self, k)}
+    fields_str = {k: format_field_value(getattr(self, k)) for k in field_names if hasattr(self, k)}
     fields_joined_str = ", ".join([f"{k}={fields_str[k]}" for k in fields_str if fields_str[k] is not None])
     return f"{self.__class__.__name__}({fields_joined_str})"
 
 
-ORM.__repr__ = __repr__  # type: ignore
-ORM.__str__ = __repr__  # type: ignore
+Registry.__repr__ = __repr__  # type: ignore
+Registry.__str__ = __repr__  # type: ignore
+
+# backward compat
+ORM = Registry
+
+
+def deferred_attribute__repr__(self):
+    return f"Field({self.field.model.__name__}.{self.field.name})"
+
+
+Field.__repr__ = deferred_attribute__repr__
```

### Comparing `lamindb_setup-0.49.4/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.49.5/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/lnschema-core/pyproject.toml` & `lamindb_setup-0.49.5/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/noxfile.py` & `lamindb_setup-0.49.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/pyproject.toml` & `lamindb_setup-0.49.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "lamindb_setup"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     "lnschema_core>=0.35.4",
-    "lamin_logger>=0.3.3",
+    "lamin_utils>=0.3.3",
     # External dependencies
     "django<5.0.0",
     "dj_database_url<3.0.0",
     "pydantic[dotenv]<2.0.0",
     "sqlalchemy<2.0.0",
     "appdirs<2.0.0",
     "python-dateutil<3.0.0",
```

### Comparing `lamindb_setup-0.49.4/tests/hub/test_instance.py` & `lamindb_setup-0.49.5/tests/hub/test_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/tests/hub/test_storage.py` & `lamindb_setup-0.49.5/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/tests/test_init_instance.py` & `lamindb_setup-0.49.5/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/tests/test_load_instance.py` & `lamindb_setup-0.49.5/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.4/PKG-INFO` & `lamindb_setup-0.49.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.49.4
+Version: 0.49.5
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
-Requires-Dist: lamin_logger>=0.3.3
+Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django<5.0.0
 Requires-Dist: dj_database_url<3.0.0
 Requires-Dist: pydantic[dotenv]<2.0.0
 Requires-Dist: sqlalchemy<2.0.0
 Requires-Dist: appdirs<2.0.0
 Requires-Dist: python-dateutil<3.0.0
 Requires-Dist: universal_pathlib==0.1.0
```

