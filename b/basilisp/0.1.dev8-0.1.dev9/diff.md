# Comparing `tmp/basilisp-0.1.dev8.tar.gz` & `tmp/basilisp-0.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/basilisp-0.1.dev8.tar", last modified: Mon Mar 11 01:33:39 2019, max compression
+gzip compressed data, was "dist/basilisp-0.1.dev9.tar", last modified: Sat Mar 30 00:01:34 2019, max compression
```

## Comparing `basilisp-0.1.dev8.tar` & `basilisp-0.1.dev9.tar`

### file list

```diff
@@ -1,61 +1,66 @@
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/
--rw-r--r--   0 christopher   (501) staff       (20)     4594 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/PKG-INFO
--rw-r--r--   0 christopher   (501) staff       (20)    11248 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/LICENSE
--rw-r--r--   0 christopher   (501) staff       (20)       35 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/MANIFEST.in
--rw-r--r--   0 christopher   (501) staff       (20)     2991 2019-03-11 01:31:10.000000 basilisp-0.1.dev8/README.md
--rw-r--r--   0 christopher   (501) staff       (20)     3656 2019-03-10 20:41:37.000000 basilisp-0.1.dev8/setup.py
--rw-r--r--   0 christopher   (501) staff       (20)       38 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/setup.cfg
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp/
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp/core/
--rw-r--r--   0 christopher   (501) staff       (20)    66204 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/core/__init__.lpy
--rw-r--r--   0 christopher   (501) staff       (20)    11416 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/importer.py
--rw-r--r--   0 christopher   (501) staff       (20)     2218 2019-03-10 20:17:16.000000 basilisp-0.1.dev8/src/basilisp/util.py
--rw-r--r--   0 christopher   (501) staff       (20)     1086 2019-03-10 20:17:16.000000 basilisp-0.1.dev8/src/basilisp/walker.py
--rw-r--r--   0 christopher   (501) staff       (20)        0 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/__init__.py
--rw-r--r--   0 christopher   (501) staff       (20)       68 2019-03-11 01:25:05.000000 basilisp-0.1.dev8/src/basilisp/__version__.py
--rw-r--r--   0 christopher   (501) staff       (20)     4408 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/set.lpy
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp/lang/
--rw-r--r--   0 christopher   (501) staff       (20)      224 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/deref.py
--rw-r--r--   0 christopher   (501) staff       (20)      447 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/associative.py
--rw-r--r--   0 christopher   (501) staff       (20)      442 2019-03-10 20:41:37.000000 basilisp-0.1.dev8/src/basilisp/lang/exception.py
--rw-r--r--   0 christopher   (501) staff       (20)     2426 2019-03-01 02:02:44.000000 basilisp-0.1.dev8/src/basilisp/lang/vector.py
--rw-r--r--   0 christopher   (501) staff       (20)     2206 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/list.py
--rw-r--r--   0 christopher   (501) staff       (20)     2832 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/util.py
--rw-r--r--   0 christopher   (501) staff       (20)        0 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/__init__.py
--rw-r--r--   0 christopher   (501) staff       (20)     1656 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/symbol.py
--rw-r--r--   0 christopher   (501) staff       (20)    35684 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/runtime.py
--rw-r--r--   0 christopher   (501) staff       (20)     6401 2019-02-06 03:20:52.000000 basilisp-0.1.dev8/src/basilisp/lang/map.py
--rw-r--r--   0 christopher   (501) staff       (20)     5702 2019-03-10 20:07:40.000000 basilisp-0.1.dev8/src/basilisp/lang/obj.py
--rw-r--r--   0 christopher   (501) staff       (20)    32889 2019-03-10 20:31:16.000000 basilisp-0.1.dev8/src/basilisp/lang/reader.py
--rw-r--r--   0 christopher   (501) staff       (20)     1530 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/keyword.py
--rw-r--r--   0 christopher   (501) staff       (20)      750 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/delay.py
--rw-r--r--   0 christopher   (501) staff       (20)      273 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/collection.py
--rw-r--r--   0 christopher   (501) staff       (20)      696 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/typing.py
--rw-r--r--   0 christopher   (501) staff       (20)     3159 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/multifn.py
--rw-r--r--   0 christopher   (501) staff       (20)     3308 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/set.py
--rw-r--r--   0 christopher   (501) staff       (20)      609 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/atom.py
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/
--rw-r--r--   0 christopher   (501) staff       (20)      692 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/exception.py
--rw-r--r--   0 christopher   (501) staff       (20)     1122 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/constants.py
--rw-r--r--   0 christopher   (501) staff       (20)     6544 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/__init__.py
--rw-r--r--   0 christopher   (501) staff       (20)    55483 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/parser.py
--rw-r--r--   0 christopher   (501) staff       (20)    70784 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/generator.py
--rw-r--r--   0 christopher   (501) staff       (20)     3507 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/optimizer.py
--rw-r--r--   0 christopher   (501) staff       (20)    17944 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/lang/compiler/nodes.py
--rw-r--r--   0 christopher   (501) staff       (20)     5738 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/seq.py
--rw-r--r--   0 christopher   (501) staff       (20)      263 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/lang/meta.py
--rw-r--r--   0 christopher   (501) staff       (20)     4682 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/test.lpy
--rw-r--r--   0 christopher   (501) staff       (20)     6751 2019-03-10 20:41:37.000000 basilisp-0.1.dev8/src/basilisp/cli.py
--rw-r--r--   0 christopher   (501) staff       (20)      768 2019-03-10 20:56:01.000000 basilisp-0.1.dev8/src/basilisp/logconfig.py
--rw-r--r--   0 christopher   (501) staff       (20)     6907 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/string.lpy
--rw-r--r--   0 christopher   (501) staff       (20)     1005 2019-03-11 01:18:23.000000 basilisp-0.1.dev8/src/basilisp/repl.lpy
--rw-r--r--   0 christopher   (501) staff       (20)      476 2019-01-22 23:27:35.000000 basilisp-0.1.dev8/src/basilisp/main.py
--rw-r--r--   0 christopher   (501) staff       (20)     7107 2019-02-12 13:49:11.000000 basilisp-0.1.dev8/src/basilisp/testrunner.py
-drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/
--rw-r--r--   0 christopher   (501) staff       (20)     4594 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/PKG-INFO
--rw-r--r--   0 christopher   (501) staff       (20)     1447 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/SOURCES.txt
--rw-r--r--   0 christopher   (501) staff       (20)      102 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/entry_points.txt
--rw-r--r--   0 christopher   (501) staff       (20)       72 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/requires.txt
--rw-r--r--   0 christopher   (501) staff       (20)        9 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/top_level.txt
--rw-r--r--   0 christopher   (501) staff       (20)        1 2019-03-11 01:33:39.000000 basilisp-0.1.dev8/src/basilisp.egg-info/dependency_links.txt
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/
+-rw-r--r--   0 christopher   (501) staff       (20)     4594 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/PKG-INFO
+-rw-r--r--   0 christopher   (501) staff       (20)    11248 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/LICENSE
+-rw-r--r--   0 christopher   (501) staff       (20)       35 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/MANIFEST.in
+-rw-r--r--   0 christopher   (501) staff       (20)     2991 2019-03-11 01:48:34.000000 basilisp-0.1.dev9/README.md
+-rw-r--r--   0 christopher   (501) staff       (20)     3656 2019-03-10 20:41:37.000000 basilisp-0.1.dev9/setup.py
+-rw-r--r--   0 christopher   (501) staff       (20)       38 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/setup.cfg
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/core/
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/core/__pycache__/
+-rw-r--r--   0 christopher   (501) staff       (20)   223101 2019-03-29 23:00:50.000000 basilisp-0.1.dev9/src/basilisp/core/__pycache__/__init__.cpython-36.lpyc
+-rw-r--r--   0 christopher   (501) staff       (20)    73321 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/core/__init__.lpy
+-rw-r--r--   0 christopher   (501) staff       (20)    11416 2019-03-28 12:06:03.000000 basilisp-0.1.dev9/src/basilisp/importer.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2218 2019-03-10 20:17:16.000000 basilisp-0.1.dev9/src/basilisp/util.py
+-rw-r--r--   0 christopher   (501) staff       (20)     1086 2019-03-10 20:17:16.000000 basilisp-0.1.dev9/src/basilisp/walker.py
+-rw-r--r--   0 christopher   (501) staff       (20)        0 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/__init__.py
+-rw-r--r--   0 christopher   (501) staff       (20)       68 2019-03-30 00:01:11.000000 basilisp-0.1.dev9/src/basilisp/__version__.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/__pycache__/
+-rw-r--r--   0 christopher   (501) staff       (20)     7215 2019-03-28 12:17:43.000000 basilisp-0.1.dev9/src/basilisp/__pycache__/repl.cpython-36.lpyc
+-rw-r--r--   0 christopher   (501) staff       (20)    14738 2019-03-28 02:33:41.000000 basilisp-0.1.dev9/src/basilisp/__pycache__/test.cpython-36.lpyc
+-rw-r--r--   0 christopher   (501) staff       (20)     4408 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/set.lpy
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/lang/
+-rw-r--r--   0 christopher   (501) staff       (20)      224 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/deref.py
+-rw-r--r--   0 christopher   (501) staff       (20)      447 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/associative.py
+-rw-r--r--   0 christopher   (501) staff       (20)      442 2019-03-10 20:41:37.000000 basilisp-0.1.dev9/src/basilisp/lang/exception.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2426 2019-03-25 12:31:01.000000 basilisp-0.1.dev9/src/basilisp/lang/vector.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2206 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/list.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2855 2019-03-23 16:35:18.000000 basilisp-0.1.dev9/src/basilisp/lang/util.py
+-rw-r--r--   0 christopher   (501) staff       (20)        0 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/__init__.py
+-rw-r--r--   0 christopher   (501) staff       (20)     1669 2019-03-16 17:35:20.000000 basilisp-0.1.dev9/src/basilisp/lang/symbol.py
+-rw-r--r--   0 christopher   (501) staff       (20)    45944 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/lang/runtime.py
+-rw-r--r--   0 christopher   (501) staff       (20)     5430 2019-03-16 17:35:20.000000 basilisp-0.1.dev9/src/basilisp/lang/map.py
+-rw-r--r--   0 christopher   (501) staff       (20)    10295 2019-03-16 17:35:20.000000 basilisp-0.1.dev9/src/basilisp/lang/obj.py
+-rw-r--r--   0 christopher   (501) staff       (20)    33631 2019-03-16 17:35:20.000000 basilisp-0.1.dev9/src/basilisp/lang/reader.py
+-rw-r--r--   0 christopher   (501) staff       (20)     2371 2019-03-20 01:26:10.000000 basilisp-0.1.dev9/src/basilisp/lang/keyword.py
+-rw-r--r--   0 christopher   (501) staff       (20)      750 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/delay.py
+-rw-r--r--   0 christopher   (501) staff       (20)      273 2019-03-17 20:17:46.000000 basilisp-0.1.dev9/src/basilisp/lang/collection.py
+-rw-r--r--   0 christopher   (501) staff       (20)      877 2019-03-16 17:35:20.000000 basilisp-0.1.dev9/src/basilisp/lang/typing.py
+-rw-r--r--   0 christopher   (501) staff       (20)     3159 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/multifn.py
+-rw-r--r--   0 christopher   (501) staff       (20)     3308 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/set.py
+-rw-r--r--   0 christopher   (501) staff       (20)      609 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/atom.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/
+-rw-r--r--   0 christopher   (501) staff       (20)      692 2019-03-11 01:18:23.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/exception.py
+-rw-r--r--   0 christopher   (501) staff       (20)     1314 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/constants.py
+-rw-r--r--   0 christopher   (501) staff       (20)     7012 2019-03-28 12:06:18.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/__init__.py
+-rw-r--r--   0 christopher   (501) staff       (20)    70183 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/parser.py
+-rw-r--r--   0 christopher   (501) staff       (20)    82751 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/generator.py
+-rw-r--r--   0 christopher   (501) staff       (20)     3507 2019-03-11 01:18:23.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/optimizer.py
+-rw-r--r--   0 christopher   (501) staff       (20)    21296 2019-03-29 23:17:06.000000 basilisp-0.1.dev9/src/basilisp/lang/compiler/nodes.py
+-rw-r--r--   0 christopher   (501) staff       (20)     5738 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/seq.py
+-rw-r--r--   0 christopher   (501) staff       (20)      263 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/lang/meta.py
+-rw-r--r--   0 christopher   (501) staff       (20)     4682 2019-03-11 01:18:23.000000 basilisp-0.1.dev9/src/basilisp/test.lpy
+-rw-r--r--   0 christopher   (501) staff       (20)     8464 2019-03-23 19:52:09.000000 basilisp-0.1.dev9/src/basilisp/cli.py
+-rw-r--r--   0 christopher   (501) staff       (20)      768 2019-03-10 20:56:01.000000 basilisp-0.1.dev9/src/basilisp/logconfig.py
+-rw-r--r--   0 christopher   (501) staff       (20)     6907 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/string.lpy
+-rw-r--r--   0 christopher   (501) staff       (20)     1005 2019-03-11 01:18:23.000000 basilisp-0.1.dev9/src/basilisp/repl.lpy
+-rw-r--r--   0 christopher   (501) staff       (20)      476 2019-01-22 23:27:35.000000 basilisp-0.1.dev9/src/basilisp/main.py
+-rw-r--r--   0 christopher   (501) staff       (20)     7107 2019-02-12 13:49:11.000000 basilisp-0.1.dev9/src/basilisp/testrunner.py
+drwxr-xr-x   0 christopher   (501) staff       (20)        0 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/
+-rw-r--r--   0 christopher   (501) staff       (20)     4594 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/PKG-INFO
+-rw-r--r--   0 christopher   (501) staff       (20)     1594 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/SOURCES.txt
+-rw-r--r--   0 christopher   (501) staff       (20)      102 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/entry_points.txt
+-rw-r--r--   0 christopher   (501) staff       (20)       72 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/requires.txt
+-rw-r--r--   0 christopher   (501) staff       (20)        9 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/top_level.txt
+-rw-r--r--   0 christopher   (501) staff       (20)        1 2019-03-30 00:01:34.000000 basilisp-0.1.dev9/src/basilisp.egg-info/dependency_links.txt
```

### Comparing `basilisp-0.1.dev8/PKG-INFO` & `basilisp-0.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basilisp
-Version: 0.1.dev8
+Version: 0.1.dev9
 Summary: A Clojure-like lisp written for Python
 Home-page: http://github.com/chrisrink10/basilisp
 Author: Christopher Rink
 Author-email: chrisrink10@gmail.com
 License: Eclipse Public License 1.0
 Description: 
         # 🐍 basilisp 🐍
