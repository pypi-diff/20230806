# Comparing `tmp/crazy-thursday-2023.8.6.0.tar.gz` & `tmp/crazy-thursday-2023.8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crazy-thursday-2023.8.6.0.tar", last modified: Sat Aug  5 17:27:08 2023, max compression
+gzip compressed data, was "crazy-thursday-2023.8.6.1.tar", last modified: Sun Aug  6 05:26:53 2023, max compression
```

## Comparing `crazy-thursday-2023.8.6.0.tar` & `crazy-thursday-2023.8.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:27:08.373620 crazy-thursday-2023.8.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-05 17:27:08.373620 crazy-thursday-2023.8.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:27:08.369620 crazy-thursday-2023.8.6.0/crazy_thursday/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-05 17:26:57.000000 crazy-thursday-2023.8.6.0/crazy_thursday/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/crazy_thursday/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-08-05 17:26:57.000000 crazy-thursday-2023.8.6.0/crazy_thursday/corpus.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/crazy_thursday/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:27:08.373620 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-05 17:27:08.000000 crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:27:08.373620 crazy-thursday-2023.8.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/scripts/get_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/scripts/update_curpus.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:27:08.373620 crazy-thursday-2023.8.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-05 17:26:51.000000 crazy-thursday-2023.8.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:26:53.548045 crazy-thursday-2023.8.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-06 05:26:53.548045 crazy-thursday-2023.8.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:26:53.544045 crazy-thursday-2023.8.6.1/crazy_thursday/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 05:26:45.000000 crazy-thursday-2023.8.6.1/crazy_thursday/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/crazy_thursday/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-08-06 05:26:45.000000 crazy-thursday-2023.8.6.1/crazy_thursday/corpus.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/crazy_thursday/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:26:53.544045 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 05:26:53.000000 crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 05:26:53.544045 crazy-thursday-2023.8.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/scripts/get_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/scripts/update_curpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 05:26:53.548045 crazy-thursday-2023.8.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-06 05:26:41.000000 crazy-thursday-2023.8.6.1/setup.py
```

### Comparing `crazy-thursday-2023.8.6.0/LICENSE` & `crazy-thursday-2023.8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/PKG-INFO` & `crazy-thursday-2023.8.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazy-thursday
-Version: 2023.8.6.0
+Version: 2023.8.6.1
 Summary: a cli tool to print crazy thursday article
 Home-page: https://github.com/zqmillet/sphinx-console
 Author: kinopico
 Author-email: zqmillet@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crazy-thursday-2023.8.6.0/README.md` & `crazy-thursday-2023.8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/crazy_thursday/__main__.py` & `crazy-thursday-2023.8.6.1/crazy_thursday/__main__.py`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/crazy_thursday/corpus.jsonl` & `crazy-thursday-2023.8.6.1/crazy_thursday/corpus.jsonl`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/crazy_thursday.egg-info/PKG-INFO` & `crazy-thursday-2023.8.6.1/crazy_thursday.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crazy-thursday
-Version: 2023.8.6.0
+Version: 2023.8.6.1
 Summary: a cli tool to print crazy thursday article
 Home-page: https://github.com/zqmillet/sphinx-console
 Author: kinopico
 Author-email: zqmillet@qq.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crazy-thursday-2023.8.6.0/scripts/get_issues.py` & `crazy-thursday-2023.8.6.1/scripts/get_issues.py`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/scripts/update_curpus.py` & `crazy-thursday-2023.8.6.1/scripts/update_curpus.py`

 * *Files identical despite different names*

### Comparing `crazy-thursday-2023.8.6.0/setup.py` & `crazy-thursday-2023.8.6.1/setup.py`

 * *Files identical despite different names*

