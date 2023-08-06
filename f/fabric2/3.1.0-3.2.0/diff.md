# Comparing `tmp/fabric2-3.1.0.tar.gz` & `tmp/fabric2-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmphwn625pb/dist/fabric2-3.1.0.tar", last modified: Thu May 25 18:13:20 2023, max compression
+gzip compressed data, was "/tmp/tmpl3sf8kkh/dist/fabric2-3.2.0.tar", last modified: Sun Aug  6 19:58:57 2023, max compression
```

## Comparing `fabric2-3.1.0.tar` & `fabric2-3.2.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/
--rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric2-3.1.0/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/integration/
--rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-05-12 17:44:52.000000 fabric2-3.1.0/integration/concurrency.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric2-3.1.0/integration/transfer.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/integration/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric2-3.1.0/integration/_support/file.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric2-3.1.0/integration/_support/funky-perms.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric2-3.1.0/integration/group.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-05-12 17:44:52.000000 fabric2-3.1.0/integration/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      549 2023-05-25 18:06:31.000000 fabric2-3.1.0/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2/testing/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric2-3.1.0/fabric2/testing/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5368 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/testing/fixtures.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14911 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/testing/base.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/tunnels.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9086 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/auth.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/group.py
--rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric2-3.1.0/fabric2/__main__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-05-09 23:14:26.000000 fabric2-3.1.0/fabric2/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7979 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric2-3.1.0/fabric2/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric2-3.1.0/fabric2/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14381 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)      540 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6702 2023-05-12 17:44:52.000000 fabric2-3.1.0/fabric2/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    45993 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-25 18:06:31.000000 fabric2-3.1.0/fabric2/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-25 18:13:20.000000 fabric2-3.1.0/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)     2889 2023-05-25 18:12:55.000000 fabric2-3.1.0/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4246 2023-05-25 00:37:09.000000 fabric2-3.1.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3581 2023-05-25 18:13:20.000000 fabric2-3.1.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric2-3.1.0/MANIFEST.in
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/docs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/transfer.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/tunnels.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-25 18:06:31.000000 fabric2-3.1.0/sites/docs/api/auth.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/group.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/api/connection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/upgrading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     5223 2023-05-25 18:06:31.000000 fabric2-3.1.0/sites/docs/cli.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    15384 2023-05-12 17:44:52.000000 fabric2-3.1.0/sites/docs/getting-started.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-05-12 17:44:52.000000 fabric2-3.1.0/sites/docs/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/docs/concepts/networking.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10676 2023-05-25 18:06:31.000000 fabric2-3.1.0/sites/docs/concepts/configuration.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     4078 2023-05-11 20:34:05.000000 fabric2-3.1.0/sites/docs/concepts/authentication.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/_shared_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/_shared_static/logo.png
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric2-3.1.0/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-05-12 17:44:52.000000 fabric2-3.1.0/sites/www/upgrading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric2-3.1.0/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/www/troubleshooting.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric2-3.1.0/sites/www/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric2-3.1.0/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-05-12 17:44:52.000000 fabric2-3.1.0/sites/www/changelog-v1.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric2-3.1.0/sites/www/roadmap.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    17277 2023-05-25 18:13:19.000000 fabric2-3.1.0/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric2-3.1.0/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric2-3.1.0/sites/www/installing-1.x.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-05-12 17:44:52.000000 fabric2-3.1.0/sites/shared_conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric2-3.1.0/LICENSE
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       70 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3581 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     2724 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        8 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2023-05-25 18:13:20.000000 fabric2-3.1.0/fabric2.egg-info/entry_points.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    59810 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2114 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/_util.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/json_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/json_conf/fabric.json
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/json_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/runtime_fabfile.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/ssh_config/
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/overridden_hostname.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/system.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/proxyjump_recursive.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/proxyjump_multi.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/runtime_identity.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/proxyjump.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/user.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/both_proxies.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/runtime.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/ssh_config/proxyjump_multi_recursive.conf
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/yaml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/yaml_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/yaml_conf/fabric.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/config.yml
--rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/prompting.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/py_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/py_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/py_conf/fabric.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/fabfile.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric2-3.1.0/tests/_support/yml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric2-3.1.0/tests/_support/yml_conf/fabric.yml
--rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric2-3.1.0/tests/_support/yml_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/group.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1301 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1197 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10450 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/auth.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7306 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14899 2023-05-25 18:06:31.000000 fabric2-3.1.0/tests/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-05-12 17:44:52.000000 fabric2-3.1.0/tests/util.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2/
+-rw-r--r--   0 jforcier  (1000) users      (100)     9086 2023-05-25 18:06:31.000000 fabric2-3.2.0/fabric2/auth.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6702 2023-05-12 17:44:52.000000 fabric2-3.2.0/fabric2/runners.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2/testing/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5971 2023-08-06 19:57:05.000000 fabric2-3.2.0/fabric2/testing/fixtures.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric2-3.2.0/fabric2/testing/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19833 2023-08-06 19:57:05.000000 fabric2-3.2.0/fabric2/testing/base.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14381 2023-05-25 18:06:31.000000 fabric2-3.2.0/fabric2/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    45993 2023-08-06 01:05:05.000000 fabric2-3.2.0/fabric2/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-05-09 23:14:26.000000 fabric2-3.2.0/fabric2/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7979 2023-05-25 18:06:31.000000 fabric2-3.2.0/fabric2/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-08-06 01:35:24.000000 fabric2-3.2.0/fabric2/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric2-3.2.0/fabric2/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-05-12 17:44:52.000000 fabric2-3.2.0/fabric2/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric2-3.2.0/fabric2/exceptions.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-08-06 19:58:56.000000 fabric2-3.2.0/fabric2/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-05-12 17:44:52.000000 fabric2-3.2.0/fabric2/tunnels.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-05-12 17:44:52.000000 fabric2-3.2.0/fabric2/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      540 2023-05-25 18:06:31.000000 fabric2-3.2.0/fabric2/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric2-3.2.0/fabric2/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-08-06 19:58:57.000000 fabric2-3.2.0/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        8 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2741 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3581 2023-08-06 19:58:57.000000 fabric2-3.2.0/fabric2.egg-info/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/integration/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/integration/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric2-3.2.0/integration/_support/file.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric2-3.2.0/integration/_support/funky-perms.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric2-3.2.0/integration/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-08-06 19:57:05.000000 fabric2-3.2.0/integration/concurrency.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-05-12 17:44:52.000000 fabric2-3.2.0/integration/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric2-3.2.0/integration/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      475 2023-08-06 19:57:05.000000 fabric2-3.2.0/dev-requirements.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2889 2023-08-02 23:50:20.000000 fabric2-3.2.0/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4246 2023-05-25 00:37:09.000000 fabric2-3.2.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3581 2023-08-06 19:58:57.000000 fabric2-3.2.0/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric2-3.2.0/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric2-3.2.0/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric2-3.2.0/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/www/troubleshooting.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric2-3.2.0/sites/www/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric2-3.2.0/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-05-12 17:44:52.000000 fabric2-3.2.0/sites/www/changelog-v1.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    18529 2023-08-06 19:58:53.000000 fabric2-3.2.0/sites/www/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric2-3.2.0/sites/www/roadmap.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/www/installing-1.x.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric2-3.2.0/sites/www/installing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-05-12 17:44:52.000000 fabric2-3.2.0/sites/www/upgrading.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/_shared_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/_shared_static/logo.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-05-12 17:44:52.000000 fabric2-3.2.0/sites/shared_conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/upgrading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    15402 2023-08-06 19:57:05.000000 fabric2-3.2.0/sites/docs/getting-started.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/connection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/transfer.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-25 18:06:31.000000 fabric2-3.2.0/sites/docs/api/auth.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/group.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/tunnels.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)     4078 2023-05-11 20:34:05.000000 fabric2-3.2.0/sites/docs/concepts/authentication.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10676 2023-05-25 18:06:31.000000 fabric2-3.2.0/sites/docs/concepts/configuration.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric2-3.2.0/sites/docs/concepts/networking.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-05-12 17:44:52.000000 fabric2-3.2.0/sites/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5223 2023-05-25 18:06:31.000000 fabric2-3.2.0/sites/docs/cli.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric2-3.2.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric2-3.2.0/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-08-06 01:37:19.000000 fabric2-3.2.0/tests/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7307 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-05-12 17:44:52.000000 fabric2-3.2.0/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14899 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-05-12 17:44:52.000000 fabric2-3.2.0/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    59810 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10450 2023-05-25 18:06:31.000000 fabric2-3.2.0/tests/auth.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1197 2023-05-25 18:06:31.000000 fabric2-3.2.0/tests/conftest.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/ssh_config/
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/proxyjump.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/user.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/both_proxies.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/proxyjump_multi.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/overridden_hostname.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/runtime.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/_support/ssh_config/runtime_identity.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/system.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/proxyjump_multi_recursive.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/ssh_config/proxyjump_recursive.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/runtime_fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/yaml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/yaml_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/yaml_conf/fabric.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/py_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/py_conf/fabric.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/py_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/yml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/yml_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/yml_conf/fabric.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-08-06 19:58:57.000000 fabric2-3.2.0/tests/_support/json_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/json_conf/fabric.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/json_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric2-3.2.0/tests/_support/prompting.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric2-3.2.0/tests/_support/config.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-05-12 17:44:52.000000 fabric2-3.2.0/tests/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2114 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-05-12 17:44:52.000000 fabric2-3.2.0/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1301 2023-05-25 18:06:31.000000 fabric2-3.2.0/tests/init.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4064 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/testing.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-08-06 19:57:05.000000 fabric2-3.2.0/tests/config.py
```

### Comparing `fabric2-3.1.0/README.rst` & `fabric2-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/integration/concurrency.py` & `fabric2-3.2.0/integration/concurrency.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         skip()
         # Kind of silly but a nice base case for "how would someone thread this
         # stuff; and are there any bizarre gotchas lurking in default
         # config/context/connection state?"
         # Specifically, cut up the local (usually 100k's long) words dict into
         # per-thread chunks, then read those chunks via shell command, as a
         # crummy "make sure each thread isn't polluting things like stored
