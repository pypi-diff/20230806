# Comparing `tmp/pwnic-0.4.0.tar.gz` & `tmp/pwnic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwnic-0.4.0.tar", max compression
+gzip compressed data, was "pwnic-0.5.0.tar", max compression
```

## Comparing `pwnic-0.4.0.tar` & `pwnic-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    32471 2023-07-09 18:22:17.480086 pwnic-0.4.0/LICENSE
--rw-r--r--   0        0        0    11979 2023-07-11 15:37:58.352880 pwnic-0.4.0/README.md
--rw-r--r--   0        0        0      346 2023-07-09 18:22:17.484086 pwnic-0.4.0/pwnic/Attacker.py
--rw-r--r--   0        0        0      239 2023-07-09 18:22:17.484086 pwnic-0.4.0/pwnic/Submitter.py
--rw-r--r--   0        0        0      576 2023-07-11 20:56:51.048536 pwnic-0.4.0/pwnic/__init__.py
--rw-r--r--   0        0        0       89 2023-07-11 20:06:54.967256 pwnic-0.4.0/pwnic/__main__.py
--rw-r--r--   0        0        0     1735 2023-07-11 20:59:23.281843 pwnic-0.4.0/pwnic/api.py
--rw-r--r--   0        0        0      468 2023-07-09 18:31:09.133305 pwnic-0.4.0/pwnic/config.py
--rw-r--r--   0        0        0      110 2023-07-09 18:22:17.485086 pwnic-0.4.0/pwnic/db.py
--rw-r--r--   0        0        0     2425 2023-07-11 20:59:06.676810 pwnic-0.4.0/pwnic/exploits.py
--rw-r--r--   0        0        0      612 2023-07-11 20:58:46.112768 pwnic-0.4.0/pwnic/utils.py
--rw-r--r--   0        0        0     3623 2023-07-11 20:59:58.341914 pwnic-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    12958 1970-01-01 00:00:00.000000 pwnic-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-07-09 18:22:17.480086 pwnic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3169 2023-07-12 17:39:49.836758 pwnic-0.5.0/README.md
+-rw-r--r--   0        0        0     1497 2023-08-05 15:33:37.288454 pwnic-0.5.0/pwnic/BaseAttacker.py
+-rw-r--r--   0        0        0      938 2023-08-05 17:31:31.926844 pwnic-0.5.0/pwnic/__init__.py
+-rw-r--r--   0        0        0      279 2023-08-05 15:33:37.288454 pwnic-0.5.0/pwnic/__main__.py
+-rw-r--r--   0        0        0     2461 2023-08-06 07:21:58.117043 pwnic-0.5.0/pwnic/api.py
+-rw-r--r--   0        0        0     2013 2023-08-05 15:33:37.288454 pwnic-0.5.0/pwnic/config.py
+-rw-r--r--   0        0        0     3551 2023-08-05 15:33:37.289371 pwnic-0.5.0/pwnic/db.py
+-rw-r--r--   0        0        0     4615 2023-08-05 19:16:38.722501 pwnic-0.5.0/pwnic/exploits.py
+-rw-r--r--   0        0        0     1114 2023-07-12 21:58:20.338488 pwnic-0.5.0/pwnic/logger.py
+-rw-r--r--   0        0        0     1260 2023-08-05 15:33:37.289371 pwnic-0.5.0/pwnic/submitter.py
+-rw-r--r--   0        0        0     2065 2023-08-05 15:33:37.255454 pwnic-0.5.0/pwnic/utils.py
+-rw-r--r--   0        0        0     3705 2023-08-06 07:34:47.534857 pwnic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 pwnic-0.5.0/PKG-INFO
```

### Comparing `pwnic-0.4.0/LICENSE` & `pwnic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwnic-0.4.0/pyproject.toml` & `pwnic-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pwnic"
-version = "0.4.0"
+version = "0.5.0"
 description = "Awesome `pwnic` is a Python cli/package created with https://github.com/TezRomacH/python-package-template"
 readme = "README.md"
 authors = ["pwnic <francesco.basile12@studenti.unina.it>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/pwnic/pwnic"
 homepage = "https://github.com/pwnic/pwnic"
 
@@ -27,37 +27,40 @@
   "Programming Language :: Python :: 3.11",
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
-pymongo = "*"
 fastapi = "^0.100.0"
 python-multipart = "^0.0.6"
+rfc3987 = "^1.3.8"
+colorlog = "^6.7.0"
+rich = "^13.4.2"
+jsonschema = "^4.18.2"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.4.1"
 pre-commit = "^3.3.3"
 pydocstyle = "^6.3.0"
-pylint = "^2.17.4"
+pylint = "^2.17.5"
 pytest = "^7.4.0"
-pyupgrade = "^3.9.0"
+pyupgrade = "^3.10.1"
 safety = "^2.3.5"
 coverage = "^7.2.7"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.1.0"
 black = {version = "^23.7.0", allow-prereleases = true}
 httpx = "^0.24.1"
-icecream = "^2.1.3"
 
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py311"]
 line-length = 79
 color = true
@@ -115,15 +118,16 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 exclude = [
     'tests/exploits',
-    'exploits'
+    'exploits',
+    'configs'
 ]
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
 norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__", "tests/exploits"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
```

