# Comparing `tmp/webint_code-0.0.23.tar.gz` & `tmp/webint_code-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_code-0.0.23.tar", max compression
+gzip compressed data, was "webint_code-0.0.24.tar", max compression
```

## Comparing `webint_code-0.0.23.tar` & `webint_code-0.0.24.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1131 2023-07-30 01:57:25.106895 webint_code-0.0.23/pyproject.toml
--rw-r--r--   0        0        0    19176 2023-07-30 01:42:02.236213 webint_code-0.0.23/webint_code/__init__.py
--rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/__init__.py
--rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.23/webint_code/templates/index.html
--rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/commit.html
--rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/project/commit_log.html
--rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/created.html
--rw-r--r--   0        0        0    10118 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/index.html
--rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/issues.html
--rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/namespace.html
--rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.23/webint_code/templates/project/release.html
--rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/release_file.html
--rw-r--r--   0        0        0     1063 2023-05-20 02:42:12.401245 webint_code-0.0.23/webint_code/templates/project/repository_file.html
--rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.23/webint_code/templates/project/settings.html
--rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/projects.html
--rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/pypi/index.html
--rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/pypi/project.html
--rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.23/webint_code/templates/search/index.html
--rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.23/webint_code/templates/search/results.html
--rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.23/webint_code/templates/system.html
--rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.23/webint_code/templates/template.html
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.23/setup.py
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.23/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-08-06 02:22:34.954934 webint_code-0.0.24/pyproject.toml
+-rw-r--r--   0        0        0    19082 2023-08-06 02:19:19.947965 webint_code-0.0.24/webint_code/__init__.py
+-rw-r--r--   0        0        0      474 2023-01-27 00:43:27.567919 webint_code-0.0.24/webint_code/templates/__init__.py
+-rw-r--r--   0        0        0      161 2023-02-20 19:30:47.711101 webint_code-0.0.24/webint_code/templates/index.html
+-rw-r--r--   0        0        0     1225 2023-01-27 00:43:27.575919 webint_code-0.0.24/webint_code/templates/project/commit.html
+-rw-r--r--   0        0        0      651 2023-01-27 00:43:27.567919 webint_code-0.0.24/webint_code/templates/project/commit_log.html
+-rw-r--r--   0        0        0      116 2023-01-27 00:43:27.571919 webint_code-0.0.24/webint_code/templates/project/created.html
+-rw-r--r--   0        0        0    10187 2023-08-06 02:19:31.420139 webint_code-0.0.24/webint_code/templates/project/index.html
+-rw-r--r--   0        0        0      872 2023-01-27 00:43:27.575919 webint_code-0.0.24/webint_code/templates/project/issues.html
+-rw-r--r--   0        0        0     2921 2023-01-27 00:43:27.571919 webint_code-0.0.24/webint_code/templates/project/namespace.html
+-rw-r--r--   0        0        0      294 2023-01-27 00:43:27.571919 webint_code-0.0.24/webint_code/templates/project/release.html
+-rw-r--r--   0        0        0      777 2023-01-27 00:43:27.575919 webint_code-0.0.24/webint_code/templates/project/release_file.html
+-rw-r--r--   0        0        0     1063 2023-05-20 02:42:12.401245 webint_code-0.0.24/webint_code/templates/project/repository_file.html
+-rw-r--r--   0        0        0      485 2023-01-27 00:43:27.575919 webint_code-0.0.24/webint_code/templates/project/settings.html
+-rw-r--r--   0        0        0      373 2023-01-27 00:43:27.579919 webint_code-0.0.24/webint_code/templates/projects.html
+-rw-r--r--   0        0        0      136 2023-01-27 00:43:27.579919 webint_code-0.0.24/webint_code/templates/pypi/index.html
+-rw-r--r--   0        0        0      227 2023-01-27 00:43:27.579919 webint_code-0.0.24/webint_code/templates/pypi/project.html
+-rw-r--r--   0        0        0       87 2023-01-27 00:43:27.579919 webint_code-0.0.24/webint_code/templates/search/index.html
+-rw-r--r--   0        0        0     1029 2023-01-27 00:43:27.583919 webint_code-0.0.24/webint_code/templates/search/results.html
+-rw-r--r--   0        0        0     4967 2023-05-18 23:21:54.011448 webint_code-0.0.24/webint_code/templates/system.html
+-rw-r--r--   0        0        0      149 2023-01-27 00:43:27.567919 webint_code-0.0.24/webint_code/templates/template.html
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 webint_code-0.0.24/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 webint_code-0.0.24/PKG-INFO
```

### Comparing `webint_code-0.0.23/pyproject.toml` & `webint_code-0.0.24/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-code"
-version = "0.0.23"
+version = "0.0.24"
 description = "manage code on your website"
 keywords = ["webint", "Git", "PyPI"]
 homepage = "https://ragt.ag/code/projects/webint-code"
 repository = "https://ragt.ag/code/projects/webint-code.git"
 documentation = "https://ragt.ag/code/projects/webint-code/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
