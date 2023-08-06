# Comparing `tmp/naruno_remote_app-0.60.3.tar.gz` & `tmp/naruno_remote_app-0.60.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.60.3.tar", last modified: Wed Aug  2 15:08:34 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.60.4.tar", last modified: Sun Aug  6 19:45:59 2023, max compression
```

## Comparing `naruno_remote_app-0.60.3.tar` & `naruno_remote_app-0.60.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:34.950726 naruno_remote_app-0.60.3/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 15:08:34.950726 naruno_remote_app-0.60.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:34.950726 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:34.000000 naruno_remote_app-0.60.3/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:08:34.950726 naruno_remote_app-0.60.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 15:08:12.000000 naruno_remote_app-0.60.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:59.203997 naruno_remote_app-0.60.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 19:45:59.203997 naruno_remote_app-0.60.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:45:59.203997 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:45:59.000000 naruno_remote_app-0.60.4/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:45:59.203997 naruno_remote_app-0.60.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 19:45:41.000000 naruno_remote_app-0.60.4/setup.py
```

