# Comparing `tmp/conda-forge-metadata-0.5.1.tar.gz` & `tmp/conda-forge-metadata-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-forge-metadata-0.5.1.tar", last modified: Fri Aug  4 16:05:58 2023, max compression
+gzip compressed data, was "conda-forge-metadata-0.5.2.tar", last modified: Sun Aug  6 11:56:50 2023, max compression
```

## Comparing `conda-forge-metadata-0.5.1.tar` & `conda-forge-metadata-0.5.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.480323 conda-forge-metadata-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/info_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/import_to_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/conda_forge_metadata/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.484323 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 16:05:58.000000 conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:05:58.488323 conda-forge-metadata-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_feedstock_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_info_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_map_import_to_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-04 16:05:42.000000 conda-forge-metadata-0.5.1/tests/test_map_pypi_to_conda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.359967 conda-forge-metadata-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.363967 conda-forge-metadata-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.363967 conda-forge-metadata-0.5.2/conda_forge_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/conda_forge_metadata/artifact_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/artifact_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/artifact_info/info_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/import_to_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/pypi_to_conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/conda_forge_metadata/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-06 11:56:50.000000 conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 11:56:50.367967 conda-forge-metadata-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_info_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_map_import_to_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-06 11:56:32.000000 conda-forge-metadata-0.5.2/tests/test_map_pypi_to_conda.py
```

### Comparing `conda-forge-metadata-0.5.1/.github/workflows/pypi.yml` & `conda-forge-metadata-0.5.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/.github/workflows/tests.yml` & `conda-forge-metadata-0.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/.gitignore` & `conda-forge-metadata-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/.pre-commit-config.yaml` & `conda-forge-metadata-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/LICENSE` & `conda-forge-metadata-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/PKG-INFO` & `conda-forge-metadata-0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.5.1
+Version: 0.5.2
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
@@ -35,9 +35,10 @@
 Project-URL: home, https://github.com/regro/conda-forge-metadata
 Description-Content-Type: text/markdown
 Provides-Extra: oci
 License-File: LICENSE
 
 # conda-forge-metadata
 [![tests](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml)
+[![Publish to PyPI](https://github.com/regro/conda-forge-metadata/actions/workflows/pypi.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/pypi.yml)
 
 programatic access to conda-forge's metadata
```

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/artifact_info/info_json.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/artifact_info/info_json.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/import_to_pkg.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/import_to_pkg.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/autotick_bot/pypi_to_conda.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/feedstock_outputs.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/feedstock_outputs.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/libcfgraph.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/libcfgraph.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/oci.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/oci.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata/types.py` & `conda-forge-metadata-0.5.2/conda_forge_metadata/types.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/PKG-INFO` & `conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.5.1
+Version: 0.5.2
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
@@ -35,9 +35,10 @@
 Project-URL: home, https://github.com/regro/conda-forge-metadata
 Description-Content-Type: text/markdown
 Provides-Extra: oci
 License-File: LICENSE
 
 # conda-forge-metadata
 [![tests](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml)
+[![Publish to PyPI](https://github.com/regro/conda-forge-metadata/actions/workflows/pypi.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/pypi.yml)
 
 programatic access to conda-forge's metadata
```

### Comparing `conda-forge-metadata-0.5.1/conda_forge_metadata.egg-info/SOURCES.txt` & `conda-forge-metadata-0.5.2/conda_forge_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/pyproject.toml` & `conda-forge-metadata-0.5.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 authors = [
     {name = "conda-forge-tick development team", email = "condaforge@gmail.com"},
 ]
 description = "programatic access to conda-forge's metadata"
 dynamic = ["version"]
 dependencies = [
     "requests",
-    "ruamel.yaml"
+    "ruamel.yaml",
+    "typing-extensions"
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 
 [project.optional-dependencies]
 oci = [
   "conda-oci-mirror"
```

### Comparing `conda-forge-metadata-0.5.1/tests/test_info_json.py` & `conda-forge-metadata-0.5.2/tests/test_info_json.py`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.5.1/tests/test_libcfgraph.py` & `conda-forge-metadata-0.5.2/tests/test_libcfgraph.py`

 * *Files identical despite different names*

