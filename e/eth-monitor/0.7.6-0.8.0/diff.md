# Comparing `tmp/eth-monitor-0.7.6.tar.gz` & `tmp/eth-monitor-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-monitor-0.7.6.tar", last modified: Sat Jun  3 07:31:53 2023, max compression
+gzip compressed data, was "eth-monitor-0.8.0.tar", last modified: Sun Aug  6 13:20:35 2023, max compression
```

## Comparing `eth-monitor-0.7.6.tar` & `eth-monitor-0.8.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.903309 eth-monitor-0.7.6/
--rw-r--r--   0 lash      (1000) lash      (1000)     1630 2023-05-13 20:44:55.000000 eth-monitor-0.7.6/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.7.6/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.7.6/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-06-03 07:31:53.903309 eth-monitor-0.7.6/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.7.6/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.7.6/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.7.6/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/
--rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.7.6/eth_monitor/callback.py
--rw-r--r--   0 lash      (1000) lash      (1000)      591 2023-06-03 07:24:54.000000 eth-monitor-0.7.6/eth_monitor/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3190 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1923 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.7.6/eth_monitor/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/cli/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.896643 eth-monitor-0.7.6/eth_monitor/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/data/config/cache.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/data/config/filter.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      243 2022-10-13 07:08:18.000000 eth-monitor-0.7.6/eth_monitor/data/config/monitor.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/data/config/renderer.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/filters/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.7.6/eth_monitor/filters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      580 2022-11-11 05:56:27.000000 eth-monitor-0.7.6/eth_monitor/filters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      263 2022-11-11 05:56:27.000000 eth-monitor-0.7.6/eth_monitor/filters/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      732 2022-11-11 05:56:27.000000 eth-monitor-0.7.6/eth_monitor/filters/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-02-23 02:16:57.000000 eth-monitor-0.7.6/eth_monitor/filters/out.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/importers/
--rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.7.6/eth_monitor/importers/etherscan.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/index.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/mock/
--rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.7.6/eth_monitor/mock/filter_plain.py
--rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.7.6/eth_monitor/mock/filter_ruled.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/rules.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/runnable/import.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/eth_monitor/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3298 2023-02-26 19:39:52.000000 eth-monitor-0.7.6/eth_monitor/runnable/sync.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.7.6/eth_monitor/runnable/sync_thread_range.py
--rw-r--r--   0 lash      (1000) lash      (1000)    12753 2023-06-03 07:24:11.000000 eth-monitor-0.7.6/eth_monitor/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/eth_monitor.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1237 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      105 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-06-03 07:31:53.000000 eth-monitor-0.7.6/eth_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.896643 eth-monitor-0.7.6/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.7.6/man/build/eth-monitor-import.1
--rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.7.6/man/build/eth-monitor-list.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.7.6/man/build/eth-monitor-sync.1
--rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.7.6/man/build/eth-monitor.1
--rw-r--r--   0 lash      (1000) lash      (1000)      105 2023-06-03 07:04:12.000000 eth-monitor-0.7.6/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-06-03 07:31:53.903309 eth-monitor-0.7.6/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.7.6/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-06-03 07:31:53.899976 eth-monitor-0.7.6/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.7.6/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1733 2023-08-06 13:10:25.000000 eth-monitor-0.8.0/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.0/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.0/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.0/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.0/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.0/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/
+-rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/callback.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      645 2023-08-06 12:18:29.000000 eth-monitor-0.8.0/eth_monitor/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3190 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1923 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.0/eth_monitor/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      271 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/cli/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.118382 eth-monitor-0.8.0/eth_monitor/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/data/config/cache.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/data/config/filter.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      243 2022-10-13 07:08:18.000000 eth-monitor-0.8.0/eth_monitor/data/config/monitor.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/data/config/renderer.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/filters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/filters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      580 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      263 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      732 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/filters/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-02-23 02:16:57.000000 eth-monitor-0.8.0/eth_monitor/filters/out.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor/importers/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.0/eth_monitor/importers/etherscan.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/eth_monitor/mock/
+-rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/mock/filter_plain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/mock/filter_ruled.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4240 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/rules.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/eth_monitor/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/runnable/import.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/eth_monitor/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3298 2023-02-26 19:39:52.000000 eth-monitor-0.8.0/eth_monitor/runnable/sync.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.0/eth_monitor/runnable/sync_thread_range.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    12798 2023-08-06 12:17:19.000000 eth-monitor-0.8.0/eth_monitor/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.121715 eth-monitor-0.8.0/eth_monitor.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1237 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-06 13:20:35.000000 eth-monitor-0.8.0/eth_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.118382 eth-monitor-0.8.0/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5946 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-import.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5557 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-list.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor-sync.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    10183 2023-05-13 20:02:53.000000 eth-monitor-0.8.0/man/build/eth-monitor.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-06 13:08:43.000000 eth-monitor-0.8.0/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.0/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-06 13:20:35.125049 eth-monitor-0.8.0/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.0/tests/test_basic.py
```

### Comparing `eth-monitor-0.7.6/CHANGELOG` & `eth-monitor-0.8.0/CHANGELOG`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+- 0.8.0
+	* Implement RPC batch limits for syncer
+- 0.7.6
+	* Make rpc dialect work with chain interface
 - 0.7.5
 	* Add readme (from man page)
 	* Add package descriptino (from man page)
 - 0.7.4
 	* Add man pages to package
 - 0.7.3
 	* Upgrade deps
```

