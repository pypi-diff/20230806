# Comparing `tmp/podmanclispawner-0.1.0.tar.gz` & `tmp/podmanclispawner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podmanclispawner-0.1.0.tar", last modified: Sun Sep 19 19:51:09 2021, max compression
+gzip compressed data, was "podmanclispawner-0.2.0.tar", last modified: Sun Aug  6 12:51:00 2023, max compression
```

## Comparing `podmanclispawner-0.1.0.tar` & `podmanclispawner-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/podmanclispawner/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/podmanclispawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8649 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/podmanclispawner/podmanspawner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/podmanclispawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      499 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-09-19 19:51:09.000000 podmanclispawner-0.1.0/podmanclispawner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:09.770741 podmanclispawner-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2021-09-19 19:51:00.000000 podmanclispawner-0.1.0/tests/test_spawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.378294 podmanclispawner-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.374294 podmanclispawner-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.374294 podmanclispawner-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-06 12:51:00.378294 podmanclispawner-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.374294 podmanclispawner-0.2.0/podmanclispawner/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/podmanclispawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/podmanclispawner/podmanspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.374294 podmanclispawner-0.2.0/podmanclispawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 12:51:00.000000 podmanclispawner-0.2.0/podmanclispawner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:51:00.378294 podmanclispawner-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:00.378294 podmanclispawner-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-06 12:50:45.000000 podmanclispawner-0.2.0/tests/test_spawner.py
```

### Comparing `podmanclispawner-0.1.0/.github/workflows/workflow.yml` & `podmanclispawner-0.2.0/.github/workflows/workflow.yml`

 * *Files 14% similar despite different names*

```diff
@@ -3,68 +3,73 @@
 name: Build
 on: [push, pull_request]
 
 jobs:
   # https://github.com/pre-commit/action
   pre-commit:
     name: Lint
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
+    timeout-minutes: 5
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
-      - uses: pre-commit/action@v2.0.0
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
+
+      - uses: pre-commit/action@v3.0.0
 
   test:
     name: Test
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
+    timeout-minutes: 10
     steps:
-      - name: Enable rootless podman
-        run: |
-          sudo apt-get update -q
-          sudo apt-get install -q -y fuse-overlayfs
-          podman info
-          slirp4netns --version
-          fuse-overlayfs --version
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
         with:
-          python-version: "3.8"
-      - uses: actions/setup-node@v1
-      - name: Cache pip
-        uses: actions/cache@v2
+          python-version: "3.10"
+          cache: pip
+          cache-dependency-path: dev-requirements.txt
+
+      - uses: actions/setup-node@v3
         with:
-          # This path is specific to Ubuntu
-          path: ~/.cache/pip
-          # Look to see if there is a cache hit for the corresponding requirements file
-          key: ${{ runner.os }}-pip-${{ hashFiles('*requirements.txt') }}
-          restore-keys: |
-            ${{ runner.os }}-pip-
-            ${{ runner.os }}-
+          node-version: "18"
+
       - name: Install dependencies
         run: |
           python -m pip install -r dev-requirements.txt
           npm install -g configurable-http-proxy
+
       - name: Update setuptools_scm version
         run: python setup.py build
+
       - name: Run tests
         run: pytest tests -v
 
   # https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
   publish-pypi:
     name: Pypi
     needs:
       # Only publish if other jobs passed
       - pre-commit
       - test
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
+    timeout-minutes: 5
     steps:
-      - uses: actions/checkout@v2
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+          cache: pip
+          cache-dependency-path: dev-requirements.txt
+
       - name: Install pypa/build
         run: python -m pip install build
+
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/
+
       - name: Publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@v1.3.0
+        uses: pypa/gh-action-pypi-publish@v1.8.8
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `podmanclispawner-0.1.0/.gitignore` & `podmanclispawner-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `podmanclispawner-0.1.0/LICENSE` & `podmanclispawner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podmanclispawner-0.1.0/PKG-INFO` & `podmanclispawner-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: podmanclispawner
-Version: 0.1.0
+Version: 0.2.0
 Summary: PodmanCLISpawner for JupyterHub
 Home-page: https://github.com/manics/podmanspawner
 Author: Simon Li, Niklas Netter
 License: BSD