```

### Comparing `basilisp-0.1.dev8/LICENSE` & `basilisp-0.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/README.md` & `basilisp-0.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/setup.py` & `basilisp-0.1.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/core/__init__.lpy` & `basilisp-0.1.dev9/src/basilisp/core/__init__.lpy`

 * *Files 10% similar despite different names*

```diff
@@ -54,26 +54,28 @@
          (.-meta o)
          nil)))
 
 (def ^{:doc      "Return o with the supplied metadata map assoc'ed into its existing metadata."
        :arglists '([o meta])}
   with-meta
   (fn* with-meta [o meta]
-       (.with-meta o meta)))
+       (if meta
+         (.with-meta o meta)
+         o)))
 
 (def ^:macro ^:redef let
-  (fn* let [&form & decl]
+  (fn* let [&env &form & decl]
        (cons 'let* decl)))
 
 (def ^:macro ^:redef loop
-  (fn* loop [&form & decl]
+  (fn* loop [&env &form & decl]
        (cons 'loop* decl)))
 
 (def ^:macro ^:redef fn
-  (fn* fn [&form & decl]
+  (fn* fn [&env &form & decl]
        (with-meta
          (cons 'fn* decl)
          (meta &form))))
 
 (def ^{:doc      "Returns its argument unmodified."
        :arglists '([v])}
   identity
@@ -258,41 +260,47 @@
   conj
   (fn conj [coll & xs]
     (apply basilisp.lang.runtime/conj coll xs)))
 
 (def
   ^{:macro    true
     :doc      "Define a new function with an optional docstring."
-    :arglists '([name & body] [name doc & body])}
+    :arglists '([name & body] [name doc? & body] [name doc? attr-map? & body])}
   defn
-  (fn defn [&form name & body]
+  (fn defn [&env &form name & body]
     (if (symbol? name)
       nil  ;; Do nothing!
       (throw (ex-info "First argument to defn must be a symbol"
                       {:found name :type (builtins/type name)})))
     (let [body   (concat body)
           doc    (if (string? (first body))
                    (first body)
                    nil)
-          fname  (if doc
-                   (with-meta name {:doc doc})
-                   name)
           body   (if doc
                    (rest body)
                    body)
+          fmeta (if (map? (first body))
+                  (first body)
+                  nil)
+          fname  (if doc
+                   (with-meta name (assoc fmeta :doc doc))
+                   (with-meta name fmeta))
+          body   (if fmeta
+                   (rest body)
+                   body)
           multi? (list? (first body))
           fsigs  (if multi?
                    (loop [arities body
                           sigs    []]
                      (if (seq arities)
                        (recur (rest arities)
                               (conj sigs (ffirst arities)))
-                       `(quote ~(apply list sigs))))
-                   `(quote ~(list (first body))))
-          fname  (with-meta fname {:arglists fsigs})
+                       (apply list sigs)))
+                   (list (first body)))
+          fname  (with-meta fname {:arglists (list 'quote fsigs)})
           body   (if multi?
                    body
                    (cons
                     (if (vector? (first body))
                       (first body)
                       (throw
                        (ex-info "Expected an argument vector"
@@ -374,45 +382,54 @@
 
 (defn namespace
   "Return the namespace of a symbol or keyword, or nil if no namespace."
   [v]
   (.-ns v))
 
 (def
-  ^{:macro true
-    :doc   "Define a new macro like defn. Macro functions are available to the
-            compiler during macroexpansion."}
+  ^{:macro    true
+    :doc      "Define a new macro like defn. Macro functions are available to the
+               compiler during macroexpansion."
+    :arglists '([name & body] [name doc? & body] [name doc? attr-map? & body])}
   defmacro
-  (fn defmacro [&form name & body]
+  (fn defmacro [&env &form name & body]
     (let [body   (concat body)
           doc    (if (string? (first body))
                    (first body)
                    nil)
-          fname  (with-meta (if doc
-                              (with-meta name {:doc doc})
-                              name)
-                   {:macro true})
           body   (if doc
                    (rest body)
                    body)
+          fmeta  (if (map? (first body))
+                   (first body)
+                   nil)
+          body   (if fmeta
+                   (rest body)
+                   body)
+          fname  (if doc
+                   (with-meta name (assoc fmeta :doc doc :macro true))
+                   (with-meta name (assoc fmeta :macro true)))
           multi? (list? (first body))
           fsigs  (if multi?
                    (loop [arities body
                           sigs    []]
                      (if (seq arities)
                        (recur (rest arities)
                               (conj sigs (ffirst arities)))
                        `(quote ~(apply list sigs))))
                    `(quote ~(list (first body))))
           fname  (with-meta fname {:arglists fsigs})
 
           add-implicit-args (fn [body]
                               (cons
                                (if (vector? (first body))
-                                 (apply vector (cons '&form (first body)))
+                                 (apply vector
+                                        (cons '&env
+                                              (cons '&form
+                                                    (first body))))
                                  (throw
                                   (ex-info "Expected an argument vector"
                                            {:found (first body)})))
                                (rest body)))
 
           add-args-for-each (fn [in out]
                               (if (seq (rest in))
@@ -422,14 +439,38 @@
 
           body (if multi?
                  (add-args-for-each body [])
                  (add-implicit-args body))]
       `(defn ~fname
          ~@body))))
 
+(defmacro defasync
+  "Define a new asynchronous function with an optional docstring."
+  [name & body]
+  (let [body   (concat body)
+        doc    (if (string? (first body))
+                 (first body)
+                 nil)
+        body   (if doc
+                 (rest body)
+                 body)
+        fmeta (if (map? (first body))
+                (assoc (first body))
+                nil)
+        body   (if fmeta
+                 (rest body)
+                 body)
+        fmeta (apply assoc fmeta (concat [:async true]
+                                         (if doc
+                                           [:doc doc]
+                                           nil)))]
+    `(defn ~name
+       ~fmeta
+       ~@body)))
+
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Logical Comparisons & Macros ;;
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
 (defmacro if-not
   "Evaluate cond and if it is true, return false-cond. Otherwise return
   true-cond."
@@ -796,14 +837,18 @@
   [m]
   (seq (.values m)))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Higher Order Functions ;;
 ;;;;;;;;;;;;;;;;;;;;;;;;;;;;
 
+(defn apply-kw
+  [f & args]
+  (basilisp.lang.runtime/apply-kw f args))
+
 (defmacro lazy-seq
   "Takes a body of expressions which will produce a seq or nil. When
   seq is first called on the resulting lazy-seq, the sequence will be
   realized."
   [& body]
   (list 'basilisp.lang.seq/LazySeq
         (concat '(fn* []) body)))
@@ -1539,20 +1584,19 @@
                                      *data-readers*
                                      eof-value
                                      eof-error?))))
 
 (defn eval
   "Evaluate a form (not a string) and return its result."
   [form]
-  (let [ctx    (basilisp.lang.compiler.CompilerContext.)
+  (let [ctx    (basilisp.lang.compiler.CompilerContext. "<Eval Input>")
         module (.-module *ns*)]
     (basilisp.lang.compiler/compile-and-exec-form form
                                                   ctx
-                                                  module
-                                                  "<Eval Input>")))
+                                                  module)))
 
 ;;;;;;;;;;;;;;;;;;;;;;;;;
 ;; Namespace Utilities ;;
 ;;;;;;;;;;;;;;;;;;;;;;;;;
 
 (defn the-ns
   "If v is a symbol, return the Namespace named by that symbol if it
@@ -2176,22 +2220,23 @@
                   (first body))
         body    (cond-> body name rest)
         arities (cond
                   (vector? (first body))
                   (fn-arity-with-destructuring body)
 
                   (seq? (first body))
-                  (map fn-arity-with-destructuring body)
+                  (apply list (map fn-arity-with-destructuring body))
 
                   :else
                   body)]
-    (if name
-      `(fn* ~name
-            ~@arities)
-      `(fn* ~@arities))))
+    (as-> arities $
+      (cond->> $ name (cons name))
+      (cons 'fn* $)
+      (cond-> $
+        (meta &form) (with-meta (meta &form))))))
 
 (defn destructure
   "Take a [binding expr] pair (as from a let block) and produce all of the
   replacement bindings for the binding which perform destructuring on the
   initial expression.
 
   As an example, for sequential destructuring like:
@@ -2241,7 +2286,144 @@
 
 (defmacro ^:no-warn-on-redef loop
   "Loop bindings with destructuring support."
   [bindings & body]
   (let [[bindings body] (loop-with-destructuring bindings body)]
     `(loop* ~bindings
         ~@body)))
+
+;;;;;;;;;;;;;;;;;;;;;;;
+;; Interop Functions ;;
+;;;;;;;;;;;;;;;;;;;;;;;
+
+(defn lisp->py
+  "Recursively convert Basilisp data structures into Python data structures.
+
+  Callers can specify a keyword argument :keyword-fn, which names a function
+  which is called for each keyword value in the input structure to return a
+  new value. By default :keyword-fn is the function `name`."
+  ([o]
+   (basilisp.lang.runtime/to-py o))
+  ([o & {:keys [keyword-fn] :or {keyword-fn name}}]
+   (basilisp.lang.runtime/to-py o keyword-fn)))
+
+(defn py->lisp
+  "Recursively convert Python data structures into Basilisp data structures.
+
+  Callers can specify a keyword argument :keywordize-keys, which defaults to
+  true. If :keywordize-keys is true, then all string keys in Python dicts will
+  be converted into keywords in the final return value."
+  ([o]
+   (basilisp.lang.runtime/to-lisp o))
+  ([o & {:keys [keywordize-keys] :or {keywordize-keys true}}]
+   (basilisp.lang.runtime/to-lisp o keywordize-keys)))
+
+;;;;;;;;;;;;;;;;;;;;;;;;;;;;
+;; Data Types & Protocols ;;
+;;;;;;;;;;;;;;;;;;;;;;;;;;;;
+
+(import* abc)
+
+(defmulti ^:private munge
+  "Munge the input value into a Python-safe string. Converts keywords and
+  symbols into strings as by `name` prior to munging. Returns a string."
+  builtins/type)
+
+(defmethod munge basilisp.lang.keyword/Keyword
+  [kw]
+  (basilisp.lang.util/munge (name kw)))
+
+(defmethod munge basilisp.lang.symbol/Symbol
+  [s]
+  (basilisp.lang.util/munge (name s)))
+
+(defmethod munge builtins/str
+  [s]
+  (basilisp.lang.util/munge s))
+
+(defn gen-interface
+  "Generate and return a new Python interface (abstract base clase).
+
+  Callers should use `definterface` to generate new interfaces."
+  [interface-name methods]
+  (let [methods (reduce (fn [m [method-name args]]
+                          (let [method-args (->> (concat ['self] args)
+                                                 (apply vector))
+                                method      (->> (list 'fn* method-name method-args)
+                                                 (eval)
+                                                 (abc/abstractmethod))]
+                            (assoc m (munge method-name) method)))
+                        {}
+                        methods)]
+    (builtins/type interface-name
+                   #py (abc/ABC)
+                   (lisp->py methods))))
+
+(defmacro definterface
+  "Define a new Python interface (abstract base clase) with the given name
+  and method signatures.
+
+  Method signatures are in the form (method-name [arg1 arg2 ...]).
+
+  Interface objects cannot be directly instantiated. Instead, you must create
+  a concrete implementation of an interface (perhaps via deftype) and supply
+  implementations for all of the abstract methods.
+
+  The generated interface derives from Python's `abc.ABC` and all method
+  definitions are declared as `abc.abstractmethod`s and thus must be implemented
+  by a concrete type.
+
+  The generated interface will be immediately available after this form has
+  been evaluated and its utility is not limited to compilation."
+  [interface-name & methods]
+  (let [name-str    (name interface-name)
+        method-sigs (map #(list 'quote %) methods)]
+    `(def ~interface-name
+       (gen-interface ~name-str [~@method-sigs]))))
+
+(defmacro deftype
+  "Define a new Python concrete type which can implement 0 or more Python
+  interfaces or Basilisp protocols.
+
+  The new type will have fields matching the names in `fields`. Fields may
+  be referred to unqualified in the bodies of implemented methods. By default
+  the fields of this type are immutable. Attempting to set non-mutable fields
+  from a method body will result in a compiler error.
+
+  Fields may be made mutable by annotating their definition with `:mutable`
+  metadata. Mutable fields may be set within method bodies using the `set!`
+  special form. It is not advised to use mutable fields unless you are sure
+  you know what you are doing. As a consequence of Python's lax policy towards
+  immutability, types with even one mutable field may be mutated by outside
+  callers using `set!`, so bear that in mind when choosing mutability.
+
+  Interface or protocol implementations are declared as the name of the
+  interface or protocol as a symbol, followed by 1 or more method
+  definitions for that interface. Types are not required to declare
+  any interface implementations. Types which do declare interface
+  implementations are required to implement all interface methods. Failing
+  to implement all interface methods is a compile time error. Types
+  implementing `object` are not required to implement all `object` methods.
+
+  Method declarations should appear as:
+
+    (method-name [arg1 arg2 ...] & body)
+
+  Type objects are created with sensible `object` defaults as by `attrs`.
+  New types may override `object` defaults. An `__init__` function is
+  automatically created which takes positional arguments matching the
+  order of definition in `fields`. Additionally, given a name `NewType`,
+  a factory function will be created `->NewType` which can be used to
+  generate new instances of the type.
+
+  Methods must supply a `this` or `self` parameter. `recur` special forms
+  used in the body of a method should not include that parameter, as it
+  will be supplied automatically."
+  [type-name fields & method-impls]
+  (let [ctor-name (with-meta
+                    (symbol (str "->" (name type-name)))
+                    (meta type-name))]
+    `(do
+       (deftype* ~type-name ~fields
+         ~@method-impls)
+       (def ~ctor-name ~type-name)
+       ~type-name)))
```

### Comparing `basilisp-0.1.dev8/src/basilisp/importer.py` & `basilisp-0.1.dev9/src/basilisp/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         # as direct Python variable access to functions and other def'ed values.
         ns_name = demunge(fullname)
         ns: runtime.Namespace = runtime.set_current_ns(ns_name).value
         ns.module = module
 
         # Check if a valid, cached version of this Basilisp namespace exists and, if so,
         # load it and bypass the expensive compilation process below.
-        if os.getenv(_NO_CACHE_ENVVAR, None) == "True":
+        if os.getenv(_NO_CACHE_ENVVAR, None) == "true":
             self._exec_module(fullname, spec.loader_state, path_stats, module)
         else:
             try:
                 self._exec_cached_module(
                     fullname, spec.loader_state, path_stats, module
                 )
             except (EOFError, ImportError, IOError, OSError) as e:
```

### Comparing `basilisp-0.1.dev8/src/basilisp/util.py` & `basilisp-0.1.dev9/src/basilisp/util.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/walker.py` & `basilisp-0.1.dev9/src/basilisp/walker.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/set.lpy` & `basilisp-0.1.dev9/src/basilisp/set.lpy`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/vector.py` & `basilisp-0.1.dev9/src/basilisp/lang/vector.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/list.py` & `basilisp-0.1.dev9/src/basilisp/lang/list.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/util.py` & `basilisp-0.1.dev9/src/basilisp/lang/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import builtins
 import datetime
 import keyword
 import re
 import uuid
 from decimal import Decimal
 from fractions import Fraction
-from typing import Pattern, Match, Iterable
+from typing import Iterable, Match, Pattern
 
 import dateutil.parser as dateparser
 
 import basilisp.lang.atom as atom
 
 _MUNGE_REPLACEMENTS = {
     "+": "__PLUS__",
@@ -19,14 +19,15 @@
     ">": "__GT__",
     "<": "__LT__",
     "!": "__BANG__",
     "=": "__EQ__",
     "?": "__Q__",
     "\\": "__IDIV__",
     "&": "__AMP__",
+    "$": "__DOLLAR__",
 }
 
 
 def count(seq: Iterable) -> int:
     return sum([1 for _ in seq])
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/symbol.py` & `basilisp-0.1.dev9/src/basilisp/lang/symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,13 +48,13 @@
 
     def __eq__(self, other):
         if not isinstance(other, Symbol):
             return False
         return self._ns == other._ns and self._name == other._name
 
     def __hash__(self):
-        return hash(str(self))
+        return hash((self._ns, self._name))
 
 
 def symbol(name: str, ns: Optional[str] = None, meta=None) -> Symbol:
     """Create a new symbol."""
     return Symbol(name, ns=ns, meta=meta)
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/runtime.py` & `basilisp-0.1.dev9/src/basilisp/lang/runtime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,103 @@
 import contextlib
 import functools
 import importlib
+import inspect
 import itertools
 import logging
 import math
+import re
 import threading
 import types
 from fractions import Fraction
-from typing import Optional, Dict, Tuple
+from typing import Any, Callable, Dict, Iterable, Optional, Tuple, Union
 
 import basilisp.lang.associative as lassoc
 import basilisp.lang.collection as lcoll
 import basilisp.lang.deref as lderef
 import basilisp.lang.keyword as kw
 import basilisp.lang.list as llist
 import basilisp.lang.map as lmap
 import basilisp.lang.obj as lobj
 import basilisp.lang.seq as lseq
 import basilisp.lang.set as lset
 import basilisp.lang.symbol as sym
+import basilisp.lang.vector as vec
 from basilisp.lang import atom
 from basilisp.lang.typing import LispNumber
 from basilisp.logconfig import TRACE
 from basilisp.util import Maybe
 
 logger = logging.getLogger(__name__)
 
-_CORE_NS = "basilisp.core"
-_REPL_DEFAULT_NS = "user"
-_NS_VAR_NAME = "*ns*"
-_NS_VAR_NS = _CORE_NS
-_PYTHON_PACKAGE_NAME = "basilisp"
+# Public constants
+CORE_NS = "basilisp.core"
+NS_VAR_NAME = "*ns*"
+NS_VAR_NS = CORE_NS
+REPL_DEFAULT_NS = "user"
+
+# Private string constants
 _GENERATED_PYTHON_VAR_NAME = "*generated-python*"
 _PRINT_GENERATED_PY_VAR_NAME = "*print-generated-python*"
 _PRINT_DUP_VAR_NAME = "*print-dup*"
 _PRINT_LENGTH_VAR_NAME = "*print-length*"
 _PRINT_LEVEL_VAR_NAME = "*print-level*"
 _PRINT_META_VAR_NAME = "*print-meta*"
 _PRINT_READABLY_VAR_NAME = "*print-readably*"
 
-
+# Common meta keys
 _DYNAMIC_META_KEY = kw.keyword("dynamic")
 _PRIVATE_META_KEY = kw.keyword("private")
 _REDEF_META_KEY = kw.keyword("redef")
 
+# Special form values, used for resolving Vars
+_AWAIT = sym.symbol("await")
 _CATCH = sym.symbol("catch")
 _DEF = sym.symbol("def")
+_DEFTYPE = sym.symbol("deftype*")
 _DO = sym.symbol("do")
 _FINALLY = sym.symbol("finally")
 _FN = sym.symbol("fn*")
 _IF = sym.symbol("if")
 _IMPORT = sym.symbol("import*")
 _INTEROP_CALL = sym.symbol(".")
 _INTEROP_PROP = sym.symbol(".-")
 _LET = sym.symbol("let*")
 _LOOP = sym.symbol("loop*")
 _QUOTE = sym.symbol("quote")
 _RECUR = sym.symbol("recur")
+_SET_BANG = sym.symbol("set!")
 _THROW = sym.symbol("throw")
 _TRY = sym.symbol("try")
 _VAR = sym.symbol("var")
 _SPECIAL_FORMS = lset.s(
+    _AWAIT,
     _CATCH,
     _DEF,
+    _DEFTYPE,
     _DO,
     _FINALLY,
     _FN,
     _IF,
     _IMPORT,
     _INTEROP_CALL,
     _INTEROP_PROP,
     _LET,
     _LOOP,
     _QUOTE,
     _RECUR,
+    _SET_BANG,
     _THROW,
     _TRY,
     _VAR,
 )
 
+CompletionMatcher = Callable[[Tuple[sym.Symbol, Any]], bool]
+CompletionTrimmer = Callable[[Tuple[sym.Symbol, Any]], str]
+
 
 def _new_module(name: str, doc=None) -> types.ModuleType:
     """Create a new empty Basilisp Python module.
     Modules are created for each Namespace when it is created."""
     mod = types.ModuleType(name, doc=doc)
     mod.__loader__ = None
     mod.__package__ = None
@@ -276,14 +291,15 @@
     """
 
     DEFAULT_IMPORTS = atom.Atom(
         lset.set(
             map(
                 sym.symbol,
                 [
+                    "attr",
                     "builtins",
                     "io",
                     "operator",
                     "sys",
                     "basilisp.lang.atom",
                     "basilisp.lang.compiler",
                     "basilisp.lang.delay",
@@ -491,15 +507,15 @@
         return cls._NAMESPACES.deref()
 
     @staticmethod
     def __get_or_create(
         ns_cache: lmap.Map,
         name: sym.Symbol,
         module: types.ModuleType = None,
-        core_ns_name=_CORE_NS,
+        core_ns_name=CORE_NS,
     ) -> lmap.Map:
         """Private swap function used by `get_or_create` to atomically swap
         the new namespace map into the global cache."""
         ns = ns_cache.entry(name, None)
         if ns is not None:
             return ns_cache
         new_ns = Namespace(name, module=module)
@@ -536,14 +552,116 @@
             ns: Optional[Namespace] = oldval.entry(name, None)
             newval = oldval
             if ns is not None:
                 newval = oldval.discard(name)
             if cls._NAMESPACES.compare_and_set(oldval, newval):
                 return ns
 
+    # REPL Completion support
+
+    @staticmethod
+    def __completion_matcher(text: str) -> CompletionMatcher:
+        """Return a function which matches any symbol keys from map entries
+        against the given text."""
+
+        def is_match(entry: Tuple[sym.Symbol, Any]) -> bool:
+            return entry[0].name.startswith(text)
+
+        return is_match
+
+    def __complete_alias(
+        self, prefix: str, name_in_ns: Optional[str] = None
+    ) -> Iterable[str]:
+        """Return an iterable of possible completions matching the given
+        prefix from the list of aliased namespaces. If name_in_ns is given,
+        further attempt to refine the list to matching names in that namespace."""
+        candidates: Iterable[Tuple[sym.Symbol, Namespace]] = filter(
+            Namespace.__completion_matcher(prefix), self.aliases
+        )
+        if name_in_ns is not None:
+            for _, candidate_ns in candidates:
+                for match in candidate_ns.__complete_interns(
+                    name_in_ns, include_private_vars=False
+                ):
+                    yield f"{prefix}/{match}"
+        else:
+            for alias, _ in candidates:
+                yield f"{alias}/"
+
+    def __complete_imports_and_aliases(
+        self, prefix: str, name_in_module: Optional[str] = None
+    ) -> Iterable[str]:
+        """Return an iterable of possible completions matching the given
+        prefix from the list of imports and aliased imports. If name_in_module
+        is given, further attempt to refine the list to matching names in that
+        namespace."""
+        imports = self.imports
+        aliases = lmap.map(
+            {
+                alias: imports.entry(import_name)
+                for alias, import_name in self.import_aliases
+            }
+        )
+
+        candidates: Iterable[Tuple[sym.Symbol, types.ModuleType]] = filter(
+            Namespace.__completion_matcher(prefix), itertools.chain(aliases, imports)
+        )
+        if name_in_module is not None:
+            for _, module in candidates:
+                for name in module.__dict__:
+                    if name.startswith(name_in_module):
+                        yield f"{prefix}/{name}"
+        else:
+            for candidate_name, _ in candidates:
+                yield f"{candidate_name}/"
+
+    def __complete_interns(
+        self, value: str, include_private_vars: bool = True
+    ) -> Iterable[str]:
+        """Return an iterable of possible completions matching the given
+        prefix from the list of interned Vars."""
+        if include_private_vars:
+            is_match = Namespace.__completion_matcher(value)
+        else:
+            _is_match = Namespace.__completion_matcher(value)
+
+            def is_match(entry: Tuple[sym.Symbol, Var]) -> bool:
+                return _is_match(entry) and not entry[1].is_private
+
+        return map(lambda entry: f"{entry[0].name}", filter(is_match, self.interns))
+
+    def __complete_refers(self, value: str) -> Iterable[str]:
+        """Return an iterable of possible completions matching the given
+        prefix from the list of referred Vars."""
+        return map(
+            lambda entry: f"{entry[0].name}",
+            filter(Namespace.__completion_matcher(value), self.refers),
+        )
+
+    def complete(self, text: str) -> Iterable[str]:
+        """Return an iterable of possible completions for the given text in
+        this namespace."""
+        assert not text.startswith(":")
+
+        if "/" in text:
+            prefix, suffix = text.split("/", maxsplit=1)
+            results = itertools.chain(
+                self.__complete_alias(prefix, name_in_ns=suffix),
+                self.__complete_imports_and_aliases(prefix, name_in_module=suffix),
+            )
+        else:
+            results = itertools.chain(
+                self.__complete_alias(text),
+                self.__complete_imports_and_aliases(text),
+                self.__complete_interns(text),
+                self.__complete_refers(text),
+            )
+
+        return results
+
 
 ###################
 # Runtime Support #
 ###################
 
 
 def first(o):
@@ -660,14 +778,31 @@
     s = to_seq(last)
     if s is not None:
         final.extend(s)
 
     return f(*final)
 
 
+def apply_kw(f, args):
+    """Apply function f to the arguments provided.
+    The last argument must always be coercible to a Mapping. Intermediate
+    arguments are not modified.
+    For example:
+        (apply builtins/dict {:a 1} {:b 2})   ;=> #py {:a 1 :b 2}
+        (apply builtins/dict {:a 1} {:a 2})   ;=> #py {:a 2}"""
+    final = list(args[:-1])
+
+    try:
+        last = args[-1]
+    except TypeError as e:
+        logger.debug("Ignored %s: %s", type(e).__name__, e)
+
+    return f(*final, **last)
+
+
 __nth_sentinel = object()
 
 
 def nth(coll, i, notfound=__nth_sentinel):
     """Returns the ith element of coll (0-indexed), if it exists.
     None otherwise. If i is out of bounds, throws an IndexError unless
     notfound is specified."""
@@ -806,19 +941,124 @@
     try:
         return m[k]
     except (KeyError, IndexError, TypeError) as e:
         logger.debug("Ignored %s: %s", type(e).__name__, e)
         return default
 
 
+@functools.singledispatch
+def to_lisp(o, keywordize_keys: bool = True):
+    """Recursively convert Python collections into Lisp collections."""
+    if not isinstance(o, (dict, frozenset, list, set, tuple)):
+        return o
+    else:  # pragma: no cover
+        return _to_lisp_backup(o, keywordize_keys=keywordize_keys)
+
+
+def _to_lisp_backup(o, keywordize_keys: bool = True):  # pragma: no cover
+    if isinstance(o, (list, tuple)):
+        return _to_lisp_vec(o, keywordize_keys=keywordize_keys)
+    elif isinstance(o, dict):
+        return _to_lisp_map(o, keywordize_keys=keywordize_keys)
+    elif isinstance(o, (frozenset, set)):
+        return _to_lisp_set(o, keywordize_keys=keywordize_keys)
+    else:
+        return o
+
+
+@to_lisp.register(list)
+@to_lisp.register(tuple)
+def _to_lisp_vec(o: Union[list, tuple], keywordize_keys: bool = True) -> vec.Vector:
+    return vec.vector(
+        map(functools.partial(to_lisp, keywordize_keys=keywordize_keys), o)
+    )
+
+
+@to_lisp.register(dict)
+def _to_lisp_map(o: dict, keywordize_keys: bool = True) -> lmap.Map:
+    kvs = {}
+    for k, v in o.items():
+        if isinstance(k, str) and keywordize_keys:
+            processed_key = kw.keyword(k)
+        else:
+            processed_key = to_lisp(k, keywordize_keys=keywordize_keys)
+
+        kvs[processed_key] = to_lisp(v, keywordize_keys=keywordize_keys)
+    return lmap.map(kvs)
+
+
+@to_lisp.register(frozenset)
+@to_lisp.register(set)
+def _to_lisp_set(o: Union[frozenset, set], keywordize_keys: bool = True) -> lset.Set:
+    return lset.set(map(functools.partial(to_lisp, keywordize_keys=keywordize_keys), o))
+
+
+def _kw_name(kw: kw.Keyword) -> str:
+    return kw.name
+
+
+@functools.singledispatch
+def to_py(o, keyword_fn: Callable[[kw.Keyword], Any] = _kw_name):
+    """Recursively convert Lisp collections into Python collections."""
+    if isinstance(o, lseq.Seq):
+        return _to_py_list(o, keyword_fn=keyword_fn)
+    elif not isinstance(o, (llist.List, lmap.Map, lset.Set, vec.Vector)):
+        return o
+    else:  # pragma: no cover
+        return _to_py_backup(o, keyword_fn=keyword_fn)
+
+
+def _to_py_backup(
+    o, keyword_fn: Callable[[kw.Keyword], Any] = _kw_name
+):  # pragma: no cover
+    if isinstance(o, (llist.List, vec.Vector)):
+        return _to_py_list(o, keyword_fn=keyword_fn)
+    elif isinstance(o, lmap.Map):
+        return _to_py_map(o, keyword_fn=keyword_fn)
+    elif isinstance(o, lset.Set):
+        return _to_py_set(o, keyword_fn=keyword_fn)
+    else:
+        return o
+
+
+@to_py.register(kw.Keyword)
+def _to_py_kw(o: kw.Keyword, keyword_fn: Callable[[kw.Keyword], Any] = _kw_name) -> Any:
+    return keyword_fn(o)
+
+
+@to_py.register(llist.List)
+@to_py.register(lseq.Seq)
+@to_py.register(vec.Vector)
+def _to_py_list(
+    o: Union[llist.List, lseq.Seq, vec.Vector],
+    keyword_fn: Callable[[kw.Keyword], Any] = _kw_name,
+) -> list:
+    return list(map(functools.partial(to_py, keyword_fn=keyword_fn), o))
+
+
+@to_py.register(lmap.Map)
+def _to_py_map(o: lmap.Map, keyword_fn: Callable[[kw.Keyword], Any] = _kw_name) -> dict:
+    return {
+        to_py(entry.key, keyword_fn=keyword_fn): to_py(
+            entry.value, keyword_fn=keyword_fn
+        )
+        for entry in o
+    }
+
+
+@to_py.register(lset.Set)
+def _to_py_set(o: lset.Set, keyword_fn: Callable[[kw.Keyword], Any] = _kw_name) -> set:
+    return set(to_py(e, keyword_fn=keyword_fn) for e in o)
+
+
 def lrepr(o, human_readable: bool = False) -> str:
     """Produce a string representation of an object. If human_readable is False,
     the string representation of Lisp objects is something that can be read back
     in by the reader as the same object."""
-    core_ns = Namespace.get(sym.symbol(_CORE_NS))
+    core_ns = Namespace.get(sym.symbol(CORE_NS))
     assert core_ns is not None
     return lobj.lrepr(
         o,
         human_readable=human_readable,
         print_dup=core_ns.find(sym.symbol(_PRINT_DUP_VAR_NAME)).value,  # type: ignore
         print_length=core_ns.find(  # type: ignore
             sym.symbol(_PRINT_LENGTH_VAR_NAME)
@@ -834,14 +1074,36 @@
 
 
 def lstr(o) -> str:
     """Produce a human readable string representation of an object."""
     return lrepr(o, human_readable=True)
 
 
+__NOT_COMPLETEABLE = re.compile(r"^[0-9].*")
+
+
+def repl_complete(text: str, state: int) -> Optional[str]:
+    """Completer function for Python's readline/libedit implementation."""
+    # Can't complete Keywords, Numerals
+    if __NOT_COMPLETEABLE.match(text):
+        return None
+    elif text.startswith(":"):
+        completions = kw.complete(text)
+    else:
+        ns = get_current_ns()
+        completions = ns.complete(text)
+
+    return list(completions)[state] if completions is not None else None
+
+
+####################
+# Compiler Support #
+####################
+
+
 def _collect_args(args) -> lseq.Seq:
     """Collect Python starred arguments into a Basilisp list."""
     if isinstance(args, tuple):
         return llist.list(args)
     raise TypeError("Python variadic arguments should always be a tuple")
 
 
@@ -888,33 +1150,82 @@
                 kwargs = ret.kwargs
                 continue
             return ret
 
     return trampoline
 
 
+def _with_attrs(**kwargs):
+    """Decorator to set attributes on a function. Returns the original
+    function after setting the attributes named by the keyword arguments."""
+
+    def decorator(f):
+        for k, v in kwargs.items():
+            setattr(f, k, v)
+        return f
+
+    return decorator
+
+
+def _fn_with_meta(f, meta: Optional[lmap.Map]):
+    """Return a new function with the given meta. If the function f already
+    has a meta map, then merge the """
+
+    if not isinstance(meta, lmap.Map):
+        raise TypeError("meta must be a map")
+
+    if inspect.iscoroutinefunction(f):
+
+        @functools.wraps(f)
+        async def wrapped_f(*args, **kwargs):
+            return await f(*args, **kwargs)
+
+    else:
+
+        @functools.wraps(f)  # type: ignore
+        def wrapped_f(*args, **kwargs):
+            return f(*args, **kwargs)
+
+    wrapped_f.meta = (  # type: ignore
+        f.meta.update(meta)
+        if hasattr(f, "meta") and isinstance(f.meta, lmap.Map)
+        else meta
+    )
+    wrapped_f.with_meta = partial(_fn_with_meta, wrapped_f)  # type: ignore
+    return wrapped_f
+
+
+def _basilisp_fn(f):
+    """Create a Basilisp function, setting meta and supplying a with_meta
+    method implementation."""
+    assert not hasattr(f, "meta")
+    f.meta = None
+    f.with_meta = partial(_fn_with_meta, f)
+    return f
+
+
 #########################
 # Bootstrap the Runtime #
 #########################
 
 
-def init_ns_var(which_ns: str = _CORE_NS, ns_var_name: str = _NS_VAR_NAME) -> Var:
+def init_ns_var(which_ns: str = CORE_NS, ns_var_name: str = NS_VAR_NAME) -> Var:
     """Initialize the dynamic `*ns*` variable in the Namespace `which_ns`."""
     core_sym = sym.Symbol(which_ns)
     core_ns = Namespace.get_or_create(core_sym)
     ns_var = Var.intern(core_sym, sym.Symbol(ns_var_name), core_ns, dynamic=True)
     logger.debug(f"Created namespace variable {sym.symbol(ns_var_name, ns=which_ns)}")
     return ns_var
 
 
 def set_current_ns(
     ns_name: str,
     module: types.ModuleType = None,
-    ns_var_name: str = _NS_VAR_NAME,
-    ns_var_ns: str = _NS_VAR_NS,
+    ns_var_name: str = NS_VAR_NAME,
+    ns_var_ns: str = NS_VAR_NS,
 ) -> Var:
     """Set the value of the dynamic variable `*ns*` in the current thread."""
     symbol = sym.Symbol(ns_name)
     ns = Namespace.get_or_create(symbol, module=module)
     ns_var_sym = sym.Symbol(ns_var_name, ns=ns_var_ns)
     ns_var = Maybe(Var.find(ns_var_sym)).or_else_raise(
         lambda: RuntimeException(
@@ -926,16 +1237,16 @@
     return ns_var
 
 
 @contextlib.contextmanager
 def ns_bindings(
     ns_name: str,
     module: types.ModuleType = None,
-    ns_var_name: str = _NS_VAR_NAME,
-    ns_var_ns: str = _NS_VAR_NS,
+    ns_var_name: str = NS_VAR_NAME,
+    ns_var_ns: str = NS_VAR_NS,
 ):
     """Context manager for temporarily changing the value of basilisp.core/*ns*."""
     symbol = sym.Symbol(ns_name)
     ns = Namespace.get_or_create(symbol, module=module)
     ns_var_sym = sym.Symbol(ns_var_name, ns=ns_var_ns)
     ns_var = Maybe(Var.find(ns_var_sym)).or_else_raise(
         lambda: RuntimeException(
@@ -949,15 +1260,15 @@
         yield ns_var.value
     finally:
         ns_var.pop_bindings()
         logger.debug(f"Reset bindings for {ns_var_sym} to {ns_var.value}")
 
 
 @contextlib.contextmanager
-def remove_ns_bindings(ns_var_name: str = _NS_VAR_NAME, ns_var_ns: str = _NS_VAR_NS):
+def remove_ns_bindings(ns_var_name: str = NS_VAR_NAME, ns_var_ns: str = NS_VAR_NS):
     """Context manager to pop the most recent bindings for basilisp.core/*ns* after
     completion of the code under management."""
     ns_var_sym = sym.Symbol(ns_var_name, ns=ns_var_ns)
     ns_var = Maybe(Var.find(ns_var_sym)).or_else_raise(
         lambda: RuntimeException(
             f"Dynamic Var {sym.Symbol(ns_var_name, ns=ns_var_ns)} not bound!"
         )
@@ -966,15 +1277,15 @@
         yield
     finally:
         ns_var.pop_bindings()
         logger.debug(f"Reset bindings for {ns_var_sym} to {ns_var.value}")
 
 
 def get_current_ns(
-    ns_var_name: str = _NS_VAR_NAME, ns_var_ns: str = _NS_VAR_NS
+    ns_var_name: str = NS_VAR_NAME, ns_var_ns: str = NS_VAR_NS
 ) -> Namespace:
     """Get the value of the dynamic variable `*ns*` in the current thread."""
     ns_sym = sym.Symbol(ns_var_name, ns=ns_var_ns)
     ns: Namespace = Maybe(Var.find(ns_sym)).map(lambda v: v.value).or_else_raise(
         lambda: RuntimeException(f"Dynamic Var {ns_sym} not bound!")
     )
     return ns
@@ -1024,26 +1335,26 @@
             meta=lmap.map({_PRIVATE_META_KEY: True}),
         )
     )
     v.value = v.value + generated_python
 
 
 def print_generated_python(
-    var_name: str = _PRINT_GENERATED_PY_VAR_NAME, core_ns_name: str = _CORE_NS
+    var_name: str = _PRINT_GENERATED_PY_VAR_NAME, core_ns_name: str = CORE_NS
 ) -> bool:
     """Return the value of the `*print-generated-python*` dynamic variable."""
     ns_sym = sym.Symbol(var_name, ns=core_ns_name)
     return (
         Maybe(Var.find(ns_sym))
         .map(lambda v: v.value)
         .or_else_raise(lambda: RuntimeException(f"Dynamic Var {ns_sym} not bound!"))
     )
 
 
-def bootstrap(ns_var_name: str = _NS_VAR_NAME, core_ns_name: str = _CORE_NS) -> None:
+def bootstrap(ns_var_name: str = NS_VAR_NAME, core_ns_name: str = CORE_NS) -> None:
     """Bootstrap the environment with functions that are are difficult to
     express with the very minimal lisp environment."""
     core_ns_sym = sym.symbol(core_ns_name)
     ns_var_sym = sym.symbol(ns_var_name, ns=core_ns_name)
     __NS = Maybe(Var.find(ns_var_sym)).or_else_raise(
         lambda: RuntimeException(f"Dynamic Var {ns_var_sym} not bound!")
     )
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/map.py` & `basilisp-0.1.dev9/src/basilisp/lang/seq.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,230 +1,227 @@
-from builtins import map as pymap
-from collections import Sequence
-from typing import Optional  # noqa # pylint: disable=unused-import
-
-from functional import seq
-from pyrsistent import pmap, PMap
-
-import basilisp.lang.obj as lobj
-import basilisp.lang.vector as vec
-from basilisp.lang.associative import Associative
-from basilisp.lang.collection import Collection
+import itertools
+from abc import ABC, abstractmethod
+from typing import Iterator, Optional, TypeVar, Iterable, Any, Callable
+
 from basilisp.lang.meta import Meta
-from basilisp.lang.obj import LispObject, lrepr
-from basilisp.lang.seq import Seqable, sequence, Seq
-from basilisp.util import partition
+from basilisp.lang.obj import LispObject
+from basilisp.util import Maybe
 
+T = TypeVar("T")
 
-class MapEntry:
-    __slots__ = ("_inner",)
 
-    def __init__(self, wrapped: vec.Vector) -> None:
-        try:
-            if not len(wrapped) == 2:
-                raise ValueError("Vector arg to map conj must be a pair")
-        except TypeError as e:
-            raise TypeError(f"Cannot make map entry from {type(wrapped)}") from e
+class Seq(LispObject, Iterable[T]):
+    __slots__ = ()
 
-        self._inner = wrapped
+    def _lrepr(self, **kwargs):
+        return LispObject.seq_lrepr(iter(self), "(", ")", **kwargs)
 
-    def __repr__(self):
-        return lrepr(self._inner)
+    @property
+    @abstractmethod
+    def is_empty(self) -> bool:
+        raise NotImplementedError()
 
-    def __eq__(self, other):
-        return self._inner == other
+    @property
+    @abstractmethod
+    def first(self) -> Optional[T]:
+        raise NotImplementedError()
 
-    def __getitem__(self, item):
-        return self._inner[item]
+    @property
+    @abstractmethod
+    def rest(self) -> "Seq[T]":
+        raise NotImplementedError()
+
+    @abstractmethod
+    def cons(self, elem):
+        raise NotImplementedError()
 
-    def __hash__(self):
-        return hash(self._inner)
+    def __eq__(self, other):
+        sentinel = object()
+        for e1, e2 in itertools.zip_longest(self, other, fillvalue=sentinel):
+            if bool(e1 is sentinel) or bool(e2 is sentinel):
+                return False
+            if e1 != e2:
+                return False
+        return True
 
     def __iter__(self):
-        yield from self._inner
+        o = self
+        while o:
+            yield o.first
+            o = o.rest
+
+
+class Seqable(ABC, Iterable[T]):
+    __slots__ = ()
+
+    def seq(self) -> Seq[T]:
+        raise NotImplementedError()
 
-    def __len__(self):
-        return len(self._inner)
+
+class _EmptySequence(Seq[T]):
+    def __repr__(self):
+        return "()"
+
+    def __bool__(self):
+        return False
+
+    @property
+    def is_empty(self) -> bool:
+        return True
 
     @property
-    def key(self):
-        return self[0]
+    def first(self) -> Optional[T]:
+        return None
 
     @property
-    def value(self):
-        return self[1]
+    def rest(self) -> Seq[T]:
+        return self
 
-    @staticmethod
-    def of(k, v) -> "MapEntry":
-        return MapEntry(vec.v(k, v))
+    def cons(self, elem):
+        return Cons(elem, self)
 
-    @staticmethod
-    def from_vec(v: Sequence) -> "MapEntry":
-        return MapEntry(vec.vector(v))
 
+EMPTY: Seq = _EmptySequence()
 
-class Map(Associative, Collection, LispObject, Meta, Seqable):
-    """Basilisp Map. Delegates internally to a pyrsistent.PMap object.
-    Do not instantiate directly. Instead use the m() and map() factory
-    methods below."""
 
-    __slots__ = ("_inner", "_meta")
+class Cons(Seq, Meta):
+    __slots__ = ("_first", "_rest", "_meta")
 
-    def __init__(self, wrapped: PMap, meta=None) -> None:
-        self._inner = wrapped
+    def __init__(self, first=None, seq: Optional[Seq[Any]] = None, meta=None) -> None:
+        self._first = first
+        self._rest = Maybe(seq).or_else_get(EMPTY)
         self._meta = meta
 
-    def __call__(self, key, default=None):
-        return self._inner.get(key, default)
+    @property
+    def is_empty(self) -> bool:
+        return False
+
+    @property
+    def first(self) -> Optional[Any]:
+        return self._first
 
-    def __contains__(self, item):
-        return item in self._inner
+    @property
+    def rest(self) -> Seq[Any]:
+        return self._rest
 
-    def __eq__(self, other):
-        return self._inner == other
+    def cons(self, elem) -> "Cons":
+        return Cons(elem, self)
 
-    def __getattr__(self, item):
-        return getattr(self._inner, item)
+    @property
+    def meta(self):
+        return self._meta
 
-    def __getitem__(self, item):
-        return self._inner[item]
+    def with_meta(self, meta) -> "Cons":
+        new_meta = meta if self._meta is None else self._meta.update(meta)
+        return Cons(first=self._first, seq=self._rest, meta=new_meta)
 
-    def __hash__(self):
-        return hash(self._inner)
 
-    def __iter__(self):
-        for k, v in self._inner.iteritems():
-            yield MapEntry.of(k, v)
+class _Sequence(Seq[T]):
+    """Sequences are a thin wrapper over Python Iterable values so they can
+    satisfy the Basilisp `Seq` interface.
 
-    def __len__(self):
-        return len(self._inner)
+    Sequences are singly linked lists which lazily traverse the input Iterable.
 
-    def _lrepr(self, **kwargs):
-        print_level = kwargs["print_level"]
-        if isinstance(print_level, int) and print_level < 1:
-            return lobj.SURPASSED_PRINT_LEVEL
+    Do not directly instantiate a Sequence. Instead use the `sequence` function
+    below."""
 
-        kwargs = LispObject._process_kwargs(**kwargs)
+    __slots__ = ("_first", "_seq", "_rest")
 
-        def entry_reprs():
-            for k, v in self._inner.iteritems():
-                yield "{k} {v}".format(k=lrepr(k, **kwargs), v=lrepr(v, **kwargs))
+    def __init__(self, s: Iterator, first: T) -> None:
+        self._seq = s  # pylint:disable=assigning-non-slot
+        self._first = first  # pylint:disable=assigning-non-slot
+        self._rest: Optional[Seq] = None  # pylint:disable=assigning-non-slot
 
-        trailer = []
-        print_dup = kwargs["print_dup"]
-        print_length = kwargs["print_length"]
-        if not print_dup and isinstance(print_length, int):
-            items = seq(entry_reprs()).take(print_length + 1).to_list()
-            if len(items) > print_length:
-                items.pop()
-                trailer.append(lobj.SURPASSED_PRINT_LENGTH)
-        else:
-            items = list(entry_reprs())
+    @property
+    def is_empty(self) -> bool:
+        return False
 
-        seq_lrepr = lobj.PRINT_SEPARATOR.join(items + trailer)
+    @property
+    def first(self) -> Optional[T]:
+        return self._first
 
-        print_meta = kwargs["print_meta"]
-        if print_meta and self._meta:
-            return f"^{lrepr(self._meta, **kwargs)} {{{seq_lrepr}}}"
+    @property
+    def rest(self) -> "Seq[T]":
+        if self._rest:
+            return self._rest
 
-        return f"{{{seq_lrepr}}}"
+        try:
+            n = next(self._seq)
+            self._rest = _Sequence(self._seq, n)  # pylint:disable=assigning-non-slot
+        except StopIteration:
+            self._rest = EMPTY  # pylint:disable=assigning-non-slot
 
-    def items(self):
-        return self._inner.items()
+        return self._rest
 
-    def keys(self):
-        return self._inner.keys()
+    def cons(self, elem):
+        return Cons(elem, self)
 
-    def values(self):
-        return self._inner.values()
 
-    @property
-    def meta(self) -> "Optional[Map]":
-        return self._meta
+class LazySeq(Seq[T]):
+    """LazySeqs are wrappers for delaying sequence computation. Create a LazySeq
+    with a function that can either return None or a Seq. If a Seq is returned,
+    the LazySeq is a proxy to that Seq."""
 
-    def with_meta(self, meta: "Map") -> "Map":
-        new_meta = meta if self._meta is None else self._meta.update(meta)
-        return Map(self._inner, meta=new_meta)
+    __slots__ = ("_gen", "_realized", "_seq")
+
+    def __init__(self, gen: Callable[[], Optional[Seq]]) -> None:
+        self._gen = gen  # pylint:disable=assigning-non-slot
+        self._realized = False  # pylint:disable=assigning-non-slot
+        self._seq: Optional[Seq] = None  # pylint:disable=assigning-non-slot
 
-    def assoc(self, *kvs) -> "Map":
-        m = self._inner.evolver()
-        for k, v in partition(kvs, 2):
-            m[k] = v
-        return Map(m.persistent())
+    def _realize(self):
+        if not self._realized:
+            self._seq = self._gen()  # pylint:disable=assigning-non-slot
+            self._realized = True  # pylint:disable=assigning-non-slot
 
-    def contains(self, k):
-        if k in self._inner:
+    @property
+    def is_empty(self) -> bool:
+        if not self._realized:
+            self._realize()
+            return self.is_empty
+        if self._seq is None or self._seq.is_empty:
             return True
         return False
 
-    def dissoc(self, *ks) -> "Map":
-        return self.discard(*ks)
-
-    def discard(self, *ks) -> "Map":
-        m = self._inner.evolver()
-        for k in ks:
-            try:
-                del m[k]
-            except KeyError:
-                pass
-        return Map(m.persistent())
-
-    def entry(self, k, default=None):
-        return self._inner.get(k, default)
-
-    def update(self, *maps) -> "Map":
-        m: PMap = self._inner.update(*maps)
-        return Map(m)
-
-    def update_with(self, merge_fn, *maps) -> "Map":
-        m: PMap = self._inner.update_with(merge_fn, *maps)
-        return Map(m)
+    @property
+    def first(self) -> Optional[T]:
+        if not self._realized:
+            self._realize()
+        try:
+            return self._seq.first  # type: ignore
+        except AttributeError:
+            return None
 
-    def cons(self, *elems) -> "Map":
-        e = self._inner.evolver()
+    @property
+    def rest(self) -> "Seq[T]":
+        if not self._realized:
+            self._realize()
         try:
-            for elem in elems:
-                if isinstance(elem, Map):
-                    for entry in elem:
-                        e.set(entry.key, entry.value)
-                elif isinstance(elem, dict):
-                    for k, v in elem.items():
-                        e.set(k, v)
-                elif isinstance(elem, MapEntry):
-                    e.set(elem.key, elem.value)
-                else:
-                    entry = MapEntry.from_vec(elem)
-                    e.set(entry.key, entry.value)
-            return Map(e.persistent(), meta=self.meta)
-        except (TypeError, ValueError):
-            raise ValueError(
-                "Argument to map conj must be another Map or castable to MapEntry"
-            )
-
-    @staticmethod
-    def empty() -> "Map":
-        return m()
-
-    def seq(self) -> Seq:
-        return sequence(self)
-
-
-def map(kvs, meta=None) -> Map:  # pylint:disable=redefined-builtin
-    """Creates a new map."""
-    return Map(pmap(initial=kvs), meta=meta)
-
-
-def m(**kvs) -> Map:
-    """Creates a new map from keyword arguments."""
-    return Map(pmap(initial=kvs))
-
-
-def from_entries(entries):
-    m = pmap().evolver()
-    for entry in entries:
-        m.set(entry.key, entry.value)
-    return Map(m.persistent())
-
-
-def hash_map(*pairs) -> Map:
-    entries = pymap(lambda v: MapEntry.of(v[0], v[1]), partition(pairs, 2))
-    return from_entries(entries)
+            return self._seq.rest  # type: ignore
+        except AttributeError:
+            return EMPTY
+
+    def cons(self, elem):
+        return Cons(elem, self)
+
+    @property
+    def is_realized(self):
+        return self._realized
+
+    def __iter__(self):
+        o = self
+        while o:
+            first = o.first
+            if isinstance(o, LazySeq):
+                if o.is_empty:
+                    return
+            yield first
+            o = o.rest
+
+
+def sequence(s: Iterable) -> Seq[Any]:
+    """Create a Sequence from Iterable s."""
+    try:
+        i = iter(s)
+        return _Sequence(i, next(i))
+    except StopIteration:
+        return EMPTY
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/reader.py` & `basilisp-0.1.dev9/src/basilisp/lang/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import basilisp.lang.map as lmap
 import basilisp.lang.meta as lmeta
 import basilisp.lang.set as lset
 import basilisp.lang.symbol as symbol
 import basilisp.lang.util as langutil
 import basilisp.lang.vector as vector
 import basilisp.walker as walk
-from basilisp.lang.typing import LispForm, IterableLispForm
+from basilisp.lang.typing import LispForm, IterableLispForm, ReaderForm
 from basilisp.util import Maybe
 
 ns_name_chars = re.compile(r"\w|-|\+|\*|\?|/|\=|\\|!|&|%|>|<|\$|\.")
 alphanumeric_chars = re.compile(r"\w")
 begin_num_chars = re.compile(r"[0-9\-]")
 num_chars = re.compile("[0-9]")
 whitespace_chars = re.compile(r"[\s,]")
@@ -77,15 +77,15 @@
 
 class Comment:
     pass
 
 
 COMMENT = Comment()
 
-LispReaderForm = Union[LispForm, Comment]
+LispReaderForm = Union[ReaderForm, Comment]
 
 
 class SyntaxError(Exception):  # pylint:disable=redefined-builtin
     pass
 
 
 class StreamReader:
@@ -158,14 +158,41 @@
         else:
             c = self._stream.read(1)
             self._update_loc(c)
             self._buffer.append(c)
         return self.peek()
 
 
+@functools.singledispatch
+def _py_from_lisp(
+    form: Union[llist.List, lmap.Map, lset.Set, vector.Vector]
+) -> ReaderForm:
+    raise SyntaxError(f"Unrecognized Python type: {type(form)}")
+
+
+@_py_from_lisp.register(llist.List)
+def _py_tuple_from_list(form: llist.List) -> tuple:
+    return tuple(form)
+
+
+@_py_from_lisp.register(lmap.Map)
+def _py_dict_from_map(form: lmap.Map) -> dict:
+    return dict(form)
+
+
+@_py_from_lisp.register(lset.Set)
+def _py_set_from_set(form: lset.Set) -> set:
+    return set(form)
+
+
+@_py_from_lisp.register(vector.Vector)
+def _py_list_from_vec(form: vector.Vector) -> list:
+    return list(form)
+
+
 def _inst_from_str(inst_str: str) -> datetime:
     try:
         return langutil.inst_from_str(inst_str)
     except (ValueError, OverflowError):
         raise SyntaxError(f"Unrecognized date/time syntax: {inst_str}")
 
 
@@ -174,15 +201,19 @@
         return langutil.uuid_from_str(uuid_str)
     except (ValueError, TypeError):
         raise SyntaxError(f"Unrecognized UUID format: {uuid_str}")
 
 
 class ReaderContext:
     _DATA_READERS = lmap.map(
-        {symbol.symbol("inst"): _inst_from_str, symbol.symbol("uuid"): _uuid_from_str}
+        {
+            symbol.symbol("inst"): _inst_from_str,
+            symbol.symbol("py"): _py_from_lisp,
+            symbol.symbol("uuid"): _uuid_from_str,
+        }
     )
 
     __slots__ = (
         "_data_readers",
         "_reader",
         "_resolve",
         "_in_anon_fn",
@@ -683,23 +714,23 @@
     """Read a quoted form from the input stream."""
     start = ctx.reader.advance()
     assert start == "'"
     next_form = _read_next_consuming_comment(ctx)
     return llist.l(_QUOTE, next_form)
 
 
-def _is_unquote(form: LispForm) -> bool:
+def _is_unquote(form: ReaderForm) -> bool:
     """Return True if this form is unquote."""
     try:
         return form.first == _UNQUOTE  # type: ignore
     except AttributeError:
         return False
 
 
-def _is_unquote_splicing(form: LispForm) -> bool:
+def _is_unquote_splicing(form: ReaderForm) -> bool:
     """Return True if this form is unquote-splicing."""
     try:
         return form.first == _UNQUOTE_SPLICING  # type: ignore
     except AttributeError:
         return False
 
 
@@ -726,15 +757,15 @@
             expanded.append(elem[1])
         else:
             expanded.append(llist.l(_LIST, _process_syntax_quoted_form(ctx, elem)))
 
     return expanded
 
 
-def _process_syntax_quoted_form(ctx: ReaderContext, form: LispForm) -> LispForm:
+def _process_syntax_quoted_form(ctx: ReaderContext, form: ReaderForm) -> ReaderForm:
     """Post-process syntax quoted forms to generate forms that can be assembled
     into the correct types at runtime.
 
     Lists are turned into:
         (basilisp.core/seq
          (basilisp.core/concat [& rest]))
 
@@ -781,15 +812,15 @@
                 ctx.gensym_env[form.name] = genned
                 return llist.l(_QUOTE, genned)
         return llist.l(_QUOTE, form)
     else:
         return form
 
 
-def _read_syntax_quoted(ctx: ReaderContext) -> LispForm:
+def _read_syntax_quoted(ctx: ReaderContext) -> ReaderForm:
     """Read a syntax-quote and set the syntax-quoting state in the reader."""
     start = ctx.reader.advance()
     assert start == "`"
 
     with ctx.syntax_quoted():
         return _process_syntax_quoted_form(ctx, _read_next_consuming_comment(ctx))
 
@@ -937,15 +968,15 @@
             reader.advance()
             return _read_next(ctx)
         if token == "":
             return ctx.eof
         reader.advance()
 
 
-def _read_next_consuming_comment(ctx: ReaderContext) -> LispForm:
+def _read_next_consuming_comment(ctx: ReaderContext) -> ReaderForm:
     """Read the next full form from the input stream, consuming any
     reader comments completely."""
     while True:
         v = _read_next(ctx)
         if v is ctx.eof:
             return ctx.eof
         if v is COMMENT or isinstance(v, Comment):
@@ -998,15 +1029,15 @@
 
 def read(
     stream,
     resolver: Resolver = None,
     data_readers: DataReaders = None,
     eof: Any = EOF,
     is_eof_error: bool = False,
-) -> Iterable[LispForm]:
+) -> Iterable[ReaderForm]:
     """Read the contents of a stream as a Lisp expression.
 
     Callers may optionally specify a namespace resolver, which will be used
     to adjudicate the fully-qualified name of symbols appearing inside of
     a syntax quote.
 
     Callers may optionally specify a map of custom data readers that will
@@ -1031,15 +1062,15 @@
 
 def read_str(
     s: str,
     resolver: Resolver = None,
     data_readers: DataReaders = None,
     eof: Any = None,
     is_eof_error: bool = False,
-) -> Iterable[LispForm]:
+) -> Iterable[ReaderForm]:
     """Read the contents of a string as a Lisp expression.
 
     Keyword arguments to this function have the same meanings as those of
     basilisp.lang.reader.read."""
     with io.StringIO(s) as buf:
         yield from read(
             buf,
@@ -1052,15 +1083,15 @@
 
 def read_file(
     filename: str,
     resolver: Resolver = None,
     data_readers: DataReaders = None,
     eof: Any = None,
     is_eof_error: bool = False,
-) -> Iterable[LispForm]:
+) -> Iterable[ReaderForm]:
     """Read the contents of a file as a Lisp expression.
 
     Keyword arguments to this function have the same meanings as those of
     basilisp.lang.reader.read."""
     with open(filename) as f:
         yield from read(
             f,
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/keyword.py` & `basilisp-0.1.dev9/src/basilisp/lang/keyword.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional
+from typing import Optional, Iterable
 
 from pyrsistent import pmap, PMap
 
 import basilisp.lang.associative as lassoc
 import basilisp.lang.atom as atom
 from basilisp.lang.obj import LispObject
 
-__INTERN = atom.Atom(pmap())
+__INTERN: atom.Atom["PMap[int, Keyword]"] = atom.Atom(pmap())
 
 
 class Keyword(LispObject):
     __slots__ = ("_name", "_ns")
 
     def __init__(self, name: str, ns: Optional[str] = None) -> None:
         self._name = name
@@ -29,31 +29,60 @@
             return ":{ns}/{name}".format(ns=self._ns, name=self._name)
         return ":{name}".format(name=self._name)
 
     def __eq__(self, other):
         return self is other
 
     def __hash__(self):
-        return hash(str(self))
+        return hash((self._name, self._ns))
 
     def __call__(self, m: lassoc.Associative, default=None):
         try:
             return m.entry(self, default)
         except AttributeError:
             return None
 
 
-def __get_or_create(kw_cache: PMap, h: int, name: str, ns: Optional[str]) -> PMap:
+def complete(
+    text: str, kw_cache: atom.Atom["PMap[int, Keyword]"] = __INTERN
+) -> Iterable[str]:
+    """Return an iterable of possible completions for the given text."""
+    assert text.startswith(":")
+    interns = kw_cache.deref()
+    text = text[1:]
+
+    if "/" in text:
+        prefix, suffix = text.split("/", maxsplit=1)
+        results = filter(
+            lambda kw: (kw.ns is not None and kw.ns == prefix)
+            and kw.name.startswith(suffix),
+            interns.itervalues(),
+        )
+    else:
+        results = filter(
+            lambda kw: kw.name.startswith(text)
+            or (kw.ns is not None and kw.ns.startswith(text)),
+            interns.itervalues(),
+        )
+
+    return map(str, results)
+
+
+def __get_or_create(
+    kw_cache: "PMap[int, Keyword]", h: int, name: str, ns: Optional[str]
+) -> PMap:
     """Private swap function used to either get the interned keyword
     instance from the input string."""
     if h in kw_cache:
         return kw_cache
     kw = Keyword(name, ns=ns)
     return kw_cache.set(h, kw)
 
 
 def keyword(
-    name: str, ns: Optional[str] = None, kw_cache: atom.Atom = __INTERN
+    name: str,
+    ns: Optional[str] = None,
+    kw_cache: atom.Atom["PMap[int, Keyword]"] = __INTERN,
 ) -> Keyword:
     """Create a new keyword."""
     h = hash((name, ns))
     return kw_cache.swap(__get_or_create, h, name, ns)[h]
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/delay.py` & `basilisp-0.1.dev9/src/basilisp/lang/delay.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/typing.py` & `basilisp-0.1.dev9/src/basilisp/lang/typing.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from decimal import Decimal
 from fractions import Fraction
 from typing import Union, Pattern
 
 import basilisp.lang.keyword as kw
 import basilisp.lang.list as llist
 import basilisp.lang.map as lmap
+import basilisp.lang.seq as lseq
 import basilisp.lang.set as lset
 import basilisp.lang.symbol as sym
 import basilisp.lang.vector as vec
 
+IterableLispForm = Union[llist.List, lmap.Map, lset.Set, vec.Vector]
 LispNumber = Union[int, float, Fraction]
 LispForm = Union[
     bool,
     complex,
     datetime,
     Decimal,
     int,
@@ -27,8 +29,10 @@
     Pattern,
     lset.Set,
     str,
     sym.Symbol,
     vec.Vector,
     uuid.UUID,
 ]
-IterableLispForm = Union[llist.List, lmap.Map, lset.Set, vec.Vector]
+PyCollectionForm = Union[dict, list, set, tuple]
+ReaderForm = Union[LispForm, lseq.Seq, PyCollectionForm]
+SpecialForm = Union[llist.List, lseq.Seq]
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/multifn.py` & `basilisp-0.1.dev9/src/basilisp/lang/multifn.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/set.py` & `basilisp-0.1.dev9/src/basilisp/lang/set.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/atom.py` & `basilisp-0.1.dev9/src/basilisp/lang/atom.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/exception.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/exception.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/constants.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import basilisp.lang.keyword as kw
 import basilisp.lang.symbol as sym
 
 
 class SpecialForm:
+    AWAIT = sym.symbol("await")
     CATCH = sym.symbol("catch")
     DEF = sym.symbol("def")
+    DEFTYPE = sym.symbol("deftype*")
     DO = sym.symbol("do")
     FINALLY = sym.symbol("finally")
     FN = sym.symbol("fn*")
     IF = sym.symbol("if")
     IMPORT = sym.symbol("import*")
     INTEROP_CALL = sym.symbol(".")
     INTEROP_PROP = sym.symbol(".-")
@@ -22,19 +24,22 @@
     VAR = sym.symbol("var")
 
 
 AMPERSAND = sym.symbol("&")
 
 DEFAULT_COMPILER_FILE_PATH = "NO_SOURCE_PATH"
 
+SYM_ASYNC_META_KEY = kw.keyword("async")
 SYM_DYNAMIC_META_KEY = kw.keyword("dynamic")
 SYM_MACRO_META_KEY = kw.keyword("macro")
+SYM_MUTABLE_META_KEY = kw.keyword("mutable")
 SYM_NO_WARN_ON_REDEF_META_KEY = kw.keyword("no-warn-on-redef")
 SYM_NO_WARN_WHEN_UNUSED_META_KEY = kw.keyword("no-warn-when-unused")
 SYM_REDEF_META_KEY = kw.keyword("redef")
 
+ARGLISTS_KW = kw.keyword("arglists")
 COL_KW = kw.keyword("col")
 DOC_KW = kw.keyword("doc")
 FILE_KW = kw.keyword("file")
 LINE_KW = kw.keyword("line")
 NAME_KW = kw.keyword("name")
 NS_KW = kw.keyword("ns")
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/__init__.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import ast
 import itertools
+import os
 import types
-from typing import Optional, Callable, Any, Iterable, List, Dict
+from typing import Any, Callable, Dict, Iterable, List, Optional
 
 from astor import code_gen as codegen
 
 import basilisp.lang.runtime as runtime
 from basilisp.lang.compiler.exception import CompilerException, CompilerPhase  # noqa
 from basilisp.lang.compiler.generator import (  # noqa
-    GeneratorContext,
     GeneratedPyAST,
+    GeneratorContext,
+    USE_VAR_INDIRECTION,
+    WARN_ON_VAR_INDIRECTION,
     expressionize as _expressionize,
     gen_py_ast,
     py_module_preamble,
     statementize as _statementize,
-    USE_VAR_INDIRECTION,
-    WARN_ON_VAR_INDIRECTION,
 )
 from basilisp.lang.compiler.optimizer import PythonASTOptimizer
 from basilisp.lang.compiler.parser import (  # noqa
     ParserContext,
-    parse_ast,
     WARN_ON_SHADOWED_NAME,
     WARN_ON_SHADOWED_VAR,
     WARN_ON_UNUSED_NAMES,
+    parse_ast,
 )
-from basilisp.lang.typing import LispForm
+from basilisp.lang.typing import ReaderForm
 from basilisp.lang.util import genname
 
 _DEFAULT_FN = "__lisp_expr__"
 
 
 def to_py_str(t: ast.AST) -> str:
     """Return a string of the Python code which would generate the input
@@ -62,16 +63,33 @@
         return self._pctx
 
     @property
     def py_ast_optimizer(self) -> PythonASTOptimizer:
         return self._optimizer
 
 
+def _emit_ast_string(module: ast.AST) -> None:  # pragma: no cover
+    """Emit the generated Python AST string either to standard out or to the
+    *generated-python* dynamic Var for the current namespace. If the
+    BASILISP_EMIT_GENERATED_PYTHON env var is not set True, this method is a
+    no-op."""
+    # TODO: eventually, this default should become "false" but during this
+    #       period of heavy development, having it set to "true" by default
+    #       is tremendously useful
+    if os.getenv("BASILISP_EMIT_GENERATED_PYTHON", "true") != "true":
+        return
+
+    if runtime.print_generated_python():
+        print(to_py_str(module))
+    else:
+        runtime.add_generated_python(to_py_str(module))
+
+
 def compile_and_exec_form(  # pylint: disable= too-many-arguments
-    form: LispForm,
+    form: ReaderForm,
     ctx: CompilerContext,
     module: types.ModuleType,
     wrapped_fn_name: str = _DEFAULT_FN,
     collect_bytecode: Optional[BytecodeCollector] = None,
 ) -> Any:
     """Compile and execute the given form. This function will be most useful
     for the REPL and testing purposes. Returns the result of the executed expression.
@@ -98,18 +116,15 @@
         )
     )
 
     ast_module = ast.Module(body=form_ast)
     ast_module = ctx.py_ast_optimizer.visit(ast_module)
     ast.fix_missing_locations(ast_module)
 
-    if runtime.print_generated_python():
-        print(to_py_str(ast_module))  # pragma: no cover
-    else:
-        runtime.add_generated_python(to_py_str(ast_module))
+    _emit_ast_string(ast_module)
 
     bytecode = compile(ast_module, ctx.filename, "exec")
     if collect_bytecode:
         collect_bytecode(bytecode)
     exec(bytecode, module.__dict__)
     return getattr(module, final_wrapped_name)()
 
@@ -131,18 +146,15 @@
         map(_statementize, itertools.chain(py_ast.dependencies, [py_ast.node]))
     )
 
     module = ast.Module(body=list(module_body))
     module = optimizer.visit(module)
     ast.fix_missing_locations(module)
 
-    if runtime.print_generated_python():
-        print(to_py_str(module))  # pragma: no cover
-    else:
-        runtime.add_generated_python(to_py_str(module))
+    _emit_ast_string(module)
 
     bytecode = compile(module, source_filename, "exec")
     if collect_bytecode:
         collect_bytecode(bytecode)
     exec(bytecode, mod.__dict__)
 
 
@@ -160,15 +172,15 @@
         source_filename=gctx.filename,
         collect_bytecode=collect_bytecode,
     )
     mod.__basilisp_bootstrapped__ = True  # type: ignore
 
 
 def compile_module(
-    forms: Iterable[LispForm],
+    forms: Iterable[ReaderForm],
     ctx: CompilerContext,
     module: types.ModuleType,
     collect_bytecode: Optional[BytecodeCollector] = None,
 ) -> None:
     """Compile an entire Basilisp module into Python bytecode which can be
     executed as a Python module.
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/parser.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,115 @@
 import builtins
 import collections
 import contextlib
+import inspect
 import logging
 import re
 import sys
 import uuid
 from datetime import datetime
 from decimal import Decimal
 from fractions import Fraction
 from functools import partial, wraps
+from itertools import chain
 from typing import (
-    Pattern,
-    Union,
-    Deque,
-    Optional,
-    Dict,
-    Callable,
-    cast,
     Any,
+    Callable,
     Collection,
+    Deque,
+    Dict,
+    FrozenSet,
+    Iterable,
+    List,
+    Optional,
+    Pattern,
     Set,
     Tuple,
+    Union,
+    cast,
 )
 
 import attr
 
 import basilisp.lang.keyword as kw
 import basilisp.lang.list as llist
 import basilisp.lang.map as lmap
+import basilisp.lang.meta as lmeta
 import basilisp.lang.reader as reader
 import basilisp.lang.runtime as runtime
 import basilisp.lang.seq as lseq
 import basilisp.lang.set as lset
 import basilisp.lang.symbol as sym
 import basilisp.lang.vector as vec
 from basilisp.lang.compiler.constants import (
-    SpecialForm,
     AMPERSAND,
-    SYM_MACRO_META_KEY,
-    DEFAULT_COMPILER_FILE_PATH,
-    SYM_DYNAMIC_META_KEY,
+    ARGLISTS_KW,
     COL_KW,
+    DEFAULT_COMPILER_FILE_PATH,
+    DOC_KW,
     FILE_KW,
     LINE_KW,
     NAME_KW,
     NS_KW,
+    SYM_ASYNC_META_KEY,
+    SYM_DYNAMIC_META_KEY,
+    SYM_MACRO_META_KEY,
+    SYM_MUTABLE_META_KEY,
     SYM_NO_WARN_WHEN_UNUSED_META_KEY,
-    DOC_KW,
+    SpecialForm,
 )
 from basilisp.lang.compiler.exception import CompilerException, CompilerPhase
 from basilisp.lang.compiler.nodes import (
+    Assignable,
+    Await,
+    Binding,
+    Catch,
     Const,
-    Node,
     ConstType,
-    Map as MapNode,
-    Set as SetNode,
-    Vector as VectorNode,
-    Local,
-    Throw,
-    Quote,
-    Invoke,
-    If,
+    Def,
+    DefType,
+    DefTypeBase,
+    Do,
+    Fn,
+    FnMethod,
     HostCall,
     HostField,
-    Do,
-    Catch,
-    Binding,
+    If,
+    Import,
+    ImportAlias,
+    Invoke,
+    Let,
+    LetFn,
+    Local,
     LocalType,
+    Loop,
+    Map as MapNode,
     MaybeClass,
-    Def,
-    WithMeta,
-    FnMethod,
-    Fn,
-    Let,
-    Try,
     MaybeHostForm,
-    VarRef,
-    ReaderLispForm,
-    SetBang,
-    Assignable,
-    Loop,
+    Method,
+    Node,
+    NodeEnv,
     NodeOp,
+    PyDict,
+    PyList,
+    PySet,
+    PyTuple,
+    Quote,
     Recur,
+    Set as SetNode,
+    SetBang,
     SpecialFormNode,
-    Import,
-    ImportAlias,
-    LetFn,
-    NodeEnv,
+    Throw,
+    Try,
+    VarRef,
+    Vector as VectorNode,
+    WithMeta,
 )
 from basilisp.lang.runtime import Var
-from basilisp.lang.typing import LispForm
+from basilisp.lang.typing import LispForm, ReaderForm
 from basilisp.lang.util import count, genname, munge
 from basilisp.util import Maybe, partition
 
 # Parser logging
 logger = logging.getLogger(__name__)
 
 # Parser options
@@ -127,37 +143,46 @@
 class RecurPoint:
     loop_id: str
     args: Collection[Binding] = ()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class SymbolTableEntry:
-    context: LocalType
-    symbol: sym.Symbol
+    binding: Binding
     used: bool = False
     warn_if_unused: bool = True
 
+    @property
+    def symbol(self) -> sym.Symbol:
+        return self.binding.form
+
+    @property
+    def context(self) -> LocalType:
+        return self.binding.local
+
 
 # pylint: disable=unsupported-membership-test,unsupported-delete-operation,unsupported-assignment-operation
 @attr.s(auto_attribs=True, slots=True)
 class SymbolTable:
     name: str
     _parent: Optional["SymbolTable"] = None
     _table: Dict[sym.Symbol, SymbolTableEntry] = attr.ib(factory=dict)
     _children: Dict[str, "SymbolTable"] = attr.ib(factory=dict)
 
     def new_symbol(
-        self, s: sym.Symbol, ctx: LocalType, warn_if_unused: bool = True
+        self, s: sym.Symbol, binding: Binding, warn_if_unused: bool = True
     ) -> "SymbolTable":
+        assert s == binding.form, "Binding symbol must match passed symbol"
+
         if s in self._table:
             self._table[s] = attr.evolve(
-                self._table[s], context=ctx, symbol=s, warn_if_unused=warn_if_unused
+                self._table[s], binding=binding, warn_if_unused=warn_if_unused
             )
         else:
-            self._table[s] = SymbolTableEntry(ctx, s, warn_if_unused=warn_if_unused)
+            self._table[s] = SymbolTableEntry(binding, warn_if_unused=warn_if_unused)
         return self
 
     def find_symbol(self, s: sym.Symbol) -> Optional[SymbolTableEntry]:
         if s in self._table:
             return self._table[s]
         if self._parent is None:
             return None
@@ -221,22 +246,40 @@
         child SymbolTable before it is popped."""
         new_frame = self.append_frame(name, parent=self)
         yield new_frame
         if warn_on_unused_names and logger.isEnabledFor(logging.WARNING):
             new_frame._warn_unused_names()
         self.pop_frame(name)
 
+    def _as_env_map(self) -> Dict[sym.Symbol, lmap.Map]:
+        locals_ = {} if self._parent is None else self._parent._as_env_map()
+        locals_.update({k: v.binding.to_map() for k, v in self._table.items()})
+        return locals_
+
+    def as_env_map(self) -> lmap.Map:
+        """Return a map of symbols to the local binding objects in the
+        local symbol table as of this call."""
+        return lmap.map(self._as_env_map())
+
 
 class ParserContext:
-    __slots__ = ("_filename", "_is_quoted", "_opts", "_recur_points", "_st")
+    __slots__ = (
+        "_filename",
+        "_func_ctx",
+        "_is_quoted",
+        "_opts",
+        "_recur_points",
+        "_st",
+    )
 
     def __init__(
         self, filename: Optional[str] = None, opts: Optional[Dict[str, bool]] = None
     ) -> None:
         self._filename = Maybe(filename).or_else_get(DEFAULT_COMPILER_FILE_PATH)
+        self._func_ctx: Deque[bool] = collections.deque([])
         self._is_quoted: Deque[bool] = collections.deque([])
         self._opts = Maybe(opts).map(lmap.map).or_else_get(lmap.Map.empty())
         self._recur_points: Deque[RecurPoint] = collections.deque([])
         self._st = collections.deque([SymbolTable("<Top>")])
 
     @property
     def current_ns(self) -> runtime.Namespace:
@@ -278,14 +321,27 @@
     @contextlib.contextmanager
     def quoted(self):
         self._is_quoted.append(True)
         yield
         self._is_quoted.pop()
 
     @property
+    def is_async_ctx(self) -> bool:
+        try:
+            return self._func_ctx[-1] is True
+        except IndexError:
+            return False
+
+    @contextlib.contextmanager
+    def new_func_ctx(self, is_async: bool = False):
+        self._func_ctx.append(is_async)
+        yield
+        self._func_ctx.pop()
+
+    @property
     def recur_point(self) -> Optional[RecurPoint]:
         try:
             return self._recur_points[-1]
         except IndexError:
             return None
 
     @contextlib.contextmanager
@@ -297,15 +353,15 @@
     @property
     def symbol_table(self) -> SymbolTable:
         return self._st[-1]
 
     def put_new_symbol(  # pylint: disable=too-many-arguments
         self,
         s: sym.Symbol,
-        sym_ctx: LocalType,
+        binding: Binding,
         warn_on_shadowed_name: bool = True,
         warn_on_shadowed_var: bool = True,
         warn_if_unused: bool = True,
     ):
         """Add a new symbol to the symbol table.
 
         This function allows individual warnings to be disabled for one run
@@ -329,28 +385,37 @@
         if (
             warn_on_shadowed_name or warn_on_shadowed_var
         ) and self.warn_on_shadowed_var:
             if self.current_ns.find(s) is not None:
                 logger.warning(f"name '{s}' shadows def'ed Var from outer scope")
         if s.meta is not None and s.meta.entry(SYM_NO_WARN_WHEN_UNUSED_META_KEY, None):
             warn_if_unused = False
-        st.new_symbol(s, sym_ctx, warn_if_unused=warn_if_unused)
+        st.new_symbol(s, binding, warn_if_unused=warn_if_unused)
 
     @contextlib.contextmanager
     def new_symbol_table(self, name):
         old_st = self.symbol_table
         with old_st.new_frame(name, self.warn_on_unused_names) as st:
             self._st.append(st)
             yield st
             self._st.pop()
 
     def get_node_env(self):
         return NodeEnv(ns=self.current_ns, file=self.filename)
 
 
+def _is_async(o: lmeta.Meta) -> bool:
+    """Return True if the meta contains :async keyword."""
+    return (
+        Maybe(o.meta)
+        .map(lambda m: m.get(SYM_ASYNC_META_KEY, None))  # type: ignore
+        .or_else_get(False)
+    )
+
+
 def _is_macro(v: Var) -> bool:
     """Return True if the Var holds a macro function."""
     return (
         Maybe(v.meta)
         .map(lambda m: m.get(SYM_MACRO_META_KEY, None))  # type: ignore
         .or_else_get(False)
     )
@@ -395,15 +460,15 @@
     else:
         new_meta = meta.discard(reader.READER_LINE_KW, reader.READER_COL_KW)
         return None if len(new_meta) == 0 else new_meta
 
 
 def _with_meta(gen_node):
     """Wraps the node generated by gen_node in a :with-meta AST node if the
-    original form has .
+    original form has meta.
 
     :with-meta AST nodes are used for non-quoted collection literals and for
     function expressions."""
 
     @wraps(gen_node)
     def with_meta(ctx: ParserContext, form: lmap.Map) -> Node:
         assert not ctx.is_quoted, "with-meta nodes are not used in quoted expressions"
@@ -422,15 +487,33 @@
                 )
 
         return descriptor
 
     return with_meta
 
 
-def _def_ast(  # pylint: disable=too-many-locals
+def _await_ast(ctx: ParserContext, form: lseq.Seq) -> Await:
+    assert form.first == SpecialForm.AWAIT
+
+    if not ctx.is_async_ctx:
+        raise ParserException(
+            f"await forms may not appear in non-async context", form=form
+        )
+
+    nelems = count(form)
+    if nelems != 2:
+        raise ParserException(
+            f"await forms must contain 2 elements, as in: (await expr)", form=form
+        )
+
+    expr = _parse_ast(ctx, runtime.nth(form, 1))
+    return Await(form=form, expr=expr, env=ctx.get_node_env())
+
+
+def _def_ast(  # pylint: disable=too-many-branches,too-many-locals
     ctx: ParserContext, form: lseq.Seq
 ) -> Def:
     assert form.first == SpecialForm.DEF
 
     nelems = count(form)
     if nelems not in (2, 3, 4):
         raise ParserException(
@@ -473,24 +556,38 @@
             )
         )
     )
     assert def_meta is not None, "def metadata must be defined at this point"
     if doc is not None:
         def_meta = def_meta.assoc(DOC_KW, doc)
 
+    # Var metadata is set both for the running Basilisp instance
+    # and cached as Python bytecode to be reread again. Argument lists
+    # are quoted so as not to resolve argument symbols. For the compiled
+    # and cached bytecode, this causes no trouble. However, for the case
+    # where we directly set the Var meta for the running Basilisp instance
+    # this causes problems since we'll end up getting something like
+    # `(quote ([] [v]))` rather than simply `([] [v])`.
+    arglists_meta = def_meta.entry(ARGLISTS_KW)
+    if isinstance(arglists_meta, llist.List):
+        assert arglists_meta.first == SpecialForm.QUOTE
+        var_meta = def_meta.update({ARGLISTS_KW: runtime.nth(arglists_meta, 1)})
+    else:
+        var_meta = def_meta
+
     # Generation fails later if we use the same symbol we received, since
     # its meta may contain values which fail to compile.
     bare_name = sym.symbol(name.name)
 
     ns_sym = sym.symbol(ctx.current_ns.name)
     var = Var.intern_unbound(
         ns_sym,
         bare_name,
         dynamic=def_meta.entry(SYM_DYNAMIC_META_KEY, False),
-        meta=def_meta,
+        meta=var_meta,
     )
     descriptor = Def(
         form=form,
         name=bare_name,
         var=var,
         init=init,
         doc=doc,
@@ -533,23 +630,281 @@
     )
     existing_children = cast(vec.Vector, descriptor.children)
     return descriptor.assoc(
         meta=meta_ast, children=vec.vector(runtime.cons(META, existing_children))
     )
 
 
+def __deftype_method(  # pylint: disable=too-many-branches,too-many-locals
+    ctx: ParserContext, form: lseq.Seq, interface: DefTypeBase
+) -> Method:
+    if not isinstance(form.first, sym.Symbol):
+        raise ParserException(
+            "deftype* method must be named by symbol: (name [& args] & body)",
+            form=form.first,
+        )
+    method_name = form.first.name
+
+    args = runtime.nth(form, 1)
+    if not isinstance(args, vec.Vector):
+        raise ParserException(
+            f"deftype* method arguments must be vector, not {type(args)}", form=args
+        )
+
+    try:
+        this_arg = args[0]
+    except IndexError:
+        raise ParserException(
+            f"deftype* method must include 'this' or 'self' argument", form=args
+        )
+    else:
+        if not isinstance(this_arg, sym.Symbol):
+            raise ParserException(
+                f"deftype* method 'this' argument must be a symbol", form=args
+            )
+        this_binding = Binding(
+            form=this_arg,
+            name=this_arg.name,
+            local=LocalType.THIS,
+            env=ctx.get_node_env(),
+        )
+
+    param_nodes = []
+    for i, s in enumerate(runtime.nthrest(args, 1)):
+        if not isinstance(s, sym.Symbol):
+            raise ParserException(
+                "deftype* method parameter name must be a symbol", form=s
+            )
+
+        binding = Binding(
+            form=s,
+            name=s.name,
+            local=LocalType.ARG,
+            arg_id=i,
+            is_variadic=False,
+            env=ctx.get_node_env(),
+        )
+        param_nodes.append(binding)
+        ctx.put_new_symbol(s, binding)
+
+    loop_id = genname(method_name)
+    with ctx.new_recur_point(loop_id, param_nodes):
+        body = list(map(partial(_parse_ast, ctx), runtime.nthrest(form, 2)))
+        if body:
+            *stmts, ret = body
+        else:
+            stmts, ret = [], _const_node(ctx, None)
+
+        method = Method(
+            form=form,
+            name=method_name,
+            interface=interface,
+            this_local=this_binding,
+            params=vec.vector(param_nodes),
+            body=Do(
+                form=form.rest,
+                statements=vec.vector(stmts),
+                ret=ret,
+                is_body=True,
+                # Use the argument vector or first body statement, whichever
+                # exists, for metadata.
+                env=ctx.get_node_env(),
+            ),
+            loop_id=loop_id,
+            env=ctx.get_node_env(),
+        )
+        method.visit(_assert_recur_is_tail)
+        return method
+
+
+def __deftype_impls(  # pylint: disable=too-many-branches
+    ctx: ParserContext, form: lseq.Seq
+) -> Tuple[List[DefTypeBase], List[Method]]:
+    """Roll up deftype* declared bases and method implementations."""
+    current_interface_sym: Optional[sym.Symbol] = None
+    current_interface: Optional[DefTypeBase] = None
+    interfaces = []
+    methods: List[Method] = []
+    interface_methods: Dict[sym.Symbol, List[Method]] = {}
+    for elem in form:
+        if isinstance(elem, sym.Symbol):
+            if current_interface is not None:
+                if current_interface_sym in interface_methods:
+                    raise ParserException(
+                        f"deftype* forms may only implement an interface once",
+                        form=elem,
+                    )
+                assert (
+                    current_interface_sym is not None
+                ), "Symbol must be defined with interface"
+                interface_methods[current_interface_sym] = methods
+
+            current_interface_sym = elem
+            current_interface = _parse_ast(ctx, elem)
+            methods = []
+
+            if not isinstance(current_interface, (MaybeClass, MaybeHostForm, VarRef)):
+                raise ParserException(
+                    f"deftype* interface implementation must be an existing interface",
+                    form=elem,
+                )
+            interfaces.append(current_interface)
+        elif isinstance(elem, lseq.Seq):
+            if current_interface is None:
+                raise ParserException(
+                    f"deftype* method cannot be declared without interface", form=elem
+                )
+            methods.append(__deftype_method(ctx, elem, current_interface))
+        else:
+            raise ParserException(
+                f"deftype* must consist of interface or protocol names and methods",
+                form=elem,
+            )
+
+    if current_interface is not None:
+        if len(methods) > 0:
+            if current_interface_sym in interface_methods:
+                raise ParserException(
+                    f"deftype* forms may only implement an interface once",
+                    form=current_interface_sym,
+                )
+            assert (
+                current_interface_sym is not None
+            ), "Symbol must be defined with interface"
+            interface_methods[current_interface_sym] = methods
+        else:
+            raise ParserException(
+                f"deftype* may not declare interface without at least one method",
+                form=current_interface_sym,
+            )
+
+    return interfaces, list(chain.from_iterable(interface_methods.values()))
+
+
+def __assert_deftype_impls_are_abstract(  # pylint: disable=too-many-branches
+    interfaces: Iterable[DefTypeBase], methods: Iterable[Method]
+) -> None:
+    method_names = frozenset(munge(method.name) for method in methods)
+    for interface in interfaces:
+        if isinstance(interface, (MaybeClass, MaybeHostForm)):
+            interface_type = interface.target
+        elif isinstance(interface, VarRef):
+            interface_type = interface.var.value
+        else:  # pragma: no cover
+            assert False, "Interface must be MaybeClass, MaybeHostForm, or VarRef"
+
+        if interface_type is object:
+            continue
+
+        if not inspect.isabstract(interface_type):
+            raise ParserException(
+                "deftype* interface must be Python abstract class or object",
+                form=interface.form,
+                lisp_ast=interface,
+            )
+
+        interface_method_names: FrozenSet[str] = interface_type.__abstractmethods__
+        if not interface_method_names.issubset(method_names):
+            missing_methods = ", ".join(interface_method_names - method_names)
+            raise ParserException(
+                "deftype* definition missing interface methods for interface "
+                f"{interface.form}: {missing_methods}"
+            )
+
+        defined_interface_methods = frozenset(
+            munge(method.name) for method in methods if method.interface == interface
+        )
+        if defined_interface_methods - interface_method_names:
+            extra_methods = ", ".join(
+                defined_interface_methods - interface_method_names
+            )
+            raise ParserException(
+                "deftype* definition for interface includes methods not part of "
+                f"{interface.form}: {extra_methods}"
+            )
+
+
+def _deftype_ast(  # pylint: disable=too-many-branches
+    ctx: ParserContext, form: lseq.Seq
+) -> DefType:
+    assert form.first == SpecialForm.DEFTYPE
+
+    nelems = count(form)
+    if nelems < 3:
+        raise ParserException(
+            f"deftype forms must have 3 or more elements, as in: (deftype* name fields [bases+impls])",
+            form=form,
+        )
+
+    name = runtime.nth(form, 1)
+    if not isinstance(name, sym.Symbol):
+        raise ParserException(
+            f"deftype* names must be symbols, not {type(name)}", form=name
+        )
+    ctx.put_new_symbol(
+        name,
+        Binding(
+            form=name, name=name.name, local=LocalType.DEFTYPE, env=ctx.get_node_env()
+        ),
+        warn_if_unused=False,
+    )
+
+    fields = runtime.nth(form, 2)
+    if not isinstance(fields, vec.Vector):
+        raise ParserException(
+            f"deftype* fields must be vector, not {type(fields)}", form=fields
+        )
+
+    with ctx.new_symbol_table(name.name):
+        is_frozen = True
+        param_nodes = []
+        for field in fields:
+            if not isinstance(field, sym.Symbol):
+                raise ParserException(f"deftype* fields must be symbols", form=field)
+
+            is_mutable = (
+                Maybe(field.meta)
+                .map(lambda m: m.entry(SYM_MUTABLE_META_KEY))  # type: ignore
+                .or_else_get(False)
+            )
+            if is_mutable:
+                is_frozen = False
+
+            binding = Binding(
+                form=field,
+                name=field.name,
+                local=LocalType.FIELD,
+                is_assignable=is_mutable,
+                env=ctx.get_node_env(),
+            )
+            param_nodes.append(binding)
+            ctx.put_new_symbol(field, binding, warn_if_unused=False)
+
+        interfaces, methods = __deftype_impls(ctx, runtime.nthrest(form, 3))
+        __assert_deftype_impls_are_abstract(interfaces, methods)
+        return DefType(
+            form=form,
+            name=name.name,
+            interfaces=vec.vector(interfaces),
+            fields=vec.vector(param_nodes),
+            methods=vec.vector(methods),
+            is_frozen=is_frozen,
+            env=ctx.get_node_env(),
+        )
+
+
 def _do_ast(ctx: ParserContext, form: lseq.Seq) -> Do:
     assert form.first == SpecialForm.DO
     *statements, ret = map(partial(_parse_ast, ctx), form.rest)
     return Do(
         form=form, statements=vec.vector(statements), ret=ret, env=ctx.get_node_env()
     )
 
 
-def __fn_method_ast(  # pylint: disable=too-many-branches
+def __fn_method_ast(  # pylint: disable=too-many-branches,too-many-locals
     ctx: ParserContext, form: lseq.Seq, fnname: Optional[sym.Symbol] = None
 ) -> FnMethod:
     with ctx.new_symbol_table("fn-method"):
         params = form.first
         if not isinstance(params, vec.Vector):
             raise ParserException(
                 "function arity arguments must be a vector", form=params
@@ -564,48 +919,44 @@
                 )
 
             if s == AMPERSAND:
                 has_vargs = True
                 vargs_idx = i
                 break
 
-            param_nodes.append(
-                Binding(
-                    form=s,
-                    name=s.name,
-                    local=LocalType.ARG,
-                    arg_id=i,
-                    is_variadic=False,
-                    env=ctx.get_node_env(),
-                )
+            binding = Binding(
+                form=s,
+                name=s.name,
+                local=LocalType.ARG,
+                arg_id=i,
+                is_variadic=False,
+                env=ctx.get_node_env(),
             )
-
-            ctx.put_new_symbol(s, LocalType.ARG)
+            param_nodes.append(binding)
+            ctx.put_new_symbol(s, binding)
 
         if has_vargs:
             try:
                 vargs_sym = params[vargs_idx + 1]
 
                 if not isinstance(vargs_sym, sym.Symbol):
                     raise ParserException(
                         "function rest parameter name must be a symbol", form=vargs_sym
                     )
 
-                param_nodes.append(
-                    Binding(
-                        form=vargs_sym,
-                        name=vargs_sym.name,
-                        local=LocalType.ARG,
-                        arg_id=vargs_idx + 1,
-                        is_variadic=True,
-                        env=ctx.get_node_env(),
-                    )
+                binding = Binding(
+                    form=vargs_sym,
+                    name=vargs_sym.name,
+                    local=LocalType.ARG,
+                    arg_id=vargs_idx + 1,
+                    is_variadic=True,
+                    env=ctx.get_node_env(),
                 )
-
-                ctx.put_new_symbol(vargs_sym, LocalType.ARG)
+                param_nodes.append(binding)
+                ctx.put_new_symbol(vargs_sym, binding)
             except IndexError:
                 raise ParserException(
                     "Expected variadic argument name after '&'", form=params
                 ) from None
 
         fn_loop_id = genname("fn_arity" if fnname is None else fnname.name)
         with ctx.new_recur_point(fn_loop_id, param_nodes):
@@ -634,16 +985,17 @@
                 # form itself is a sequence with no meaningful metadata.
                 env=ctx.get_node_env(),
             )
             method.visit(_assert_recur_is_tail)
             return method
 
 
-def _fn_ast(  # pylint: disable=too-many-branches  # noqa: MC0001
-    ctx: ParserContext, form: lseq.Seq
+@_with_meta  # noqa: MC0001
+def _fn_ast(  # pylint: disable=too-many-branches
+    ctx: ParserContext, form: Union[llist.List, lseq.Seq]
 ) -> Fn:
     assert form.first == SpecialForm.FN
 
     idx = 1
 
     with ctx.new_symbol_table("fn"):
         try:
@@ -651,52 +1003,58 @@
         except IndexError:
             raise ParserException(
                 "fn form must match: (fn* name? [arg*] body*) or (fn* name? method*)",
                 form=form,
             )
 
         if isinstance(name, sym.Symbol):
-            ctx.put_new_symbol(name, LocalType.FN, warn_if_unused=False)
             name_node: Optional[Binding] = Binding(
                 form=name, name=name.name, local=LocalType.FN, env=ctx.get_node_env()
             )
+            assert name_node is not None
+            is_async = (
+                _is_async(name) or isinstance(form, lmeta.Meta) and _is_async(form)
+            )
+            ctx.put_new_symbol(name, name_node, warn_if_unused=False)
             idx += 1
         elif isinstance(name, (llist.List, vec.Vector)):
             name = None
             name_node = None
+            is_async = isinstance(form, lmeta.Meta) and _is_async(form)
         else:
             raise ParserException(
                 "fn form must match: (fn* name? [arg*] body*) or (fn* name? method*)",
                 form=form,
             )
 
         try:
             arity_or_args = runtime.nth(form, idx)
         except IndexError:
             raise ParserException(
                 "fn form expects either multiple arities or a vector of arguments",
                 form=form,
             )
 
-        if isinstance(arity_or_args, llist.List):
-            methods = vec.vector(
-                map(
-                    partial(__fn_method_ast, ctx, fnname=name),
-                    runtime.nthrest(form, idx),
+        with ctx.new_func_ctx(is_async=is_async):
+            if isinstance(arity_or_args, llist.List):
+                methods = vec.vector(
+                    map(
+                        partial(__fn_method_ast, ctx, fnname=name),
+                        runtime.nthrest(form, idx),
+                    )
+                )
+            elif isinstance(arity_or_args, vec.Vector):
+                methods = vec.v(
+                    __fn_method_ast(ctx, runtime.nthrest(form, idx), fnname=name)
+                )
+            else:
+                raise ParserException(
+                    "fn form must match: (fn* name? [arg*] body*) or (fn* name? method*)",
+                    form=form,
                 )
-            )
-        elif isinstance(arity_or_args, vec.Vector):
-            methods = vec.v(
-                __fn_method_ast(ctx, runtime.nthrest(form, idx), fnname=name)
-            )
-        else:
-            raise ParserException(
-                "fn form must match: (fn* name? [arg*] body*) or (fn* name? method*)",
-                form=form,
-            )
 
         assert count(methods) > 0, "fn must have at least one arity"
 
         fixed_arities: Set[int] = set()
         fixed_arity_for_variadic: Optional[int] = None
         num_variadic = 0
         for method in methods:
@@ -732,17 +1090,16 @@
 
         return Fn(
             form=form,
             is_variadic=num_variadic == 1,
             max_fixed_arity=max([node.fixed_arity for node in methods]),
             methods=methods,
             local=name_node,
-            # Use the function name for metadata if it exists or otherwise
-            # try the `fn*` symbol.
             env=ctx.get_node_env(),
+            is_async=is_async,
         )
 
 
 def _host_call_ast(ctx: ParserContext, form: lseq.Seq) -> HostCall:
     assert isinstance(form.first, sym.Symbol)
 
     method = form.first
@@ -901,15 +1258,15 @@
 ) -> Import:
     assert form.first == SpecialForm.IMPORT
 
     aliases = []
     for f in form.rest:
         if isinstance(f, sym.Symbol):
             module_name = f
-            module_alias = module_name.name.split(".", maxsplit=1)[0]
+            module_alias = None
         elif isinstance(f, vec.Vector):
             if len(f) != 3:
                 raise ParserException(
                     "import alias must take the form: [module :as alias]", form=f
                 )
             module_name = f.entry(0)
             if not isinstance(module_name, sym.Symbol):
@@ -937,15 +1294,16 @@
 
 def _invoke_ast(ctx: ParserContext, form: Union[llist.List, lseq.Seq]) -> Node:
     fn = _parse_ast(ctx, form.first)
 
     if fn.op == NodeOp.VAR and isinstance(fn, VarRef):
         if _is_macro(fn.var):
             try:
-                expanded = fn.var.value(form, *form.rest)
+                macro_env = ctx.symbol_table.as_env_map()
+                expanded = fn.var.value(macro_env, form, *form.rest)
                 expanded_ast = _parse_ast(ctx, expanded)
 
                 # Verify that macroexpanded code also does not have any
                 # non-tail recur forms
                 if ctx.recur_point is not None:
                     _assert_recur_is_tail(expanded_ast)
 
@@ -990,26 +1348,24 @@
 
     with ctx.new_symbol_table("let"):
         binding_nodes = []
         for name, value in partition(bindings, 2):
             if not isinstance(name, sym.Symbol):
                 raise ParserException("let binding name must be a symbol", form=name)
 
-            binding_nodes.append(
-                Binding(
-                    form=name,
-                    name=name.name,
-                    local=LocalType.LET,
-                    init=_parse_ast(ctx, value),
-                    children=vec.v(INIT),
-                    env=ctx.get_node_env(),
-                )
+            binding = Binding(
+                form=name,
+                name=name.name,
+                local=LocalType.LET,
+                init=_parse_ast(ctx, value),
+                children=vec.v(INIT),
+                env=ctx.get_node_env(),
             )
-
-            ctx.put_new_symbol(name, LocalType.LET)
+            binding_nodes.append(binding)
+            ctx.put_new_symbol(name, binding)
 
         let_body = runtime.nthrest(form, 2)
         *statements, ret = map(partial(_parse_ast, ctx), let_body)
         return Let(
             form=form,
             bindings=vec.vector(binding_nodes),
             body=Do(
@@ -1043,25 +1399,23 @@
     loop_id = genname("loop")
     with ctx.new_symbol_table(loop_id):
         binding_nodes = []
         for name, value in partition(bindings, 2):
             if not isinstance(name, sym.Symbol):
                 raise ParserException("loop binding name must be a symbol", form=name)
 
-            binding_nodes.append(
-                Binding(
-                    form=name,
-                    name=name.name,
-                    local=LocalType.LOOP,
-                    init=_parse_ast(ctx, value),
-                    env=ctx.get_node_env(),
-                )
+            binding = Binding(
+                form=name,
+                name=name.name,
+                local=LocalType.LOOP,
+                init=_parse_ast(ctx, value),
+                env=ctx.get_node_env(),
             )
-
-            ctx.put_new_symbol(name, LocalType.LOOP)
+            binding_nodes.append(binding)
+            ctx.put_new_symbol(name, binding)
 
         with ctx.new_recur_point(loop_id, binding_nodes):
             loop_body = runtime.nthrest(form, 2)
             *statements, ret = map(partial(_parse_ast, ctx), loop_body)
             loop_node = Loop(
                 form=form,
                 bindings=vec.vector(binding_nodes),
@@ -1108,16 +1462,16 @@
     `recur` forms may only appear in `do` nodes (both literal and synthetic
     `do` nodes) and in either the :then or :else expression of an `if` node."""
     if node.op == NodeOp.DO:
         assert isinstance(node, Do)
         for child in node.statements:
             _assert_no_recur(child)
         _assert_recur_is_tail(node.ret)
-    elif node.op in {NodeOp.FN, NodeOp.FN_METHOD}:
-        assert isinstance(node, (Fn, FnMethod))
+    elif node.op in {NodeOp.FN, NodeOp.FN_METHOD, NodeOp.METHOD}:
+        assert isinstance(node, (Fn, FnMethod, Method))
         node.visit(_assert_recur_is_tail)
     elif node.op == NodeOp.IF:
         assert isinstance(node, If)
         _assert_no_recur(node.test)
         _assert_recur_is_tail(node.then)
         _assert_recur_is_tail(node.else_)
     elif node.op in {NodeOp.LET, NodeOp.LETFN}:
@@ -1215,27 +1569,28 @@
         )
 
     local_name = runtime.nth(form, 2)
     if not isinstance(local_name, sym.Symbol):
         raise ParserException("catch local must be a symbol", form=local_name)
 
     with ctx.new_symbol_table("catch"):
-        ctx.put_new_symbol(local_name, LocalType.CATCH)
+        catch_binding = Binding(
+            form=local_name,
+            name=local_name.name,
+            local=LocalType.CATCH,
+            env=ctx.get_node_env(),
+        )
+        ctx.put_new_symbol(local_name, catch_binding)
 
         catch_body = runtime.nthrest(form, 3)
         *catch_statements, catch_ret = map(partial(_parse_ast, ctx), catch_body)
         return Catch(
             form=form,
             class_=catch_cls,
-            local=Binding(
-                form=local_name,
-                name=local_name.name,
-                local=LocalType.CATCH,
-                env=ctx.get_node_env(),
-            ),
+            local=catch_binding,
             body=Do(
                 form=catch_body,
                 statements=vec.vector(catch_statements),
                 ret=catch_ret,
                 is_body=True,
                 env=ctx.get_node_env(),
             ),
@@ -1334,16 +1689,18 @@
         raise ParserException(f"cannot resolve var {var_sym}", form=form)
 
     return VarRef(form=var_sym, var=var, return_var=True, env=ctx.get_node_env())
 
 
 SpecialFormHandler = Callable[[ParserContext, lseq.Seq], SpecialFormNode]
 _SPECIAL_FORM_HANDLERS: Dict[sym.Symbol, SpecialFormHandler] = {
+    SpecialForm.AWAIT: _await_ast,
     SpecialForm.DEF: _def_ast,
     SpecialForm.DO: _do_ast,
+    SpecialForm.DEFTYPE: _deftype_ast,
     SpecialForm.FN: _fn_ast,
     SpecialForm.IF: _if_ast,
     SpecialForm.IMPORT: _import_ast,
     SpecialForm.INTEROP_CALL: _host_interop_ast,
     SpecialForm.LET: _let_ast,
     SpecialForm.LOOP: _loop_ast,
     SpecialForm.QUOTE: _quote_ast,
@@ -1379,18 +1736,22 @@
     assert form.ns is not None
 
     if form.ns == ctx.current_ns.name:
         v = ctx.current_ns.find(sym.symbol(form.name))
         if v is not None:
             return VarRef(form=form, var=v, env=ctx.get_node_env())
     elif form.ns == _BUILTINS_NS:
+        class_ = munge(form.name, allow_builtins=True)
+        target = getattr(builtins, class_, None)
+        if target is None:
+            raise ParserException(
+                f"cannot resolve builtin function '{class_}'", form=form
+            )
         return MaybeClass(
-            form=form,
-            class_=munge(form.name, allow_builtins=True),
-            env=ctx.get_node_env(),
+            form=form, class_=class_, target=target, env=ctx.get_node_env()
         )
 
     if "." in form.name:
         raise ParserException(
             "symbol names may not contain the '.' operator", form=form
         )
 
@@ -1417,33 +1778,35 @@
         assert (
             safe_module_name in sys.modules
         ), f"Module '{safe_module_name}' is not imported"
         ns_module = sys.modules[safe_module_name]
         safe_name = munge(form.name)
 
         # Try without allowing builtins first
-        if safe_name in ns_module.__dict__:
+        if safe_name in vars(ns_module):
             return MaybeHostForm(
                 form=form,
                 class_=munge(ns_sym.name),
                 field=safe_name,
+                target=vars(ns_module)[safe_name],
                 env=ctx.get_node_env(),
             )
 
         # Then allow builtins
         safe_name = munge(form.name, allow_builtins=True)
-        if safe_name not in ns_module.__dict__:
+        if safe_name not in vars(ns_module):
             raise ParserException("can't identify aliased form", form=form)
 
         # Aliased imports generate code which uses the import alias, so we
         # don't need to care if this is an import or an alias.
         return MaybeHostForm(
             form=form,
             class_=munge(ns_sym.name),
             field=safe_name,
+            target=vars(ns_module)[safe_name],
             env=ctx.get_node_env(),
         )
     elif ns_sym in ctx.current_ns.aliases:
         aliased_ns: runtime.Namespace = ctx.current_ns.aliases[ns_sym]
         v = Var.find(sym.symbol(form.name, ns=aliased_ns.name))
         if v is None:
             raise ParserException(
@@ -1470,22 +1833,24 @@
         return VarRef(form=form, var=v, env=ctx.get_node_env())
 
     if "." in form.name:
         raise ParserException(
             "symbol names may not contain the '.' operator", form=form
         )
 
-    if form.name in builtins.__dict__:
+    munged = munge(form.name, allow_builtins=True)
+    if munged in vars(builtins):
         return MaybeClass(
             form=form,
-            class_=munge(form.name, allow_builtins=True),
+            class_=munged,
+            target=vars(builtins)[munged],
             env=ctx.get_node_env(),
         )
 
-    assert form.name not in ctx.current_ns.module.__dict__
+    assert munged not in vars(ctx.current_ns.module)
     raise ParserException(
         f"unable to resolve symbol '{form}' in this context", form=form
     )
 
 
 def _resolve_sym(
     ctx: ParserContext, form: sym.Symbol
@@ -1517,21 +1882,56 @@
     sym_entry = ctx.symbol_table.find_symbol(form)
     if sym_entry is not None:
         ctx.symbol_table.mark_used(form)
         return Local(
             form=form,
             name=form.name,
             local=sym_entry.context,
-            is_assignable=False,
+            is_assignable=sym_entry.binding.is_assignable,
             env=ctx.get_node_env(),
         )
 
     return _resolve_sym(ctx, form)
 
 
+def _py_dict_node(ctx: ParserContext, form: dict) -> PyDict:
+    keys, vals = [], []
+    for k, v in form.items():
+        keys.append(_parse_ast(ctx, k))
+        vals.append(_parse_ast(ctx, v))
+
+    return PyDict(
+        form=form, keys=vec.vector(keys), vals=vec.vector(vals), env=ctx.get_node_env()
+    )
+
+
+def _py_list_node(ctx: ParserContext, form: list) -> PyList:
+    return PyList(
+        form=form,
+        items=vec.vector(map(partial(_parse_ast, ctx), form)),
+        env=ctx.get_node_env(),
+    )
+
+
+def _py_set_node(ctx: ParserContext, form: set) -> PySet:
+    return PySet(
+        form=form,
+        items=vec.vector(map(partial(_parse_ast, ctx), form)),
+        env=ctx.get_node_env(),
+    )
+
+
+def _py_tuple_node(ctx: ParserContext, form: tuple) -> PyTuple:
+    return PyTuple(
+        form=form,
+        items=vec.vector(map(partial(_parse_ast, ctx), form)),
+        env=ctx.get_node_env(),
+    )
+
+
 @_with_meta
 def _map_node(ctx: ParserContext, form: lmap.Map) -> MapNode:
     keys, vals = [], []
     for k, v in form.items():
         keys.append(_parse_ast(ctx, k))
         vals.append(_parse_ast(ctx, v))
 
@@ -1559,32 +1959,36 @@
 
 
 _CONST_NODE_TYPES = {  # type: ignore
     bool: ConstType.BOOL,
     complex: ConstType.NUMBER,
     datetime: ConstType.INST,
     Decimal: ConstType.DECIMAL,
+    dict: ConstType.PY_DICT,
     float: ConstType.NUMBER,
     Fraction: ConstType.FRACTION,
     int: ConstType.NUMBER,
     kw.Keyword: ConstType.KEYWORD,
+    list: ConstType.PY_LIST,
     llist.List: ConstType.SEQ,
     lmap.Map: ConstType.MAP,
     lset.Set: ConstType.SET,
     lseq.Seq: ConstType.SEQ,
     type(re.compile("")): ConstType.REGEX,
+    set: ConstType.PY_SET,
     sym.Symbol: ConstType.SYMBOL,
     str: ConstType.STRING,
+    tuple: ConstType.PY_TUPLE,
     type(None): ConstType.NIL,
     uuid.UUID: ConstType.UUID,
     vec.Vector: ConstType.VECTOR,
 }
 
 
-def _const_node(ctx: ParserContext, form: ReaderLispForm) -> Const:
+def _const_node(ctx: ParserContext, form: ReaderForm) -> Const:
     assert (
         (
             ctx.is_quoted
             and isinstance(
                 form, (sym.Symbol, vec.Vector, llist.List, lmap.Map, lset.Set, lseq.Seq)
             )
         )
@@ -1592,20 +1996,24 @@
         or isinstance(
             form,
             (
                 bool,
                 complex,
                 datetime,
                 Decimal,
+                dict,
                 float,
                 Fraction,
                 int,
                 kw.Keyword,
+                list,
                 Pattern,
+                set,
                 str,
+                tuple,
                 type(None),
                 uuid.UUID,
             ),
         )
     )
 
     node_type = _CONST_NODE_TYPES.get(type(form), ConstType.UNKNOWN)
@@ -1626,24 +2034,27 @@
                 isinstance(meta_ast, Const) and meta_ast.type == ConstType.MAP
             )
             return descriptor.assoc(meta=meta_ast, children=vec.v(META))
 
     return descriptor
 
 
-@_with_loc
+@_with_loc  # noqa: MC0001
 def _parse_ast(  # pylint: disable=too-many-branches
-    ctx: ParserContext, form: Union[LispForm, lseq.Seq]
+    ctx: ParserContext, form: Union[ReaderForm, lseq.Seq]
 ) -> Node:
     if isinstance(form, (llist.List, lseq.Seq)):
         # Special case for unquoted empty list
         if form == llist.List.empty():
             with ctx.quoted():
                 return _const_node(ctx, form)
-        return _list_node(ctx, form)
+        elif ctx.is_quoted:
+            return _const_node(ctx, form)
+        else:
+            return _list_node(ctx, form)
     elif isinstance(form, vec.Vector):
         if ctx.is_quoted:
             return _const_node(ctx, form)
         return _vector_node(ctx, form)
     elif isinstance(form, lmap.Map):
         if ctx.is_quoted:
             return _const_node(ctx, form)
@@ -1669,15 +2080,31 @@
             sym.Symbol,
             str,
             type(None),
             uuid.UUID,
         ),
     ):
         return _const_node(ctx, form)
+    elif isinstance(form, dict):
+        if ctx.is_quoted:
+            return _const_node(ctx, form)
+        return _py_dict_node(ctx, form)
+    elif isinstance(form, list):
+        if ctx.is_quoted:
+            return _const_node(ctx, form)
+        return _py_list_node(ctx, form)
+    elif isinstance(form, set):
+        if ctx.is_quoted:
+            return _const_node(ctx, form)
+        return _py_set_node(ctx, form)
+    elif isinstance(form, tuple):
+        if ctx.is_quoted:
+            return _const_node(ctx, form)
+        return _py_tuple_node(ctx, form)
     else:  # pragma: no cover
         raise ParserException(f"Unexpected form type {type(form)}", form=form)
 
 
-def parse_ast(ctx: ParserContext, form: LispForm) -> Node:
+def parse_ast(ctx: ParserContext, form: ReaderForm) -> Node:
     """Take a Lisp form as an argument and produce a Basilisp syntax
     tree matching the clojure.tools.analyzer AST spec."""
     return _parse_ast(ctx, form).assoc(top_level=True)
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/generator.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import re
 import types
 import uuid
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from fractions import Fraction
-from functools import wraps, partial
+from functools import partial, wraps
 from itertools import chain
 from typing import (
-    Iterable,
-    Pattern,
-    Optional,
-    List,
-    Union,
+    Callable,
+    Collection,
     Deque,
     Dict,
-    Callable,
+    Iterable,
+    List,
+    Optional,
+    Pattern,
     Tuple,
     Type,
-    Collection,
+    Union,
 )
 
 import attr
 
 import basilisp.lang.keyword as kw
 import basilisp.lang.list as llist
 import basilisp.lang.map as lmap
@@ -42,77 +42,79 @@
     DEFAULT_COMPILER_FILE_PATH,
     SYM_DYNAMIC_META_KEY,
     SYM_NO_WARN_ON_REDEF_META_KEY,
     SYM_REDEF_META_KEY,
 )
 from basilisp.lang.compiler.exception import CompilerException, CompilerPhase
 from basilisp.lang.compiler.nodes import (
-    Node,
-    NodeOp,
-    ConstType,
+    Await,
+    Binding,
+    Catch,
     Const,
-    WithMeta,
+    ConstType,
     Def,
+    DefType,
     Do,
-    If,
-    VarRef,
+    Fn,
+    FnMethod,
     HostCall,
     HostField,
+    If,
+    Import,
+    Invoke,
+    Let,
+    Local,
+    LocalType,
+    Loop,
+    Map as MapNode,
     MaybeClass,
     MaybeHostForm,
-    Map as MapNode,
-    Set as SetNode,
-    Vector as VectorNode,
+    Method,
+    Node,
+    NodeEnv,
+    NodeOp,
+    PyDict,
+    PyList,
+    PySet,
+    PyTuple,
     Quote,
     ReaderLispForm,
-    Invoke,
+    Recur,
+    Set as SetNode,
+    SetBang,
     Throw,
     Try,
-    LocalType,
-    SetBang,
-    Local,
-    Let,
-    Loop,
-    Recur,
-    Fn,
-    Import,
-    FnMethod,
-    Binding,
-    NodeEnv,
-    Catch,
+    VarRef,
+    Vector as VectorNode,
+    WithMeta,
 )
-from basilisp.lang.runtime import Var
+from basilisp.lang.runtime import CORE_NS, NS_VAR_NAME as LISP_NS_VAR, Var
 from basilisp.lang.typing import LispForm
 from basilisp.lang.util import count, genname, munge
 from basilisp.util import Maybe
 
 # Generator logging
 logger = logging.getLogger(__name__)
 
 # Generator options
 USE_VAR_INDIRECTION = "use_var_indirection"
 WARN_ON_VAR_INDIRECTION = "warn_on_var_indirection"
 
-# Lisp AST node keywords
-INIT = kw.keyword("init")
-
 # String constants used in generating code
 _BUILTINS_NS = "builtins"
-_CORE_NS = "basilisp.core"
 _DEFAULT_FN = "__lisp_expr__"
 _DO_PREFIX = "lisp_do"
 _FN_PREFIX = "lisp_fn"
 _IF_PREFIX = "lisp_if"
 _IF_RESULT_PREFIX = "if_result"
 _IF_TEST_PREFIX = "if_test"
 _MULTI_ARITY_ARG_NAME = "multi_arity_args"
 _THROW_PREFIX = "lisp_throw"
 _TRY_PREFIX = "lisp_try"
 _NS_VAR = "__NS"
-_LISP_NS_VAR = "*ns*"
 
 
 GeneratorException = partial(CompilerException, phase=CompilerPhase.CODE_GENERATION)
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class SymbolTableEntry:
@@ -159,36 +161,38 @@
         new_frame = self.append_frame(name, parent=self)
         yield new_frame
         self.pop_frame(name)
 
 
 class RecurType(Enum):
     FN = kw.keyword("fn")
+    METHOD = kw.keyword("method")
     LOOP = kw.keyword("loop")
 
 
 @attr.s(auto_attribs=True, slots=True)
 class RecurPoint:
     loop_id: str
     type: RecurType
     binding_names: Optional[Collection[str]] = None
     is_variadic: Optional[bool] = None
     has_recur: bool = False
 
 
 class GeneratorContext:
-    __slots__ = ("_filename", "_opts", "_recur_points", "_st")
+    __slots__ = ("_filename", "_opts", "_recur_points", "_st", "_this")
 
     def __init__(
         self, filename: Optional[str] = None, opts: Optional[Dict[str, bool]] = None
     ) -> None:
         self._filename = Maybe(filename).or_else_get(DEFAULT_COMPILER_FILE_PATH)
         self._opts = Maybe(opts).map(lmap.map).or_else_get(lmap.m())
         self._recur_points: Deque[RecurPoint] = collections.deque([])
         self._st = collections.deque([SymbolTable("<Top>")])
+        self._this: Deque[sym.Symbol] = collections.deque([])
 
         if logger.isEnabledFor(logging.DEBUG):  # pragma: no cover
             for k, v in self._opts:
                 logger.debug("Compiler option %s=%s", k, v)
 
     @property
     def current_ns(self) -> runtime.Namespace:
@@ -246,14 +250,24 @@
     def add_import(self, imp: sym.Symbol, mod: types.ModuleType, *aliases: sym.Symbol):
         self.current_ns.add_import(imp, mod, *aliases)
 
     @property
     def imports(self) -> lmap.Map:
         return self.current_ns.imports
 
+    @property
+    def current_this(self):
+        return self._this[-1]
+
+    @contextlib.contextmanager
+    def new_this(self, this: sym.Symbol):
+        self._this.append(this)
+        yield
+        self._this.pop()
+
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class GeneratedPyAST:
     node: ast.AST
     dependencies: Iterable[ast.AST] = ()
 
     @staticmethod
@@ -286,18 +300,21 @@
 def _load_attr(name: str, ctx: ast.AST = ast.Load()) -> ast.Attribute:
     """Generate recursive Python Attribute AST nodes for resolving nested
     names."""
     attrs = name.split(".")
 
     def attr_node(node, idx):
         if idx >= len(attrs):
+            node.ctx = ctx
             return node
-        return attr_node(ast.Attribute(value=node, attr=attrs[idx], ctx=ctx), idx + 1)
+        return attr_node(
+            ast.Attribute(value=node, attr=attrs[idx], ctx=ast.Load()), idx + 1
+        )
 
-    return attr_node(ast.Name(id=attrs[0], ctx=ctx), 1)
+    return attr_node(ast.Name(id=attrs[0], ctx=ast.Load()), 1)
 
 
 def _simple_ast_generator(gen_ast):
     """Wrap simpler AST generators to return a GeneratedPyAST."""
 
     @wraps(gen_ast)
     def wrapped_ast_generator(ctx: GeneratorContext, form: LispForm) -> GeneratedPyAST:
@@ -424,16 +441,20 @@
 _NEW_REGEX_FN_NAME = _load_attr(f"{_UTIL_ALIAS}.regex_from_str")
 _NEW_SET_FN_NAME = _load_attr(f"{_SET_ALIAS}.set")
 _NEW_SYM_FN_NAME = _load_attr(f"{_SYM_ALIAS}.symbol")
 _NEW_UUID_FN_NAME = _load_attr(f"{_UTIL_ALIAS}.uuid_from_str")
 _NEW_VEC_FN_NAME = _load_attr(f"{_VEC_ALIAS}.vector")
 _INTERN_VAR_FN_NAME = _load_attr(f"{_VAR_ALIAS}.intern")
 _FIND_VAR_FN_NAME = _load_attr(f"{_VAR_ALIAS}.find_safe")
+_ATTR_CLASS_DECORATOR_NAME = _load_attr(f"attr.s")
+_ATTRIB_FIELD_FN_NAME = _load_attr(f"attr.ib")
 _COLLECT_ARGS_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}._collect_args")
 _COERCE_SEQ_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}.to_seq")
+_BASILISP_FN_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}._basilisp_fn")
+_FN_WITH_ATTRS_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}._with_attrs")
 _TRAMPOLINE_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}._trampoline")
 _TRAMPOLINE_ARGS_FN_NAME = _load_attr(f"{_RUNTIME_ALIAS}._TrampolineArgs")
 
 
 ###################
 # Public Utilities
 ###################
@@ -512,14 +533,23 @@
 
 
 #################
 # Special Forms
 #################
 
 
+@_with_ast_loc_deps
+def _await_to_py_ast(ctx: GeneratorContext, node: Await) -> GeneratedPyAST:
+    assert node.op == NodeOp.AWAIT
+    expr_ast = gen_py_ast(ctx, node.expr)
+    return GeneratedPyAST(
+        node=ast.Await(value=expr_ast.node), dependencies=expr_ast.dependencies
+    )
+
+
 def __should_warn_on_redef(
     ctx: GeneratorContext, defsym: sym.Symbol, safe_name: str, def_meta: lmap.Map
 ) -> bool:
     """Return True if the compiler should emit a warning about this name being redefined."""
     no_warn_on_redef = def_meta.entry(SYM_NO_WARN_ON_REDEF_META_KEY, False)
     if no_warn_on_redef:
         return False
@@ -545,25 +575,32 @@
 ) -> GeneratedPyAST:
     """Return a Python AST Node for a `def` expression."""
     assert node.op == NodeOp.DEF
 
     defsym = node.name
     is_defn = False
 
-    if INIT in node.children:
+    if node.init is not None:
         # Since Python function definitions always take the form `def name(...):`,
         # it is redundant to assign them to the their final name after they have
         # been defined under a private alias. This codepath generates `defn`
         # declarations by directly generating the Python `def` with the correct
         # function name and short-circuiting the default double-declaration.
-        assert node.init is not None, "Def init must be defined"
         if node.init.op == NodeOp.FN:
             assert isinstance(node.init, Fn)
             def_ast = _fn_to_py_ast(ctx, node.init, def_name=defsym.name)
             is_defn = True
+        elif (
+            node.init.op == NodeOp.WITH_META
+            and isinstance(node.init, WithMeta)
+            and node.init.expr.op == NodeOp.FN
+        ):
+            assert isinstance(node.init, WithMeta)
+            def_ast = _with_meta_to_py_ast(ctx, node.init, def_name=defsym.name)
+            is_defn = True
         else:
             def_ast = gen_py_ast(ctx, node.init)
     else:
         def_ast = GeneratedPyAST(node=ast.NameConstant(None))
 
     ns_name = ast.Call(func=_NEW_SYM_FN_NAME, args=[_NS_VAR_NAME], keywords=[])
     def_name = ast.Call(func=_NEW_SYM_FN_NAME, args=[ast.Str(defsym.name)], keywords=[])
@@ -630,24 +667,129 @@
                 )
             ),  # type: ignore
         ),
         dependencies=def_dependencies,
     )
 
 
+@_with_ast_loc
+def __deftype_method_to_py_ast(  # pylint: disable=too-many-branches
+    ctx: GeneratorContext, node: Method
+) -> GeneratedPyAST:
+    assert node.op == NodeOp.METHOD
+    method_name = munge(node.name)
+
+    with ctx.new_symbol_table(node.name), ctx.new_recur_point(
+        node.loop_id, RecurType.METHOD, is_variadic=False
+    ):
+        this_name = genname(munge(node.this_local.name))
+        this_sym = sym.symbol(node.this_local.name)
+        ctx.symbol_table.new_symbol(this_sym, this_name, LocalType.THIS)
+
+        with ctx.new_this(this_sym):
+            fn_args, varg, fn_body_ast = __fn_args_to_py_ast(
+                ctx, node.params, node.body
+            )
+            return GeneratedPyAST(
+                node=ast.FunctionDef(
+                    name=method_name,
+                    args=ast.arguments(
+                        args=list(
+                            chain([ast.arg(arg=this_name, annotation=None)], fn_args)
+                        ),
+                        kwarg=None,
+                        vararg=varg,
+                        kwonlyargs=[],
+                        defaults=[],
+                        kw_defaults=[],
+                    ),
+                    body=fn_body_ast,
+                    decorator_list=list(
+                        chain(
+                            [_BASILISP_FN_FN_NAME],
+                            [_TRAMPOLINE_FN_NAME] if ctx.recur_point.has_recur else [],
+                        )
+                    ),
+                    returns=None,
+                )
+            )
+
+
+@_with_ast_loc
+def _deftype_to_py_ast(  # pylint: disable=too-many-branches
+    ctx: GeneratorContext, node: DefType
+) -> GeneratedPyAST:
+    """Return a Python AST Node for a `deftype*` expression."""
+    assert node.op == NodeOp.DEFTYPE
+    type_name = munge(node.name)
+    ctx.symbol_table.new_symbol(sym.symbol(node.name), type_name, LocalType.DEFTYPE)
+
+    bases = []
+    for base in node.interfaces:
+        base_node = gen_py_ast(ctx, base)
+        assert (
+            count(base_node.dependencies) == 0
+        ), "Class and host form nodes do not have dependencies"
+        bases.append(base_node.node)
+
+    decorator = ast.Call(
+        func=_ATTR_CLASS_DECORATOR_NAME,
+        args=[],
+        keywords=[
+            ast.keyword(arg="cmp", value=ast.NameConstant(False)),
+            ast.keyword(arg="frozen", value=ast.NameConstant(node.is_frozen)),
+            ast.keyword(arg="slots", value=ast.NameConstant(True)),
+        ],
+    )
+
+    with ctx.new_symbol_table(node.name):
+        type_nodes = []
+        for field in node.fields:
+            safe_field = munge(field.name)
+            type_nodes.append(
+                ast.Assign(
+                    targets=[ast.Name(id=safe_field, ctx=ast.Store())],
+                    value=ast.Call(func=_ATTRIB_FIELD_FN_NAME, args=[], keywords=[]),
+                )
+            )
+            ctx.symbol_table.new_symbol(sym.symbol(field.name), safe_field, field.local)
+
+        type_deps: List[ast.AST] = []
+        for method in node.methods:
+            type_ast = __deftype_method_to_py_ast(ctx, method)
+            type_nodes.append(type_ast.node)
+            type_deps.extend(type_ast.dependencies)
+
+        return GeneratedPyAST(
+            node=ast.Name(id=type_name, ctx=ast.Load()),
+            dependencies=list(
+                chain(
+                    type_deps,
+                    [
+                        ast.ClassDef(
+                            name=type_name,
+                            bases=bases,
+                            keywords=[],
+                            body=type_nodes,
+                            decorator_list=[decorator],
+                        )
+                    ],
+                )
+            ),
+        )
+
+
 @_with_ast_loc_deps
 def _do_to_py_ast(ctx: GeneratorContext, node: Do) -> GeneratedPyAST:
     """Return a Python AST Node for a `do` expression."""
     assert node.op == NodeOp.DO
     assert not node.is_body
 
     body_ast = GeneratedPyAST.reduce(
-        *chain(
-            map(partial(gen_py_ast, ctx), node.statements), [gen_py_ast(ctx, node.ret)]
-        )
+        *map(partial(gen_py_ast, ctx), chain(node.statements, [node.ret]))
     )
 
     fn_body_ast: List[ast.AST] = []
     do_result_name = genname(_DO_PREFIX)
     fn_body_ast.extend(map(statementize, body_ast.dependencies))
     fn_body_ast.append(
         ast.Assign(
@@ -666,20 +808,21 @@
     (e.g. a :do node which acts as a body for another node)."""
     assert node.op == NodeOp.DO
     assert node.is_body
 
     # TODO: investigate how to handle recur in node.ret
 
     return GeneratedPyAST.reduce(
-        *chain(
-            map(partial(gen_py_ast, ctx), node.statements), [gen_py_ast(ctx, node.ret)]
-        )
+        *map(partial(gen_py_ast, ctx), chain(node.statements, [node.ret]))
     )
 
 
+MetaNode = Union[Const, MapNode]
+
+
 def __fn_name(s: Optional[str]) -> str:
     """Generate a safe Python function name from a function name symbol.
     If no symbol is provided, generate a name with a default prefix."""
     return genname("__" + munge(Maybe(s).or_else_get(_FN_PREFIX)))
 
 
 def __fn_args_to_py_ast(
@@ -718,64 +861,111 @@
     body_ast = _synthetic_do_to_py_ast(ctx, body)
     fn_body_ast.extend(map(statementize, body_ast.dependencies))
     fn_body_ast.append(ast.Return(value=body_ast.node))
 
     return fn_args, varg, fn_body_ast
 
 
+def __fn_meta(
+    ctx: GeneratorContext, meta_node: Optional[MetaNode] = None
+) -> Tuple[Iterable[ast.AST], Iterable[ast.AST]]:
+    if meta_node is not None:
+        meta_ast = gen_py_ast(ctx, meta_node)
+        return (
+            meta_ast.dependencies,
+            [
+                ast.Call(
+                    func=_FN_WITH_ATTRS_FN_NAME,
+                    args=[],
+                    keywords=[ast.keyword(arg="meta", value=meta_ast.node)],
+                )
+            ],
+        )
+    else:
+        return (), ()
+
+
 @_with_ast_loc_deps
 def __single_arity_fn_to_py_ast(
-    ctx: GeneratorContext, node: Fn, method: FnMethod, def_name: Optional[str] = None
+    ctx: GeneratorContext,
+    node: Fn,
+    method: FnMethod,
+    def_name: Optional[str] = None,
+    meta_node: Optional[MetaNode] = None,
 ) -> GeneratedPyAST:
     """Return a Python AST node for a function with a single arity."""
     assert node.op == NodeOp.FN
     assert method.op == NodeOp.FN_METHOD
 
     lisp_fn_name = node.local.name if node.local is not None else None
     py_fn_name = __fn_name(lisp_fn_name) if def_name is None else munge(def_name)
+    py_fn_node = ast.AsyncFunctionDef if node.is_async else ast.FunctionDef
     with ctx.new_symbol_table(py_fn_name), ctx.new_recur_point(
         method.loop_id, RecurType.FN, is_variadic=node.is_variadic
     ):
         # Allow named anonymous functions to recursively call themselves
         if lisp_fn_name is not None:
             ctx.symbol_table.new_symbol(
                 sym.symbol(lisp_fn_name), py_fn_name, LocalType.FN
             )
 
         fn_args, varg, fn_body_ast = __fn_args_to_py_ast(
             ctx, method.params, method.body
         )
+        meta_deps, meta_decorators = __fn_meta(ctx, meta_node)
         return GeneratedPyAST(
             node=ast.Name(id=py_fn_name, ctx=ast.Load()),
-            dependencies=[
-                ast.FunctionDef(
-                    name=py_fn_name,
-                    args=ast.arguments(
-                        args=fn_args,
-                        kwarg=None,
-                        vararg=varg,
-                        kwonlyargs=[],
-                        defaults=[],
-                        kw_defaults=[],
-                    ),
-                    body=fn_body_ast,
-                    decorator_list=[_TRAMPOLINE_FN_NAME]
-                    if ctx.recur_point.has_recur
-                    else [],
-                    returns=None,
+            dependencies=list(
+                chain(
+                    meta_deps,
+                    [
+                        py_fn_node(
+                            name=py_fn_name,
+                            args=ast.arguments(
+                                args=fn_args,
+                                kwarg=None,
+                                vararg=varg,
+                                kwonlyargs=[],
+                                defaults=[],
+                                kw_defaults=[],
+                            ),
+                            body=fn_body_ast,
+                            decorator_list=list(
+                                chain(
+                                    meta_decorators,
+                                    [_BASILISP_FN_FN_NAME],
+                                    [_TRAMPOLINE_FN_NAME]
+                                    if ctx.recur_point.has_recur
+                                    else [],
+                                )
+                            ),
+                            returns=None,
+                        )
+                    ],
                 )
-            ],
+            ),
         )
 
 
-def __multi_arity_dispatch_fn(
+def __handle_async_return(node: ast.AST) -> ast.Return:
+    return ast.Return(value=ast.Await(value=node))
+
+
+def __handle_return(node: ast.AST) -> ast.Return:
+    return ast.Return(value=node)
+
+
+def __multi_arity_dispatch_fn(  # pylint: disable=too-many-arguments,too-many-locals
+    ctx: GeneratorContext,
     name: str,
     arity_map: Dict[int, str],
     default_name: Optional[str] = None,
     max_fixed_arity: Optional[int] = None,
+    meta_node: Optional[MetaNode] = None,
+    is_async: bool = False,
 ) -> GeneratedPyAST:
     """Return the Python AST nodes for a argument-length dispatch function
     for multi-arity functions.
 
     def fn(*args):
         nargs = len(args)
         method = __fn_dispatch_map.get(nargs)
@@ -789,14 +979,17 @@
     dispatch_map_name = f"{name}_dispatch_map"
 
     dispatch_keys, dispatch_vals = [], []
     for k, v in arity_map.items():
         dispatch_keys.append(ast.Num(k))
         dispatch_vals.append(ast.Name(id=v, ctx=ast.Load()))
 
+    # Async functions should return await, otherwise just return
+    handle_return = __handle_async_return if is_async else __handle_return
+
     nargs_name = genname("nargs")
     method_name = genname("method")
     body = [
         ast.Assign(
             targets=[ast.Name(id=nargs_name, ctx=ast.Store())],
             value=ast.Call(
                 func=ast.Name(id="len", ctx=ast.Load()),
@@ -819,16 +1012,16 @@
         ast.If(
             test=ast.Compare(
                 left=ast.NameConstant(None),
                 ops=[ast.IsNot()],
                 comparators=[ast.Name(id=method_name, ctx=ast.Load())],
             ),
             body=[
-                ast.Return(
-                    value=ast.Call(
+                handle_return(
+                    ast.Call(
                         func=ast.Name(id=method_name, ctx=ast.Load()),
                         args=[
                             ast.Starred(
                                 value=ast.Name(
                                     id=_MULTI_ARITY_ARG_NAME, ctx=ast.Load()
                                 ),
                                 ctx=ast.Load(),
@@ -844,16 +1037,16 @@
                 ast.If(
                     test=ast.Compare(
                         left=ast.Name(id=nargs_name, ctx=ast.Load()),
                         ops=[ast.GtE()],
                         comparators=[ast.Num(max_fixed_arity)],
                     ),
                     body=[
-                        ast.Return(
-                            value=ast.Call(
+                        handle_return(
+                            ast.Call(
                                 func=ast.Name(id=default_name, ctx=ast.Load()),
                                 args=[
                                     ast.Starred(
                                         value=ast.Name(
                                             id=_MULTI_ARITY_ARG_NAME, ctx=ast.Load()
                                         ),
                                         ctx=ast.Load(),
@@ -876,53 +1069,63 @@
                 ],
                 keywords=[],
             ),
             cause=None,
         ),
     ]
 
+    py_fn_node = ast.AsyncFunctionDef if is_async else ast.FunctionDef
+    meta_deps, meta_decorators = __fn_meta(ctx, meta_node)
     return GeneratedPyAST(
         node=ast.Name(id=name, ctx=ast.Load()),
-        dependencies=[
-            ast.Assign(
-                targets=[ast.Name(id=dispatch_map_name, ctx=ast.Store())],
-                value=ast.Dict(keys=dispatch_keys, values=dispatch_vals),
-            ),
-            ast.FunctionDef(
-                name=name,
-                args=ast.arguments(
-                    args=[],
-                    kwarg=None,
-                    vararg=ast.arg(arg=_MULTI_ARITY_ARG_NAME, annotation=None),
-                    kwonlyargs=[],
-                    defaults=[],
-                    kw_defaults=[],
-                ),
-                body=body,
-                decorator_list=[],
-                returns=None,
-            ),
-        ],
+        dependencies=chain(
+            [
+                ast.Assign(
+                    targets=[ast.Name(id=dispatch_map_name, ctx=ast.Store())],
+                    value=ast.Dict(keys=dispatch_keys, values=dispatch_vals),
+                )
+            ],
+            meta_deps,
+            [
+                py_fn_node(
+                    name=name,
+                    args=ast.arguments(
+                        args=[],
+                        kwarg=None,
+                        vararg=ast.arg(arg=_MULTI_ARITY_ARG_NAME, annotation=None),
+                        kwonlyargs=[],
+                        defaults=[],
+                        kw_defaults=[],
+                    ),
+                    body=body,
+                    decorator_list=list(chain(meta_decorators, [_BASILISP_FN_FN_NAME])),
+                    returns=None,
+                )
+            ],
+        ),
     )
 
 
 @_with_ast_loc_deps
-def __multi_arity_fn_to_py_ast(
+def __multi_arity_fn_to_py_ast(  # pylint: disable=too-many-locals
     ctx: GeneratorContext,
     node: Fn,
     methods: Collection[FnMethod],
     def_name: Optional[str] = None,
+    meta_node: Optional[MetaNode] = None,
 ) -> GeneratedPyAST:
     """Return a Python AST node for a function with multiple arities."""
     assert node.op == NodeOp.FN
     assert all([method.op == NodeOp.FN_METHOD for method in methods])
 
     lisp_fn_name = node.local.name if node.local is not None else None
     py_fn_name = __fn_name(lisp_fn_name) if def_name is None else munge(def_name)
 
+    py_fn_node = ast.AsyncFunctionDef if node.is_async else ast.FunctionDef
+
     arity_to_name = {}
     rest_arity_name: Optional[str] = None
     fn_defs = []
     for method in methods:
         arity_name = f"{py_fn_name}__arity{'_rest' if method.is_variadic else method.fixed_arity}"
         if method.is_variadic:
             rest_arity_name = arity_name
@@ -938,15 +1141,15 @@
                     sym.symbol(lisp_fn_name), py_fn_name, LocalType.FN
                 )
 
             fn_args, varg, fn_body_ast = __fn_args_to_py_ast(
                 ctx, method.params, method.body
             )
             fn_defs.append(
-                ast.FunctionDef(
+                py_fn_node(
                     name=arity_name,
                     args=ast.arguments(
                         args=fn_args,
                         kwarg=None,
                         vararg=varg,
                         kwonlyargs=[],
                         defaults=[],
@@ -957,38 +1160,46 @@
                     if ctx.recur_point.has_recur
                     else [],
                     returns=None,
                 )
             )
 
     dispatch_fn_ast = __multi_arity_dispatch_fn(
+        ctx,
         py_fn_name,
         arity_to_name,
         default_name=rest_arity_name,
         max_fixed_arity=node.max_fixed_arity,
+        meta_node=meta_node,
+        is_async=node.is_async,
     )
 
     return GeneratedPyAST(
         node=dispatch_fn_ast.node,
         dependencies=list(chain(fn_defs, dispatch_fn_ast.dependencies)),
     )
 
 
 @_with_ast_loc
 def _fn_to_py_ast(
-    ctx: GeneratorContext, node: Fn, def_name: Optional[str] = None
+    ctx: GeneratorContext,
+    node: Fn,
+    def_name: Optional[str] = None,
+    meta_node: Optional[MetaNode] = None,
 ) -> GeneratedPyAST:
     """Return a Python AST Node for a `fn` expression."""
     assert node.op == NodeOp.FN
     if len(node.methods) == 1:
         return __single_arity_fn_to_py_ast(
-            ctx, node, next(iter(node.methods)), def_name=def_name
+            ctx, node, next(iter(node.methods)), def_name=def_name, meta_node=meta_node
         )
     else:
-        return __multi_arity_fn_to_py_ast(ctx, node, node.methods, def_name=def_name)
+        return __multi_arity_fn_to_py_ast(
+            ctx, node, node.methods, def_name=def_name, meta_node=meta_node
+        )
 
 
 @_with_ast_loc_deps
 def __if_body_to_py_ast(
     ctx: GeneratorContext, node: Node, result_name: str
 ) -> GeneratedPyAST:
     """Generate custom `if` nodes to handle `recur` bodies.
@@ -1078,38 +1289,42 @@
     """Return a Python AST node for a Basilisp `import*` expression."""
     assert node.op == NodeOp.IMPORT
 
     last = None
     deps: List[ast.AST] = []
     for alias in node.aliases:
         safe_name = munge(alias.name)
-        safe_alias = munge(alias.alias)
 
         try:
             module = importlib.import_module(safe_name)
-            if alias.name != alias.alias:
+            if alias.alias is not None:
                 ctx.add_import(sym.symbol(alias.name), module, sym.symbol(alias.alias))
             else:
                 ctx.add_import(sym.symbol(alias.name), module)
         except ModuleNotFoundError as e:
             raise ImportError(
                 f"Python module '{alias.name}' not found", node.form, node
             ) from e
 
+        py_import_alias = (
+            munge(alias.alias)
+            if alias.alias is not None
+            else safe_name.split(".", maxsplit=1)[0]
+        )
         deps.append(
             ast.Assign(
-                targets=[ast.Name(id=safe_alias, ctx=ast.Store())],
+                targets=[ast.Name(id=py_import_alias, ctx=ast.Store())],
                 value=ast.Call(
                     func=_load_attr("builtins.__import__"),
                     args=[ast.Str(safe_name)],
                     keywords=[],
                 ),
             )
         )
-        last = ast.Name(id=safe_alias, ctx=ast.Load())
+        last = ast.Name(id=py_import_alias, ctx=ast.Load())
 
         # Note that we add this import to the live running system in the above
         # calls to `ctx.add_import`, however, since we compile and cache Python
         # bytecode, we need to generate calls to `add_import` for the running
         # namespace so when this code is reloaded from the cache, the runtime
         # is correctly configured.
         deps.append(
@@ -1275,14 +1490,49 @@
             ),
             keywords=[],
         ),
         dependencies=recur_deps,
     )
 
 
+@_with_ast_loc
+def __deftype_method_recur_to_py_ast(
+    ctx: GeneratorContext, node: Recur
+) -> GeneratedPyAST:
+    """Return a Python AST node for `recur` occurring inside a `deftype*` method."""
+    assert node.op == NodeOp.RECUR
+    recur_nodes: List[ast.AST] = []
+    recur_deps: List[ast.AST] = []
+    for expr in node.exprs:
+        expr_ast = gen_py_ast(ctx, expr)
+        recur_nodes.append(expr_ast.node)
+        recur_deps.extend(expr_ast.dependencies)
+
+    this_entry = ctx.symbol_table.find_symbol(ctx.current_this)
+    assert this_entry is not None, "Field type local must have this"
+
+    return GeneratedPyAST(
+        node=ast.Call(
+            func=_TRAMPOLINE_ARGS_FN_NAME,
+            args=list(
+                chain(
+                    [
+                        # For the moment at least, deftype methods cannot be variadic
+                        ast.NameConstant(False),
+                        ast.Name(id=this_entry.munged, ctx=ast.Load()),
+                    ],
+                    recur_nodes,
+                )  # type: ignore
+            ),
+            keywords=[],
+        ),
+        dependencies=recur_deps,
+    )
+
+
 @_with_ast_loc_deps
 def __loop_recur_to_py_ast(ctx: GeneratorContext, node: Recur) -> GeneratedPyAST:
     """Return a Python AST node for `recur` occurring inside a `loop`."""
     assert node.op == NodeOp.RECUR
 
     recur_deps: List[ast.AST] = []
     recur_targets: List[ast.Name] = []
@@ -1306,14 +1556,15 @@
     recur_deps.append(ast.Continue())
 
     return GeneratedPyAST(node=ast.NameConstant(None), dependencies=recur_deps)
 
 
 _RECUR_TYPE_HANDLER = {
     RecurType.FN: __fn_recur_to_py_ast,
+    RecurType.METHOD: __deftype_method_recur_to_py_ast,
     RecurType.LOOP: __loop_recur_to_py_ast,
 }
 
 
 def _recur_to_py_ast(ctx: GeneratorContext, node: Recur) -> GeneratedPyAST:
     """Return a Python AST Node for a `recur` expression.
 
@@ -1347,23 +1598,20 @@
         target, (HostField, Local, VarRef)
     ), f"invalid set! target type {type(target)}"
 
     if isinstance(target, HostField):
         target_ast = _interop_prop_to_py_ast(ctx, target, is_assigning=True)
     elif isinstance(target, VarRef):
         target_ast = _var_sym_to_py_ast(ctx, target, is_assigning=True)
-    elif isinstance(target, Local):  # pragma: no cover
-        # Local nodes cannot be assigned by any existing code, but the
-        # clojure.tools.analyzer.jvm AST adds additional specialized Java
-        # nodes to the base clojure.tools.analyzer AST spec which include
-        # assignable locals (such as fields in deftype forms). I'm going
-        # to keep this branch here for now since I suspect I'll eventually
-        # enrich the AST to include assignable locals.
-        safe_name = munge(target.name)
-        target_ast = GeneratedPyAST(node=ast.Name(id=safe_name, ctx=ast.Store()))
+    elif isinstance(target, Local):
+        target_ast = _local_sym_to_py_ast(ctx, target, is_assigning=True)
+    else:  # pragma: no cover
+        raise GeneratorException(
+            f"invalid set! target type {type(target)}", lisp_ast=target
+        )
 
     return GeneratedPyAST(
         node=ast.Name(id=val_temp_name, ctx=ast.Load()),
         dependencies=list(
             chain(
                 val_ast.dependencies,
                 [
@@ -1499,19 +1747,30 @@
 ) -> GeneratedPyAST:
     """Generate a Python AST node for accessing a locally defined Python variable."""
     assert node.op == NodeOp.LOCAL
 
     sym_entry = ctx.symbol_table.find_symbol(sym.symbol(node.name))
     assert sym_entry is not None
 
-    return GeneratedPyAST(
-        node=ast.Name(
-            id=sym_entry.munged, ctx=ast.Store() if is_assigning else ast.Load()
+    if node.local == LocalType.FIELD:
+        this_entry = ctx.symbol_table.find_symbol(ctx.current_this)
+        assert this_entry is not None, "Field type local must have this"
+
+        return GeneratedPyAST(
+            node=_load_attr(
+                f"{this_entry.munged}.{sym_entry.munged}",
+                ctx=ast.Store() if is_assigning else ast.Load(),
+            )
+        )
+    else:
+        return GeneratedPyAST(
+            node=ast.Name(
+                id=sym_entry.munged, ctx=ast.Store() if is_assigning else ast.Load()
+            )
         )
-    )
 
 
 def __var_find_to_py_ast(
     var_name: str, ns_name: str, py_var_ctx: ast.AST
 ) -> GeneratedPyAST:
     """Generate Var.find calls for the named symbol."""
     return GeneratedPyAST(
@@ -1657,17 +1916,14 @@
 
 
 #########################
 # Non-Quoted Collections
 #########################
 
 
-MetaNode = Union[Const, MapNode]
-
-
 @_with_ast_loc
 def _map_to_py_ast(
     ctx: GeneratorContext, node: MapNode, meta_node: Optional[MetaNode] = None
 ) -> GeneratedPyAST:
     assert node.op == NodeOp.MAP
 
     if meta_node is not None:
@@ -1748,36 +2004,83 @@
                 Maybe(meta_ast).map(lambda p: list(p.dependencies)).or_else_get([]),
                 elem_deps,
             )
         ),
     )
 
 
+#####################
+# Python Collections
+#####################
+
+
+@_with_ast_loc
+def _py_dict_to_py_ast(ctx: GeneratorContext, node: PyDict) -> GeneratedPyAST:
+    assert node.op == NodeOp.PY_DICT
+
+    key_deps, keys = _chain_py_ast(*map(partial(gen_py_ast, ctx), node.keys))
+    val_deps, vals = _chain_py_ast(*map(partial(gen_py_ast, ctx), node.vals))
+    return GeneratedPyAST(
+        node=ast.Dict(keys=list(keys), values=list(vals)),
+        dependencies=list(chain(key_deps, val_deps)),
+    )
+
+
+@_with_ast_loc
+def _py_list_to_py_ast(ctx: GeneratorContext, node: PyList) -> GeneratedPyAST:
+    assert node.op == NodeOp.PY_LIST
+
+    elem_deps, elems = _chain_py_ast(*map(partial(gen_py_ast, ctx), node.items))
+    return GeneratedPyAST(
+        node=ast.List(elts=list(elems), ctx=ast.Load()), dependencies=list(elem_deps)
+    )
+
+
+@_with_ast_loc
+def _py_set_to_py_ast(ctx: GeneratorContext, node: PySet) -> GeneratedPyAST:
+    assert node.op == NodeOp.PY_SET
+
+    elem_deps, elems = _chain_py_ast(*map(partial(gen_py_ast, ctx), node.items))
+    return GeneratedPyAST(node=ast.Set(elts=list(elems)), dependencies=list(elem_deps))
+
+
+@_with_ast_loc
+def _py_tuple_to_py_ast(ctx: GeneratorContext, node: PyTuple) -> GeneratedPyAST:
+    assert node.op == NodeOp.PY_TUPLE
+
+    elem_deps, elems = _chain_py_ast(*map(partial(gen_py_ast, ctx), node.items))
+    return GeneratedPyAST(
+        node=ast.Tuple(elts=list(elems), ctx=ast.Load()), dependencies=list(elem_deps)
+    )
+
+
 ############
 # With Meta
 ############
 
 
 _WITH_META_EXPR_HANDLER = {  # type: ignore
-    NodeOp.FN: None,  # TODO: function with meta
+    NodeOp.FN: _fn_to_py_ast,
     NodeOp.MAP: _map_to_py_ast,
     NodeOp.SET: _set_to_py_ast,
     NodeOp.VECTOR: _vec_to_py_ast,
 }
 
 
-def _with_meta_to_py_ast(ctx: GeneratorContext, node: WithMeta) -> GeneratedPyAST:
+def _with_meta_to_py_ast(
+    ctx: GeneratorContext, node: WithMeta, **kwargs
+) -> GeneratedPyAST:
     """Generate a Python AST node for Python interop method calls."""
     assert node.op == NodeOp.WITH_META
 
     handle_expr = _WITH_META_EXPR_HANDLER.get(node.expr.op)
     assert (
         handle_expr is not None
     ), "No expression handler for with-meta child node type"
-    return handle_expr(ctx, node.expr, meta_node=node.meta)  # type: ignore
+    return handle_expr(ctx, node.expr, meta_node=node.meta, **kwargs)  # type: ignore
 
 
 #################
 # Constant Nodes
 #################
 
 
@@ -1867,14 +2170,42 @@
 
 
 @_simple_ast_generator
 def _uuid_to_py_ast(_: GeneratorContext, form: uuid.UUID) -> ast.AST:
     return ast.Call(func=_NEW_UUID_FN_NAME, args=[ast.Str(str(form))], keywords=[])
 
 
+def _const_py_dict_to_py_ast(ctx: GeneratorContext, node: dict) -> GeneratedPyAST:
+    key_deps, keys = _chain_py_ast(*_collection_literal_to_py_ast(ctx, node.keys()))
+    val_deps, vals = _chain_py_ast(*_collection_literal_to_py_ast(ctx, node.values()))
+    return GeneratedPyAST(
+        node=ast.Dict(keys=list(keys), values=list(vals)),
+        dependencies=list(chain(key_deps, val_deps)),
+    )
+
+
+def _const_py_list_to_py_ast(ctx: GeneratorContext, node: list) -> GeneratedPyAST:
+    elem_deps, elems = _chain_py_ast(*_collection_literal_to_py_ast(ctx, node))
+    return GeneratedPyAST(
+        node=ast.List(elts=list(elems), ctx=ast.Load()), dependencies=list(elem_deps)
+    )
+
+
+def _const_py_set_to_py_ast(ctx: GeneratorContext, node: set) -> GeneratedPyAST:
+    elem_deps, elems = _chain_py_ast(*_collection_literal_to_py_ast(ctx, node))
+    return GeneratedPyAST(node=ast.Set(elts=list(elems)), dependencies=list(elem_deps))
+
+
+def _const_py_tuple_to_py_ast(ctx: GeneratorContext, node: tuple) -> GeneratedPyAST:
+    elem_deps, elems = _chain_py_ast(*_collection_literal_to_py_ast(ctx, node))
+    return GeneratedPyAST(
+        node=ast.Tuple(elts=list(elems), ctx=ast.Load()), dependencies=list(elem_deps)
+    )
+
+
 def _const_map_to_py_ast(ctx: GeneratorContext, form: lmap.Map) -> GeneratedPyAST:
     key_deps, keys = _chain_py_ast(*_collection_literal_to_py_ast(ctx, form.keys()))
     val_deps, vals = _chain_py_ast(*_collection_literal_to_py_ast(ctx, form.values()))
     meta = _const_meta_kwargs_ast(ctx, form)
     return GeneratedPyAST(
         node=ast.Call(
             func=_NEW_MAP_FN_NAME,
@@ -1947,25 +2278,29 @@
 
 
 _CONST_VALUE_HANDLERS: Dict[Type, SimplePyASTGenerator] = {  # type: ignore
     bool: _name_const_to_py_ast,
     complex: _num_to_py_ast,
     datetime: _inst_to_py_ast,
     Decimal: _decimal_to_py_ast,
+    dict: _const_py_dict_to_py_ast,
     float: _num_to_py_ast,
     Fraction: _fraction_to_py_ast,
     int: _num_to_py_ast,
     kw.Keyword: _kw_to_py_ast,
+    list: _const_py_list_to_py_ast,
     llist.List: _const_seq_to_py_ast,
     lmap.Map: _const_map_to_py_ast,
     lset.Set: _const_set_to_py_ast,
     lseq.Seq: _const_seq_to_py_ast,
     type(re.compile("")): _regex_to_py_ast,
+    set: _const_py_set_to_py_ast,
     sym.Symbol: _const_sym_to_py_ast,
     str: _str_to_py_ast,
+    tuple: _const_py_tuple_to_py_ast,
     type(None): _name_const_to_py_ast,
     uuid.UUID: _uuid_to_py_ast,
     vec.Vector: _const_vec_to_py_ast,
 }
 
 
 def _const_val_to_py_ast(ctx: GeneratorContext, form: LispForm) -> GeneratedPyAST:
@@ -2004,14 +2339,18 @@
     ConstType.SET: _const_set_to_py_ast,
     ConstType.SEQ: _const_seq_to_py_ast,
     ConstType.REGEX: _regex_to_py_ast,
     ConstType.SYMBOL: _const_sym_to_py_ast,
     ConstType.STRING: _str_to_py_ast,
     ConstType.NIL: _name_const_to_py_ast,
     ConstType.UUID: _uuid_to_py_ast,
+    ConstType.PY_DICT: _const_py_dict_to_py_ast,
+    ConstType.PY_LIST: _const_py_list_to_py_ast,
+    ConstType.PY_SET: _const_py_set_to_py_ast,
+    ConstType.PY_TUPLE: _const_py_tuple_to_py_ast,
     ConstType.VECTOR: _const_vec_to_py_ast,
 }
 
 
 @_with_ast_loc
 def _const_node_to_py_ast(ctx: GeneratorContext, lisp_ast: Const) -> GeneratedPyAST:
     """Generate Python AST nodes for a :const Lisp AST node.
@@ -2024,30 +2363,36 @@
     handle_const_node = _CONSTANT_HANDLER.get(node_type)
     assert handle_const_node is not None, f"No :const AST type handler for {node_type}"
     node_val = lisp_ast.val
     return handle_const_node(ctx, node_val)
 
 
 _NODE_HANDLERS: Dict[NodeOp, PyASTGenerator] = {  # type: ignore
+    NodeOp.AWAIT: _await_to_py_ast,
     NodeOp.CONST: _const_node_to_py_ast,
     NodeOp.DEF: _def_to_py_ast,
+    NodeOp.DEFTYPE: _deftype_to_py_ast,
     NodeOp.DO: _do_to_py_ast,
     NodeOp.FN: _fn_to_py_ast,
     NodeOp.HOST_CALL: _interop_call_to_py_ast,
     NodeOp.HOST_FIELD: _interop_prop_to_py_ast,
     NodeOp.IF: _if_to_py_ast,
     NodeOp.IMPORT: _import_to_py_ast,
     NodeOp.INVOKE: _invoke_to_py_ast,
     NodeOp.LET: _let_to_py_ast,
     NodeOp.LETFN: None,
     NodeOp.LOCAL: _local_sym_to_py_ast,
     NodeOp.LOOP: _loop_to_py_ast,
     NodeOp.MAP: _map_to_py_ast,
     NodeOp.MAYBE_CLASS: _maybe_class_to_py_ast,
     NodeOp.MAYBE_HOST_FORM: _maybe_host_form_to_py_ast,
+    NodeOp.PY_DICT: _py_dict_to_py_ast,
+    NodeOp.PY_LIST: _py_list_to_py_ast,
+    NodeOp.PY_SET: _py_set_to_py_ast,
+    NodeOp.PY_TUPLE: _py_tuple_to_py_ast,
     NodeOp.QUOTE: _quote_to_py_ast,
     NodeOp.RECUR: _recur_to_py_ast,
     NodeOp.SET: _set_to_py_ast,
     NodeOp.SET_BANG: _set_bang_to_py_ast,
     NodeOp.THROW: _throw_to_py_ast,
     NodeOp.TRY: _try_to_py_ast,
     NodeOp.VAR: _var_sym_to_py_ast,
@@ -2110,17 +2455,15 @@
         module="basilisp.lang.runtime",
         names=[ast.alias(name="Var", asname=_VAR_ALIAS)],
         level=0,
     )
 
 
 def _ns_var(
-    py_ns_var: str = _NS_VAR,
-    lisp_ns_var: str = _LISP_NS_VAR,
-    lisp_ns_ns: str = _CORE_NS,
+    py_ns_var: str = _NS_VAR, lisp_ns_var: str = LISP_NS_VAR, lisp_ns_ns: str = CORE_NS
 ) -> ast.Assign:
     """Assign a Python variable named `ns_var` to the value of the current
     namespace."""
     return ast.Assign(
         targets=[ast.Name(id=py_ns_var, ctx=ast.Store())],
         value=ast.Call(
             func=_FIND_VAR_FN_NAME,
```

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/optimizer.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/optimizer.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/lang/compiler/nodes.py` & `basilisp-0.1.dev9/src/basilisp/lang/compiler/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import (
+    Any,
+    Callable,
     Collection,
-    Union,
-    Optional,
-    Iterable,
+    Dict,
     Generic,
-    TypeVar,
-    Callable,
+    Iterable,
+    Optional,
     Tuple,
-    Dict,
+    TypeVar,
+    Union,
 )
 
 import attr
 
 import basilisp.lang.keyword as kw
-import basilisp.lang.list as llist
 import basilisp.lang.map as lmap
-import basilisp.lang.seq as lseq
 import basilisp.lang.set as lset
 import basilisp.lang.symbol as sym
 import basilisp.lang.vector as vec
-from basilisp.lang.runtime import Namespace, Var
-from basilisp.lang.typing import LispForm
+from basilisp.lang.runtime import Namespace, Var, to_lisp
+from basilisp.lang.typing import LispForm, ReaderForm as ReaderLispForm, SpecialForm
 from basilisp.lang.util import munge
 
 BODY = kw.keyword("body")
 CLASS = kw.keyword("class")
 LOCAL = kw.keyword("local")
 STATEMENTS = kw.keyword("statements")
 RET = kw.keyword("ret")
+THIS_LOCAL = kw.keyword("this-local")
+FIELDS = kw.keyword("fields")
 METHODS = kw.keyword("methods")
 PARAMS = kw.keyword("params")
 TARGET = kw.keyword("target")
 VAL = kw.keyword("val")
 ARGS = kw.keyword("args")
 FN = kw.keyword("fn")
 BINDINGS = kw.keyword("bindings")
@@ -46,18 +47,20 @@
 META = kw.keyword("meta")
 TEST = kw.keyword("test")
 THEN = kw.keyword("then")
 ELSE = kw.keyword("else")
 
 
 class NodeOp(Enum):
+    AWAIT = kw.keyword("await")
     BINDING = kw.keyword("binding")
     CATCH = kw.keyword("catch")
     CONST = kw.keyword("const")
     DEF = kw.keyword("def")
+    DEFTYPE = kw.keyword("deftype")
     DO = kw.keyword("do")
     FN = kw.keyword("fn")
     FN_METHOD = kw.keyword("fn-method")
     HOST_CALL = kw.keyword("host-call")
     HOST_FIELD = kw.keyword("host-field")
     HOST_INTEROP = kw.keyword("host-interop")
     IF = kw.keyword("if")
@@ -67,14 +70,19 @@
     LET = kw.keyword("let")
     LETFN = kw.keyword("letfn")
     LOCAL = kw.keyword("local")
     LOOP = kw.keyword("loop")
     MAP = kw.keyword("map")
     MAYBE_CLASS = kw.keyword("maybe-class")
     MAYBE_HOST_FORM = kw.keyword("maybe-host-form")
+    METHOD = kw.keyword("method")
+    PY_DICT = kw.keyword("py-dict")
+    PY_LIST = kw.keyword("py-list")
+    PY_SET = kw.keyword("py-set")
+    PY_TUPLE = kw.keyword("py-tuple")
     QUOTE = kw.keyword("quote")
     RECUR = kw.keyword("recur")
     SET = kw.keyword("set")
     SET_BANG = kw.keyword("set!")
     THROW = kw.keyword("throw")
     TRY = kw.keyword("try")
     VAR = kw.keyword("var")
@@ -114,14 +122,17 @@
         raise NotImplementedError()
 
     @property
     @abstractmethod
     def env(self) -> "NodeEnv":
         raise NotImplementedError()
 
+    def to_map(self) -> lmap.Map:
+        return to_lisp(attr.asdict(self))
+
     def assoc(self, **kwargs):
         return attr.evolve(self, **kwargs)
 
     def visit(self, f: Callable[..., None], *args, **kwargs):
         """Visit all immediate children of this node, calling
         f(child, *args, **kwargs) on each child."""
         for child_kw in self.children:
@@ -200,48 +211,65 @@
     RECORD = kw.keyword("record")
     SEQ = kw.keyword("seq")
     CHAR = kw.keyword("char")
     REGEX = kw.keyword("regex")
     CLASS = kw.keyword("class")
     INST = kw.keyword("inst")
     UUID = kw.keyword("uuid")
+    PY_DICT = kw.keyword("py-dict")
+    PY_LIST = kw.keyword("py-list")
+    PY_SET = kw.keyword("py-set")
+    PY_TUPLE = kw.keyword("py-tuple")
     UNKNOWN = kw.keyword("unknown")
 
 
 NodeMeta = Union[None, "Const", "Map"]
-ReaderLispForm = Union[LispForm, lseq.Seq]
-SpecialForm = Union[llist.List, lseq.Seq]
 LoopID = str
 
 
 class LocalType(Enum):
     ARG = kw.keyword("arg")
     CATCH = kw.keyword("catch")
+    DEFTYPE = kw.keyword("deftype")
+    FIELD = kw.keyword("field")
     FN = kw.keyword("fn")
     LET = kw.keyword("let")
     LETFN = kw.keyword("letfn")
     LOOP = kw.keyword("loop")
+    THIS = kw.keyword("this")
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class NodeEnv:
     ns: Namespace
     file: str
     line: Optional[int] = None
     col: Optional[int] = None
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
-class Binding(Node[sym.Symbol]):
+class Await(Node[ReaderLispForm]):
+    form: ReaderLispForm
+    expr: Node
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(EXPR)
+    op: NodeOp = NodeOp.AWAIT
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, frozen=True, slots=True)
+class Binding(Node[sym.Symbol], Assignable):
     form: sym.Symbol
     name: str
     local: LocalType
     env: NodeEnv
     arg_id: Optional[int] = None
     is_variadic: bool = False
+    is_assignable: bool = False
     init: Optional[Node] = None
     meta: NodeMeta = None
     children: Collection[kw.Keyword] = vec.Vector.empty()
     op: NodeOp = NodeOp.BINDING
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
@@ -284,14 +312,33 @@
     meta: NodeMeta = None
     children: Collection[kw.Keyword] = vec.Vector.empty()
     op: NodeOp = NodeOp.DEF
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
+DefTypeBase = Union["MaybeClass", "MaybeHostForm", "VarRef"]
+
+
+@attr.s(auto_attribs=True, frozen=True, slots=True)
+class DefType(Node[SpecialForm]):
+    form: SpecialForm
+    name: str
+    interfaces: Iterable[DefTypeBase]
+    fields: Iterable[Binding]
+    methods: Iterable["Method"]
+    env: NodeEnv
+    is_frozen: bool = True
+    meta: NodeMeta = None
+    children: Collection[kw.Keyword] = vec.v(FIELDS, METHODS)
+    op: NodeOp = NodeOp.DEFTYPE
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Do(Node[SpecialForm]):
     form: SpecialForm
     statements: Iterable[Node]
     ret: Node
     env: NodeEnv
     is_body: bool = False
@@ -305,14 +352,15 @@
 class Fn(Node[SpecialForm]):
     form: SpecialForm
     max_fixed_arity: int
     methods: Collection["FnMethod"]
     env: NodeEnv
     local: Optional[Binding] = None
     is_variadic: bool = False
+    is_async: bool = False
     children: Collection[kw.Keyword] = vec.v(METHODS)
     op: NodeOp = NodeOp.FN
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
@@ -380,15 +428,15 @@
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class ImportAlias(Node[Union[sym.Symbol, vec.Vector]]):
     form: Union[sym.Symbol, vec.Vector]
     name: str
-    alias: str
+    alias: Optional[str]
     env: NodeEnv
     children: Collection[kw.Keyword] = vec.Vector.empty()
     op: NodeOp = NodeOp.IMPORT_ALIAS
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
@@ -468,34 +516,97 @@
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class MaybeClass(Node[sym.Symbol]):
     form: sym.Symbol
     class_: str
+    target: Any
     env: NodeEnv
     children: Collection[kw.Keyword] = vec.Vector.empty()
     op: NodeOp = NodeOp.MAYBE_CLASS
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class MaybeHostForm(Node[sym.Symbol]):
     form: sym.Symbol
     class_: str
     field: str
+    target: Any
     env: NodeEnv
     children: Collection[kw.Keyword] = vec.Vector.empty()
     op: NodeOp = NodeOp.MAYBE_HOST_FORM
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
+class Method(Node[SpecialForm]):
+    form: SpecialForm
+    name: str
+    interface: DefTypeBase
+    this_local: Binding
+    loop_id: LoopID
+    params: Iterable[Binding]
+    body: Do
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(THIS_LOCAL, PARAMS, BODY)
+    op: NodeOp = NodeOp.METHOD
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, cmp=False, frozen=True, slots=True)
+class PyDict(Node[dict]):
+    form: dict
+    keys: Iterable[Node]
+    vals: Iterable[Node]
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(KEYS, VALS)
+    op: NodeOp = NodeOp.PY_DICT
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, cmp=False, frozen=True, slots=True)
+class PyList(Node[list]):
+    form: list
+    items: Iterable[Node]
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(ITEMS)
+    op: NodeOp = NodeOp.PY_LIST
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, cmp=False, frozen=True, slots=True)
+class PySet(Node[Union[frozenset, set]]):
+    form: Union[frozenset, set]
+    items: Iterable[Node]
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(ITEMS)
+    op: NodeOp = NodeOp.PY_SET
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, frozen=True, slots=True)
+class PyTuple(Node[tuple]):
+    form: tuple
+    items: Iterable[Node]
+    env: NodeEnv
+    children: Collection[kw.Keyword] = vec.v(ITEMS)
+    op: NodeOp = NodeOp.PY_TUPLE
+    top_level: bool = False
+    raw_forms: Collection[LispForm] = vec.Vector.empty()
+
+
+@attr.s(auto_attribs=True, frozen=True, slots=True)
 class Quote(Node[SpecialForm]):
     form: SpecialForm
     expr: Const
     env: NodeEnv
     is_literal: bool = True
     children: Collection[kw.Keyword] = vec.v(EXPR)
     op: NodeOp = NodeOp.QUOTE
@@ -598,14 +709,15 @@
     children: Collection[kw.Keyword] = vec.v(META, EXPR)
     op: NodeOp = NodeOp.WITH_META
     top_level: bool = False
     raw_forms: Collection[LispForm] = vec.Vector.empty()
 
 
 ParentNode = Union[
+    Await,
     Const,
     Def,
     Do,
     Fn,
     HostCall,
     HostField,
     If,
@@ -613,27 +725,33 @@
     Invoke,
     Let,
     LetFn,
     Loop,
     Map,
     MaybeClass,
     MaybeHostForm,
+    PyDict,
+    PyList,
+    PySet,
+    PyTuple,
     Quote,
     Set,
     SetBang,
     Throw,
     Try,
     VarRef,
     Vector,
     WithMeta,
 ]
 ChildOnlyNode = Union[Binding, Catch, FnMethod, ImportAlias, Local, Recur]
 AnyNode = Union[ParentNode, ChildOnlyNode]
 SpecialFormNode = Union[
+    Await,
     Def,
+    DefType,
     Do,
     Fn,
     If,
     HostCall,
     HostField,
     Import,
     Invoke,
```

### Comparing `basilisp-0.1.dev8/src/basilisp/test.lpy` & `basilisp-0.1.dev9/src/basilisp/test.lpy`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/cli.py` & `basilisp-0.1.dev9/src/basilisp/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,74 @@
+import atexit
 import importlib
-
-# noinspection PyUnresolvedReferences
-import readline  # noqa: F401
+import os.path
+import platform
 import traceback
 import types
 from typing import Any
 
 import click
 import pytest
 
 import basilisp.lang.compiler as compiler
 import basilisp.lang.reader as reader
 import basilisp.lang.runtime as runtime
 import basilisp.lang.symbol as sym
 import basilisp.main as basilisp
 
 CLI_INPUT_FILE_PATH = "<CLI Input>"
+BASILISP_REPL_HISTORY_FILE_PATH = os.path.join(
+    os.path.expanduser("~"), ".basilisp_history"
+)
+BASILISP_REPL_HISTORY_LENGTH = 1000
 REPL_INPUT_FILE_PATH = "<REPL Input>"
+STDIN_INPUT_FILE_PATH = "<stdin>"
+STDIN_FILE_NAME = "-"
+
+
+try:
+    import readline
+except ImportError:  # pragma: no cover
+    pass
+else:
+    readline.parse_and_bind("tab: complete")
+    readline.set_completer_delims("()[]{} \n\t")
+    readline.set_completer(runtime.repl_complete)
+
+    try:
+        readline.read_history_file(BASILISP_REPL_HISTORY_FILE_PATH)
+        readline.set_history_length(BASILISP_REPL_HISTORY_LENGTH)
+    except FileNotFoundError:  # pragma: no cover
+        pass
+    except Exception:  # noqa  # pragma: no cover
+        # PyPy 3.6's ncurses implementation throws an error here
+        if platform.python_implementation() != "PyPy":
+            raise
+    else:
+        atexit.register(readline.write_history_file, BASILISP_REPL_HISTORY_FILE_PATH)
 
 
 @click.group()
 def cli():
     """Basilisp is a Lisp dialect inspired by Clojure targeting Python 3."""
-    pass
 
 
 def eval_file(filename: str, ctx: compiler.CompilerContext, module: types.ModuleType):
     """Evaluate a file with the given name into a Python module AST node."""
     last = None
     for form in reader.read_file(filename, resolver=runtime.resolve_alias):
-        last = compiler.compile_and_exec_form(form, ctx, module, filename)
+        last = compiler.compile_and_exec_form(form, ctx, module)
+    return last
+
+
+def eval_stream(stream, ctx: compiler.CompilerContext, module: types.ModuleType):
+    """Evaluate the forms in stdin into a Python module AST node."""
+    last = None
+    for form in reader.read(stream, resolver=runtime.resolve_alias):
+        last = compiler.compile_and_exec_form(form, ctx, module)
     return last
 
 
 def eval_str(s: str, ctx: compiler.CompilerContext, module: types.ModuleType, eof: Any):
     """Evaluate the forms in a string into a Python module AST node."""
     last = eof
     for form in reader.read_str(s, resolver=runtime.resolve_alias, eof=eof):
@@ -52,15 +87,15 @@
     ns.refer_all(repl_ns)
     return repl_module
 
 
 @cli.command(short_help="start the Basilisp REPL")
 @click.option(
     "--default-ns",
-    default=runtime._REPL_DEFAULT_NS,
+    default=runtime.REPL_DEFAULT_NS,
     help="default namespace to use for the REPL",
 )
 @click.option(
     "--use-var-indirection",
     default=False,
     is_flag=True,
     envvar="BASILISP_USE_VAR_INDIRECTION",
@@ -109,24 +144,24 @@
     eof = object()
     while True:
         ns: runtime.Namespace = ns_var.value
         try:
             lsrc = input(f"{ns.name}=> ")
         except EOFError:
             break
-        except KeyboardInterrupt:
+        except KeyboardInterrupt:  # pragma: no cover
             print("")
             continue
 
         if len(lsrc) == 0:
             continue
 
         try:
             result = eval_str(lsrc, ctx, ns.module, eof)
-            if result is eof:
+            if result is eof:  # pragma: no cover
                 continue
             print(runtime.lrepr(result))
             repl_module.mark_repl_result(result)
         except reader.SyntaxError as e:
             traceback.print_exception(reader.SyntaxError, e, e.__traceback__)
             repl_module.mark_exception(e)
             continue
@@ -142,15 +177,15 @@
 
 @cli.command(short_help="run a Basilisp script or code")
 @click.argument("file-or-code")
 @click.option(
     "-c", "--code", is_flag=True, help="if provided, treat argument as a string of code"
 )
 @click.option(
-    "--in-ns", default=runtime._REPL_DEFAULT_NS, help="namespace to use for the code"
+    "--in-ns", default=runtime.REPL_DEFAULT_NS, help="namespace to use for the code"
 )
 @click.option(
     "--use-var-indirection",
     default=False,
     is_flag=True,
     envvar="BASILISP_USE_VAR_INDIRECTION",
     help="if provided, all Var accesses will be performed via Var indirection",
@@ -184,33 +219,50 @@
     warn_on_shadowed_name,
     warn_on_shadowed_var,
     warn_on_var_indirection,
 ):
     """Run a Basilisp script or a line of code, if it is provided."""
     basilisp.init()
     ctx = compiler.CompilerContext(
-        filename=CLI_INPUT_FILE_PATH if code else file_or_code,
+        filename=CLI_INPUT_FILE_PATH
+        if code
+        else (
+            STDIN_INPUT_FILE_PATH if file_or_code == STDIN_FILE_NAME else file_or_code
+        ),
         opts={
             compiler.WARN_ON_SHADOWED_NAME: warn_on_shadowed_name,
             compiler.WARN_ON_SHADOWED_VAR: warn_on_shadowed_var,
             compiler.USE_VAR_INDIRECTION: use_var_indirection,
             compiler.WARN_ON_VAR_INDIRECTION: warn_on_var_indirection,
         },
     )
     eof = object()
 
     with runtime.ns_bindings(in_ns) as ns:
         if code:
             print(runtime.lrepr(eval_str(file_or_code, ctx, ns.module, eof)))
+        elif file_or_code == STDIN_FILE_NAME:
+            print(
+                runtime.lrepr(
+                    eval_stream(click.get_text_stream("stdin"), ctx, ns.module)
+                )
+            )
         else:
             print(runtime.lrepr(eval_file(file_or_code, ctx, ns.module)))
 
 
 @cli.command(short_help="run tests in a Basilisp project")
 @click.argument("args", nargs=-1)
-def test(args):
+def test(args):  # pragma: no cover
     """Run tests in a Basilisp project."""
     pytest.main(args=list(args))
 
 
+@cli.command(short_help="print the version of Basilisp")
+def version():
+    from basilisp.__version__ import __version__
+
+    print(f"Basilisp {__version__}")
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `basilisp-0.1.dev8/src/basilisp/logconfig.py` & `basilisp-0.1.dev9/src/basilisp/logconfig.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/string.lpy` & `basilisp-0.1.dev9/src/basilisp/string.lpy`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/repl.lpy` & `basilisp-0.1.dev9/src/basilisp/repl.lpy`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp/testrunner.py` & `basilisp-0.1.dev9/src/basilisp/testrunner.py`

 * *Files identical despite different names*

### Comparing `basilisp-0.1.dev8/src/basilisp.egg-info/PKG-INFO` & `basilisp-0.1.dev9/src/basilisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basilisp
-Version: 0.1.dev8
+Version: 0.1.dev9
 Summary: A Clojure-like lisp written for Python
 Home-page: http://github.com/chrisrink10/basilisp
 Author: Christopher Rink
 Author-email: chrisrink10@gmail.com
 License: Eclipse Public License 1.0
 Description: 
         # 🐍 basilisp 🐍
```

### Comparing `basilisp-0.1.dev8/src/basilisp.egg-info/SOURCES.txt` & `basilisp-0.1.dev9/src/basilisp.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 src/basilisp/walker.py
 src/basilisp.egg-info/PKG-INFO
 src/basilisp.egg-info/SOURCES.txt
 src/basilisp.egg-info/dependency_links.txt
 src/basilisp.egg-info/entry_points.txt
 src/basilisp.egg-info/requires.txt
 src/basilisp.egg-info/top_level.txt
+src/basilisp/__pycache__/repl.cpython-36.lpyc
+src/basilisp/__pycache__/test.cpython-36.lpyc
 src/basilisp/core/__init__.lpy
+src/basilisp/core/__pycache__/__init__.cpython-36.lpyc
 src/basilisp/lang/__init__.py
 src/basilisp/lang/associative.py
 src/basilisp/lang/atom.py
 src/basilisp/lang/collection.py
 src/basilisp/lang/delay.py
 src/basilisp/lang/deref.py
 src/basilisp/lang/exception.py
```

