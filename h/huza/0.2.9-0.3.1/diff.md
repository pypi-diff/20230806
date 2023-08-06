# Comparing `tmp/huza-0.2.9.tar.gz` & `tmp/huza-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huza-0.2.9.tar", last modified: Wed May 10 02:15:56 2023, max compression
+gzip compressed data, was "huza-0.3.1.tar", last modified: Sun Aug  6 03:57:57 2023, max compression
```

## Comparing `huza-0.2.9.tar` & `huza-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.429268 huza-0.2.9/
--rw-r--r--   0 root         (0) root         (0)     1062 2022-11-21 06:24:02.000000 huza-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-10 02:15:56.429268 huza-0.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2022-11-21 06:24:02.000000 huza-0.2.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.420268 huza-0.2.9/huza/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.422268 huza-0.2.9/huza/base/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      751 2022-01-04 03:29:52.000000 huza-0.2.9/huza/base/action.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-05 12:11:37.000000 huza-0.2.9/huza/base/dockview.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-11-21 06:24:02.000000 huza-0.2.9/huza/base/mainwindow.py
--rw-r--r--   0 root         (0) root         (0)     6674 2023-04-04 07:57:27.000000 huza-0.2.9/huza/base/mainwindow_run.py
--rw-r--r--   0 root         (0) root         (0)      653 2022-05-17 09:25:15.000000 huza-0.2.9/huza/base/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.422268 huza-0.2.9/huza/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      701 2022-01-04 03:29:52.000000 huza-0.2.9/huza/cli/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.423268 huza-0.2.9/huza/icons/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33436 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/iconbase.py
--rw-r--r--   0 root         (0) root         (0)     1281 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/iconcore.py
--rw-r--r--   0 root         (0) root         (0)  1532400 2022-01-04 03:29:52.000000 huza-0.2.9/huza/icons/img.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.425268 huza-0.2.9/huza/mainwindow/
--rw-r--r--   0 root         (0) root         (0)       33 2022-01-04 03:29:52.000000 huza-0.2.9/huza/mainwindow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-04 07:57:27.000000 huza-0.2.9/huza/mainwindow/main.py
--rw-r--r--   0 root         (0) root         (0)      538 2022-01-04 03:29:52.000000 huza-0.2.9/huza/mainwindow/main_actions.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-04-04 07:57:27.000000 huza-0.2.9/huza/mainwindow/main_docks.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-06 07:13:51.000000 huza-0.2.9/huza/mainwindow/main_ribbon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.426268 huza-0.2.9/huza/ribbon/
--rw-r--r--   0 root         (0) root         (0)     1599 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonButton.py
--rw-r--r--   0 root         (0) root         (0)     2370 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonPane.py
--rw-r--r--   0 root         (0) root         (0)      719 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonTab.py
--rw-r--r--   0 root         (0) root         (0)      937 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/RibbonWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/ribbon/qss/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6330 2022-07-25 02:53:50.000000 huza-0.2.9/huza/ribbon/qss/default_qss.py
--rw-r--r--   0 root         (0) root         (0)       55 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/mainqss.py
--rw-r--r--   0 root         (0) root         (0)       97 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonpaneqss.py
--rw-r--r--   0 root         (0) root         (0)      900 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonqss.py
--rw-r--r--   0 root         (0) root         (0)      706 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbonsmallbuttonqss.py
--rw-r--r--   0 root         (0) root         (0)      745 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/qss/ribbosbutton.py
--rw-r--r--   0 root         (0) root         (0)      158 2022-01-04 03:29:52.000000 huza-0.2.9/huza/ribbon/scale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1026 2022-06-16 03:42:50.000000 huza-0.2.9/huza/scripts/img2base64.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.428268 huza-0.2.9/huza/splash/
--rw-r--r--   0 root         (0) root         (0)      189 2022-01-04 03:29:52.000000 huza-0.2.9/huza/splash/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2269 2022-01-04 03:29:52.000000 huza-0.2.9/huza/splash/splash.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.429268 huza-0.2.9/huza/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.2.9/huza/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-04-03 08:25:57.000000 huza-0.2.9/huza/util/buildui.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-01-04 03:29:52.000000 huza-0.2.9/huza/util/constant.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-05-10 02:12:48.000000 huza-0.2.9/huza/util/mainui.py
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-10 02:12:48.000000 huza-0.2.9/huza/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 02:15:56.421268 huza-0.2.9/huza.egg-info/
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1229 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-10 02:15:56.000000 huza-0.2.9/huza.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-04 03:36:49.000000 huza-0.2.9/huza.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     5644 2022-01-04 03:29:52.000000 huza-0.2.9/nsis.nsi
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 02:15:56.429268 huza-0.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2166 2023-05-10 02:12:48.000000 huza-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.345006 huza-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1062 2022-11-21 06:24:02.000000 huza-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-08-06 03:57:57.345006 huza-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2022-11-21 06:24:02.000000 huza-0.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.333006 huza-0.3.1/huza/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.335006 huza-0.3.1/huza/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      751 2022-01-04 03:29:52.000000 huza-0.3.1/huza/base/action.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-20 03:51:47.000000 huza-0.3.1/huza/base/dockview.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2022-11-21 06:24:02.000000 huza-0.3.1/huza/base/mainwindow.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-06-08 06:13:00.000000 huza-0.3.1/huza/base/mainwindow_run.py
+-rw-r--r--   0 root         (0) root         (0)      653 2022-05-17 09:25:15.000000 huza-0.3.1/huza/base/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.336006 huza-0.3.1/huza/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-06 01:42:17.000000 huza-0.3.1/huza/cli/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.336006 huza-0.3.1/huza/icons/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/icons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59876 2023-06-07 07:58:05.000000 huza-0.3.1/huza/icons/iconbase.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-06-20 03:51:47.000000 huza-0.3.1/huza/icons/iconcore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.340006 huza-0.3.1/huza/icons/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:58:05.000000 huza-0.3.1/huza/icons/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2297885 2023-06-07 07:58:05.000000 huza-0.3.1/huza/icons/images/img.py
+-rw-r--r--   0 root         (0) root         (0)   350245 2023-06-07 07:58:05.000000 huza-0.3.1/huza/icons/images/img1.py
+-rw-r--r--   0 root         (0) root         (0)   478061 2023-06-07 07:58:05.000000 huza-0.3.1/huza/icons/images/img3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.341006 huza-0.3.1/huza/mainwindow/
+-rw-r--r--   0 root         (0) root         (0)       33 2022-01-04 03:29:52.000000 huza-0.3.1/huza/mainwindow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-27 00:54:51.000000 huza-0.3.1/huza/mainwindow/main.py
+-rw-r--r--   0 root         (0) root         (0)      538 2022-01-04 03:29:52.000000 huza-0.3.1/huza/mainwindow/main_actions.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-08-06 03:57:09.000000 huza-0.3.1/huza/mainwindow/main_docks.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-06 07:13:51.000000 huza-0.3.1/huza/mainwindow/main_ribbon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.341006 huza-0.3.1/huza/puis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:58:05.000000 huza-0.3.1/huza/puis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3786 2023-06-07 07:58:05.000000 huza-0.3.1/huza/puis/showicon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.342006 huza-0.3.1/huza/ribbon/
+-rw-r--r--   0 root         (0) root         (0)     1599 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/RibbonButton.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/RibbonPane.py
+-rw-r--r--   0 root         (0) root         (0)      719 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/RibbonTab.py
+-rw-r--r--   0 root         (0) root         (0)      937 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/RibbonWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.343006 huza-0.3.1/huza/ribbon/qss/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6330 2022-07-25 02:53:50.000000 huza-0.3.1/huza/ribbon/qss/default_qss.py
+-rw-r--r--   0 root         (0) root         (0)       55 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/mainqss.py
+-rw-r--r--   0 root         (0) root         (0)       97 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/ribbonpaneqss.py
+-rw-r--r--   0 root         (0) root         (0)      900 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/ribbonqss.py
+-rw-r--r--   0 root         (0) root         (0)      706 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/ribbonsmallbuttonqss.py
+-rw-r--r--   0 root         (0) root         (0)      745 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/qss/ribbosbutton.py
+-rw-r--r--   0 root         (0) root         (0)      158 2022-01-04 03:29:52.000000 huza-0.3.1/huza/ribbon/scale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.344006 huza-0.3.1/huza/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2022-06-16 03:42:50.000000 huza-0.3.1/huza/scripts/img2base64.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.344006 huza-0.3.1/huza/splash/
+-rw-r--r--   0 root         (0) root         (0)      189 2022-01-04 03:29:52.000000 huza-0.3.1/huza/splash/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-06-07 07:58:05.000000 huza-0.3.1/huza/splash/splash.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.345006 huza-0.3.1/huza/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-04 03:29:52.000000 huza-0.3.1/huza/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-06-06 01:42:17.000000 huza-0.3.1/huza/util/buildui.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-06 03:57:09.000000 huza-0.3.1/huza/util/constant.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-01 11:57:28.000000 huza-0.3.1/huza/util/mainui.py
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-06 03:57:09.000000 huza-0.3.1/huza/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 03:57:57.334006 huza-0.3.1/huza.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-06 03:57:57.000000 huza-0.3.1/huza.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-04 03:36:49.000000 huza-0.3.1/huza.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     5644 2022-01-04 03:29:52.000000 huza-0.3.1/nsis.nsi
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 03:57:57.345006 huza-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-06-07 07:58:05.000000 huza-0.3.1/setup.py
```

### Comparing `huza-0.2.9/LICENSE` & `huza-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/PKG-INFO` & `huza-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: huza
-Version: 0.2.9
+Version: 0.3.1
 Summary: Self-use pyqt framework
 Home-page: https://github.com/huyidao625/Huza
 Author: hufei
 Author-email: hufei625@qq.com
 License: MIT License
 Project-URL: Wiki, https://www.hudh.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: System :: Networking
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 Huza
 ======
 
 自用的PyQT框架
