# Comparing `tmp/veilid-0.1.0.tar.gz` & `tmp/veilid-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilid-0.1.0.tar", max compression
+gzip compressed data, was "veilid-0.1.7.tar", max compression
```

## Comparing `veilid-0.1.0.tar` & `veilid-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,14 @@
--rw-r--r--   0        0        0       30 2023-07-11 20:15:33.000114 veilid-0.1.0/README.md
--rw-r--r--   0        0        0      403 2023-07-11 20:13:59.508622 veilid-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 20:14:14.597658 veilid-0.1.0/veilid/__init__.py
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 veilid-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    15581 2023-08-02 19:08:47.242155 veilid-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0      291 2023-08-02 19:08:47.242155 veilid-0.1.7/README.md
+-rw-r--r--   0        0        0      472 2023-08-05 14:40:00.554881 veilid-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-08-02 19:08:47.242155 veilid-0.1.7/veilid/__init__.py
+-rw-r--r--   0        0        0     9363 2023-08-05 14:40:00.554881 veilid-0.1.7/veilid/api.py
+-rw-r--r--   0        0        0     5129 2023-08-02 19:08:47.242155 veilid-0.1.7/veilid/config.py
+-rw-r--r--   0        0        0     3560 2023-08-05 14:40:00.554881 veilid-0.1.7/veilid/error.py
+-rw-r--r--   0        0        0    37749 2023-08-05 14:40:00.554881 veilid-0.1.7/veilid/json_api.py
+-rw-r--r--   0        0        0     2873 2023-08-05 14:40:00.558881 veilid-0.1.7/veilid/operations.py
+-rw-r--r--   0        0        0    96049 2023-08-02 19:08:47.242155 veilid-0.1.7/veilid/schema/RecvMessage.json
+-rw-r--r--   0        0        0    34019 2023-08-02 19:08:47.242155 veilid-0.1.7/veilid/schema/Request.json
+-rw-r--r--   0        0        0    11874 2023-08-05 14:40:00.558881 veilid-0.1.7/veilid/state.py
+-rw-r--r--   0        0        0    11399 2023-08-05 14:40:00.558881 veilid-0.1.7/veilid/types.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 veilid-0.1.7/PKG-INFO
```

