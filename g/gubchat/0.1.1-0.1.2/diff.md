# Comparing `tmp/gubchat-0.1.1.tar.gz` & `tmp/gubchat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gubchat-0.1.1.tar", last modified: Sat Aug  5 02:54:18 2023, max compression
+gzip compressed data, was "gubchat-0.1.2.tar", last modified: Sun Aug  6 20:24:05 2023, max compression
```

## Comparing `gubchat-0.1.1.tar` & `gubchat-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2023-08-05 02:54:18.595061 gubchat-0.1.1/
--rw-r--r--   0 douglas   (1000) douglas   (1000)     1071 2023-08-05 01:51:51.000000 gubchat-0.1.1/LICENSE
--rw-r--r--   0 douglas   (1000) douglas   (1000)      187 2023-08-05 02:54:18.595061 gubchat-0.1.1/PKG-INFO
--rw-r--r--   0 douglas   (1000) douglas   (1000)       35 2023-08-05 01:51:51.000000 gubchat-0.1.1/README.md
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2023-08-05 02:54:18.595061 gubchat-0.1.1/gubchat/
--rw-r--r--   0 douglas   (1000) douglas   (1000)        0 2023-08-04 13:59:34.000000 gubchat-0.1.1/gubchat/__init__.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)     6625 2023-08-05 01:47:13.000000 gubchat-0.1.1/gubchat/main.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)     4360 2023-08-05 01:39:00.000000 gubchat-0.1.1/gubchat/user_auth.py
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2023-08-05 02:54:18.595061 gubchat-0.1.1/gubchat.egg-info/
--rw-r--r--   0 douglas   (1000) douglas   (1000)      187 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/PKG-INFO
--rw-r--r--   0 douglas   (1000) douglas   (1000)      277 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/SOURCES.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)        1 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/dependency_links.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)       46 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/entry_points.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)       58 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/requires.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)        8 2023-08-05 02:54:18.000000 gubchat-0.1.1/gubchat.egg-info/top_level.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)      449 2023-08-05 02:52:46.000000 gubchat-0.1.1/pyproject.toml
--rw-r--r--   0 douglas   (1000) douglas   (1000)       38 2023-08-05 02:54:18.595061 gubchat-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.247000 gubchat-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 20:23:56.000000 gubchat-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-06 20:24:05.247000 gubchat-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 20:23:56.000000 gubchat-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.243000 gubchat-0.1.2/gubchat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/gubchatapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/twitch_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-08-06 20:23:56.000000 gubchat-0.1.2/gubchat/user_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:24:05.243000 gubchat-0.1.2/gubchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 20:24:05.000000 gubchat-0.1.2/gubchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-06 20:23:56.000000 gubchat-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:24:05.247000 gubchat-0.1.2/setup.cfg
```

### Comparing `gubchat-0.1.1/LICENSE` & `gubchat-0.1.2/LICENSE`

 * *Files identical despite different names*

