# Comparing `tmp/peprock-1.6.0.tar.gz` & `tmp/peprock-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peprock-1.6.0.tar", max compression
+gzip compressed data, was "peprock-1.6.1.tar", max compression
```

## Comparing `peprock-1.6.0.tar` & `peprock-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1083 2023-03-15 09:00:20.745728 peprock-1.6.0/LICENSE
--rw-r--r--   0        0        0     1780 2023-03-15 09:00:20.745728 peprock-1.6.0/README.md
--rw-r--r--   0        0        0       27 2023-03-15 09:00:57.818086 peprock-1.6.0/peprock/_version/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/_version/py.typed
--rw-r--r--   0        0        0      753 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/datetime/__init__.py
--rw-r--r--   0        0        0     2455 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/datetime/awareness.py
--rw-r--r--   0        0        0      896 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/datetime/constants.py
--rw-r--r--   0        0        0        0 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/datetime/py.typed
--rw-r--r--   0        0        0      298 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/models/__init__.py
--rw-r--r--   0        0        0    20113 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/models/measurement.py
--rw-r--r--   0        0        0     4311 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/models/metric_prefix.py
--rw-r--r--   0        0        0        0 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/models/py.typed
--rw-r--r--   0        0        0     1964 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/models/unit.py
--rw-r--r--   0        0        0      128 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/patterns/__init__.py
--rw-r--r--   0        0        0     2062 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/patterns/observer.py
--rw-r--r--   0        0        0        0 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/patterns/py.typed
--rw-r--r--   0        0        0     1729 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/subclasses/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 09:00:20.745728 peprock-1.6.0/peprock/subclasses/py.typed
--rw-r--r--   0        0        0     3812 2023-03-15 09:00:57.874086 peprock-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 peprock-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-06 17:14:26.272859 peprock-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1780 2023-08-06 17:14:26.272859 peprock-1.6.1/README.md
+-rw-r--r--   0        0        0       27 2023-08-06 17:14:52.834633 peprock-1.6.1/peprock/_version/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/_version/py.typed
+-rw-r--r--   0        0        0      753 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/__init__.py
+-rw-r--r--   0        0        0     2456 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/awareness.py
+-rw-r--r--   0        0        0      897 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/constants.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/datetime/py.typed
+-rw-r--r--   0        0        0      298 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/__init__.py
+-rw-r--r--   0        0        0    20114 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/measurement.py
+-rw-r--r--   0        0        0     4312 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/metric_prefix.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/py.typed
+-rw-r--r--   0        0        0     1965 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/models/unit.py
+-rw-r--r--   0        0        0      128 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/__init__.py
+-rw-r--r--   0        0        0     2063 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/observer.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/patterns/py.typed
+-rw-r--r--   0        0        0     1730 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/subclasses/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 17:14:26.272859 peprock-1.6.1/peprock/subclasses/py.typed
+-rw-r--r--   0        0        0     4081 2023-08-06 17:14:52.894636 peprock-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 peprock-1.6.1/PKG-INFO
```

### Comparing `peprock-1.6.0/LICENSE` & `peprock-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peprock-1.6.0/README.md` & `peprock-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `peprock-1.6.0/peprock/datetime/__init__.py` & `peprock-1.6.1/peprock/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `peprock-1.6.0/peprock/datetime/awareness.py` & `peprock-1.6.1/peprock/datetime/awareness.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 False
 
 >>> aware = ensure_aware(naive, assumed_tz=datetime.timezone.utc)
 >>> is_naive(aware)
 False
 >>> is_aware(aware)
 True
+
 """
 
 from __future__ import annotations
 
 import datetime  # noqa: TCH003
 import functools
```

### Comparing `peprock-1.6.0/peprock/datetime/constants.py` & `peprock-1.6.1/peprock/datetime/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Timedelta constants.
 
 Examples
 --------
 >>> dt = datetime.datetime(2023, 3, 2, 21, 17, 12)
 >>> dt + ONE_HOUR + 5 * ONE_SECOND
 datetime.datetime(2023, 3, 2, 22, 17, 17)
+
 """
 
 import datetime
 import typing
 
 ONE_MICROSECOND: typing.Final[datetime.timedelta] = datetime.timedelta(microseconds=1)
 ONE_MILLISECOND: typing.Final[datetime.timedelta] = datetime.timedelta(milliseconds=1)
```

### Comparing `peprock-1.6.0/peprock/models/measurement.py` & `peprock-1.6.1/peprock/models/measurement.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Measurement(magnitude=4001.2, prefix=<MetricPrefix.NONE: 0>, unit=None)
 
 >>> str(abs(2 * Measurement(decimal.Decimal("-12.3"), MetricPrefix.mega, Unit.watt)))
 '24.6 MW'
 
 >>> int(Measurement(0.123456, MetricPrefix.kilo))
 123
+
 """
 
 from __future__ import annotations
 
 import dataclasses
 import decimal
 import fractions
```

### Comparing `peprock-1.6.0/peprock/models/metric_prefix.py` & `peprock-1.6.1/peprock/models/metric_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Examples
 --------
 >>> MetricPrefix.mega.convert(5, to=MetricPrefix.kilo)
 5000
 
 >>> MetricPrefix.centi.convert(0.7, to=MetricPrefix.milli)
 7.0
+
 """
 
 from __future__ import annotations
 
 import enum
 import functools
 import types