-        # stdout" sanity test
+        # stdout" safety test
         queue = Queue()
         # TODO: skip test on Windows or find suitable alternative file
         with codecs.open(_words, encoding="utf-8") as fd:
             data = [x.strip() for x in fd.readlines()]
         threads = []
         num_words = len(data)
         chunksize = len(data) / len(self.cxns)  # will be an int, which is fine
```

### Comparing `fabric2-3.1.0/integration/transfer.py` & `fabric2-3.2.0/integration/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/integration/group.py` & `fabric2-3.2.0/integration/group.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/integration/connection.py` & `fabric2-3.2.0/integration/connection.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/testing/fixtures.py` & `fabric2-3.2.0/fabric2/testing/fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,29 +64,46 @@
 
 #: A convenience rebinding of `connection`.
 #:
 #: .. versionadded:: 2.1
 cxn = connection
 
 
+# TODO 4.0: remove old remote() and make this the new remote()
+@fixture
+def remote_with_sftp():
+    """
+    Like `remote`, but with ``enable_sftp=True``.
+
+    To access the internal mocked SFTP client (eg for asserting SFTP
+    functionality was called), note that the returned `MockRemote` object has a
+    ``.sftp`` attribute when created in this mode.
+    """
+    # NOTE: recall that by default an instantiated MockRemote has a single
+    # internal anonymous session; so these fixtures are useful for autouse
+    # guardrails.
+    with MockRemote(enable_sftp=True) as remote:
+        yield remote
+
+
 @fixture
 def remote():
     """
     Fixture allowing setup of a mocked remote session & access to sub-mocks.
 
     Yields a `.MockRemote` object (which may need to be updated via
     `.MockRemote.expect`, `.MockRemote.expect_sessions`, etc; otherwise a
-    default session will be used) & calls `.MockRemote.sanity` and
+    default session will be used) & calls `.MockRemote.safety` and
     `.MockRemote.stop` on teardown.
 
     .. versionadded:: 2.1
     """
     remote = MockRemote()
     yield remote
