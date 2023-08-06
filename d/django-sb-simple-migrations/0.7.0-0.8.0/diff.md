# Comparing `tmp/django_sb_simple_migrations-0.7.0.tar.gz` & `tmp/django_sb_simple_migrations-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sb_simple_migrations-0.7.0.tar", max compression
+gzip compressed data, was "django_sb_simple_migrations-0.8.0.tar", max compression
```

## Comparing `django_sb_simple_migrations-0.7.0.tar` & `django_sb_simple_migrations-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1082 2023-04-20 05:53:07.857550 django_sb_simple_migrations-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2022-12-12 01:48:28.326594 django_sb_simple_migrations-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     3191 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/README.md
--rw-r--r--   0        0        0     2225 2023-04-20 05:53:07.853549 django_sb_simple_migrations-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/admin.py
--rw-r--r--   0        0        0      229 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/apps.py
--rw-r--r--   0        0        0     2190 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/conf.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/__init__.py
--rw-r--r--   0        0        0     1868 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/makemigrations.py
--rw-r--r--   0        0        0     1117 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/migrate.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/models.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/tests.py
--rw-r--r--   0        0        0       20 2023-04-20 05:53:07.861549 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/version.py
--rw-r--r--   0        0        0        0 2023-04-20 05:49:56.975711 django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/views.py
--rw-r--r--   0        0        0     4762 1970-01-01 00:00:00.000000 django_sb_simple_migrations-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1204 2023-08-06 05:34:08.605455 django_sb_simple_migrations-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2022-12-12 01:48:28.326594 django_sb_simple_migrations-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     3191 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/README.md
+-rw-r--r--   0        0        0     2680 2023-08-06 05:34:08.605455 django_sb_simple_migrations-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/admin.py
+-rw-r--r--   0        0        0      229 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/apps.py
+-rw-r--r--   0        0        0     2190 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/conf.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1868 2023-08-06 05:32:33.684964 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/commands/makemigrations.py
+-rw-r--r--   0        0        0     1117 2023-08-06 05:32:33.684964 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/commands/migrate.py
+-rw-r--r--   0        0        0        0 2023-08-06 05:32:33.684964 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/models.py
+-rw-r--r--   0        0        0        0 2023-08-05 22:14:37.779941 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/tests.py
+-rw-r--r--   0        0        0       20 2023-08-06 05:34:08.605455 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/version.py
+-rw-r--r--   0        0        0        0 2023-04-20 05:54:06.902742 django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/views.py
+-rw-r--r--   0        0        0     4838 1970-01-01 00:00:00.000000 django_sb_simple_migrations-0.8.0/PKG-INFO
```

### Comparing `django_sb_simple_migrations-0.7.0/CHANGELOG.md` & `django_sb_simple_migrations-0.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.8.0] - 2023-08-05
+
+* Update dependencies
+* Drop support for python 3.8.0
+* Add base clases for testing
+* Add CI/CD
+
 ## [0.7.0] - 2023-04-20
 
 - Drop support for python 3.8.0
 - Update dependencies
 - Update development tools configuration
 - Update repository structure
 - Update references from Github to GitLab
```

### Comparing `django_sb_simple_migrations-0.7.0/LICENSE.txt` & `django_sb_simple_migrations-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_sb_simple_migrations-0.7.0/README.md` & `django_sb_simple_migrations-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `django_sb_simple_migrations-0.7.0/pyproject.toml` & `django_sb_simple_migrations-0.8.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-sb-simple-migrations"
-version = "0.7.0"
+version = "0.8.0"
 description = "Django migrations without unnecesary change alert triggers."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -18,52 +18,57 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Framework :: Django :: 2",
+  "Framework :: Django :: 3",
+  "Framework :: Django :: 4",
+  "Framework :: Wagtail :: 3",
+  "Framework :: Wagtail :: 4",
+  "Framework :: Wagtail :: 5",
 ]
 packages = [
     { include = "django_sb_simple_migrations", from = "src" }
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.7.0.tar.gz"
+"Download" = "https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.8.0.tar.gz"
 "Bug Tracker" = "https://github.com/softbutterfly/django-sb-simple-migrations/issues"
 
 
 [tool.poetry.dependencies]
-python = ">= 3.8, < 4.0.0"
+python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0.0"
 
 [tool.poetry.dev-dependencies]
-autopep8 = "^1.6.0"
-black = "^22.3.0"
-codecov = "^2.1.12"
-coverage = "^6.3.3"
-flake8 = "^4.0.1"
-flake8-black = "^0.3.3"
-jupyterlab = "^3.4.2"
-mypy = "^0.950"
-pre-commit = "^2.19.0"
-pydocstyle = "^6.1.1"
-pylint = "^2.13.9"
+autopep8 = "^2.0.2"
+bandit = "^1.7.5"
+black = "^23.3.0"
+coverage = "^7.2.7"
+flake8 = "^6.0.0"
+flake8-black = "^0.3.6"
+isort = "^5.12.0"
+mypy = "^1.3.0"
+pre-commit = "^3.3.3"
+pydocstyle = "^6.3.0"
+pylint = "^2.17.4"
 pylint-django = "^2.5.3"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-pytest-vcr = "^1.0.2"
-python-dotenv = "^0.20.0"
-tox = "^3.25.0"
-twine = "^4.0.0"
-tbump = "^6.9.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pytest-django = "^4.5.2"
+python-dotenv = "^1.0.0"
+tbump = "^6.10.0"
+tox = "^4.6.2"
 
 [tool.black]
 target_version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 /(\.git/
   |\.eggs
@@ -80,10 +85,25 @@
   |build
   |dist
   |legacy
   |example
 )/
 '''
 
+[tool.pytest.ini_options]
+DJANGO_SETTINGS_MODULE = "demoproject.settings"
+pythonpath = "demoproject"
+testpaths = "tests"
+python_files = [
+  "**/test_*.py",
+]
+filterwarnings =[
+  "ignore::DeprecationWarning",
+  "ignore::PendingDeprecationWarning"
+]
+addopts = [
+  "--import-mode=importlib",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/conf.py` & `django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/conf.py`

 * *Files identical despite different names*

### Comparing `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/makemigrations.py` & `django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `django_sb_simple_migrations-0.7.0/src/django_sb_simple_migrations/management/commands/migrate.py` & `django_sb_simple_migrations-0.8.0/src/django_sb_simple_migrations/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `django_sb_simple_migrations-0.7.0/PKG-INFO` & `django_sb_simple_migrations-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: django-sb-simple-migrations
-Version: 0.7.0
+Version: 0.8.0
 Summary: Django migrations without unnecesary change alert triggers.
 Home-page: https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
-Requires-Python: >=3.8,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Django :: 2
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0.0)
 Project-URL: Bug Tracker, https://github.com/softbutterfly/django-sb-simple-migrations/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations/-/wikis
-Project-URL: Download, https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.7.0.tar.gz
+Project-URL: Download, https://github.com/softbutterfly/django-sb-simple-migrations/archive/v0.8.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/django-sb-simple-migrations
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/django-sb-simple-migrations)
 ![PyPI - Package version](https://img.shields.io/pypi/v/django-sb-simple-migrations)
```

