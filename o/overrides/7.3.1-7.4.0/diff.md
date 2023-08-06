# Comparing `tmp/overrides-7.3.1.tar.gz` & `tmp/overrides-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overrides-7.3.1.tar", last modified: Mon Oct 17 20:35:03 2022, max compression
+gzip compressed data, was "overrides-7.4.0.tar", last modified: Sun Aug  6 13:46:06 2023, max compression
```

## Comparing `overrides-7.3.1.tar` & `overrides-7.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.154137 overrides-7.3.1/
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.147890 overrides-7.3.1/.github/
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.149917 overrides-7.3.1/.github/workflows/
--rw-r--r--   0 mkorpela   (501) staff       (20)      742 2022-10-17 20:27:21.000000 overrides-7.3.1/.github/workflows/ci.yml
--rw-r--r--   0 mkorpela   (501) staff       (20)      753 2022-10-03 15:31:58.000000 overrides-7.3.1/.gitignore
--rw-r--r--   0 mkorpela   (501) staff       (20)    11358 2022-10-03 15:31:58.000000 overrides-7.3.1/LICENSE
--rw-r--r--   0 mkorpela   (501) staff       (20)      113 2022-10-03 15:31:58.000000 overrides-7.3.1/MANIFEST.in
--rw-r--r--   0 mkorpela   (501) staff       (20)     7020 2022-10-17 20:35:03.154009 overrides-7.3.1/PKG-INFO
--rw-r--r--   0 mkorpela   (501) staff       (20)     5071 2022-10-17 20:27:21.000000 overrides-7.3.1/README.rst
--rwxr-xr-x   0 mkorpela   (501) staff       (20)      114 2022-10-03 15:31:58.000000 overrides-7.3.1/check_mypy.sh
--rw-r--r--   0 mkorpela   (501) staff       (20)      281 2022-10-03 15:31:58.000000 overrides-7.3.1/conftest.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.150213 overrides-7.3.1/mypy_fails/
--rw-r--r--   0 mkorpela   (501) staff       (20)      202 2022-10-15 20:20:46.000000 overrides-7.3.1/mypy_fails/wrong_signature.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      180 2022-10-15 20:20:46.000000 overrides-7.3.1/mypy_fails/wrong_signature_forward_ref.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.150362 overrides-7.3.1/mypy_passes/
--rw-r--r--   0 mkorpela   (501) staff       (20)      297 2022-10-15 20:20:46.000000 overrides-7.3.1/mypy_passes/passing_override.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.151391 overrides-7.3.1/overrides/
--rw-r--r--   0 mkorpela   (501) staff       (20)      333 2022-10-17 20:27:21.000000 overrides-7.3.1/overrides/__init__.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     2349 2022-10-15 20:20:46.000000 overrides-7.3.1/overrides/enforce.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     1511 2022-10-15 20:20:46.000000 overrides-7.3.1/overrides/final.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     7514 2022-10-17 20:33:29.000000 overrides-7.3.1/overrides/overrides.py
--rw-r--r--   0 mkorpela   (501) staff       (20)        0 2022-10-03 15:31:58.000000 overrides-7.3.1/overrides/py.typed
--rw-r--r--   0 mkorpela   (501) staff       (20)    11649 2022-10-10 15:47:10.000000 overrides-7.3.1/overrides/signature.py
--rw-r--r--   0 mkorpela   (501) staff       (20)    13930 2022-10-17 20:30:46.000000 overrides-7.3.1/overrides/typing_utils.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.152091 overrides-7.3.1/overrides.egg-info/
--rw-r--r--   0 mkorpela   (501) staff       (20)     7020 2022-10-17 20:35:03.000000 overrides-7.3.1/overrides.egg-info/PKG-INFO
--rw-r--r--   0 mkorpela   (501) staff       (20)      853 2022-10-17 20:35:03.000000 overrides-7.3.1/overrides.egg-info/SOURCES.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)        1 2022-10-17 20:35:03.000000 overrides-7.3.1/overrides.egg-info/dependency_links.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       34 2022-10-17 20:35:03.000000 overrides-7.3.1/overrides.egg-info/requires.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       10 2022-10-17 20:35:03.000000 overrides-7.3.1/overrides.egg-info/top_level.txt
--rwxr-xr-x   0 mkorpela   (501) staff       (20)       69 2022-10-10 15:47:10.000000 overrides-7.3.1/release.sh
--rw-r--r--   0 mkorpela   (501) staff       (20)       92 2022-10-03 15:31:58.000000 overrides-7.3.1/requirements-dev.txt
--rw-r--r--   0 mkorpela   (501) staff       (20)       38 2022-10-17 20:35:03.154186 overrides-7.3.1/setup.cfg
--rw-r--r--   0 mkorpela   (501) staff       (20)     1253 2022-10-17 20:33:37.000000 overrides-7.3.1/setup.py
-drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2022-10-17 20:35:03.153802 overrides-7.3.1/tests/
--rw-r--r--   0 mkorpela   (501) staff       (20)      554 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_decorator_params.py
--rw-r--r--   0 mkorpela   (501) staff       (20)    12846 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_enforce__py38.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     4161 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_final.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      398 2022-10-10 15:47:10.000000 overrides-7.3.1/tests/test_issubtype_with_typeddict__py38.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     2834 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_named_and_positional__py38.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     4564 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_overrides.py
--rw-r--r--   0 mkorpela   (501) staff       (20)     2450 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_signatures.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      211 2022-10-03 15:31:58.000000 overrides-7.3.1/tests/test_somefinalpackage.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      100 2022-10-03 15:31:58.000000 overrides-7.3.1/tests/test_somepackage.py
--rw-r--r--   0 mkorpela   (501) staff       (20)      961 2022-10-15 20:20:46.000000 overrides-7.3.1/tests/test_special_cases.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.218605 overrides-7.4.0/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.213080 overrides-7.4.0/.github/
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.214752 overrides-7.4.0/.github/workflows/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      728 2023-08-06 13:00:42.000000 overrides-7.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 mkorpela   (501) staff       (20)      753 2022-10-03 15:31:58.000000 overrides-7.4.0/.gitignore
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11358 2022-10-03 15:31:58.000000 overrides-7.4.0/LICENSE
+-rw-r--r--   0 mkorpela   (501) staff       (20)      113 2022-10-03 15:31:58.000000 overrides-7.4.0/MANIFEST.in
+-rw-r--r--   0 mkorpela   (501) staff       (20)     5689 2023-08-06 13:46:06.218496 overrides-7.4.0/PKG-INFO
+-rw-r--r--   0 mkorpela   (501) staff       (20)     5085 2023-07-11 10:37:33.000000 overrides-7.4.0/README.rst
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)      114 2022-10-03 15:31:58.000000 overrides-7.4.0/check_mypy.sh
+-rw-r--r--   0 mkorpela   (501) staff       (20)      281 2022-10-03 15:31:58.000000 overrides-7.4.0/conftest.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.215031 overrides-7.4.0/mypy_fails/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      202 2022-10-15 20:20:46.000000 overrides-7.4.0/mypy_fails/wrong_signature.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      180 2022-10-15 20:20:46.000000 overrides-7.4.0/mypy_fails/wrong_signature_forward_ref.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.215187 overrides-7.4.0/mypy_passes/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      297 2022-10-15 20:20:46.000000 overrides-7.4.0/mypy_passes/passing_override.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.216122 overrides-7.4.0/overrides/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      333 2022-10-17 20:27:21.000000 overrides-7.4.0/overrides/__init__.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2349 2022-10-15 20:20:46.000000 overrides-7.4.0/overrides/enforce.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1511 2022-10-15 20:20:46.000000 overrides-7.4.0/overrides/final.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     7514 2023-08-06 13:45:33.000000 overrides-7.4.0/overrides/overrides.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)        0 2022-10-03 15:31:58.000000 overrides-7.4.0/overrides/py.typed
+-rw-r--r--   0 mkorpela   (501) staff       (20)    11649 2023-07-11 19:46:54.000000 overrides-7.4.0/overrides/signature.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    14294 2023-08-06 13:42:46.000000 overrides-7.4.0/overrides/typing_utils.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.216824 overrides-7.4.0/overrides.egg-info/
+-rw-r--r--   0 mkorpela   (501) staff       (20)     5689 2023-08-06 13:46:06.000000 overrides-7.4.0/overrides.egg-info/PKG-INFO
+-rw-r--r--   0 mkorpela   (501) staff       (20)      885 2023-08-06 13:46:06.000000 overrides-7.4.0/overrides.egg-info/SOURCES.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)        1 2023-08-06 13:46:06.000000 overrides-7.4.0/overrides.egg-info/dependency_links.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       34 2023-08-06 13:46:06.000000 overrides-7.4.0/overrides.egg-info/requires.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       10 2023-08-06 13:46:06.000000 overrides-7.4.0/overrides.egg-info/top_level.txt
+-rwxr-xr-x   0 mkorpela   (501) staff       (20)       69 2022-10-10 15:47:10.000000 overrides-7.4.0/release.sh
+-rw-r--r--   0 mkorpela   (501) staff       (20)       92 2022-10-03 15:31:58.000000 overrides-7.4.0/requirements-dev.txt
+-rw-r--r--   0 mkorpela   (501) staff       (20)       38 2023-08-06 13:46:06.218648 overrides-7.4.0/setup.cfg
+-rw-r--r--   0 mkorpela   (501) staff       (20)     1253 2023-08-06 13:45:23.000000 overrides-7.4.0/setup.py
+drwxr-xr-x   0 mkorpela   (501) staff       (20)        0 2023-08-06 13:46:06.218322 overrides-7.4.0/tests/
+-rw-r--r--   0 mkorpela   (501) staff       (20)      554 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_decorator_params.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)    12846 2023-08-06 13:41:32.000000 overrides-7.4.0/tests/test_enforce__py38.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     4161 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_final.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      398 2022-10-10 15:47:10.000000 overrides-7.4.0/tests/test_issubtype_with_typeddict__py38.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2834 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_named_and_positional__py38.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      632 2023-08-06 13:37:41.000000 overrides-7.4.0/tests/test_new_union__py3_10.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     4564 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_overrides.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)     2450 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_signatures.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      211 2022-10-03 15:31:58.000000 overrides-7.4.0/tests/test_somefinalpackage.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      100 2022-10-03 15:31:58.000000 overrides-7.4.0/tests/test_somepackage.py
+-rw-r--r--   0 mkorpela   (501) staff       (20)      961 2022-10-15 20:20:46.000000 overrides-7.4.0/tests/test_special_cases.py
```

### Comparing `overrides-7.3.1/.github/workflows/ci.yml` & `overrides-7.4.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   pull_request:
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11.0-rc.2']
+        python: ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v2
       - name: Setup Python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python }}
