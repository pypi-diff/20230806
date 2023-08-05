# Comparing `tmp/pyschlage-2023.7.0.tar.gz` & `tmp/pyschlage-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschlage-2023.7.0.tar", last modified: Thu Jul 27 02:47:25 2023, max compression
+gzip compressed data, was "pyschlage-2023.8.0.tar", last modified: Sat Aug  5 22:04:02 2023, max compression
```

## Comparing `pyschlage-2023.7.0.tar` & `pyschlage-2023.8.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.216322 pyschlage-2023.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.220322 pyschlage-2023.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.220322 pyschlage-2023.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.220322 pyschlage-2023.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.220322 pyschlage-2023.7.0/pyschlage/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/pyschlage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/pyschlage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 02:47:25.000000 pyschlage-2023.7.0/pyschlage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:47:24.000000 pyschlage-2023.7.0/pyschlage.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:25.224321 pyschlage-2023.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-27 02:47:08.000000 pyschlage-2023.7.0/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.225493 pyschlage-2023.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.225493 pyschlage-2023.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.225493 pyschlage-2023.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.225493 pyschlage-2023.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/pyschlage/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/pyschlage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/pyschlage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 22:04:02.000000 pyschlage-2023.8.0/pyschlage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:04:01.000000 pyschlage-2023.8.0/pyschlage.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:04:02.229493 pyschlage-2023.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-05 22:03:47.000000 pyschlage-2023.8.0/tests/test_user.py
```

### Comparing `pyschlage-2023.7.0/.devcontainer.json` & `pyschlage-2023.8.0/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/.github/workflows/build-and-test.yml` & `pyschlage-2023.8.0/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/.github/workflows/publish-python.yml` & `pyschlage-2023.8.0/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/.gitignore` & `pyschlage-2023.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/.pre-commit-config.yaml` & `pyschlage-2023.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/LICENSE` & `pyschlage-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/PKG-INFO` & `pyschlage-2023.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.7.0/README.md` & `pyschlage-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/docs/Makefile` & `pyschlage-2023.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/docs/api.rst` & `pyschlage-2023.8.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/docs/index.rst` & `pyschlage-2023.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/docs/make.bat` & `pyschlage-2023.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyproject.toml` & `pyschlage-2023.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage/api.py` & `pyschlage-2023.8.0/pyschlage/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,15 +23,19 @@
 
         :rtype: list[Lock]
         :raise pyschlage.exceptions.NotAuthorizedError: When authentication fails.
         :raise pyschlage.exceptions.UnknownError: On other errors.
         """
         path = Lock.request_path()
         response = self._auth.request("get", path, params={"archetype": "lock"})
-        return [Lock.from_json(self._auth, d) for d in response.json()]
+        locks = []
+        for lock_json in response.json():
+            lock = Lock.from_json(self._auth, lock_json)
+            lock.refresh_access_codes()
+        return locks
 
     def users(self) -> list[User]:
         """Retrieves all users associated with this account's locks.
 
         :rtype: list[User]
         :raise pyschlage.exceptions.NotAuthorizedError: When authentication fails.
         :raise pyschlage.exceptions.UnknownError: On other errors.
```

### Comparing `pyschlage-2023.7.0/pyschlage/auth.py` & `pyschlage-2023.8.0/pyschlage/auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage/code.py` & `pyschlage-2023.8.0/pyschlage/code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage/common.py` & `pyschlage-2023.8.0/pyschlage/common.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage/device.py` & `pyschlage-2023.8.0/pyschlage/device.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage/log.py` & `pyschlage-2023.8.0/pyschlage/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,23 +66,23 @@
 @dataclass
 class LockLog:
     """A lock log entry."""
 
     created_at: datetime
     """The time at which the log entry was created."""
 
-    accessor_id: str | None
+    message: str
+    """The human-readable message associated with the log entry."""
+
+    accessor_id: str | None = None
     """Unique identifier for the user that triggered the log entry."""
 
-    access_code_id: str | None
+    access_code_id: str | None = None
     """Unique identifier for the access code that triggered the log entry."""
 
-    message: str
-    """The human-readable message associated with the log entry."""
-
     @staticmethod
     def request_path(device_id: str) -> str:
         """Returns the request path for the LockLog.
 
         :meta private:
         """
         return f"devices/{device_id}/logs"
```

### Comparing `pyschlage-2023.7.0/pyschlage/user.py` & `pyschlage-2023.8.0/pyschlage/user.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/pyschlage.egg-info/PKG-INFO` & `pyschlage-2023.8.0/pyschlage.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschlage
-Version: 2023.7.0
+Version: 2023.8.0
 Summary: Python API for interacting with Schlage WiFi locks.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Project-URL: Documentation, https://pyschlage.readthedocs.io
```

### Comparing `pyschlage-2023.7.0/pyschlage.egg-info/SOURCES.txt` & `pyschlage-2023.8.0/pyschlage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/tests/conftest.py` & `pyschlage-2023.8.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from unittest import mock
 
 from pytest import fixture
 
 from pyschlage.auth import Auth
+from pyschlage.code import AccessCode
+from pyschlage.lock import Lock
 
 
 @fixture
 def mock_auth():
     yield mock.create_autospec(Auth, spec_set=True, user_id="<user-id>")
 
 
@@ -100,14 +102,23 @@
         "serialNumber": "serial-number",
         "timezone": -20,
         "users": lock_users_json,
     }
 
 
 @fixture
+def wifi_lock(
+    mock_auth: mock.Mock, wifi_lock_json: dict, access_code: AccessCode
+) -> Lock:
+    lock = Lock.from_json(mock_auth, wifi_lock_json)
+    lock.access_codes = {access_code.access_code_id: access_code}
+    return lock
+
+
+@fixture
 def wifi_lock_unavailable_json(wifi_lock_json):
     keep = ("modelName", "serialNumber", "macAddress", "SAT", "CAT")
     for k in list(wifi_lock_json["attributes"].keys()):
         if k not in keep:
             del wifi_lock_json["attributes"][k]
     return wifi_lock_json
 
@@ -182,14 +193,19 @@
             "startHour": 0,
             "startMinute": 0,
         },
     }
 
 
 @fixture
+def access_code(mock_auth: mock.Mock, access_code_json: dict) -> AccessCode:
+    return AccessCode.from_json(mock_auth, access_code_json, "__device_uuid__")
+
+
+@fixture
 def log_json():
     return {
         "createdAt": "2023-03-01T17:26:47.366Z",
         "deviceId": "__device_uuid__",
         "logId": "__log_uuid__",
         "message": {
             "accessorUuid": "ffffffff-ffff-ffff-ffff-ffffffffffff",
```

### Comparing `pyschlage-2023.7.0/tests/test_auth.py` & `pyschlage-2023.8.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/tests/test_code.py` & `pyschlage-2023.8.0/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `pyschlage-2023.7.0/tests/test_log.py` & `pyschlage-2023.8.0/tests/test_log.py`

 * *Files identical despite different names*