```

### Comparing `huza-0.2.9/huza/base/action.py` & `huza-0.3.1/huza/base/action.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/base/dockview.py` & `huza-0.3.1/huza/base/dockview.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class DockView(object):
     def __init__(self, mainui: MainWindow_Form):
         self.mainui = mainui
         self.extra = get_extra(mainui)
         self.iconlist = self.get_icon_list()  # IconListHandler
 
-    def set_dock_view(self, name, displayname, dockname, formclass):
-        return self.mainui.set_dock_view(name, displayname, dockname, formclass)
+    def set_dock_view(self, name, displayname, dockname, formclass, showthisview=True):
+        return self.mainui.set_dock_view(name, displayname, dockname, formclass, showthisview)
 
     def get_icon_list(self) -> IconListHandler:
         return self.mainui.icon_list
 
     def emit(self, signal, data):
         self.form.signal.emit(signal, data)
 
@@ -26,15 +26,27 @@
 
     def get_action(self, action_name):
         return get_action(self.mainui, action_name)
 
     def get_dock(self, dock_name):
         return get_dock(self.mainui, dock_name)
 
+    def get_all_dock(self):
+        return get_all_dock(self.mainui)
+
+    def get_all_action(self):
+        return get_all_action(self.mainui)
+
+    def get_all_dockview(self):
+        return get_all_dockview(self.mainui)
+
     def get_dock_current_ui(self, dock_name):
         return get_dock_current_ui(self.mainui, dock_name)
 
     def get_dock_ui(self, dock_name, ui_name):
         return get_dock_ui(self.mainui, dock_name, ui_name)
 
