# Comparing `tmp/instld-0.0.8.tar.gz` & `tmp/instld-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instld-0.0.8.tar", last modified: Wed May  3 08:20:28 2023, max compression
+gzip compressed data, was "instld-0.0.9.tar", last modified: Wed May  3 09:50:06 2023, max compression
```

## Comparing `instld-0.0.8.tar` & `instld-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 08:20:28.288493 instld-0.0.8/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.8/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)     9917 2023-05-03 08:20:28.288234 instld-0.0.8/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)     9346 2023-05-03 08:19:37.000000 instld-0.0.8/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 08:20:28.285510 instld-0.0.8/installed/
--rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.8/installed/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1101 2023-05-02 05:39:10.000000 instld-0.0.8/installed/context.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1838 2023-05-02 09:21:50.000000 instld-0.0.8/installed/context_manager.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.8/installed/empty_logger.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.8/installed/errors.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       43 2023-05-01 17:48:12.000000 instld-0.0.8/installed/lock.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     4043 2023-05-02 09:00:29.000000 instld-0.0.8/installed/proxy_module.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1040 2023-05-02 09:23:26.000000 instld-0.0.8/installed/runner.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 08:20:28.286630 instld-0.0.8/instld.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)     9917 2023-05-03 08:20:28.000000 instld-0.0.8/instld.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      440 2023-05-03 08:20:28.000000 instld-0.0.8/instld.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-05-03 08:20:28.000000 instld-0.0.8/instld.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-05-03 08:20:28.000000 instld-0.0.8/instld.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-05-03 08:20:28.288554 instld-0.0.8/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      852 2023-05-03 08:19:03.000000 instld-0.0.8/setup.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 08:20:28.281186 instld-0.0.8/tests/
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 08:20:28.287779 instld-0.0.8/tests/units/
--rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.8/tests/units/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      217 2023-05-02 06:02:42.000000 instld-0.0.8/tests/units/test_context.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.8/tests/units/test_errors.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1459 2023-05-02 09:22:37.000000 instld-0.0.8/tests/units/test_proxy_module.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 09:50:06.098844 instld-0.0.9/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.9/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9950 2023-05-03 09:50:06.098496 instld-0.0.9/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9379 2023-05-03 09:46:09.000000 instld-0.0.9/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 09:50:06.095179 instld-0.0.9/installed/
+-rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.9/installed/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1101 2023-05-02 05:39:10.000000 instld-0.0.9/installed/context.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1838 2023-05-02 09:21:50.000000 instld-0.0.9/installed/context_manager.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.9/installed/empty_logger.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.9/installed/errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       43 2023-05-01 17:48:12.000000 instld-0.0.9/installed/lock.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     4043 2023-05-02 09:00:29.000000 instld-0.0.9/installed/proxy_module.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1040 2023-05-02 09:23:26.000000 instld-0.0.9/installed/runner.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 09:50:06.096236 instld-0.0.9/instld.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9950 2023-05-03 09:50:06.000000 instld-0.0.9/instld.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      440 2023-05-03 09:50:06.000000 instld-0.0.9/instld.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-05-03 09:50:06.000000 instld-0.0.9/instld.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-05-03 09:50:06.000000 instld-0.0.9/instld.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-05-03 09:50:06.098926 instld-0.0.9/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      852 2023-05-03 09:49:32.000000 instld-0.0.9/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 09:50:06.090455 instld-0.0.9/tests/
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-03 09:50:06.097420 instld-0.0.9/tests/units/
+-rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.9/tests/units/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      217 2023-05-02 06:02:42.000000 instld-0.0.9/tests/units/test_context.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.9/tests/units/test_errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1459 2023-05-02 09:22:37.000000 instld-0.0.9/tests/units/test_proxy_module.py
```

### Comparing `instld-0.0.8/LICENSE` & `instld-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `instld-0.0.8/PKG-INFO` & `instld-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.8
+Version: 0.0.9
 Summary: The simplest package management in runtime
 Home-page: https://github.com/pomponchik/instld
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![logo](/docs/assets/logo5.png)
+
 # INSTLD: the simplest package management in runtime
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
 [![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/instld)
 [![Test-Package](https://github.com/pomponchik/instld/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/instld/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
```

### Comparing `instld-0.0.8/README.md` & `instld-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![logo](/docs/assets/logo5.png)
+
 # INSTLD: the simplest package management in runtime
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
 [![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/instld)
 [![Test-Package](https://github.com/pomponchik/instld/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/instld/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
```

### Comparing `instld-0.0.8/installed/context.py` & `instld-0.0.9/installed/context.py`

 * *Files identical despite different names*

### Comparing `instld-0.0.8/installed/context_manager.py` & `instld-0.0.9/installed/context_manager.py`

 * *Files identical despite different names*

### Comparing `instld-0.0.8/installed/proxy_module.py` & `instld-0.0.9/installed/proxy_module.py`

 * *Files identical despite different names*

### Comparing `instld-0.0.8/installed/runner.py` & `instld-0.0.9/installed/runner.py`

 * *Files identical despite different names*

### Comparing `instld-0.0.8/instld.egg-info/PKG-INFO` & `instld-0.0.9/instld.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: instld
-Version: 0.0.8
+Version: 0.0.9
 Summary: The simplest package management in runtime
 Home-page: https://github.com/pomponchik/instld
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![logo](/docs/assets/logo5.png)
+
 # INSTLD: the simplest package management in runtime
 
 [![Downloads](https://pepy.tech/badge/instld/month)](https://pepy.tech/project/instld)
 [![Downloads](https://pepy.tech/badge/instld)](https://pepy.tech/project/instld)
 [![codecov](https://codecov.io/gh/pomponchik/installed/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/instld)
 [![Test-Package](https://github.com/pomponchik/instld/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/instld/actions/workflows/coverage.yml)
 [![Python versions](https://img.shields.io/pypi/pyversions/instld.svg)](https://pypi.python.org/pypi/instld)
```

### Comparing `instld-0.0.8/setup.py` & `instld-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="instld",
-    version="0.0.8",
+    version="0.0.9",
     author="Evgeniy Blinov",
     author_email="zheni-b@yandex.ru",
     description="The simplest package management in runtime",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pomponchik/instld",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `instld-0.0.8/tests/units/test_proxy_module.py` & `instld-0.0.9/tests/units/test_proxy_module.py`

 * *Files identical despite different names*

