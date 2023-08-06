# Comparing `tmp/pynose-1.4.7.tar.gz` & `tmp/pynose-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynose-1.4.7.tar", last modified: Mon Jul 31 02:20:42 2023, max compression
+gzip compressed data, was "pynose-1.4.8.tar", last modified: Sun Aug  6 18:03:36 2023, max compression
```

## Comparing `pynose-1.4.7.tar` & `pynose-1.4.8.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.451276 pynose-1.4.7/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.442920 pynose-1.4.7/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.444496 pynose-1.4.7/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.7/.github/workflows/python-package-legacy.yml
--rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.7/.github/workflows/python-package.yml
--rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.7/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.7/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.7/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-31 02:20:42.451355 pynose-1.4.7/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)    17086 2023-07-08 03:28:10.000000 pynose-1.4.7/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.444932 pynose-1.4.7/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.7/bin/nosetests
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.7/bin/pynose
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.447395 pynose-1.4.7/nose/
--rw-r--r--   0 michael    (501) staff       (20)      643 2023-07-07 23:53:47.000000 pynose-1.4.7/nose/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      144 2023-07-07 23:40:25.000000 pynose-1.4.7/nose/__main__.py
--rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/case.py
--rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.7/nose/commands.py
--rw-r--r--   0 michael    (501) staff       (20)    24529 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/config.py
--rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.7/nose/core.py
--rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.7/nose/exc.py
--rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.7/nose/failure.py
--rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/importer.py
--rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.7/nose/inspector.py
--rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.7/nose/loader.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.449999 pynose-1.4.7/nose/plugins/
--rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.7/nose/plugins/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.7/nose/plugins/allmodules.py
--rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.7/nose/plugins/attrib.py
--rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.7/nose/plugins/base.py
--rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.7/nose/plugins/builtin.py
--rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.7/nose/plugins/capture.py
--rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.7/nose/plugins/collect.py
--rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.7/nose/plugins/cover.py
--rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.7/nose/plugins/debug.py
--rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.7/nose/plugins/deprecated.py
--rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.7/nose/plugins/doctests.py
--rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.7/nose/plugins/errorclass.py
--rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.7/nose/plugins/failuredetail.py
--rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.7/nose/plugins/isolate.py
--rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.7/nose/plugins/logcapture.py
--rw-r--r--   0 michael    (501) staff       (20)    15004 2023-07-08 03:28:10.000000 pynose-1.4.7/nose/plugins/manager.py
--rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.7/nose/plugins/multiprocess.py
--rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.7/nose/plugins/plugintest.py
--rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.7/nose/plugins/skip.py
--rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.7/nose/plugins/testid.py
--rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.7/nose/plugins/xunit.py
--rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.7/nose/proxy.py
--rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.7/nose/pyversion.py
--rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/result.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.7/nose/selector.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.450242 pynose-1.4.7/nose/sphinx/
--rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.7/nose/sphinx/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.7/nose/sphinx/pluginopts.py
--rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.7/nose/suite.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.450595 pynose-1.4.7/nose/tools/
--rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.7/nose/tools/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.7/nose/tools/nontrivial.py
--rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.7/nose/tools/trivial.py
--rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.7/nose/twistedtools.py
--rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.7/nose/usage.txt
--rw-r--r--   0 michael    (501) staff       (20)    18927 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.451176 pynose-1.4.7/pynose.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1273 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       86 2023-07-31 02:20:42.451605 pynose-1.4.7/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     5413 2023-07-31 02:19:59.000000 pynose-1.4.7/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.151667 pynose-1.4.8/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.141867 pynose-1.4.8/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.143348 pynose-1.4.8/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.8/.github/workflows/python-package-legacy.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.8/.github/workflows/python-package.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.8/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.8/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.8/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-08-06 18:03:36.151743 pynose-1.4.8/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)    17086 2023-07-08 03:28:10.000000 pynose-1.4.8/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.143895 pynose-1.4.8/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.8/bin/nosetests
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.8/bin/pynose
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.146948 pynose-1.4.8/nose/
+-rw-r--r--   0 michael    (501) staff       (20)      643 2023-07-07 23:53:47.000000 pynose-1.4.8/nose/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      144 2023-07-07 23:40:25.000000 pynose-1.4.8/nose/__main__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-08-06 18:02:05.000000 pynose-1.4.8/nose/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.8/nose/case.py
+-rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.8/nose/commands.py
+-rw-r--r--   0 michael    (501) staff       (20)    24529 2023-07-31 02:19:59.000000 pynose-1.4.8/nose/config.py
+-rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.8/nose/core.py
+-rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.8/nose/exc.py
+-rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.8/nose/failure.py
+-rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.8/nose/importer.py
+-rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.8/nose/inspector.py
+-rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.8/nose/loader.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.150267 pynose-1.4.8/nose/plugins/
+-rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.8/nose/plugins/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.8/nose/plugins/allmodules.py
+-rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.8/nose/plugins/attrib.py
+-rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.8/nose/plugins/base.py
+-rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.8/nose/plugins/builtin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3803 2023-08-06 18:02:05.000000 pynose-1.4.8/nose/plugins/capture.py
+-rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.8/nose/plugins/collect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.8/nose/plugins/cover.py
+-rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.8/nose/plugins/debug.py
+-rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.8/nose/plugins/deprecated.py
+-rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.8/nose/plugins/doctests.py
+-rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.8/nose/plugins/errorclass.py
+-rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.8/nose/plugins/failuredetail.py
+-rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.8/nose/plugins/isolate.py
+-rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.8/nose/plugins/logcapture.py
+-rw-r--r--   0 michael    (501) staff       (20)    15004 2023-07-08 03:28:10.000000 pynose-1.4.8/nose/plugins/manager.py
+-rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.8/nose/plugins/multiprocess.py
+-rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.8/nose/plugins/plugintest.py
+-rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.8/nose/plugins/skip.py
+-rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.8/nose/plugins/testid.py
+-rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.8/nose/plugins/xunit.py
+-rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.8/nose/proxy.py
+-rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.8/nose/pyversion.py
+-rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.8/nose/result.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.8/nose/selector.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.150525 pynose-1.4.8/nose/sphinx/
+-rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.8/nose/sphinx/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.8/nose/sphinx/pluginopts.py
+-rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.8/nose/suite.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.150900 pynose-1.4.8/nose/tools/
+-rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.8/nose/tools/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.8/nose/tools/nontrivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.8/nose/tools/trivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.8/nose/twistedtools.py
+-rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.8/nose/usage.txt
+-rw-r--r--   0 michael    (501) staff       (20)    18927 2023-07-31 02:19:59.000000 pynose-1.4.8/nose/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-06 18:03:36.151552 pynose-1.4.8/pynose.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-08-06 18:03:36.000000 pynose-1.4.8/pynose.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1273 2023-08-06 18:03:36.000000 pynose-1.4.8/pynose.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-08-06 18:03:36.000000 pynose-1.4.8/pynose.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-08-06 18:03:36.000000 pynose-1.4.8/pynose.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-08-06 18:03:36.000000 pynose-1.4.8/pynose.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       86 2023-08-06 18:03:36.152126 pynose-1.4.8/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     5413 2023-07-31 02:19:59.000000 pynose-1.4.8/setup.py
```

### Comparing `pynose-1.4.7/.github/workflows/python-package-legacy.yml` & `pynose-1.4.8/.github/workflows/python-package-legacy.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/.github/workflows/python-package.yml` & `pynose-1.4.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/.gitignore` & `pynose-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/LICENSE` & `pynose-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/PKG-INFO` & `pynose-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.7
+Version: 1.4.8
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynose Version: 1.4.7 Summary: pynose fixes nose to
+Metadata-Version: 2.1 Name: pynose Version: 1.4.8 Summary: pynose fixes nose to
 extend unittest and make testing easier Home-page: https://github.com/mdmintz/
 pynose Author: Michael Mintz Author-email: mdmintz@gmail.com License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files Project-URL:
 PyPI, https://pypi.org/project/pynose/ Project-URL: Source, https://github.com/
 mdmintz/pynose Project-URL: Documentation, https://nose.readthedocs.io/en/
 latest/ Keywords: test unittest doctest automatic discovery Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
