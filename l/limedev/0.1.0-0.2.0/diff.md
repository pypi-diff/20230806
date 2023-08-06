# Comparing `tmp/limedev-0.1.0.tar.gz` & `tmp/limedev-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limedev-0.1.0.tar", last modified: Sat May 13 20:20:40 2023, max compression
+gzip compressed data, was "limedev-0.2.0.tar", last modified: Sun Aug  6 18:43:15 2023, max compression
```

## Comparing `limedev-0.1.0.tar` & `limedev-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:20:40.016701 limedev-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 20:20:08.000000 limedev-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-13 20:20:40.016701 limedev-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-13 20:20:08.000000 limedev-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:20:40.016701 limedev-0.1.0/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-13 20:20:08.000000 limedev-0.1.0/dependencies/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-13 20:20:08.000000 limedev-0.1.0/dependencies/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-13 20:20:08.000000 limedev-0.1.0/dependencies/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-13 20:20:32.000000 limedev-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 20:20:40.016701 limedev-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:20:40.016701 limedev-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:20:40.016701 limedev-0.1.0/src/limedev/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-13 20:20:08.000000 limedev-0.1.0/src/limedev/_API.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-13 20:20:08.000000 limedev-0.1.0/src/limedev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-13 20:20:08.000000 limedev-0.1.0/src/limedev/_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-13 20:20:08.000000 limedev-0.1.0/src/limedev/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-13 20:20:08.000000 limedev-0.1.0/src/limedev/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 20:20:40.016701 limedev-0.1.0/src/limedev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-13 20:20:40.000000 limedev-0.1.0/src/limedev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-06 18:42:57.000000 limedev-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-06 18:43:15.594129 limedev-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-06 18:43:08.000000 limedev-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/_main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/package.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-06 18:42:57.000000 limedev-0.2.0/dependencies/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-06 18:43:08.000000 limedev-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:43:15.594129 limedev-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.590129 limedev-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/src/limedev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-08-06 18:42:57.000000 limedev-0.2.0/src/limedev/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:43:15.594129 limedev-0.2.0/src/limedev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 18:43:15.000000 limedev-0.2.0/src/limedev.egg-info/top_level.txt
```

### Comparing `limedev-0.1.0/LICENSE` & `limedev-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `limedev-0.1.0/PKG-INFO` & `limedev-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limedev
-Version: 0.1.0
+Version: 0.2.0
 Summary: Toolkit for Python development, especially packaging 
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/limedev
 Project-URL: Changelog, https://github.com/Limespy/limedev/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/limedev/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
+Provides-Extra: package
+Provides-Extra: readme
+Provides-Extra: test
 License-File: LICENSE
 
 [![PyPI Package latest release](https://img.shields.io/pypi/v/limedev.svg)][1]
 [![PyPI Wheel](https://img.shields.io/pypi/wheel/limedev.svg)][1]
 [![Supported versions](https://img.shields.io/pypi/pyversions/limedev.svg)][1]
 [![Supported implementations](https://img.shields.io/pypi/implementation/limedev.svg)][1]
 
@@ -58,12 +61,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
-## 0.1.0 2023-05-13 <!-- omit in toc -->
+## 0.2.0 2023-08-06 <!-- omit in toc -->
+
+- Bugfixes
+- Cleaner structure
+- Reworked readme build
+
+## 0.1.0 2023-05-04 <!-- omit in toc -->
 
 - Initial assembly of the tools
 
 [1]: <https://pypi.org/project/limedev> "Project PyPI page"
```

### Comparing `limedev-0.1.0/README.md` & `limedev-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,12 +34,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
-## 0.1.0 2023-05-13 <!-- omit in toc -->
+## 0.2.0 2023-08-06 <!-- omit in toc -->
+
+- Bugfixes
+- Cleaner structure
+- Reworked readme build
+
+## 0.1.0 2023-05-04 <!-- omit in toc -->
 
 - Initial assembly of the tools
 
 [1]: <https://pypi.org/project/limedev> "Project PyPI page"
```

### Comparing `limedev-0.1.0/pyproject.toml` & `limedev-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -20,32 +20,42 @@
     "Programming Language :: Python :: 3.11",
 ]
 authors = [
     { name = "Limespy" },
 ]
 requires-python = ">=3.9"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 dynamic = [
     "dependencies",
     "optional-dependencies",
 ]
 
 [project.scripts]
 package = "limedev.package:main"
 test = "limedev.test:main"