@@ -17,22 +17,22 @@
 python = ">=3.10,<3.11"
 pygments = "^2.14.0"
 webint = ">=0.0"
 webagt = ">=0.0"
 gmpg = ">=0.0"
 bgq = ">=0.0"
 
-[tool.poetry.group.dev.dependencies]
-gmpg = {path="../gmpg", develop=true}
-bgq = {path="../bgq", develop=true}
-webint = {path="../webint", develop=true}
-webagt = {path="../webagt", develop=true}
-newmath = {path="../newmath", develop=true}
-sqlyte = {path="../sqlyte", develop=true}
-microformats = {path="../python-microformats", develop=true}
+# [tool.poetry.group.dev.dependencies]
+# gmpg = {path="../gmpg", develop=true}
+# bgq = {path="../bgq", develop=true}
+# webint = {path="../webint", develop=true}
+# webagt = {path="../webagt", develop=true}
+# newmath = {path="../newmath", develop=true}
+# sqlyte = {path="../sqlyte", develop=true}
+# microformats = {path="../python-microformats", develop=true}
 
 # [[tool.poetry.source]]
 # name = "main"
 # url = "https://ragt.ag/code/pypi"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `webint_code-0.0.23/webint_code/__init__.py` & `webint_code-0.0.24/webint_code/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [0]: https://www.python.org/dev/peps/pep-0503/
 
 """
 
 # TODO PEP 592 -- Adding "Yank" Support to the Simple API
 # TODO PEP 658 -- Serve Distribution Metadata in the Simple Repository API
 
+import os
 import pathlib
 import re
 import shutil
 import subprocess
 import time
 
 import gmpg
@@ -80,32 +81,28 @@
     Execute tests.
 
     """
     project_dir = meta_dir / project
     testing_dir = project_dir / "testing"
     shutil.rmtree(testing_dir, ignore_errors=True)
     gmpg.clone_repo(project_dir / "source.git", testing_dir)