-Project-URL: Documentation, https://jupyterhub.readthedocs.io
-Project-URL: Source, https://github.com/manics/podmanspawner
-Project-URL: Tracker, https://github.com/manics/podmanspawner/issues
+Project-URL: Source, https://github.com/manics/podmanclispawner
+Project-URL: Tracker, https://github.com/manics/podmanclispawner/issues
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -47,9 +46,7 @@
     pip install git+https://github.com/manics/podmanclispawner
 
 ## JupyterHub configuration
 
 ```python
 c.JupyterHub.spawner_class = 'podmancli'
 ```
-
-
```

### Comparing `podmanclispawner-0.1.0/README.md` & `podmanclispawner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `podmanclispawner-0.1.0/podmanclispawner/podmanspawner.py` & `podmanclispawner-0.2.0/podmanclispawner/podmanspawner.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 class PodmanCLISpawner(Spawner):
     """
     A Spawner that uses `subprocess.Popen` to start single-user servers as
     podman containers.
     Does not work on Windows.
     """
 
+    ip = Unicode(
+        "0.0.0.0", help="The IP address the single-user server should listen on"
+    ).tag(config=True)
+
     popen_kwargs = Dict(
         help="""Extra keyword arguments to pass to Popen
         when spawning single-user servers.
         For example::
             popen_kwargs = dict(shell=True)
         """
     ).tag(config=True)
@@ -103,16 +107,16 @@
         Local processes only need the process id.
         """
         super().load_state(state)
         if "cid" in state:
             self.cid = state["cid"]
 
     def get_state(self):
-        """Save state that is needed to restore this spawner instance after a hub restore.
-        Local processes only need the process id.
+        """Save state that is needed to restore this spawner instance after a hub
+        restore. Local processes only need the process id.
         """
         state = super().get_state()
         if self.cid:
             state["cid"] = self.cid
         return state
 
     def clear_state(self):
```

### Comparing `podmanclispawner-0.1.0/podmanclispawner.egg-info/PKG-INFO` & `podmanclispawner-0.2.0/podmanclispawner.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: podmanclispawner
-Version: 0.1.0
+Version: 0.2.0
 Summary: PodmanCLISpawner for JupyterHub
 Home-page: https://github.com/manics/podmanspawner
 Author: Simon Li, Niklas Netter
 License: BSD
-Project-URL: Documentation, https://jupyterhub.readthedocs.io
-Project-URL: Source, https://github.com/manics/podmanspawner
-Project-URL: Tracker, https://github.com/manics/podmanspawner/issues
+Project-URL: Source, https://github.com/manics/podmanclispawner
+Project-URL: Tracker, https://github.com/manics/podmanclispawner/issues
 Platform: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -47,9 +46,7 @@
     pip install git+https://github.com/manics/podmanclispawner
 
 ## JupyterHub configuration
 
 ```python
 c.JupyterHub.spawner_class = 'podmancli'
 ```
-
-
```

### Comparing `podmanclispawner-0.1.0/setup.py` & `podmanclispawner-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,16 @@
         "Intended Audience :: System Administrators",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     project_urls={
-        "Documentation": "https://jupyterhub.readthedocs.io",
-        "Source": "https://github.com/manics/podmanspawner",
-        "Tracker": "https://github.com/manics/podmanspawner/issues",
+        "Source": "https://github.com/manics/podmanclispawner",
+        "Tracker": "https://github.com/manics/podmanclispawner/issues",
     },
     platforms="Linux",
     python_requires=">=3.6",
     setup_requires=["setuptools_scm"],
     install_requires=["jupyterhub", "traitlets>=4.3.2"],
     entry_points={
         "jupyterhub.spawners": [
```

### Comparing `podmanclispawner-0.1.0/tests/conftest.py` & `podmanclispawner-0.2.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ pytest config for ansiblespawner tests """
 # https://github.com/jupyterhub/yarnspawner/blob/0.4.0/yarnspawner/tests/conftest.py
-import pytest
+import pytest_asyncio
 
 from jupyterhub.tests.mocking import MockHub
 import os
 import socket
 import sys
 from traitlets.config import Config
 
@@ -23,15 +23,15 @@
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
         # doesn't even have to be reachable
         s.connect(("10.255.255.255", 1))
         return s.getsockname()[0]
 
 
 # https://docs.pytest.org/en/latest/example/parametrize.html#apply-indirect-on-particular-arguments
-@pytest.fixture
+@pytest_asyncio.fixture()
 async def app(request):
     """
     Mock a jupyterhub app for testing
 
     Takes a parameter indicating the name of the directory under examples
     """
```

### Comparing `podmanclispawner-0.1.0/tests/test_spawner.py` & `podmanclispawner-0.2.0/tests/test_spawner.py`

 * *Files identical despite different names*

