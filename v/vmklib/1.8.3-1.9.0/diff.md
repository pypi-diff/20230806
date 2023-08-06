# Comparing `tmp/vmklib-1.8.3.tar.gz` & `tmp/vmklib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmklib-1.8.3.tar", last modified: Tue Jun 20 07:45:59 2023, max compression
+gzip compressed data, was "vmklib-1.9.0.tar", last modified: Wed Jul 12 21:50:16 2023, max compression
```

## Comparing `vmklib-1.8.3.tar` & `vmklib-1.9.0.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.542767 vmklib-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 07:43:08.000000 vmklib-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-06-20 07:45:59.542767 vmklib-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-06-20 07:43:08.000000 vmklib-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-20 07:43:08.000000 vmklib-1.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:45:59.542767 vmklib-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 07:43:08.000000 vmklib-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.534767 vmklib-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-20 07:43:08.000000 vmklib-1.8.3/tests/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.534767 vmklib-1.8.3/vmklib/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/conf.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/data/edit_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/data/fresh_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/data/header.mk
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/datazen.mk
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/functions.mk
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/grip.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/data/lib_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/lib_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/data/lib_tasks/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-20 07:43:21.000000 vmklib-1.8.3/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/lib_tasks/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/python/build.mk
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/python/docs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/python/pypi.mk
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/python/upload.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/python.mk
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/time.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/venv.mk
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/vmklib.mk
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/data/yaml.mk
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/tasks/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/mixins/concrete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.538767 vmklib-1.8.3/vmklib/tasks/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.542767 vmklib-1.8.3/vmklib/tasks/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/datazen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/python/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-20 07:43:08.000000 vmklib-1.8.3/vmklib/tasks/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:45:59.534767 vmklib-1.8.3/vmklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 07:45:59.000000 vmklib-1.8.3/vmklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.962616 vmklib-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 21:47:23.000000 vmklib-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-12 21:50:16.958615 vmklib-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-12 21:47:23.000000 vmklib-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 21:47:23.000000 vmklib-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:50:16.962616 vmklib-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-12 21:47:23.000000 vmklib-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-12 21:47:23.000000 vmklib-1.9.0/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/conf.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/edit_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/fresh_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/data/header.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/datazen.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/functions.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/grip.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/lib_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/lib_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-12 21:47:37.000000 vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/lib_tasks/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/build.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/docs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/pypi.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python/upload.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/python.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/time.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/venv.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/vmklib.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/data/yaml.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/concrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/mixins/curl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.958615 vmklib-1.9.0/vmklib/tasks/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/datazen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/python/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-12 21:47:23.000000 vmklib-1.9.0/vmklib/tasks/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:50:16.954615 vmklib-1.9.0/vmklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 21:50:16.000000 vmklib-1.9.0/vmklib.egg-info/top_level.txt
```

### Comparing `vmklib-1.8.3/LICENSE` & `vmklib-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/PKG-INFO` & `vmklib-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.3
+Version: 1.9.0
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -26,39 +26,38 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: workflow,tool,make
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=84b7fe19dafb7682480119b63d53aa24
+    hash=1280d00c2447ef272e48abbae9617e0a
     =====================================
 -->
 
-# vmklib ([1.8.3](https://pypi.org/project/vmklib/))
+# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -67,15 +66,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vmklib-1.8.3/README.md` & `vmklib-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=84b7fe19dafb7682480119b63d53aa24
+    hash=1280d00c2447ef272e48abbae9617e0a
     =====================================
 -->
 
-# vmklib ([1.8.3](https://pypi.org/project/vmklib/))
+# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -19,15 +19,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vmklib-1.8.3/pyproject.toml` & `vmklib-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vmklib"
-version = "1.8.3"
+version = "1.9.0"
 description = "Simplify project workflows by standardizing use of GNU Make."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = [
   "workflow",
   "tool",
   "make"
 ]
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
   "Topic :: Software Development :: Build Tools",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
```

### Comparing `vmklib-1.8.3/setup.py` & `vmklib-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=ab812b89eee40b1fec8ddff61dc0552a
+# hash=c29553a5eb8c58f39d08f72dfa51d217
 # =====================================
 
 """
 vmklib - Package definition for distribution.
 """
 
 # third-party