+    def del_dock_ui(self, dock_name, ui_name):
+        return del_dock_ui(self.mainui, dock_name, ui_name)
+
     def get_ui(self, ui_name):
         return get_ui(self.mainui, ui_name)
```

### Comparing `huza-0.2.9/huza/base/mainwindow.py` & `huza-0.3.1/huza/base/mainwindow.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/base/mainwindow_run.py` & `huza-0.3.1/huza/base/mainwindow_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,30 +43,35 @@
 
     def init_menu(self, rabbons: dict):
         self.window.init_ribbon(rabbons)
 
     def init_docks(self, docks: dict, layout: list):
         self.window.init_docks(docks, layout)
 
+    def get_all_dock(self):
+        return self.window.get_all_dock()
+
+    def get_all_action(self):
+        return self.window.get_all_action()
+
+    def get_all_dockview(self):
+        return self.window.get_all_dockview()
+
     def emit(self, signal, data):
         self.window.emit(signal, data)
 
     def get_ribbon_tab(self):
         return self.window.get_ribbon_tab()
 
     def bind_signal(self, signal, func):
         if func.__name__ in dir(self.window):
             raise Exception(f'绑定的函数[{func.__name__}]与内置函数冲突，请更换函数名称')
         setattr(self.window, func.__name__, types.MethodType(func, self.window))
         self.window.bind_signal(signal, getattr(self.window, func.__name__))
 