### Comparing `eth-monitor-0.7.6/LICENSE` & `eth-monitor-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/PKG-INFO` & `eth-monitor-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.7.6
+Version: 0.8.0
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NAME
 
 eth-monitor - Cache, index and monitor transactions with an EVM node rpc
```

### Comparing `eth-monitor-0.7.6/README.md` & `eth-monitor-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/WAIVER` & `eth-monitor-0.8.0/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/WAIVER.asc` & `eth-monitor-0.8.0/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/callback.py` & `eth-monitor-0.8.0/eth_monitor/callback.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/chain.py` & `eth-monitor-0.8.0/eth_monitor/chain.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from chainlib.eth.tx import (
         receipt,
         Tx,
         )
 
 class EthChainInterface(ChainInterface):
 
-    def __init__(self, dialect_filter=None):
+    def __init__(self, dialect_filter=None, batch_limit=1):
+        self.batch_limit = batch_limit
         self._block_latest = block_latest
         self._block_by_number = block_by_number
         self._block_from_src = Block.from_src
         self._tx_receipt = receipt
         self._src_normalize = Tx.src_normalize
         self._dialect_filter = dialect_filter
```

### Comparing `eth-monitor-0.7.6/eth_monitor/cli/arg.py` & `eth-monitor-0.8.0/eth_monitor/cli/arg.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/cli/config.py` & `eth-monitor-0.8.0/eth_monitor/cli/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/cli/log.py` & `eth-monitor-0.8.0/eth_monitor/cli/log.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/config.py` & `eth-monitor-0.8.0/eth_monitor/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/filters/base.py` & `eth-monitor-0.8.0/eth_monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/filters/cache.py` & `eth-monitor-0.8.0/eth_monitor/filters/cache.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/filters/out.py` & `eth-monitor-0.8.0/eth_monitor/filters/out.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/importers/etherscan.py` & `eth-monitor-0.8.0/eth_monitor/importers/etherscan.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/index.py` & `eth-monitor-0.8.0/eth_monitor/index.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/rules.py` & `eth-monitor-0.8.0/eth_monitor/rules.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/runnable/import.py` & `eth-monitor-0.8.0/eth_monitor/runnable/import.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/runnable/list.py` & `eth-monitor-0.8.0/eth_monitor/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/runnable/sync.py` & `eth-monitor-0.8.0/eth_monitor/runnable/sync.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/runnable/sync_thread_range.py` & `eth-monitor-0.8.0/eth_monitor/runnable/sync_thread_range.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/eth_monitor/settings.py` & `eth-monitor-0.8.0/eth_monitor/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     ifc = EthChainInterface(dialect=settings.get('RPC_DIALECT_FILTER'))
     settings.set('SYNCER_INTERFACE', ifc)
     return settings
 
 
 def process_sync(settings, config):
     dialect_filter = settings.get('RPC_DIALECT_FILTER')
-    settings.set('SYNCER_INTERFACE', EthChainInterface(dialect_filter=dialect_filter))
+    settings.set('SYNCER_INTERFACE', EthChainInterface(dialect_filter=dialect_filter, batch_limit=settings.get('RPC_BATCH_LIMIT')))
     settings = process_sync_range(settings, config)
     return settings
 #def process_sync(settings, config):
 #    settings = process_sync_interface(settings, config)
 #    settings = process_sync_backend(settings, config)
 #    settings = process_sync_range(settings, config)
 #    return settings
```

### Comparing `eth-monitor-0.7.6/eth_monitor.egg-info/PKG-INFO` & `eth-monitor-0.8.0/eth_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.7.6
+Version: 0.8.0
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NAME
 
 eth-monitor - Cache, index and monitor transactions with an EVM node rpc
```

### Comparing `eth-monitor-0.7.6/eth_monitor.egg-info/SOURCES.txt` & `eth-monitor-0.8.0/eth_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/man/build/eth-monitor-import.1` & `eth-monitor-0.8.0/man/build/eth-monitor-import.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/man/build/eth-monitor-list.1` & `eth-monitor-0.8.0/man/build/eth-monitor-list.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/man/build/eth-monitor-sync.1` & `eth-monitor-0.8.0/man/build/eth-monitor-sync.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/man/build/eth-monitor.1` & `eth-monitor-0.8.0/man/build/eth-monitor.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/setup.cfg` & `eth-monitor-0.8.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-monitor
-version = 0.7.6
+version = 0.8.0
 description = Monitor and cache transactions using match filters
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-monitor
 keywords = 
 	dlt
 	blockchain
@@ -21,15 +21,15 @@
 	Topic :: Internet
 license = AGPLv3+
 licence_files = 
 	LICENSE
 
 [options]
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 packages = 
 	eth_monitor
 	eth_monitor.importers
 	eth_monitor.filters
 	eth_monitor.runnable
 	eth_monitor.mock
 	eth_monitor.cli
```

### Comparing `eth-monitor-0.7.6/setup.py` & `eth-monitor-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.7.6/tests/test_basic.py` & `eth-monitor-0.8.0/tests/test_basic.py`

 * *Files identical despite different names*

