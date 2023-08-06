# Comparing `tmp/parol-1.0.1.tar.gz` & `tmp/parol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parol-1.0.1.tar", max compression
+gzip compressed data, was "parol-1.1.0.tar", max compression
```

## Comparing `parol-1.0.1.tar` & `parol-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-08-04 20:33:16.295293 parol-1.0.1/LICENSE
--rw-r--r--   0        0        0      720 2023-08-04 20:33:16.295293 parol-1.0.1/README.md
--rw-r--r--   0        0        0     2234 2023-08-04 20:33:16.295293 parol-1.0.1/parol/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 20:33:16.295293 parol-1.0.1/parol/py.typed
--rw-r--r--   0        0        0     2342 2023-08-04 20:33:16.295293 parol-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 parol-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-08-06 07:30:35.081808 parol-1.1.0/LICENSE
+-rw-r--r--   0        0        0      706 2023-08-06 07:30:35.081808 parol-1.1.0/README.md
+-rw-r--r--   0        0        0     1404 2023-08-06 07:30:35.081808 parol-1.1.0/parol/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 07:30:35.081808 parol-1.1.0/parol/py.typed
+-rw-r--r--   0        0        0     2360 2023-08-06 07:30:35.081808 parol-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 parol-1.1.0/PKG-INFO
```

### Comparing `parol-1.0.1/LICENSE` & `parol-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parol-1.0.1/README.md` & `parol-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 ```
 pip install parol
 ```
 
 ## Usage
 
 ```python
->>> import parol
->>> pwd = parol.generate()
->>> parol.validate(pwd.password, pwd.salt, pwd.hash)
+>>> from parol import Password
+>>> pwd = Password.gen()
+>>> pwd.verify(pwd.hash())
 True
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

### Comparing `parol-1.0.1/pyproject.toml` & `parol-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
+version = "1.1.0"
 tag_format = "$version"
 version_files = [
     "parol/__init__.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "parol"
-version = "1.0.1"
+version = "1.1.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/parol"
 homepage = "https://pypi.org/project/parol"
 keywords = []
 
 [tool.poetry.urls]
 Changelog = "https://github.com/daxartio/parol/blob/main/CHANGELOG.md/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+bcrypt = "^4.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-deadfixtures = "^2.2.1"
```

### Comparing `parol-1.0.1/PKG-INFO` & `parol-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: parol
-Version: 1.0.1
+Version: 1.1.0
 Summary: 
 Home-page: https://pypi.org/project/parol
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
 Project-URL: Changelog, https://github.com/daxartio/parol/blob/main/CHANGELOG.md/
 Project-URL: Repository, https://github.com/daxartio/parol
 Description-Content-Type: text/markdown
 
 # parol
 
 [![PyPI](https://img.shields.io/pypi/v/parol)](https://pypi.org/project/parol/)
@@ -29,17 +30,17 @@
 ```
 pip install parol
 ```
 
 ## Usage
 
 ```python
->>> import parol
->>> pwd = parol.generate()
->>> parol.validate(pwd.password, pwd.salt, pwd.hash)
+>>> from parol import Password
+>>> pwd = Password.gen()
+>>> pwd.verify(pwd.hash())
 True
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