-    remote.sanity()
+    remote.safety()
     remote.stop()
 
 
 @fixture
 def sftp():
     """
     Fixture allowing setup of a mocked remote SFTP session.
```

### Comparing `fabric2-3.1.0/fabric2/testing/base.py` & `fabric2-3.2.0/fabric2/testing/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,20 +11,26 @@
     grabbing ``fabric[pytest]`` instead, which encompasses the dependencies of
     both this module and the `fabric.testing.fixtures` module, which contains
     pytest fixtures.
 
 .. versionadded:: 2.1
 """
 
+import os
 from itertools import chain, repeat
 from io import BytesIO
-import os
-
 from unittest.mock import Mock, PropertyMock, call, patch, ANY
 
+from deprecated.sphinx import deprecated
+from deprecated.classic import deprecated as deprecated_no_docstring
+
+
+# TODO 4.0: reorganize harder (eg building blocks in one module, central
+# classes in another?)
+
 
 class Command:
     """
     Data record specifying params of a command execution to mock/expect.
 
     :param str cmd:
         Command string to expect. If not given, no expectations about the
@@ -135,37 +141,51 @@
         Iterable of `.Command` objects, used when mocking nontrivial sessions
         involving >1 command execution per host. Default: ``None``.
 
         .. note::
             Giving ``cmd``, ``out`` etc alongside explicit ``commands`` is not
             allowed and will result in an error.
 
+    :param bool enable_sftp: Whether to enable basic SFTP mocking support.
+
+    :param transfers:
+        None if no transfers to expect; otherwise, should be a list of dicts of
+        the form ``{"method": "get|put", **kwargs}`` where ``**kwargs`` are the
+        kwargs expected in the relevant `~paramiko.sftp_client.SFTPClient`
+        method. (eg: ``{"method": "put", "localpath": "/some/path"}``)
+
     .. versionadded:: 2.1
+    .. versionchanged:: 3.2
+        Added the ``enable_sftp`` and ``transfers`` parameters.
     """
 
     def __init__(
         self,
         host=None,
         user=None,
         port=None,
         commands=None,
         cmd=None,
         out=None,
         in_=None,
         err=None,
         exit=None,
         waits=None,
+        enable_sftp=False,
+        transfers=None,
     ):
