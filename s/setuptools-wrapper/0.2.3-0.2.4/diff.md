# Comparing `tmp/setuptools-wrapper-0.2.3.tar.gz` & `tmp/setuptools-wrapper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-wrapper-0.2.3.tar", last modified: Thu Nov 17 20:38:50 2022, max compression
+gzip compressed data, was "setuptools-wrapper-0.2.4.tar", last modified: Sun Aug  6 07:15:29 2023, max compression
```

## Comparing `setuptools-wrapper-0.2.3.tar` & `setuptools-wrapper-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/setuptools_wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/setuptools_wrapper/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6712 2022-11-17 20:37:41.000000 setuptools-wrapper-0.2.3/setuptools_wrapper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:38:50.690816 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-11-17 20:38:50.000000 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-17 20:38:50.000000 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:38:50.000000 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-17 20:38:50.000000 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-17 20:38:50.000000 setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/setuptools_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/setuptools_wrapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/setuptools_wrapper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-08-06 07:15:29.000000 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-06 07:15:29.000000 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:15:29.000000 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 07:15:29.000000 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-06 07:15:29.000000 setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:15:29.703204 setuptools-wrapper-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-06 07:14:14.000000 setuptools-wrapper-0.2.4/tests/test_setup.py
```

### Comparing `setuptools-wrapper-0.2.3/LICENSE` & `setuptools-wrapper-0.2.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vaughn Kottler
+Copyright (c) 2023 Vaughn Kottler
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `setuptools-wrapper-0.2.3/PKG-INFO` & `setuptools-wrapper-0.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 Metadata-Version: 2.1
 Name: setuptools-wrapper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple interface to setuptools's setup function.
 Home-page: https://github.com/vkottler/setuptools-wrapper
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
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
-    version=3.1.0
-    hash=f62e7926101137426b8edba2efe30343
+    version=3.1.2
+    hash=d33d73fa711b3715c68d36e6a6ded29c
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.3](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.4](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
 
 *A simple interface to setuptools's setup function.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/setuptools-wrapper)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
```

### Comparing `setuptools-wrapper-0.2.3/README.md` & `setuptools-wrapper-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 <!--
     =====================================
     generator=datazen
-    version=3.1.0
-    hash=f62e7926101137426b8edba2efe30343
+    version=3.1.2
+    hash=d33d73fa711b3715c68d36e6a6ded29c
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.3](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.4](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
 
 *A simple interface to setuptools's setup function.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/setuptools-wrapper)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
```

### Comparing `setuptools-wrapper-0.2.3/pyproject.toml` & `setuptools-wrapper-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [build-system]
 requires = ["setuptools", "wheel", "trove-classifiers"]
 
 [project]
 name = "setuptools-wrapper"
-version = "0.2.3"
+version = "0.2.4"
 description = "A simple interface to setuptools's setup function."
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
   "Topic :: Software Development :: Build Tools",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
   "pylint",
   "flake8",
-  "pytest",
-  "pytest-cov",
-  "mypy",
   "black",
+  "ruff",
+  "mypy",
   "isort",
+  "yamllint",
+  "yambs",
+  "vmklib",
   "types-setuptools",
   "vcorelib"
 ]
```

### Comparing `setuptools-wrapper-0.2.3/setuptools_wrapper/setup.py` & `setuptools-wrapper-0.2.4/setuptools_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-wrapper-0.2.3/setuptools_wrapper.egg-info/PKG-INFO` & `setuptools-wrapper-0.2.4/setuptools_wrapper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,66 @@
 Metadata-Version: 2.1
 Name: setuptools-wrapper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple interface to setuptools's setup function.
 Home-page: https://github.com/vkottler/setuptools-wrapper
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
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
-    version=3.1.0
-    hash=f62e7926101137426b8edba2efe30343
+    version=3.1.2
+    hash=d33d73fa711b3715c68d36e6a6ded29c
     =====================================
 -->
 
-# setuptools-wrapper ([0.2.3](https://pypi.org/project/setuptools-wrapper/))
+# setuptools-wrapper ([0.2.4](https://pypi.org/project/setuptools-wrapper/))
 
 [![python](https://img.shields.io/pypi/pyversions/setuptools-wrapper.svg)](https://pypi.org/project/setuptools-wrapper/)
 ![Build Status](https://github.com/vkottler/setuptools-wrapper/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/setuptools-wrapper/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/setuptools-wrapper)
 ![PyPI - Status](https://img.shields.io/pypi/status/setuptools-wrapper)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/setuptools-wrapper)
 
 *A simple interface to setuptools's setup function.*
 
-See also: [generated documentation](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
-(created with [`pydoc`](https://docs.python.org/3/library/pydoc.html)).
+## Documentation
+
+### Generated
+
+* By [sphinx-apidoc](https://vkottler.github.io/python/sphinx/setuptools-wrapper)
+(What's [`sphinx-apidoc`](https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html)?)
+* By [pydoc](https://vkottler.github.io/python/pydoc/setuptools_wrapper.html)
+(What's [`pydoc`](https://docs.python.org/3/library/pydoc.html)?)
 
 ## Python Version Support
 
 This package is tested with the following Python minor versions:
 
-* [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
```