@@ -23,10 +23,10 @@
          pip install -U pip
          pip install -r requirements-dev.txt
          pip install .
       - name: Run pytest
         run: pytest tests
       - name: Run mypy
         run:  mypy overrides
-      - name: Run mypy static tests (Python=3.10)
-        if: matrix.python == '3.10'
+      - name: Run mypy static tests (Python=3.11)
+        if: matrix.python == '3.11'
         run: ./check_mypy.sh
```

### Comparing `overrides-7.3.1/.gitignore` & `overrides-7.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/LICENSE` & `overrides-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/PKG-INFO` & `overrides-7.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: overrides
-Version: 7.3.1
+Version: 7.4.0
 Summary: A decorator to automatically detect mismatch when overriding a method.
 Home-page: https://github.com/mkorpela/overrides
 Author: Mikko Korpela
 Author-email: mikko.korpela@gmail.com
 License: Apache License, Version 2.0
-Description: overrides
-        =========
-        
-        .. image:: https://img.shields.io/pypi/v/overrides.svg
-          :target: https://pypi.python.org/pypi/overrides
-        
-        .. image:: http://pepy.tech/badge/overrides
-          :target: http://pepy.tech/project/overrides
-        
-        A decorator ``@override`` that verifies that a method that should override an inherited method actually does it.
-        
-        Copies the docstring of the inherited method to the overridden method.
-        
-        Since signature validation and docstring inheritance are performed on class creation and not on class instantiation,
-        this library significantly improves the safety and experience of creating class hierarchies in 
-        Python without significantly impacting performance. See https://stackoverflow.com/q/1167617 for the
-        initial inspiration for this library.
-        
-        Motivation
-        ----------
-        
-        Python has no standard mechanism by which to guarantee that (1) a method that previously overrode an inherited method
-        continues to do so, and (2) a method that previously did not override an inherited will not override now.
-        This opens the door for subtle problems as class hierarchies evolve over time. For example,
-        
-        1. A method that is added to a superclass is shadowed by an existing method with the same name in a 
-           subclass.
-        
-        2. A method of a superclass that is overridden by a subclass is renamed in the superclass but not in 
-           the subclass.
-        
-        3. A method of a superclass that is overridden by a subclass is removed in the superclass but not in
-           the subclass.
-        
-        4. A method of a superclass that is overridden by a subclass but the signature of the overridden
-           method is incompatible with that of the inherited one.
-        
-        These can be only checked by explicitly marking method override in the code.
-        
-        Python also has no standard mechanism by which to inherit docstrings in overridden methods. Because 
-        most standard linters (e.g., flake8) have rules that require all public methods to have a docstring, 
-        this inevitably leads to a proliferation of ``See parent class for usage`` docstrings on overridden
-        methods, or, worse, to a disabling of these rules altogether. In addition, mediocre or missing
-        docstrings degrade the quality of tooltips and completions that can be provided by an editor.
-        
-        Installation
-        ------------
-        
-        Compatible with Python 3.6+.
-        
-        .. code-block:: bash
-        
-            $ pip install overrides
-        
-        Usage
-        -----
-        
-        Use ``@override`` to indicate that a subclass method should override a superclass method.
-        
-        .. code-block:: python
-        
-            from overrides import override
-        
-            class SuperClass:
-        
-                def foo(self):
-                    """This docstring will be inherited by any method that overrides this!"""
-                    return 1
-        
-                def bar(self, x) -> str:
-                    return x
-        
-            class SubClass(SuperClass):
-        
-                @override
-                def foo(self):
-                    return 2
-        
-                @override
-                def bar(self, y) -> int: # Raises, because the signature is not compatible.
-                    return y
-                    
-                @override
-                def zoo(self): # Raises, because does not exist in the super class.
-                    return "foobarzoo"
-        
-        Use ``EnforceOverrides`` to require subclass methods that shadow superclass methods to be decorated 
-        with ``@override``.
-        
-        .. code-block:: python
-         
-            from overrides import EnforceOverrides
-        
-            class SuperClass(EnforceOverrides):
-        
-                def foo(self):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                def foo(self): # Raises, because @override is missing.
-                    return 2
-        
-        Use ``@final`` to indicate that a superclass method cannot be overriden.
-        With Python 3.11 and above ``@final`` is directly `typing.final <https://docs.python.org/3.11/library/typing.html#typing.final>`_.
-        
-        .. code-block:: python
-        
-            from overrides import EnforceOverrides, final, override
-        
-            class SuperClass(EnforceOverrides):
-        
-                @final
-                def foo(self):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                @override
-                def foo(self): # Raises, because overriding a final method is forbidden.
-                    return 2
-        
-        Note that ``@classmethod`` and ``@staticmethod`` must be declared before ``@override``.
-        
-        .. code-block:: python
-        
-            from overrides import override
-        
-            class SuperClass:
-        
-                @staticmethod
-                def foo(x):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                @staticmethod
-                @override
-                def foo(x):
-                    return 2
-        
-        
-        Flags of control
-        ----------------
-        
-        .. code-block:: python
-        
-            # To prevent all signature checks do:
-            @override(check_signature=False)
-            def some_method(self, now_this_can_be_funny_and_wrong: str, what_ever: int) -> "Dictirux":
-                pass
-        
-            # To do the check only at runtime and solve some forward reference problems
-            @override(check_at_runtime=True)
-            def some_other_method(self, ..) -> "SomethingDefinedLater":
-                pass
-        
-            a.some_other_method() # Kaboom if not SomethingDefinedLater
-        
-        
-        Contributors
-        ------------
-        
-        This project exists only through the work of all the people who contribute.
-        
-        mkorpela, drorasaf, ngoodman90, TylerYep, leeopop, donpatrice, jayvdb, joelgrus, lisyarus, 
-        soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart.
-        
 Keywords: override,inheritence,OOP
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+License-File: LICENSE
+
+overrides
+=========
+
+.. image:: https://img.shields.io/pypi/v/overrides.svg
+  :target: https://pypi.python.org/pypi/overrides
+
+.. image:: http://pepy.tech/badge/overrides
+  :target: http://pepy.tech/project/overrides
+
+A decorator ``@override`` that verifies that a method that should override an inherited method actually does it.
+
+Copies the docstring of the inherited method to the overridden method.
+
+Since signature validation and docstring inheritance are performed on class creation and not on class instantiation,
+this library significantly improves the safety and experience of creating class hierarchies in 
+Python without significantly impacting performance. See https://stackoverflow.com/q/1167617 for the
+initial inspiration for this library.
+
+Motivation
+----------
+
+Python has no standard mechanism by which to guarantee that (1) a method that previously overrode an inherited method
+continues to do so, and (2) a method that previously did not override an inherited will not override now.
+This opens the door for subtle problems as class hierarchies evolve over time. For example,
+
+1. A method that is added to a superclass is shadowed by an existing method with the same name in a 
+   subclass.
+
+2. A method of a superclass that is overridden by a subclass is renamed in the superclass but not in 
+   the subclass.
+
+3. A method of a superclass that is overridden by a subclass is removed in the superclass but not in
+   the subclass.
+
+4. A method of a superclass that is overridden by a subclass but the signature of the overridden
+   method is incompatible with that of the inherited one.
+
+These can be only checked by explicitly marking method override in the code.
+
+Python also has no standard mechanism by which to inherit docstrings in overridden methods. Because 
+most standard linters (e.g., flake8) have rules that require all public methods to have a docstring, 
+this inevitably leads to a proliferation of ``See parent class for usage`` docstrings on overridden
+methods, or, worse, to a disabling of these rules altogether. In addition, mediocre or missing
+docstrings degrade the quality of tooltips and completions that can be provided by an editor.
+
+Installation
+------------
+
+Compatible with Python 3.6+.
+
+.. code-block:: bash
+
+    $ pip install overrides
+
+Usage
+-----
+
+Use ``@override`` to indicate that a subclass method should override a superclass method.
+
+.. code-block:: python
+
+    from overrides import override
+
+    class SuperClass:
+
+        def foo(self):
+            """This docstring will be inherited by any method that overrides this!"""
+            return 1
+
+        def bar(self, x) -> str:
+            return x
+
+    class SubClass(SuperClass):
+
+        @override
+        def foo(self):
+            return 2
+
+        @override
+        def bar(self, y) -> int: # Raises, because the signature is not compatible.
+            return y
+            
+        @override
+        def zoo(self): # Raises, because does not exist in the super class.
+            return "foobarzoo"
+
+Use ``EnforceOverrides`` to require subclass methods that shadow superclass methods to be decorated 
+with ``@override``.
+
+.. code-block:: python
+ 
+    from overrides import EnforceOverrides
+
+    class SuperClass(EnforceOverrides):
+
+        def foo(self):
+            return 1
+
+    class SubClass(SuperClass):
+
+        def foo(self): # Raises, because @override is missing.
+            return 2
+
+Use ``@final`` to indicate that a superclass method cannot be overriden.
+With Python 3.11 and above ``@final`` is directly `typing.final <https://docs.python.org/3.11/library/typing.html#typing.final>`_.
+
+.. code-block:: python
+
+    from overrides import EnforceOverrides, final, override
+
+    class SuperClass(EnforceOverrides):
+
+        @final
+        def foo(self):
+            return 1
+
+    class SubClass(SuperClass):
+
+        @override
+        def foo(self): # Raises, because overriding a final method is forbidden.
+            return 2
+
+Note that ``@classmethod`` and ``@staticmethod`` must be declared before ``@override``.
+
+.. code-block:: python
+
+    from overrides import override
+
+    class SuperClass:
+
+        @staticmethod
+        def foo(x):
+            return 1
+
+    class SubClass(SuperClass):
+
+        @staticmethod
+        @override
+        def foo(x):
+            return 2
+
+
+Flags of control
+----------------
+
+.. code-block:: python
+
+    # To prevent all signature checks do:
+    @override(check_signature=False)
+    def some_method(self, now_this_can_be_funny_and_wrong: str, what_ever: int) -> "Dictirux":
+        pass
+
+    # To do the check only at runtime and solve some forward reference problems
+    @override(check_at_runtime=True)
+    def some_other_method(self, ..) -> "SomethingDefinedLater":
+        pass
+
+    a.some_other_method() # Kaboom if not SomethingDefinedLater
+
+
+Contributors
+------------
+
+This project exists only through the work of all the people who contribute.
+
+mkorpela, drorasaf, ngoodman90, TylerYep, leeopop, donpatrice, jayvdb, joelgrus, lisyarus, 
+soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart, bersbersbers.
```

### Comparing `overrides-7.3.1/README.rst` & `overrides-7.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -160,8 +160,8 @@
 
 Contributors
 ------------
 
 This project exists only through the work of all the people who contribute.
 
 mkorpela, drorasaf, ngoodman90, TylerYep, leeopop, donpatrice, jayvdb, joelgrus, lisyarus, 
-soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart.
+soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart, bersbersbers.
```

### Comparing `overrides-7.3.1/overrides/enforce.py` & `overrides-7.4.0/overrides/enforce.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/overrides/final.py` & `overrides-7.4.0/overrides/final.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/overrides/overrides.py` & `overrides-7.4.0/overrides/overrides.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import dis
 import functools
 import inspect
 import sys
 from types import FunctionType
 from typing import Callable, List, Optional, Tuple, TypeVar, Union, overload
 
-__VERSION__ = "7.3.1"
+__VERSION__ = "7.4.0"
 
 from overrides.signature import ensure_signature_is_compatible
 
 _WrappedMethod = TypeVar("_WrappedMethod", bound=Union[FunctionType, Callable])
 _DecoratorMethod = Callable[[_WrappedMethod], _WrappedMethod]
```

### Comparing `overrides-7.3.1/overrides/signature.py` & `overrides-7.4.0/overrides/signature.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/overrides/typing_utils.py` & `overrides-7.4.0/overrides/typing_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 ## Install
 
 ``` bash
     pip install typing_utils
 ```
 """
 
-
 import collections.abc
 import io
 import itertools
+import types
 import typing
 
 if hasattr(typing, "ForwardRef"):  # python3.8
     ForwardRef = getattr(typing, "ForwardRef")
 elif hasattr(typing, "_ForwardRef"):  # python3.6
     ForwardRef = getattr(typing, "_ForwardRef")
 else:
@@ -31,39 +31,49 @@
     Literal = None
 
 if hasattr(typing, "_TypedDictMeta"):
     _TypedDictMeta = getattr(typing, "_TypedDictMeta")
 else:
     _TypedDictMeta = None
 
+if hasattr(types, "UnionType"):
+    UnionType = getattr(types, "UnionType")
+else:
+    UnionType = None
 
 unknown = None
 
-
 BUILTINS_MAPPING = {
     typing.List: list,
     typing.Set: set,
     typing.Dict: dict,
     typing.Tuple: tuple,
     typing.ByteString: bytes,  # https://docs.python.org/3/library/typing.html#typing.ByteString
     typing.Callable: collections.abc.Callable,
     typing.Sequence: collections.abc.Sequence,
     type(None): None,
 }
 
-
 STATIC_SUBTYPE_MAPPING: typing.Dict[type, typing.Type] = {
     io.TextIOWrapper: typing.TextIO,
     io.TextIOBase: typing.TextIO,
     io.StringIO: typing.TextIO,
     io.BufferedReader: typing.BinaryIO,
     io.BufferedWriter: typing.BinaryIO,
     io.BytesIO: typing.BinaryIO,
 }
 
+if UnionType:
+    def is_union(element: object) -> bool:
+        return element is typing.Union or element is UnionType
+
+else:
+    def is_union(element: object) -> bool:
+        return element is typing.Union
+
 
 def optional_all(elements) -> typing.Optional[bool]:
     if all(elements):
         return True
     if all(e is False for e in elements):
         return False
     return unknown
@@ -171,15 +181,15 @@
     ```
     """
     if hasattr(typing, "get_args"):  # python 3.8+
         _getter = getattr(typing, "get_args")
         res = _getter(type_)
     elif hasattr(typing.List, "_special"):  # python 3.7
         if (
-            isinstance(type_, GenericClass) and not type_._special  # type: ignore
+                isinstance(type_, GenericClass) and not type_._special  # type: ignore
         ):  # backport for python 3.8
             res = type_.__args__  # type: ignore
             if get_origin(type_) is collections.abc.Callable and res[0] is not Ellipsis:
                 res = (list(res[:-1]), res[-1])
         else:
             res = ()
     else:  # python 3.6