-        # Sanity check
+        # Safety check
         params = cmd or out or err or exit or waits
         if commands and params:
             raise ValueError(
                 "You can't give both 'commands' and individual "
                 "Command parameters!"
             )  # noqa
+        # Early test for "did user actually request expectations?"
+        self.guard_only = not (commands or cmd or transfers)
         # Fill in values
         self.host = host
         self.user = user
         self.port = port
         self.commands = commands
         if params:
             # Honestly dunno which is dumber, this or duplicating Command's
@@ -182,14 +202,16 @@
             if exit is not None:
                 kwargs["exit"] = exit
             if waits is not None:
                 kwargs["waits"] = waits
             self.commands = [Command(**kwargs)]
         if not self.commands:
             self.commands = [Command()]
+        self._enable_sftp = enable_sftp
+        self.transfers = transfers
 
     def generate_mocks(self):
         """
         Mocks `~paramiko.client.SSHClient` and `~paramiko.channel.Channel`.
 
         Specifically, the client will expect itself to be connected to
         ``self.host`` (if given), the channels will be associated with the
@@ -237,18 +259,62 @@
 
             channels.append(channel)
 
         # Have our transport yield those channel mocks in order when
         # open_session() is called.
         transport.open_session.side_effect = channels
 
+        # SFTP, if enabled
+        if self._enable_sftp:
+            self._start_sftp(client)
+
         self.client = client
         self.channels = channels
 
+    def _start_sftp(self, client):
+        # Patch os module for local stat and similar
+        self.os_patcher = patch("fabric.transfer.os")
+        mock_os = self.os_patcher.start()
+        # Patch Path class inside transfer.py to prevent real fs touchery
+        self.path_patcher = patch("fabric.transfer.Path")
+        self.path_patcher.start()
+        self.sftp = sftp = client.open_sftp.return_value
+
+        # Handle common filepath massage actions; tests will assume these.
+        def fake_abspath(path):
+            # Run normpath to avoid tests not seeing abspath wrinkles (like
+            # trailing slash chomping)
+            return "/local/{}".format(os.path.normpath(path))
+
+        mock_os.path.abspath.side_effect = fake_abspath
+        sftp.getcwd.return_value = "/remote"
+        # Ensure stat st_mode is a real number; Python 3's stat.S_IMODE doesn't
+        # like just being handed a MagicMock?
+        fake_mode = 0o644  # arbitrary real-ish mode
+        sftp.stat.return_value.st_mode = fake_mode
+        mock_os.stat.return_value.st_mode = fake_mode
+        # Not super clear to me why the 'wraps' functionality in mock isn't
+        # working for this :( reinstate a bunch of os(.path) so it still works
+        mock_os.sep = os.sep
+        for name in ("basename", "split", "join", "normpath"):
+            getattr(mock_os.path, name).side_effect = getattr(os.path, name)
+
+    @deprecated_no_docstring(
+        version="3.2",
+        reason="This method has been renamed to `safety_check` & will be removed in 4.0",  # noqa
+    )
     def sanity_check(self):
+        return self.safety_check()
+
+    def safety_check(self):
+        # Short-circuit if user didn't give any expectations; otherwise our
+        # assumptions below will be inaccurately violated and explode.
+        if self.guard_only:
+            return
+
         # Per-session we expect a single transport get
         transport = self.client.get_transport
         transport.assert_called_once_with()
         # And a single connect to our target host.
         self.client.connect.assert_called_once_with(
             username=self.user or ANY,
             hostname=self.host or ANY,
@@ -269,44 +335,73 @@
             if command.in_:
                 assert channel._stdin.getvalue() == command.in_
 
         # Make sure open_session was called expected number of times.
         calls = transport.return_value.open_session.call_args_list
         assert calls == session_opens
 
+        # SFTP transfers
+        for transfer in self.transfers or []:
+            method_name = transfer.pop("method")
+            method = getattr(self.sftp, method_name)
+            method.assert_any_call(**transfer)
+
+    def stop(self):
+        """
+        Stop any internal per-session mocks.
+
+        .. versionadded:: 3.2
+        """
+        if hasattr(self, "os_patcher"):
+            self.os_patcher.stop()
+        if hasattr(self, "path_patcher"):
+            self.path_patcher.stop()
+
 
 class MockRemote:
     """
