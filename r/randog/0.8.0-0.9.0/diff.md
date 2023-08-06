# Comparing `tmp/randog-0.8.0.tar.gz` & `tmp/randog-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randog-0.8.0.tar", last modified: Sun Jul 23 11:18:20 2023, max compression
+gzip compressed data, was "randog-0.9.0.tar", last modified: Sun Jul 30 12:25:30 2023, max compression
```

## Comparing `randog-0.8.0.tar` & `randog-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-23 11:18:10.000000 randog-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-23 11:18:20.340670 randog-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-23 11:18:10.000000 randog-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.336670 randog-0.8.0/randog/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-23 11:18:10.000000 randog-0.8.0/randog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-23 11:18:10.000000 randog-0.8.0/randog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.336670 randog-0.8.0/randog/_main/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_main_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/randog/_main/_subcmd_def/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_byfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_main/_subcmd_def/_timedelta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/randog/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_utils/nullsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-23 11:18:10.000000 randog-0.8.0/randog/_utils/type.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-23 11:18:10.000000 randog-0.8.0/randog/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/randog/factory/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_by_callable.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_by_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_float.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_from_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_from_pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_increment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/randog/factory/_str/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_str/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_str/_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-23 11:18:10.000000 randog-0.8.0/randog/factory/_union.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.340670 randog-0.8.0/randog/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-23 11:18:10.000000 randog-0.8.0/randog/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-23 11:18:10.000000 randog-0.8.0/randog/sqlalchemy/_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-23 11:18:10.000000 randog-0.8.0/randog/sqlalchemy/_custom_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-23 11:18:10.000000 randog-0.8.0/randog/timedelta_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 11:18:20.336670 randog-0.8.0/randog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-23 11:18:20.000000 randog-0.8.0/randog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-23 11:18:20.000000 randog-0.8.0/randog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 11:18:20.000000 randog-0.8.0/randog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-23 11:18:20.000000 randog-0.8.0/randog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 11:18:20.340670 randog-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-23 11:18:10.000000 randog-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-30 12:25:20.000000 randog-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-30 12:25:30.478049 randog-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-30 12:25:20.000000 randog-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.474049 randog-0.9.0/randog/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-30 12:25:20.000000 randog-0.9.0/randog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-30 12:25:20.000000 randog-0.9.0/randog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.474049 randog-0.9.0/randog/_main/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_main_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/randog/_main/_subcmd_def/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_byfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_main/_subcmd_def/_timedelta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/randog/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_utils/nullsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-30 12:25:20.000000 randog-0.9.0/randog/_utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-30 12:25:20.000000 randog-0.9.0/randog/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/randog/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_by_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_by_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_from_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_from_pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_increment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/randog/factory/_str/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_str/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_str/_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-30 12:25:20.000000 randog-0.9.0/randog/factory/_union.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.478049 randog-0.9.0/randog/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-30 12:25:20.000000 randog-0.9.0/randog/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-07-30 12:25:20.000000 randog-0.9.0/randog/sqlalchemy/_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-30 12:25:20.000000 randog-0.9.0/randog/sqlalchemy/_custom_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-30 12:25:20.000000 randog-0.9.0/randog/timedelta_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 12:25:30.474049 randog-0.9.0/randog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-30 12:25:30.000000 randog-0.9.0/randog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-30 12:25:30.000000 randog-0.9.0/randog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 12:25:30.000000 randog-0.9.0/randog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 12:25:30.000000 randog-0.9.0/randog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 12:25:30.478049 randog-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-30 12:25:20.000000 randog-0.9.0/setup.py
```

### Comparing `randog-0.8.0/LICENSE` & `randog-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/PKG-INFO` & `randog-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.8.0 — Randomly object generator**
+Description: **randog 0.9.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.8.0/README.md` & `randog-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-**randog 0.8.0 — Randomly object generator**
+**randog 0.9.0 — Randomly object generator**
 
 **randog** is a package which helps to generate data randomly.
 
 ## Install
 
 You can install from PyPI.