```

### Comparing `pynose-1.4.7/README.md` & `pynose-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/__init__.py` & `pynose-1.4.8/nose/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/case.py` & `pynose-1.4.8/nose/case.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/commands.py` & `pynose-1.4.8/nose/commands.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/config.py` & `pynose-1.4.8/nose/config.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/core.py` & `pynose-1.4.8/nose/core.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/failure.py` & `pynose-1.4.8/nose/failure.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/importer.py` & `pynose-1.4.8/nose/importer.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/inspector.py` & `pynose-1.4.8/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/loader.py` & `pynose-1.4.8/nose/loader.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/__init__.py` & `pynose-1.4.8/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/allmodules.py` & `pynose-1.4.8/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/attrib.py` & `pynose-1.4.8/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/base.py` & `pynose-1.4.8/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/builtin.py` & `pynose-1.4.8/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/capture.py` & `pynose-1.4.8/nose/plugins/capture.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-"""This plugin captures stdout during test execution. If the test fails
+"""This plugin captures stdout during test execution. If a test fails
 or raises an error, the captured output will be appended to the error
-or failure output. It is enabled by default but can be disabled with
-the options ``-s`` or ``--nocapture``.
+or failure output. It is disabled by default, but can be enabled with
+the options: ``--capture-output`` or ``--capture_output``.
+Or enable it by setting os.environ["NOSE_CAPTURE"] to "1".
 
 :Options:
