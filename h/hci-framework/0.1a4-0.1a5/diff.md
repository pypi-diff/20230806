# Comparing `tmp/hci-framework-0.1a4.tar.gz` & `tmp/hci-framework-0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hci-framework-0.1a4.tar", last modified: Tue Aug  1 03:15:24 2023, max compression
+gzip compressed data, was "hci-framework-0.1a5.tar", last modified: Sun Aug  6 02:19:59 2023, max compression
```

## Comparing `hci-framework-0.1a4.tar` & `hci-framework-0.1a5.tar`

### file list

```diff
@@ -1,753 +1,759 @@
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.068163 hci-framework-0.1a4/
--rw-r--r--   0 yeison    (1000) users      (984)     1321 2021-07-29 02:00:34.000000 hci-framework-0.1a4/LICENSE
--rw-r--r--   0 yeison    (1000) users      (984)      229 2023-07-16 01:05:40.000000 hci-framework-0.1a4/MANIFEST.in
--rw-r--r--   0 yeison    (1000) users      (984)     1366 2023-08-01 03:15:24.068163 hci-framework-0.1a4/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)       16 2023-07-16 01:07:26.000000 hci-framework-0.1a4/README.md
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-07-16 00:31:29.000000 hci-framework-0.1a4/hci_framework/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/hci_framework/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/__init__.py
--rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/asgi.py
--rw-r--r--   0 yeison    (1000) users      (984)     3242 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/settings.py
--rw-r--r--   0 yeison    (1000) users      (984)      755 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/urls.py
--rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/wsgi.py
--rwxr-xr-x   0 yeison    (1000) users      (984)      669 2023-06-22 22:07:41.000000 hci-framework-0.1a4/hci_framework/hci_framework/manage.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/radiant/
--rw-r--r--   0 yeison    (1000) users      (984)        2 2023-07-09 21:08:21.000000 hci-framework-0.1a4/hci_framework/radiant/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.004829 hci-framework-0.1a4/hci_framework/radiant/brython/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/__init__.py
--rw-r--r--   0 yeison    (1000) users      (984)     1737 2023-07-10 00:34:54.000000 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/figurestream.py
--rw-r--r--   0 yeison    (1000) users      (984)      245 2023-07-09 23:50:50.000000 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/server.py
--rw-r--r--   0 yeison    (1000) users      (984)       57 2023-07-09 21:07:45.000000 hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/utils.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/radiant/python_tools/
--rw-r--r--   0 yeison    (1000) users      (984)      402 2023-08-01 02:58:23.000000 hci-framework-0.1a4/hci_framework/radiant/python_tools/python_logger.py
--rw-r--r--   0 yeison    (1000) users      (984)      853 2023-08-01 03:12:35.000000 hci-framework-0.1a4/hci_framework/radiant/python_tools/python_swarm.py
--rw-r--r--   0 yeison    (1000) users      (984)     3257 2023-08-01 03:13:57.000000 hci-framework-0.1a4/hci_framework/radiant/server.py
--rw-r--r--   0 yeison    (1000) users      (984)      306 2023-08-01 02:26:57.000000 hci-framework-0.1a4/hci_framework/radiant/template.html
--rw-r--r--   0 yeison    (1000) users      (984)       56 2023-07-09 21:07:01.000000 hci-framework-0.1a4/hci_framework/radiant/utils.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/utils/
--rw-r--r--   0 yeison    (1000) users      (984)       54 2023-07-23 22:33:21.000000 hci-framework-0.1a4/hci_framework/utils/__init__.py
--rw-r--r--   0 yeison    (1000) users      (984)     1037 2023-07-30 21:22:16.000000 hci-framework-0.1a4/hci_framework/utils/kafkalogs.py
--rw-r--r--   0 yeison    (1000) users      (984)     9820 2023-07-30 20:09:40.000000 hci-framework-0.1a4/hci_framework/utils/swarm.py
--rw-r--r--   0 yeison    (1000) users      (984)     9692 2023-07-31 01:05:02.000000 hci-framework-0.1a4/hci_framework/utils/workers.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/workers/
--rw-r--r--   0 yeison    (1000) users      (984)      182 2023-07-16 00:36:22.000000 hci-framework-0.1a4/hci_framework/workers/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/django_worker/
--rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-22 00:12:49.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/db.sqlite3
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/django_worker/djangoship/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangoship/access.log
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangoship/error.log
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/
--rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:08:17.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/__init__.py
--rwxr-xr-x   0 yeison    (1000) users      (984)      397 2023-07-21 23:08:17.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/asgi.py
--rwxr-xr-x   0 yeison    (1000) users      (984)     3233 2023-07-21 23:08:17.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/settings.py
--rwxr-xr-x   0 yeison    (1000) users      (984)      766 2023-07-21 23:08:17.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/urls.py
--rwxr-xr-x   0 yeison    (1000) users      (984)      485 2023-07-22 00:19:20.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/wsgi.py
--rwxr-xr-x   0 yeison    (1000) users      (984)      666 2023-07-21 23:08:17.000000 hci-framework-0.1a4/hci_framework/workers/django_worker/manage.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/
--rw-r--r--   0 yeison    (1000) users      (984)     1510 2023-07-10 00:37:51.000000 hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/main.py
--rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-01 02:06:44.000000 hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/requirements.txt
--rwxr-xr-x   0 yeison    (1000) users      (984)     1480 2023-07-09 23:24:03.000000 hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/stream.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/figurestream_worker/
--rwxr-xr-x   0 yeison    (1000) users      (984)     1194 2023-07-31 01:58:18.000000 hci-framework-0.1a4/hci_framework/workers/figurestream_worker/main.py
--rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-01 02:06:42.000000 hci-framework-0.1a4/hci_framework/workers/figurestream_worker/requirements.txt
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/main_app/
--rw-r--r--   0 yeison    (1000) users      (984)     1146 2023-08-01 03:13:18.000000 hci-framework-0.1a4/hci_framework/workers/main_app/main.py
--rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-01 03:02:50.000000 hci-framework-0.1a4/hci_framework/workers/main_app/requirements.txt
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/python_logs/
--rw-r--r--   0 yeison    (1000) users      (984)      172 2023-07-31 00:52:13.000000 hci-framework-0.1a4/hci_framework/workers/python_logs/main.py
--rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-01 02:06:28.000000 hci-framework-0.1a4/hci_framework/workers/python_logs/requirements.txt
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/
--rw-r--r--   0 yeison    (1000) users      (984)   131072 2023-07-27 02:19:49.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/db.sqlite3
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/djangoship/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:49.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/djangoship/access.log
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:49.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/djangoship/error.log
--rwxr-xr-x   0 yeison    (1000) users      (984)      671 2023-07-22 20:40:50.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/manage.py
--rw-r--r--   0 yeison    (1000) users      (984)      182 2023-07-22 22:50:08.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/requirements.txt
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.011496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.004829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.014829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/
--rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css
--rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css
--rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    21357 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css
--rw-r--r--   0 yeison    (1000) users      (984)     4847 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    21207 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.css
--rw-r--r--   0 yeison    (1000) users      (984)     4737 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css
--rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css
--rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css
--rw-r--r--   0 yeison    (1000) users      (984)      849 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css
--rw-r--r--   0 yeison    (1000) users      (984)      849 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.css
--rw-r--r--   0 yeison    (1000) users      (984)      267 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css
--rw-r--r--   0 yeison    (1000) users      (984)      267 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     9090 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css
--rw-r--r--   0 yeison    (1000) users      (984)     2236 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     9047 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css
--rw-r--r--   0 yeison    (1000) users      (984)     2199 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      958 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css
--rw-r--r--   0 yeison    (1000) users      (984)      417 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      958 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.css
--rw-r--r--   0 yeison    (1000) users      (984)      417 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css
--rw-r--r--   0 yeison    (1000) users      (984)      779 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css
--rw-r--r--   0 yeison    (1000) users      (984)      779 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css
--rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css
--rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css
--rw-r--r--   0 yeison    (1000) users      (984)      527 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css
--rw-r--r--   0 yeison    (1000) users      (984)      527 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     4878 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css
--rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     4788 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css
--rw-r--r--   0 yeison    (1000) users      (984)     1229 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.004829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.014829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/
--rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md
--rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md
--rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md.gz
--rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css
--rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css
--rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css
--rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css
--rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    12110 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css
--rw-r--r--   0 yeison    (1000) users      (984)     2561 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    11900 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css
--rw-r--r--   0 yeison    (1000) users      (984)     2468 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.021496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/
--rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE
--rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c
--rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c.gz
--rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.gz
--rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt
--rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/README.txt
--rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/README.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg
--rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg
--rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.024829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/
--rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg
--rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg
--rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg
--rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.svg
--rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg
--rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.svg
--rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg
--rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg
--rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg
--rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.svg
--rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg
--rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg
--rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg
--rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg
--rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg
--rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg
--rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg
--rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg
--rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg
--rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg
--rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg
--rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg
--rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg
--rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.svg
--rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg
--rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg
--rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg
--rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/search.svg
--rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/search.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg
--rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg
--rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg
--rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg
--rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg
--rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.svg
--rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg
--rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg
--rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.028162 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/
--rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js
--rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js
--rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js
--rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js
--rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js
--rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js
--rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.028162 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/
--rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js
--rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js
--rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js
--rw-r--r--   0 yeison    (1000) users      (984)      425 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js
--rw-r--r--   0 yeison    (1000) users      (984)      425 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js
--rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js
--rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      884 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js
--rw-r--r--   0 yeison    (1000) users      (984)      430 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      884 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js
--rw-r--r--   0 yeison    (1000) users      (984)      430 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      606 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js
--rw-r--r--   0 yeison    (1000) users      (984)      322 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      606 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js
--rw-r--r--   0 yeison    (1000) users      (984)      322 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js
--rw-r--r--   0 yeison    (1000) users      (984)      614 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js
--rw-r--r--   0 yeison    (1000) users      (984)      614 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js
--rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.js
--rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      978 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js
--rw-r--r--   0 yeison    (1000) users      (984)      502 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      978 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js
--rw-r--r--   0 yeison    (1000) users      (984)      502 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js
--rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js
--rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      347 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js
--rw-r--r--   0 yeison    (1000) users      (984)      236 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      347 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.js
--rw-r--r--   0 yeison    (1000) users      (984)      236 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js
--rw-r--r--   0 yeison    (1000) users      (984)      845 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js
--rw-r--r--   0 yeison    (1000) users      (984)      845 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js
--rw-r--r--   0 yeison    (1000) users      (984)      270 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js
--rw-r--r--   0 yeison    (1000) users      (984)      270 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js
--rw-r--r--   0 yeison    (1000) users      (984)      536 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js
--rw-r--r--   0 yeison    (1000) users      (984)      536 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      586 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js
--rw-r--r--   0 yeison    (1000) users      (984)      277 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      586 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js
--rw-r--r--   0 yeison    (1000) users      (984)      277 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js
--rw-r--r--   0 yeison    (1000) users      (984)      605 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js
--rw-r--r--   0 yeison    (1000) users      (984)      605 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js
--rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js
--rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.004829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.031496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/
--rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt
--rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt
--rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js
--rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js
--rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js
--rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js
--rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.031496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/
--rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md
--rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md
--rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.051496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/
--rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js
--rw-r--r--   0 yeison    (1000) users      (984)      460 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js
--rw-r--r--   0 yeison    (1000) users      (984)      460 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      905 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js
--rw-r--r--   0 yeison    (1000) users      (984)      498 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      905 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js
--rw-r--r--   0 yeison    (1000) users      (984)      498 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      721 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js
--rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      721 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js
--rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      968 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js
--rw-r--r--   0 yeison    (1000) users      (984)      541 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      968 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js
--rw-r--r--   0 yeison    (1000) users      (984)      541 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js
--rw-r--r--   0 yeison    (1000) users      (984)      553 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js
--rw-r--r--   0 yeison    (1000) users      (984)      553 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      965 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js
--rw-r--r--   0 yeison    (1000) users      (984)      523 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      965 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js
--rw-r--r--   0 yeison    (1000) users      (984)      523 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js
--rw-r--r--   0 yeison    (1000) users      (984)      623 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js
--rw-r--r--   0 yeison    (1000) users      (984)      623 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      828 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js
--rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      828 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js
--rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js
--rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js
--rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js
--rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js
--rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js
--rw-r--r--   0 yeison    (1000) users      (984)      644 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js
--rw-r--r--   0 yeison    (1000) users      (984)      644 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      844 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js
--rw-r--r--   0 yeison    (1000) users      (984)      447 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      844 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js
--rw-r--r--   0 yeison    (1000) users      (984)      447 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      922 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js
--rw-r--r--   0 yeison    (1000) users      (984)      474 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      922 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js
--rw-r--r--   0 yeison    (1000) users      (984)      474 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      801 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js
--rw-r--r--   0 yeison    (1000) users      (984)      432 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      801 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js
--rw-r--r--   0 yeison    (1000) users      (984)      432 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      868 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js
--rw-r--r--   0 yeison    (1000) users      (984)      450 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      868 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js
--rw-r--r--   0 yeison    (1000) users      (984)      450 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js
--rw-r--r--   0 yeison    (1000) users      (984)      538 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js
--rw-r--r--   0 yeison    (1000) users      (984)      538 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      803 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js
--rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      803 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js
--rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js
--rw-r--r--   0 yeison    (1000) users      (984)      484 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js
--rw-r--r--   0 yeison    (1000) users      (984)      484 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js
--rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js
--rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      984 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js
--rw-r--r--   0 yeison    (1000) users      (984)      518 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      984 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js
--rw-r--r--   0 yeison    (1000) users      (984)      518 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js
--rw-r--r--   0 yeison    (1000) users      (984)      572 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js
--rw-r--r--   0 yeison    (1000) users      (984)      572 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      852 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js
--rw-r--r--   0 yeison    (1000) users      (984)      477 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      852 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js
--rw-r--r--   0 yeison    (1000) users      (984)      477 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js
--rw-r--r--   0 yeison    (1000) users      (984)      556 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js
--rw-r--r--   0 yeison    (1000) users      (984)      556 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      831 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js
--rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      831 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js
--rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js
--rw-r--r--   0 yeison    (1000) users      (984)      530 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js
--rw-r--r--   0 yeison    (1000) users      (984)      530 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js
--rw-r--r--   0 yeison    (1000) users      (984)      416 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js
--rw-r--r--   0 yeison    (1000) users      (984)      416 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      807 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js
--rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      807 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js
--rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      897 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js
--rw-r--r--   0 yeison    (1000) users      (984)      488 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      897 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js
--rw-r--r--   0 yeison    (1000) users      (984)      488 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      862 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js
--rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      862 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js
--rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js
--rw-r--r--   0 yeison    (1000) users      (984)      533 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js
--rw-r--r--   0 yeison    (1000) users      (984)      533 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js
--rw-r--r--   0 yeison    (1000) users      (984)      540 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js
--rw-r--r--   0 yeison    (1000) users      (984)      540 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      855 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js
--rw-r--r--   0 yeison    (1000) users      (984)      506 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      855 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js
--rw-r--r--   0 yeison    (1000) users      (984)      506 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      944 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js
--rw-r--r--   0 yeison    (1000) users      (984)      521 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      944 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js
--rw-r--r--   0 yeison    (1000) users      (984)      521 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js
--rw-r--r--   0 yeison    (1000) users      (984)      505 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js
--rw-r--r--   0 yeison    (1000) users      (984)      505 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js
--rw-r--r--   0 yeison    (1000) users      (984)      557 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js
--rw-r--r--   0 yeison    (1000) users      (984)      557 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      811 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js
--rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      811 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js
--rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      778 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js
--rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      778 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js
--rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js
--rw-r--r--   0 yeison    (1000) users      (984)      591 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js
--rw-r--r--   0 yeison    (1000) users      (984)      591 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      904 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js
--rw-r--r--   0 yeison    (1000) users      (984)      469 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      904 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js
--rw-r--r--   0 yeison    (1000) users      (984)      469 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      947 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js
--rw-r--r--   0 yeison    (1000) users      (984)      524 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      947 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js
--rw-r--r--   0 yeison    (1000) users      (984)      524 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js
--rw-r--r--   0 yeison    (1000) users      (984)      587 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js
--rw-r--r--   0 yeison    (1000) users      (984)      587 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      876 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js
--rw-r--r--   0 yeison    (1000) users      (984)      486 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      876 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js
--rw-r--r--   0 yeison    (1000) users      (984)      486 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      878 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      878 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js
--rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      938 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js
--rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      938 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js
--rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js
--rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js
--rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js
--rw-r--r--   0 yeison    (1000) users      (984)      617 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js
--rw-r--r--   0 yeison    (1000) users      (984)      617 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      925 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js
--rw-r--r--   0 yeison    (1000) users      (984)      487 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      925 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js
--rw-r--r--   0 yeison    (1000) users      (984)      487 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      903 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js
--rw-r--r--   0 yeison    (1000) users      (984)      490 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      903 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js
--rw-r--r--   0 yeison    (1000) users      (984)      490 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js
--rw-r--r--   0 yeison    (1000) users      (984)      608 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rw-r--r--   0 yeison    (1000) users      (984)      608 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      980 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js
--rw-r--r--   0 yeison    (1000) users      (984)      552 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      980 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js
--rw-r--r--   0 yeison    (1000) users      (984)      552 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      786 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js
--rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      786 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js
--rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js
--rw-r--r--   0 yeison    (1000) users      (984)      515 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js
--rw-r--r--   0 yeison    (1000) users      (984)      515 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      771 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js
--rw-r--r--   0 yeison    (1000) users      (984)      434 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      771 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js
--rw-r--r--   0 yeison    (1000) users      (984)      434 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      775 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js
--rw-r--r--   0 yeison    (1000) users      (984)      423 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      775 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js
--rw-r--r--   0 yeison    (1000) users      (984)      423 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js
--rw-r--r--   0 yeison    (1000) users      (984)      626 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js
--rw-r--r--   0 yeison    (1000) users      (984)      626 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      796 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js
--rw-r--r--   0 yeison    (1000) users      (984)      479 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      796 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js
--rw-r--r--   0 yeison    (1000) users      (984)      479 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js
--rw-r--r--   0 yeison    (1000) users      (984)      468 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js
--rw-r--r--   0 yeison    (1000) users      (984)      468 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      707 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js
--rw-r--r--   0 yeison    (1000) users      (984)      451 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)      707 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js
--rw-r--r--   0 yeison    (1000) users      (984)      451 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js
--rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js
--rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js
--rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js
--rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.051496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/
--rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt
--rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt
--rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt.gz
--rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js
--rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js
--rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js
--rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.054829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/
--rw-r--r--   0 yeison    (1000) users      (984)      753 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css
--rw-r--r--   0 yeison    (1000) users      (984)      452 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      740 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css
--rw-r--r--   0 yeison    (1000) users      (984)      440 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.054829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/img/
--rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.03ce3dcc84af.gif
--rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.gif
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.054829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/
--rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js
--rw-r--r--   0 yeison    (1000) users      (984)      960 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js
--rw-r--r--   0 yeison    (1000) users      (984)      960 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js
--rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js
--rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js
--rw-r--r--   0 yeison    (1000) users      (984)      814 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js
--rw-r--r--   0 yeison    (1000) users      (984)      814 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.058163 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/
--rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css
--rw-r--r--   0 yeison    (1000) users      (984)     2783 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    23411 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css
--rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map
--rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2772 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map
--rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3398 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css
--rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3385 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css
--rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)   121457 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css
--rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map
--rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map.gz
--rw-r--r--   0 yeison    (1000) users      (984)    19586 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map
--rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map.gz
--rw-r--r--   0 yeison    (1000) users      (984)   121560 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css
--rw-r--r--   0 yeison    (1000) users      (984)    19657 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css
--rw-r--r--   0 yeison    (1000) users      (984)      612 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css
--rw-r--r--   0 yeison    (1000) users      (984)      612 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    21723 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css
--rw-r--r--   0 yeison    (1000) users      (984)     4230 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)    21658 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css
--rw-r--r--   0 yeison    (1000) users      (984)     4186 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      817 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css
--rw-r--r--   0 yeison    (1000) users      (984)      390 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)      817 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css
--rw-r--r--   0 yeison    (1000) users      (984)      390 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.058163 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/
--rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css
--rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css
--rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css
--rw-r--r--   0 yeison    (1000) users      (984)      671 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css
--rw-r--r--   0 yeison    (1000) users      (984)      671 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css
--rw-r--r--   0 yeison    (1000) users      (984)      640 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css
--rw-r--r--   0 yeison    (1000) users      (984)      640 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.058163 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/
--rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico
--rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico.gz
--rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico
--rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.a4b938cf382b.png
--rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.png
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.061496 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/
--rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js
--rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js
--rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js
--rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js
--rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js
--rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js
--rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js.gz
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.064829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/
--rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.3293616ec0c6.woff
--rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg
--rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.8b27bc96115c.eot
--rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf
--rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf.gz
--rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.eot
--rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg
--rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf.gz
--rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.woff
--rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg
--rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.448c34a56d69.woff2
--rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf
--rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf.gz
--rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.f4769f9bdb74.eot
--rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.fa2772327f55.woff
--rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg.gz
--rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf.gz
--rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.064829 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/
--rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.9bbc6e960299.png
--rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.png
--rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.90233c9067e9.png
--rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.png
--rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.a4b938cf382b.png
--rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.png
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.068163 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/
--rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js
--rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js
--rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js
--rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js
--rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    63224 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js
--rw-r--r--   0 yeison    (1000) users      (984)    14375 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)   157600 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js
--rw-r--r--   0 yeison    (1000) users      (984)    40759 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js
--rw-r--r--   0 yeison    (1000) users      (984)      787 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js
--rw-r--r--   0 yeison    (1000) users      (984)      787 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js
--rw-r--r--   0 yeison    (1000) users      (984)      571 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js
--rw-r--r--   0 yeison    (1000) users      (984)      571 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js
--rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js
--rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js
--rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js
--rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-07-22 23:45:33.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js.gz
--rw-r--r--   0 yeison    (1000) users      (984)    14226 2023-07-27 02:19:45.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/staticfiles.json
--rw-r--r--   0 yeison    (1000) users      (984)      336 2023-07-23 01:07:34.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/startup.sh
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.068163 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/
--rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-22 20:40:50.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/__init__.py
--rw-r--r--   0 yeison    (1000) users      (984)      407 2023-07-22 20:40:50.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/asgi.py
--rw-r--r--   0 yeison    (1000) users      (984)     5910 2023-07-23 00:02:18.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/settings.py
--rw-r--r--   0 yeison    (1000) users      (984)     1062 2023-07-22 20:56:12.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/urls.py
--rw-r--r--   0 yeison    (1000) users      (984)      494 2023-07-22 20:41:41.000000 hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/wsgi.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-01 03:15:24.008162 hci-framework-0.1a4/hci_framework.egg-info/
--rw-r--r--   0 yeison    (1000) users      (984)     1366 2023-08-01 03:15:23.000000 hci-framework-0.1a4/hci_framework.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)    59910 2023-08-01 03:15:24.000000 hci-framework-0.1a4/hci_framework.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-08-01 03:15:23.000000 hci-framework-0.1a4/hci_framework.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (984)       25 2023-08-01 03:15:23.000000 hci-framework-0.1a4/hci_framework.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) users      (984)       14 2023-08-01 03:15:23.000000 hci-framework-0.1a4/hci_framework.egg-info/top_level.txt
--rw-r--r--   0 yeison    (1000) users      (984)       38 2023-08-01 03:15:24.068163 hci-framework-0.1a4/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (984)     2025 2023-08-01 03:14:46.000000 hci-framework-0.1a4/setup.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.227549 hci-framework-0.1a5/
+-rw-r--r--   0 yeison    (1000) users      (984)     1321 2021-07-29 02:00:34.000000 hci-framework-0.1a5/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)      229 2023-07-16 01:05:40.000000 hci-framework-0.1a5/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) users      (984)     1366 2023-08-06 02:19:59.227549 hci-framework-0.1a5/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)       16 2023-07-16 01:07:26.000000 hci-framework-0.1a5/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/cmd/
+-rw-r--r--   0 yeison    (1000) users      (984)     1586 2023-08-06 02:18:57.000000 hci-framework-0.1a5/cmd/foundation_logs
+-rw-r--r--   0 yeison    (1000) users      (984)     5806 2023-08-05 18:20:43.000000 hci-framework-0.1a5/cmd/foundation_status
+-rw-r--r--   0 yeison    (1000) users      (984)     1236 2023-08-05 19:13:08.000000 hci-framework-0.1a5/cmd/run_framework.py
+-rw-r--r--   0 yeison    (1000) users      (984)      887 2023-08-02 23:44:24.000000 hci-framework-0.1a5/cmd/start_worker.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-07-16 00:31:29.000000 hci-framework-0.1a5/hci_framework/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/hci_framework/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/asgi.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3242 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/settings.py
+-rw-r--r--   0 yeison    (1000) users      (984)      755 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/urls.py
+-rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/wsgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      669 2023-06-22 22:07:41.000000 hci-framework-0.1a5/hci_framework/hci_framework/manage.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/radiant/
+-rw-r--r--   0 yeison    (1000) users      (984)        2 2023-07-09 21:08:21.000000 hci-framework-0.1a5/hci_framework/radiant/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/radiant/brython/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1737 2023-07-10 00:34:54.000000 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/figurestream.py
+-rw-r--r--   0 yeison    (1000) users      (984)      254 2023-08-05 02:22:37.000000 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/server.py
+-rw-r--r--   0 yeison    (1000) users      (984)       57 2023-07-09 21:07:45.000000 hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/utils.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/radiant/python_tools/
+-rw-r--r--   0 yeison    (1000) users      (984)      691 2023-08-05 17:34:07.000000 hci-framework-0.1a5/hci_framework/radiant/python_tools/python_logger.py
+-rw-r--r--   0 yeison    (1000) users      (984)      853 2023-08-05 02:01:42.000000 hci-framework-0.1a5/hci_framework/radiant/python_tools/python_swarm.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3264 2023-08-05 01:59:05.000000 hci-framework-0.1a5/hci_framework/radiant/server.py
+-rw-r--r--   0 yeison    (1000) users      (984)      306 2023-08-01 02:26:57.000000 hci-framework-0.1a5/hci_framework/radiant/template.html
+-rw-r--r--   0 yeison    (1000) users      (984)       56 2023-07-09 21:07:01.000000 hci-framework-0.1a5/hci_framework/radiant/utils.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/utils/
+-rw-r--r--   0 yeison    (1000) users      (984)       67 2023-08-02 23:40:21.000000 hci-framework-0.1a5/hci_framework/utils/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1500 2023-08-06 02:15:06.000000 hci-framework-0.1a5/hci_framework/utils/kafkalogs.py
+-rw-r--r--   0 yeison    (1000) users      (984)    10236 2023-08-06 02:05:32.000000 hci-framework-0.1a5/hci_framework/utils/swarm.py
+-rw-r--r--   0 yeison    (1000) users      (984)     9914 2023-08-02 23:34:45.000000 hci-framework-0.1a5/hci_framework/utils/workers.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/workers/
+-rw-r--r--   0 yeison    (1000) users      (984)      535 2023-08-02 21:50:34.000000 hci-framework-0.1a5/hci_framework/workers/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/workers/django_worker/
+-rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-22 00:12:49.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/db.sqlite3
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework/workers/django_worker/djangoship/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangoship/access.log
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangoship/error.log
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/
+-rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:08:17.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/__init__.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      397 2023-07-21 23:08:17.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/asgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)     3233 2023-07-21 23:08:17.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/settings.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      766 2023-07-21 23:08:17.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/urls.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      485 2023-07-22 00:19:20.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/wsgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      666 2023-07-21 23:08:17.000000 hci-framework-0.1a5/hci_framework/workers/django_worker/manage.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/
+-rw-r--r--   0 yeison    (1000) users      (984)     1510 2023-07-10 00:37:51.000000 hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/main.py
+-rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-05 01:41:31.000000 hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/requirements.txt
+-rwxr-xr-x   0 yeison    (1000) users      (984)     1480 2023-07-09 23:24:03.000000 hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/stream.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/figurestream_worker/
+-rwxr-xr-x   0 yeison    (1000) users      (984)     1194 2023-07-31 01:58:18.000000 hci-framework-0.1a5/hci_framework/workers/figurestream_worker/main.py
+-rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-05 01:40:17.000000 hci-framework-0.1a5/hci_framework/workers/figurestream_worker/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/main_app/
+-rw-r--r--   0 yeison    (1000) users      (984)     1657 2023-08-05 02:46:12.000000 hci-framework-0.1a5/hci_framework/workers/main_app/main.py
+-rw-r--r--   0 yeison    (1000) users      (984)       47 2023-08-05 01:41:47.000000 hci-framework-0.1a5/hci_framework/workers/main_app/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/main_app/styles/
+-rw-r--r--   0 yeison    (1000) users      (984)      402 2023-08-05 02:47:40.000000 hci-framework-0.1a5/hci_framework/workers/main_app/styles/styles.css
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/main_app/templates/
+-rw-r--r--   0 yeison    (1000) users      (984)      125 2023-08-05 02:31:01.000000 hci-framework-0.1a5/hci_framework/workers/main_app/templates/main_area.html
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/
+-rw-r--r--   0 yeison    (1000) users      (984)   131072 2023-07-27 02:19:49.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/db.sqlite3
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/djangoship/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:49.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/djangoship/access.log
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:49.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/djangoship/error.log
+-rwxr-xr-x   0 yeison    (1000) users      (984)      671 2023-07-22 20:40:50.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/manage.py
+-rw-r--r--   0 yeison    (1000) users      (984)      182 2023-07-22 22:50:08.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.160882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.164215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/
+-rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21357 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4847 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21207 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4737 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css
+-rw-r--r--   0 yeison    (1000) users      (984)      849 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css
+-rw-r--r--   0 yeison    (1000) users      (984)      849 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.css
+-rw-r--r--   0 yeison    (1000) users      (984)      267 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css
+-rw-r--r--   0 yeison    (1000) users      (984)      267 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9090 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2236 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9047 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2199 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      958 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css
+-rw-r--r--   0 yeison    (1000) users      (984)      417 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      958 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.css
+-rw-r--r--   0 yeison    (1000) users      (984)      417 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css
+-rw-r--r--   0 yeison    (1000) users      (984)      779 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css
+-rw-r--r--   0 yeison    (1000) users      (984)      779 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css
+-rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css
+-rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css
+-rw-r--r--   0 yeison    (1000) users      (984)      527 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css
+-rw-r--r--   0 yeison    (1000) users      (984)      527 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4878 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4788 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1229 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.167548 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    12110 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2561 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    11900 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2468 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.174215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/README.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/README.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.174215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-addlink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-alert.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-changelink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-yes.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/search.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/search.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-add.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.180882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.180882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/
+-rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js
+-rw-r--r--   0 yeison    (1000) users      (984)      425 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js
+-rw-r--r--   0 yeison    (1000) users      (984)      425 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      884 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js
+-rw-r--r--   0 yeison    (1000) users      (984)      430 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      884 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js
+-rw-r--r--   0 yeison    (1000) users      (984)      430 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      606 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js
+-rw-r--r--   0 yeison    (1000) users      (984)      322 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      606 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js
+-rw-r--r--   0 yeison    (1000) users      (984)      322 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      614 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js
+-rw-r--r--   0 yeison    (1000) users      (984)      614 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      978 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js
+-rw-r--r--   0 yeison    (1000) users      (984)      502 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      978 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js
+-rw-r--r--   0 yeison    (1000) users      (984)      502 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      347 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js
+-rw-r--r--   0 yeison    (1000) users      (984)      236 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      347 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.js
+-rw-r--r--   0 yeison    (1000) users      (984)      236 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/jquery.init.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      845 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js
+-rw-r--r--   0 yeison    (1000) users      (984)      845 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js
+-rw-r--r--   0 yeison    (1000) users      (984)      270 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js
+-rw-r--r--   0 yeison    (1000) users      (984)      270 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      536 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js
+-rw-r--r--   0 yeison    (1000) users      (984)      536 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      586 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js
+-rw-r--r--   0 yeison    (1000) users      (984)      277 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      586 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js
+-rw-r--r--   0 yeison    (1000) users      (984)      277 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      605 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js
+-rw-r--r--   0 yeison    (1000) users      (984)      605 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.184215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js
+-rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js
+-rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.187548 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.210882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      460 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js
+-rw-r--r--   0 yeison    (1000) users      (984)      460 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      905 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      498 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      905 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js
+-rw-r--r--   0 yeison    (1000) users      (984)      498 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      721 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      721 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      968 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      541 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      968 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js
+-rw-r--r--   0 yeison    (1000) users      (984)      541 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js
+-rw-r--r--   0 yeison    (1000) users      (984)      553 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js
+-rw-r--r--   0 yeison    (1000) users      (984)      553 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      965 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js
+-rw-r--r--   0 yeison    (1000) users      (984)      523 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      965 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js
+-rw-r--r--   0 yeison    (1000) users      (984)      523 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js
+-rw-r--r--   0 yeison    (1000) users      (984)      623 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js
+-rw-r--r--   0 yeison    (1000) users      (984)      623 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      828 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      828 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js
+-rw-r--r--   0 yeison    (1000) users      (984)      644 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js
+-rw-r--r--   0 yeison    (1000) users      (984)      644 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      844 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js
+-rw-r--r--   0 yeison    (1000) users      (984)      447 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      844 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js
+-rw-r--r--   0 yeison    (1000) users      (984)      447 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      922 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      474 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      922 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js
+-rw-r--r--   0 yeison    (1000) users      (984)      474 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      801 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      432 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      801 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js
+-rw-r--r--   0 yeison    (1000) users      (984)      432 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      868 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      450 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      868 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js
+-rw-r--r--   0 yeison    (1000) users      (984)      450 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js
+-rw-r--r--   0 yeison    (1000) users      (984)      538 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js
+-rw-r--r--   0 yeison    (1000) users      (984)      538 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      803 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      803 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js
+-rw-r--r--   0 yeison    (1000) users      (984)      484 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      484 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      984 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js
+-rw-r--r--   0 yeison    (1000) users      (984)      518 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      984 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js
+-rw-r--r--   0 yeison    (1000) users      (984)      518 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      572 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      572 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      852 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js
+-rw-r--r--   0 yeison    (1000) users      (984)      477 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      852 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      477 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js
+-rw-r--r--   0 yeison    (1000) users      (984)      556 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      556 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      831 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      831 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js
+-rw-r--r--   0 yeison    (1000) users      (984)      530 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js
+-rw-r--r--   0 yeison    (1000) users      (984)      530 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      416 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js
+-rw-r--r--   0 yeison    (1000) users      (984)      416 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      807 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      807 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      897 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js
+-rw-r--r--   0 yeison    (1000) users      (984)      488 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      897 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js
+-rw-r--r--   0 yeison    (1000) users      (984)      488 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      862 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      862 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      533 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js
+-rw-r--r--   0 yeison    (1000) users      (984)      533 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js
+-rw-r--r--   0 yeison    (1000) users      (984)      540 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js
+-rw-r--r--   0 yeison    (1000) users      (984)      540 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      855 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js
+-rw-r--r--   0 yeison    (1000) users      (984)      506 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      855 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js
+-rw-r--r--   0 yeison    (1000) users      (984)      506 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      944 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js
+-rw-r--r--   0 yeison    (1000) users      (984)      521 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      944 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js
+-rw-r--r--   0 yeison    (1000) users      (984)      521 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      505 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js
+-rw-r--r--   0 yeison    (1000) users      (984)      505 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js
+-rw-r--r--   0 yeison    (1000) users      (984)      557 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      557 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      811 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      811 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      778 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      778 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js
+-rw-r--r--   0 yeison    (1000) users      (984)      591 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js
+-rw-r--r--   0 yeison    (1000) users      (984)      591 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      904 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js
+-rw-r--r--   0 yeison    (1000) users      (984)      469 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      904 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      469 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      947 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js
+-rw-r--r--   0 yeison    (1000) users      (984)      524 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      947 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      524 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      587 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js
+-rw-r--r--   0 yeison    (1000) users      (984)      587 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      876 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      486 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      876 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js
+-rw-r--r--   0 yeison    (1000) users      (984)      486 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      878 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      878 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      938 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      938 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js
+-rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js
+-rw-r--r--   0 yeison    (1000) users      (984)      617 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      617 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      925 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js
+-rw-r--r--   0 yeison    (1000) users      (984)      487 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      925 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      487 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      903 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      490 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      903 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js
+-rw-r--r--   0 yeison    (1000) users      (984)      490 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      608 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      608 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      980 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js
+-rw-r--r--   0 yeison    (1000) users      (984)      552 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      980 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      552 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      786 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      786 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      515 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js
+-rw-r--r--   0 yeison    (1000) users      (984)      515 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      771 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      434 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      771 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      434 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      775 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js
+-rw-r--r--   0 yeison    (1000) users      (984)      423 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      775 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      423 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      626 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      626 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      796 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      479 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      796 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      479 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      468 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js
+-rw-r--r--   0 yeison    (1000) users      (984)      468 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      707 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      451 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      707 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js
+-rw-r--r--   0 yeison    (1000) users      (984)      451 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js
+-rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.210882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/
+-rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js
+-rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.210882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/
+-rw-r--r--   0 yeison    (1000) users      (984)      753 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css
+-rw-r--r--   0 yeison    (1000) users      (984)      452 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      740 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css
+-rw-r--r--   0 yeison    (1000) users      (984)      440 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.210882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.03ce3dcc84af.gif
+-rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.gif
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.214215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js
+-rw-r--r--   0 yeison    (1000) users      (984)      960 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js
+-rw-r--r--   0 yeison    (1000) users      (984)      960 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js
+-rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js
+-rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      814 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js
+-rw-r--r--   0 yeison    (1000) users      (984)      814 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.217549 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2783 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    23411 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map
+-rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2772 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3398 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3385 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   121457 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map
+-rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    19586 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map
+-rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   121560 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css
+-rw-r--r--   0 yeison    (1000) users      (984)    19657 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css
+-rw-r--r--   0 yeison    (1000) users      (984)      612 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css
+-rw-r--r--   0 yeison    (1000) users      (984)      612 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21723 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4230 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21658 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4186 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      817 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css
+-rw-r--r--   0 yeison    (1000) users      (984)      390 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      817 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css
+-rw-r--r--   0 yeison    (1000) users      (984)      390 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.154215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.217549 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/
+-rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css
+-rw-r--r--   0 yeison    (1000) users      (984)      671 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css
+-rw-r--r--   0 yeison    (1000) users      (984)      671 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css
+-rw-r--r--   0 yeison    (1000) users      (984)      640 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)      640 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.217549 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico
+-rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico
+-rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.a4b938cf382b.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.png
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.220882 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/
+-rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js
+-rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js
+-rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.224215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/
+-rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.3293616ec0c6.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.8b27bc96115c.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.448c34a56d69.woff2
+-rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.f4769f9bdb74.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.fa2772327f55.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.224215 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.9bbc6e960299.png
+-rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.png
+-rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.90233c9067e9.png
+-rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.a4b938cf382b.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.png
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.227549 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    63224 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js
+-rw-r--r--   0 yeison    (1000) users      (984)    14375 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   157600 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js
+-rw-r--r--   0 yeison    (1000) users      (984)    40759 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js
+-rw-r--r--   0 yeison    (1000) users      (984)      787 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js
+-rw-r--r--   0 yeison    (1000) users      (984)      787 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js
+-rw-r--r--   0 yeison    (1000) users      (984)      571 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js
+-rw-r--r--   0 yeison    (1000) users      (984)      571 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js
+-rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js
+-rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-07-22 23:45:33.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14226 2023-07-27 02:19:45.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/staticfiles.json
+-rw-r--r--   0 yeison    (1000) users      (984)      336 2023-07-23 01:07:34.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/startup.sh
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.227549 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-22 20:40:50.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)      407 2023-07-22 20:40:50.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/asgi.py
+-rw-r--r--   0 yeison    (1000) users      (984)     5910 2023-07-23 00:02:18.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/settings.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1062 2023-07-22 20:56:12.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/urls.py
+-rw-r--r--   0 yeison    (1000) users      (984)      494 2023-07-22 20:41:41.000000 hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/wsgi.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-06 02:19:59.157548 hci-framework-0.1a5/hci_framework.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)     1366 2023-08-06 02:19:59.000000 hci-framework-0.1a5/hci_framework.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)    60005 2023-08-06 02:19:59.000000 hci-framework-0.1a5/hci_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-08-06 02:19:59.000000 hci-framework-0.1a5/hci_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       25 2023-08-06 02:19:59.000000 hci-framework-0.1a5/hci_framework.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       14 2023-08-06 02:19:59.000000 hci-framework-0.1a5/hci_framework.egg-info/top_level.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-08-06 02:19:59.227549 hci-framework-0.1a5/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     2124 2023-08-06 02:17:18.000000 hci-framework-0.1a5/setup.py
```

### Comparing `hci-framework-0.1a4/LICENSE` & `hci-framework-0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/PKG-INFO` & `hci-framework-0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hci-framework
-Version: 0.1a4
+Version: 0.1a5
 Summary: A real-time tool for acquisition, analysis and stimuli delivery.
 Download-URL: https://github.com/dunderlab/hci_framework
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
```

### Comparing `hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/settings.py` & `hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/settings.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/hci_framework/hci_framework/urls.py` & `hci-framework-0.1a5/hci_framework/hci_framework/hci_framework/urls.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/hci_framework/manage.py` & `hci-framework-0.1a5/hci_framework/hci_framework/manage.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/radiant/brython/hci_framework/radiant/figurestream.py` & `hci-framework-0.1a5/hci_framework/radiant/brython/hci_framework/radiant/figurestream.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/radiant/python_tools/python_swarm.py` & `hci-framework-0.1a5/hci_framework/radiant/python_tools/python_swarm.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/radiant/server.py` & `hci-framework-0.1a5/hci_framework/radiant/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from radiant.framework.server import RadiantAPI, RadiantServer
+from radiant.framework.server import RadiantAPI, RadiantServer, render
 from radiant.framework.utils import environ, run_script
 
 import os
 
 
 FigureStream = None
 