```

### Comparing `randog-0.8.0/randog/__main__.py` & `randog-0.9.0/randog/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
 import json
 import random
 import sys
 import typing as t
 
 import randog.factory
-from .factory import FactoryDef
+from .factory import FactoryDef, FactoryStopException
 from ._main import Args, Subcmd, get_subcmd_def
 
 
 def _build_factories(args: Args) -> t.Iterator[randog.factory.Factory]:
     subcmd_def = get_subcmd_def(args.sub_cmd)
 
     if args.sub_cmd == Subcmd.Byfile:
@@ -139,71 +139,87 @@
 
 def _output_to_csv(
     factory: randog.factory.Factory[t.Optional[t.Sequence[t.Sequence[t.Any]]]],
     line_num: int,
     fp: t.TextIO,
     regenerate: float,
     discard: float,
+    raise_on_factory_stopped: bool,
 ):
     csv_writer = csv.writer(fp, lineterminator="\n")
     csv_writer.writerows(
         filter(
             lambda x: x is not None,
             factory.iter(
                 line_num,
                 regenerate=regenerate,
                 discard=discard,
+                raise_on_factory_stopped=raise_on_factory_stopped,
             ),
         )
     )
 
 
 def main():
     args = Args(sys.argv)
 
-    with _open_output_fp_only(args) as fp_only:
-        index = 0
-        for factory in _build_factories(args):
-            for r_index in range(args.repeat):
-                with _open_output_fp_numbered(args, index) as fp_numbered:
-                    index += 1
-                    # args と index に応じて出力先 fp を決定する。
-                    # args と index に応じて fp_numbered, fp_only の状態が異なるので、それを条件に使用する。
-                    if not isinstance(fp_numbered, _DummyIO):
-                        fp = fp_numbered
-                    elif not isinstance(fp_only, _DummyIO):
-                        fp = fp_only
-                    else:
-                        fp = sys.stdout
-
-                    # 生成処理と出力処理
-                    # CSV 出力の場合に生成の方法が異なるので、生成と出力をひとまとめにした。
-                    if args.csv is not None:
-                        _output_to_csv(
-                            factory,
-                            args.csv,
-                            fp,
-                            regenerate=args.regenerate,
-                            discard=args.discard,
-                        )
-                    else:
-                        if args.list is not None:
-                            generated = list(
-                                factory.iter(
-                                    args.list,
-                                    regenerate=args.regenerate,
-                                    discard=args.discard,
-                                )
+    try:
+        with _open_output_fp_only(args) as fp_only:
+            index = 0
+            for factory in _build_factories(args):
+                for r_index in range(args.repeat):
+                    with _open_output_fp_numbered(args, index) as fp_numbered:
+                        index += 1
+                        # args と index に応じて出力先 fp を決定する。
+                        # args と index に応じて fp_numbered, fp_only の状態が異なるので、それを条件に使用する。
+                        if not isinstance(fp_numbered, _DummyIO):
+                            fp = fp_numbered
+                        elif not isinstance(fp_only, _DummyIO):
+                            fp = fp_only
+                        else:
+                            fp = sys.stdout
+
+                        # 生成処理と出力処理
+                        # CSV 出力の場合に生成の方法が異なるので、生成と出力をひとまとめにした。
+                        if args.csv is not None:
+                            _output_to_csv(
+                                factory,
+                                args.csv,
+                                fp,
+                                regenerate=args.regenerate,
+                                discard=args.discard,
+                                raise_on_factory_stopped=args.error_on_factory_stopped,
                             )
                         else:
-                            while True:
-                                generated = factory.next()
-                                if random.random() >= args.regenerate:
+                            if args.list is not None:
+                                generated = list(
+                                    factory.iter(
+                                        args.list,
+                                        regenerate=args.regenerate,
+                                        discard=args.discard,
+                                        raise_on_factory_stopped=args.error_on_factory_stopped,
+                                    )
+                                )
+                            else:
+                                try:
+                                    while True:
+                                        generated = factory.next(
+                                            raise_on_factory_stopped=args.error_on_factory_stopped
+                                        )
+                                        if random.random() >= args.regenerate:
+                                            break
+                                except StopIteration:
                                     break
-                            if random.random() < args.discard:
-                                continue
+                                if random.random() < args.discard:
+                                    continue
 
-                        _output_generated(generated, fp, args=args)
+                            _output_generated(generated, fp, args=args)
+    except FactoryStopException:
+        print(
+            "error: the factory stopped generating before the process was complete",
+            file=sys.stderr,
+        )
+        exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `randog-0.8.0/randog/_examples.py` & `randog-0.9.0/randog/_examples.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_main_args.py` & `randog-0.9.0/randog/_main/_main_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,14 +100,18 @@
     @property
     def csv(self) -> t.Optional[int]:
         if hasattr(self._args, "csv"):
             return self._args.csv
         else:
             return None
 
+    @property
+    def error_on_factory_stopped(self) -> bool:
+        return self.get("error_on_factory_stopped", False)
+
     def output_path_for(self, number: int) -> t.Optional[str]:
         if self._args.output is None:
             return None
         else:
             return self._args.output.format(number)
 
     def get(self, key: str, default: t.Any = None) -> t.Any:
```

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/__init__.py` & `randog-0.9.0/randog/_main/_subcmd_def/__init__.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_base.py` & `randog-0.9.0/randog/_main/_subcmd_def/_base.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_bool.py` & `randog-0.9.0/randog/_main/_subcmd_def/_bool.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_byfile.py` & `randog-0.9.0/randog/_main/_subcmd_def/_byfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return Subcmd.Byfile
 
     def add_parser(self, subparsers) -> argparse.ArgumentParser:
         byfile_parser = subparsers.add_parser(
             Subcmd.Byfile.value,
             usage=(
                 "python -m randog byfile FACTORY_PATH [FACTORY_PATH ...] [--regenerate PROB_REGEN] "
-                "[--discard PROB_DISCARD] [--csv ROW_NUM] [common-options]"
+                "[--discard PROB_DISCARD] [--csv ROW_NUM] [--error-on-factory-stopped] [common-options]"
             ),
             description="It generates values according to factory definition files.",
             add_help=False,
         )
         byfile_args_group = byfile_parser.add_argument_group("arguments")
         byfile_args_group.add_argument(
             "factories",
@@ -54,14 +54,20 @@
             "--csv",
             metavar="ROW_NUM",
             type=positive_int,
             help="if specified, it outputs generated ROW_NUM objects as CSV. "
             "When using this option, it is recommended to use a factory that generates dictionaries and "
             "to define CSV_COLUMNS in the definition file to specify the fields of the CSV.",
         )
+        byfile_args_group.add_argument(
+            "--error-on-factory-stopped",
+            action="store_true",
+            help="If specified, error is occurred in case the factory cannot generate value due to StopIteration. "
+            "If not specified, the generation simply stops in the case.",
+        )
         add_common_arguments(byfile_parser)
 
         return byfile_parser
 
     def validate_parser(self, args: Args, subparser: argparse.ArgumentParser):
         if args.output_fmt == "repr" and args.csv is not None:
             subparser.error("argument --csv: not allowed with argument --repr")
```

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_date.py` & `randog-0.9.0/randog/_main/_subcmd_def/_date.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_datetime.py` & `randog-0.9.0/randog/_main/_subcmd_def/_datetime.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_decimal.py` & `randog-0.9.0/randog/_main/_subcmd_def/_decimal.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_float.py` & `randog-0.9.0/randog/_main/_subcmd_def/_float.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_int.py` & `randog-0.9.0/randog/_main/_subcmd_def/_int.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_str.py` & `randog-0.9.0/randog/_main/_subcmd_def/_str.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_time.py` & `randog-0.9.0/randog/_main/_subcmd_def/_time.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_main/_subcmd_def/_timedelta.py` & `randog-0.9.0/randog/_main/_subcmd_def/_timedelta.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/_utils/type.py` & `randog-0.9.0/randog/_utils/type.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/factory/__init__.py` & `randog-0.9.0/randog/factory/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._base import Factory, REGENERATE_PROB_MAX
+from ._base import Factory, REGENERATE_PROB_MAX, FactoryStopException
 from ._choice import ChoiceRandomFactory, randchoice, randenum
 from ._const import const
 from ._bool import BoolRandomFactory, randbool
 from ._int import IntRandomFactory, randint
 from ._float import FloatRandomFactory, randfloat
 from ._decimal import DecimalRandomFactory, randdecimal
 from ._str import StrRandomFactory, randstr
@@ -40,9 +40,10 @@
     "randdict",
     "by_callable",
     "by_iterator",
     "increment",
     "union",
     "DictItem",
     "FactoryDef",
+    "FactoryStopException",
     "REGENERATE_PROB_MAX",
 ]
```

### Comparing `randog-0.8.0/randog/factory/_base.py` & `randog-0.9.0/randog/factory/_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,23 +9,42 @@
 T = t.TypeVar("T")
 R = t.TypeVar("R")
 
 REGENERATE_PROB_MAX = float(Fraction(1023, 1024))
 
 
 class Factory(ABC, t.Generic[T]):
-    @abstractmethod
-    def next(self) -> T:
+    def next(
+        self,
+        *,
+        raise_on_factory_stopped: bool = False,
+    ) -> T:
         """Generate a value randomly according to the rules specified when assembling the factory.
 
+        Parameters
+        ----------
+        raise_on_factory_stopped : bool, default=False
+            If True, raises `FactoryStopException` in case the factory cannot generate value due to `StopIteration`.
+            If False, simply raises `StopIteration`.
+
         Returns
         -------
         T
             a value generated randomly
         """
+        try:
+            return self._next()
+        except StopIteration:
+            if raise_on_factory_stopped:
+                raise FactoryStopException()
+            else:
+                raise
+
+    @abstractmethod
+    def _next(self) -> T:
         pass
 
     def or_none(
         self,
         prob: float = 0.1,
         *,
         lazy_choice: bool = False,
@@ -101,14 +120,15 @@
 
     def iter(
         self,
         size: int,
         *,
         regenerate: float = 0.0,
         discard: float = 0.0,
+        raise_on_factory_stopped: bool = False,
         rnd: t.Optional[Random] = None,
     ) -> t.Iterator[T]:
         """Returns an iterator which serves result randomly `size` times.
 
         Examples
         --------
         >>> import randog
@@ -119,41 +139,59 @@
         >>>
         >>> results = list(factory.iter(5))
         >>> assert len(results) == 5
 
         Parameters
         ----------
         size : int
-            the number of the iterator
+            the number of the iterator.
+            However, if the argument `raise_on_factory_stopped` is not True,
+            fewer iterations than the specified `size` will be executed if the factory is stopped.
+            Also, if the argument `discard` is specified, the size may be less.
         regenerate : float, default=0.0
             the probability that the original factory generation value is not returned as is, but is regenerated.
             It affects cases where the original factory returns a value that is not completely random.
         discard : float, default=0.0
             the probability that the original factory generation value is not returned as is, but is discarded.
             If discarded, the number of times the value is generated is less than `size`.
+        raise_on_factory_stopped : bool, default=False
+            If True, the iteration raises `FactoryStopException` in case the factory cannot generate value due to
+            `StopIteration`.
+            If False, the iteration simply stops in the case.
         rnd : Random, optional
             random number generator to be used
 
         Returns
         -------
         Iterator[T]
             An iterator
         """
-        return FactoryIter(self, size, regenerate=regenerate, discard=discard, rnd=rnd)
+        return FactoryIter(
+            self,
+            size,
+            regenerate=regenerate,
+            discard=discard,
+            raise_on_factory_stopped=raise_on_factory_stopped,
+            rnd=rnd,
+        )
 
     def infinity_iter(
         self,
         *,
         regenerate: float = 0.0,
+        raise_on_factory_stopped: bool = False,
         rnd: t.Optional[Random] = None,
     ) -> t.Iterator[T]:
         """Returns an infinity iterator which serves result randomly.
 
         The result is INFINITY so do NOT use it directly with `for`, `list`, and so on.
 
+        However, if the argument `raise_on_factory_stopped` is not True,
+        the iterator will be stopped if the factory is stopped.
+
         Examples
         --------
         >>> import randog
         >>> factory = randog.factory.randstr(length=5)
         >>>
         >>> keys = ["foo", "bar"]
         >>> for k, v in zip(keys, factory.infinity_iter()):
@@ -161,53 +199,65 @@
         ...     assert isinstance(v, str)
 
         Parameters
         ----------
         regenerate : float, default=0.0
             the probability that the original factory generation value is not returned as is, but is regenerated.
             It affects cases where the original factory returns a value that is not completely random.
+        raise_on_factory_stopped : bool, default=False
+            If True, the iteration raises `FactoryStopException` in case the factory cannot generate value due to
+            `StopIteration`.
+            If False, the iteration simply stops in the case.
         rnd : Random, optional
             random number generator to be used
 
         Returns
         -------
         Iterator[T]
             An infinity iterator
         """
-        return FactoryIter(self, None, regenerate=regenerate, rnd=rnd)
+        return FactoryIter(
+            self,
+            None,
+            regenerate=regenerate,
+            raise_on_factory_stopped=raise_on_factory_stopped,
+            rnd=rnd,
+        )
 
 
 class PostFactory(Factory[R], t.Generic[T, R]):
     _base_factory: Factory[T]
     _post_process: t.Callable[[T], R]
 
     def __init__(self, base_factory: Factory[T], post_process: t.Callable[[T], R]):
         self._base_factory = base_factory
         self._post_process = post_process
 
-    def next(self) -> R:
+    def _next(self) -> R:
         pre_result = self._base_factory.next()
         return self._post_process(pre_result)
 
 
 class FactoryIter(t.Generic[T], t.Iterator[T]):
     _rnd: random.Random
     _factory: Factory[T]
     _size: t.Union[int, float]
     _regenerate_prob: float
     _discard_prob: float
+    _raise_on_factory_stopped: bool
     _count: int = 0
 
     def __init__(
         self,
         factory: Factory[T],
         size: t.Union[int, None],
         *,
         regenerate: float = 0.0,
         discard: float = 0.0,
+        raise_on_factory_stopped: bool = False,
         rnd: t.Optional[Random] = None,
     ):
         self._rnd = dfor(rnd, random.Random())
         self._factory = factory
 
         if regenerate > 0 and discard > 0:
             raise ValueError(
@@ -219,29 +269,38 @@
             )
         if discard < 0 or 1 < discard:
             raise ValueError("the probability `discard` must range from 0 to 1")
 
         self._size = size if size is not None else float("Infinity")
         self._regenerate_prob = regenerate
         self._discard_prob = discard
+        self._raise_on_factory_stopped = raise_on_factory_stopped
 
     def __next__(self) -> T:
         while True:
             if self._count >= self._size:
                 raise StopIteration()
 
             self._count += 1
 
             # Regenerate until break
             while True:
-                generated = self._factory.next()
+                generated = self._factory.next(
+                    raise_on_factory_stopped=self._raise_on_factory_stopped
+                )
+
                 if (
                     self._regenerate_prob <= 0
                     or self._rnd.random() >= self._regenerate_prob
                 ):
                     break
 
             # Probabilistically, discard the value generated this time and proceed to the next one
             if self._discard_prob > 0 and self._rnd.random() < self._discard_prob:
                 continue
 
             return generated
+
+
+class FactoryStopException(Exception):
+    def __init__(self):
+        super().__init__("the factory stopped generating")
```

### Comparing `randog-0.8.0/randog/factory/_bool.py` & `randog-0.9.0/randog/factory/_bool.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,9 +58,9 @@
         self._prop_true = prop_true
 
         if self._prop_true < 0.0 or 1.0 < self._prop_true:
             raise FactoryConstructionError(
                 "the probability `prob_true` must range from 0 to 1"
             )
 
-    def next(self) -> int:
+    def _next(self) -> int:
         return self._random.random() < self._prop_true
```

### Comparing `randog-0.8.0/randog/factory/_by_callable.py` & `randog-0.9.0/randog/factory/_by_callable.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,9 +30,9 @@
         Parameters
         ----------
         func : () -> T
             the function generating value
         """
         self._callable = func
 
-    def next(self) -> T:
+    def _next(self) -> T:
         return self._callable()
```

### Comparing `randog-0.8.0/randog/factory/_by_iterator.py` & `randog-0.9.0/randog/factory/_by_iterator.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,9 +30,9 @@
         Parameters
         ----------
         iterator : Iterator[T]
             the iterator generating value
         """
         self._iterator = iterator
 
-    def next(self) -> T:
+    def _next(self) -> T:
         return next(self._iterator)
```

### Comparing `randog-0.8.0/randog/factory/_choice.py` & `randog-0.9.0/randog/factory/_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         if len(values) <= 0:
             raise FactoryConstructionError("empty candidate for randchoice")
         if self._weights is not None and len(self._weights) != len(self._values):
             raise FactoryConstructionError(
                 "the number of weights must match the candidates"
             )
 
-    def next(self) -> t.Any:
+    def _next(self) -> t.Any:
         return self._random.choices(self._values, self._weights)[0]
 
 
 def __validate_num(value, *, err_msg) -> numbers.Real:
     if isinstance(value, numbers.Real) and not isinstance(value, bool):
         return value
     else:
```

### Comparing `randog-0.8.0/randog/factory/_date.py` & `randog-0.9.0/randog/factory/_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._min, self._max = self._normalize(minimum, maximum)
 
         if self._min > self._max:
             raise FactoryConstructionError("empty range for randdate")
 
         self._range = (self._max - self._min).days
 
-    def next(self) -> dt.date:
+    def _next(self) -> dt.date:
         relative_days = self._random.randint(0, self._range)
         return self._min + dt.timedelta(days=relative_days)
 
     @classmethod
     def _normalize(
         cls,
         minimum: t.Union[dt.date, dt.datetime, None] = None,
```

### Comparing `randog-0.8.0/randog/factory/_datetime.py` & `randog-0.9.0/randog/factory/_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 "cannot define range for randdatetime with a naive datetime and an aware datetime"
             )
         if self._min > self._max:
             raise FactoryConstructionError("empty range for randdatetime")
 
         self._range = self._max - self._min
 
-    def next(self) -> dt.datetime:
+    def _next(self) -> dt.datetime:
         weight = self._random.random()
 
         pre_result = self._min + self._range * weight
         if self._fix_timezone:
             if pre_result.tzinfo is not None and self._fixed_timezone is not None:
                 return pre_result.astimezone(self._fixed_timezone)
             else:
```

### Comparing `randog-0.8.0/randog/factory/_decimal.py` & `randog-0.9.0/randog/factory/_decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         """
         self._random = dfor(rnd, Random())
         self._factory = randfloat(
             minimum, maximum, p_inf=p_inf, n_inf=n_inf, nan=nan, rnd=self._random
         )
         self._decimal_len = dforc(lambda x: Decimal(1).scaleb(-x), decimal_len)
 
-    def next(self) -> Decimal:
+    def _next(self) -> Decimal:
         pre_value = self._factory.next()
         value = Decimal(pre_value)
 
         if self._decimal_len is not None and value.is_finite():
             value = value.quantize(self._decimal_len)
 
         return value
```

### Comparing `randog-0.8.0/randog/factory/_dict.py` & `randog-0.9.0/randog/factory/_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             the factories of each key
         rnd : Random, optional
             random number generator to be used
         """
         self._random = dfor(rnd, Random())
         self._items = items
 
-    def next(self) -> dict:
+    def _next(self) -> dict:
         result = {}
 
         for key, cond in self._items.items():
             if self._random.random() < cond.prop_exists:
                 result[key] = cond.factory.next()
 
         return result
```

### Comparing `randog-0.8.0/randog/factory/_float.py` & `randog-0.9.0/randog/factory/_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 "the probabilities `p_inf`, `n_inf`, and `nan` must range from 0 to 1"
             )
         if self._p_inf + self._n_inf + self._nan > 1.0:
             raise FactoryConstructionError(
                 "the sum of probabilities `p_inf`, `n_inf`, and `nan` must range from 0 to 1"
             )
 
-    def next(self) -> float:
+    def _next(self) -> float:
         pre_weight = self._random.random()
         pre_weight -= self._p_inf
         if pre_weight < 0:
             return float("inf")
         pre_weight -= self._n_inf
         if pre_weight < 0:
             return float("-inf")
```

### Comparing `randog-0.8.0/randog/factory/_from_example.py` & `randog-0.9.0/randog/factory/_from_example.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/factory/_from_pyfile.py` & `randog-0.9.0/randog/factory/_from_pyfile.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/factory/_increment.py` & `randog-0.9.0/randog/factory/_increment.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/factory/_int.py` & `randog-0.9.0/randog/factory/_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
         self._random = dfor(rnd, Random())
         self._min = minimum
         self._max = maximum
 
         if minimum > maximum:
             raise FactoryConstructionError("empty range for randint")
 
-    def next(self) -> int:
+    def _next(self) -> int:
         return self._random.randint(self._min, self._max)
```

### Comparing `randog-0.8.0/randog/factory/_list.py` & `randog-0.9.0/randog/factory/_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,18 +116,38 @@
             generated += 1
         while generated < length:
             yield last_factory
             generated += 1
 
     def _next_generator(self) -> t.Iterator[t.Any]:
         length = self._next_length()
-        for factory in self._factory_generator(length):
-            yield factory.next()
+        return _GeneratedAsIter(self._factory_generator(length))
 
     def _next_length(self) -> int:
         if isinstance(self._length, Factory):
             return self._length.next()
         else:
             return self._length
 
-    def next(self) -> T:
-        return self._type(self._next_generator())
+    def _next(self) -> T:
+        try:
+            return self._type(self._next_generator())
+        except _StopIterationOfItem:
+            raise StopIteration()
+
+
+class _GeneratedAsIter(t.Iterator[t.Any]):
+    _factories_iter: t.Iterator[Factory]
+
+    def __init__(self, factories_iter: t.Iterator[Factory]):
+        self._factories_iter = factories_iter
+
+    def __next__(self) -> t.Any:
+        factory = next(self._factories_iter)
+        try:
+            return factory.next()
+        except StopIteration:
+            raise _StopIterationOfItem()
+
+
+class _StopIterationOfItem(Exception):
+    pass
```

### Comparing `randog-0.8.0/randog/factory/_str/__init__.py` & `randog-0.9.0/randog/factory/_str/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             and self._length > 0
             and len(self._charset) == 0
         ):
             raise FactoryConstructionError(
                 "the charset for randstr() must not be empty if length is positive"
             )
 
