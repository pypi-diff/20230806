# Comparing `tmp/grimoirelab-0.9.1.tar.gz` & `tmp/grimoirelab-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab-0.9.1.tar", max compression
+gzip compressed data, was "grimoirelab-0.9.2.tar", max compression
```

## Comparing `grimoirelab-0.9.1.tar` & `grimoirelab-0.9.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2023-04-27 10:21:08.903849 grimoirelab-0.9.1/LICENSE
--rw-r--r--   0        0        0     8685 2023-04-27 10:21:08.903849 grimoirelab-0.9.1/README.md
--rw-r--r--   0        0        0       34 2023-04-27 10:21:08.987842 grimoirelab-0.9.1/grimoirelab/__init__.py
--rw-r--r--   0        0        0       86 2023-04-27 10:21:08.987842 grimoirelab-0.9.1/grimoirelab/_version.py
--rwxr-xr-x   0        0        0     1844 2023-04-27 10:21:08.987842 grimoirelab-0.9.1/grimoirelab/grimoirelab.py
--rw-r--r--   0        0        0     1845 2023-04-27 10:21:08.987842 grimoirelab-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10208 1970-01-01 00:00:00.000000 grimoirelab-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-04-28 17:19:02.418544 grimoirelab-0.9.2/LICENSE
+-rw-r--r--   0        0        0     8685 2023-04-28 17:19:02.418544 grimoirelab-0.9.2/README.md
+-rw-r--r--   0        0        0       34 2023-04-28 17:19:02.502552 grimoirelab-0.9.2/grimoirelab/__init__.py
+-rw-r--r--   0        0        0       86 2023-04-28 17:19:02.502552 grimoirelab-0.9.2/grimoirelab/_version.py
+-rwxr-xr-x   0        0        0     1844 2023-04-28 17:19:02.502552 grimoirelab-0.9.2/grimoirelab/grimoirelab.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:19:02.506552 grimoirelab-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10208 1970-01-01 00:00:00.000000 grimoirelab-0.9.2/PKG-INFO
```

### Comparing `grimoirelab-0.9.1/LICENSE` & `grimoirelab-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.1/README.md` & `grimoirelab-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.1/grimoirelab/grimoirelab.py` & `grimoirelab-0.9.2/grimoirelab/grimoirelab.py`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.1/pyproject.toml` & `grimoirelab-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab"
-version = "0.9.1"
+version = "0.9.2"
 description = "Tool set for software development analytics"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -39,21 +39,21 @@
 python = "^3.7.1"
 
 grimoirelab-toolkit = {version = ">=0.3.4", allow-prereleases = true}
 perceval-mozilla = {version = ">=0.3.10", allow-prereleases = true}
 perceval-opnfv = {version = ">=0.2.10", allow-prereleases = true}
 perceval-puppet = {version = ">=0.2.10", allow-prereleases = true}
 perceval-weblate = {version = ">=0.2.10", allow-prereleases = true}
-sortinghat = {version = ">=0.9.2", allow-prereleases = true}
+sortinghat = {version = ">=0.9.3", allow-prereleases = true}
 kidash = {version = ">=0.5.5", allow-prereleases = true}
 grimoirelab-panels = {version = ">=0.2.0", allow-prereleases = true}
-grimoire-elk = {version = ">=0.104.5", allow-prereleases = true}
-sirmordred = {version = ">=0.7.1", allow-prereleases = true}
+grimoire-elk = {version = ">=0.104.6", allow-prereleases = true}
+sirmordred = {version = ">=0.7.2", allow-prereleases = true}
 cereslib = {version = ">=0.4.0", allow-prereleases = true}
-graal = {version = ">=0.4.7", allow-prereleases = true}
+graal = {version = ">=0.4.8", allow-prereleases = true}
 statsmodels = "^0.13.2"
 perceval = {version = ">=0.21.6", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `grimoirelab-0.9.1/PKG-INFO` & `grimoirelab-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tool set for software development analytics
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,26 +14,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: cereslib (>=0.4.0)
-Requires-Dist: graal (>=0.4.7)
-Requires-Dist: grimoire-elk (>=0.104.5)
+Requires-Dist: graal (>=0.4.8)
+Requires-Dist: grimoire-elk (>=0.104.6)
 Requires-Dist: grimoirelab-panels (>=0.2.0)
 Requires-Dist: grimoirelab-toolkit (>=0.3.4)
 Requires-Dist: kidash (>=0.5.5)
 Requires-Dist: perceval (>=0.21.6)
 Requires-Dist: perceval-mozilla (>=0.3.10)
 Requires-Dist: perceval-opnfv (>=0.2.10)
 Requires-Dist: perceval-puppet (>=0.2.10)
 Requires-Dist: perceval-weblate (>=0.2.10)
-Requires-Dist: sirmordred (>=0.7.1)
-Requires-Dist: sortinghat (>=0.9.2)
+Requires-Dist: sirmordred (>=0.7.2)
+Requires-Dist: sortinghat (>=0.9.3)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab
 Description-Content-Type: text/markdown
 
 # GrimoireLab
```