-########################################################################
-
 
+########################################################################
 class FrameworkAPI(RadiantAPI):
     """Rename Randiant with a arand new class."""
 
     # ---------------------------------------------------------------------
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `hci-framework-0.1a4/hci_framework/utils/swarm.py` & `hci-framework-0.1a5/hci_framework/utils/swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,63 +131,66 @@
                 ),
             ]
         )
         return service_name in self.services
 
     # ----------------------------------------------------------------------
     def start_kafka(self, kafka_service_name="kafka-service",
-                    zookeeper_service_name="zookeeper-service", kafka_port=9092,
+                    zookeeper_service_name="zookeeper-service",
+                    kafka_port=9092, kafka_port_external=19092,
                     zookeeper_port=2181, restart=False):
         """"""
         if restart and (kafka_service_name in self.services):
             self.stop_service(kafka_service_name)
             logging.warning(f"Restarting service '{kafka_service_name}'")
 
         if restart and (zookeeper_service_name in self.services):
             self.stop_service(zookeeper_service_name)
             logging.warning(f"Restarting service '{zookeeper_service_name}'")
 
         if not kafka_service_name in self.services:
             kafka_service = self.client.services.create(
                 image="dunderlab/kafka:latest",
+                restart_policy=docker.types.RestartPolicy(condition='any'),
                 name=kafka_service_name,
                 networks=self.networks,
-                endpoint_spec=docker.types.EndpointSpec(
-                    ports={kafka_port: kafka_port}),
+                endpoint_spec=docker.types.EndpointSpec(ports={kafka_port: kafka_port,
+                                                               kafka_port_external: kafka_port_external, }),
                 env=[
                     f"KAFKA_ZOOKEEPER_CONNECT={zookeeper_service_name}:{zookeeper_port}",
-                    f"KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://{kafka_service_name}:{kafka_port}",
+                    f"KAFKA_LISTENER_SECURITY_PROTOCOL_MAP=PLAINTEXT:PLAINTEXT,PLAINTEXT_HOST:PLAINTEXT",
+                    f"KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://{kafka_service_name}:{kafka_port},PLAINTEXT_HOST://localhost:{kafka_port_external}",
                 ],
             )
         else:
             logging.warning(f"Service '{kafka_service_name}' already exist")
 
         if not zookeeper_service_name in self.services:
             zookeeper_service = self.client.services.create(
                 image="dunderlab/zookeeper:latest",
                 name=zookeeper_service_name,
                 networks=self.networks,
-                endpoint_spec=docker.types.EndpointSpec(
-                    ports={zookeeper_port: zookeeper_port}),
+                endpoint_spec=docker.types.EndpointSpec(ports={zookeeper_port: zookeeper_port}),
                 env=[
                     f"ZOOKEEPER_CLIENT_PORT={zookeeper_port}",
                 ],
             )
         else:
             logging.warning(
                 f"Service '{zookeeper_service_name}' already exist")
 
         return kafka_service_name in self.services, zookeeper_service_name in self.services
 
     # ----------------------------------------------------------------------
     def start_kafka_logs(self, kafka_service_name="kafka-logs-service",
-                         zookeeper_service_name="zookeeper-logs-service", kafka_port=9093,
+                         zookeeper_service_name="zookeeper-logs-service",
+                         kafka_port=9093, kafka_port_external=19093,
                          zookeeper_port=2182, restart=False):
         """"""
-        return self.start_kafka(kafka_service_name, zookeeper_service_name, kafka_port, zookeeper_port, restart)
+        return self.start_kafka(kafka_service_name, zookeeper_service_name, kafka_port, kafka_port_external, zookeeper_port, restart)
 
     # ----------------------------------------------------------------------
     def start_timescaledb(self, service_name="timescaledb-service", port=5432, volume_name=None, restart=False):
         """"""
         if restart and (service_name in self.services):
             self.stop_service(service_name)
             logging.warning(f"Restarting service '{service_name}'")
```