-    time.sleep(5)
-    gmpg.strip_local_dev_deps(testing_dir)
-
-    def run_poetry(*command, capture_output=False):
-        return subprocess.run(
-            ["/home/admin/.local/bin/poetry", *command],
+    admin_home = "/home/admin"
+    env = os.environ.copy()
+    env["HOME"] = admin_home
+    print(
+        subprocess.run(
+            [f"{admin_home}/bin/act", "--artifact-server-path", "artifacts"],
             cwd=testing_dir,
-            capture_output=capture_output,
+            env=env,
         )
-
-    print(run_poetry("install"))
-    print("installation complete")
-    run_poetry("run", "gmpg", "test")
-    print("testing complete")
-    run_poetry("run", "gmpg", "analyze")
-    print("API analysis complete")
-    run_poetry("run", "gmpg", "graph")
-    print("dependency visualization complete")
+    )
+    for artifact in (testing_dir / "artifacts/1/analysis").iterdir():
+        shortened = artifact.name[:-2]
+        artifact.rename(testing_dir / shortened)
+        subprocess.run(["gunzip", shortened], cwd=testing_dir)
 
 
 @app.query
 def search(db, query):
     """Search for `query` in commited code."""
     files = {}
     context = "2"
@@ -338,20 +335,20 @@
             pyproject = None
         testing_dir = project_dir / "testing"
         try:
             api_python = web.load(path=testing_dir / "api_python.json")
         except FileNotFoundError:
             api_python = {}
         try:
-            test_results = gmpg.analysis._parse_junit(testing_dir / ".test_results.xml")
+            test_results = gmpg.analysis._parse_junit(testing_dir / "test_results.xml")
         except FileNotFoundError:
             test_results = {}
         try:
             test_coverage = gmpg.analysis._parse_coverage(
-                testing_dir / ".test_coverage.xml"
+                testing_dir / "test_coverage.xml"
             )
         except FileNotFoundError:
             test_coverage = {}
         return app.view.project.index(
             project,
             gmpg.get_repo(project_dir / "working"),
             readme,
@@ -383,15 +380,15 @@
 
 @app.control("projects/{project}/api/{namespace}.svg")
 class ProjectAPIDeps:
     """Project's API in JSON."""
 
     def get(self, project, namespace):
         """Return the API's JSON."""
-        return meta_dir / project / "testing" / f"{namespace}.svg"
+        return meta_dir / project / "testing" / f"deps.svg"
 
 
 @app.control("projects/{project}/api/{namespace}")
 class ProjectAPINamespace:
     """Project's API namespace."""
 
     def get(self, project, namespace):
```

### Comparing `webint_code-0.0.23/webint_code/templates/project/commit.html` & `webint_code-0.0.24/webint_code/templates/project/commit.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/project/commit_log.html` & `webint_code-0.0.24/webint_code/templates/project/commit_log.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/project/index.html` & `webint_code-0.0.24/webint_code/templates/project/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             $if not loop.last:
                 ,
         </small>
     </p>
     $ license = py_project.pop("license")
     $ licenses = {"0BSD": "BSD Zero Clause License",
     $             "BSD-2-Clause": 'BSD 2-Clause "Simplified" License',
+    $             "BSD-3-Clause": 'BSD 3-Clause "Modified" License',
     $             "AGPL-3.0-or-later": "GNU Affero General Public License v3.0 or later"}
     <p><small><strong>Licensed:</strong> <a href=https://spdx.org/licenses/$(license).html><code>$licenses[license]</code></a></small></p>
     $ plugins = py_project.pop("plugins", None)
     $ scripts = py_project.pop("scripts", None)
     $if plugins or scripts:
         <p><small><strong>Provides:</strong></small>
     $if plugins:
```

#### html2text {}

```diff
@@ -22,16 +22,17 @@
 $comment_count comment$("s" if comment_count > 1 else "") $#
  $#
 $if pyproject: $ py_project = pyproject["tool"]["poetry"] $ title += f"&thinsp;
 {py_project.pop('version')}"
 $py_project.pop("description") $if keywords := py_project.pop("keywords",
 None): $for keyword in keywords: $keyword\ $if not loop.last: ,
 $ license = py_project.pop("license") $ licenses = {"0BSD": "BSD Zero Clause
-License", $ "BSD-2-Clause": 'BSD 2-Clause "Simplified" License', $ "AGPL-3.0-
-or-later": "GNU Affero General Public License v3.0 or later"}
+License", $ "BSD-2-Clause": 'BSD 2-Clause "Simplified" License', $ "BSD-3-
+Clause": 'BSD 3-Clause "Modified" License', $ "AGPL-3.0-or-later": "GNU Affero
+General Public License v3.0 or later"}
 Licensed: $licenses[license]
 $ plugins = py_project.pop("plugins", None) $ scripts = py_project.pop
 ("scripts", None) $if plugins or scripts:
 Provides: $if plugins: $if webapps := plugins.pop("webapps", None): webapps
 ( $for webapp, webapp_callable in webapps.items(): $ webapp_path =
 webapp_callable.replace(".", "/").replace(":", "#") $webapp\ $if not loop.last:
 , \ ) $if websites := plugins.pop("websites", None): websites ( $for webapp,
```

### Comparing `webint_code-0.0.23/webint_code/templates/project/issues.html` & `webint_code-0.0.24/webint_code/templates/project/issues.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/project/namespace.html` & `webint_code-0.0.24/webint_code/templates/project/namespace.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/project/release_file.html` & `webint_code-0.0.24/webint_code/templates/project/release_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/project/repository_file.html` & `webint_code-0.0.24/webint_code/templates/project/repository_file.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/search/results.html` & `webint_code-0.0.24/webint_code/templates/search/results.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/webint_code/templates/system.html` & `webint_code-0.0.24/webint_code/templates/system.html`

 * *Files identical despite different names*

### Comparing `webint_code-0.0.23/setup.py` & `webint_code-0.0.24/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['code = webint_code:app']}
 
 setup_kwargs = {
     'name': 'webint-code',
-    'version': '0.0.23',
+    'version': '0.0.24',
     'description': 'manage code on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-code',
```

### Comparing `webint_code-0.0.23/PKG-INFO` & `webint_code-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-code
-Version: 0.0.23
+Version: 0.0.24
 Summary: manage code on your website
 Home-page: https://ragt.ag/code/projects/webint-code
 License: BSD-2-Clause
 Keywords: webint,Git,PyPI
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