@@ -257,29 +267,29 @@
     """
     args = get_args(type_)
     origin = get_origin(type_)
     if not origin:
         return NormalizedType(_normalize_aliases(type_))
     origin = _normalize_aliases(origin)
 
-    if origin is typing.Union:  # sort args when the origin is Union
+    if is_union(origin):  # sort args when the origin is Union
         args = _normalize_args(frozenset(args))
     else:
         args = _normalize_args(args)
     return NormalizedType(origin, args)
 
 
 def _is_origin_subtype(left: OriginType, right: OriginType) -> bool:
     if left is right:
         return True
 
     if (
-        left is not None
-        and left in STATIC_SUBTYPE_MAPPING
-        and right == STATIC_SUBTYPE_MAPPING[left]
+            left is not None
+            and left in STATIC_SUBTYPE_MAPPING
+            and right == STATIC_SUBTYPE_MAPPING[left]
     ):
         return True
 
     if hasattr(left, "mro"):
         for parent in left.mro():  # type: ignore
             if parent == right:
                 return True
@@ -292,17 +302,17 @@
 
 NormalizedTypeArgs = typing.Union[
     typing.Tuple[typing.Any, ...], typing.FrozenSet[NormalizedType], NormalizedType,
 ]
 
 
 def _is_origin_subtype_args(
-    left: "NormalizedTypeArgs",
-    right: "NormalizedTypeArgs",
-    forward_refs: typing.Optional[typing.Mapping[str, type]],
+        left: "NormalizedTypeArgs",
+        right: "NormalizedTypeArgs",
+        forward_refs: typing.Optional[typing.Mapping[str, type]],
 ) -> typing.Optional[bool]:
     if isinstance(left, frozenset):
         if not isinstance(right, frozenset):
             return False
 
         excluded = left - right
         if not excluded:
@@ -311,26 +321,26 @@
 
         # Union[list, int] <> Union[typing.Sequence, int]
         return all(
             any(_is_normal_subtype(e, r, forward_refs) for r in right) for e in excluded
         )
 
     if isinstance(left, collections.abc.Sequence) and not isinstance(
-        left, NormalizedType
+            left, NormalizedType
     ):
         if not isinstance(right, collections.abc.Sequence) or isinstance(
-            right, NormalizedType
+                right, NormalizedType
         ):
             return False
 
         if (
-            left
-            and left[-1].origin is not Ellipsis
-            and right
-            and right[-1].origin is Ellipsis
+                left
+                and left[-1].origin is not Ellipsis
+                and right
+                and right[-1].origin is Ellipsis
         ):
             # Tuple[type, type] <> Tuple[type, ...]
             return all(_is_origin_subtype_args(l, right[0], forward_refs) for l in left)
 
         if len(left) != len(right):
             return False
 
@@ -344,50 +354,49 @@
     assert isinstance(left, NormalizedType)
     assert isinstance(right, NormalizedType)
 
     return _is_normal_subtype(left, right, forward_refs)
 
 
 def _is_normal_subtype(
-    left: NormalizedType,
-    right: NormalizedType,
-    forward_refs: typing.Optional[typing.Mapping[str, type]],
+        left: NormalizedType,
+        right: NormalizedType,
+        forward_refs: typing.Optional[typing.Mapping[str, type]],
 ) -> typing.Optional[bool]:
-
     if isinstance(left.origin, ForwardRef):
         left = normalize(eval_forward_ref(left.origin, forward_refs=forward_refs))
 
     if isinstance(right.origin, ForwardRef):
         right = normalize(eval_forward_ref(right.origin, forward_refs=forward_refs))
 
     # Any
     if right.origin is typing.Any:
         return True
 
     # Union
-    if right.origin is typing.Union and left.origin is typing.Union:
+    if is_union(right.origin) and is_union(left.origin):
         return _is_origin_subtype_args(left.args, right.args, forward_refs)
-    if right.origin is typing.Union:
+    if is_union(right.origin):
         return optional_any(
             _is_normal_subtype(left, a, forward_refs) for a in right.args
         )
-    if left.origin is typing.Union:
+    if is_union(left.origin):
         return optional_all(
             _is_normal_subtype(a, right, forward_refs) for a in left.args
         )
 
     # Literal
     if right.origin is Literal:
         if left.origin is not Literal:
             return False
         return set(left.args).issubset(set(right.args))
 
     # TypeVar
     if isinstance(left.origin, typing.TypeVar) and isinstance(
-        right.origin, typing.TypeVar
+            right.origin, typing.TypeVar
     ):
         if left.origin is right.origin:
             return True
 
         left_bound = getattr(left.origin, "__bound__", None)
         right_bound = getattr(right.origin, "__bound__", None)
         if right_bound is None or left_bound is None:
@@ -412,15 +421,15 @@
     if _is_origin_subtype(left.origin, right.origin):
         return _is_origin_subtype_args(left.args, right.args, forward_refs)
 
     return False
 
 
 def issubtype(
-    left: Type, right: Type, forward_refs: typing.Optional[dict] = None,
+        left: Type, right: Type, forward_refs: typing.Optional[dict] = None,
 ) -> typing.Optional[bool]:
     """Check that the left argument is a subtype of the right.
     For unions, check if the type arguments of the left is a subset of the right.
     Also works for nested types including ForwardRefs.
 
     Examples:
```

### Comparing `overrides-7.3.1/overrides.egg-info/PKG-INFO` & `overrides-7.4.0/overrides.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: overrides
-Version: 7.3.1
+Version: 7.4.0
 Summary: A decorator to automatically detect mismatch when overriding a method.
 Home-page: https://github.com/mkorpela/overrides
 Author: Mikko Korpela
 Author-email: mikko.korpela@gmail.com
 License: Apache License, Version 2.0
-Description: overrides
-        =========
-        
-        .. image:: https://img.shields.io/pypi/v/overrides.svg
-          :target: https://pypi.python.org/pypi/overrides
-        
-        .. image:: http://pepy.tech/badge/overrides
-          :target: http://pepy.tech/project/overrides
-        
-        A decorator ``@override`` that verifies that a method that should override an inherited method actually does it.
-        
-        Copies the docstring of the inherited method to the overridden method.
-        
-        Since signature validation and docstring inheritance are performed on class creation and not on class instantiation,
-        this library significantly improves the safety and experience of creating class hierarchies in 
-        Python without significantly impacting performance. See https://stackoverflow.com/q/1167617 for the
-        initial inspiration for this library.
-        
-        Motivation
-        ----------
-        
-        Python has no standard mechanism by which to guarantee that (1) a method that previously overrode an inherited method
-        continues to do so, and (2) a method that previously did not override an inherited will not override now.
-        This opens the door for subtle problems as class hierarchies evolve over time. For example,
-        
-        1. A method that is added to a superclass is shadowed by an existing method with the same name in a 
-           subclass.
-        
-        2. A method of a superclass that is overridden by a subclass is renamed in the superclass but not in 
-           the subclass.
-        
-        3. A method of a superclass that is overridden by a subclass is removed in the superclass but not in
-           the subclass.
-        
-        4. A method of a superclass that is overridden by a subclass but the signature of the overridden
-           method is incompatible with that of the inherited one.
-        
-        These can be only checked by explicitly marking method override in the code.
-        
-        Python also has no standard mechanism by which to inherit docstrings in overridden methods. Because 
-        most standard linters (e.g., flake8) have rules that require all public methods to have a docstring, 
-        this inevitably leads to a proliferation of ``See parent class for usage`` docstrings on overridden
-        methods, or, worse, to a disabling of these rules altogether. In addition, mediocre or missing
-        docstrings degrade the quality of tooltips and completions that can be provided by an editor.
-        
-        Installation
-        ------------
-        
-        Compatible with Python 3.6+.
-        
-        .. code-block:: bash
-        
-            $ pip install overrides
-        
-        Usage
-        -----
-        
-        Use ``@override`` to indicate that a subclass method should override a superclass method.
-        
-        .. code-block:: python
-        
-            from overrides import override
-        
-            class SuperClass:
-        
-                def foo(self):
-                    """This docstring will be inherited by any method that overrides this!"""
-                    return 1
-        
-                def bar(self, x) -> str:
-                    return x
-        
-            class SubClass(SuperClass):
-        
-                @override
-                def foo(self):
-                    return 2
-        
-                @override
-                def bar(self, y) -> int: # Raises, because the signature is not compatible.
-                    return y
-                    
-                @override
-                def zoo(self): # Raises, because does not exist in the super class.
-                    return "foobarzoo"
-        
-        Use ``EnforceOverrides`` to require subclass methods that shadow superclass methods to be decorated 
-        with ``@override``.
-        
-        .. code-block:: python
-         
-            from overrides import EnforceOverrides
-        
-            class SuperClass(EnforceOverrides):
-        
-                def foo(self):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                def foo(self): # Raises, because @override is missing.
-                    return 2
-        
-        Use ``@final`` to indicate that a superclass method cannot be overriden.
-        With Python 3.11 and above ``@final`` is directly `typing.final <https://docs.python.org/3.11/library/typing.html#typing.final>`_.
-        
-        .. code-block:: python
-        
-            from overrides import EnforceOverrides, final, override
-        
-            class SuperClass(EnforceOverrides):
-        
-                @final
-                def foo(self):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                @override
-                def foo(self): # Raises, because overriding a final method is forbidden.
-                    return 2
-        
-        Note that ``@classmethod`` and ``@staticmethod`` must be declared before ``@override``.
-        
-        .. code-block:: python
-        
-            from overrides import override
-        
-            class SuperClass:
-        
-                @staticmethod
-                def foo(x):
-                    return 1
-        
-            class SubClass(SuperClass):
-        
-                @staticmethod
-                @override
-                def foo(x):
-                    return 2
-        
-        
-        Flags of control
-        ----------------
-        
-        .. code-block:: python
-        
-            # To prevent all signature checks do:
-            @override(check_signature=False)
-            def some_method(self, now_this_can_be_funny_and_wrong: str, what_ever: int) -> "Dictirux":
-                pass
-        
-            # To do the check only at runtime and solve some forward reference problems
-            @override(check_at_runtime=True)
-            def some_other_method(self, ..) -> "SomethingDefinedLater":
-                pass
-        
-            a.some_other_method() # Kaboom if not SomethingDefinedLater
-        
-        
-        Contributors
-        ------------
-        
-        This project exists only through the work of all the people who contribute.
-        
-        mkorpela, drorasaf, ngoodman90, TylerYep, leeopop, donpatrice, jayvdb, joelgrus, lisyarus, 
-        soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart.
-        
 Keywords: override,inheritence,OOP
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
+License-File: LICENSE
+
+overrides
+=========
+
+.. image:: https://img.shields.io/pypi/v/overrides.svg
+  :target: https://pypi.python.org/pypi/overrides
+
+.. image:: http://pepy.tech/badge/overrides
+  :target: http://pepy.tech/project/overrides
+
+A decorator ``@override`` that verifies that a method that should override an inherited method actually does it.
+
+Copies the docstring of the inherited method to the overridden method.
+
+Since signature validation and docstring inheritance are performed on class creation and not on class instantiation,
+this library significantly improves the safety and experience of creating class hierarchies in 
+Python without significantly impacting performance. See https://stackoverflow.com/q/1167617 for the
+initial inspiration for this library.
+
+Motivation
+----------
+
+Python has no standard mechanism by which to guarantee that (1) a method that previously overrode an inherited method
+continues to do so, and (2) a method that previously did not override an inherited will not override now.
+This opens the door for subtle problems as class hierarchies evolve over time. For example,
+
+1. A method that is added to a superclass is shadowed by an existing method with the same name in a 
+   subclass.
+
+2. A method of a superclass that is overridden by a subclass is renamed in the superclass but not in 
+   the subclass.
+
+3. A method of a superclass that is overridden by a subclass is removed in the superclass but not in
+   the subclass.
+
+4. A method of a superclass that is overridden by a subclass but the signature of the overridden
+   method is incompatible with that of the inherited one.
+
+These can be only checked by explicitly marking method override in the code.
+
+Python also has no standard mechanism by which to inherit docstrings in overridden methods. Because 
+most standard linters (e.g., flake8) have rules that require all public methods to have a docstring, 
+this inevitably leads to a proliferation of ``See parent class for usage`` docstrings on overridden
+methods, or, worse, to a disabling of these rules altogether. In addition, mediocre or missing
+docstrings degrade the quality of tooltips and completions that can be provided by an editor.
+
+Installation
+------------
+
+Compatible with Python 3.6+.
+
+.. code-block:: bash
+
+    $ pip install overrides
+
+Usage
+-----
+
+Use ``@override`` to indicate that a subclass method should override a superclass method.
+
+.. code-block:: python
+
+    from overrides import override
+
+    class SuperClass:
+
+        def foo(self):
+            """This docstring will be inherited by any method that overrides this!"""
+            return 1
+
+        def bar(self, x) -> str:
+            return x
+
+    class SubClass(SuperClass):
+
+        @override
+        def foo(self):
+            return 2
+
+        @override
+        def bar(self, y) -> int: # Raises, because the signature is not compatible.
+            return y
+            
+        @override
+        def zoo(self): # Raises, because does not exist in the super class.
+            return "foobarzoo"
+
+Use ``EnforceOverrides`` to require subclass methods that shadow superclass methods to be decorated 
+with ``@override``.
+
+.. code-block:: python
+ 
+    from overrides import EnforceOverrides
+
+    class SuperClass(EnforceOverrides):
+
+        def foo(self):
+            return 1
+
+    class SubClass(SuperClass):
+
+        def foo(self): # Raises, because @override is missing.
+            return 2
+
+Use ``@final`` to indicate that a superclass method cannot be overriden.
+With Python 3.11 and above ``@final`` is directly `typing.final <https://docs.python.org/3.11/library/typing.html#typing.final>`_.
+
+.. code-block:: python
+
+    from overrides import EnforceOverrides, final, override
+
+    class SuperClass(EnforceOverrides):
+
+        @final
+        def foo(self):
+            return 1
+
+    class SubClass(SuperClass):
+
+        @override
+        def foo(self): # Raises, because overriding a final method is forbidden.
+            return 2
+
+Note that ``@classmethod`` and ``@staticmethod`` must be declared before ``@override``.
+
+.. code-block:: python
+
+    from overrides import override
+
+    class SuperClass:
+
+        @staticmethod
+        def foo(x):
+            return 1
+
+    class SubClass(SuperClass):
+
+        @staticmethod
+        @override
+        def foo(x):
+            return 2
+
+
+Flags of control
+----------------
+
+.. code-block:: python
+
+    # To prevent all signature checks do:
+    @override(check_signature=False)
+    def some_method(self, now_this_can_be_funny_and_wrong: str, what_ever: int) -> "Dictirux":
+        pass
+
+    # To do the check only at runtime and solve some forward reference problems
+    @override(check_at_runtime=True)
+    def some_other_method(self, ..) -> "SomethingDefinedLater":
+        pass
+
+    a.some_other_method() # Kaboom if not SomethingDefinedLater
+
+
+Contributors
+------------
+
+This project exists only through the work of all the people who contribute.
+
+mkorpela, drorasaf, ngoodman90, TylerYep, leeopop, donpatrice, jayvdb, joelgrus, lisyarus, 
+soulmerge, rkr-at-dbx, ashwin153, brentyi,  jobh, tjsmart, bersbersbers.
```

### Comparing `overrides-7.3.1/overrides.egg-info/SOURCES.txt` & `overrides-7.4.0/overrides.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 overrides.egg-info/requires.txt
 overrides.egg-info/top_level.txt
 tests/test_decorator_params.py
 tests/test_enforce__py38.py
 tests/test_final.py
 tests/test_issubtype_with_typeddict__py38.py
 tests/test_named_and_positional__py38.py