### Comparing `hci-framework-0.1a4/hci_framework/utils/workers.py` & `hci-framework-0.1a5/hci_framework/utils/workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
             return
 
         if port is None:
             port = self.get_open_port()
 
         if service_name is None:
             service_name = self.gen_worker_name()
+        else:
+            service_name = WORKER_NAME.format(service_name)
         service_name_env = os.path.split(worker_path)[-1]
 
         if restart and (service_name in self.swarm.services):
             self.swarm.stop_service(service_name)
             logging.warning(f"Restarting service '{service_name}'")
         elif service_name in self.swarm.services:
             logging.warning(f"Service '{service_name}' already exist")
@@ -115,14 +117,16 @@
         if port_stream is None:
             port_stream = self.get_open_port()
         if port_radiant is None:
             port_radiant = self.get_open_port()
 
         if service_name is None:
             service_name = self.gen_worker_name()
+        else:
+            service_name = WORKER_NAME.format(service_name)
         service_name_env = os.path.split(worker_path)[-1]
 
         if restart and (service_name in self.swarm.services):
             self.swarm.stop_service(service_name)
             logging.warning(f"Restarting service '{service_name}'")
         elif service_name in self.swarm.services:
             logging.warning(f"Service '{service_name}' already exist")
@@ -175,14 +179,16 @@
             worker_path = select_worker(worker_path)
 
         if port is None:
             port = self.get_open_port()
 
         if service_name is None:
             service_name = self.gen_worker_name()
