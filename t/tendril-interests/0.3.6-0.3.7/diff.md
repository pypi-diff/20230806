# Comparing `tmp/tendril-interests-0.3.6.tar.gz` & `tmp/tendril-interests-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-interests-0.3.6.tar", last modified: Tue Aug  1 21:49:12 2023, max compression
+gzip compressed data, was "tendril-interests-0.3.7.tar", last modified: Sun Aug  6 17:55:00 2023, max compression
```

## Comparing `tendril-interests-0.3.6.tar` & `tendril-interests-0.3.7.tar`

### file list

```diff
@@ -1,110 +1,115 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.305773 tendril-interests-0.3.6/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.6/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.6/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.305773 tendril-interests-0.3.6/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.6/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.309773 tendril-interests-0.3.6/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.6/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.6/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.6/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      812 2023-08-01 11:41:37.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21775 2023-08-01 21:47:57.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.6/src/tendril/apiserver/templates/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.6/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.6/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.6/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.6/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.6/src/tendril/authz/roles/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.6/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.6/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.6/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.6/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.6/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.6/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.6/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.6/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.313773 tendril-interests-0.3.6/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.6/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.6/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.6/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.6/src/tendril/db/controllers/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.6/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.6/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.6/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.6/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.6/src/tendril/db/models/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.6/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    19717 2023-08-01 21:37:28.000000 tendril-interests-0.3.6/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.6/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17517 2023-07-29 04:40:45.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      284 2023-07-29 03:58:12.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6240 2023-07-29 13:52:16.000000 tendril-interests-0.3.6/src/tendril/interests/mixins/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.6/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.6/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.6/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.6/src/tendril/libraries/mixins/interests_approvals.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.6/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1062 2023-07-29 12:20:20.000000 tendril-interests-0.3.6/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.317773 tendril-interests-0.3.6/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2557 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-01 21:49:12.000000 tendril-interests-0.3.6/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-01 21:49:12.321773 tendril-interests-0.3.6/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.6/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.7/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3288 2023-07-29 05:48:32.000000 tendril-interests-0.3.7/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.687314 tendril-interests-0.3.7/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.7/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.7/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.7/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.7/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.691314 tendril-interests-0.3.7/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.7/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      812 2023-08-01 11:41:37.000000 tendril-interests-0.3.7/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21775 2023-08-01 21:47:57.000000 tendril-interests-0.3.7/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.7/src/tendril/apiserver/templates/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.7/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.7/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.7/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.7/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.7/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.7/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.7/src/tendril/authz/roles/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.7/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.7/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.7/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.7/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.7/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.7/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.7/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.7/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.7/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.7/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.7/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril-interests-0.3.7/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 21:22:37.000000 tendril-interests-0.3.7/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      374 2023-08-06 12:44:38.000000 tendril-interests-0.3.7/src/tendril/core/topology/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.7/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.7/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.7/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.7/src/tendril/db/controllers/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.7/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.7/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.7/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.7/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.7/src/tendril/db/models/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.7/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19717 2023-08-01 21:37:28.000000 tendril-interests-0.3.7/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.7/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.7/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17919 2023-08-02 11:53:25.000000 tendril-interests-0.3.7/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      285 2023-08-02 11:44:31.000000 tendril-interests-0.3.7/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    10621 2023-08-06 16:29:09.000000 tendril-interests-0.3.7/src/tendril/interests/mixins/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.7/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.695314 tendril-interests-0.3.7/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.7/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.7/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.7/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.7/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.7/src/tendril/libraries/mixins/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril-interests-0.3.7/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3568 2023-08-06 12:19:06.000000 tendril-interests-0.3.7/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-08-06 17:55:00.000000 tendril-interests-0.3.7/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2662 2023-08-06 17:55:00.000000 tendril-interests-0.3.7/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-08-06 17:55:00.000000 tendril-interests-0.3.7/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      586 2023-08-06 17:55:00.000000 tendril-interests-0.3.7/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-08-06 17:55:00.000000 tendril-interests-0.3.7/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-08-06 17:55:00.699314 tendril-interests-0.3.7/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.7/tox.ini
```

### Comparing `tendril-interests-0.3.6/.gitignore` & `tendril-interests-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/.readthedocs.yml` & `tendril-interests-0.3.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/.travis.yml` & `tendril-interests-0.3.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/LICENSE` & `tendril-interests-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/PKG-INFO` & `tendril-interests-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.6
+Version: 0.3.7
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.6/README.rst` & `tendril-interests-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/Makefile` & `tendril-interests-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/_static/custom.css` & `tendril-interests-0.3.7/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/_static/favicon.ico` & `tendril-interests-0.3.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/_static/logo.png` & `tendril-interests-0.3.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/_static/logo_packed.png` & `tendril-interests-0.3.7/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/_templates/about.html` & `tendril-interests-0.3.7/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/conf.py` & `tendril-interests-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/index.rst` & `tendril-interests-0.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/docs/installation.rst` & `tendril-interests-0.3.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/setup.py` & `tendril-interests-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.3.7/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/apiserver/templates/base.py` & `tendril-interests-0.3.7/src/tendril/apiserver/templates/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.3.7/src/tendril/apiserver/templates/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/apiserver/templates/interests_approvals.py` & `tendril-interests-0.3.7/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/authz/approvals/interests.py` & `tendril-interests-0.3.7/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/authz/approvals/manager.py` & `tendril-interests-0.3.7/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/authz/roles/interests.py` & `tendril-interests-0.3.7/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/authz/roles/interests_approvals.py` & `tendril-interests-0.3.7/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/common/interests/approvals.py` & `tendril-interests-0.3.7/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.3.7/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/common/interests/memberships.py` & `tendril-interests-0.3.7/src/tendril/common/interests/memberships.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/config/__init__.py` & `tendril-interests-0.3.7/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/config/interests.py` & `tendril-interests-0.3.7/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/db/controllers/interests.py` & `tendril-interests-0.3.7/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/db/controllers/interests_approvals.py` & `tendril-interests-0.3.7/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/db/models/interests.py` & `tendril-interests-0.3.7/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/db/models/interests_approvals.py` & `tendril-interests-0.3.7/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/interests/base.py` & `tendril-interests-0.3.7/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/interests/manager.py` & `tendril-interests-0.3.7/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/interests/mixins/approvals.py` & `tendril-interests-0.3.7/src/tendril/interests/mixins/approvals.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from tendril.authz.roles.interests import require_state
 from tendril.authz.roles.interests import require_permission
 
 from tendril.authz.approvals.interests import InterestApprovalSpec
 from tendril.authz.approvals.interests import ApprovalRequirement
 from tendril.common.interests.approvals import ApprovalCollector
 
