# Comparing `tmp/statham-schema-0.8.0.tar.gz` & `tmp/statham-schema-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/statham-schema-0.8.0.tar", last modified: Thu Apr  9 15:14:16 2020, max compression
+gzip compressed data, was "dist/statham-schema-0.9.0.tar", last modified: Mon Apr 20 22:13:04 2020, max compression
```

## Comparing `statham-schema-0.8.0.tar` & `statham-schema-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/
--rw-rw-r--   0 jack      (1000) jack      (1000)      209 2019-11-14 10:08:15.000000 statham-schema-0.8.0/pyproject.toml
--rw-r--r--   0 jack      (1000) jack      (1000)     4504 2020-04-04 00:07:18.000000 statham-schema-0.8.0/README.md
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)       14 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)     1394 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)     5890 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)       75 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/requires.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       58 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham_schema.egg-info/entry_points.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       79 2020-04-09 15:14:16.000000 statham-schema-0.8.0/setup.cfg
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham/dsl/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham/dsl/validation/
--rw-r--r--   0 jack      (1000) jack      (1000)     2494 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/validation/array.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1337 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/validation/string.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1681 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/validation/numeric.py
--rw-r--r--   0 jack      (1000) jack      (1000)     4043 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/validation/base.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1696 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/validation/format.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1430 2020-04-04 00:07:18.000000 statham-schema-0.8.0/statham/dsl/validation/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2590 2020-04-04 00:07:18.000000 statham-schema-0.8.0/statham/dsl/validation/object.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2922 2020-04-03 17:31:48.000000 statham-schema-0.8.0/statham/dsl/helpers.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/statham/dsl/elements/
--rw-r--r--   0 jack      (1000) jack      (1000)     5493 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/elements/composition.py
--rw-r--r--   0 jack      (1000) jack      (1000)      655 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/elements/null.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2257 2020-04-05 18:40:48.000000 statham-schema-0.8.0/statham/dsl/elements/array.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1269 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/elements/items.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1093 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/elements/string.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1720 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/elements/numeric.py
--rw-r--r--   0 jack      (1000) jack      (1000)     7505 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/dsl/elements/base.py
--rw-r--r--   0 jack      (1000) jack      (1000)     5378 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/dsl/elements/meta.py
--rw-r--r--   0 jack      (1000) jack      (1000)      585 2020-04-03 22:29:44.000000 statham-schema-0.8.0/statham/dsl/elements/boolean.py
--rw-r--r--   0 jack      (1000) jack      (1000)      458 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/elements/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3023 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/dsl/elements/object.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3223 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/dsl/elements/properties.py
--rw-r--r--   0 jack      (1000) jack      (1000)      859 2020-04-04 00:07:18.000000 statham-schema-0.8.0/statham/dsl/constants.py
--rw-r--r--   0 jack      (1000) jack      (1000)    15538 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/dsl/parser.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2712 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/dsl/exceptions.py
--rw-r--r--   0 jack      (1000) jack      (1000)        0 2020-03-08 16:48:01.000000 statham-schema-0.8.0/statham/dsl/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3686 2020-04-06 13:31:23.000000 statham-schema-0.8.0/statham/dsl/property.py
--rw-r--r--   0 jack      (1000) jack      (1000)       22 2020-04-09 15:13:57.000000 statham-schema-0.8.0/statham/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     5290 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/orderer.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3408 2020-04-02 21:13:50.000000 statham-schema-0.8.0/statham/__main__.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1370 2020-03-20 16:54:56.000000 statham-schema-0.8.0/statham/titles.py
--rw-r--r--   0 jack      (1000) jack      (1000)      761 2020-04-09 15:04:38.000000 statham-schema-0.8.0/statham/serializer.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1345 2019-12-13 11:57:14.000000 statham-schema-0.8.0/setup.py
--rw-r--r--   0 jack      (1000) jack      (1000)     7187 2020-04-09 15:13:57.000000 statham-schema-0.8.0/CHANGELOG.md
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/tests/
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-09 15:14:16.000000 statham-schema-0.8.0/tests/models/
--rw-r--r--   0 jack      (1000) jack      (1000)     2231 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/field_validation.py
--rw-r--r--   0 jack      (1000) jack      (1000)      704 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/remote_ref.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1107 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/autoname.py
--rw-r--r--   0 jack      (1000) jack      (1000)      968 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/union_types.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1127 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/simple.py
--rw-r--r--   0 jack      (1000) jack      (1000)      594 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/multi_object.py
--rw-rw-r--   0 jack      (1000) jack      (1000)        0 2019-11-16 17:48:23.000000 statham-schema-0.8.0/tests/models/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)      346 2020-04-09 15:04:38.000000 statham-schema-0.8.0/tests/models/array_item_validation.py
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2019-11-25 12:58:52.000000 statham-schema-0.8.0/MANIFEST.in
--rw-r--r--   0 jack      (1000) jack      (1000)       75 2020-04-04 12:34:08.000000 statham-schema-0.8.0/requirements.txt
--rw-r--r--   0 jack      (1000) jack      (1000)     5890 2020-04-09 15:14:16.000000 statham-schema-0.8.0/PKG-INFO
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham/
+-rw-r--r--   0 jack      (1000) jack      (1000)       22 2020-04-20 22:12:39.000000 statham-schema-0.9.0/statham/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3308 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/__main__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1371 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/titles.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham/serializers/
+-rw-r--r--   0 jack      (1000) jack      (1000)      233 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/serializers/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3052 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/serializers/python.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     4394 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/serializers/orderer.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     4458 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/serializers/json.py
+-rw-r--r--   0 jack      (1000) jack      (1000)        0 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/py.typed
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham/dsl/
+-rw-r--r--   0 jack      (1000) jack      (1000)        0 2020-04-17 14:23:22.000000 statham-schema-0.9.0/statham/dsl/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3649 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/property.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2923 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/helpers.py
+-rw-r--r--   0 jack      (1000) jack      (1000)    16853 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/parser.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      859 2020-04-17 14:23:22.000000 statham-schema-0.9.0/statham/dsl/constants.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2906 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/exceptions.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham/dsl/elements/
+-rw-r--r--   0 jack      (1000) jack      (1000)      458 2020-04-17 14:23:22.000000 statham-schema-0.9.0/statham/dsl/elements/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1603 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/numeric.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     5378 2020-04-19 17:37:44.000000 statham-schema-0.9.0/statham/dsl/elements/meta.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      592 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/boolean.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      662 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/null.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2275 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/array.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     6419 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/composition.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3368 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/properties.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3287 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/object.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1029 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/string.py
+-rw-r--r--   0 jack      (1000) jack      (1000)    11886 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/base.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1413 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/elements/items.py
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham/dsl/validation/
+-rw-r--r--   0 jack      (1000) jack      (1000)     2121 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2030 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/numeric.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2877 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/array.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1992 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/format.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     3004 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/object.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1712 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/string.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     5075 2020-04-20 22:09:21.000000 statham-schema-0.9.0/statham/dsl/validation/base.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      209 2020-04-17 14:23:22.000000 statham-schema-0.9.0/pyproject.toml
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/
+-rw-r--r--   0 jack      (1000) jack      (1000)        1 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)       58 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/entry_points.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)       14 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/top_level.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)     5708 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)     1491 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)      102 2020-04-20 22:13:04.000000 statham-schema-0.9.0/statham_schema.egg-info/requires.txt
+-rw-r--r--   0 jack      (1000) jack      (1000)      102 2020-04-20 22:09:21.000000 statham-schema-0.9.0/requirements.txt
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/tests/
+drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2020-04-20 22:13:04.000000 statham-schema-0.9.0/tests/models/
+-rw-r--r--   0 jack      (1000) jack      (1000)        0 2020-04-17 14:23:22.000000 statham-schema-0.9.0/tests/models/__init__.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      578 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/remote_ref.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      863 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/union_types.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      252 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/array_item_validation.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     2202 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/field_validation.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1041 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/autoname.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1050 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/simple.py
+-rw-r--r--   0 jack      (1000) jack      (1000)      500 2020-04-17 15:05:54.000000 statham-schema-0.9.0/tests/models/multi_object.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     1388 2020-04-20 22:09:21.000000 statham-schema-0.9.0/setup.py
+-rw-r--r--   0 jack      (1000) jack      (1000)     4411 2020-04-20 22:09:21.000000 statham-schema-0.9.0/README.md
+-rw-r--r--   0 jack      (1000) jack      (1000)     8529 2020-04-20 22:12:39.000000 statham-schema-0.9.0/CHANGELOG.md
+-rw-r--r--   0 jack      (1000) jack      (1000)       79 2020-04-20 22:13:04.000000 statham-schema-0.9.0/setup.cfg
+-rw-r--r--   0 jack      (1000) jack      (1000)     5708 2020-04-20 22:13:04.000000 statham-schema-0.9.0/PKG-INFO
+-rw-r--r--   0 jack      (1000) jack      (1000)       38 2020-04-17 14:23:22.000000 statham-schema-0.9.0/MANIFEST.in
```

### Comparing `statham-schema-0.8.0/README.md` & `statham-schema-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [![Build Status](https://travis-ci.com/jacksmith15/statham-schema.svg?token=JrMQr8Ynsmu5tphpTQ2p&branch=master)](https://travis-ci.com/jacksmith15/statham-schema)
 # Statham Schema
-A tool for generating Python objects from [JSONSchema](https://json-schema.org/) documents.
+A tool for generating Python objects from [JSON Schema](https://json-schema.org/) documents.
 
 This project aims to simplify the experience of integrating with external sources, by providing:
 1. **External validation**: Ensure that incoming data matches what you expect.
 2. **Internal validation**: Ensure your application logic is consistent with the schema. Static type checking (see [mypy](http://mypy-lang.org/)) can do this job for you.
-3. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
+3. **Extensibility**: Extend the generated models with properties and methods useful to you.
+4. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
 
 The models generated by this tool are declared using a JSONSchema DSL. This DSL can easily be used to write schemas by hand, and extend models with extra features.
 
 ## Example DSL Definition
 ```python
 from typing import List
 
@@ -19,20 +20,18 @@
 
 class Choice(Object):
     choice_text: str = Property(String(maxLength=200), required=True)
     votes: int = Property(Integer(default=0))
 
 
 class Poll(Object):
-    question: str = Property(String(maxLength=200), required=True)
+    question: str = Property(String(), required=True)
     choices: List[Choice] = Property(Array(Choice), required=True)
 ```
 
-Development currently targets compatibility with JSONSchema Draft 6.
-
 # Requirements
 This package is currently tested for Python 3.6.
 
 # Installation
 This project may be installed using [pip](https://pip.pypa.io/en/stable/):
 ```
 pip install statham-schema
@@ -74,46 +73,36 @@
 
 @format_checker.register("my_format")
 def _check_my_format(value: str) -> bool:
     ...
 ```
 
 # Supported JSONSchema features
-- [x] Basic types (primitves, array, object)
-- [x] Composite primitive types
-- [x] Type validation on generated classes
-- [x] Validation of `required`
-- [x] Local references
-- [x] Type-specific validation (pattern, format, minimum, maximum etc)
-- [x] Custom string format validation
-- [x] Remote references
-- [x] `anyOf`, `oneOf`, `allOf`, `not`
-- [x] `additionalProperties`
-- [x] Tuple validation of arrays
-- [x] `additionalItems` keyword
-- [x] `minProperties`, `maxProperties` keywords
-- [x] `patternProperties` keyword
-- [x] `uniqueItems` keyword
-- [x] `propertyNames` keyword
-- [x] `const` keyword
-- [x] `contains` keyword
-- [x] `enum` keyword
-- [x] `dependencies` keyword
-- [ ] Built-in string format validation #6
-- [ ] `if`, `then`, `else` keywords
+This library is tested to support [JSON Schema Draft 6](https://json-schema.org/specification-links.html#draft-6), with the following notable exceptions:
+- Recursive references are not supported.
+- Location-independent references are not supported.
+- Changes of base URI via the `$id` keyword are not detected.
+
+Priority order for remaining features is roughly as follows:
+1. Support for features of more recent drafts.
+2. Support for the exceptions listed above.
+3. Support for features of less recent drafts.
+
+However, contributions in any of these areas are welcome.
 
 # Development
 1. Clone the repository: `git clone git@github.com:jacksmith15/statham-schema.git && cd statham-schema`
 2. Install the requirements: `pip install -r requirements.txt -r requirements-test.txt`
 3. Run `pre-commit install`
 4. Run the tests: `bash run_test.sh -c -a`
 
 This project uses the following QA tools:
 - [PyTest](https://docs.pytest.org/en/latest/) - for running unit tests.
 - [PyLint](https://www.pylint.org/) - for enforcing code style.
 - [MyPy](http://mypy-lang.org/) - for static type checking.
 - [Travis CI](https://travis-ci.org/) - for continuous integration.
+- [Black](https://black.readthedocs.io/en/stable/) - for uniform code formatting.
 
 # License
 This project is distributed under the MIT license.
 
 ![statham](https://giant.gfycat.com/GrotesqueNauticalCaracal.gif)
```

### Comparing `statham-schema-0.8.0/statham_schema.egg-info/SOURCES.txt` & `statham-schema-0.9.0/statham_schema.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 statham/__init__.py
 statham/__main__.py
-statham/orderer.py
-statham/serializer.py
+statham/py.typed
 statham/titles.py
 statham/dsl/__init__.py
 statham/dsl/constants.py
 statham/dsl/exceptions.py
 statham/dsl/helpers.py
 statham/dsl/parser.py
 statham/dsl/property.py
@@ -31,14 +30,18 @@
 statham/dsl/validation/__init__.py
 statham/dsl/validation/array.py
 statham/dsl/validation/base.py
 statham/dsl/validation/format.py
 statham/dsl/validation/numeric.py
 statham/dsl/validation/object.py
 statham/dsl/validation/string.py
+statham/serializers/__init__.py
+statham/serializers/json.py
+statham/serializers/orderer.py
+statham/serializers/python.py
 statham_schema.egg-info/PKG-INFO
 statham_schema.egg-info/SOURCES.txt
 statham_schema.egg-info/dependency_links.txt
 statham_schema.egg-info/entry_points.txt
 statham_schema.egg-info/requires.txt
 statham_schema.egg-info/top_level.txt
 tests/models/__init__.py
```

### Comparing `statham-schema-0.8.0/statham_schema.egg-info/PKG-INFO` & `statham-schema-0.9.0/statham_schema.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: statham-schema
-Version: 0.8.0
-Summary: Tools for generating Python models from JSONSchema definitions.
+Version: 0.9.0
+Summary: Tools for generating Python models from JSON Schema documents.
 Home-page: https://github.com/jacksmith15/statham-schema
 Author: Jack Smith
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/jacksmith15/statham-schema.svg?token=JrMQr8Ynsmu5tphpTQ2p&branch=master)](https://travis-ci.com/jacksmith15/statham-schema)
         # Statham Schema
-        A tool for generating Python objects from [JSONSchema](https://json-schema.org/) documents.
+        A tool for generating Python objects from [JSON Schema](https://json-schema.org/) documents.
         
         This project aims to simplify the experience of integrating with external sources, by providing:
         1. **External validation**: Ensure that incoming data matches what you expect.
         2. **Internal validation**: Ensure your application logic is consistent with the schema. Static type checking (see [mypy](http://mypy-lang.org/)) can do this job for you.
-        3. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
+        3. **Extensibility**: Extend the generated models with properties and methods useful to you.
+        4. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
         
         The models generated by this tool are declared using a JSONSchema DSL. This DSL can easily be used to write schemas by hand, and extend models with extra features.
         
         ## Example DSL Definition
         ```python
         from typing import List
         
@@ -26,20 +27,18 @@
         
         class Choice(Object):
             choice_text: str = Property(String(maxLength=200), required=True)
             votes: int = Property(Integer(default=0))
         
         
         class Poll(Object):
-            question: str = Property(String(maxLength=200), required=True)
+            question: str = Property(String(), required=True)
             choices: List[Choice] = Property(Array(Choice), required=True)
         ```
         
-        Development currently targets compatibility with JSONSchema Draft 6.
-        
         # Requirements
         This package is currently tested for Python 3.6.
         
         # Installation
         This project may be installed using [pip](https://pip.pypa.io/en/stable/):
         ```
         pip install statham-schema
@@ -81,48 +80,38 @@
         
         @format_checker.register("my_format")
         def _check_my_format(value: str) -> bool:
             ...
         ```
         
         # Supported JSONSchema features
-        - [x] Basic types (primitves, array, object)
-        - [x] Composite primitive types
-        - [x] Type validation on generated classes
-        - [x] Validation of `required`
-        - [x] Local references
-        - [x] Type-specific validation (pattern, format, minimum, maximum etc)
-        - [x] Custom string format validation
-        - [x] Remote references
-        - [x] `anyOf`, `oneOf`, `allOf`, `not`
-        - [x] `additionalProperties`
-        - [x] Tuple validation of arrays
-        - [x] `additionalItems` keyword
-        - [x] `minProperties`, `maxProperties` keywords
-        - [x] `patternProperties` keyword
-        - [x] `uniqueItems` keyword
-        - [x] `propertyNames` keyword
-        - [x] `const` keyword
-        - [x] `contains` keyword
-        - [x] `enum` keyword
-        - [x] `dependencies` keyword
-        - [ ] Built-in string format validation #6
-        - [ ] `if`, `then`, `else` keywords
+        This library is tested to support [JSON Schema Draft 6](https://json-schema.org/specification-links.html#draft-6), with the following notable exceptions:
+        - Recursive references are not supported.
+        - Location-independent references are not supported.
+        - Changes of base URI via the `$id` keyword are not detected.
+        
+        Priority order for remaining features is roughly as follows:
+        1. Support for features of more recent drafts.
+        2. Support for the exceptions listed above.
+        3. Support for features of less recent drafts.
+        
+        However, contributions in any of these areas are welcome.
         
         # Development
         1. Clone the repository: `git clone git@github.com:jacksmith15/statham-schema.git && cd statham-schema`
         2. Install the requirements: `pip install -r requirements.txt -r requirements-test.txt`
         3. Run `pre-commit install`
         4. Run the tests: `bash run_test.sh -c -a`
         
         This project uses the following QA tools:
         - [PyTest](https://docs.pytest.org/en/latest/) - for running unit tests.
         - [PyLint](https://www.pylint.org/) - for enforcing code style.
         - [MyPy](http://mypy-lang.org/) - for static type checking.
         - [Travis CI](https://travis-ci.org/) - for continuous integration.
+        - [Black](https://black.readthedocs.io/en/stable/) - for uniform code formatting.
         
         # License
         This project is distributed under the MIT license.
         
         ![statham](https://giant.gfycat.com/GrotesqueNauticalCaracal.gif)
         
 Platform: UNKNOWN
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/array.py` & `statham-schema-0.9.0/statham/dsl/validation/array.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,63 +2,74 @@
 
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.helpers import remove_duplicates
 from statham.dsl.validation.base import Validator, replace_bool
 
 
 class MinItems(Validator):
+    """Validate that arrays have a minimum number of items."""
+
     types = (list,)
     keywords = ("minItems",)
     message = "Must contain at least {minItems} items."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) < self.params["minItems"]:
             raise ValidationError
 
 
 class MaxItems(Validator):
+    """Validate that arrays have a maximum number of items."""
+
     types = (list,)
     keywords = ("maxItems",)
     message = "Must contain fewer than {maxItems} items."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) > self.params["maxItems"]:
             raise ValidationError
 
 
 class AdditionalItems(Validator):
+    """Validate array items not covered by the ``"items"`` keyword.
+
+    Only relevant when using "tuple" style ``"items"``.
+    """
+
     types = (list,)
     keywords = ("items", "additionalItems")
     message = "Must not contain additional items. Accepts: {items}"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if not isinstance(self.params["items"], list):
             return
         if len(value) <= len(self.params["items"]):
             return
         if self.params["additionalItems"]:
             return
         raise ValidationError
 
 
 class UniqueItems(Validator):
+    """Validate that array items are unique."""
+
     types = (list,)
     keywords = ("uniqueItems",)
     message = "Must not contain duplicates."
 
     @classmethod
     def from_element(cls, element) -> Optional["UniqueItems"]:
         validator: Optional[UniqueItems] = cast(
             Optional[UniqueItems], super().from_element(element)
         )
         if validator and validator.params["uniqueItems"] is False:
             return None
         return validator
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         # Once again, Cpython's 1 in [True] nightmare.
         aliased_value = list(map(replace_bool, value))
         length = len(aliased_value)
         try:
             # Try the hashable approach
             if len(set(aliased_value)) == length:
                 return
@@ -66,19 +77,21 @@
             # Long version
             if len(remove_duplicates(aliased_value)) == length:
                 return
         raise ValidationError
 
 
 class Contains(Validator):
+    """Validate that at least one array item matches a schema."""
+
     types = (list,)
     keywords = ("contains",)
     message = "Must contain one element matching {contains}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         for sub_value in value:
             try:
                 _ = self.params["contains"](sub_value)
                 return
             except (TypeError, ValidationError):
                 continue
         raise ValidationError
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/string.py` & `statham-schema-0.9.0/statham/dsl/validation/string.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,48 +2,60 @@
 from typing import Any
 
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.validation.base import Validator
 from statham.dsl.validation.format import format_checker
 
 
-class Format(Validator):
-    types = (str,)
-    keywords = ("format",)
-    message = "Must match format described by '{format}'."
-
-    def validate(self, value: Any):
-        if not format_checker(self.params["format"], value):
-            raise ValidationError
-
-
 class Pattern(Validator):
+    """Validate that string values match a regular expression."""
+
     types = (str,)
     keywords = ("pattern",)
     message = "Must match regex pattern {pattern}."
 
     def error_message(self):
         return self.message.format(pattern=repr(self.params["pattern"]))
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if not re.search(self.params["pattern"], value):
             raise ValidationError
 
 
 class MinLength(Validator):
+    """Validate that string values are over a minimum length."""
+
     types = (str,)
     keywords = ("minLength",)
     message = "Must be at least {minLength} characters long."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) < self.params["minLength"]:
             raise ValidationError
 
 
 class MaxLength(Validator):
+    """Validate that string values are under a maximum length."""
+
     types = (str,)
     keywords = ("maxLength",)
     message = "Must be at most {maxLength} characters long."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) > self.params["maxLength"]:
             raise ValidationError
+
+
+class Format(Validator):
+    """Validate that string values match a named format.
+
+    Additional formats may be registered via
+    :func:`~statham.dsl.validation.format.format_checker`.
+    """
+
+    types = (str,)
+    keywords = ("format",)
+    message = "Must match format described by '{format}'."
+
+    def _validate(self, value: Any):
+        if not format_checker(self.params["format"], value):
+            raise ValidationError
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/numeric.py` & `statham-schema-0.9.0/statham/dsl/validation/numeric.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 from typing import Any
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.validation.base import Validator
 
 
 class Minimum(Validator):
+    """Validate that numeric values conform to a minimum."""
+
     types = (int, float)
     keywords = ("minimum",)
     message = "Must be greater than or equal to {minimum}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value < self.params["minimum"]:
             raise ValidationError
 
 
 class Maximum(Validator):
+    """Validate that numeric values conform to a maximum."""
+
     types = (int, float)
     keywords = ("maximum",)
     message = "Must be less than or equal to {maximum}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value > self.params["maximum"]:
             raise ValidationError
 
 
 class ExclusiveMinimum(Validator):
+    """Validate that numeric values conform to an exclusive minimum."""
+
     types = (int, float)
     keywords = ("exclusiveMinimum",)
     message = "Must be strictly greater than {exclusiveMinimum}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value <= self.params["exclusiveMinimum"]:
             raise ValidationError
 
 
 class ExclusiveMaximum(Validator):
+    """Validate that numeric values conform to an exclusive maximum."""
+
     types = (int, float)
     keywords = ("exclusiveMaximum",)
     message = "Must be strictly less than {exclusiveMaximum}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value >= self.params["exclusiveMaximum"]:
             raise ValidationError
 
 
 class MultipleOf(Validator):
+    """Validate that numeric values are a multiple of a given number."""
+
     types = (int, float)
     keywords = ("multipleOf",)
     message = "Must be a multiple of {multipleOf}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         multiple_of = self.params["multipleOf"]
         if isinstance(multiple_of, float):
             quotient = value / multiple_of
             if int(quotient) != quotient:
                 raise ValidationError
             return
         if value % multiple_of:
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/base.py` & `statham-schema-0.9.0/statham/dsl/validation/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,37 @@
         return False
     return isinstance(value, type_args)
 
 
 class Validator:
     """Base validator type.
 
-    Logic for given validation keywords may be implemented as subclasses.
+    Logic for given validation keywords is implemented in subclasses by
+    overriding class variables and implementing the ``_validate()``
+    method.
     """
 
     types: ClassVar[Optional[Tuple[Type, ...]]] = None
+    """Types on which this validator applies.
+
+    If ``None``, apply to all values.
+    """
+
     message: ClassVar[str] = ""
+    """The error message to display on validation failure.
+
+    Can be tamplated on :attr:`Validator.keywords`.
+    """
+
     keywords: Tuple[str, ...] = tuple()
+    """Keywords which configure this validator.
+
+    These are used to configure the validator based on the
+    :class:`statham.dsl.elements.Element`.
+    """
 
     def __init__(self, *args):
         """Accepts the parameters specified by the `keywords` class variable."""
         if len(self.keywords) != len(args):
             raise TypeError(
                 f"{type(self).__name__}.__init__ takes exactly "
                 f"{len(self.keywords)} ({len(args)} given)"
@@ -54,15 +71,15 @@
             getattr(element, keyword, NotPassed()) for keyword in cls.keywords
         )
         if NotPassed() in params:
             return None
         return cls(*params)
 
     # pylint: disable=no-self-use
-    def validate(self, _value: Any):
+    def _validate(self, _value: Any):
         """Validate a value.
 
         Validation logic should be added by base classes, and raise a
         bare `ValidationError` on a failure. The error message will be
         automatically generated from the `message` class variable for
         consistency.
         """
@@ -73,63 +90,80 @@
         return self.message.format(**self.params)
 
     def __call__(self, value: Any, property_: Any):
         """Apply the validator to a value.
 
         Checks that `value` has correct type for this validator, runs
         validation logic and constructs the error message on failure.
+
+        :param value: The value to validate.
+        :param property_: The enclosing property if present - used for
+            error reporting.
+        :raises: :class:`~statham.dsl.exceptions.ValidationError` if
+            :paramref:`~Validator.__call__.value` fails validation.
         """
         if self.types and not _is_instance(value, self.types):
             return
         try:
-            self.validate(value)
+            self._validate(value)
         except ValidationError:
             raise ValidationError.from_validator(
                 property_, value, self.error_message()
             )
 
 
 class InstanceOf(Validator):
+    """Validate the type of a value."""
+
     message = "Must be of type {type_names}."
 
     def __init__(self, *args):
         super().__init__()
         self.params["types"] = args
         names = (type_.__name__ for type_ in self.params["types"])
         self.params["type_names"] = f"({','.join(names)})"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value == NotPassed() or not self.params["types"]:
             return
         if not _is_instance(value, self.params["types"]):
             raise ValidationError
 
 
 class NoMatch(Validator):
+    """Don't accept any passed value.
+
+    Used exclusively by :class:`~statham.dsl.elements.base.Nothing`.
+    """
+
     message = "Schema does not accept any values."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if value is NotPassed():
             return
         raise ValidationError
 
 
 class Const(Validator):
+    """Validate that passed values match a constant value."""
+
     keywords = ("const",)
     message = "Must match constant value: {const}"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         aliased = replace_bool(value)
         const = replace_bool(self.params["const"])
         if aliased != const:
             raise ValidationError
 
 
 class Enum(Validator):
+    """Validate that passed values are members of an enumeration."""
+
     keywords = ("enum",)
     message = "Must be one of these values: {enum}"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         aliased = replace_bool(value)
         enum = list(map(replace_bool, self.params["enum"]))
         if aliased not in enum:
             raise ValidationError
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/format.py` & `statham-schema-0.9.0/statham/dsl/validation/format.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,25 @@
                 RuntimeWarning,
             )
             return True
         return self._callable_register[format_string](value)
 
 
 format_checker: _FormatString = _FormatString("format_checker")
+"""Extensible implementation of the ``"format"`` keyword.
+
+Validators for new formats may be registered as follows:
+
+.. code:: python
+
+    @format_checker.register("my_format")
+    def _validate_my_format(value: str) -> bool:
+        # Return True if `value` matches `my_format`.
+        ...
+"""
 
 
 @format_checker.register("uuid")
 def _is_uuid(value: str) -> bool:
     try:
         UUID(value)
     except (ValueError, TypeError):
```

### Comparing `statham-schema-0.8.0/statham/dsl/validation/object.py` & `statham-schema-0.9.0/statham/dsl/validation/object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 from typing import Any
 
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.validation.base import Validator
 
 
 class Required(Validator):
+    """Validate that object values contain all required properties."""
+
     types = (dict,)
     keywords = ("required",)
     message = "Must contain all required fields: {required}"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if set(self.params["required"]) - set(value):
             raise ValidationError
 
 
 class AdditionalProperties(Validator):
+    """Validate that prohibited properties are not included."""
+
     types = (dict,)
     keywords = ("__properties__",)
     message = "Must not contain unspecified properties. Accepts: {properties}"
 
     def error_message(self):
         return self.message.format(
             properties=set(self.params["__properties__"])
         )
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if self.params["__properties__"].additional:
             return
         bad_properties = {
             key for key in value if key not in self.params["__properties__"]
         }
         if bad_properties:
             raise ValidationError
 
 
 class MinProperties(Validator):
+    """Validate that object values contain a minimum number of properties."""
+
     types = (dict,)
     keywords = ("minProperties",)
     message = "Must contain at least {minProperties} properties."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) < self.params["minProperties"]:
             raise ValidationError
 
 
 class MaxProperties(Validator):
+    """Validate that object values contain a maximum number of properties."""
+
     types = (dict,)
     keywords = ("maxProperties",)
     message = "Must contain at most {maxProperties} properties."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         if len(value) > self.params["maxProperties"]:
             raise ValidationError
 
 
 class PropertyNames(Validator):
+    """Validate that property names conform to a schema."""
+
     types = (dict,)
     keywords = ("propertyNames",)
     message = "Property names must match schema {propertyNames}"
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         for prop_name in value:
             try:
                 self.params["propertyNames"](prop_name)
             except (ValidationError, TypeError):
                 raise ValidationError
 
 
 class Dependencies(Validator):
     types = (dict,)
     keywords = ("dependencies",)
     message = "Must match defined dependencies: {dependencies}."
 
-    def validate(self, value: Any):
+    def _validate(self, value: Any):
         for key, dep in self.params["dependencies"].items():
             if key not in value:
                 continue
             if isinstance(dep, list):
-                Required(dep).validate(value)
+                # pylint: disable=protected-access
+                Required(dep)._validate(value)
             else:
                 self.validate_schema_dependency(dep, value)
 
     @staticmethod
     def validate_schema_dependency(dependency, value):
         try:
             _ = dependency(value)
```

### Comparing `statham-schema-0.8.0/statham/dsl/helpers.py` & `statham-schema-0.9.0/statham/dsl/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     return _decorator
 
 
 T = TypeVar("T")
 
 
 def split_dict(
-    keys: Container[T]
+    keys: Container[T],
 ) -> Callable[[Dict[T, Any]], Tuple[Dict[T, Any], Dict[T, Any]]]:
     """Split a dictionary on matching and non-matching keys."""
 
     def _split(dictionary: Dict[T, Any]) -> Tuple[Dict[T, Any], Dict[T, Any]]:
         match = {key: value for key, value in dictionary.items() if key in keys}
         complement = {
             key: value for key, value in dictionary.items() if key not in keys
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/composition.py` & `statham-schema-0.9.0/statham/dsl/elements/composition.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 from statham.dsl.constants import NotPassed
 from statham.dsl.elements.base import Element
 from statham.dsl.helpers import remove_duplicates
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.property import _Property
 
-# TODO: if, then, else
 
 # This is a type annotation.
 Mode = Literal["anyOf", "oneOf", "allOf"]  # pylint: disable=invalid-name
 T = TypeVar("T")
 
 
 class Not(Element[T]):
-    """JSONSchema "not" element.
+    """JSON Schema ``"not"`` element.
 
     Element fails to validate if enclosed schema validates.
+
+    :param element: The enclosed :class:`~statham.dsl.elements.Element`.
+    :param default: Inherited from :class:`~statham.dsl.elements.Element`.
     """
 
-    def __init__(self, element: Element, default: Any = NotPassed()):
+    def __init__(self, element: Element, *, default: Any = NotPassed()):
         self.element = element
         super().__init__(default=default)
 
     def construct(self, value: Any, property_: _Property):
         try:
             _ = self.element(value, property_)
         except (TypeError, ValidationError):
@@ -34,14 +36,18 @@
         )
 
 
 class CompositionElement(Element):
     """Composition Base Element.
 
     The "oneOf", "anyOf" and "allOf" elements share the same interface.
+
+    :param elements: The composed :class:`~statham.dsl.elements.Element`
+        objects.
+    :param default: Inherited from :class:`~statham.dsl.elements.Element`.
     """
 
     mode: Mode
 
     def __init__(self, *elements: Element, default: Any = NotPassed()):
         super().__init__()
         self.elements = list(elements)
@@ -64,27 +70,48 @@
     def construct(self, value: Any, property_: _Property):
         if not getattr(self, "mode", None):
             raise NotImplementedError
         return _attempt_schemas(self.elements, value, property_, mode=self.mode)
 
 
 class AnyOf(CompositionElement):
-    """Must match at least one of the provided schemas."""
+    """JSON Schema ``"anyOf"`` element.
+
+    Must match at least one of the provided schemas.
+
+    :param elements: The composed :class:`~statham.dsl.elements.Element`
+        objects.
+    :param default: Inherited from :class:`~statham.dsl.elements.Element`.
+    """
 
     mode: Mode = "anyOf"
 
 
 class OneOf(CompositionElement):
-    """Must match exactly one of the provided schemas.."""
+    """JSON Schema ``"oneOf"`` element.
+
+    Must match exactly one of the provided schemas.
+
+    :param elements: The composed :class:`~statham.dsl.elements.Element`
+        objects.
+    :param default: Inherited from :class:`~statham.dsl.elements.Element`.
+    """
 
     mode: Mode = "oneOf"
 
 
 class AllOf(CompositionElement):
-    """Must match all provided schemas."""
+    """JSON Schema ``"allOf"`` element.
+
+    Must match all provided schemas.
+
+    :param elements: The composed :class:`~statham.dsl.elements.Element`
+        objects.
+    :param default: Inherited from :class:`~statham.dsl.elements.Element`.
+    """
 
     mode: Mode = "allOf"
 
     @property
     def annotation(self):
         """Get type annotation for element.
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/null.py` & `statham-schema-0.9.0/statham/dsl/elements/null.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from statham.dsl.elements.base import Element
 from statham.dsl.constants import Maybe, NotPassed
 from statham.dsl.validation import InstanceOf
 
 
 class Null(Element[None]):
-    """JSONSchema null element."""
+    """JSON Schema ``"null"`` element."""
 
     def __init__(
         self,
         *,
         default: Maybe[None] = NotPassed(),
         const: Maybe[Any] = NotPassed(),
         enum: Maybe[List[Any]] = NotPassed(),
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/array.py` & `statham-schema-0.9.0/statham/dsl/elements/array.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from statham.dsl.validation import InstanceOf
 
 
 Item = TypeVar("Item")
 
 
 # pylint: disable=too-many-instance-attributes
-class Array(Element[List[Item]]):
-    """JSONSchema array element.
+class Array(Element[List[Item]]):  # pylint: disable=missing-param-doc
+    """JSON Schema ``"array"`` element.
 
-    Requires schema element for "items" keyword as first positional
-    argument. Supported validation keywords provided via keyword arguments.
+    :param items:
+        As in :class:`statham.dsl.elements.Element`, but as a required
+        positional argument.
     """
 
     items: Union[Element[Item], List[Element]]
 
     def __init__(
         self,
         items: Union[Element[Item], List[Element]],
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/items.py` & `statham-schema-0.9.0/statham/dsl/elements/items.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from statham.dsl.constants import NotPassed
 from statham.dsl.elements.base import Element, Nothing
 
 
 class Items:
+    """Interface for retrieving relevant schemas given an array index.
+
+    Used internally by :class:`~statham.dsl.elements.Element`.
+    """
+
     def __init__(self, items, additional=True):
         self.items = Element() if isinstance(items, NotPassed) else items
         if isinstance(additional, bool):
             self.additional = {True: Element(), False: Nothing()}[additional]
         else:
             self.additional = additional
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/string.py` & `statham-schema-0.9.0/statham/dsl/elements/string.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,23 @@
 
 from statham.dsl.elements.base import Element
 from statham.dsl.constants import Maybe, NotPassed
 from statham.dsl.validation import InstanceOf
 
 
 class String(Element[str]):
-    """JSONSchema string element.
-
-    Provides supported validation settings via keyword arguments.
-    """
+    """JSON Schema ``"string"`` element."""
 
     def __init__(
         self,
         *,
         default: Maybe[str] = NotPassed(),
         const: Maybe[Any] = NotPassed(),
         enum: Maybe[List[Any]] = NotPassed(),
-        # Bad name to match JSONSchema keywords.
+        # Bad name to match JSON Schema keywords.
         # pylint: disable=redefined-builtin
         format: Maybe[str] = NotPassed(),
         # pylint: enable=redefined-builtin
         pattern: Maybe[str] = NotPassed(),
         minLength: Maybe[int] = NotPassed(),
         maxLength: Maybe[int] = NotPassed(),
     ):
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/numeric.py` & `statham-schema-0.9.0/statham/dsl/elements/numeric.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 T = TypeVar("T", int, float)
 
 Numeric = Union[int, float]
 
 
 # pylint: disable=too-many-instance-attributes
 class NumericElement(Element[T]):
-    """JSONSchema base numeric element.
-
-    Provides supported validation settings via keyword arguments.
-    """
+    """JSON Schema base numeric element."""
 
     def __init__(
         self,
         *,
         default: Maybe[T] = NotPassed(),
         const: Maybe[Any] = NotPassed(),
         enum: Maybe[List[Any]] = NotPassed(),
@@ -36,28 +33,28 @@
         self.maximum = maximum
         self.exclusiveMinimum = exclusiveMinimum
         self.exclusiveMaximum = exclusiveMaximum
         self.multipleOf = multipleOf
 
 
 class Integer(NumericElement[int]):
-    """JSONSchema integer element.
+    """JSON Schema ``"integer"`` element.
 
-    Provides supported validation settings via keyword arguments.
+    Accepts only python `int`.
     """
 
     @property
     def type_validator(self):
         return InstanceOf(int)
 
 
 class Number(NumericElement[float]):
-    """JSONSchema number element.
+    """JSON Schema ``"number"`` element.
 
-    Provides supported validation settings via keyword arguments.
+    Accepts python ``int`` or ``float``.
     """
 
     def construct(self, value, _property):  # pylint: disable=no-self-use
         return float(value)
 
     @property
     def type_validator(self):
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/meta.py` & `statham-schema-0.9.0/statham/dsl/elements/meta.py`

 * *Files identical despite different names*

### Comparing `statham-schema-0.8.0/statham/dsl/elements/boolean.py` & `statham-schema-0.9.0/statham/dsl/elements/boolean.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from statham.dsl.elements.base import Element
 from statham.dsl.constants import Maybe, NotPassed
 from statham.dsl.validation import InstanceOf
 
 
 class Boolean(Element[bool]):
-    """JSONSchema boolean element."""
+    """JSON Schema ``"boolean"`` element."""
 
     def __init__(
         self,
         *,
         default: Maybe[bool] = NotPassed(),
         const: Maybe[Any] = NotPassed(),
         enum: Maybe[List[Any]] = NotPassed(),
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/object.py` & `statham-schema-0.9.0/statham/dsl/elements/object.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,31 +4,38 @@
 from statham.dsl.elements.meta import ObjectMeta
 from statham.dsl.exceptions import ValidationError
 from statham.dsl.property import _Property
 from statham.dsl.constants import NotPassed
 
 
 class Object(metaclass=ObjectMeta):
-    """Base model for JSONSchema objects.
+    """Base model for JSON Schema ``"object"`` elements.
 
-    New object schemas are defined by implementing subclasses of Object.
+    ``"object"`` schemas are defined by declaring subclasses of
+    :class:`Object`. Properties are declared as class attributes, and
+    other keywords are set as class arguments.
 
     For example:
-    ```python
-    from statham.dsl.elements import Object, String
-    from statham.dsl.property import Property
 
-    class Poll(Object):
+    .. code:: python
 
-        questions: List[str] = Property(String(), required=True)
+        from statham.dsl.elements import Object, String
+        from statham.dsl.property import Property
+
+        class Poll(Object, additionalProperties=False):
+
+            questions: List[str] = Property(String(), required=True)
+
+        poll = Poll({"questions": ["What's up?"]})
 
-    poll = Poll({"questions": ["What's up?"]})
-    ```
     """
 
+    # TODO: Add an inline constructor
+    # Object.inline("MyObject", properties={}, ...)
+
     properties: ClassVar[Dict[str, _Property]]
     default: ClassVar[Any]
     additionalProperties: ClassVar[Union[Element, bool]]
 
     def __new__(
         cls, value: Any = NotPassed(), property_: _Property = UNBOUND_PROPERTY
     ):
```

### Comparing `statham-schema-0.8.0/statham/dsl/elements/properties.py` & `statham-schema-0.9.0/statham/dsl/elements/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from statham.dsl.constants import NotPassed
 from statham.dsl.elements.base import Element, Nothing
 from statham.dsl.elements.composition import AllOf
 from statham.dsl.property import _Property as Property
 
 
 class Properties:
+    """Interface for retrieving relevant schemas given a property name.
+
+    Used internally by :class:`~statham.dsl.elements.Element`.
+    """
+
     def __init__(self, element, props, pattern=None, additional=True):
         self.element = element
         self.props = props or {}
         self.pattern = PatternDict(pattern or {})
         for name, prop in self.props.items():
             prop.bind_name(name)
             prop.bind_class(self.element)
```

### Comparing `statham-schema-0.8.0/statham/dsl/constants.py` & `statham-schema-0.9.0/statham/dsl/constants.py`

 * *Files identical despite different names*

### Comparing `statham-schema-0.8.0/statham/dsl/parser.py` & `statham-schema-0.9.0/statham/dsl/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# pylint: disable=too-many-lines
+"""Parsing tools to convert JSON Schema dictionaries to DSL Element instances.
+
+Some JSON Schema documents will be converted to an equivalent but structurally
+differing representation. In particular, those that combine composition
+keywords or use multiple types will be recomposed using ``"allOf"`` and
+``"anyOf"`` respectively. See :mod:`statham.dsl.elements.composition` for more
+details.
+"""
 from collections import defaultdict
 from functools import partial
 import inspect
 from itertools import chain
 import operator as op
 import re
 import string
@@ -45,15 +54,15 @@
     "integer": Integer,
     "null": Null,
     "number": Number,
     "string": String,
 }
 
 
-class ParseState:
+class _ParseState:
     """Recusive state.
 
     Used to de-duplicate models which are traversed multiple times, and to
     rename distinct models with the same name.
     """
 
     def __init__(self):
@@ -74,113 +83,135 @@
         if count:
             object_type.__name__ = name + f"_{count}"
         self.seen[name].append(object_type)
         return object_type
 
 
 def parse(schema: Dict[str, Any]) -> List[Element]:
-    """Parse a JSONSchema document to DSL Element format.
+    """Parse a JSON Schema document to DSL Element format.
+
+    Assumes references are already resolved, and that any ``"object"`` schemas
+    or sub-schemas contain either a ``"title"`` annotation or an
+    ``"_x_autotitle"`` annotation. See
+    `json-ref-dict <https://pypi.org/project/json-ref-dict/0.6.0/>`_ for
+    reference resolution and annotation tools.
 
-    Checks the top-level and definitions keyword to collect elements.
+    :return: A list of DSL elements, starting with the top level element,
+        followed by each element in the top-level schema ``"definitions"``.
     """
-    state = ParseState()
+    state = _ParseState()
     return [parse_element(schema, state)] + [
         parse_element(definition, state)
         for definition in schema.get("definitions", {}).values()
         if isinstance(definition, (dict, bool, Element))
     ]
 
 
 @reraise(
     RecursionError,
-    SchemaParseError,
+    FeatureNotImplementedError,
     "Could not parse cyclical dependencies of this schema.",
 )
 def parse_element(
-    schema: Union[bool, Dict[str, Any]], state: ParseState = None
+    schema: Union[bool, Dict[str, Any]], state: _ParseState = None
 ) -> Element:
-    """Parse a JSONSchema element to a DSL Element object."""
+    """Parse a single JSON Schema element to a DSL Element object.
+
+    Called by :func:`parse` when parsing entire documents.
+
+    >>> parse_element({"type": "string", "minLength": 3})
+    String(minLength=3)
+
+    :raises: :exc:`~statham.dsl.exceptions.FeatureNotImplementedError` if
+        recursive cycles are detected.
+    :raises: :exc:`statham.dsl.exceptions.SchemaParseError` if problems are
+        found in the provided schema.
+    :return: A single :class:`~statham.dsl.elements.Element` object equivalent
+        to the schema described by :paramref:`parse_element.schema`.
+    """
     if isinstance(schema, bool):
         return Element() if schema else Nothing()
-    state = state or ParseState()
+    state = state or _ParseState()
     if isinstance(schema, Element):
         return schema
     if set(schema) & UNSUPPORTED_SCHEMA_KEYWORDS:
         raise FeatureNotImplementedError.unsupported_keywords(
             set(schema) & UNSUPPORTED_SCHEMA_KEYWORDS
         )
     for literal_key in ("default", "const", "enum"):
         if literal_key in schema:
-            schema[literal_key] = parse_literal(schema[literal_key])
+            schema[literal_key] = _parse_literal(schema[literal_key])
     for keyword, parser in (
-        ("properties", parse_properties),
-        ("items", parse_items),
-        ("patternProperties", parse_pattern_properties),
-        ("propertyNames", parse_property_names),
-        ("contains", parse_contains),
-        ("dependencies", parse_dependencies),
+        ("properties", _parse_properties),
+        ("items", _parse_items),
+        ("patternProperties", _parse_pattern_properties),
+        ("propertyNames", _parse_property_names),
+        ("contains", _parse_contains),
+        ("dependencies", _parse_dependencies),
     ):
         if keyword in schema:
             schema[keyword] = parser(schema, state)  # type: ignore
-    schema["additionalProperties"] = parse_additional_properties(schema, state)
-    schema["additionalItems"] = parse_additional_items(schema, state)
+    schema["additionalProperties"] = _parse_additional_properties(schema, state)
+    schema["additionalItems"] = _parse_additional_items(schema, state)
     if set(COMPOSITION_KEYWORDS) & set(schema):
-        return parse_composition(schema, state)
+        return _parse_composition(schema, state)
     if "type" not in schema:
-        return Element(**keyword_filter(Element)(schema))
-    return parse_typed(schema["type"], schema, state)
+        return Element(**_keyword_filter(Element)(schema))
+    return _parse_typed(schema["type"], schema, state)
 
 
-def parse_literal(literal: Any) -> Any:
+def _parse_literal(literal: Any) -> Any:
     """Parse literal values from schema.
 
     Keywords like `const`, `enum` and `default` refer to non-schema values.
     Annotations should be removed to prevent side effects.
     """
     if not isinstance(literal, (dict, list)):
         return literal
     if isinstance(literal, list):
-        return [parse_literal(val) for val in literal]
+        return [_parse_literal(val) for val in literal]
     return {
-        key: parse_literal(val)
+        key: _parse_literal(val)
         for key, val in literal.items()
         if key != "_x_autotitle"
     }
 
 
-def parse_contains(schema: Dict[str, Any], state: ParseState = None) -> Element:
+def _parse_contains(
+    schema: Dict[str, Any], state: _ParseState = None
+) -> Element:
     """Parse schema contains keyword."""
-    state = state or ParseState()
+    state = state or _ParseState()
     return parse_element(schema["contains"], state)
 
 
-def parse_composition(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_composition(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Element:
     """Parse a schema with composition keywords.
 
     Handles multiple composition keywords by wrapping them in an AllOf
     element. Similarly, non-keyword elements are parsed as usual and
     included in an allOf element.
 
     For example:
     ```python
     schema = {
         "type": "integer",
         "oneOf": [{"minimum": 3}, {"maximum": 5}],
         "anyOf": [{"multipleOf": 2}, {"multipleOf": 3}],
     }
-    parse_composition(schema) == AllOf(
+    _parse_composition(schema) == AllOf(
         Integer(),
         OneOf(Element(minimum=3), Element(maximum=5)),
         AnyOf(Element(multipleOf=2), Element(multipleOf=3)),
     )
     ```
     """
-    state = state or ParseState()
+    state = state or _ParseState()
     composition, other = split_dict(set(COMPOSITION_KEYWORDS) | {"default"})(
         schema
     )
     base_element = parse_element(other, state)
     for key in set(COMPOSITION_KEYWORDS) - {"not"}:
         composition[key] = [
             parse_element(sub_schema, state)
@@ -197,93 +228,89 @@
     default = schema.get("default", NotPassed())
     if isinstance(element, ObjectMeta):
         return AllOf(element, default=default)
     element.default = default or element.default
     return element
 
 
-def parse_typed(
-    type_value: Any, schema: Dict[str, Any], state: ParseState = None
+def _parse_typed(
+    type_value: Any, schema: Dict[str, Any], state: _ParseState = None
 ) -> Element:
-    """Parse a typed schema with no composition keywords.
-
-    :raises KeyError: if no "type" key is present.
-    :raises SchemaParseError: if value at "type" is not a `str` or `list`.
-    """
-    state = state or ParseState()
+    """Parse a typed schema with no composition keywords."""
+    state = state or _ParseState()
     if not isinstance(type_value, (str, list)):
         raise SchemaParseError.invalid_type(type_value)
     if isinstance(type_value, list):
-        return parse_multi_typed(type_value, schema, state)
+        return _parse_multi_typed(type_value, schema, state)
     if schema["type"] == "object":
-        return parse_object(schema, state)
+        return _parse_object(schema, state)
     if schema["type"] == "array":
-        return parse_array(schema, state)
+        return _parse_array(schema, state)
     element_type = _TYPE_MAPPING[type_value]
-    sub_schema = keyword_filter(element_type)(schema)
+    sub_schema = _keyword_filter(element_type)(schema)
     return element_type(**sub_schema)
 
 
-def parse_multi_typed(
-    type_list: List[str], schema: Dict[str, Any], state: ParseState = None
+def _parse_multi_typed(
+    type_list: List[str], schema: Dict[str, Any], state: _ParseState = None
 ) -> CompositionElement:
     """Parse a schema with multiple type values.
 
     Converts schema to an equivalent representation using "anyOf". For example:
     ```python
     {"type": ["string", "integer"]}
     ```
     becomes
     ```
     {"anyOf": [{"type": "string"}, {"type": "integer"}]}
     ```
     """
-    state = state or ParseState()
+    state = state or _ParseState()
     default = schema.get("default", NotPassed())
     schema = {key: val for key, val in schema.items() if key != "default"}
     if len(type_list) == 1:
         return parse_element({**schema, "type": type_list[0]}, state)
     return AnyOf(
         *(
             parse_element({**schema, "type": type_value}, state)
             for type_value in type_list
         ),
         default=default,
     )
 
 
-def parse_object(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_object(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> ObjectMeta:
     """Parse an object schema element to an `Object` subclass.
 
     The name of the generated class is derived from the following keys
     in precedence order:
     - "title"
     - "_x_autotitle"
 
     Also requires that "properties" and "additionalProperties" values have
     already been parsed.
 
     :raises SchemaParseError: if keys exist from which to derive the class
         title.
     """
-    state = state or ParseState()
+    state = state or _ParseState()
     title = schema.get("title", schema.get("_x_autotitle"))
     if not title:
         raise SchemaParseError.missing_title(schema)
     title = _title_format(title)
     properties = schema.get("properties", {})
     properties.update(
         {
-            parse_attribute_name(key): _Property(
+            _parse_attribute_name(key): _Property(
                 Element(), required=True, source=key
             )
             for key in schema.get("required", [])
-            if parse_attribute_name(key) not in properties
+            if _parse_attribute_name(key) not in properties
         }
     )
     class_dict = ObjectClassDict()
     for key, value in properties.items():
         class_dict[key] = value
     cls_args = dict(additionalProperties=schema["additionalProperties"])
     for key in [
@@ -298,41 +325,41 @@
     ]:
         if key in schema:
             cls_args[key] = schema[key]
     object_type = ObjectMeta(title, (Object,), class_dict, **cls_args)
     return state.dedupe(object_type)
 
 
-def parse_properties(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_properties(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Dict[str, _Property]:
     """Parse properties from a schema element."""
-    state = state or ParseState()
+    state = state or _ParseState()
     required = set(schema.get("required", []))
     properties = schema.get("properties", {})
     return {
         **{
-            parse_attribute_name(key): _Property(
+            _parse_attribute_name(key): _Property(
                 parse_element(value, state),
                 required=key in required,
                 source=key,
             )
             for key, value in properties.items()
             # Ignore malformed values.
             if isinstance(value, (dict, bool))
         },
         **{
-            parse_attribute_name(key): prop
+            _parse_attribute_name(key): prop
             for key, prop in properties.items()
             if isinstance(prop, _Property)
         },
     }
 
 
-def parse_attribute_name(name: str) -> str:
+def _parse_attribute_name(name: str) -> str:
     """Convert attibute name to valid python attribute.
 
     Attempts to replace special characters with their unicode names.
     """
 
     def _char_map(idx: int, char: str) -> str:
         if char.isalnum() or char in ("_", "-", " "):
@@ -347,109 +374,109 @@
         return label
 
     chars = map(expand(_char_map), enumerate(name))
     name = "".join(chars).replace(" ", "_").replace("-", "_")
     if not name:
         return "blank"
     first_chars = set(string.ascii_letters) | {"_"}
-    return (
-        name
-        if name not in RESERVED_PROPERTIES and name[0] in first_chars
-        else f"_{name}"
-    )
+    if name[0] not in first_chars:
+        name = f"_{name}"
+    if name in RESERVED_PROPERTIES:
+        name = f"{name}_"
+    return name
 
 
-def parse_pattern_properties(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_pattern_properties(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Dict[str, Element]:
     """Parse schema patternProperties keyword."""
-    state = state or ParseState()
+    state = state or _ParseState()
     return {
         **{
             key: parse_element(value, state)
             for key, value in schema["patternProperties"].items()
             if isinstance(value, (dict, bool))
         },
         **{
             key: value
             for key, value in schema["patternProperties"].items()
             if isinstance(value, Element)
         },
     }
 
 
-def parse_property_names(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_property_names(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Element:
     """Parse schema propertyNames keyword."""
-    state = state or ParseState()
+    state = state or _ParseState()
     return parse_element(schema["propertyNames"], state)
 
 
-def parse_additional(
-    key: str, schema: Dict[str, Any], state: ParseState = None
+def _parse_additional(
+    key: str, schema: Dict[str, Any], state: _ParseState = None
 ) -> Union[Element, bool]:
     """Parse additional items or properties.
 
     Booleans are retained for these values, as they are more semantically
     meaningful than in general schemas.
     """
-    state = state or ParseState()
+    state = state or _ParseState()
     additional = schema.get(key, True)
     if isinstance(additional, bool):
         return additional
     return parse_element(additional, state)
 
 
-def parse_additional_properties(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_additional_properties(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Union[Element, bool]:
     """Parse additionalProperties from a schema element.
 
     If key is not present, defaults to `True`.
     """
-    return parse_additional("additionalProperties", schema, state)
+    return _parse_additional("additionalProperties", schema, state)
 
 
-def parse_additional_items(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_additional_items(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Union[Element, bool]:
     """Parse additionalProperties from a schema element.
 
     If key is not present, defaults to `True`.
     """
-    return parse_additional("additionalItems", schema, state)
+    return _parse_additional("additionalItems", schema, state)
 
 
-def parse_array(schema: Dict[str, Any], state: ParseState = None) -> Array:
+def _parse_array(schema: Dict[str, Any], state: _ParseState = None) -> Array:
     """Parse an array schema element."""
-    state = state or ParseState()
+    state = state or _ParseState()
     items = schema.get("items", Element())
-    return Array(**{**keyword_filter(Array)(schema), "items": items})
+    return Array(**{**_keyword_filter(Array)(schema), "items": items})
 
 
-def parse_items(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_items(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Union[Element, List[Element]]:
     """Parse array items keyword to DSL Element.
 
     If not present, defaults to `Element()`.
     """
-    state = state or ParseState()
+    state = state or _ParseState()
     items = schema.get("items", {})
     if isinstance(items, list):
         return [parse_element(item, state) for item in items]
     return parse_element(items, state)
 
 
-def parse_dependencies(
-    schema: Dict[str, Any], state: ParseState = None
+def _parse_dependencies(
+    schema: Dict[str, Any], state: _ParseState = None
 ) -> Dict[str, Union[List[str], Element]]:
     """Parse dependencies keyword from schema."""
-    state = state or ParseState()
+    state = state or _ParseState()
     return {
         **{
             key: value
             for key, value in schema["dependencies"].items()
             if isinstance(value, (list, Element))
         },
         **{
@@ -472,15 +499,15 @@
     if not elements:
         return Element()
     if len(elements) == 1:
         return elements[0]
     return element_type(*elements)
 
 
-def keyword_filter(type_: Type) -> Callable[[Dict[str, Any]], Dict[str, Any]]:
+def _keyword_filter(type_: Type) -> Callable[[Dict[str, Any]], Dict[str, Any]]:
     """Create a filter to pull out only relevant keywords for a given type."""
     params = inspect.signature(type_.__init__).parameters.values()
     args = {param.name for param in params}
 
     def _filter(schema: Dict[str, Any]) -> Dict[str, Any]:
         return {key: value for key, value in schema.items() if key in args}
```

### Comparing `statham-schema-0.8.0/statham/dsl/exceptions.py` & `statham-schema-0.9.0/statham/dsl/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from typing import Dict
 
 from statham.dsl.constants import JSONElement
 
 
 class StathamError(Exception):
-    """Base exception"""
+    """Base exception for errors relating to :mod:`statham`."""
 
 
 class SchemaDefinitionError(StathamError):
-    """Failure when declaring schemas using DSL."""
+    """Raised when invalid schemas are declared in the DSL."""
 
     @classmethod
     def reserved_attribute(cls, attribute_name: str) -> "SchemaDefinitionError":
-        # TODO: Default to underscore after not before.
         return cls(
             f"May not use reserved attribute `{attribute_name}` as a property "
             "attribute name. Instead use "
-            f"`_{attribute_name} = Property(<element>, "
+            f"`{attribute_name}_ = Property(<element>, "
             f"source='{attribute_name}'`"
         )
 
 
 class ValidationError(StathamError):
-    """Validation failure in generated models."""
+    """Raised when JSON Schema validation fails for input data."""
 
     @classmethod
     def from_validator(cls, property_, value, message) -> "ValidationError":
-        return cls(
-            f"Failed validating `{repr(property_.parent)}."
-            f"{property_.name} = {repr(value)}`. {message}"
+        value_string = (
+            f"{repr(property_.parent)}{property_.name} = {repr(value)}`"
+            if property_.name != "<unbound>"
+            else repr(value)
         )
+        return cls(f"Failed validating `{value_string}`. {message}")
 
     @classmethod
     def combine(
         cls, property_, value, exceptions, message
     ) -> "ValidationError":
         base_message = str(cls.from_validator(property_, value, ""))
         error_breakdown = ", ".join(str(exc) for exc in exceptions)
@@ -48,15 +49,15 @@
             "Matches multiple possible models. Must only match one.\n"
             f"Data: {data}\n"
             f"Models: {matching_models}"
         )
 
 
 class SchemaParseError(StathamError):
-    """Failure during parsing of provided JSON Schema input."""
+    """Raised when parsing JSON Schema documents to DSL objects."""
 
     @classmethod
     def missing_title(
         cls, schema: Dict[str, JSONElement]
     ) -> "SchemaParseError":
         return cls(
             "No title defined in schema. Use "
@@ -72,15 +73,16 @@
         )
 
     @classmethod
     def invalid_type(cls, value):
         return cls(f"Got invalid type keyword: {value}.")
 
 
+# pylint: disable=line-too-long
 class FeatureNotImplementedError(SchemaParseError):
-    """Functionality not yet implemented."""
+    """Raised when parsing valid JSON Schema features currently unsupported by the DSL."""
 
     @classmethod
     def unsupported_keywords(cls, keywords) -> "FeatureNotImplementedError":
         return cls(
             f"The following provided keywords are not supported: {keywords}"
         )
```

### Comparing `statham-schema-0.8.0/statham/dsl/property.py` & `statham-schema-0.9.0/statham/dsl/property.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,26 +90,27 @@
 
 
 # Behaves as a wrapper for the `_Property` class.
 # pylint: disable=invalid-name
 def Property(element: "Element", *, required: bool = False, source: str = None):
     """Descriptor for adding a property when declaring an object schema model.
 
-    Return value is typed to inform instance-level interface. See type stubs of
-    this module for more detail.
+    Return value is typed to inform instance-level interface (see type stubs).
 
-    :param element: The JSONSchema Element object accepted by this property.
+    :param element: The JSON Schema Element object accepted by this property.
     :param required: Whether this property is required. If false, then this
         field may be omitted when data is passed to the outer object's
         constructor.
     :param source: The source name of this property. Only necessary if it must
-        differ from that of the attribute, for example when the property name
-        conflicts with a reserved keyword. For example, to express a property
-        called `class`, one could do the following:
-        ```python
-        class MyObject(Object):
+        differ from that of the attribute.
+
+    To hand property name conflicts, use the :paramref:`Property.source`
+    option. For example, to express a property called `class`, one could
+    do the following:
 
+    .. code:: python
+
+        class MyObject(Object):
             # Property called class
-            _class: str = Property(String(), source="class")
-        ```
+            class_: str = Property(String(), source="class")
     """
     return _Property(element, required=required, source=source)
```

### Comparing `statham-schema-0.8.0/statham/__main__.py` & `statham-schema-0.9.0/statham/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,54 +4,51 @@
 from os import path
 from typing import Iterator, TextIO, Tuple
 from sys import argv, stdout
 
 from json_ref_dict import materialize, RefDict
 
 from statham.dsl.parser import parse
-from statham.serializer import serialize_python
+from statham.serializers import serialize_python
 from statham.titles import title_labeller
 
 
-# TODO: Write tests for references via keys containing /.
-
-
 LOGGER = getLogger(__name__)
 LOGGER.setLevel(INFO)
 
 
 def parse_input_arg(input_arg: str) -> str:
-    """Parse input URI as a valid JSONSchema ref.
+    """Parse input URI as a valid JSON Schema ref.
 
     This tool accepts bare base URIs, without the JSON Pointer,
     so these should be converted to a root pointer.
     """
     if "#" not in input_arg:
         return input_arg + "#/"
     return input_arg
 
 
 @contextmanager
 def parse_args(args) -> Iterator[Tuple[str, TextIO]]:
     """Parse arguments, abstracting IO in a context manager."""
 
     parser = ArgumentParser(
-        description="Generate statham DSL models from JSONSchema files.",
+        description="Generate statham DSL models from JSON Schema files.",
         formatter_class=RawTextHelpFormatter,
         add_help=False,
     )
     required = parser.add_argument_group("Required arguments")
     required.add_argument(
         "--input",
         type=str,
         required=True,
         help="""Specify the path to the JSON Schema to be generated.
 
 If the target schema is not at the root of a document, specify the
-JSON Pointer in the same format as a JSONSchema `$ref`, e.g.
+JSON Pointer in the same format as a JSON Schema `$ref`, e.g.
 `--input path/to/document.json#/definitions/schema`
 
 """,
     )
     optional = parser.add_argument_group("Optional arguments")
     optional.add_argument(
         "--output",
@@ -83,23 +80,18 @@
             yield input_arg, file
         return
     yield input_arg, stdout
     return
 
 
 def main(input_uri: str) -> str:
-    """Get the schema, and then return the generated python module.
-
-    Example:
-    ```
-    main("https://json-schema.org/draft-04/schema#/")
-    ```
+    """Get a schema from a URI, and then return the generated python module.
 
-    :param input_uri: This must follow the conventions of a JSONSchema
-        '$ref' attribute.
+    :param input_uri: URI of the target schema. This must follow the conventions
+        of a JSON Schema ``"$ref"`` attribute.
     :return: Python module contents for generated models, as a string.
     """
     schema = materialize(
         RefDict.from_uri(input_uri), context_labeller=title_labeller()
     )
     return serialize_python(*parse(schema))
```

### Comparing `statham-schema-0.8.0/statham/titles.py` & `statham-schema-0.9.0/statham/titles.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from json_ref_dict import URI
 
 from statham.dsl.constants import COMPOSITION_KEYWORDS
 
 
 def _get_title_from_reference(reference: str) -> str:
-    """Convert JSONSchema references to title fields.
+    """Convert JSON Schema references to title fields.
 
     If the reference has a pointer, use the final segment, otherwise
     use the final segment of the base uri stripping any content type
     extension.
 
     :param reference: The JSONPointer reference.
     """
```

### Comparing `statham-schema-0.8.0/setup.py` & `statham-schema-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,23 +26,24 @@
 with open("README.md", "r") as readme_file:
     LONG_DESCRIPTION = readme_file.read()
 
 setup(
     name="statham-schema",
     version=statham.__version__,
     description=(
-        "Tools for generating Python models from JSONSchema definitions."
+        "Tools for generating Python models from JSON Schema documents."
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jacksmith15/statham-schema",
     author="Jack Smith",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.6",
     ],
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
+    package_data={"statham": ["py.typed"]},
     install_requires=REQUIREMENTS_FILE,
     dependency_links=[],
     entry_points={"console_scripts": ["statham=statham.__main__:entry_point"]},
 )
```

### Comparing `statham-schema-0.8.0/CHANGELOG.md` & `statham-schema-0.9.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,45 @@
 * **Added** for new features.
 * **Changed** for changes in existing functionality.
 * **Removed** for now removed features.
 * **Fixed** for any bug fixes.
 
 ## [Unreleased]
 
+## [0.9.0] - 2020-04-20
+### Added
+* Added functions for converting DSL defined schemas to JSON Schema
+  dictionaries.
+  - `serialize_json` supports serialization of schemas with
+    definitions and references.
+  - `serialize_element` supports simple inline serialization
+    of elements.
+* Documentation including a tutorial and API reference.
+
+### Changed
+* Moved `serialize_python` to from `statham.serializer` to
+  `statham.serializers`.
+* `serialize_python` now dynamically infers which imports
+  to include based on the supplied elements.
+* Rewrote `statham.orderer.Orderer` in functional style, renamed
+  to `orderer`. This allows more general use of some of its
+  functionality via the `get_children` and `get_object_classes`
+  functions in this module.
+* Attempting to parse schemas with recursive references now
+  raises a `FeatureNotImplementedError`.
+* Raised version of `json-ref-dict` to `0.6.0` - now supports
+  references with URL-encoded characters.
+* Property names which conflict with reserved names now have an
+  underscore appended by the parser (previously prepended).
+* Better validation error messages on unbound elements.
+
+### Fixed
+* Fixed missing imports in generated python modules.
+* Type hints are now correctly detected when installed.
+
 ## [0.8.0] - 2020-04-09
 ### Changed
 * `default` is now a class argument on subclasses of `ObjectMeta`.
 * Bump `json-ref-dict` to version `0.5.3`.
 * Improve implementation of official JSON Schema test suite.
 
 ## [0.7.0] - 2020-04-04
@@ -179,15 +210,16 @@
         + `maxLength`
     - `null`
 
 
 ## [0.0.0]
 Nothing here.
 
-[Unreleased]: http://github.com/jacksmith15/statham-schema/compare/0.8.0..HEAD
+[Unreleased]: http://github.com/jacksmith15/statham-schema/compare/0.9.0..HEAD
+[0.9.0]: http://github.com/jacksmith15/statham-schema/compare/0.8.0..0.9.0
 [0.8.0]: http://github.com/jacksmith15/statham-schema/compare/0.7.0..0.8.0
 [0.7.0]: http://github.com/jacksmith15/statham-schema/compare/0.6.0..0.7.0
 [0.6.0]: http://github.com/jacksmith15/statham-schema/compare/0.5.0..0.6.0
 [0.5.0]: http://github.com/jacksmith15/statham-schema/compare/0.4.0..0.5.0
 [0.4.0]: http://github.com/jacksmith15/statham-schema/compare/0.3.0..0.4.0
 [0.3.0]: http://github.com/jacksmith15/statham-schema/compare/0.2.0..0.3.0
 [0.2.0]: http://github.com/jacksmith15/statham-schema/compare/0.1.1..0.2.0
```

### Comparing `statham-schema-0.8.0/tests/models/field_validation.py` & `statham-schema-0.9.0/tests/models/field_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from typing import List, Union
+from typing import List
 
 from statham.dsl.constants import Maybe
 from statham.dsl.elements import (
-    AnyOf,
     Array,
     Boolean,
     Integer,
     Null,
     Number,
-    OneOf,
     Object,
     String,
 )
 from statham.dsl.property import Property
 
 
 class Model(Object):
```

### Comparing `statham-schema-0.8.0/tests/models/remote_ref.py` & `statham-schema-0.9.0/tests/models/remote_ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-from typing import List, Union
-
 from statham.dsl.constants import Maybe
-from statham.dsl.elements import (
-    AnyOf,
-    Array,
-    Boolean,
-    Integer,
-    Null,
-    Number,
-    OneOf,
-    Object,
-    String,
-)
+from statham.dsl.elements import Object, String
 from statham.dsl.property import Property
 
 
 class Category(Object):
 
     required_name: str = Property(String(), required=True)
```

### Comparing `statham-schema-0.8.0/tests/models/autoname.py` & `statham-schema-0.9.0/tests/models/autoname.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-from typing import List, Union
+from typing import Any, List, Union
 
 from statham.dsl.constants import Maybe
-from statham.dsl.elements import (
-    AnyOf,
-    Array,
-    Boolean,
-    Integer,
-    Null,
-    Number,
-    OneOf,
-    Object,
-    String,
-)
+from statham.dsl.elements import AnyOf, Array, Integer, Object, String
 from statham.dsl.property import Property
 
 
 class ListOfStringsItem(Object, additionalProperties=False):
 
     string_property: Maybe[str] = Property(String())
```

### Comparing `statham-schema-0.8.0/tests/models/union_types.py` & `statham-schema-0.9.0/tests/models/union_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-from typing import List, Union
+from typing import Any, Union
 
-from statham.dsl.constants import Maybe
-from statham.dsl.elements import (
-    AnyOf,
-    Array,
-    Boolean,
-    Integer,
-    Null,
-    Number,
-    OneOf,
-    Object,
-    String,
-)
+from statham.dsl.elements import AnyOf, Integer, Null, Number, Object, String
 from statham.dsl.property import Property
 
 
 class Model(Object):
 
     number_integer: Union[float, int] = Property(
         AnyOf(
```

### Comparing `statham-schema-0.8.0/tests/models/simple.py` & `statham-schema-0.9.0/tests/models/simple.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-from typing import List, Union
+from typing import List
 
 from statham.dsl.constants import Maybe
-from statham.dsl.elements import (
-    AnyOf,
-    Array,
-    Boolean,
-    Integer,
-    Null,
-    Number,
-    OneOf,
-    Object,
-    String,
-)
+from statham.dsl.elements import Array, Integer, Number, Object, String
 from statham.dsl.property import Property
 
 
 class NestedSchema(Object):
 
     id: str = Property(
         String(
```

### Comparing `statham-schema-0.8.0/PKG-INFO` & `statham-schema-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: statham-schema
-Version: 0.8.0
-Summary: Tools for generating Python models from JSONSchema definitions.
+Version: 0.9.0
+Summary: Tools for generating Python models from JSON Schema documents.
 Home-page: https://github.com/jacksmith15/statham-schema
 Author: Jack Smith
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.com/jacksmith15/statham-schema.svg?token=JrMQr8Ynsmu5tphpTQ2p&branch=master)](https://travis-ci.com/jacksmith15/statham-schema)
         # Statham Schema
-        A tool for generating Python objects from [JSONSchema](https://json-schema.org/) documents.
+        A tool for generating Python objects from [JSON Schema](https://json-schema.org/) documents.
         
         This project aims to simplify the experience of integrating with external sources, by providing:
         1. **External validation**: Ensure that incoming data matches what you expect.
         2. **Internal validation**: Ensure your application logic is consistent with the schema. Static type checking (see [mypy](http://mypy-lang.org/)) can do this job for you.
-        3. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
+        3. **Extensibility**: Extend the generated models with properties and methods useful to you.
+        4. **Visibility**: Update the model layer against schema changes automatically, and let static tools identify any issues.
         
         The models generated by this tool are declared using a JSONSchema DSL. This DSL can easily be used to write schemas by hand, and extend models with extra features.
         
         ## Example DSL Definition
         ```python
         from typing import List
         
@@ -26,20 +27,18 @@
         
         class Choice(Object):
             choice_text: str = Property(String(maxLength=200), required=True)
             votes: int = Property(Integer(default=0))
         
         
         class Poll(Object):
-            question: str = Property(String(maxLength=200), required=True)
+            question: str = Property(String(), required=True)
             choices: List[Choice] = Property(Array(Choice), required=True)
         ```
         
-        Development currently targets compatibility with JSONSchema Draft 6.
-        
         # Requirements
         This package is currently tested for Python 3.6.
         
         # Installation
         This project may be installed using [pip](https://pip.pypa.io/en/stable/):
         ```
         pip install statham-schema
@@ -81,48 +80,38 @@
         
         @format_checker.register("my_format")
         def _check_my_format(value: str) -> bool:
             ...
         ```
         
         # Supported JSONSchema features
-        - [x] Basic types (primitves, array, object)
-        - [x] Composite primitive types
-        - [x] Type validation on generated classes
-        - [x] Validation of `required`
-        - [x] Local references
-        - [x] Type-specific validation (pattern, format, minimum, maximum etc)
-        - [x] Custom string format validation
-        - [x] Remote references
-        - [x] `anyOf`, `oneOf`, `allOf`, `not`
-        - [x] `additionalProperties`
-        - [x] Tuple validation of arrays
-        - [x] `additionalItems` keyword
-        - [x] `minProperties`, `maxProperties` keywords
-        - [x] `patternProperties` keyword
-        - [x] `uniqueItems` keyword
-        - [x] `propertyNames` keyword
-        - [x] `const` keyword
-        - [x] `contains` keyword
-        - [x] `enum` keyword
-        - [x] `dependencies` keyword
-        - [ ] Built-in string format validation #6
-        - [ ] `if`, `then`, `else` keywords
+        This library is tested to support [JSON Schema Draft 6](https://json-schema.org/specification-links.html#draft-6), with the following notable exceptions:
+        - Recursive references are not supported.
+        - Location-independent references are not supported.
+        - Changes of base URI via the `$id` keyword are not detected.
+        
+        Priority order for remaining features is roughly as follows:
+        1. Support for features of more recent drafts.
+        2. Support for the exceptions listed above.
+        3. Support for features of less recent drafts.
+        
+        However, contributions in any of these areas are welcome.
         
         # Development
         1. Clone the repository: `git clone git@github.com:jacksmith15/statham-schema.git && cd statham-schema`
         2. Install the requirements: `pip install -r requirements.txt -r requirements-test.txt`
         3. Run `pre-commit install`
         4. Run the tests: `bash run_test.sh -c -a`
         
         This project uses the following QA tools:
         - [PyTest](https://docs.pytest.org/en/latest/) - for running unit tests.
         - [PyLint](https://www.pylint.org/) - for enforcing code style.
         - [MyPy](http://mypy-lang.org/) - for static type checking.
         - [Travis CI](https://travis-ci.org/) - for continuous integration.
+        - [Black](https://black.readthedocs.io/en/stable/) - for uniform code formatting.
         
         # License
         This project is distributed under the MIT license.
         
         ![statham](https://giant.gfycat.com/GrotesqueNauticalCaracal.gif)
         
 Platform: UNKNOWN
```