+        else:
+            service_name = WORKER_NAME.format(service_name)
         service_name_env = os.path.split(worker_path)[-1]
 
         if restart and (service_name in self.swarm.services):
             self.swarm.stop_service(service_name)
             logging.warning(f"Restarting service '{service_name}'")
         elif service_name in self.swarm.services:
             logging.warning(f"Service '{service_name}' already exist")
```

### Comparing `hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/settings.py` & `hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/settings.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/django_worker/djangotest/urls.py` & `hci-framework-0.1a5/hci_framework/workers/django_worker/djangotest/urls.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/django_worker/manage.py` & `hci-framework-0.1a5/hci_framework/workers/django_worker/manage.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/main.py` & `hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/main.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/figurestream_brython_worker/stream.py` & `hci-framework-0.1a5/hci_framework/workers/figurestream_brython_worker/stream.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/figurestream_worker/main.py` & `hci-framework-0.1a5/hci_framework/workers/figurestream_worker/main.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/main_app/main.py` & `hci-framework-0.1a5/hci_framework/workers/main_app/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-from hci_framework.radiant.server import FrameworkAPI
-from browser import html
+from hci_framework.radiant.server import FrameworkAPI, render
+from browser import html, document
 
 # Material 3
 # https://m3.material.io/develop/web
 import material_3 as md
 
 
 ########################################################################
 class BareMinimum(FrameworkAPI):
 
     # ----------------------------------------------------------------------
     def __init__(self, *args, **kwargs):
         """"""
         super().__init__(*args, **kwargs)