-    def __getattr__(self, attr):
-        if hasattr(self.window, attr):
-            return getattr(self.window, attr)
-        return super(MainWindowRun, self).__getattr__(attr)
 
     def bind_func(self, func):
         if func.__name__ in dir(self.window):
             raise Exception(f'绑定的函数[{func.__name__}]与内置函数冲突，请更换函数名称')
         setattr(self.window, func.__name__, types.MethodType(func, self.window))
 
     def get_action(self, name: str) -> QAction:
@@ -87,16 +92,16 @@
 
     def get_ui(self, ui_name):
         return get_ui(self.window, ui_name)
 
     def get_dock_current_ui(self, dock_name):
         return get_dock_current_ui(self.window, dock_name)
 
-    def set_dock_view(self, name, displayname, dockname, formclass):
-        return self.window.set_dock_view(name, displayname, dockname, formclass)
+    def set_dock_view(self, name, displayname, dockname, formclass, showthisview=True):
+        return self.window.set_dock_view(name, displayname, dockname, formclass, showthisview)
 
     def _init_log(self):
         try:
             if os.path.exists(LOGFILE):
                 os.remove(LOGFILE)
             logger.configure(**LOGGINGCONFIG)
         except Exception as e:
```

### Comparing `huza-0.2.9/huza/base/widget.py` & `huza-0.3.1/huza/base/widget.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/cli/shell.py` & `huza-0.3.1/huza/cli/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     """
     base = os.path.abspath(os.path.dirname(__file__))
     import argparse
     parser = argparse.ArgumentParser()
     parser.description = 'Huza 命令行工具'
     parser.add_argument("-genimg", help="生成图片集文件", action='store_true')
     parser.add_argument('-i', "--input", help="输入目录", default='.')
-    parser.add_argument('-o', "--output", help="计算包描述", default='.')
+    parser.add_argument('-o', "--output", help="输出目录", default='.')
 
     args = parser.parse_args()
     if args.genimg:
         image2base64(args.input, args.output)
     else:
         parser.print_help()
```

### Comparing `huza-0.2.9/huza/icons/iconcore.py` & `huza-0.3.1/huza/icons/iconcore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import re
 from PyQt5 import QtGui, QtCore
 from loguru import logger
 
-from huza.icons.iconbase import DefaultIconHandler, IconHandler
-from huza.icons.img import image_dict
+from huza.icons.iconbase import DefaultIconHandler, IconHandler, Default1IconHandler, Default3IconHandler
 
 
 class IconListHandlerBase(object):
     def __init__(self):
-        self.default = DefaultIconHandler()
-        self._iconlist = {}
+        self._iconlist = {'default': DefaultIconHandler(),
+                          'd1': Default1IconHandler(),
+                          'd3': Default3IconHandler(),
+                          }
 
     def __getattr__(self, attr):
         if self._iconlist.get(attr) is not None:
             iconhandler = self._iconlist.get(attr)
             return iconhandler
         return None
 
+
 class IconListHandler(IconListHandlerBase):
     def add_icon_list(self, name, img_database):
-        if name == 'default':
+        if name in ['default', 'd1', 'd3']:
             raise Exception(f'不能覆盖默认的图表集 {name}')
         if name in self._iconlist:
             raise Exception(f'图表集已经存在 {name}')
         if not re.match(r'^[_]?[a-zA-Z]+[0-9]*$', name):
             raise Exception(f'图表集命名不规范 {name}')
         iconhandler = IconHandler()
         iconhandler._set_img_database(img_database)
         self._iconlist[name] = iconhandler
 
 
 if __name__ == '__main__':
+    from huza.icons.images.img import image_dict
     import sys
     from PyQt5.QtWidgets import QApplication
 
     app = QApplication(sys.argv)
     c = IconListHandler()
     c.add_icon_list('dd', image_dict)
     dd = c.default.Calculatehortestpath_grid_671
```

### Comparing `huza-0.2.9/huza/mainwindow/main.py` & `huza-0.3.1/huza/mainwindow/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,23 @@
     set_dock_view = setDockView
     get_extra = get_extra
     get_action = get_action
     get_dock = get_dock
     get_dock_current_ui = get_dock_current_ui
     get_dock_ui = get_dock_ui
     del_dock_ui = del_dock_ui
+    get_all_dock = get_all_dock
+    get_all_action = get_all_action
+    get_all_dockview = get_all_dockview
     get_ui = get_ui
 
     def __init__(self, extra, icon_list):
         self.extra = extra
         self.icon_list = icon_list
+        self.iconlist = self.icon_list
         super(MainWindow_Form, self).__init__()
 
     def setupUi(self, Form):
         self.form = Form
         self.docks = {}
         self.actions = {}
         self.signals = {}
@@ -43,14 +47,16 @@
     def load(self):
         self.addRibbon()
         self._init_dock_env()
 
     def signalHeadle(self, key, args):
         if key in self.signals:
             self.signals[key](args)
+        else:
+            logger.warning(f'signal [{key}] emited, but there is no binding')
 
     def addRibbon(self):
         self.form._ribbon = RibbonWidget(self.form)
         self.form.addToolBar(self.form._ribbon)
         self._ribbon = self.form._ribbon
 
     def get_ribbon_tab(self) -> QTabWidget:
```

### Comparing `huza-0.2.9/huza/mainwindow/main_actions.py` & `huza-0.3.1/huza/mainwindow/main_actions.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/mainwindow/main_docks.py` & `huza-0.3.1/huza/mainwindow/main_docks.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 
 def init_docks(self, docks: dict, layout: list):
     """docks = {
         'main': QDockWidget(""),
         'para': QDockWidget(""),
         'setup': QDockWidget(""),
         'info': QDockWidget(""),
+        'monitor': QDockWidget(""),
     }
     layout = [('add', 'left', 'para'),
          ('split', 'para', 'setup', 'h'),
          ('split', 'setup', 'main', 'h'),
          ('split', 'main', 'info', 'v'),
+         ('tabify','para','monitor')
          ]
 
     :param self:
     :type self:
     :param docks_dict:
     :type docks_dict:
     :return:
@@ -32,44 +34,50 @@
         hand = l[0]
         if hand == DOCK_LAYOUT_ADD:
             _, oriz, dockname = l
             self.form.addDockWidget(DockWidgetAreadict[oriz], self.docks[dockname])
         elif hand == DOCK_LAYOUT_SPLIT:
             _, d1, d2, ori = l
             self.form.splitDockWidget(self.docks[d1], self.docks[d2], Orientiondict[ori])
+        elif hand == DOCK_LAYOUT_TABILY:
+            _, d1, d2 = l
+            self.form.tabifyDockWidget(self.docks[d1], self.docks[d2])
 
 
-def setDockView(self, name, displayname, dockname, formclass):
+def setDockView(self, name, displayname, dockname, formclass, showthisview=True, widgetclass=MainQWidget):
     def _check_name_exist(name):
         """保证dockviews下的id唯一"""
         for k, v in self.dockviews.items():
             for uname, ui in v.items():
                 if uname == name:
                     return k
         return None
 
     dock = self.docks.get(dockname)
     if dock.windowTitle() == name:
         return
-    dock.setWindowTitle(displayname)
-    dock.setVisible(True)
+    if showthisview:
+        dock.setWindowTitle(displayname)
+        dock.setVisible(True)
     dockviews = self.dockviews[dockname]
     if name in dockviews:
         w = dockviews.get(name)