-    def next(self) -> str:
+    def _next(self) -> str:
         length = self._next_length()
         return "".join(self._random.choices(self._charset, k=length))
 
     def _next_length(self) -> int:
         if isinstance(self._length, Factory):
             return self._length.next()
         else:
```

### Comparing `randog-0.8.0/randog/factory/_str/_regex.py` & `randog-0.9.0/randog/factory/_str/_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
         Raises
         ------
         FactoryConstructionError
             When the specified generating conditions are inconsistent.
         """
         self._regex = regex
 
-    def next(self) -> str:
+    def _next(self) -> str:
         return rstr.xeger(self._regex)
```

### Comparing `randog-0.8.0/randog/factory/_time.py` & `randog-0.9.0/randog/factory/_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             min_datetime,
             max_datetime,
             fix_timezone=fix_timezone,
             fixed_timezone=fixed_timezone,
             rnd=rnd,
         ).post_process(lambda v: v.time().replace(tzinfo=v.tzinfo))
 
-    def next(self) -> dt.time:
+    def _next(self) -> dt.time:
         return self._base.next()
 
     @classmethod
     def _normalize(
         cls,
         minimum: t.Union[dt.time, None],
         maximum: t.Union[dt.time, None],
```

### Comparing `randog-0.8.0/randog/factory/_timedelta.py` & `randog-0.9.0/randog/factory/_timedelta.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         self._min_by_unit = math.ceil(self._min / self._unit)
         self._max_by_unit = math.floor(self._max / self._unit)
         if self._min_by_unit > self._max_by_unit:
             raise FactoryConstructionError("empty range for randtimedelta")
         self._inner_factory = randint(self._min_by_unit, self._max_by_unit, rnd=rnd)
 
-    def next(self) -> dt.timedelta:
+    def _next(self) -> dt.timedelta:
         return self._unit * self._inner_factory.next()
 
     @classmethod
     def _normalize(
         cls,
         minimum: t.Optional[dt.timedelta] = None,
         maximum: t.Optional[dt.timedelta] = None,
```

### Comparing `randog-0.8.0/randog/factory/_union.py` & `randog-0.9.0/randog/factory/_union.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if len(factories) <= 0:
             raise FactoryConstructionError("no factory is given to union()")
         if self._weights is not None and len(self._weights) != len(self._factories):
             raise FactoryConstructionError(
                 "the number of weights must match the factories"
             )
 
-    def next(self) -> t.Any:
+    def _next(self) -> t.Any:
         return self._random.choices(self._factories, self._weights)[0].next()
 
 
 class UnionRandomLazyChoiceFactory(UnionRandomFactory):
-    def next(self) -> t.Any:
+    def _next(self) -> t.Any:
         values = [f.next() for f in self._factories]
         return self._random.choices(values, self._weights)[0]
```

### Comparing `randog-0.8.0/randog/sqlalchemy/_construct.py` & `randog-0.9.0/randog/sqlalchemy/_construct.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/sqlalchemy/_custom_func.py` & `randog-0.9.0/randog/sqlalchemy/_custom_func.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog/timedelta_util.py` & `randog-0.9.0/randog/timedelta_util.py`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/randog.egg-info/PKG-INFO` & `randog-0.9.0/randog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: randog
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generate data randomly
 Home-page: UNKNOWN
 Author: k-izumi
 Author-email: k.izumi.ysk@gmail.com
 Maintainer: k-izumi
 Maintainer-email: k.izumi.ysk@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/unaguna/random-obj-generator/issues
 Project-URL: Documentation, https://unaguna.github.io/random-obj-generator/
 Project-URL: Source Code, https://github.com/unaguna/random-obj-generator
-Description: **randog 0.8.0 — Randomly object generator**
+Description: **randog 0.9.0 — Randomly object generator**
         
         **randog** is a package which helps to generate data randomly.
         
         ## Install
         
         You can install from PyPI.
```

### Comparing `randog-0.8.0/randog.egg-info/SOURCES.txt` & `randog-0.9.0/randog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `randog-0.8.0/setup.py` & `randog-0.9.0/setup.py`

 * *Files identical despite different names*