-        # self.add_css_file('css/theme.css')
+        self.add_css_file('styles/styles.css')
 
         # md_list = md.list()
         # self.body <= md_list
         # for i, service in enumerate(self.MyClass.services()):
             # list_item = md.list_item(headline=service, active=(i == 0))
             # md_list <= list_item
 
-        button = md.text_button('Logging')
-        button.bind('click', self.send_log)
-        self.body <= button
+        self.body <= self.main_area()
 
-        self.body <= html.PRE(self.swarm.get_join_command())
+        md_list = md.list()
+        document.select_one('#radiant-drawer') <= md_list
+        for i in range(10):
+            list_item = md.list_item(headline=f'Item {i}', active=(i == 0))
+            md_list <= list_item
+
+        # button = md.text_button('Logging')
+        # button.bind('click', self.send_log)
+        # self.body <= button
+
+        document.select_one('#radiant-main_area') <= html.PRE(self.swarm.get_join_command())
+
+    # # ----------------------------------------------------------------------
+    # def send_log(self, evt):
+        # """"""
+        # print('logging message')
+        # self.logging.warning('logging message')
 
     # ----------------------------------------------------------------------
-    def send_log(self, evt):
+    def main_area(self):
         """"""
-        print('logging message')
-        self.logging.warning('logging message')
+        return render('templates/main_area.html', context={})
 
 
 if __name__ == '__main__':
     BareMinimum()
