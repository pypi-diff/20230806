# Comparing `tmp/json-ref-dict-0.7.1.tar.gz` & `tmp/json-ref-dict-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-ref-dict-0.7.1.tar", last modified: Fri Sep 10 09:54:08 2021, max compression
+gzip compressed data, was "json-ref-dict-0.7.2.tar", last modified: Sun Aug  6 10:14:00 2023, max compression
```

## Comparing `json-ref-dict-0.7.1.tar` & `json-ref-dict-0.7.2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/
--rw-rw-r--   0 jack      (1000) jack      (1000)       14 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/top_level.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)      464 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/SOURCES.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)       17 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/requires.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     4177 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)        1 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict.egg-info/dependency_links.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     1063 2020-10-29 18:55:08.000000 json-ref-dict-0.7.1/LICENSE.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)     5816 2021-09-10 09:53:45.000000 json-ref-dict-0.7.1/CHANGELOG.md
--rw-rw-r--   0 jack      (1000) jack      (1000)       79 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/setup.cfg
--rw-rw-r--   0 jack      (1000) jack      (1000)     3718 2020-10-29 18:55:08.000000 json-ref-dict-0.7.1/README.md
--rw-rw-r--   0 jack      (1000) jack      (1000)     1458 2021-04-01 09:29:33.000000 json-ref-dict-0.7.1/setup.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4177 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)       17 2021-04-01 09:30:40.000000 json-ref-dict-0.7.1/requirements.txt
--rw-rw-r--   0 jack      (1000) jack      (1000)      209 2020-10-29 18:55:08.000000 json-ref-dict-0.7.1/pyproject.toml
--rw-rw-r--   0 jack      (1000) jack      (1000)       38 2020-10-29 18:55:08.000000 json-ref-dict-0.7.1/MANIFEST.in
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-09-10 09:54:08.000000 json-ref-dict-0.7.1/json_ref_dict/
--rw-rw-r--   0 jack      (1000) jack      (1000)      260 2020-10-29 18:55:08.000000 json-ref-dict-0.7.1/json_ref_dict/exceptions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5560 2021-09-08 15:26:09.000000 json-ref-dict-0.7.1/json_ref_dict/materialize.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3526 2021-04-01 09:29:33.000000 json-ref-dict-0.7.1/json_ref_dict/uri.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     7292 2021-09-10 09:51:44.000000 json-ref-dict-0.7.1/json_ref_dict/ref_pointer.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4658 2021-09-08 15:26:09.000000 json-ref-dict-0.7.1/json_ref_dict/loader.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3051 2021-09-10 09:51:44.000000 json-ref-dict-0.7.1/json_ref_dict/ref_dict.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      601 2021-09-10 09:53:45.000000 json-ref-dict-0.7.1/json_ref_dict/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5956 2023-08-06 10:13:32.000000 json-ref-dict-0.7.2/CHANGELOG.md
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1063 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/LICENSE.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/MANIFEST.in
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4153 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3718 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/json_ref_dict/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      601 2023-08-06 10:13:32.000000 json-ref-dict-0.7.2/json_ref_dict/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      260 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/exceptions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4658 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/loader.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5560 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/materialize.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3051 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/ref_dict.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7292 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/ref_pointer.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3526 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/json_ref_dict/uri.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/json_ref_dict.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4153 2023-08-06 10:14:00.000000 json-ref-dict-0.7.2/json_ref_dict.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      596 2023-08-06 10:14:00.000000 json-ref-dict-0.7.2/json_ref_dict.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-08-06 10:14:00.000000 json-ref-dict-0.7.2/json_ref_dict.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       17 2023-08-06 10:14:00.000000 json-ref-dict-0.7.2/json_ref_dict.egg-info/requires.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       14 2023-08-06 10:14:00.000000 json-ref-dict-0.7.2/json_ref_dict.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)      209 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/pyproject.toml
+-rw-rw-r--   0 jack      (1000) jack      (1000)       17 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/requirements.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       79 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1477 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/setup.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-08-06 10:14:00.744392 json-ref-dict-0.7.2/tests/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    14401 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_dict.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      566 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_lib.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4797 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_loader.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5112 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_materialize.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      310 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_readme_snippets.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      707 2023-08-06 10:04:15.000000 json-ref-dict-0.7.2/tests/test_uri.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `json-ref-dict-0.7.1/json_ref_dict.egg-info/PKG-INFO` & `json-ref-dict-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: json-ref-dict
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python dict-like object which abstracts resolution of JSONSchema references
 Home-page: https://github.com/jacksmith15/json-ref-dict
 Author: Jack Smith
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Build Status](https://travis-ci.com/jacksmith15/json-ref-dict.svg?branch=master)](https://travis-ci.com/jacksmith15/json-ref-dict)
@@ -113,9 +112,7 @@
 - [PyLint](https://www.pylint.org/) - for enforcing code style.
 - [MyPy](http://mypy-lang.org/) - for static type checking.
 - [Travis CI](https://travis-ci.org/) - for continuous integration.
 - [Black](https://black.readthedocs.io/en/stable/) - for uniform code formatting.
 
 # License
 This project is distributed under the MIT license.
-
-
```

