# Comparing `tmp/lino-welcht-23.6.0.tar.gz` & `tmp/lino-welcht-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welcht-23.6.0.tar", last modified: Tue Jun 20 12:12:37 2023, max compression
+gzip compressed data, was "lino-welcht-23.8.0.tar", last modified: Sun Aug  6 15:49:31 2023, max compression
```

## Comparing `lino-welcht-23.6.0.tar` & `lino-welcht-23.8.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/COPYING
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      110 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/MANIFEST.in
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1655 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      734 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/README.rst
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      880 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      224 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/help_texts.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1549 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/layouts.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      258 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      546 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1013 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1465 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4722 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      907 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1357 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/ui.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/cv/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1134 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      655 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/demo.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      931 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7570 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/isip/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      290 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/isip/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1924 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/isip/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      418 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      457 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/choicelists.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      613 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       60 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/demo2.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       58 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/std.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7176 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/models.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/de/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39041 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    74719 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/fr/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4021 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     9514 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/nl/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      409 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    93297 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7024 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/migrate.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     7594 2023-03-31 11:55:46.000000 lino-welcht-23.6.0/lino_welcht/settings.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4938 2023-06-20 12:12:03.000000 lino-welcht-23.6.0/lino_welcht/setup_info.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      247 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/workflows.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht.egg-info/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1655 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1703 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/SOURCES.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/dependency_links.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht.egg-info/not-zip-safe
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       72 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/requires.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       12 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/top_level.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1052 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.python3.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.stable.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      931 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/setup.cfg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      163 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/setup.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      377 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tasks.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/tests/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      552 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tests/__init__.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      171 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tests/test_docs.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:58.000000 lino-welcht-23.8.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      110 2019-02-28 04:54:23.000000 lino-welcht-23.8.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1692 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      734 2021-08-19 05:39:07.000000 lino-welcht-23.8.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      880 2021-04-28 10:35:43.000000 lino-welcht-23.8.0/lino_welcht/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      224 2022-09-30 14:29:59.000000 lino-welcht-23.8.0/lino_welcht/help_texts.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1549 2022-09-30 11:46:19.000000 lino-welcht-23.8.0/lino_welcht/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      258 2022-10-02 10:41:58.000000 lino-welcht-23.8.0/lino_welcht/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      546 2022-10-06 13:38:44.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.426055 lino-welcht-23.8.0/lino_welcht/lib/courses/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/Enrolment/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1013 2015-09-19 03:53:35.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1465 2015-09-19 03:53:35.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:35.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4722 2021-04-14 18:14:38.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      907 2021-04-07 10:22:55.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3793 2022-11-08 12:29:27.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1357 2022-11-08 12:30:48.000000 lino-welcht-23.8.0/lino_welcht/lib/courses/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/cv/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1134 2021-04-07 10:22:54.000000 lino-welcht-23.8.0/lino_welcht/lib/cv/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:36.000000 lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      655 2021-04-15 06:04:50.000000 lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-04-07 10:22:55.000000 lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7570 2023-02-18 14:56:22.000000 lino-welcht-23.8.0/lino_welcht/lib/cv/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/isip/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      290 2021-04-07 10:22:54.000000 lino-welcht-23.8.0/lino_welcht/lib/isip/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2022-10-07 01:03:12.000000 lino-welcht-23.8.0/lino_welcht/lib/isip/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/pcsw/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      472 2023-08-04 11:16:25.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2021-04-07 10:22:54.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/choicelists.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/pcsw/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/pcsw/config/pcsw/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      613 2015-09-19 03:53:35.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/lib/pcsw/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-08 13:29:44.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2017-04-22 06:37:57.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       58 2016-06-08 13:30:04.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7176 2022-10-03 08:53:52.000000 lino-welcht-23.8.0/lino_welcht/lib/pcsw/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39041 2018-12-10 08:06:01.000000 lino-welcht-23.8.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    74719 2021-02-11 19:06:41.000000 lino-welcht-23.8.0/lino_welcht/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/lino_welcht/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4021 2019-03-29 10:29:37.000000 lino-welcht-23.8.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9514 2021-02-11 19:06:42.000000 lino-welcht-23.8.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht/locale/nl/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/lino_welcht/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welcht-23.8.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welcht-23.8.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7024 2021-04-07 10:22:53.000000 lino-welcht-23.8.0/lino_welcht/migrate.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7594 2023-04-01 07:25:20.000000 lino-welcht-23.8.0/lino_welcht/settings.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4938 2023-08-06 15:49:13.000000 lino-welcht-23.8.0/lino_welcht/setup_info.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2018-12-08 06:32:49.000000 lino-welcht-23.8.0/lino_welcht/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.434055 lino-welcht-23.8.0/lino_welcht.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1692 2023-08-06 15:49:31.000000 lino-welcht-23.8.0/lino_welcht.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1703 2023-08-06 15:49:31.000000 lino-welcht-23.8.0/lino_welcht.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-08-06 15:49:31.000000 lino-welcht-23.8.0/lino_welcht.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-02-27 20:03:15.000000 lino-welcht-23.8.0/lino_welcht.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       72 2023-08-06 15:49:31.000000 lino-welcht-23.8.0/lino_welcht.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2023-08-06 15:49:31.000000 lino-welcht-23.8.0/lino_welcht.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1052 2021-05-05 05:16:56.000000 lino-welcht-23.8.0/requirements.python3.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-05-05 05:16:56.000000 lino-welcht-23.8.0/requirements.stable.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-05-05 05:16:56.000000 lino-welcht-23.8.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      163 2019-02-27 13:45:16.000000 lino-welcht-23.8.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2021-03-22 12:47:21.000000 lino-welcht-23.8.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-08-06 15:49:31.438055 lino-welcht-23.8.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      552 2021-04-07 10:22:53.000000 lino-welcht-23.8.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      171 2019-03-07 07:55:55.000000 lino-welcht-23.8.0/tests/test_docs.py
```

### Comparing `lino-welcht-23.6.0/COPYING` & `lino-welcht-23.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/PKG-INFO` & `lino-welcht-23.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 23.6.0
+Version: 23.8.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -38,7 +40,9 @@
   `Lino Welfare <https://welfare.lino-framework.org>`__.
 
 - The `French project homepage <https://fr.welfare.lino-framework.org>`__
   contains release notes and end-user docs.
 
 - Online demo site at https://welfare-demo.lino-framework.org
 