```

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/db.sqlite3` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/db.sqlite3`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/manage.py` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/manage.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/autocomplete.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/base.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/base.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/changelists.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/forms.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/login.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/nav_sidebar.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/responsive_rtl.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/rtl.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/css/widgets.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/LICENSE.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-no.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/selector-icons.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/img/sorting-icons.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectBox.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/SelectFilter2.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/actions.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/calendar.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/collapse.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/core.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/core.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/filters.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/inlines.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/nav_sidebar.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/prepopulate_init.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/theme.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/urlify.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.03ce3dcc84af.gif` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.03ce3dcc84af.gif`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.gif` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/img/indicator.gif`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/default.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/css/prettify.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.a4b938cf382b.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.a4b938cf382b.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/img/grid.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/api.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.3293616ec0c6.woff` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.3293616ec0c6.woff`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.8b27bc96115c.eot` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.8b27bc96115c.eot`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.eot` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.woff` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.448c34a56d69.woff2` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.448c34a56d69.woff2`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.eot` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.f4769f9bdb74.eot` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.f4769f9bdb74.eot`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.fa2772327f55.woff` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.fa2772327f55.woff`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff2` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.9bbc6e960299.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.9bbc6e960299.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.90233c9067e9.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.90233c9067e9.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.a4b938cf382b.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.a4b938cf382b.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.png` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/img/grid.png`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/csrf.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/default.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js.gz` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js.gz`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/resources/staticfiles.json` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/resources/staticfiles.json`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/settings.py` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/settings.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework/workers/timescaledb_api/timescaledb_api/urls.py` & `hci-framework-0.1a5/hci_framework/workers/timescaledb_api/timescaledb_api/urls.py`

 * *Files identical despite different names*

