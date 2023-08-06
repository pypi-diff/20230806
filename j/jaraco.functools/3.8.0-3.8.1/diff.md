# Comparing `tmp/jaraco.functools-3.8.0.tar.gz` & `tmp/jaraco.functools-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.functools-3.8.0.tar", last modified: Mon Jun 26 01:20:44 2023, max compression
+gzip compressed data, was "jaraco.functools-3.8.1.tar", last modified: Sun Aug  6 00:02:42 2023, max compression
```

## Comparing `jaraco.functools-3.8.0.tar` & `jaraco.functools-3.8.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/jaraco/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/jaraco.functools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-26 01:20:44.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.112311 jaraco.functools-3.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/jaraco/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:02:42.116311 jaraco.functools-3.8.1/jaraco.functools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-06 00:02:42.000000 jaraco.functools-3.8.1/jaraco.functools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-06 00:02:42.000000 jaraco.functools-3.8.1/jaraco.functools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:02:42.000000 jaraco.functools-3.8.1/jaraco.functools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 00:02:42.000000 jaraco.functools-3.8.1/jaraco.functools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 00:02:42.000000 jaraco.functools-3.8.1/jaraco.functools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 00:02:42.120311 jaraco.functools-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-06 00:02:17.000000 jaraco.functools-3.8.1/tox.ini
```

### Comparing `jaraco.functools-3.8.0/.github/workflows/main.yml` & `jaraco.functools-3.8.1/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,29 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -109,16 +109,16 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.functools-3.8.0/LICENSE` & `jaraco.functools-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.8.0/NEWS.rst` & `jaraco.functools-3.8.1/NEWS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.8.1
+======
+
+Bugfixes
+--------
+
+- Restored type checking and repaired broken exclusion. (#50550895)
+
+
 v3.8.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `jaraco.functools-3.8.0/PKG-INFO` & `jaraco.functools-3.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.8.0
+Version: 3.8.1
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -47,14 +47,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.functools-3.8.0/README.rst` & `jaraco.functools-3.8.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.functools-3.8.0/conftest.py` & `jaraco.functools-3.8.1/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.8.0/docs/conf.py` & `jaraco.functools-3.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.8.0/jaraco/functools.py` & `jaraco.functools-3.8.1/jaraco/functools.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,17 @@
         cached_method = cache_wrapper(bound_method)
         setattr(self, method.__name__, cached_method)
         return cached_method(*args, **kwargs)
 
     # Support cache clear even before cache has been created.
     wrapper.cache_clear = lambda: None  # type: ignore[attr-defined]
 
-    return (  # type: ignore[return-value]
-        _special_method_cache(method, cache_wrapper) or wrapper
+    return (
+        _special_method_cache(method, cache_wrapper)  # type: ignore[return-value]
+        or wrapper
     )
 
 
 def _special_method_cache(method, cache_wrapper):
     """
     Because Python treats special methods differently, it's not
     possible to use instance attributes to implement the cached
```

### Comparing `jaraco.functools-3.8.0/jaraco.functools.egg-info/PKG-INFO` & `jaraco.functools-3.8.1/jaraco.functools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.8.0
+Version: 3.8.1
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -47,14 +47,7 @@
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
 
 `Learn more <https://tidelift.com/subscription/pkg/pypi-jaraco.functools?utm_source=pypi-jaraco.functools&utm_medium=referral&utm_campaign=github>`_.
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
```

### Comparing `jaraco.functools-3.8.0/jaraco.functools.egg-info/SOURCES.txt` & `jaraco.functools-3.8.1/jaraco.functools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 NEWS.rst
 README.rst
+SECURITY.md
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 test_functools.py
 towncrier.toml
```

### Comparing `jaraco.functools-3.8.0/pytest.ini` & `jaraco.functools-3.8.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.8.0/setup.cfg` & `jaraco.functools-3.8.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	jaraco.classes
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 	
 	jaraco.tidelift >= 1.4
 
 [options.entry_points]
```

### Comparing `jaraco.functools-3.8.0/test_functools.py` & `jaraco.functools-3.8.1/test_functools.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.8.0/tox.ini` & `jaraco.functools-3.8.1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[tox]
-toxworkdir={env:TOX_WORK_DIR:.tox}
-
-
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
```