```

### Comparing `peprock-1.6.0/peprock/models/unit.py` & `peprock-1.6.1/peprock/models/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Examples
 --------
 >>> Unit.ohm.symbol
 'Ω'
 
 >>> Unit("W")
 <Unit.watt: 'W'>
+
 """
 
 from __future__ import annotations
 
 import enum
```

### Comparing `peprock-1.6.0/peprock/patterns/observer.py` & `peprock-1.6.1/peprock/patterns/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ...         print(f"My observer notified by {type(subject).__name__}: {message}")
 ...
 >>> observer = MyObserver()
 >>> subject = Subject()
 >>> subject.register_observer(observer)
 >>> subject.notify_observers("Hello, world!")
 My observer notified by Subject: Hello, world!
+
 """
 
 from __future__ import annotations
 
 import abc
 import functools
 import typing
```

### Comparing `peprock-1.6.0/peprock/subclasses/__init__.py` & `peprock-1.6.1/peprock/subclasses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 [<enum 'IntEnum'>, <enum 'IntFlag'>, <class 'sre_constants._NamedIntConstant'>, <class 'bool'>]
 
 >>> get_by_name(int, name="bool")
 <class 'bool'>
 
 >>> len(get(object))  # doctest: +SKIP
 280
+
 """
 
 from __future__ import annotations
 
 import inspect
 import typing
```

### Comparing `peprock-1.6.0/pyproject.toml` & `peprock-1.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.commitizen]
 bump_message = "chore: bump version to $new_version"
 changelog_incremental = true
 update_changelog_on_bump = true
-version = "1.6.0"
+version = "1.6.1"
 version_files = [
     "peprock/_version/__init__.py",
     "pyproject.toml",
 ]
 
 
 [tool.coverage.report]
@@ -33,15 +33,15 @@
 warn_unused_ignores = true
 warn_unused_configs = true
 warn_unreachable = true
 
 
 [tool.poetry]
 name = "peprock"
-version = "1.6.0"
+version = "1.6.1"
 description = "Foundational Python library"
 license = "MIT"
 authors = [
     "Jakob Keller <57402305+jakob-keller@users.noreply.github.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Ponte-Energy-Partners/peprock"
@@ -62,22 +62,22 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = { version = "^4.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 coverage = { version = "^7.2.1", extras = ["toml"] }
 mypy = "^1.1.1"
 pre-commit = "^3.1.1"
 pdoc3 = "^0.10.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.256"
+ruff = "^0.0.282"
 
 [tool.poetry.urls]
 "Ponte Energy Partners" = "https://ponte.energy"
 
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --import-mode=importlib"
@@ -96,49 +96,59 @@
     "C90", # mccabe
     "I", # isort
     "N", # pep8-naming
     "D", # pydocstyle
     "UP", # pyupgrade
     "YTT", # flake8-2020
     "ANN", # flake8-annotations
+    "ASYNC",  # flake8-async
     "S", # flake8-bandit
     "BLE", # flake8-blind-except
     "FBT", # flake8-boolean-trap
     "B", # flake8-bugbear
     "A", # flake8-builtins
     "COM", # flake8-commas
+    "CPY", # flake-copyright
     "C4", # flake8-comprehensions
     "DTZ", # flake8-datetimez
     "T10", # flake8-debugger
     "DJ", # flake8-django
     "EM", # flake8-errmsg
     "EXE", # flake8-executable
+    "FA",  # flake8-future-annotations
     "ISC", # flake8-implicit-str-concat
     "ICN", # flake8-import-conventions
     "G", # flake8-logging-format
     "INP", # flake8-no-pep420
     "PIE", # flake8-pie
     "T20", # flake8-print
     "PYI", # flake8-pyi
     "PT", # flake8-pytest-style
     "Q", # flake8-quotes
     "RSE", # flake8-raise
     "RET", # flake8-return
     "SLF", # flake8-self
+    "SLOT", # flake8-slots
     "SIM", # flake8-simplify
     "TID", # flake8-tidy-imports
     "TCH", # flake8-type-checking
+    "INT", # flake8-gettext
     "ARG", # flake8-unused-arguments
     "PTH", # flake8-use-pathlib
+    "TD",  # flake8-todos
+    "FIX",  # flake8-fixme
     "ERA", # eradicate
     "PD", # pandas-vet
     "PGH", # pygrep-hooks
     "PL", # Pylint
     "TRY", # tryceratops
+    "FLY",  # flynt
     "NPY", # NumPy-specific rules
+    "AIR", # Airflow
+    "PERF", # Perflint
     "RUF", # Ruff-specific rules
 ]
 ignore = [
     "D203", # one-blank-line-before-class
     "D213", # multi-line-summary-second-line
 ]
```

### Comparing `peprock-1.6.0/PKG-INFO` & `peprock-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peprock
-Version: 1.6.0
+Version: 1.6.1
 Summary: Foundational Python library
 Home-page: https://github.com/Ponte-Energy-Partners/peprock
 License: MIT
 Keywords: peprock,datetime,models,patterns,subclasses
 Author: Jakob Keller
 Author-email: 57402305+jakob-keller@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