+readme = "limedev.readme:main"
 
 [project.urls]
 Homepage = "https://github.com/Limespy/limedev"
 Changelog = "https://github.com/Limespy/limedev/blob/main/README.md#Changelog"
 "Issue Tracker" = "https://github.com/Limespy/limedev/issues"
 
 [tool.setuptools.dynamic.dependencies]
 file = [
-    "dependencies/main.txt",
+    "dependencies/_main.txt",
 ]
 
 [tool.setuptools.dynamic.optional-dependencies.dev]
 file = "dependencies/dev.txt"
 
 [tool.setuptools.dynamic.optional-dependencies.build]
 file = "dependencies/build.txt"
+
+[tool.setuptools.dynamic.optional-dependencies.package]
+file = "dependencies/package.txt"
+
+[tool.setuptools.dynamic.optional-dependencies.readme]
+file = "dependencies/readme.txt"
+
+[tool.setuptools.dynamic.optional-dependencies.test]
+file = "dependencies/test.txt"
```

### Comparing `limedev-0.1.0/src/limedev/package.py` & `limedev-0.2.0/src/limedev/package.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 #!/usr/bin/env python
 # type: ignore
+'''Updating the pyproject.toml metadata and packaging into wheel and
+source distributions'''
 #%%═════════════════════════════════════════════════════════════════════
 # IMPORT
-import pathlib
 import re
 import sys
 import time
 
 import tomli_w
 from build import __main__ as build
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
-def main(args = sys.argv[1:]):
-    path_cwd = pathlib.Path.cwd()
-    try:
-        path_pyproject = next(path_cwd.rglob('pyproject.toml'))
-    except StopIteration:
-        print(f'Tests not found under {path_cwd}')
-
-    path_base = path_pyproject.parent
-    path_readme = path_base / 'readme.md'
-
-    sys.path.insert(1, str(path_base))
-    if (path_base_str := str(path_base)) not in sys.path[:3]:
-        sys.path.insert(1, path_base_str)
-    import readme
+from ._aux import _import_from_path
+from ._aux import _upsearch
+from ._aux import PATH_BASE
+
+def main(args = sys.argv[1:]) -> None: # pylint: disable=dangerous-default-value
+    '''Command line interface entry point. Builds README and the package'''
+    if (path_pyproject := _upsearch('pyproject.toml')) is None:
+        raise FileNotFoundError('pyproject.toml not found')
+
+    path_readme = PATH_BASE / 'README.md'
     #%%═════════════════════════════════════════════════════════════════════
     # BUILD INFO
 
     # Loading the pyproject TOML file
     pyproject = tomllib.loads(path_pyproject.read_text())
     project_info = pyproject['project']
-    path_package_init = next((path_base / 'src').rglob('__init__.py'))
     version = re.search(r"(?<=__version__ = ').*(?=')",
-                        path_package_init.read_text())[0]
+                        next((PATH_BASE / 'src').rglob('__init__.py')
+                             ).read_text())[0]
 
     if '--build-number' in args:
         version += f'.{time.time():.0f}'
 
     project_info['version'] = version
     #───────────────────────────────────────────────────────────────────────
     # URL
     source_url = project_info['urls'].get('Source Code',
                                           project_info['urls']['Homepage'])
     if source_url.startswith('https://github.com'):
         source_main_url = source_url + '/blob/main/'
     #───────────────────────────────────────────────────────────────────────
     # Long Description
-    readme_text = str(readme.make(project_info)) + '\n'
+    user_readme  = _import_from_path(PATH_BASE / 'readme' / 'readme.py').main
+    readme_text = str(user_readme(project_info)) + '\n'
     readme_text_pypi = readme_text.replace('./', source_main_url)
     #%%═════════════════════════════════════════════════════════════════════
     # RUNNING THE BUILD
 
     pyproject['project'] = project_info
     path_pyproject.write_text(tomli_w.dumps(pyproject))
 
-    for path in (path_base / 'dist').glob('*'):
+    for path in (PATH_BASE / 'dist').glob('*'):
         path.unlink()
 
     path_readme.write_text(readme_text_pypi)
 