-        dock.setWidget(w)
+        if showthisview:
+            dock.setWidget(w)
         if hasattr(w, 'refresh'):
             w.refresh()
         return w.ui()
     else:
         nameexist = _check_name_exist(name)
         if nameexist is not None:
             raise Exception(f'dockviews已经存在相同的id，位于[{nameexist}]')
 
-        w = MainQWidget(self.form)
+        w = widgetclass(self.form)
         w.signal.connect(self.signalHeadle)
         ui = formclass(self)
         ui._name_sig = name  # 用于标记名称
         ui.setupUi(w)
         w._ui = ui
-        dock.setWidget(w)
+        if showthisview:
+            dock.setWidget(w)
         dockviews[name] = w
         return ui
```

### Comparing `huza-0.2.9/huza/mainwindow/main_ribbon.py` & `huza-0.3.1/huza/mainwindow/main_ribbon.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/RibbonButton.py` & `huza-0.3.1/huza/ribbon/RibbonButton.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/RibbonPane.py` & `huza-0.3.1/huza/ribbon/RibbonPane.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/RibbonTab.py` & `huza-0.3.1/huza/ribbon/RibbonTab.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/RibbonWidget.py` & `huza-0.3.1/huza/ribbon/RibbonWidget.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/qss/default_qss.py` & `huza-0.3.1/huza/ribbon/qss/default_qss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/qss/ribbonqss.py` & `huza-0.3.1/huza/ribbon/qss/ribbonqss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/qss/ribbonsmallbuttonqss.py` & `huza-0.3.1/huza/ribbon/qss/ribbonsmallbuttonqss.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/ribbon/qss/ribbosbutton.py` & `huza-0.3.1/huza/ribbon/qss/ribbosbutton.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/scripts/img2base64.py` & `huza-0.3.1/huza/scripts/img2base64.py`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/huza/splash/splash.py` & `huza-0.3.1/huza/splash/splash.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.setProgressText(5)
         time.sleep(0.1)
         self.setProgressText(10)
         time.sleep(0.1)
         self.setProgressText(15)
         time.sleep(0.10)
         self.setProgressText(20)  # PyQt5, i18n are loaded, so before 20% do nothing
-        time.sleep(0.01)
+        time.sleep(0.10)
         self.setProgressText(40)
-        time.sleep(0.01)
+        time.sleep(0.10)
         self.setProgressText(60)
-        time.sleep(0.01)
+        time.sleep(0.10)
         self.setProgressText(80)
-        time.sleep(0.01)
+        time.sleep(0.10)
         self.setProgressText(100)
```

### Comparing `huza-0.2.9/huza/util/buildui.py` & `huza-0.3.1/huza/util/buildui.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,34 +35,56 @@
 
     with codecs.open(_outfile, 'r', 'utf-8') as f:
         _old = f.read()
 
     return newmd5
 
 
+def is_include_all_file(uics, outpath):
+    all_autoui_file = []
+    for i in os.listdir(outpath):
+        f = os.path.join(outpath, i)
+        if os.path.isfile(f):
+            all_autoui_file.append(i)
+
+    for i in uics:
+        py_f = f'{i}.py'
+        if py_f not in all_autoui_file:
+            return False
+
+    return True
+
+
 def build_uidir(uipath, outpath):
     if not os.path.exists(outpath):
         os.makedirs(outpath)
         with open(os.path.join(outpath, '__init__.py'), 'w') as f:
             f.write('import os')
     _uics = []