### Comparing `json-ref-dict-0.7.1/LICENSE.txt` & `json-ref-dict-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/CHANGELOG.md` & `json-ref-dict-0.7.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 * **Added** for new features.
 * **Changed** for changes in existing functionality.
 * **Removed** for now removed features.
 * **Fixed** for any bug fixes.
 
 ## [Unreleased]
 
+## [0.7.2] - 2023-08-06
+
+### Fixed
+* Added license to `setup.py`
+
 ## [0.7.1] - 2021-09-10
 
 ### Fixed
 * Fixed recursive references pointing to remote documents.
   References with ref_pointer can recurse to new remote
   documents. ref_dict URIs need to be updated to point
   to remote documents for the relative URI resolving to
@@ -140,15 +145,16 @@
   references.
 * Added general document loading by URI (deferring to
   `urllib.request.urlopen`).
 
 ## [0.0.0]
 Nothing here.
 
-[Unreleased]: http://github.com/jacksmith15/json-ref-dict/compare/0.7.1..HEAD
+[Unreleased]: http://github.com/jacksmith15/json-ref-dict/compare/0.7.2..HEAD
+[0.7.2]: http://github.com/jacksmith15/json-ref-dict/compare/0.7.1..0.7.2
 [0.7.1]: http://github.com/jacksmith15/json-ref-dict/compare/0.7.0..0.7.1
 [0.7.0]: http://github.com/jacksmith15/json-ref-dict/compare/0.6.2..0.7.0
 [0.6.2]: http://github.com/jacksmith15/json-ref-dict/compare/0.6.1..0.6.2
 [0.6.1]: http://github.com/jacksmith15/json-ref-dict/compare/0.6.0..0.6.1
 [0.6.0]: http://github.com/jacksmith15/json-ref-dict/compare/0.5.3..0.6.0
 [0.5.3]: http://github.com/jacksmith15/json-ref-dict/compare/0.5.2..0.5.3
 [0.5.2]: http://github.com/jacksmith15/json-ref-dict/compare/0.5.1..0.5.2
```

### Comparing `json-ref-dict-0.7.1/README.md` & `json-ref-dict-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/setup.py` & `json-ref-dict-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,9 +45,10 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.6",
     ],
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
     install_requires=REQUIREMENTS_FILE,
+    license="MIT",
     dependency_links=[],
 )
```

### Comparing `json-ref-dict-0.7.1/PKG-INFO` & `json-ref-dict-0.7.2/json_ref_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: json-ref-dict
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python dict-like object which abstracts resolution of JSONSchema references
 Home-page: https://github.com/jacksmith15/json-ref-dict
 Author: Jack Smith
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Build Status](https://travis-ci.com/jacksmith15/json-ref-dict.svg?branch=master)](https://travis-ci.com/jacksmith15/json-ref-dict)
@@ -113,9 +112,7 @@
 - [PyLint](https://www.pylint.org/) - for enforcing code style.
 - [MyPy](http://mypy-lang.org/) - for static type checking.
 - [Travis CI](https://travis-ci.org/) - for continuous integration.
 - [Black](https://black.readthedocs.io/en/stable/) - for uniform code formatting.
 
 # License
 This project is distributed under the MIT license.
-
-
```

### Comparing `json-ref-dict-0.7.1/json_ref_dict/materialize.py` & `json-ref-dict-0.7.2/json_ref_dict/materialize.py`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/json_ref_dict/uri.py` & `json-ref-dict-0.7.2/json_ref_dict/uri.py`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/json_ref_dict/ref_pointer.py` & `json-ref-dict-0.7.2/json_ref_dict/ref_pointer.py`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/json_ref_dict/loader.py` & `json-ref-dict-0.7.2/json_ref_dict/loader.py`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/json_ref_dict/ref_dict.py` & `json-ref-dict-0.7.2/json_ref_dict/ref_dict.py`

 * *Files identical despite different names*

### Comparing `json-ref-dict-0.7.1/json_ref_dict/__init__.py` & `json-ref-dict-0.7.2/json_ref_dict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from json_ref_dict.exceptions import JSONRefParseError
 from json_ref_dict.materialize import materialize
 from json_ref_dict.ref_pointer import RefPointer, resolve_uri
 from json_ref_dict.ref_dict import RefDict
 from json_ref_dict.uri import URI
 
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
```

