# Comparing `tmp/npc_session-0.1.0.tar.gz` & `tmp/npc_session-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_session-0.1.0.tar", last modified: Sun Aug  6 05:37:30 2023, max compression
+gzip compressed data, was "npc_session-0.1.1.tar", last modified: Sun Aug  6 06:17:56 2023, max compression
```

## Comparing `npc_session-0.1.0.tar` & `npc_session-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 05:37:30.135563 npc_session-0.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1205 2023-08-06 05:37:30.135563 npc_session-0.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      519 2023-08-06 05:13:34.000000 npc_session-0.1.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2983 2023-08-06 05:34:40.000000 npc_session-0.1.0/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-06 05:37:30.135563 npc_session-0.1.0/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 05:37:30.131563 npc_session-0.1.0/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 05:37:30.131563 npc_session-0.1.0/src/npc_session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      129 2023-08-06 05:18:15.000000 npc_session-0.1.0/src/npc_session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4621 2023-08-06 03:51:30.000000 npc_session-0.1.0/src/npc_session/parsing.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14216 2023-08-06 05:32:36.000000 npc_session-0.1.0/src/npc_session/records.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      743 2023-08-06 05:11:45.000000 npc_session-0.1.0/src/npc_session/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 05:37:30.135563 npc_session-0.1.0/src/npc_session.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1205 2023-08-06 05:37:30.000000 npc_session-0.1.0/src/npc_session.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      325 2023-08-06 05:37:30.000000 npc_session-0.1.0/src/npc_session.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-06 05:37:30.000000 npc_session-0.1.0/src/npc_session.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2023-08-06 05:37:30.000000 npc_session-0.1.0/src/npc_session.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-08-06 05:37:30.000000 npc_session-0.1.0/src/npc_session.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 06:17:56.439563 npc_session-0.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1379 2023-08-06 06:17:56.439563 npc_session-0.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      643 2023-08-06 05:39:40.000000 npc_session-0.1.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2904 2023-08-06 06:17:15.000000 npc_session-0.1.1/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-06 06:17:56.439563 npc_session-0.1.1/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 06:17:56.435563 npc_session-0.1.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 06:17:56.435563 npc_session-0.1.1/src/npc_session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      129 2023-08-06 05:18:15.000000 npc_session-0.1.1/src/npc_session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4743 2023-08-06 06:11:55.000000 npc_session-0.1.1/src/npc_session/jobs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4621 2023-08-06 03:51:30.000000 npc_session-0.1.1/src/npc_session/parsing.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14216 2023-08-06 05:32:36.000000 npc_session-0.1.1/src/npc_session/records.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      743 2023-08-06 05:11:45.000000 npc_session-0.1.1/src/npc_session/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-06 06:17:56.439563 npc_session-0.1.1/src/npc_session.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1379 2023-08-06 06:17:56.000000 npc_session-0.1.1/src/npc_session.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      349 2023-08-06 06:17:56.000000 npc_session-0.1.1/src/npc_session.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-06 06:17:56.000000 npc_session-0.1.1/src/npc_session.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      106 2023-08-06 06:17:56.000000 npc_session-0.1.1/src/npc_session.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-08-06 06:17:56.000000 npc_session-0.1.1/src/npc_session.egg-info/top_level.txt
```

### Comparing `npc_session-0.1.0/PKG-INFO` & `npc_session-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: npc_session
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # npc_session
-**n**euro**p**ixels **c**loud **session**
 
+**n**euro**p**ixels **c**loud **session**
+	
 Interfaces for working with behavior and epyhys sessions from the
 Mindscope Neuropixels team, in the cloud.
 