### Comparing `hci-framework-0.1a4/hci_framework.egg-info/PKG-INFO` & `hci-framework-0.1a5/hci_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hci-framework
-Version: 0.1a4
+Version: 0.1a5
 Summary: A real-time tool for acquisition, analysis and stimuli delivery.
 Download-URL: https://github.com/dunderlab/hci_framework
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
```

### Comparing `hci-framework-0.1a4/hci_framework.egg-info/SOURCES.txt` & `hci-framework-0.1a5/hci_framework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+cmd/foundation_logs
+cmd/foundation_status
+cmd/run_framework.py
+cmd/start_worker.py
 hci_framework/__init__.py
 hci_framework.egg-info/PKG-INFO
 hci_framework.egg-info/SOURCES.txt
 hci_framework.egg-info/dependency_links.txt
 hci_framework.egg-info/requires.txt
 hci_framework.egg-info/top_level.txt
 hci_framework/hci_framework/manage.py
@@ -42,16 +46,16 @@
 hci_framework/workers/figurestream_brython_worker/main.py
 hci_framework/workers/figurestream_brython_worker/requirements.txt
 hci_framework/workers/figurestream_brython_worker/stream.py
 hci_framework/workers/figurestream_worker/main.py
 hci_framework/workers/figurestream_worker/requirements.txt
 hci_framework/workers/main_app/main.py
 hci_framework/workers/main_app/requirements.txt