-  ``--nocapture``
-    Don't capture stdout (any stdout output will be printed immediately) """
+  ``--capture-output`` or ``--capture_output``
+    Capture stdout (stdout output will not be printed) """
 import logging
+import os
 import sys
 from nose.plugins.base import Plugin
 from nose.pyversion import exc_to_unicode, force_unicode
 from nose.util import ln
 from io import StringIO
 
 log = logging.getLogger(__name__)
 
 
 class Capture(Plugin):
-    """Output capture plugin. Enabled by default. Disable with ``-s`` or
-    ``--nocapture``. This plugin captures stdout during test execution,
-    appending any output captured to the error or failure output,
-    should the test fail or raise an error."""
+    """Output-capturing plugin. Now disabled by default.
+    Can be enabled with ``--capture-output`` or ``--capture_output``.
+    Or enable it with os.environ["NOSE_CAPTURE"]="1" before tests."""
     enabled = True
     name = "capture"
     score = 1600
 
     def __init__(self):
         self.stdout = []
         self._buf = None
@@ -33,19 +34,32 @@
         """Register commandline options"""
         parser.add_option(
             "-s", "--nocapture", action="store_false",
             default=False, dest="capture",
             help="Don't capture stdout (any stdout output "
             "will be printed immediately) [NOSE_NOCAPTURE]"
         )
+        parser.add_option(
+            "--capture-output", "--capture_output", action="store_true",
+            default=False, dest="capture_output",
+            help="Capture stdout (stdout output "
+            "will not be printed) [NOSE_CAPTURE]"
+        )
 
     def configure(self, options, conf):
         """Configure plugin. Plugin is enabled by default."""
         self.conf = conf
-        if not options.capture:
+        if (
+            "NOSE_CAPTURE" in os.environ.keys()
+            and os.environ["NOSE_CAPTURE"] == "1"
+        ):
+            self.enabled = True
+        elif options.capture_output:
+            self.enabled = True
+        elif not options.capture:
             self.enabled = False
 
     def afterTest(self, test):
         """Clear capture buffer."""
         self.end()
         self._buf = None
```

### Comparing `pynose-1.4.7/nose/plugins/collect.py` & `pynose-1.4.8/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/cover.py` & `pynose-1.4.8/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/debug.py` & `pynose-1.4.8/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/deprecated.py` & `pynose-1.4.8/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/doctests.py` & `pynose-1.4.8/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/errorclass.py` & `pynose-1.4.8/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/failuredetail.py` & `pynose-1.4.8/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/isolate.py` & `pynose-1.4.8/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/logcapture.py` & `pynose-1.4.8/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/manager.py` & `pynose-1.4.8/nose/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/multiprocess.py` & `pynose-1.4.8/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/plugintest.py` & `pynose-1.4.8/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/skip.py` & `pynose-1.4.8/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/testid.py` & `pynose-1.4.8/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/plugins/xunit.py` & `pynose-1.4.8/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/proxy.py` & `pynose-1.4.8/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/pyversion.py` & `pynose-1.4.8/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/result.py` & `pynose-1.4.8/nose/result.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/selector.py` & `pynose-1.4.8/nose/selector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/sphinx/pluginopts.py` & `pynose-1.4.8/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/suite.py` & `pynose-1.4.8/nose/suite.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/tools/nontrivial.py` & `pynose-1.4.8/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/tools/trivial.py` & `pynose-1.4.8/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/twistedtools.py` & `pynose-1.4.8/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/usage.txt` & `pynose-1.4.8/nose/usage.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/nose/util.py` & `pynose-1.4.8/nose/util.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/pynose.egg-info/PKG-INFO` & `pynose-1.4.8/pynose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.7
+Version: 1.4.8
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynose Version: 1.4.7 Summary: pynose fixes nose to
+Metadata-Version: 2.1 Name: pynose Version: 1.4.8 Summary: pynose fixes nose to
 extend unittest and make testing easier Home-page: https://github.com/mdmintz/
 pynose Author: Michael Mintz Author-email: mdmintz@gmail.com License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files Project-URL:
 PyPI, https://pypi.org/project/pynose/ Project-URL: Source, https://github.com/
 mdmintz/pynose Project-URL: Documentation, https://nose.readthedocs.io/en/
 latest/ Keywords: test unittest doctest automatic discovery Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
```

### Comparing `pynose-1.4.7/pynose.egg-info/SOURCES.txt` & `pynose-1.4.8/pynose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.7/setup.py` & `pynose-1.4.8/setup.py`

 * *Files identical despite different names*