-    for i in os.listdir(uipath):
+    list_ui_path = os.listdir(uipath)
+    for i in list_ui_path:
         _n, _p = os.path.splitext(i)
         if _p == '.ui':
             _uics.append(_n)
     if not os.path.exists('cache.md5'):
         md5s = {}
         for i in _uics:
             _infile = '{n}.ui'.format(n=i)
             md5s[i] = 1
-        md5s['yukina'] = 1
         md5s = md5s
     else:
         with codecs.open('cache.md5', 'r', 'utf-8') as f:
             md5s = json.loads(f.read())
+        if not is_include_all_file(_uics, outpath):
+            md5s = {}
+            for i in _uics:
+                _infile = '{n}.ui'.format(n=i)
+                md5s[i] = 1
+            md5s = md5s
+
     for i in _uics:
         if i not in md5s:
             md5s[i] = '0'
         changed = buildui(uipath, i, outpath, md5s[i])
         if changed:
             md5s[i] = changed
     with codecs.open('cache.md5', 'w', 'utf-8') as f:
```

### Comparing `huza-0.2.9/huza/util/constant.py` & `huza-0.3.1/huza/util/constant.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     ],
 }
 
 FLOAT_RE = re.compile('^[+-]?\d+$|^[-+]?\d*\.\d+$|^[+-]?\d+\.\d+[Ee]{1}[+-]?\d+$')
 
 DOCK_LAYOUT_ADD = 'add'  # 对应addDockWidget函数
 DOCK_LAYOUT_SPLIT = 'split'  # 对应splitDockWidget函数
+DOCK_LAYOUT_TABILY = 'tabify'  # 对应tabifyDockWidget函数
 DockWidgetAreadict = {'left': Qt.LeftDockWidgetArea, 'right': Qt.RightDockWidgetArea, 'top': Qt.TopDockWidgetArea,
                       'bottom': Qt.BottomDockWidgetArea}
 Orientiondict = {'h': Qt.Horizontal, 'v': Qt.Vertical}
```

### Comparing `huza-0.2.9/huza/util/mainui.py` & `huza-0.3.1/huza/util/mainui.py`

 * *Files 27% similar despite different names*

```diff
@@ -38,14 +38,26 @@
     for k, v in mainui.dockviews.items():
         for ui_name, ui_f in v.items():
             if uiname == ui_name:
                 return ui_f.ui()
     return None
 
 
+def get_all_dock(mainui):
+    return mainui.docks
+
+
+def get_all_action(mainui):
+    return mainui.actions
+
+
+def get_all_dockview(mainui):
+    return mainui.dockviews
+
+
 def del_dock_ui(mainui, dock_name: str, uiname: str):
     if dock_name in mainui.dockviews:
         dockviews = mainui.dockviews.get(dock_name)
         if uiname in dockviews:
             w = dockviews[uiname]
             dock = mainui.docks.get(dock_name).widget()
             if dock == w:
```

### Comparing `huza-0.2.9/huza.egg-info/PKG-INFO` & `huza-0.3.1/huza.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: huza
-Version: 0.2.9
+Version: 0.3.1
 Summary: Self-use pyqt framework
 Home-page: https://github.com/huyidao625/Huza
 Author: hufei
 Author-email: hufei625@qq.com
 License: MIT License
 Project-URL: Wiki, https://www.hudh.cn
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: System :: Networking
+Classifier: Environment :: X11 Applications :: Qt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 Huza
 ======
 
 自用的PyQT框架
```

### Comparing `huza-0.2.9/nsis.nsi` & `huza-0.3.1/nsis.nsi`

 * *Files identical despite different names*

### Comparing `huza-0.2.9/setup.py` & `huza-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,21 +61,22 @@
             'huza=huza.cli.shell:main',
         ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Topic :: System :: Networking',
+        'Environment :: X11 Applications :: Qt',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11'
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Software Development :: Libraries'
     ],
     project_urls={
         'Wiki': 'https://www.hudh.cn'
     }
 
 )
```