-    Class representing mocked remote state.
+    Class representing mocked remote SSH/SFTP state.
 
-    By default this class is set up for start/stop style patching as opposed to
-    the more common context-manager or decorator approach; this is so it can be
-    used in situations requiring setup/teardown semantics.
-
-    Defaults to setting up a single anonymous `Session`, so it can be used as a
-    "request & forget" pytest fixture. Users requiring detailed remote session
-    expectations can call methods like `expect`, which wipe that anonymous
-    Session & set up a new one instead.
+    It supports stop/start style patching (useful for doctests) but then wraps
+    that in a more convenient/common contextmanager pattern (useful in most
+    other situations). The latter is also leveraged by the
+    `fabric.testing.fixtures` module, recommended if you're using pytest.
+
+    Note that the `expect` and `expect_sessions` methods automatically call
+    `start`, so you won't normally need to do so by hand.
+
+    By default, a single anonymous/internal `Session` is created, for
+    convenience (eg mocking out SSH functionality as a safety measure). Users
+    requiring detailed remote session expectations can call methods like
+    `expect` or `expect_sessions`, which wipe that anonymous Session & set up a
+    new one instead.
 
     .. versionadded:: 2.1
+    .. versionchanged:: 3.2
+        Added the ``enable_sftp`` init kwarg to enable mocking both SSH and
+        SFTP at the same time.
+    .. versionchanged:: 3.2
+        Added contextmanager semantics to the class, so you don't have to
+        remember to call `safety`/`stop`.
     """
 
-    def __init__(self):
-        self.expect_sessions(Session())
-
-    # TODO: make it easier to assume single session w/ >1 command?
+    # TODO 4.0: delete enable_sftp and make its behavior default
+    def __init__(self, enable_sftp=False):
+        self._enable_sftp = enable_sftp
+        self.expect_sessions(Session(enable_sftp=enable_sftp))
 
     def expect(self, *args, **kwargs):
         """
         Convenience method for creating & 'expect'ing a single `Session`.
 
         Returns the single `MockChannel` yielded by that Session.
 
         .. versionadded:: 2.1
         """
+        kwargs.setdefault("enable_sftp", self._enable_sftp)
         return self.expect_sessions(Session(*args, **kwargs))[0]
 
     def expect_sessions(self, *sessions):
         """
         Sets the mocked remote environment to expect the given ``sessions``.
 
         Returns a list of `MockChannel` objects, one per input `Session`.
@@ -317,60 +412,90 @@
         # be running.
         self.stop()
         # Update sessions list with new session(s)
         self.sessions = sessions
         # And start patching again, returning mocked channels
         return self.start()
 
+    # TODO 4.0: definitely clean this up once the SFTP bit isn't opt-in, doing
+    # that backwards compatibly was real gross
     def start(self):
         """
         Start patching SSHClient with the stored sessions, returning channels.
 
         .. versionadded:: 2.1
         """
         # Patch SSHClient so the sessions' generated mocks can be set as its
         # return values
         self.patcher = patcher = patch("fabric.connection.SSHClient")
         SSHClient = patcher.start()
-        # Mock clients, to be inspected afterwards during sanity-checks
+        # Mock clients, to be inspected afterwards during safety-checks
         clients = []
         for session in self.sessions:
             session.generate_mocks()
             clients.append(session.client)
         # Each time the mocked SSHClient class is instantiated, it will
-        # yield one of our mocked clients (w/ mocked transport & channel)
-        # generated above.
+        # yield one of our mocked clients (w/ mocked transport & channel, and
+        # optionally SFTP subclient) generated above.
         SSHClient.side_effect = clients
-        return list(chain.from_iterable(x.channels for x in self.sessions))
+        sessions = list(chain.from_iterable(x.channels for x in self.sessions))
+        # TODO: in future we _may_ want to change this so it returns SFTP file
+        # data as well?
+        return sessions
 
     def stop(self):
         """
         Stop patching SSHClient.
 
         .. versionadded:: 2.1
         """
         # Short circuit if we don't seem to have start()ed yet.
         if not hasattr(self, "patcher"):
             return
         # Stop patching SSHClient
         self.patcher.stop()
