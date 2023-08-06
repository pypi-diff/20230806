# Comparing `tmp/rcmpy-1.5.2.tar.gz` & `tmp/rcmpy-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.5.2.tar", last modified: Fri Jun 23 07:27:19 2023, max compression
+gzip compressed data, was "rcmpy-1.5.3.tar", last modified: Sun Aug  6 07:13:33 2023, max compression
```

## Comparing `rcmpy-1.5.2.tar` & `rcmpy-1.5.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 07:26:11.000000 rcmpy-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-23 07:27:19.369839 rcmpy-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-23 07:26:11.000000 rcmpy-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-23 07:26:11.000000 rcmpy-1.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.361839 rcmpy-1.5.2/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/watch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/watch/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-23 07:26:11.000000 rcmpy-1.5.2/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.365839 rcmpy-1.5.2/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 07:27:19.000000 rcmpy-1.5.2/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 07:27:19.369839 rcmpy-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-23 07:26:11.000000 rcmpy-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:27:19.369839 rcmpy-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 07:26:11.000000 rcmpy-1.5.2/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:12:12.000000 rcmpy-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 07:13:33.480410 rcmpy-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-08-06 07:12:12.000000 rcmpy-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-06 07:12:12.000000 rcmpy-1.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/watch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/watch/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-06 07:12:12.000000 rcmpy-1.5.3/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.476410 rcmpy-1.5.3/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:13:33.000000 rcmpy-1.5.3/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:13:33.480410 rcmpy-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-06 07:12:12.000000 rcmpy-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:13:33.480410 rcmpy-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-06 07:12:12.000000 rcmpy-1.5.3/tests/test_xdg.py
```

### Comparing `rcmpy-1.5.2/LICENSE` & `rcmpy-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/PKG-INFO` & `rcmpy-1.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.2
+Version: 1.5.3
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
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
-    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
+    hash=1378c10a9410bc7e897df3efc11350c1
     =====================================
 -->
 
-# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
 *A configuration-file management system.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/rcmpy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/rcmpy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `rcmpy-1.5.2/README.md` & `rcmpy-1.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
+    hash=1378c10a9410bc7e897df3efc11350c1
     =====================================
 -->
 
-# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
 *A configuration-file management system.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/rcmpy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/rcmpy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `rcmpy-1.5.2/pyproject.toml` & `rcmpy-1.5.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.5.2"
+version = "1.5.3"
 description = "A configuration-file management system."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
@@ -34,13 +33,15 @@
   "pylint",
   "flake8",
   "black",
   "ruff",
   "mypy",
   "isort",
   "yamllint",
+  "yambs",
+  "vmklib",
   "setuptools-wrapper",
   "types-setuptools"
 ]
 
 [project.scripts]
 rcmpy = "rcmpy.entry:main"
```

### Comparing `rcmpy-1.5.2/rcmpy/app.py` & `rcmpy-1.5.3/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/all.py` & `rcmpy-1.5.3/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/apply.py` & `rcmpy-1.5.3/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/common.py` & `rcmpy-1.5.3/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/dump.py` & `rcmpy-1.5.3/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/use.py` & `rcmpy-1.5.3/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/variant.py` & `rcmpy-1.5.3/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/commands/watch.py` & `rcmpy-1.5.3/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/config/__init__.py` & `rcmpy-1.5.3/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/config/file.py` & `rcmpy-1.5.3/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.5.3/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/entry.py` & `rcmpy-1.5.3/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/environment/__init__.py` & `rcmpy-1.5.3/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/environment/base.py` & `rcmpy-1.5.3/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/environment/data.py` & `rcmpy-1.5.3/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/environment/template.py` & `rcmpy-1.5.3/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/paths/__init__.py` & `rcmpy-1.5.3/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/schemas.py` & `rcmpy-1.5.3/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/state/__init__.py` & `rcmpy-1.5.3/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/watch/__init__.py` & `rcmpy-1.5.3/rcmpy/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/watch/params.py` & `rcmpy-1.5.3/rcmpy/watch/params.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy/xdg/__init__.py` & `rcmpy-1.5.3/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.5.3/rcmpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.5.2
+Version: 1.5.3
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
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
-    hash=3c7a54d3f5dd7f524b8ad29c1dee448d
+    hash=1378c10a9410bc7e897df3efc11350c1
     =====================================
 -->
 
-# rcmpy ([1.5.2](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.5.3](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
 *A configuration-file management system.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/rcmpy.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/rcmpy)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/rcmpy.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
 * [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
```

### Comparing `rcmpy-1.5.2/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.5.3/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.5.2/setup.py` & `rcmpy-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=dc0d9f835ecbdaf7ba7d62dc617acb8d
+# hash=41029b1d344eff0720907ad9b29da09b
 # =====================================
 
 """
 rcmpy - Package definition for distribution.
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

### Comparing `rcmpy-1.5.2/tests/test_entry.py` & `rcmpy-1.5.3/tests/test_entry.py`

 * *Files identical despite different names*

