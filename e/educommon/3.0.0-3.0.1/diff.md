# Comparing `tmp/educommon-3.0.0.tar.gz` & `tmp/educommon-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educommon-3.0.0.tar", last modified: Mon Jul 24 05:37:24 2023, max compression
+gzip compressed data, was "educommon-3.0.1.tar", last modified: Sun Aug  6 20:48:17 2023, max compression
```

## Comparing `educommon-3.0.0.tar` & `educommon-3.0.1.tar`

### file list

```diff
@@ -1,435 +1,435 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.812141 educommon-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-24 05:37:24.811141 educommon-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-3.0.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-3.0.0/UPGRADE.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 05:37:24.812141 educommon-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2023-07-24 05:37:11.000000 educommon-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.622141 educommon-3.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.639141 educommon-3.0.0/src/educommon/
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.642141 educommon-3.0.0/src/educommon/about/
--rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/README.rst
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/__init__.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.622141 educommon-3.0.0/src/educommon/about/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.643141 educommon-3.0.0/src/educommon/about/static/edu_about/
--rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/static/edu_about/barsgroup.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.649141 educommon-3.0.0/src/educommon/about/ui/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/about-window.js
--rw-r--r--   0 root         (0) root         (0)     5975 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/actions.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/common-tab.html
--rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/packages-tab.js
--rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/about/ui/postgresql-extensions-tab.js
--rw-r--r--   0 root         (0) root         (0)     5272 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/ui/ui.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/about/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.652141 educommon-3.0.0/src/educommon/async_tasks/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/apps.py
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.652141 educommon-3.0.0/src/educommon/async_tasks/fixtures/
--rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/async_tasks/fixtures/initial_data.json
--rw-r--r--   0 root         (0) root         (0)     3489 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/locks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.654141 educommon-3.0.0/src/educommon/async_tasks/migrations/
--rw-r--r--   0 root         (0) root         (0)     4205 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/0002_load_initial_data.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3539 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/models.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/statuses.py
--rw-r--r--   0 root         (0) root         (0)    11237 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/async_tasks/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.659141 educommon-3.0.0/src/educommon/audit_log/
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5980 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/apps.py
--rw-r--r--   0 root         (0) root         (0)      880 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.660141 educommon-3.0.0/src/educommon/audit_log/error_log/
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/error_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/error_log/actions.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.660141 educommon-3.0.0/src/educommon/audit_log/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.661141 educommon-3.0.0/src/educommon/audit_log/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.665141 educommon-3.0.0/src/educommon/audit_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     4461 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0002_install_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0003_logproxy.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0005_postgresql_error.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8173 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/models.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/permissions.py
--rw-r--r--   0 root         (0) root         (0)     8562 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/proxies.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/routers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.668141 educommon-3.0.0/src/educommon/audit_log/sql/
--rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/configure_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/sql/configure_selective_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/create_selective_tables_function.sql
--rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/audit_log/sql/install_audit_log.sql
--rw-r--r--   0 root         (0) root         (0)     2117 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.669141 educommon-3.0.0/src/educommon/audit_log/utils/
--rw-r--r--   0 root         (0) root         (0)    12533 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/audit_log/utils/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.669141 educommon-3.0.0/src/educommon/auth/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.672141 educommon-3.0.0/src/educommon/auth/rbac/
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26872 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/actions.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/app_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.673141 educommon-3.0.0/src/educommon/auth/rbac/backends/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/base.py
--rw-r--r--   0 root         (0) root         (0)    10290 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/caching.py
--rw-r--r--   0 root         (0) root         (0)     5038 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/backends/simple.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/checker.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/config.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.674141 educommon-3.0.0/src/educommon/auth/rbac/management/
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.674141 educommon-3.0.0/src/educommon/auth/rbac/management/commands/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/management/commands/rbac.py
--rw-r--r--   0 root         (0) root         (0)    16250 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.675141 educommon-3.0.0/src/educommon/auth/rbac/migrations/
--rw-r--r--   0 root         (0) root         (0)     5474 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
--rw-r--r--   0 root         (0) root         (0)      470 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15185 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/models.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.625141 educommon-3.0.0/src/educommon/auth/rbac/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.678141 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/
--rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-add-window.js
--rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
--rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
--rw-r--r--   0 root         (0) root         (0)    15735 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/ui.py
--rw-r--r--   0 root         (0) root         (0)     7819 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/utils.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/rbac/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.682141 educommon-3.0.0/src/educommon/auth/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11943 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/actions.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/checkers.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.683141 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.626141 educommon-3.0.0/src/educommon/auth/simple_auth/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.684141 educommon-3.0.0/src/educommon/auth/simple_auth/static/simple_auth/
--rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.626141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.686141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/
--rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.687141 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/
--rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
--rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
--rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
--rw-r--r--   0 root         (0) root         (0)     4620 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/ui.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/auth/simple_auth/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.690141 educommon-3.0.0/src/educommon/contingent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/actions.py
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     6854 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/base.py
--rw-r--r--   0 root         (0) root         (0)    60031 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/catalogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.695141 educommon-3.0.0/src/educommon/contingent/contingent_plugin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      717 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/actions.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.696141 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/
--rw-r--r--   0 root         (0) root         (0)     1594 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/model_views.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/models.py
--rw-r--r--   0 root         (0) root         (0)     5181 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/observer.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     3314 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/storage.py
--rw-r--r--   0 root         (0) root         (0)     7161 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/contingent/contingent_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.698141 educommon-3.0.0/src/educommon/contingent/json_data/
--rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/contingent/json_data/okogu.json
--rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/contingent/json_data/oksm.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.700141 educommon-3.0.0/src/educommon/django/
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.702141 educommon-3.0.0/src/educommon/django/db/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7049 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.703141 educommon-3.0.0/src/educommon/django/db/migration/
--rw-r--r--   0 root         (0) root         (0)     1882 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9527 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/migration/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.704141 educommon-3.0.0/src/educommon/django/db/mixins/
--rw-r--r--   0 root         (0) root         (0)    14740 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24715 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/date_interval.py
--rw-r--r--   0 root         (0) root         (0)    12225 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/mixins/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.705141 educommon-3.0.0/src/educommon/django/db/model_view/
--rw-r--r--   0 root         (0) root         (0)    12365 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/model_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/model_view/table-view.html
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/models.py
--rw-r--r--   0 root         (0) root         (0)    10990 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/observer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.710141 educommon-3.0.0/src/educommon/django/db/partitioning/
--rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/README.md
--rw-r--r--   0 root         (0) root         (0)    22378 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.712141 educommon-3.0.0/src/educommon/django/db/partitioning/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.714141 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/clear_table.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/split_table.py
--rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/partitioning.sql
--rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/db/partitioning/triggers.sql
--rw-r--r--   0 root         (0) root         (0)     3268 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/routers.py
--rw-r--r--   0 root         (0) root         (0)     9366 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.714141 educommon-3.0.0/src/educommon/django/db/validators/
--rw-r--r--   0 root         (0) root         (0)     1986 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38608 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/db/validators/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.715141 educommon-3.0.0/src/educommon/django/storages/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.719141 educommon-3.0.0/src/educommon/django/storages/atcfs/
--rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/README.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6004 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/api.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.720141 educommon-3.0.0/src/educommon/django/storages/atcfs/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.721141 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7416 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/models.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/monkey_patching.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/settings.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.721141 educommon-3.0.0/src/educommon/django/storages/atcfs/templates/
--rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.725141 educommon-3.0.0/src/educommon/extjs/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.725141 educommon-3.0.0/src/educommon/extjs/fields/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/extjs/fields/input_params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.731141 educommon-3.0.0/src/educommon/importer/
--rw-r--r--   0 root         (0) root         (0)    37531 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/XLSReader.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13402 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/api.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/constants.py
--rw-r--r--   0 root         (0) root         (0)    10270 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/loggers.py
--rw-r--r--   0 root         (0) root         (0)    37353 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/proxy_import.py
--rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/importer/refactoring-notes.txt
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/report.py
--rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/importer/test_file.xls
--rw-r--r--   0 root         (0) root         (0)     3918 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/ui.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/importer/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.733141 educommon-3.0.0/src/educommon/integration_entities/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/README.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/consts.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/entities.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/enums.py
--rw-r--r--   0 root         (0) root         (0)     8675 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/helpers.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/integration_entities/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.733141 educommon-3.0.0/src/educommon/ioc/
--rw-r--r--   0 root         (0) root         (0)     4028 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ioc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.735141 educommon-3.0.0/src/educommon/logger/
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/app_settings.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/apps.py
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/consts.py
--rw-r--r--   0 root         (0) root         (0)      400 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/formatters.py
--rw-r--r--   0 root         (0) root         (0)     1596 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/helpers.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/loggers.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/logger/records.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.736141 educommon-3.0.0/src/educommon/m3/
--rw-r--r--   0 root         (0) root         (0)    17570 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.736141 educommon-3.0.0/src/educommon/m3/extensions/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.737141 educommon-3.0.0/src/educommon/m3/extensions/listeners/
--rw-r--r--   0 root         (0) root         (0)     8897 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.740141 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
--rw-r--r--   0 root         (0) root         (0)     6200 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py
--rw-r--r--   0 root         (0) root         (0)     7660 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
--rw-r--r--   0 root         (0) root         (0)      467 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/signals.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/ui.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/utils.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/extensions/ui.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/m3/transaction_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.741141 educommon-3.0.0/src/educommon/objectpack/
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14320 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/actions.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.747141 educommon-3.0.0/src/educommon/objectpack/templates/
--rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/base-grid-window.js
--rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/filter-panel.js
--rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/grid-panel.js
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/multiSelectWindow.js
--rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/multiselect-page-fix.js
--rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/objectpack/templates/relations-check-mixin-template.html
--rw-r--r--   0 root         (0) root         (0)    14752 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/objectpack/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.748141 educommon-3.0.0/src/educommon/report/
--rw-r--r--   0 root         (0) root         (0)    17854 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8705 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.753141 educommon-3.0.0/src/educommon/report/constructor/
--rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/README.rst
--rw-r--r--   0 root         (0) root         (0)     1252 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/app_meta.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/apps.py
--rw-r--r--   0 root         (0) root         (0)    25938 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.754141 educommon-3.0.0/src/educommon/report/constructor/builders/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.755141 educommon-3.0.0/src/educommon/report/constructor/builders/excel/
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55790 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/_base.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/_header.py
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/constants.py
--rw-r--r--   0 root         (0) root         (0)     6229 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/product.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/config.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.759141 educommon-3.0.0/src/educommon/report/constructor/editor/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38811 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/actions.py
--rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/editor/edit-window.js
--rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/report/constructor/editor/list-window.js
--rw-r--r--   0 root         (0) root         (0)    24628 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/editor/ui.py
--rw-r--r--   0 root         (0) root         (0)     1287 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.762141 educommon-3.0.0/src/educommon/report/constructor/migrations/
--rw-r--r--   0 root         (0) root         (0)     3393 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0002_report_filters.py
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0006_reportsorting.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0007_include_available_units.py
--rw-r--r--   0 root         (0) root         (0)      557 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/mixins.py
--rw-r--r--   0 root         (0) root         (0)    18764 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/models.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/plugin_meta.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/registries.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/utils.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/constructor/validators.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/reporter.py
--rw-r--r--   0 root         (0) root         (0)     9974 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/report/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.763141 educommon-3.0.0/src/educommon/rest/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/actions.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/context.py
--rw-r--r--   0 root         (0) root         (0)     2516 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/controllers.py
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/misc.py
--rw-r--r--   0 root         (0) root         (0)     4840 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/rest/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.765141 educommon-3.0.0/src/educommon/secure_media/
--rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/secure_media/README.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/secure_media/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/secure_media/app_meta.py
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/thread_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.768141 educommon-3.0.0/src/educommon/utils/
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4066 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/caching.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/conversion.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)     9122 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/date.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.769141 educommon-3.0.0/src/educommon/utils/db/
--rw-r--r--   0 root         (0) root         (0)     7734 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/db/postgresql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.783141 educommon-3.0.0/src/educommon/utils/fonts/
--rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Arial.ttf
--rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Calibri.ttf
--rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/fonts/Tahoma.ttf
--rw-r--r--   0 root         (0) root         (0)     4815 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.783141 educommon-3.0.0/src/educommon/utils/licence/
--rw-r--r--   0 root         (0) root         (0)     5095 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/licence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/licence/converters.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     1157 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/patches.py
--rw-r--r--   0 root         (0) root         (0)     9469 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/plugins.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/registry.py
--rw-r--r--   0 root         (0) root         (0)      520 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/seqtools.py
--rw-r--r--   0 root         (0) root         (0)     8787 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/serializer.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/storage.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.784141 educommon-3.0.0/src/educommon/utils/system_app/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9297 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/management/commands/delete_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.785141 educommon-3.0.0/src/educommon/utils/system_app/templatetags/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      273 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/system_app/templatetags/educommon.py
--rw-r--r--   0 root         (0) root         (0)    14251 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.795141 educommon-3.0.0/src/educommon/utils/xml/
--rw-r--r--   0 root         (0) root         (0)     2194 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/xml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1750 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/utils/xml/resolver.py
--rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
--rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/xenc-schema.xsd
--rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/utils/xml/xmldsig-core-schema.xsd
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon/version.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.800141 educommon-3.0.0/src/educommon/ws_log/
--rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/README.rst
--rw-r--r--   0 root         (0) root         (0)      932 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9153 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/actions.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/app_meta.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.803141 educommon-3.0.0/src/educommon/ws_log/migrations/
--rw-r--r--   0 root         (0) root         (0)     2706 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5634 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/models.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/provider.py
--rw-r--r--   0 root         (0) root         (0)     3487 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.804141 educommon-3.0.0/src/educommon/ws_log/smev/
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/applications.py
--rw-r--r--   0 root         (0) root         (0)      601 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/smev/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.635141 educommon-3.0.0/src/educommon/ws_log/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.804141 educommon-3.0.0/src/educommon/ws_log/templates/report/
--rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/report/smev_logs.xlsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.807141 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/
--rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
--rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
--rw-r--r--   0 root         (0) root         (0)     4038 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/ui.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-07-24 05:37:11.000000 educommon-3.0.0/src/educommon/ws_log/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.640141 educommon-3.0.0/src/educommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15521 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-24 05:37:24.000000 educommon-3.0.0/src/educommon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 05:37:24.811141 educommon-3.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     6188 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_contingent_plugin_utils.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_delete_check.py
--rw-r--r--   0 root         (0) root         (0)     5018 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_delete_objects.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_django_db_utils.py
--rw-r--r--   0 root         (0) root         (0)    21544 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_interval_mixins.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_patches.py
--rw-r--r--   0 root         (0) root         (0)     7024 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_personal_data_fields.py
--rw-r--r--   0 root         (0) root         (0)    14369 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_report.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_service_db_router.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_utils_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8031 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/test_validators.py
--rw-r--r--   0 root         (0) root         (0)     5881 2023-07-24 05:37:11.000000 educommon-3.0.0/tests/tests_rbac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.834901 educommon-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-07-05 14:23:59.000000 educommon-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-06 20:48:17.833901 educommon-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2022-07-05 14:23:59.000000 educommon-3.0.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1981 2022-07-05 14:23:59.000000 educommon-3.0.1/UPGRADE.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 20:48:17.834901 educommon-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-08-06 20:48:04.000000 educommon-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.593901 educommon-3.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.615901 educommon-3.0.1/src/educommon/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.618901 educommon-3.0.1/src/educommon/about/
+-rw-r--r--   0 root         (0) root         (0)     2685 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/README.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.594901 educommon-3.0.1/src/educommon/about/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.619901 educommon-3.0.1/src/educommon/about/static/edu_about/
+-rw-r--r--   0 root         (0) root         (0)     8382 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/static/edu_about/barsgroup.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.631901 educommon-3.0.1/src/educommon/about/ui/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      535 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/ui/about-window.js
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/ui/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/ui/common-tab.html
+-rw-r--r--   0 root         (0) root         (0)    11192 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/ui/packages-tab.js
+-rw-r--r--   0 root         (0) root         (0)      129 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/about/ui/postgresql-extensions-tab.js
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/ui/ui.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/about/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.633901 educommon-3.0.1/src/educommon/async_tasks/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/apps.py
+-rw-r--r--   0 root         (0) root         (0)      251 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.634901 educommon-3.0.1/src/educommon/async_tasks/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      303 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/async_tasks/fixtures/initial_data.json
+-rw-r--r--   0 root         (0) root         (0)     3489 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/locks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.636901 educommon-3.0.1/src/educommon/async_tasks/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4205 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/migrations/0002_load_initial_data.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/models.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/statuses.py
+-rw-r--r--   0 root         (0) root         (0)    11237 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/async_tasks/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.640901 educommon-3.0.1/src/educommon/audit_log/
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/apps.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.640901 educommon-3.0.1/src/educommon/audit_log/error_log/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/error_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/error_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.640901 educommon-3.0.1/src/educommon/audit_log/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.641901 educommon-3.0.1/src/educommon/audit_log/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/management/commands/reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.643901 educommon-3.0.1/src/educommon/audit_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4461 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0002_install_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0003_logproxy.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0005_postgresql_error.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8173 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/models.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     8562 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/proxies.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/routers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.646901 educommon-3.0.1/src/educommon/audit_log/sql/
+-rw-r--r--   0 root         (0) root         (0)     1395 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/audit_log/sql/configure_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)      431 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/sql/configure_selective_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/audit_log/sql/create_selective_tables_function.sql
+-rw-r--r--   0 root         (0) root         (0)    14310 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/audit_log/sql/install_audit_log.sql
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.647901 educommon-3.0.1/src/educommon/audit_log/utils/
+-rw-r--r--   0 root         (0) root         (0)    12533 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/audit_log/utils/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.648901 educommon-3.0.1/src/educommon/auth/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.651901 educommon-3.0.1/src/educommon/auth/rbac/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26872 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/actions.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/app_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.652901 educommon-3.0.1/src/educommon/auth/rbac/backends/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/backends/caching.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/backends/simple.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/checker.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/config.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.652901 educommon-3.0.1/src/educommon/auth/rbac/management/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.653901 educommon-3.0.1/src/educommon/auth/rbac/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/management/commands/rbac.py
+-rw-r--r--   0 root         (0) root         (0)    16250 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.654901 educommon-3.0.1/src/educommon/auth/rbac/migrations/
+-rw-r--r--   0 root         (0) root         (0)     5474 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15185 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/models.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.597901 educommon-3.0.1/src/educommon/auth/rbac/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.660901 educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/
+-rw-r--r--   0 root         (0) root         (0)      335 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/role-add-window.js
+-rw-r--r--   0 root         (0) root         (0)     7914 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3768 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
+-rw-r--r--   0 root         (0) root         (0)      536 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
+-rw-r--r--   0 root         (0) root         (0)    15735 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/ui.py
+-rw-r--r--   0 root         (0) root         (0)     7819 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/utils.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/rbac/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.668901 educommon-3.0.1/src/educommon/auth/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11943 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/checkers.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.669901 educommon-3.0.1/src/educommon/auth/simple_auth/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.598901 educommon-3.0.1/src/educommon/auth/simple_auth/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.669901 educommon-3.0.1/src/educommon/auth/simple_auth/static/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)      123 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.599901 educommon-3.0.1/src/educommon/auth/simple_auth/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.673901 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/
+-rw-r--r--   0 root         (0) root         (0)     1577 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.678901 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/email/
+-rw-r--r--   0 root         (0) root         (0)      635 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
+-rw-r--r--   0 root         (0) root         (0)     1444 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/ui.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/auth/simple_auth/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.681901 educommon-3.0.1/src/educommon/contingent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/actions.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/base.py
+-rw-r--r--   0 root         (0) root         (0)    60031 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/catalogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.685901 educommon-3.0.1/src/educommon/contingent/contingent_plugin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/actions.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.686901 educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/model_views.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/models.py
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/observer.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/storage.py
+-rw-r--r--   0 root         (0) root         (0)     7161 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/contingent/contingent_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.692901 educommon-3.0.1/src/educommon/contingent/json_data/
+-rw-r--r--   0 root         (0) root         (0)    53540 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/contingent/json_data/okogu.json
+-rw-r--r--   0 root         (0) root         (0)    30723 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/contingent/json_data/oksm.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.694901 educommon-3.0.1/src/educommon/django/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.696901 educommon-3.0.1/src/educommon/django/db/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7049 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.696901 educommon-3.0.1/src/educommon/django/db/migration/
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9527 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/migration/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.697901 educommon-3.0.1/src/educommon/django/db/mixins/
+-rw-r--r--   0 root         (0) root         (0)    14740 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24715 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/mixins/date_interval.py
+-rw-r--r--   0 root         (0) root         (0)    12225 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/mixins/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.698901 educommon-3.0.1/src/educommon/django/db/model_view/
+-rw-r--r--   0 root         (0) root         (0)    12365 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/model_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/db/model_view/table-view.html
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/models.py
+-rw-r--r--   0 root         (0) root         (0)    10990 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.702901 educommon-3.0.1/src/educommon/django/db/partitioning/
+-rw-r--r--   0 root         (0) root         (0)     4455 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/db/partitioning/README.md
+-rw-r--r--   0 root         (0) root         (0)    22378 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.703901 educommon-3.0.1/src/educommon/django/db/partitioning/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.705901 educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/clear_table.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/split_table.py
+-rw-r--r--   0 root         (0) root         (0)    20345 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/db/partitioning/partitioning.sql
+-rw-r--r--   0 root         (0) root         (0)     3401 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/db/partitioning/triggers.sql
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/routers.py
+-rw-r--r--   0 root         (0) root         (0)     9366 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.705901 educommon-3.0.1/src/educommon/django/db/validators/
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38608 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/db/validators/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.706901 educommon-3.0.1/src/educommon/django/storages/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.710901 educommon-3.0.1/src/educommon/django/storages/atcfs/
+-rw-r--r--   0 root         (0) root         (0)     2656 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/api.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.710901 educommon-3.0.1/src/educommon/django/storages/atcfs/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.711901 educommon-3.0.1/src/educommon/django/storages/atcfs/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7416 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/models.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/monkey_patching.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/settings.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.711901 educommon-3.0.1/src/educommon/django/storages/atcfs/templates/
+-rw-r--r--   0 root         (0) root         (0)      196 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.712901 educommon-3.0.1/src/educommon/extjs/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/extjs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.712901 educommon-3.0.1/src/educommon/extjs/fields/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/extjs/fields/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/extjs/fields/input_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.722901 educommon-3.0.1/src/educommon/importer/
+-rw-r--r--   0 root         (0) root         (0)    37531 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/XLSReader.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13402 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/api.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/constants.py
+-rw-r--r--   0 root         (0) root         (0)    10270 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/loggers.py
+-rw-r--r--   0 root         (0) root         (0)    37353 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/proxy_import.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/importer/refactoring-notes.txt
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/report.py
+-rw-r--r--   0 root         (0) root         (0)     8704 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/importer/test_file.xls
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/importer/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.724901 educommon-3.0.1/src/educommon/integration_entities/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/consts.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/entities.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/enums.py
+-rw-r--r--   0 root         (0) root         (0)     8675 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/integration_entities/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.725901 educommon-3.0.1/src/educommon/ioc/
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ioc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.727901 educommon-3.0.1/src/educommon/logger/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/apps.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/consts.py
+-rw-r--r--   0 root         (0) root         (0)      400 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/formatters.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/logger/records.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.727901 educommon-3.0.1/src/educommon/m3/
+-rw-r--r--   0 root         (0) root         (0)    17570 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.728901 educommon-3.0.1/src/educommon/m3/extensions/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.728901 educommon-3.0.1/src/educommon/m3/extensions/listeners/
+-rw-r--r--   0 root         (0) root         (0)     8897 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.732901 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
+-rw-r--r--   0 root         (0) root         (0)     6200 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/listeners.py
+-rw-r--r--   0 root         (0) root         (0)     7660 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/mixins.py
+-rw-r--r--   0 root         (0) root         (0)       94 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
+-rw-r--r--   0 root         (0) root         (0)      467 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/signals.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/ui.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/extensions/ui.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/m3/transaction_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.734901 educommon-3.0.1/src/educommon/objectpack/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/objectpack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14320 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/objectpack/actions.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/objectpack/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.740901 educommon-3.0.1/src/educommon/objectpack/templates/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/base-grid-window.js
+-rw-r--r--   0 root         (0) root         (0)     1408 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/filter-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1544 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/grid-panel.js
+-rw-r--r--   0 root         (0) root         (0)     1842 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/multiSelectWindow.js
+-rw-r--r--   0 root         (0) root         (0)     6741 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/multiselect-page-fix.js
+-rw-r--r--   0 root         (0) root         (0)     1838 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/objectpack/templates/relations-check-mixin-template.html
+-rw-r--r--   0 root         (0) root         (0)    14752 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/objectpack/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.744901 educommon-3.0.1/src/educommon/report/
+-rw-r--r--   0 root         (0) root         (0)    17854 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8705 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.748901 educommon-3.0.1/src/educommon/report/constructor/
+-rw-r--r--   0 root         (0) root         (0)     1138 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/report/constructor/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/apps.py
+-rw-r--r--   0 root         (0) root         (0)    25938 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.749901 educommon-3.0.1/src/educommon/report/constructor/builders/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.750901 educommon-3.0.1/src/educommon/report/constructor/builders/excel/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55790 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/_header.py
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6229 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/product.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/builders/excel/with_merged_cells.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/config.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.756901 educommon-3.0.1/src/educommon/report/constructor/editor/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/editor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38811 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/editor/actions.py
+-rw-r--r--   0 root         (0) root         (0)    39225 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/report/constructor/editor/edit-window.js
+-rw-r--r--   0 root         (0) root         (0)     3247 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/report/constructor/editor/list-window.js
+-rw-r--r--   0 root         (0) root         (0)    24628 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/editor/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.759901 educommon-3.0.1/src/educommon/report/constructor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0002_report_filters.py
+-rw-r--r--   0 root         (0) root         (0)      472 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0006_reportsorting.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0007_include_available_units.py
+-rw-r--r--   0 root         (0) root         (0)      557 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    18764 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/models.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/plugin_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/registries.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/utils.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/constructor/validators.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/reporter.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/report/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.761901 educommon-3.0.1/src/educommon/rest/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/actions.py
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/context.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/controllers.py
+-rw-r--r--   0 root         (0) root         (0)      475 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4840 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/rest/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.763901 educommon-3.0.1/src/educommon/secure_media/
+-rw-r--r--   0 root         (0) root         (0)     4001 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/secure_media/README.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/secure_media/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/secure_media/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/thread_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.767901 educommon-3.0.1/src/educommon/utils/
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4066 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/caching.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/conversion.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/date.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.767901 educommon-3.0.1/src/educommon/utils/db/
+-rw-r--r--   0 root         (0) root         (0)     7734 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/db/postgresql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.801901 educommon-3.0.1/src/educommon/utils/fonts/
+-rw-r--r--   0 root         (0) root         (0)   275572 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/fonts/Arial.ttf
+-rw-r--r--   0 root         (0) root         (0)   811820 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/fonts/Calibri.ttf
+-rw-r--r--   0 root         (0) root         (0)   265528 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/fonts/Tahoma.ttf
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.802901 educommon-3.0.1/src/educommon/utils/licence/
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/licence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/licence/converters.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/patches.py
+-rw-r--r--   0 root         (0) root         (0)     9469 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/registry.py
+-rw-r--r--   0 root         (0) root         (0)      520 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/seqtools.py
+-rw-r--r--   0 root         (0) root         (0)     8787 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/storage.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.802901 educommon-3.0.1/src/educommon/utils/system_app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.802901 educommon-3.0.1/src/educommon/utils/system_app/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.803901 educommon-3.0.1/src/educommon/utils/system_app/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9297 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/management/commands/delete_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.804901 educommon-3.0.1/src/educommon/utils/system_app/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      273 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/system_app/templatetags/educommon.py
+-rw-r--r--   0 root         (0) root         (0)    14251 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.816901 educommon-3.0.1/src/educommon/utils/xml/
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/xml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/xml/catalog.json
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/utils/xml/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    13160 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)    13465 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
+-rw-r--r--   0 root         (0) root         (0)     5234 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/xml/xenc-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)    10293 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/utils/xml/xmldsig-core-schema.xsd
+-rw-r--r--   0 root         (0) root         (0)      448 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon/version.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.822901 educommon-3.0.1/src/educommon/ws_log/
+-rw-r--r--   0 root         (0) root         (0)     5467 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/ws_log/README.rst
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9153 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/actions.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/app_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.825901 educommon-3.0.1/src/educommon/ws_log/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/models.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/provider.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.825901 educommon-3.0.1/src/educommon/ws_log/smev/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/smev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/smev/applications.py
+-rw-r--r--   0 root         (0) root         (0)      601 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/smev/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.612901 educommon-3.0.1/src/educommon/ws_log/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.826901 educommon-3.0.1/src/educommon/ws_log/templates/report/
+-rw-r--r--   0 root         (0) root         (0)    10439 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/ws_log/templates/report/smev_logs.xlsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.829901 educommon-3.0.1/src/educommon/ws_log/templates/ui-js/
+-rw-r--r--   0 root         (0) root         (0)      513 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
+-rw-r--r--   0 root         (0) root         (0)     1103 2022-07-05 14:23:59.000000 educommon-3.0.1/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+-rw-r--r--   0 root         (0) root         (0)     4038 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/ui.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-08-06 20:48:04.000000 educommon-3.0.1/src/educommon/ws_log/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.617901 educommon-3.0.1/src/educommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      330 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-06 20:48:17.000000 educommon-3.0.1/src/educommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 20:48:17.833901 educommon-3.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_contingent_plugin_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_delete_check.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_delete_objects.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_django_db_utils.py
+-rw-r--r--   0 root         (0) root         (0)    21544 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_interval_mixins.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_patches.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_personal_data_fields.py
+-rw-r--r--   0 root         (0) root         (0)    14369 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_report.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_service_db_router.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_utils_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8031 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/test_validators.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2023-08-06 20:48:04.000000 educommon-3.0.1/tests/tests_rbac.py
```

### Comparing `educommon-3.0.0/PKG-INFO` & `educommon-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 3.0.0
+Version: 3.0.1
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-3.0.0/README.rst` & `educommon-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/UPGRADE.rst` & `educommon-3.0.1/UPGRADE.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/setup.py` & `educommon-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/README.rst` & `educommon-3.0.1/src/educommon/about/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/static/edu_about/barsgroup.png` & `educommon-3.0.1/src/educommon/about/static/edu_about/barsgroup.png`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/ui/about-window.js` & `educommon-3.0.1/src/educommon/about/ui/about-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/ui/actions.py` & `educommon-3.0.1/src/educommon/about/ui/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/ui/common-tab.html` & `educommon-3.0.1/src/educommon/about/ui/common-tab.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/ui/packages-tab.js` & `educommon-3.0.1/src/educommon/about/ui/packages-tab.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/ui/ui.py` & `educommon-3.0.1/src/educommon/about/ui/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/about/utils.py` & `educommon-3.0.1/src/educommon/about/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/async_tasks/locks.py` & `educommon-3.0.1/src/educommon/async_tasks/locks.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/async_tasks/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/async_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/async_tasks/models.py` & `educommon-3.0.1/src/educommon/async_tasks/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/async_tasks/statuses.py` & `educommon-3.0.1/src/educommon/async_tasks/statuses.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/async_tasks/tasks.py` & `educommon-3.0.1/src/educommon/async_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/__init__.py` & `educommon-3.0.1/src/educommon/audit_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/actions.py` & `educommon-3.0.1/src/educommon/audit_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/apps.py` & `educommon-3.0.1/src/educommon/audit_log/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/constants.py` & `educommon-3.0.1/src/educommon/audit_log/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/error_log/actions.py` & `educommon-3.0.1/src/educommon/audit_log/error_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/helpers.py` & `educommon-3.0.1/src/educommon/audit_log/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/management/commands/reinstall_audit_log.py` & `educommon-3.0.1/src/educommon/audit_log/management/commands/reinstall_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/middleware.py` & `educommon-3.0.1/src/educommon/audit_log/middleware.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/audit_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/migrations/0002_install_audit_log.py` & `educommon-3.0.1/src/educommon/audit_log/migrations/0002_install_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/migrations/0005_postgresql_error.py` & `educommon-3.0.1/src/educommon/audit_log/migrations/0005_postgresql_error.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py` & `educommon-3.0.1/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py` & `educommon-3.0.1/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/models.py` & `educommon-3.0.1/src/educommon/audit_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/permissions.py` & `educommon-3.0.1/src/educommon/audit_log/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/proxies.py` & `educommon-3.0.1/src/educommon/audit_log/proxies.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/sql/configure_audit_log.sql` & `educommon-3.0.1/src/educommon/audit_log/sql/configure_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/sql/create_selective_tables_function.sql` & `educommon-3.0.1/src/educommon/audit_log/sql/create_selective_tables_function.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/sql/install_audit_log.sql` & `educommon-3.0.1/src/educommon/audit_log/sql/install_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/ui.py` & `educommon-3.0.1/src/educommon/audit_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/utils/__init__.py` & `educommon-3.0.1/src/educommon/audit_log/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/audit_log/utils/operations.py` & `educommon-3.0.1/src/educommon/audit_log/utils/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/actions.py` & `educommon-3.0.1/src/educommon/auth/rbac/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/backends/base.py` & `educommon-3.0.1/src/educommon/auth/rbac/backends/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/backends/caching.py` & `educommon-3.0.1/src/educommon/auth/rbac/backends/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/backends/simple.py` & `educommon-3.0.1/src/educommon/auth/rbac/backends/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/checker.py` & `educommon-3.0.1/src/educommon/auth/rbac/checker.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/config.py` & `educommon-3.0.1/src/educommon/auth/rbac/config.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/management/commands/rbac.py` & `educommon-3.0.1/src/educommon/auth/rbac/management/commands/rbac.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/manager.py` & `educommon-3.0.1/src/educommon/auth/rbac/manager.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/auth/rbac/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py` & `educommon-3.0.1/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py` & `educommon-3.0.1/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/models.py` & `educommon-3.0.1/src/educommon/auth/rbac/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/permissions.py` & `educommon-3.0.1/src/educommon/auth/rbac/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/role-edit-window.js` & `educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/role-edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-list-window.js` & `educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/roles-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js` & `educommon-3.0.1/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/ui.py` & `educommon-3.0.1/src/educommon/auth/rbac/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/rbac/utils.py` & `educommon-3.0.1/src/educommon/auth/rbac/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/actions.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/app_meta.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/checkers.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/checkers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/models.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html` & `educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html` & `educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html` & `educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html` & `educommon-3.0.1/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/auth/simple_auth/ui.py` & `educommon-3.0.1/src/educommon/auth/simple_auth/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/actions.py` & `educommon-3.0.1/src/educommon/contingent/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/base.py` & `educommon-3.0.1/src/educommon/contingent/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/catalogs.py` & `educommon-3.0.1/src/educommon/contingent/catalogs.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/actions.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/apps.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/model_views.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/model_views.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/models.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/observer.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/storage.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/contingent_plugin/utils.py` & `educommon-3.0.1/src/educommon/contingent/contingent_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/json_data/okogu.json` & `educommon-3.0.1/src/educommon/contingent/json_data/okogu.json`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/contingent/json_data/oksm.json` & `educommon-3.0.1/src/educommon/contingent/json_data/oksm.json`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/fields.py` & `educommon-3.0.1/src/educommon/django/db/fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/migration/__init__.py` & `educommon-3.0.1/src/educommon/django/db/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/migration/operations.py` & `educommon-3.0.1/src/educommon/django/db/migration/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/mixins/__init__.py` & `educommon-3.0.1/src/educommon/django/db/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/mixins/date_interval.py` & `educommon-3.0.1/src/educommon/django/db/mixins/date_interval.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/mixins/validation.py` & `educommon-3.0.1/src/educommon/django/db/mixins/validation.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/model_view/__init__.py` & `educommon-3.0.1/src/educommon/django/db/model_view/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/model_view/table-view.html` & `educommon-3.0.1/src/educommon/django/db/model_view/table-view.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/models.py` & `educommon-3.0.1/src/educommon/django/db/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/observer.py` & `educommon-3.0.1/src/educommon/django/db/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/README.md` & `educommon-3.0.1/src/educommon/django/db/partitioning/README.md`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/__init__.py` & `educommon-3.0.1/src/educommon/django/db/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py` & `educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/clear_table.py` & `educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/clear_table.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/management/commands/split_table.py` & `educommon-3.0.1/src/educommon/django/db/partitioning/management/commands/split_table.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/partitioning.sql` & `educommon-3.0.1/src/educommon/django/db/partitioning/partitioning.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/partitioning/triggers.sql` & `educommon-3.0.1/src/educommon/django/db/partitioning/triggers.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/routers.py` & `educommon-3.0.1/src/educommon/django/db/routers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/utils.py` & `educommon-3.0.1/src/educommon/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/validators/__init__.py` & `educommon-3.0.1/src/educommon/django/db/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/db/validators/simple.py` & `educommon-3.0.1/src/educommon/django/db/validators/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/README.rst` & `educommon-3.0.1/src/educommon/django/storages/atcfs/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/api.py` & `educommon-3.0.1/src/educommon/django/storages/atcfs/api.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py` & `educommon-3.0.1/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/monkey_patching.py` & `educommon-3.0.1/src/educommon/django/storages/atcfs/monkey_patching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/settings.py` & `educommon-3.0.1/src/educommon/django/storages/atcfs/settings.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/django/storages/atcfs/storage.py` & `educommon-3.0.1/src/educommon/django/storages/atcfs/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/extjs/fields/input_params.py` & `educommon-3.0.1/src/educommon/extjs/fields/input_params.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/XLSReader.py` & `educommon-3.0.1/src/educommon/importer/XLSReader.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/api.py` & `educommon-3.0.1/src/educommon/importer/api.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/constants.py` & `educommon-3.0.1/src/educommon/importer/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/loggers.py` & `educommon-3.0.1/src/educommon/importer/loggers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/proxy.py` & `educommon-3.0.1/src/educommon/importer/proxy.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/proxy_import.py` & `educommon-3.0.1/src/educommon/importer/proxy_import.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/refactoring-notes.txt` & `educommon-3.0.1/src/educommon/importer/refactoring-notes.txt`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/report.py` & `educommon-3.0.1/src/educommon/importer/report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/test_file.xls` & `educommon-3.0.1/src/educommon/importer/test_file.xls`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/ui.py` & `educommon-3.0.1/src/educommon/importer/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/importer/validators.py` & `educommon-3.0.1/src/educommon/importer/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/integration_entities/entities.py` & `educommon-3.0.1/src/educommon/integration_entities/entities.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/integration_entities/helpers.py` & `educommon-3.0.1/src/educommon/integration_entities/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/integration_entities/mixins.py` & `educommon-3.0.1/src/educommon/integration_entities/mixins.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from typing import (
+    TYPE_CHECKING,
     List,
 )
 
 from django.utils.decorators import (
     classproperty,
 )
 
 