@@ -24,15 +24,14 @@
 }
 pkg_info = {
     "name": PKG_NAME,
     "slug": PKG_NAME.replace("-", "_"),
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
-        "3.7",
         "3.8",
         "3.9",
         "3.10",
         "3.11",
     ],
 }
 setup(
```

### Comparing `vmklib-1.8.3/tests/test_entry.py` & `vmklib-1.9.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/app.py` & `vmklib-1.9.0/vmklib/app.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/conf.mk` & `vmklib-1.9.0/vmklib/data/conf.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/data/header.mk` & `vmklib-1.9.0/vmklib/data/data/header.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/datazen.mk` & `vmklib-1.9.0/vmklib/data/datazen.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/functions.mk` & `vmklib-1.9.0/vmklib/data/functions.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/grip.mk` & `vmklib-1.9.0/vmklib/data/grip.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc` & `vmklib-1.9.0/vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 07:43:08 2023 UTC, .py size: 2374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,201 @@
-00000000: 550d 0d0a 0000 0000 8c58 9164 4609 0000  U........X.dF...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
-00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0f  m.Z...d.d.l.m.Z.
-00000080: 0100 6401 6408 6c10 6d11 5a11 6d12 5a12  ..d.d.l.m.Z.m.Z.
-00000090: 0100 6401 6407 6c13 6d0e 5a14 0100 6401  ..d.d.l.m.Z...d.
-000000a0: 6407 6c15 6d0e 5a16 0100 6401 6407 6c17  d.l.m.Z...d.d.l.
-000000b0: 6d0e 5a18 0100 6401 6407 6c19 6d0e 5a1a  m.Z...d.d.l.m.Z.
-000000c0: 0100 6401 6407 6c1b 6d0e 5a1c 0100 6401  ..d.d.l.m.Z...d.
-000000d0: 6407 6c1d 6d0e 5a1e 0100 6401 6407 6c1f  d.l.m.Z...d.d.l.
-000000e0: 6d0e 5a20 0100 6401 6407 6c21 6d0e 5a22  m.Z ..d.d.l!m.Z"
-000000f0: 0100 6401 6407 6c23 6d0e 5a24 0100 4700  ..d.d.l#m.Z$..G.
-00000100: 6409 640a 8400 640a 6508 8303 5a25 650c  d.d...d.e...Z%e.
-00000110: 6526 6502 6504 6526 6526 6602 1900 6527  e&e.e.e&e&f...e'
-00000120: 640b 9c05 640c 640d 8404 5a0e 640e 5300  d...d.d...Z.d.S.
-00000130: 290f 7a29 0a41 206d 6f64 756c 6520 666f  ).z).A module fo
-00000140: 7220 7265 6769 7374 6572 696e 6720 7061  r registering pa
-00000150: 636b 6167 6520 7461 736b 732e 0ae9 0000  ckage tasks.....
-00000160: 0000 2901 da04 5061 7468 2901 da04 4469  ..)...Path)...Di
-00000170: 6374 2903 da05 496e 626f 78da 064f 7574  ct)...Inbox..Out
-00000180: 626f 78da 0454 6173 6b29 01da 0a44 6963  box..Task)...Dic
-00000190: 744d 6572 6765 7229 01da 0b54 6173 6b4d  tMerger)...TaskM
-000001a0: 616e 6167 6572 2901 da08 7265 6769 7374  anager)...regist
-000001b0: 6572 2902 da08 7665 6e76 5f62 696e da08  er)...venv_bin..
-000001c0: 7665 6e76 5f64 6972 6300 0000 0000 0000  venv_dirc.......
-000001d0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-000001e0: 0073 2200 0000 6500 5a01 6400 5a02 6401  .s"...e.Z.d.Z.d.
-000001f0: 5a03 6504 6505 6506 6402 9c03 6403 6404  Z.e.e.e.d...d.d.
-00000200: 8404 5a07 6405 5300 2906 da08 4661 696c  ..Z.d.S.)...Fail
-00000210: 5461 736b 7a19 4120 7461 736b 2074 6861  Taskz.A task tha
-00000220: 7420 616c 7761 7973 2066 6169 6c73 2e29  t always fails.)
-00000230: 03da 0569 6e62 6f78 da06 6f75 7462 6f78  ...inbox..outbox
-00000240: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
-00000250: 0000 0000 0005 0000 0001 0000 00cf 0000  ................
-00000260: 0073 0400 0000 6401 5300 2902 4e46 a900  .s....d.S.).NF..
-00000270: 2905 da04 7365 6c66 720d 0000 0072 0e00  )...selfr....r..
-00000280: 0000 da04 6172 6773 da06 6b77 6172 6773  ....args..kwargs
-00000290: 7210 0000 0072 1000 0000 fa3d 2f68 6f6d  r....r.....=/hom
-000002a0: 652f 7275 6e6e 6572 2f77 6f72 6b2f 766d  e/runner/work/vm
-000002b0: 6b6c 6962 2f76 6d6b 6c69 622f 766d 6b6c  klib/vmklib/vmkl
-000002c0: 6962 2f64 6174 612f 6c69 625f 7461 736b  ib/data/lib_task
-000002d0: 732f 636f 6e66 2e70 79da 0372 756e 1f00  s/conf.py..run..
-000002e0: 0000 7302 0000 0000 017a 0c46 6169 6c54  ..s......z.FailT
-000002f0: 6173 6b2e 7275 6e4e 2908 da08 5f5f 6e61  ask.runN)...__na
-00000300: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000310: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-00000320: 5f5f 646f 635f 5f72 0400 0000 7205 0000  __doc__r....r...
-00000330: 00da 0462 6f6f 6c72 1500 0000 7210 0000  ...boolr....r...
-00000340: 0072 1000 0000 7210 0000 0072 1400 0000  .r....r....r....
-00000350: 720c 0000 001c 0000 0073 0400 0000 0801  r........s......
-00000360: 0402 720c 0000 0029 05da 076d 616e 6167  ..r....)...manag
-00000370: 6572 da07 7072 6f6a 6563 74da 0363 7764  er..project..cwd
-00000380: da0d 7375 6273 7469 7475 7469 6f6e 7372  ..substitutionsr
-00000390: 0f00 0000 6304 0000 0000 0000 0000 0000  ....c...........
-000003a0: 0007 0000 000a 0000 0043 0000 0073 8a00  .........C...s..
-000003b0: 0000 7c02 a000 6401 a101 7401 7c02 8301  ..|...d...t.|...
-000003c0: 7402 7c02 8301 7c02 a000 7c01 a101 6402  t.|...|...|...d.
-000003d0: 9c04 6403 7402 7c02 6403 8302 6901 6404  ..d.t.|.d...i.d.
-000003e0: 9c02 7d04 7c00 a003 7404 6405 8301 a101  ..}.|...t.d.....
-000003f0: 0100 7c00 a003 7405 6406 7c04 7c03 8303  ..|...t.d.|.|...
-00000400: a101 0100 6407 7d05 7406 7407 7408 7409  ....d.}.t.t.t.t.
-00000410: 740a 740b 740c 740d 740e 740f 660a 4400  t.t.t.t.t.t.f.D.
-00000420: 5d16 7d06 7c05 726e 7c06 7c00 7c01 7c02  ].}.|.rn|.|.|.|.
-00000430: 7c03 8304 7d05 716e 7c05 5300 2908 7a26  |...}.qn|.S.).z&
-00000440: 5265 6769 7374 6572 2070 6163 6b61 6765  Register package
-00000450: 2074 6173 6b73 2074 6f20 7468 6520 6d61   tasks to the ma
-00000460: 6e61 6765 722e da05 6275 696c 6429 0472  nager...build).r
-00000470: 1f00 0000 da04 7665 6e76 720a 0000 00da  ......venvr.....
-00000480: 0470 726f 6ada 0670 7974 686f 6e29 025a  .proj..python).Z
-00000490: 085f 5f64 6972 735f 5f5a 095f 5f66 696c  .__dirs__Z.__fil
-000004a0: 6573 5f5f 5a04 6661 696c 7a0b 766d 6b6c  es__Z.failz.vmkl
-000004b0: 6962 2e69 6e69 7454 2910 da08 6a6f 696e  ib.initT)...join
-000004c0: 7061 7468 720b 0000 0072 0a00 0000 7209  pathr....r....r.
-000004d0: 0000 0072 0c00 0000 7207 0000 00da 0d72  ...r....r......r
-000004e0: 6567 6973 7465 725f 7665 6e76 da14 7265  egister_venv..re
-000004f0: 6769 7374 6572 5f70 7974 686f 6e5f 6c69  gister_python_li
-00000500: 6e74 da17 7265 6769 7374 6572 5f70 7974  nt..register_pyt
-00000510: 686f 6e5f 7061 636b 6167 65da 1472 6567  hon_package..reg
-00000520: 6973 7465 725f 7079 7468 6f6e 5f79 616d  ister_python_yam
-00000530: 6cda 1572 6567 6973 7465 725f 7079 7468  l..register_pyth
-00000540: 6f6e 5f62 7569 6c64 da12 7265 6769 7374  on_build..regist
-00000550: 6572 5f70 7974 686f 6e5f 7361 da14 7265  er_python_sa..re
-00000560: 6769 7374 6572 5f70 7974 686f 6e5f 7465  gister_python_te
-00000570: 7374 da10 7265 6769 7374 6572 5f64 6174  st..register_dat
-00000580: 617a 656e da14 7265 6769 7374 6572 5f70  azen..register_p
-00000590: 7974 686f 6e5f 646f 6373 da0d 7265 6769  ython_docs..regi
-000005a0: 7374 6572 5f6e 6f64 6529 0772 1b00 0000  ster_node).r....
-000005b0: 721c 0000 0072 1d00 0000 721e 0000 005a  r....r....r....Z
-000005c0: 0969 6e69 745f 6461 7461 da06 7265 7375  .init_data..resu
-000005d0: 6c74 da03 6465 7072 1000 0000 7210 0000  lt..depr....r...
-000005e0: 0072 1400 0000 7209 0000 0023 0000 0073  .r....r....#...s
-000005f0: 3000 0000 000c 0801 0601 0601 08fc 0406  0...............
-00000600: 0cf9 060b 0e03 1203 0402 0201 0201 0201  ................
-00000610: 0201 0201 0201 0201 0201 0201 02f6 080c  ................
-00000620: 0401 1002 7209 0000 004e 2928 7219 0000  ....r....N)(r...
-00000630: 00da 0770 6174 686c 6962 7202 0000 00da  ...pathlibr.....
-00000640: 0674 7970 696e 6772 0300 0000 da0d 7663  .typingr......vc
-00000650: 6f72 656c 6962 2e74 6173 6b72 0400 0000  orelib.taskr....
-00000660: 7205 0000 0072 0600 0000 5a19 7663 6f72  r....r....Z.vcor
-00000670: 656c 6962 2e74 6173 6b2e 6469 6374 2e6d  elib.task.dict.m
-00000680: 656c 6465 7272 0700 0000 da15 7663 6f72  elderr......vcor
-00000690: 656c 6962 2e74 6173 6b2e 6d61 6e61 6765  elib.task.manage
-000006a0: 7272 0800 0000 5a11 766d 6b6c 6962 2e74  rr....Z.vmklib.t
-000006b0: 6173 6b73 2e6e 6f64 6572 0900 0000 722d  asks.noder....r-
-000006c0: 0000 005a 1376 6d6b 6c69 622e 7461 736b  ...Z.vmklib.task
-000006d0: 732e 7079 7468 6f6e 720a 0000 0072 0b00  s.pythonr....r..
-000006e0: 0000 5a19 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
-000006f0: 2e70 7974 686f 6e2e 6275 696c 6472 2800  .python.buildr(.
-00000700: 0000 5a1b 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
-00000710: 2e70 7974 686f 6e2e 6461 7461 7a65 6e72  .python.datazenr
-00000720: 2b00 0000 5a18 766d 6b6c 6962 2e74 6173  +...Z.vmklib.tas
-00000730: 6b73 2e70 7974 686f 6e2e 646f 6373 722c  ks.python.docsr,
-00000740: 0000 005a 1876 6d6b 6c69 622e 7461 736b  ...Z.vmklib.task
-00000750: 732e 7079 7468 6f6e 2e6c 696e 7472 2500  s.python.lintr%.
-00000760: 0000 5a1b 766d 6b6c 6962 2e74 6173 6b73  ..Z.vmklib.tasks
-00000770: 2e70 7974 686f 6e2e 7061 636b 6167 6572  .python.packager
-00000780: 2600 0000 5a16 766d 6b6c 6962 2e74 6173  &...Z.vmklib.tas
-00000790: 6b73 2e70 7974 686f 6e2e 7361 7229 0000  ks.python.sar)..
-000007a0: 005a 1876 6d6b 6c69 622e 7461 736b 732e  .Z.vmklib.tasks.
-000007b0: 7079 7468 6f6e 2e74 6573 7472 2a00 0000  python.testr*...
-000007c0: 5a18 766d 6b6c 6962 2e74 6173 6b73 2e70  Z.vmklib.tasks.p
-000007d0: 7974 686f 6e2e 7961 6d6c 7227 0000 005a  ython.yamlr'...Z
-000007e0: 1176 6d6b 6c69 622e 7461 736b 732e 7665  .vmklib.tasks.ve
-000007f0: 6e76 7224 0000 0072 0c00 0000 da03 7374  nvr$...r......st
-00000800: 7272 1a00 0000 7210 0000 0072 1000 0000  rr....r....r....
-00000810: 7210 0000 0072 1400 0000 da08 3c6d 6f64  r....r......<mod
-00000820: 756c 653e 0100 0000 732e 0000 0004 050c  ule>....s.......
-00000830: 010c 0314 010c 010c 030c 0110 010c 010c  ................
-00000840: 010c 010c 010c 010c 010c 010c 010c 0310  ................
-00000850: 0802 0102 0102 010a 0102 fb              ...........
+00000000: a70d 0d0a 0000 0000 6b1f af64 4609 0000  ........k..dF...
+00000010: e300 0000 0000 0000 0000 0000 000a 0000  ................
+00000020: 0000 0000 00f3 1e01 0000 9700 6400 5a00  ............d.Z.
+00000030: 6401 6402 6c01 6d02 5a02 0100 6401 6403  d.d.l.m.Z...d.d.
+00000040: 6c03 6d04 5a04 0100 6401 6404 6c05 6d06  l.m.Z...d.d.l.m.
+00000050: 5a06 6d07 5a07 6d08 5a08 0100 6401 6405  Z.m.Z.m.Z...d.d.
+00000060: 6c09 6d0a 5a0a 0100 6401 6406 6c0b 6d0c  l.m.Z...d.d.l.m.
+00000070: 5a0c 0100 6401 6407 6c0d 6d0e 5a0f 0100  Z...d.d.l.m.Z...
+00000080: 6401 6408 6c10 6d11 5a11 6d12 5a12 0100  d.d.l.m.Z.m.Z...
+00000090: 6401 6407 6c13 6d0e 5a14 0100 6401 6407  d.d.l.m.Z...d.d.
+000000a0: 6c15 6d0e 5a16 0100 6401 6407 6c17 6d0e  l.m.Z...d.d.l.m.
+000000b0: 5a18 0100 6401 6407 6c19 6d0e 5a1a 0100  Z...d.d.l.m.Z...
+000000c0: 6401 6407 6c1b 6d0e 5a1c 0100 6401 6407  d.d.l.m.Z...d.d.
+000000d0: 6c1d 6d0e 5a1e 0100 6401 6407 6c1f 6d0e  l.m.Z...d.d.l.m.
+000000e0: 5a20 0100 6401 6407 6c21 6d0e 5a22 0100  Z ..d.d.l!m.Z"..
+000000f0: 6401 6407 6c23 6d0e 5a24 0100 0200 4700  d.d.l#m.Z$....G.
+00000100: 6409 8400 640a 6508 a603 0000 ab03 0000  d...d.e.........
+00000110: 0000 0000 0000 5a25 640b 650c 640c 6526  ......Z%d.e.d.e&
+00000120: 640d 6502 640e 6504 6526 6526 6602 1900  d.e.d.e.e&e&f...
+00000130: 0000 0000 0000 0000 640f 6527 660a 6410  ........d.e'f.d.
+00000140: 8404 5a0e 6411 5300 2912 7a29 0a41 206d  ..Z.d.S.).z).A m
+00000150: 6f64 756c 6520 666f 7220 7265 6769 7374  odule for regist
+00000160: 6572 696e 6720 7061 636b 6167 6520 7461  ering package ta
+00000170: 736b 732e 0ae9 0000 0000 2901 da04 5061  sks.......)...Pa
+00000180: 7468 2901 da04 4469 6374 2903 da05 496e  th)...Dict)...In
+00000190: 626f 78da 064f 7574 626f 78da 0454 6173  box..Outbox..Tas
+000001a0: 6b29 01da 0a44 6963 744d 6572 6765 7229  k)...DictMerger)
+000001b0: 01da 0b54 6173 6b4d 616e 6167 6572 2901  ...TaskManager).
+000001c0: da08 7265 6769 7374 6572 2902 da08 7665  ..register)...ve
+000001d0: 6e76 5f62 696e da08 7665 6e76 5f64 6972  nv_bin..venv_dir
+000001e0: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
+000001f0: 0000 0000 00f3 2600 0000 9700 6500 5a01  ......&.....e.Z.
+00000200: 6400 5a02 6401 5a03 6402 6504 6403 6505  d.Z.d.Z.d.e.d.e.
+00000210: 6404 6506 6606 6405 8404 5a07 6406 5300  d.e.f.d...Z.d.S.
+00000220: 2907 da08 4661 696c 5461 736b 7a19 4120  )...FailTaskz.A 
+00000230: 7461 736b 2074 6861 7420 616c 7761 7973  task that always
+00000240: 2066 6169 6c73 2eda 0569 6e62 6f78 da06   fails...inbox..
+00000250: 6f75 7462 6f78 da06 7265 7475 726e 6303  outbox..returnc.
+00000260: 0000 0000 0000 0000 0000 0001 0000 008f  ................
+00000270: 0000 00f3 0a00 0000 4b00 0100 9700 6401  ........K.....d.
+00000280: 5300 2902 4e46 a900 2905 da04 7365 6c66  S.).NF..)...self
+00000290: 720f 0000 0072 1000 0000 da04 6172 6773  r....r......args
+000002a0: da06 6b77 6172 6773 7305 0000 0020 2020  ..kwargss....   
+000002b0: 2020 fa3d 2f68 6f6d 652f 7275 6e6e 6572    .=/home/runner
+000002c0: 2f77 6f72 6b2f 766d 6b6c 6962 2f76 6d6b  /work/vmklib/vmk
+000002d0: 6c69 622f 766d 6b6c 6962 2f64 6174 612f  lib/vmklib/data/
+000002e0: 6c69 625f 7461 736b 732f 636f 6e66 2e70  lib_tasks/conf.p
+000002f0: 79da 0372 756e 7a0c 4661 696c 5461 736b  y..runz.FailTask
+00000300: 2e72 756e 1f00 0000 730b 0000 00e8 00e8  .run....s.......
+00000310: 0080 00d8 0f14 8875 f300 0000 004e 2908  .......u.....N).
+00000320: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000330: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000340: 6d65 5f5f da07 5f5f 646f 635f 5f72 0500  me__..__doc__r..
+00000350: 0000 7206 0000 00da 0462 6f6f 6c72 1800  ..r......boolr..
+00000360: 0000 7213 0000 0072 1900 0000 7217 0000  ..r....r....r...
+00000370: 0072 0e00 0000 720e 0000 001c 0000 0073  .r....r........s
+00000380: 4300 0000 8000 8000 8000 8000 8000 d804  C...............
+00000390: 23d0 0423 f004 0105 1598 75f0 0001 0515  #..#......u.....
+000003a0: a866 f000 0105 15c8 24f0 0001 0515 f000  .f......$.......
+000003b0: 0105 15f0 0001 0515 f000 0105 15f0 0001  ................
+000003c0: 0515 f000 0105 1572 1900 0000 720e 0000  .......r....r...
+000003d0: 00da 076d 616e 6167 6572 da07 7072 6f6a  ...manager..proj
+000003e0: 6563 74da 0363 7764 da0d 7375 6273 7469  ect..cwd..substi
+000003f0: 7475 7469 6f6e 7372 1100 0000 6304 0000  tutionsr....c...
+00000400: 0000 0000 0000 0000 000a 0000 0003 0000  ................
+00000410: 00f3 ec01 0000 9700 7c02 a000 0000 0000  ........|.......
+00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000430: 6401 a601 0000 ab01 0000 0000 0000 0000  d...............
+00000440: 7403 0000 0000 0000 0000 0000 7c02 a601  t...........|...
+00000450: 0000 ab01 0000 0000 0000 0000 7405 0000  ............t...
+00000460: 0000 0000 0000 0000 7c02 a601 0000 ab01  ........|.......
+00000470: 0000 0000 0000 0000 7c02 a000 0000 0000  ........|.......
+00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000490: 7c01 a601 0000 ab01 0000 0000 0000 0000  |...............
+000004a0: 6402 9c04 6403 7405 0000 0000 0000 0000  d...d.t.........
+000004b0: 0000 7c02 6403 a602 0000 ab02 0000 0000  ..|.d...........
+000004c0: 0000 0000 6901 6404 9c02 7d04 7c00 a003  ....i.d...}.|...
+000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000004e0: 0000 0000 7409 0000 0000 0000 0000 0000  ....t...........
+000004f0: 6405 a601 0000 ab01 0000 0000 0000 0000  d...............
+00000500: a601 0000 ab01 0000 0000 0000 0000 0100  ................
+00000510: 7c00 a003 0000 0000 0000 0000 0000 0000  |...............
+00000520: 0000 0000 0000 0000 740b 0000 0000 0000  ........t.......
+00000530: 0000 0000 6406 7c04 7c03 a603 0000 ab03  ....d.|.|.......
+00000540: 0000 0000 0000 0000 a601 0000 ab01 0000  ................
+00000550: 0000 0000 0000 0100 6407 7d05 740c 0000  ........d.}.t...
+00000560: 0000 0000 0000 0000 740e 0000 0000 0000  ........t.......
+00000570: 0000 0000 7410 0000 0000 0000 0000 0000  ....t...........
+00000580: 7412 0000 0000 0000 0000 0000 7414 0000  t...........t...
+00000590: 0000 0000 0000 0000 7416 0000 0000 0000  ........t.......
+000005a0: 0000 0000 7418 0000 0000 0000 0000 0000  ....t...........
+000005b0: 741a 0000 0000 0000 0000 0000 741c 0000  t...........t...
+000005c0: 0000 0000 0000 0000 741e 0000 0000 0000  ........t.......
+000005d0: 0000 0000 660a 4400 5d12 7d06 7c05 720e  ....f.D.].}.|.r.
+000005e0: 0200 7c06 7c00 7c01 7c02 7c03 a604 0000  ..|.|.|.|.|.....
+000005f0: ab04 0000 0000 0000 0000 7d05 8c13 7c05  ..........}...|.
+00000600: 5300 2908 7a26 5265 6769 7374 6572 2070  S.).z&Register p
+00000610: 6163 6b61 6765 2074 6173 6b73 2074 6f20  ackage tasks to 
+00000620: 7468 6520 6d61 6e61 6765 722e da05 6275  the manager...bu
+00000630: 696c 6429 0472 2400 0000 da04 7665 6e76  ild).r$.....venv
+00000640: 720b 0000 00da 0470 726f 6ada 0670 7974  r......proj..pyt
+00000650: 686f 6e29 02da 085f 5f64 6972 735f 5fda  hon)...__dirs__.
+00000660: 095f 5f66 696c 6573 5f5f da04 6661 696c  .__files__..fail
+00000670: 7a0b 766d 6b6c 6962 2e69 6e69 7454 2910  z.vmklib.initT).
+00000680: da08 6a6f 696e 7061 7468 720c 0000 0072  ..joinpathr....r
+00000690: 0b00 0000 720a 0000 0072 0e00 0000 7208  ....r....r....r.
+000006a0: 0000 00da 0d72 6567 6973 7465 725f 7665  .....register_ve
+000006b0: 6e76 da14 7265 6769 7374 6572 5f70 7974  nv..register_pyt
+000006c0: 686f 6e5f 6c69 6e74 da17 7265 6769 7374  hon_lint..regist
+000006d0: 6572 5f70 7974 686f 6e5f 7061 636b 6167  er_python_packag
+000006e0: 65da 1472 6567 6973 7465 725f 7079 7468  e..register_pyth
+000006f0: 6f6e 5f79 616d 6cda 1572 6567 6973 7465  on_yaml..registe
+00000700: 725f 7079 7468 6f6e 5f62 7569 6c64 da12  r_python_build..
+00000710: 7265 6769 7374 6572 5f70 7974 686f 6e5f  register_python_
+00000720: 7361 da14 7265 6769 7374 6572 5f70 7974  sa..register_pyt
+00000730: 686f 6e5f 7465 7374 da10 7265 6769 7374  hon_test..regist
+00000740: 6572 5f64 6174 617a 656e da14 7265 6769  er_datazen..regi
+00000750: 7374 6572 5f70 7974 686f 6e5f 646f 6373  ster_python_docs
+00000760: da0d 7265 6769 7374 6572 5f6e 6f64 6529  ..register_node)
+00000770: 0772 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00000780: 7222 0000 00da 0969 6e69 745f 6461 7461  r".....init_data
+00000790: da06 7265 7375 6c74 da03 6465 7073 0700  ..result..deps..
+000007a0: 0000 2020 2020 2020 2072 1700 0000 720a  ..       r....r.
+000007b0: 0000 0072 0a00 0000 2300 0000 73f9 0000  ...r....#...s...
+000007c0: 0080 00f0 1800 1619 975c 925c a027 d115  .........\.\.'..
+000007d0: 2ad4 152a dd14 1c98 5391 4d94 4ddd 1820  *..*....S.M.M.. 
+000007e0: a013 990d 9c0d d814 1797 4c92 4ca0 17d1  ..........L.L...
+000007f0: 1429 d414 29f0 0905 150a f000 0515 0af0  .)..)...........
+00000800: 0c00 171f a508 a813 a868 d120 37d4 2037  .........h. 7. 7
+00000810: d015 38f0 0f08 1106 f000 0811 0680 49f0  ..8...........I.
+00000820: 1600 050c d704 14d2 0414 9558 9866 d115  ...........X.f..
+00000830: 25d4 1525 d104 26d4 0426 d004 26f0 0600  %..%..&..&..&...
+00000840: 050c d704 14d2 0414 955a a00d a879 b82d  .........Z...y.-
+00000850: d115 48d4 1548 d104 49d4 0449 d004 49f0  ..H..H..I..I..I.
+00000860: 0600 0e12 8046 e508 15dd 081c dd08 1fdd  .....F..........
+00000870: 081c dd08 1ddd 081a dd08 1cdd 0818 dd08  ................
+00000880: 1cdd 0815 f015 0b10 06f0 000d 053f f000  .............?..
+00000890: 0d05 3f88 03f0 1800 0c12 f000 0109 3fd8  ..?...........?.
+000008a0: 1518 9053 9817 a027 a833 b00d d115 3ed4  ...S...'.3....>.
+000008b0: 153e 8846 f8e0 0b11 804d 7219 0000 004e  .>.F.....Mr....N
+000008c0: 2928 721d 0000 00da 0770 6174 686c 6962  )(r......pathlib
+000008d0: 7203 0000 00da 0674 7970 696e 6772 0400  r......typingr..
+000008e0: 0000 da0d 7663 6f72 656c 6962 2e74 6173  ....vcorelib.tas
+000008f0: 6b72 0500 0000 7206 0000 0072 0700 0000  kr....r....r....
+00000900: da19 7663 6f72 656c 6962 2e74 6173 6b2e  ..vcorelib.task.
+00000910: 6469 6374 2e6d 656c 6465 7272 0800 0000  dict.melderr....
+00000920: da15 7663 6f72 656c 6962 2e74 6173 6b2e  ..vcorelib.task.
+00000930: 6d61 6e61 6765 7272 0900 0000 da11 766d  managerr......vm
+00000940: 6b6c 6962 2e74 6173 6b73 2e6e 6f64 6572  klib.tasks.noder
+00000950: 0a00 0000 7235 0000 00da 1376 6d6b 6c69  ....r5.....vmkli
+00000960: 622e 7461 736b 732e 7079 7468 6f6e 720b  b.tasks.pythonr.
+00000970: 0000 0072 0c00 0000 da19 766d 6b6c 6962  ...r......vmklib
+00000980: 2e74 6173 6b73 2e70 7974 686f 6e2e 6275  .tasks.python.bu
+00000990: 696c 6472 3000 0000 da1b 766d 6b6c 6962  ildr0.....vmklib
+000009a0: 2e74 6173 6b73 2e70 7974 686f 6e2e 6461  .tasks.python.da
+000009b0: 7461 7a65 6e72 3300 0000 da18 766d 6b6c  tazenr3.....vmkl
+000009c0: 6962 2e74 6173 6b73 2e70 7974 686f 6e2e  ib.tasks.python.
+000009d0: 646f 6373 7234 0000 00da 1876 6d6b 6c69  docsr4.....vmkli
+000009e0: 622e 7461 736b 732e 7079 7468 6f6e 2e6c  b.tasks.python.l
+000009f0: 696e 7472 2d00 0000 da1b 766d 6b6c 6962  intr-.....vmklib
+00000a00: 2e74 6173 6b73 2e70 7974 686f 6e2e 7061  .tasks.python.pa
+00000a10: 636b 6167 6572 2e00 0000 da16 766d 6b6c  ckager......vmkl
+00000a20: 6962 2e74 6173 6b73 2e70 7974 686f 6e2e  ib.tasks.python.
+00000a30: 7361 7231 0000 00da 1876 6d6b 6c69 622e  sar1.....vmklib.
+00000a40: 7461 736b 732e 7079 7468 6f6e 2e74 6573  tasks.python.tes
+00000a50: 7472 3200 0000 da18 766d 6b6c 6962 2e74  tr2.....vmklib.t
+00000a60: 6173 6b73 2e70 7974 686f 6e2e 7961 6d6c  asks.python.yaml
+00000a70: 722f 0000 00da 1176 6d6b 6c69 622e 7461  r/.....vmklib.ta
+00000a80: 736b 732e 7665 6e76 722c 0000 0072 0e00  sks.venvr,...r..
+00000a90: 0000 da03 7374 7272 1e00 0000 7213 0000  ....strr....r...
+00000aa0: 0072 1900 0000 7217 0000 00fa 083c 6d6f  .r....r......<mo
+00000ab0: 6475 6c65 3e72 4a00 0000 0100 0000 73c5  dule>rJ.......s.
+00000ac0: 0100 00f0 0301 0101 f002 0201 04f0 0002  ................
+00000ad0: 0104 f00a 0001 19d0 0018 d000 18d0 0018  ................
+00000ae0: d000 18d0 0018 d800 17d0 0017 d000 17d0  ................
+00000af0: 0017 d000 17d0 0017 f006 0001 2ed0 002d  ...............-
+00000b00: d000 2dd0 002d d000 2dd0 002d d000 2dd0  ..-..-..-..-..-.
+00000b10: 002d d000 2dd0 002d d800 30d0 0030 d000  .-..-..-..0..0..
+00000b20: 30d0 0030 d000 30d0 0030 d800 2dd0 002d  0..0..0..0..-..-
+00000b30: d000 2dd0 002d d000 2dd0 002d f006 0001  ..-..-..-..-....
+00000b40: 38d0 0037 d000 37d0 0037 d000 37d0 0037  8..7..7..7..7..7
+00000b50: d800 32d0 0032 d000 32d0 0032 d000 32d0  ..2..2..2..2..2.
+00000b60: 0032 d000 32d0 0032 d800 47d0 0047 d000  .2..2..2..G..G..
+00000b70: 47d0 0047 d000 47d0 0047 d800 44d0 0044  G..G..G..G..D..D
+00000b80: d000 44d0 0044 d000 44d0 0044 d800 45d0  ..D..D..D..D..E.
+00000b90: 0045 d000 45d0 0045 d000 45d0 0045 d800  .E..E..E..E..E..
+00000ba0: 45d0 0045 d000 45d0 0045 d000 45d0 0045  E..E..E..E..E..E
+00000bb0: d800 4bd0 004b d000 4bd0 004b d000 4bd0  ..K..K..K..K..K.
+00000bc0: 004b d800 41d0 0041 d000 41d0 0041 d000  .K..A..A..A..A..
+00000bd0: 41d0 0041 d800 45d0 0045 d000 45d0 0045  A..A..E..E..E..E
+00000be0: d000 45d0 0045 d800 45d0 0045 d000 45d0  ..E..E..E..E..E.
+00000bf0: 0045 d000 45d0 0045 d800 37d0 0037 d000  .E..E..E..7..7..
+00000c00: 37d0 0037 d000 37d0 0037 f006 0401 15f0  7..7..7..7......
+00000c10: 0004 0115 f000 0401 15f0 0004 0115 f000  ................
+00000c20: 0401 1588 74f1 0004 0115 f400 0401 15f0  ....t...........
+00000c30: 0004 0115 f00e 2b01 12d8 0d18 f003 2b01  ......+.......+.
+00000c40: 12e0 0d10 f005 2b01 12f0 0600 0a0e f007  ......+.........
+00000c50: 2b01 12f0 0800 1418 9803 9853 9808 943e  +..........S...>
+00000c60: f009 2b01 12f0 0a00 060a f00b 2b01 12f0  ..+.........+...
+00000c70: 002b 0112 f000 2b01 12f0 002b 0112 f000  .+....+....+....
+00000c80: 2b01 12f0 002b 0112 7219 0000 00         +....+..r....
```

### Comparing `vmklib-1.8.3/vmklib/data/lib_tasks/conf.py` & `vmklib-1.9.0/vmklib/data/lib_tasks/conf.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/python/build.mk` & `vmklib-1.9.0/vmklib/data/python/build.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/python/docs.mk` & `vmklib-1.9.0/vmklib/data/python/docs.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/python/pypi.mk` & `vmklib-1.9.0/vmklib/data/python/pypi.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/python/upload.mk` & `vmklib-1.9.0/vmklib/data/python/upload.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/python.mk` & `vmklib-1.9.0/vmklib/data/python.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/time.mk` & `vmklib-1.9.0/vmklib/data/time.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/venv.mk` & `vmklib-1.9.0/vmklib/data/venv.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/data/vmklib.mk` & `vmklib-1.9.0/vmklib/data/vmklib.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/entry.py` & `vmklib-1.9.0/vmklib/entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/resources.py` & `vmklib-1.9.0/vmklib/resources.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/args.py` & `vmklib-1.9.0/vmklib/tasks/args.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/mixins/concrete.py` & `vmklib-1.9.0/vmklib/tasks/mixins/concrete.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/node/__init__.py` & `vmklib-1.9.0/vmklib/tasks/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/__init__.py` & `vmklib-1.9.0/vmklib/tasks/python/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/build.py` & `vmklib-1.9.0/vmklib/tasks/python/build.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/datazen.py` & `vmklib-1.9.0/vmklib/tasks/python/datazen.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/docs.py` & `vmklib-1.9.0/vmklib/tasks/python/docs.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/lint.py` & `vmklib-1.9.0/vmklib/tasks/python/lint.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/package.py` & `vmklib-1.9.0/vmklib/tasks/python/package.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/sa.py` & `vmklib-1.9.0/vmklib/tasks/python/sa.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/test.py` & `vmklib-1.9.0/vmklib/tasks/python/test.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/python/yaml.py` & `vmklib-1.9.0/vmklib/tasks/python/yaml.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib/tasks/venv.py` & `vmklib-1.9.0/vmklib/tasks/venv.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.3/vmklib.egg-info/PKG-INFO` & `vmklib-1.9.0/vmklib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.3
+Version: 1.9.0
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -26,39 +26,38 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Keywords: workflow,tool,make
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=84b7fe19dafb7682480119b63d53aa24
+    hash=1280d00c2447ef272e48abbae9617e0a
     =====================================
 -->
 
-# vmklib ([1.8.3](https://pypi.org/project/vmklib/))
+# vmklib ([1.9.0](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -67,15 +66,14 @@
 See also: [generated documentation](https://vkottler.github.io/python/pydoc/vmklib.html)
 (created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `vmklib-1.8.3/vmklib.egg-info/SOURCES.txt` & `vmklib-1.9.0/vmklib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 vmklib/data/vmklib.mk
 vmklib/data/yaml.mk
 vmklib/data/data/edit_venv.txt
 vmklib/data/data/fresh_venv.txt
 vmklib/data/data/header.mk
 vmklib/data/lib_tasks/__init__.py
 vmklib/data/lib_tasks/conf.py
-vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
+vmklib/data/lib_tasks/__pycache__/conf.cpython-311.pyc
 vmklib/data/python/build.mk
 vmklib/data/python/docs.mk
 vmklib/data/python/pypi.mk
 vmklib/data/python/upload.mk
 vmklib/tasks/__init__.py
 vmklib/tasks/args.py
+vmklib/tasks/clean.py
+vmklib/tasks/github.py
 vmklib/tasks/venv.py
 vmklib/tasks/mixins/__init__.py
 vmklib/tasks/mixins/concrete.py
+vmklib/tasks/mixins/curl.py
 vmklib/tasks/node/__init__.py
 vmklib/tasks/python/__init__.py
 vmklib/tasks/python/build.py
 vmklib/tasks/python/datazen.py
 vmklib/tasks/python/docs.py
 vmklib/tasks/python/lint.py
 vmklib/tasks/python/package.py
```