+[![Python
+Versions](https://img.shields.io/pypi/pyversions/npc_sessions.svg)](https://pypi.python.org/pypi/npc-sessions/)
 ## quickstart
 
 ```bash
 pip install npc_session
 ```
 
 Parse a normalized IDs from a path or string:
```

### Comparing `npc_session-0.1.0/README.md` & `npc_session-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # npc_session
-**n**euro**p**ixels **c**loud **session**
 
+**n**euro**p**ixels **c**loud **session**
+	
 Interfaces for working with behavior and epyhys sessions from the
 Mindscope Neuropixels team, in the cloud.
 
+[![Python
+Versions](https://img.shields.io/pypi/pyversions/npc_sessions.svg)](https://pypi.python.org/pypi/npc-sessions/)
 ## quickstart
 
 ```bash
 pip install npc_session
 ```
 
 Parse a normalized IDs from a path or string:
```

### Comparing `npc_session-0.1.0/pyproject.toml` & `npc_session-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "npc_session"
-version = "0.1.0"
+version = "0.1.1"
 description = "Interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud."
 authors = [
     {name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org"},
 ]
 dependencies = [
     "typing-extensions>=4.7.1",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
@@ -27,27 +28,27 @@
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.4.0",
     "ruff>=0.0.282",
     "pytest-cov>=4.1.0",
     "mypy>=1.4.1",
+    "pdm-bump>=0.4.0",
 ]
 
 [tool.pdm.scripts]
 # usage: pdm run <script> [args]
 ruff = "ruff check src --fix-only"
 black = "black src"
 test = "pytest --cov"
-prebuild = {composite = ["black", "ruff", "test", "pdm run mypy src"]}
-bump = "pdm bump -p pyproject.toml" # defaults to patch; `pdm run bump -m` to bump minor
-build = {composite = ["prebuild", "pdm build"]}
+mypy = "mypy src"
+prebuild = {composite = ["black", "ruff", "test", "mypy"]}
+bump = "pdm bump micro"
 dryrun = {composite = ["prebuild", "pdm build", "pdm publish --no-build --repository https://test.pypi.org/simple"]}
-publish = {composite = ["prebuild", "pdm build", "pdm publish --no-build"]}
-pub = {composite = ["bump", "pdm publish"]}
+pub = {composite = ["prebuild", "pdm build", "bump", "pdm publish --no-build"]}
 
 [tool.ruff]
 fix = true
 ignore-init-module-imports = true
 # See https://github.com/charliermarsh/ruff#rules for error code definitions.
 select = [
     "ANN", # annotations
@@ -60,18 +61,18 @@
     "N", # naming
     "U", # upgrade
     "W", # style warnings
     "YTT", # sys.version
 ]
 extend-exclude = ["tests"]
 src = ["src", "tests"]
-target-version = "py39"
+target-version = "py38"
 
 [tool.black]
-target-version = ['py39']
+target-version = ['py38']
 
 [tool.ruff.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
 
 [tool.coverage.paths]
 source = ["src"]
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_yki0v5tf_/tmpmk8p1wfi_TarContainer/0/3.toml", line 116, column 1: CDATA terminal not found*

 * *File "/tmp/diffoscope_yki0v5tf_/tmpmk8p1wfi_TarContainer/0/3.toml", line 116, column 1: CDATA terminal not found*

```diff
@@ -1,13 +1,14 @@
-[project] name = "npc_session" version = "0.1.0" description = "Interfaces for
+[project] name = "npc_session" version = "0.1.1" description = "Interfaces for
 working with behavior and epyhys sessions from the Mindscope Neuropixels team,
 in the cloud." authors = [ {name = "Ben Hardcastle", email =
 "ben.hardcastle@alleninstitute.org"}, ] dependencies = [ "typing-
-extensions>=4.7.1", ] requires-python = ">=3.9" readme = "README.md" license =
+extensions>=4.7.1", ] requires-python = ">=3.8" readme = "README.md" license =
 {text = "MIT"} classifiers = [ "Programming Language :: Python :: 3",
-"Programming Language :: Python :: 3.9", "Programming Language :: Python ::
-3.10", "Programming Language :: Python :: 3.11", "License :: OSI Approved ::
-MIT License", "Operating System :: Microsoft :: Windows", "Operating System ::
-POSIX :: Linux", ] [build-system] requires = ["setuptools>=61", "wheel"] build-
-backend = "setuptools.build_meta" [project.optional-dependencies] dev =
-[ "pytest>=7.4.0", "ruff>=0.0.282", "pytest-cov>=4.1.0", "mypy>=1.4.1", ]
-[tool.pdm.scripts] # usage: pdm run
+"Programming Language :: Python :: 3.8", "Programming Language :: Python ::
+3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python
+:: 3.11", "License :: OSI Approved :: MIT License", "Operating System ::
+Microsoft :: Windows", "Operating System :: POSIX :: Linux", ] [build-system]
+requires = ["setuptools>=61", "wheel"] build-backend = "setuptools.build_meta"
+[project.optional-dependencies] dev = [ "pytest>=7.4.0", "ruff>=0.0.282",
+"pytest-cov>=4.1.0", "mypy>=1.4.1", "pdm-bump>=0.4.0", ] [tool.pdm.scripts] #
+usage: pdm run
```

### Comparing `npc_session-0.1.0/src/npc_session/parsing.py` & `npc_session-0.1.1/src/npc_session/parsing.py`

 * *Files identical despite different names*

### Comparing `npc_session-0.1.0/src/npc_session/records.py` & `npc_session-0.1.1/src/npc_session/records.py`

 * *Files identical despite different names*

### Comparing `npc_session-0.1.0/src/npc_session/utils.py` & `npc_session-0.1.1/src/npc_session/utils.py`

 * *Files identical despite different names*

### Comparing `npc_session-0.1.0/src/npc_session.egg-info/PKG-INFO` & `npc_session-0.1.1/src/npc_session.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: npc-session
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interfaces for working with behavior and epyhys sessions from the Mindscope Neuropixels team, in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # npc_session
-**n**euro**p**ixels **c**loud **session**
 
+**n**euro**p**ixels **c**loud **session**
+	
 Interfaces for working with behavior and epyhys sessions from the
 Mindscope Neuropixels team, in the cloud.
 
+[![Python
+Versions](https://img.shields.io/pypi/pyversions/npc_sessions.svg)](https://pypi.python.org/pypi/npc-sessions/)
 ## quickstart
 
 ```bash
 pip install npc_session
 ```
 
 Parse a normalized IDs from a path or string:
```