+if TYPE_CHECKING:
+    from m3_db_utils.models import (
+        ModelEnumValue,
+    )
+
+
 class EntitiesMixin:
     """
     Добавляет метод подготовки сущностей и свойства для доступа к ним.
     """
 
     # flake8: noqa: N805
     @classproperty
-    def first_entity(cls) -> str:
+    def first_entity(cls) -> 'ModelEnumValue':
         """
         Возвращает первый ключ модели-перечисления сущностей.
         """
         return cls._prepare_entities()[0]
 
     # flake8: noqa: N805
     @classproperty
-    def entities(cls) -> List[str]:
+    def entities(cls) -> List['ModelEnumValue']:
         """
         Возвращает ключи модели-перечисления сущностей.
         """
         return cls._prepare_entities()
 
     @classmethod
-    def _prepare_entities(cls) -> List[str]:
+    def _prepare_entities(cls) -> List['ModelEnumValue']:
         """
         Формирование списка ключей модели-перечисления сущностей.
         """
         return []
```

### Comparing `educommon-3.0.0/src/educommon/ioc/__init__.py` & `educommon-3.0.1/src/educommon/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/logger/__init__.py` & `educommon-3.0.1/src/educommon/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/logger/apps.py` & `educommon-3.0.1/src/educommon/logger/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/logger/helpers.py` & `educommon-3.0.1/src/educommon/logger/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/logger/loggers.py` & `educommon-3.0.1/src/educommon/logger/loggers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/__init__.py` & `educommon-3.0.1/src/educommon/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/__init__.py` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/listeners.py` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/listeners.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/mixins.py` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/ui.py` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/listeners/delete_check/utils.py` & `educommon-3.0.1/src/educommon/m3/extensions/listeners/delete_check/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/extensions/ui.py` & `educommon-3.0.1/src/educommon/m3/extensions/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/m3/transaction_context.py` & `educommon-3.0.1/src/educommon/m3/transaction_context.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/actions.py` & `educommon-3.0.1/src/educommon/objectpack/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/templates/filter-panel.js` & `educommon-3.0.1/src/educommon/objectpack/templates/filter-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/templates/grid-panel.js` & `educommon-3.0.1/src/educommon/objectpack/templates/grid-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/templates/multiSelectWindow.js` & `educommon-3.0.1/src/educommon/objectpack/templates/multiSelectWindow.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/templates/multiselect-page-fix.js` & `educommon-3.0.1/src/educommon/objectpack/templates/multiselect-page-fix.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/templates/relations-check-mixin-template.html` & `educommon-3.0.1/src/educommon/objectpack/templates/relations-check-mixin-template.html`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/objectpack/ui.py` & `educommon-3.0.1/src/educommon/objectpack/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/__init__.py` & `educommon-3.0.1/src/educommon/report/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/actions.py` & `educommon-3.0.1/src/educommon/report/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/README.rst` & `educommon-3.0.1/src/educommon/report/constructor/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/__init__.py` & `educommon-3.0.1/src/educommon/report/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/base.py` & `educommon-3.0.1/src/educommon/report/constructor/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/builders/excel/_base.py` & `educommon-3.0.1/src/educommon/report/constructor/builders/excel/_base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/builders/excel/_header.py` & `educommon-3.0.1/src/educommon/report/constructor/builders/excel/_header.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/builders/excel/product.py` & `educommon-3.0.1/src/educommon/report/constructor/builders/excel/product.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/builders/excel/with_merged_cells.py` & `educommon-3.0.1/src/educommon/report/constructor/builders/excel/with_merged_cells.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/config.py` & `educommon-3.0.1/src/educommon/report/constructor/config.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/constants.py` & `educommon-3.0.1/src/educommon/report/constructor/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/editor/actions.py` & `educommon-3.0.1/src/educommon/report/constructor/editor/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/editor/edit-window.js` & `educommon-3.0.1/src/educommon/report/constructor/editor/edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/editor/list-window.js` & `educommon-3.0.1/src/educommon/report/constructor/editor/list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/editor/ui.py` & `educommon-3.0.1/src/educommon/report/constructor/editor/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/exceptions.py` & `educommon-3.0.1/src/educommon/report/constructor/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0002_report_filters.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0002_report_filters.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0006_reportsorting.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0006_reportsorting.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0007_include_available_units.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0007_include_available_units.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py` & `educommon-3.0.1/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/mixins.py` & `educommon-3.0.1/src/educommon/report/constructor/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/models.py` & `educommon-3.0.1/src/educommon/report/constructor/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/registries.py` & `educommon-3.0.1/src/educommon/report/constructor/registries.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/utils.py` & `educommon-3.0.1/src/educommon/report/constructor/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/constructor/validators.py` & `educommon-3.0.1/src/educommon/report/constructor/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/reporter.py` & `educommon-3.0.1/src/educommon/report/reporter.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/report/utils.py` & `educommon-3.0.1/src/educommon/report/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/rest/actions.py` & `educommon-3.0.1/src/educommon/rest/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/rest/context.py` & `educommon-3.0.1/src/educommon/rest/context.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/rest/controllers.py` & `educommon-3.0.1/src/educommon/rest/controllers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/rest/mixins.py` & `educommon-3.0.1/src/educommon/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/secure_media/README.rst` & `educommon-3.0.1/src/educommon/secure_media/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/secure_media/app_meta.py` & `educommon-3.0.1/src/educommon/secure_media/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/__init__.py` & `educommon-3.0.1/src/educommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/caching.py` & `educommon-3.0.1/src/educommon/utils/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/conversion.py` & `educommon-3.0.1/src/educommon/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/crypto.py` & `educommon-3.0.1/src/educommon/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/date.py` & `educommon-3.0.1/src/educommon/utils/date.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/db/__init__.py` & `educommon-3.0.1/src/educommon/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/db/postgresql.py` & `educommon-3.0.1/src/educommon/utils/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/fonts/Arial.ttf` & `educommon-3.0.1/src/educommon/utils/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/fonts/Calibri.ttf` & `educommon-3.0.1/src/educommon/utils/fonts/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/fonts/Tahoma.ttf` & `educommon-3.0.1/src/educommon/utils/fonts/Tahoma.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/fonts/__init__.py` & `educommon-3.0.1/src/educommon/utils/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/licence/__init__.py` & `educommon-3.0.1/src/educommon/utils/licence/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/licence/converters.py` & `educommon-3.0.1/src/educommon/utils/licence/converters.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/misc.py` & `educommon-3.0.1/src/educommon/utils/misc.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/patches.py` & `educommon-3.0.1/src/educommon/utils/patches.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/plugins.py` & `educommon-3.0.1/src/educommon/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/registry.py` & `educommon-3.0.1/src/educommon/utils/registry.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/seqtools.py` & `educommon-3.0.1/src/educommon/utils/seqtools.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/serializer.py` & `educommon-3.0.1/src/educommon/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/storage.py` & `educommon-3.0.1/src/educommon/utils/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/system.py` & `educommon-3.0.1/src/educommon/utils/system.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/system_app/management/commands/delete_objects.py` & `educommon-3.0.1/src/educommon/utils/system_app/management/commands/delete_objects.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/ui.py` & `educommon-3.0.1/src/educommon/utils/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/__init__.py` & `educommon-3.0.1/src/educommon/utils/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/catalog.json` & `educommon-3.0.1/src/educommon/utils/xml/catalog.json`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/resolver.py` & `educommon-3.0.1/src/educommon/utils/xml/resolver.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd` & `educommon-3.0.1/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd` & `educommon-3.0.1/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/xenc-schema.xsd` & `educommon-3.0.1/src/educommon/utils/xml/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/utils/xml/xmldsig-core-schema.xsd` & `educommon-3.0.1/src/educommon/utils/xml/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/README.rst` & `educommon-3.0.1/src/educommon/ws_log/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/__init__.py` & `educommon-3.0.1/src/educommon/ws_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/actions.py` & `educommon-3.0.1/src/educommon/ws_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/base.py` & `educommon-3.0.1/src/educommon/ws_log/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0001_initial.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py` & `educommon-3.0.1/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/models.py` & `educommon-3.0.1/src/educommon/ws_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/provider.py` & `educommon-3.0.1/src/educommon/ws_log/provider.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/report.py` & `educommon-3.0.1/src/educommon/ws_log/report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/smev/applications.py` & `educommon-3.0.1/src/educommon/ws_log/smev/applications.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/smev/exceptions.py` & `educommon-3.0.1/src/educommon/ws_log/smev/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/templates/report/smev_logs.xlsx` & `educommon-3.0.1/src/educommon/ws_log/templates/report/smev_logs.xlsx`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js` & `educommon-3.0.1/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js` & `educommon-3.0.1/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/ui.py` & `educommon-3.0.1/src/educommon/ws_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon/ws_log/utils.py` & `educommon-3.0.1/src/educommon/ws_log/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/src/educommon.egg-info/PKG-INFO` & `educommon-3.0.1/src/educommon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 3.0.0
+Version: 3.0.1
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-3.0.0/src/educommon.egg-info/SOURCES.txt` & `educommon-3.0.1/src/educommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_contingent_plugin_utils.py` & `educommon-3.0.1/tests/test_contingent_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_delete_check.py` & `educommon-3.0.1/tests/test_delete_check.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_delete_objects.py` & `educommon-3.0.1/tests/test_delete_objects.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_django_db_utils.py` & `educommon-3.0.1/tests/test_django_db_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_interval_mixins.py` & `educommon-3.0.1/tests/test_interval_mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_patches.py` & `educommon-3.0.1/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_personal_data_fields.py` & `educommon-3.0.1/tests/test_personal_data_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_report.py` & `educommon-3.0.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_service_db_router.py` & `educommon-3.0.1/tests/test_service_db_router.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_utils.py` & `educommon-3.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_utils_plugins.py` & `educommon-3.0.1/tests/test_utils_plugins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/test_validators.py` & `educommon-3.0.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.0.0/tests/tests_rbac.py` & `educommon-3.0.1/tests/tests_rbac.py`

 * *Files identical despite different names*