+tests/test_new_union__py3_10.py
 tests/test_overrides.py
 tests/test_signatures.py
 tests/test_somefinalpackage.py
 tests/test_somepackage.py
 tests/test_special_cases.py
```

### Comparing `overrides-7.3.1/setup.py` & `overrides-7.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 CURDIR = dirname(abspath(__file__))
 
 with open(join(CURDIR, "README.rst")) as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="overrides",
-    version="7.3.1",
+    version="7.4.0",
     description=desc,
     long_description=LONG_DESCRIPTION,
     author=name,
     author_email=address,
     url="https://github.com/mkorpela/overrides",
     packages=find_packages(),
     package_data={"overrides": ["*.pyi", "py.typed"],},
```

### Comparing `overrides-7.3.1/tests/test_decorator_params.py` & `overrides-7.4.0/tests/test_decorator_params.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_enforce__py38.py` & `overrides-7.4.0/tests/test_enforce__py38.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_final.py` & `overrides-7.4.0/tests/test_final.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_named_and_positional__py38.py` & `overrides-7.4.0/tests/test_named_and_positional__py38.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_overrides.py` & `overrides-7.4.0/tests/test_overrides.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_signatures.py` & `overrides-7.4.0/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `overrides-7.3.1/tests/test_special_cases.py` & `overrides-7.4.0/tests/test_special_cases.py`

 * *Files identical despite different names*