-    if not '--no-build' in args:
+    if '--no-build' not in args:
         build.main([])
 
     path_readme.write_text(readme_text)
 #=======================================================================
 if __name__ =='__main__':
     raise SystemExit(main())
```

### Comparing `limedev-0.1.0/src/limedev/test.py` & `limedev-0.2.0/src/limedev/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,113 @@
-#%%═════════════════════════════════════════════════════════════════════
+'''Test invokers'''
+#%%=====================================================================
 # IMPORT
 import os
 import pathlib
 import sys
-from importlib import import_module
 from typing import Callable
-from typing import NoReturn
 from typing import Optional
-from typing import Union
 
-PATH_CONFIG = pathlib.Path(__file__).parent / 'config'
-#%%═════════════════════════════════════════════════════════════════════
+import yaml # type: ignore
+
+from ._aux import _import_from_path
+from ._aux import _upsearch
+
+PATH_CONFIGS = pathlib.Path(__file__).parent / 'configs'
+TEST_FOLDER_NAME = 'tests'
+#%%=====================================================================
 # TEST CASES
 
-#══════════════════════════════════════════════════════════════════════════════
+#%%=====================================================================
+def _get_path_config(patterns, path_start):
+    '''Loads test configuration file paths or supplies default if not found'''
+    return (PATH_CONFIGS / patterns[0]
+            if (path_local := _upsearch(patterns, path_start)) is None
+            else path_local)
+#==============================================================================
 def unittests(path_tests: pathlib.Path) -> None:
-    import pytest
+    '''Starts pytest unit tests'''
+    import pytest # pylint: disable=import-outside-toplevel
     CWD = pathlib.Path.cwd()
     os.chdir(str(path_tests / 'unittests'))
     pytest.main(["--cov=numba_integrators", "--cov-report=html"])
     os.chdir(str(CWD))
-    return None
-#══════════════════════════════════════════════════════════════════════════════
+#==============================================================================
 def typing(path_tests: pathlib.Path) -> Optional[tuple[str, str, int]]:
-    path_mypy_config = (path_local
-                        if (path_local := (path_tests / 'mypy.ini')).exists()
-                        else PATH_CONFIG / 'mypy.ini')
+    '''Starts mypy typing tests'''
     args = [str(path_tests.parent / 'src'),
             '--config-file',
-            str(path_mypy_config)]
-    from mypy.main import main
-    main(args = args)
-#══════════════════════════════════════════════════════════════════════════════
+            str(_get_path_config(('mypy.ini',), path_tests))]
+    from mypy.main import main as mypy # pylint: disable=import-outside-toplevel
+    mypy(args = args)
+#==============================================================================
 def lint(path_tests: pathlib.Path) -> None:
-    from pylint import lint
-    lint.Run([str(path_tests.parent / 'src'),
-              f'--rcfile={str(PATH_CONFIG / ".pylintrc")}',
-              '--output-format=colorized',
-              '--msg-template="{path}:{line}:{column}:{msg_id}:{symbol}\n'
+    '''Starts pylin linter'''
+    from pylint import lint as linter # type: ignore # pylint: disable=import-outside-toplevel
+    linter.Run([str(path_tests.parent / 'src'),
+                f'--rcfile={str(_get_path_config((".pylintrc",), path_tests))}',
+                '--output-format=colorized',
+                '--msg-template="{path}:{line}:{column}:{msg_id}:{symbol}\n'
                               '    {msg}"'])
-#═══════════════════════════════════════════════════════════════════════
-def profile(path_tests: pathlib.Path):
-    import subprocess
-
-    import cProfile
-    import gprof2dot
+#=======================================================================
+def profiling(path_tests: pathlib.Path) -> None:
+    '''Runs profiling and converts results into a PDF'''
+    import cProfile # pylint: disable=import-outside-toplevel
+    import gprof2dot # type: ignore # pylint: disable=import-outside-toplevel
+    import subprocess # pylint: disable=import-outside-toplevel
 
-    from profile import main as profile_run # type: ignore
+    profile_run = _import_from_path(path_tests / 'profiling.py').main
 
     path_profile = path_tests / 'profile'
     path_pstats = path_profile.with_suffix('.pstats')
     path_dot = path_profile.with_suffix('.dot')
     path_pdf = path_profile.with_suffix('.pdf')
 
-    profile_run()
+    profile_run() # Prep to eliminate first run overhead
     with cProfile.Profile() as pr:
         profile_run()
         pr.dump_stats(path_pstats)
 
     gprof2dot.main(['-f', 'pstats', str(path_pstats), '-o', path_dot])
     path_pstats.unlink()
     try:
         subprocess.run(['dot', '-Tpdf', str(path_dot), '-o', str(path_pdf)])
-    except FileNotFoundError:
-        raise RuntimeError('Conversion to PDF failed, maybe graphviz dot program is not installed. http://www.graphviz.org/download/')
+    except FileNotFoundError as exc:
+        raise RuntimeError('Conversion to PDF failed, maybe graphviz dot'
+                           ' program is not installed.'
+                           ' See http://www.graphviz.org/download/') from exc
     path_dot.unlink()
-#══════════════════════════════════════════════════════════════════════════════
+#==============================================================================
+def performance(path_tests: pathlib.Path) -> None:
+    '''Runs performance tests and save sresults into YAML file'''
+    performance_tests = _import_from_path(path_tests / 'performance.py').main
+    path_performance_data = path_tests / 'performance.yaml'
+    version, results = performance_tests()
+    with open(path_performance_data, encoding = 'utf8', mode = 'w+') as f:
+        if (data := yaml.safe_load(f)) is None:
+            data = {}
+        f.seek(0)
+        data[version] = results
+        f.write(yaml.safe_dump(data))
+        f.truncate()
+#==============================================================================
 TESTS: dict[str, Callable] = {function.__name__: function # type: ignore
                               for function in
-                              (lint, unittests, typing, profile)}
-def main(args: list[str] = sys.argv[1:]) -> Union[list, None, NoReturn]:
-    path_cwd = pathlib.Path.cwd()
-    try:
-        path_tests = next(path_cwd.rglob('tests'))
-    except StopIteration:
-        print(f'Tests not found under {path_cwd}')
-
-    sys.path.insert(1, str(path_tests))
+                              (lint, unittests, typing, profiling, performance)}
+def main(args: list[str] = sys.argv[1:]) -> int: # pylint: disable=dangerous-default-value
+    '''Command line interface entry point'''
+    if (path_tests := _upsearch(TEST_FOLDER_NAME)) is None:
+        raise FileNotFoundError('Tests not found')
 
     if not args:
-        return None
+        return 0
     for arg in args:
         if arg.startswith('--'):
             name = arg[2:]
             if (function := TESTS.get(name)) is None:
-                module = import_module(name)
-                module.main()
+                _import_from_path(path_tests / f'{name}.py').main()
             else:
                 function(path_tests)
-    return None
-#══════════════════════════════════════════════════════════════════════════════
+    return 0
+#==============================================================================
 if __name__ == '__main__':
     raise SystemExit(main())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `limedev-0.1.0/src/limedev.egg-info/PKG-INFO` & `limedev-0.2.0/src/limedev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limedev
-Version: 0.1.0
+Version: 0.2.0
 Summary: Toolkit for Python development, especially packaging 
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/limedev
 Project-URL: Changelog, https://github.com/Limespy/limedev/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/limedev/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: build
+Provides-Extra: package
+Provides-Extra: readme
+Provides-Extra: test
 License-File: LICENSE
 
 [![PyPI Package latest release](https://img.shields.io/pypi/v/limedev.svg)][1]
 [![PyPI Wheel](https://img.shields.io/pypi/wheel/limedev.svg)][1]
 [![Supported versions](https://img.shields.io/pypi/pyversions/limedev.svg)][1]
 [![Supported implementations](https://img.shields.io/pypi/implementation/limedev.svg)][1]
 
@@ -58,12 +61,18 @@
 
 ```python
 import limedev
 ```
 
 # Changelog <!-- omit in toc -->
 
-## 0.1.0 2023-05-13 <!-- omit in toc -->
+## 0.2.0 2023-08-06 <!-- omit in toc -->
+
+- Bugfixes
+- Cleaner structure
+- Reworked readme build
+
+## 0.1.0 2023-05-04 <!-- omit in toc -->
 
 - Initial assembly of the tools
 
 [1]: <https://pypi.org/project/limedev> "Project PyPI page"
```

