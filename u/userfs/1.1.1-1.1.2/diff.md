# Comparing `tmp/userfs-1.1.1.tar.gz` & `tmp/userfs-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-1.1.1.tar", last modified: Wed May 31 05:50:26 2023, max compression
+gzip compressed data, was "userfs-1.1.2.tar", last modified: Sun Aug  6 07:17:50 2023, max compression
```

## Comparing `userfs-1.1.1.tar` & `userfs-1.1.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 05:49:01.000000 userfs-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-31 05:50:26.263870 userfs-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-31 05:49:01.000000 userfs-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 05:49:01.000000 userfs-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:50:26.263870 userfs-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-31 05:49:01.000000 userfs-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.255869 userfs-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 05:49:01.000000 userfs-1.1.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 05:49:01.000000 userfs-1.1.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.255869 userfs-1.1.1/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.263870 userfs-1.1.1/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-31 05:49:01.000000 userfs-1.1.1/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:50:26.259869 userfs-1.1.1/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 05:50:26.000000 userfs-1.1.1/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.419095 userfs-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:16:30.000000 userfs-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-08-06 07:17:50.419095 userfs-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-08-06 07:16:30.000000 userfs-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-06 07:16:30.000000 userfs-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:17:50.419095 userfs-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-06 07:16:30.000000 userfs-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-06 07:16:30.000000 userfs-1.1.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-06 07:16:30.000000 userfs-1.1.2/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.419095 userfs-1.1.2/userfs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.419095 userfs-1.1.2/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.419095 userfs-1.1.2/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-06 07:16:30.000000 userfs-1.1.2/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:17:50.415095 userfs-1.1.2/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 07:17:50.000000 userfs-1.1.2/userfs.egg-info/top_level.txt
```

### Comparing `userfs-1.1.1/LICENSE` & `userfs-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/PKG-INFO` & `userfs-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.1
+Version: 1.1.2
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
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
-    hash=c140d059bd4f3630373f891ee3b3cc15
+    hash=937da2931f9c0387ead4e59c8f242a53
     =====================================
 -->
 
-# userfs ([1.1.1](https://pypi.org/project/userfs/))
+# userfs ([1.1.2](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
 *A system-bootstrapping automation and introspection tool.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/userfs.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/userfs)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/userfs.html)
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

### Comparing `userfs-1.1.1/README.md` & `userfs-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c140d059bd4f3630373f891ee3b3cc15
+    hash=937da2931f9c0387ead4e59c8f242a53
     =====================================
 -->
 
-# userfs ([1.1.1](https://pypi.org/project/userfs/))
+# userfs ([1.1.2](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
 *A system-bootstrapping automation and introspection tool.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/userfs.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/userfs)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/userfs.html)
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

### Comparing `userfs-1.1.1/pyproject.toml` & `userfs-1.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "1.1.1"
+version = "1.1.2"
 description = "A system-bootstrapping automation and introspection tool."
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
 ufs = "userfs.entry:main"
```

### Comparing `userfs-1.1.1/setup.py` & `userfs-1.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=adbd3386d75866f59abf0027f730de43
+# hash=eb962b24d32e1e0e14d30b920fd304e3
 # =====================================
 
 """
 userfs - Package definition for distribution.
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

### Comparing `userfs-1.1.1/tests/test_entry.py` & `userfs-1.1.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/app.py` & `userfs-1.1.2/userfs/app.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/build/__init__.py` & `userfs-1.1.2/userfs/build/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/commands/all.py` & `userfs-1.1.2/userfs/commands/all.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/commands/build.py` & `userfs-1.1.2/userfs/commands/build.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/commands/common.py` & `userfs-1.1.2/userfs/commands/common.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/commands/custom.py` & `userfs-1.1.2/userfs/commands/custom.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/commands/fetch.py` & `userfs-1.1.2/userfs/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/config/__init__.py` & `userfs-1.1.2/userfs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/config/project.py` & `userfs-1.1.2/userfs/config/project.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/config/source.py` & `userfs-1.1.2/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/data/schemas/Config.yaml` & `userfs-1.1.2/userfs/data/schemas/Config.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-1.1.2/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/entry.py` & `userfs-1.1.2/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/fetch/__init__.py` & `userfs-1.1.2/userfs/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/hooks/__init__.py` & `userfs-1.1.2/userfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/paths.py` & `userfs-1.1.2/userfs/paths.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/project/__init__.py` & `userfs-1.1.2/userfs/project/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/schemas.py` & `userfs-1.1.2/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs/update/__init__.py` & `userfs-1.1.2/userfs/update/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-1.1.1/userfs.egg-info/PKG-INFO` & `userfs-1.1.2/userfs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 1.1.1
+Version: 1.1.2
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
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
-    hash=c140d059bd4f3630373f891ee3b3cc15
+    hash=937da2931f9c0387ead4e59c8f242a53
     =====================================
 -->
 
-# userfs ([1.1.1](https://pypi.org/project/userfs/))
+# userfs ([1.1.2](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
 *A system-bootstrapping automation and introspection tool.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/userfs.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/userfs)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/userfs.html)
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

### Comparing `userfs-1.1.1/userfs.egg-info/SOURCES.txt` & `userfs-1.1.2/userfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

