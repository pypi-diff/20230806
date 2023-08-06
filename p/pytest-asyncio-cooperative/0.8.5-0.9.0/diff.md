# Comparing `tmp/pytest-asyncio-cooperative-0.8.5.tar.gz` & `tmp/pytest-asyncio-cooperative-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-asyncio-cooperative-0.8.5.tar", last modified: Sun May 24 02:37:14 2020, max compression
+gzip compressed data, was "dist/pytest-asyncio-cooperative-0.9.0.tar", last modified: Sun May 31 03:17:41 2020, max compression
```

## Comparing `pytest-asyncio-cooperative-0.8.5.tar` & `pytest-asyncio-cooperative-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/
--rw-r--r--   0 willem     (501) staff       (20)     3121 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/PKG-INFO
--rw-r--r--   0 willem     (501) staff       (20)     1608 2020-05-23 04:35:42.000000 pytest-asyncio-cooperative-0.8.5/README.rst
-drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/
--rw-r--r--   0 willem     (501) staff       (20)        0 2020-03-22 04:51:18.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/__init__.py
--rw-r--r--   0 willem     (501) staff       (20)      764 2020-03-29 01:08:52.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/assertion.py
--rw-r--r--   0 willem     (501) staff       (20)        0 2020-05-23 04:21:05.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/hypothesis.py
--rw-r--r--   0 willem     (501) staff       (20)    12573 2020-05-24 02:31:11.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/plugin.py
-drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/
--rw-r--r--   0 willem     (501) staff       (20)     3121 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/PKG-INFO
--rw-r--r--   0 willem     (501) staff       (20)      478 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/SOURCES.txt
--rw-r--r--   0 willem     (501) staff       (20)        1 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/dependency_links.txt
--rw-r--r--   0 willem     (501) staff       (20)       68 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/entry_points.txt
--rw-r--r--   0 willem     (501) staff       (20)       14 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/requires.txt
--rw-r--r--   0 willem     (501) staff       (20)       27 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/top_level.txt
--rw-r--r--   0 willem     (501) staff       (20)       38 2020-05-24 02:37:14.000000 pytest-asyncio-cooperative-0.8.5/setup.cfg
--rw-r--r--   0 willem     (501) staff       (20)     1506 2020-05-24 02:36:50.000000 pytest-asyncio-cooperative-0.8.5/setup.py
+drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/
+-rw-r--r--   0 willem     (501) staff       (20)     3537 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/PKG-INFO
+-rw-r--r--   0 willem     (501) staff       (20)     1976 2020-05-31 03:10:08.000000 pytest-asyncio-cooperative-0.9.0/README.rst
+drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/
+-rw-r--r--   0 willem     (501) staff       (20)        0 2020-03-22 04:51:18.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/__init__.py
+-rw-r--r--   0 willem     (501) staff       (20)      764 2020-03-29 01:08:52.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/assertion.py
+-rw-r--r--   0 willem     (501) staff       (20)        0 2020-05-23 04:21:05.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/hypothesis.py
+-rw-r--r--   0 willem     (501) staff       (20)    12854 2020-05-31 03:14:58.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/plugin.py
+drwxr-xr-x   0 willem     (501) staff       (20)        0 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/
+-rw-r--r--   0 willem     (501) staff       (20)     3537 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/PKG-INFO
+-rw-r--r--   0 willem     (501) staff       (20)      478 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/SOURCES.txt
+-rw-r--r--   0 willem     (501) staff       (20)        1 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/dependency_links.txt
+-rw-r--r--   0 willem     (501) staff       (20)       68 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/entry_points.txt
+-rw-r--r--   0 willem     (501) staff       (20)       14 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/requires.txt
+-rw-r--r--   0 willem     (501) staff       (20)       27 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/top_level.txt
+-rw-r--r--   0 willem     (501) staff       (20)       38 2020-05-31 03:17:41.000000 pytest-asyncio-cooperative-0.9.0/setup.cfg
+-rw-r--r--   0 willem     (501) staff       (20)     1506 2020-05-31 03:15:53.000000 pytest-asyncio-cooperative-0.9.0/setup.py
```

### Comparing `pytest-asyncio-cooperative-0.8.5/PKG-INFO` & `pytest-asyncio-cooperative-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-asyncio-cooperative
-Version: 0.8.5
+Version: 0.9.0
 Summary: Run all your asynchronous tests cooperatively.
 Home-page: https://github.com/willemt/pytest-asyncio-cooperative
 Author: Willem Thiart
 Author-email: himself@willemthiart.com
 Maintainer: Willem Thiart
 Maintainer-email: himself@willemthiart.com
 License: MIT