+from tendril.common.interests.exceptions import ActivationError
 from tendril.db.models.interests_approvals import InterestApprovalModel
 from tendril.db.controllers.interests import get_interest
 from tendril.db.controllers.interests_approvals import get_approval
 from tendril.db.controllers.interests_approvals import register_approval
 from tendril.db.controllers.interests_approvals import withdraw_approval
 
 from .base import InterestMixinBase
 
 from tendril.utils.db import with_db
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 class InterestBaseApprovalTMixin(TendrilTBaseModel):
-    approved: bool
+    has_required_approvals: bool
 
 
 class InterestApprovalsMixin(InterestMixinBase):
     additional_activation_checks = ['check_activation_approvals']
 
     @property
     def approval_spec(self) -> InterestApprovalSpec:
@@ -229,21 +230,28 @@
         logger.info(msg)
         self.model_instance.status = LifecycleStatus.APPROVAL
         return msg
 
     @with_db
     @require_permission('read_approvals', strip_auth=False, required=False)
     def export(self, session=None, auth_user=None, **kwargs):
-        rv = {}
-        if next(self.approvals_pending(auth_user=auth_user, session=session), None):
-            rv['approved'] = False
-        else:
-            rv['approved'] = True
+        # TODO Simplify this by moving the {} creation to the
+        #  ABC and removing the hasattr check.
         if hasattr(super(), 'export'):
-            rv.update(super().export(session=session, auth_user=auth_user, **kwargs))
+            rv = super().export(session=session, auth_user=auth_user, **kwargs)
+        else:
+            rv = {}
+        try:
+            self._check_activation_requirements(session=session)
+            if next(self.approvals_pending(auth_user=auth_user, session=session), None):
+                rv['has_required_approvals'] = False
+            else:
+                rv['has_required_approvals'] = True
+        except ActivationError:
+            rv['has_required_approvals'] = False
         return rv
 
 
 class ApprovalTypeAmbiguity(Exception):
     pass
```

### Comparing `tendril-interests-0.3.6/src/tendril/libraries/interests/base.py` & `tendril-interests-0.3.7/src/tendril/libraries/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.3.7/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.3.7/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.3.6
+Version: 0.3.7
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril-interests-0.3.6/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.3.7/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 src/tendril/common/interests/__init__.py
 src/tendril/common/interests/approvals.py
 src/tendril/common/interests/exceptions.py
 src/tendril/common/interests/memberships.py
 src/tendril/common/interests/representations.py
 src/tendril/config/__init__.py
 src/tendril/config/interests.py
+src/tendril/core/__init__.py
+src/tendril/core/topology/__init__.py
+src/tendril/core/topology/monitors.py
 src/tendril/db/__init__.py
 src/tendril/db/controllers/__init__.py
 src/tendril/db/controllers/interests.py
 src/tendril/db/controllers/interests_approvals.py
 src/tendril/db/mixins/__init__.py
 src/tendril/db/mixins/interests.py
 src/tendril/db/models/__init__.py
```

### Comparing `tendril-interests-0.3.6/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.3.7/src/tendril_interests.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/tests/coveralls.py` & `tendril-interests-0.3.7/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.3.6/tox.ini` & `tendril-interests-0.3.7/tox.ini`

 * *Files identical despite different names*