-hci_framework/workers/python_logs/main.py
-hci_framework/workers/python_logs/requirements.txt
+hci_framework/workers/main_app/styles/styles.css
+hci_framework/workers/main_app/templates/main_area.html
 hci_framework/workers/timescaledb_api/db.sqlite3
 hci_framework/workers/timescaledb_api/manage.py
 hci_framework/workers/timescaledb_api/requirements.txt
 hci_framework/workers/timescaledb_api/startup.sh
 hci_framework/workers/timescaledb_api/djangoship/access.log
 hci_framework/workers/timescaledb_api/djangoship/error.log
 hci_framework/workers/timescaledb_api/resources/staticfiles.json
```

### Comparing `hci-framework-0.1a4/setup.py` & `hci-framework-0.1a5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-version_str = '0.1a4'
+version_str = '0.1a5'
 
 setup(
     name='hci-framework',
     version=version_str,
     packages=['hci_framework'],
 
     author='Yeison Cardona',
@@ -37,15 +37,18 @@
     python_requires='>=3.11',
 
     # entry_points={
     # 'console_scripts': ['bci-framework=bci_framework.__main__:main'],
     # },
 
     scripts=[
-       # "cmd/openbci_cli",
+        "cmd/foundation_status",
+        "cmd/foundation_logs",
+        "cmd/run_framework.py",
+        "cmd/start_worker.py",
     ],
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Healthcare Industry',
```