+
+
```

### Comparing `lino-welcht-23.6.0/README.rst` & `lino-welcht-23.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/__init__.py` & `lino-welcht-23.8.0/lino_welcht/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/layouts.py` & `lino-welcht-23.8.0/lino_welcht/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/__init__.py` & `lino-welcht-23.8.0/lino_welcht/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html` & `lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html` & `lino-welcht-23.8.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/demo.py` & `lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/std.py` & `lino-welcht-23.8.0/lino_welcht/lib/courses/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/models.py` & `lino-welcht-23.8.0/lino_welcht/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/courses/ui.py` & `lino-welcht-23.8.0/lino_welcht/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/cv/__init__.py` & `lino-welcht-23.8.0/lino_welcht/lib/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/demo.py` & `lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/std.py` & `lino-welcht-23.8.0/lino_welcht/lib/cv/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/cv/models.py` & `lino-welcht-23.8.0/lino_welcht/lib/cv/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/isip/models.py` & `lino-welcht-23.8.0/lino_welcht/lib/isip/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html` & `lino-welcht-23.8.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/lib/pcsw/models.py` & `lino-welcht-23.8.0/lino_welcht/lib/pcsw/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.mo` & `lino-welcht-23.8.0/lino_welcht/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.po` & `lino-welcht-23.8.0/lino_welcht/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo` & `lino-welcht-23.8.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.po` & `lino-welcht-23.8.0/lino_welcht/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.po` & `lino-welcht-23.8.0/lino_welcht/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/migrate.py` & `lino-welcht-23.8.0/lino_welcht/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/settings.py` & `lino-welcht-23.8.0/lino_welcht/settings.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/lino_welcht/setup_info.py` & `lino-welcht-23.8.0/lino_welcht/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     requires.append('suds-py3')
     # requires.append('suds-jurko')
 
 
 
 SETUP_INFO = dict(
     name='lino-welcht',
-    version='23.6.0',
+    version='23.8.0',
     install_requires=requires,
     test_suite='tests',
     tests_require=['pytest'],
     include_package_data=True,
     zip_safe=False,
     description="A Lino Django application for the PCSW of Châtelet",
     long_description=u"""\
```

### Comparing `lino-welcht-23.6.0/lino_welcht.egg-info/PKG-INFO` & `lino-welcht-23.8.0/lino_welcht.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 23.6.0
+Version: 23.8.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -38,7 +40,9 @@
   `Lino Welfare <https://welfare.lino-framework.org>`__.
 
 - The `French project homepage <https://fr.welfare.lino-framework.org>`__
   contains release notes and end-user docs.
 
 - Online demo site at https://welfare-demo.lino-framework.org
 
+
+
```

### Comparing `lino-welcht-23.6.0/lino_welcht.egg-info/SOURCES.txt` & `lino-welcht-23.8.0/lino_welcht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/requirements.python3.txt` & `lino-welcht-23.8.0/requirements.python3.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/requirements.txt` & `lino-welcht-23.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-23.6.0/tests/__init__.py` & `lino-welcht-23.8.0/tests/__init__.py`

 * *Files identical despite different names*

