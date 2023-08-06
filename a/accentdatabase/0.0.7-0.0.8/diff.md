# Comparing `tmp/accentdatabase-0.0.7.tar.gz` & `tmp/accentdatabase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accentdatabase-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "accentdatabase-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `accentdatabase-0.0.7.tar` & `accentdatabase-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.7/.flake8
--rw-r--r--   0        0        0      929 2023-07-10 10:47:48.676086 accentdatabase-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.7/.gitignore
--rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.7/LICENSE
--rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.7/README.md
--rw-r--r--   0        0        0      134 2023-07-18 11:10:48.248747 accentdatabase-0.0.7/accentdatabase/__init__.py
--rw-r--r--   0        0        0      481 2023-03-30 07:48:07.000000 accentdatabase-0.0.7/accentdatabase/base.py
--rw-r--r--   0        0        0      384 2023-07-18 11:09:14.197112 accentdatabase-0.0.7/accentdatabase/config.py
--rw-r--r--   0        0        0      243 2023-07-10 10:09:15.252548 accentdatabase-0.0.7/accentdatabase/engine.py
--rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.7/accentdatabase/mixins.py
--rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.7/accentdatabase/operations.py
--rw-r--r--   0        0        0      852 2023-07-10 10:52:21.692037 accentdatabase-0.0.7/accentdatabase/session.py
--rw-r--r--   0        0        0     1007 2023-07-10 10:09:51.012364 accentdatabase-0.0.7/accentdatabase/testing.py
--rw-r--r--   0        0        0     1304 2023-07-10 10:45:05.999094 accentdatabase-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 accentdatabase-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       99 2022-10-05 10:37:49.000000 accentdatabase-0.0.8/.flake8
+-rw-r--r--   0        0        0      929 2023-07-10 10:47:48.676086 accentdatabase-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0       98 2022-10-05 13:05:19.000000 accentdatabase-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1090 2022-10-10 11:22:41.000000 accentdatabase-0.0.8/LICENSE
+-rw-r--r--   0        0        0      319 2022-10-06 08:19:07.000000 accentdatabase-0.0.8/README.md
+-rw-r--r--   0        0        0      134 2023-08-06 00:28:24.051302 accentdatabase-0.0.8/accentdatabase/__init__.py
+-rw-r--r--   0        0        0      481 2023-03-30 07:48:07.000000 accentdatabase-0.0.8/accentdatabase/base.py
+-rw-r--r--   0        0        0      384 2023-07-18 11:09:14.197112 accentdatabase-0.0.8/accentdatabase/config.py
+-rw-r--r--   0        0        0      243 2023-07-10 10:09:15.252548 accentdatabase-0.0.8/accentdatabase/engine.py
+-rw-r--r--   0        0        0      658 2023-02-24 15:56:58.000000 accentdatabase-0.0.8/accentdatabase/mixins.py
+-rw-r--r--   0        0        0     6675 2023-01-03 13:49:46.000000 accentdatabase-0.0.8/accentdatabase/operations.py
+-rw-r--r--   0        0        0      852 2023-07-10 10:52:21.692037 accentdatabase-0.0.8/accentdatabase/session.py
+-rw-r--r--   0        0        0     1007 2023-07-10 10:09:51.012364 accentdatabase-0.0.8/accentdatabase/testing.py
+-rw-r--r--   0        0        0     1304 2023-08-06 00:23:33.121022 accentdatabase-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 accentdatabase-0.0.8/PKG-INFO
```

### Comparing `accentdatabase-0.0.7/.github/workflows/test.yml` & `accentdatabase-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/LICENSE` & `accentdatabase-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/accentdatabase/mixins.py` & `accentdatabase-0.0.8/accentdatabase/mixins.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/accentdatabase/operations.py` & `accentdatabase-0.0.8/accentdatabase/operations.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/accentdatabase/session.py` & `accentdatabase-0.0.8/accentdatabase/session.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/accentdatabase/testing.py` & `accentdatabase-0.0.8/accentdatabase/testing.py`

 * *Files identical despite different names*

### Comparing `accentdatabase-0.0.7/pyproject.toml` & `accentdatabase-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
 ]
 dependencies = [
-    "pydantic>=2.0.1,<2.1.0",
+    "pydantic>=2.0.1,<2.2.0",
     "pydantic-settings>=2.0.1,<2.1.0",
     "sqlalchemy>=2.0.0,<2.1.0",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Homepage = "https://github.com/accentdesign/accentdatabase"
```

### Comparing `accentdatabase-0.0.7/PKG-INFO` & `accentdatabase-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: accentdatabase
-Version: 0.0.7
+Version: 0.0.8
 Summary: Handling sqlalchemy connection and test helpers including
 Author-email: Accent Design Group Ltd <support@accentdesign.co.uk>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.1.0
+Requires-Dist: pydantic>=2.0.1,<2.2.0
 Requires-Dist: pydantic-settings>=2.0.1,<2.1.0
 Requires-Dist: sqlalchemy>=2.0.0,<2.1.0
 Requires-Dist: alembic ; extra == "alembic"
 Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.7 Summary: Handling
+Metadata-Version: 2.1 Name: accentdatabase Version: 0.0.8 Summary: Handling
 sqlalchemy connection and test helpers including Author-email: Accent Design
 Group Ltd
 accentdesign.co.uk> Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Requires-Dist: pydantic>=2.0.1,<2.1.0 Requires-Dist: pydantic-
+Requires-Dist: pydantic>=2.0.1,<2.2.0 Requires-Dist: pydantic-
 settings>=2.0.1,<2.1.0 Requires-Dist: sqlalchemy>=2.0.0,<2.1.0 Requires-Dist:
 alembic ; extra == "alembic" Requires-Dist: autoflake ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev" Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: mypy ; extra ==
 "test" Requires-Dist: flake8 ; extra == "test" Requires-Dist: black ; extra ==
 "test" Requires-Dist: isort ; extra == "test" Project-URL: Homepage, https://
 github.com/accentdesign/accentdatabase Provides-Extra: alembic Provides-Extra:
```