@@ -70,14 +70,20 @@
         
         - Order of tests is not guaranteed (ie. some blocking operations might taken longer and affect the order of test results)
         
         - Tests MUST be isolated from each other (ie. NO shared resources, NO `mock.patch`)
         
         - There is NO parallelism, CPU bound tests will NOT get a performance benefit
         
+        Known Issues
+        ------------
+        
+        *Synchronous tests fail to run when async tests fail*
+        Async tests are run BEFORE synchronous tests. If an async test fails then synchronous tests will NOT run. Therefore the synchronous tests will not report to have passed or failed. It's recommended that if you are using asyncio-cooperative, then you should use `async` for ALL fixtures.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-asyncio-cooperative-0.8.5/README.rst` & `pytest-asyncio-cooperative-0.9.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -59,7 +59,13 @@
 - All tests MUST be coroutines (ie. have the `async` keyword)
 
 - Order of tests is not guaranteed (ie. some blocking operations might taken longer and affect the order of test results)
 
 - Tests MUST be isolated from each other (ie. NO shared resources, NO `mock.patch`)
 
 - There is NO parallelism, CPU bound tests will NOT get a performance benefit
+
+Known Issues
+------------
+
+*Synchronous tests fail to run when async tests fail*
+Async tests are run BEFORE synchronous tests. If an async test fails then synchronous tests will NOT run. Therefore the synchronous tests will not report to have passed or failed. It's recommended that if you are using asyncio-cooperative, then you should use `async` for ALL fixtures.
```

### Comparing `pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/assertion.py` & `pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/assertion.py`

 * *Files identical despite different names*

### Comparing `pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative/plugin.py` & `pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,29 +172,35 @@
 
         value = await fixture.func(*fixture_values)
         return value, teardowns
 
     # Regular fixture
     # FIXME: we should use more of pytest's fixture system
     elif inspect.isgeneratorfunction(fixture.func):
-        gen = fixture.func()
-        return gen.__next__(), [gen]
+        fixture_values, teardowns = await _fill_fixture_fixtures(
+            _fixtureinfo, fixture, item
+        )
+        gen = fixture.func(*fixture_values)
+        return gen.__next__(), teardowns + [gen]
 
     # It's a parameterization
     # FIXME: we should use more of pytest's fixture system
     elif fixture.params:
         request = item._request
         request.param = item._pyfuncitem.callspec.params[fixture.argname]
         val = fixture.func(request)
         return val, []
 
     # FIXME: we should use more of pytest's fixture system
     elif inspect.isfunction(fixture.func):
-        val = fixture.func()
-        return val, []
+        fixture_values, teardowns = await _fill_fixture_fixtures(
+            _fixtureinfo, fixture, item
+        )
+        val = fixture.func(*fixture_values)
+        return val, teardowns
 
     else:
         raise Exception(
             f"Something is strange about the fixture '{fixture.func.__name__}'.\n"
             f"Please create an issue with reproducible sample on github."
         )
```

### Comparing `pytest-asyncio-cooperative-0.8.5/pytest_asyncio_cooperative.egg-info/PKG-INFO` & `pytest-asyncio-cooperative-0.9.0/pytest_asyncio_cooperative.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-asyncio-cooperative
-Version: 0.8.5
+Version: 0.9.0
 Summary: Run all your asynchronous tests cooperatively.
 Home-page: https://github.com/willemt/pytest-asyncio-cooperative
 Author: Willem Thiart
 Author-email: himself@willemthiart.com
 Maintainer: Willem Thiart
 Maintainer-email: himself@willemthiart.com
 License: MIT
@@ -70,14 +70,20 @@
         
         - Order of tests is not guaranteed (ie. some blocking operations might taken longer and affect the order of test results)
         
         - Tests MUST be isolated from each other (ie. NO shared resources, NO `mock.patch`)
         
         - There is NO parallelism, CPU bound tests will NOT get a performance benefit
         
+        Known Issues
+        ------------
+        
+        *Synchronous tests fail to run when async tests fail*
+        Async tests are run BEFORE synchronous tests. If an async test fails then synchronous tests will NOT run. Therefore the synchronous tests will not report to have passed or failed. It's recommended that if you are using asyncio-cooperative, then you should use `async` for ALL fixtures.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-asyncio-cooperative-0.8.5/setup.py` & `pytest-asyncio-cooperative-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-asyncio-cooperative",
-    version="0.8.5",
+    version="0.9.0",
     author="Willem Thiart",
     author_email="himself@willemthiart.com",
     maintainer="Willem Thiart",
     maintainer_email="himself@willemthiart.com",
     license="MIT",
     url="https://github.com/willemt/pytest-asyncio-cooperative",
     description="Run all your asynchronous tests cooperatively.",
```