+        # Also ask all sessions to stop any of their self-owned mocks
+        for session in self.sessions:
+            session.stop()
 
+    @deprecated(
+        version="3.2",
+        reason="This method has been renamed to `safety` & will be removed in 4.0",  # noqa
+    )
     def sanity(self):
         """
         Run post-execution sanity checks (usually 'was X called' tests.)
 
         .. versionadded:: 2.1
         """
+        return self.safety()
+
+    def safety(self):
+        """
+        Run post-execution safety checks (eg ensuring expected calls happened).
+
+        .. versionadded:: 3.2
+        """
         for session in self.sessions:
-            # Basic sanity tests about transport, channel etc
-            session.sanity_check()
+            session.safety_check()
 
+    def __enter__(self):
+        return self
 
-# TODO: unify with the stuff in paramiko itself (now in its tests/conftest.py),
-# they're quite distinct and really shouldn't be.
+    def __exit__(self, *exc):
+        try:
+            self.safety()
+        finally:
+            self.stop()
+
+
+@deprecated(
+    version="3.2",
+    reason="This class has been merged with `MockRemote` which can now handle SFTP mocking too. Please switch to it!",  # noqa
+)
 class MockSFTP:
     """
     Class managing mocked SFTP remote state.
 
     Used in start/stop fashion in eg doctests; wrapped in the SFTP fixtures in
     conftest.py for main use.
```

### Comparing `fabric2-3.1.0/fabric2/transfer.py` & `fabric2-3.2.0/fabric2/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/tunnels.py` & `fabric2-3.2.0/fabric2/tunnels.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/auth.py` & `fabric2-3.2.0/fabric2/auth.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/group.py` & `fabric2-3.2.0/fabric2/group.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/util.py` & `fabric2-3.2.0/fabric2/util.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/main.py` & `fabric2-3.2.0/fabric2/main.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/exceptions.py` & `fabric2-3.2.0/fabric2/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/tasks.py` & `fabric2-3.2.0/fabric2/tasks.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/executor.py` & `fabric2-3.2.0/fabric2/executor.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/config.py` & `fabric2-3.2.0/fabric2/config.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/__init__.py` & `fabric2-3.2.0/fabric2/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/runners.py` & `fabric2-3.2.0/fabric2/runners.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2/connection.py` & `fabric2-3.2.0/fabric2/connection.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tasks.py` & `fabric2-3.2.0/tasks.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/setup.py` & `fabric2-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/PKG-INFO` & `fabric2-3.2.0/fabric2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric2
-Version: 3.1.0
+Version: 3.2.0
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
```

### Comparing `fabric2-3.1.0/sites/docs/api/testing.rst` & `fabric2-3.2.0/sites/docs/api/testing.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/index.rst` & `fabric2-3.2.0/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/cli.rst` & `fabric2-3.2.0/sites/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/getting-started.rst` & `fabric2-3.2.0/sites/docs/getting-started.rst`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
 Besides shell command execution, the other common use of SSH connections is
 file transfer; `.Connection.put` and `.Connection.get` exist to fill this need.
 For example, say you had an archive file you wanted to upload:
 
 .. testsetup:: transfers
 
-    mock = MockSFTP()
+    mock = MockRemote(enable_sftp=True)
 
 .. testcleanup:: transfers
 
     mock.stop()
 
 .. doctest:: transfers
```

### Comparing `fabric2-3.1.0/sites/docs/conf.py` & `fabric2-3.2.0/sites/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/concepts/networking.rst` & `fabric2-3.2.0/sites/docs/concepts/networking.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/concepts/configuration.rst` & `fabric2-3.2.0/sites/docs/concepts/configuration.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/docs/concepts/authentication.rst` & `fabric2-3.2.0/sites/docs/concepts/authentication.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/_shared_static/logo.png` & `fabric2-3.2.0/sites/_shared_static/logo.png`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/installing.rst` & `fabric2-3.2.0/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/upgrading.rst` & `fabric2-3.2.0/sites/www/upgrading.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/contact.rst` & `fabric2-3.2.0/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/troubleshooting.rst` & `fabric2-3.2.0/sites/www/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/index.rst` & `fabric2-3.2.0/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/development.rst` & `fabric2-3.2.0/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/changelog-v1.rst` & `fabric2-3.2.0/sites/www/changelog-v1.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/roadmap.rst` & `fabric2-3.2.0/sites/www/roadmap.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/faq.rst` & `fabric2-3.2.0/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/changelog.rst` & `fabric2-3.2.0/sites/www/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,36 @@
     Keep in mind that Fabric is largely a wrapper around `Paramiko
     <https://paramiko.org/changelog.html>`_  and `Invoke
     <https://pyinvoke.org/changelog.html>`_ - Fabric's capabilities can often
     improve simply by upgrading your copies of those libraries! Click their
     names in this paragraph to visit their changelogs and see what you might get
     if you upgrade your dependencies.
 
+- :release:`3.2.0 <2023-08-06>`
+- :feature:`-` Enhanced `fabric.testing` in ways large and small:
+
+    - Backwards-compatibly merged the functionality of
+      `~fabric.testing.base.MockSFTP` into `~fabric.testing.base.MockRemote`
+      (may be opted-into by instantiating the latter with ``enable_sftp=True``)
+      so you can mock out both SSH *and* SFTP functionality in the same test,
+      which was previously impossible. It also means you can use this in a
+      Pytest autouse fixture to prevent any tests from accidentally hitting the
+      network!
+    - A new pytest fixture, `~fabric.testing.fixtures.remote_with_sftp`, has
+      been added which leverages the previous bullet point (an all-in-one
+      fixture suitable for, eg, preventing any incidental ssh/sftp attempts
+      during test execution).
+    - A pile of documentation and test enhancements (yes, testing our testing
+      helpers is a thing).
+
+- :support:`-` Language update: applied `s/sanity/safety/g` to the codebase
+  (with the few actual API members using the term now marked deprecated & new
+  ones added in the meantime, mostly in `fabric.testing`).
+- :support:`-` Added a new runtime dependency on the `Deprecated
+  <https://pypi.org/project/Deprecated/>`_ library.
 - :release:`3.1.0 <2023-05-25>`
 - :feature:`-` Implement opt-in support for Paramiko 3.2's
   `~paramiko.auth_strategy.AuthStrategy` machinery, as follows:
 
   - Added a new module and class, `fabric.auth.OpenSSHAuthStrategy`, which
     leverages aforementioned new Paramiko functionality to marry loaded SSH
     config files with Fabric-level and runtime-level parameters, arriving at
```

### Comparing `fabric2-3.1.0/sites/www/conf.py` & `fabric2-3.2.0/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/www/installing-1.x.rst` & `fabric2-3.2.0/sites/www/installing-1.x.rst`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/sites/shared_conf.py` & `fabric2-3.2.0/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/LICENSE` & `fabric2-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/fabric2.egg-info/PKG-INFO` & `fabric2-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric2
-Version: 3.1.0
+Version: 3.2.0
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
```

### Comparing `fabric2-3.1.0/fabric2.egg-info/SOURCES.txt` & `fabric2-3.2.0/fabric2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 tests/connection.py
 tests/executor.py
 tests/group.py
 tests/init.py
 tests/main.py
 tests/runners.py
 tests/task.py
+tests/testing.py
 tests/transfer.py
 tests/util.py
 tests/_support/config.yml
 tests/_support/fabfile.py
 tests/_support/prompting.py
 tests/_support/runtime_fabfile.py
 tests/_support/json_conf/fabfile.py
```

### Comparing `fabric2-3.1.0/tests/config.py` & `fabric2-3.2.0/tests/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             Config(overrides={"load_ssh_configs": False})
             assert not method.called
 
         @patch.object(Config, "_load_ssh_file")
         def does_not_affect_explicit_object(self, method):
             sc = SSHConfig()
             c = Config(ssh_config=sc, overrides={"load_ssh_configs": False})
-            # Implicit loading still doesn't happen...sanity check
+            # Implicit loading still doesn't happen...safety check
             assert not method.called
             # Real test: the obj we passed in is present as usual
             assert c.base_ssh_config is sc
 
         @patch.object(Config, "_load_ssh_file")
         def does_not_skip_loading_runtime_path(self, method):
             Config(
```

### Comparing `fabric2-3.1.0/tests/connection.py` & `fabric2-3.2.0/tests/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
 
                 def gateway_Connections_get_parent_connection_configs(self):
                     conf = self._runtime_config(
                         basename="proxyjump",
                         overrides={"some_random_option": "a-value"},
                     )
                     cxn = Connection("runtime", config=conf)
-                    # Sanity
+                    # Safety
                     assert cxn.config is conf
                     assert cxn.gateway == self._expected_gw
                     # Real check
                     assert cxn.gateway.config.some_random_option == "a-value"
                     # Prove copy not reference
                     # TODO: would we ever WANT a reference? can't imagine...
                     assert cxn.gateway.config is not conf
@@ -1155,15 +1155,15 @@
             # own Mock having the same ID here and in code under test. WTF!!)
             expected = [
                 call(context=cxn, inline_env=True),
                 call().run(cmd, watchers=ANY),
             ]
             assert Remote.mock_calls == expected
             # NOTE: we used to have a "sudo return value is literally the same
-            # return value from Remote.run()" sanity check here, which is
+            # return value from Remote.run()" safety check here, which is
             # completely impossible now thanks to the above issue.
 
         def per_host_password_works_as_expected(self):
             # TODO: needs clearly defined "per-host" config API, if a distinct
             # one is necessary besides "the config obj handed in when
             # instantiating the Connection".
             # E.g. generate a Connection pulling in a sudo.password value from
```

### Comparing `fabric2-3.1.0/tests/executor.py` & `fabric2-3.2.0/tests/executor.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/_util.py` & `fabric2-3.2.0/tests/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         gateway=None,
         host_string="localghost",
         key_filename=None,
         no_agent=False,
         password=None,
         port=22,
         ssh_config_path=None,
-        # Used in a handful of sanity tests, so it gets a 'real' value. eh.
+        # Used in a handful of safety tests, so it gets a 'real' value. eh.
         sudo_password="nope",
         sudo_prompt=None,
         timeout=None,
         use_ssh_config=False,
         user="localuser",
         warn_only=False,
     )
```

### Comparing `fabric2-3.1.0/tests/_support/fabfile.py` & `fabric2-3.2.0/tests/_support/fabfile.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/group.py` & `fabric2-3.2.0/tests/group.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/init.py` & `fabric2-3.2.0/tests/init.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/conftest.py` & `fabric2-3.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/auth.py` & `fabric2-3.2.0/tests/auth.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/task.py` & `fabric2-3.2.0/tests/task.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/transfer.py` & `fabric2-3.2.0/tests/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric2-3.1.0/tests/runners.py` & `fabric2-3.2.0/tests/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 "PATH" in env
             )  # assuming this will be in every test environment
             assert "JUST" in env
             assert env["JUST"] == "ME"
 
     class run:
         def calls_expected_paramiko_bits(self, remote):
-            # remote mocking makes generic sanity checks like "were
+            # remote mocking makes generic safety checks like "were
             # get_transport and open_session called", but we also want to make
             # sure that exec_command got run with our arg to run().
             remote.expect(cmd=CMD)
             _runner().run(CMD)
 
         def writes_remote_streams_to_local_streams(self, remote):
             remote.expect(out=b"hello yes this is dog")
@@ -54,15 +54,15 @@
             _runner().run(CMD, out_stream=fakeout)
             assert fakeout.getvalue() == "hello yes this is dog"
 
         def return_value_is_Result_subclass_exposing_cxn_used(self, remote):
             c = _Connection("host")
             result = Remote(context=c).run(CMD)
             assert isinstance(result, Result)
-            # Mild sanity test for other Result superclass bits
+            # Mild safety check for other Result superclass bits
             assert result.ok is True
             assert result.exited == 0
             # Test the attr our own subclass adds
             assert result.connection is c
 
         def channel_is_closed_normally(self, remote):
             chan = remote.expect()
```

### Comparing `fabric2-3.1.0/tests/main.py` & `fabric2-3.2.0/tests/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         def uses_FABRIC_env_prefix(self, environ):
             environ["FABRIC_RUN_ECHO"] = "1"
             with cd(support):
                 make_program().run("fab expect-from-env")
 
         def basic_pre_and_post_tasks_still_work(self):
             with cd(support):
-                # Sanity
+                # Safety
                 expect("first", "First!\n")
                 expect("third", "Third!\n")
                 # Real test
                 expect("second", "First!\nSecond!\nThird!\n")
 
     class filenames:
         def loads_fabfile_not_tasks(self):
@@ -362,15 +362,15 @@
         @trap
         def complete_flag_does_not_trigger_remainder_only_behavior(self):
             # When bug present, 'fab --complete -- fab' fails to load any
             # collections because it thinks it's in remainder-only,
             # work-without-a-collection mode.
             with cd(support):
                 make_program().run("fab --complete -- fab", exit=False)
-            # Cherry-picked sanity checks looking for tasks from fixture
+            # Cherry-picked safety checks looking for tasks from fixture
             # fabfile
             output = sys.stdout.getvalue()
             for name in ("build", "deploy", "expect-from-env"):
                 assert name in output
 
 
 class main:
```

### Comparing `fabric2-3.1.0/tests/util.py` & `fabric2-3.2.0/tests/util.py`

 * *Files identical despite different names*

