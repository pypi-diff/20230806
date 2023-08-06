# Comparing `tmp/python2verilog-0.0.4.tar.gz` & `tmp/python2verilog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python2verilog-0.0.4.tar", last modified: Wed Jul 26 23:04:16 2023, max compression
+gzip compressed data, was "python2verilog-0.1.0.tar", last modified: Sun Aug  6 19:57:27 2023, max compression
```

## Comparing `python2verilog-0.0.4.tar` & `python2verilog-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.900687 python2verilog-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 23:04:16.900687 python2verilog-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-26 23:04:05.000000 python2verilog-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-26 23:04:05.000000 python2verilog-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/backend/verilog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/generator2graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/frontend/generator_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/ir/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/ir/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.896687 python2verilog-0.0.4/python2verilog/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.900687 python2verilog-0.0.4/python2verilog/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-26 23:04:05.000000 python2verilog-0.0.4/python2verilog/utils/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:04:16.892687 python2verilog-0.0.4/python2verilog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 23:04:16.000000 python2verilog-0.0.4/python2verilog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:04:16.900687 python2verilog-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:57:27.766492 python2verilog-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 19:57:27.766492 python2verilog-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-08-06 19:57:17.000000 python2verilog-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 19:57:17.000000 python2verilog-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:57:27.766492 python2verilog-0.1.0/python2verilog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-06 19:57:27.000000 python2verilog-0.1.0/python2verilog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:57:27.766492 python2verilog-0.1.0/setup.cfg
```

### Comparing `python2verilog-0.0.4/PKG-INFO` & `python2verilog-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,116 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.4
+Version: 0.1.0
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
-![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+[![pypi](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)](https://pypi.org/project/python2verilog/)
+![py versions](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2FWorldofKerry%2FPython2Verilog%2Fmain%2F.github%2Fworkflows%2Fpytest.yml&query=%24.jobs.build.strategy.matrix%5B%22python-version%22%5D&label=python%20versions)
+[![pypi downloads](https://img.shields.io/pypi/dm/python2verilog)](https://pypi.org/project/python2verilog/)
+[![pytest](https://github.com/worldofkerry/python2verilog/actions/workflows/pytest.yml/badge.svg)](https://github.com/WorldofKerry/Python2Verilog/actions/workflows/pytest.yml)
+[![docs](https://github.com/worldofkerry/python2verilog/actions/workflows/sphinx.yml/badge.svg)](https://worldofkerry.github.io/Python2Verilog/)
 
-# Python 2 Verilog
+# python2verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench can also be generated and asserted against the Python outputs.
-
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
 
-**Warning**: Variables are treated as global and therefore no variable shadowing.
+A testbench can also be generated and asserted against the Python outputs.
+
+## Usage
 
-## Sample Usage
-`pip install python2verilog`
+`python3 -m pip install --upgrade pip`
+`python3 -m pip install python2verilog`
 
-### Basic Usage
-Create a python file containing a generator function with output type hints, named `<name>.py`.
+### Basics
 
-A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
+Create a python file containing a generator function with output type hints, named `python.py`.
 
-`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
+You can find a sample [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/happy_face/python.py), and a directory of samples [here](https://github.com/WorldofKerry/Python2Verilog/tree/main/tests/integration/data)
+
+Run `python3 -m python2verilog python.py` to generate a testbench file at `python.sv`.
+
+Use the arg `--help` for additional options, including outputting a testbench and running optimizers.
 
 ## Testing
 
 ### Requirements
 
-Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used for speed)
+
+Install required python libraries with `python3 -m pip install -r tests/requirements.txt`
+
+For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
+`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
 
-Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
-Python Libraries: `python3 -m pip install -r tests/requirements.txt`
+For most up-to-date information, refer to the pytest [github workflow](.github/workflows/python-package.yml).
 
 ### Creating New Test
 
 To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
-To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/integration/data/integration/<test-name>/`.
+To run tests, use `python3 -m pytest -sv`.
+
+Additional CLI flags can be found in [tests/conftest.py](tests/conftest.py).
 
 ## Tested Generations
 
-Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
+The Github Actions run all the tests with writing enabled.
+You may find its output as a [Github Artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/pytest/main/tests-data.zip).
 
 ## For Developers
 
-Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
-
-Architecture is based on [LLVM](https://llvm.org/).
-
 To setup pre-commit, run `pre-commit install`.
 
+[Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) is used for tracking.
+
 ### Epics
 
-- Support arrays
+- Support arrays (and their unrolling)
 - Mimic combinational logic with "regular" Python functions
-- Division approximations
+- Division approximations (and area/timing analysis)
 
 ## Docs
 
-- cd to `docs/`
-- `sphinx-apidoc -o . ../python2verilog/`
-- `make html`
+Uses sphinx.
+Run commands used by [Github Actions](.github/workflows/sphinx.yml).
 
 ## Random Planning, Design, and Notes
 
-## What needs to be duplicated in testbenches?
+### What needs to be duplicated in testbenches?
+
 declare I/O and other signals
 declare DUT
 start clock
 
 loop for each test case
+
 - start signal
 - while wait for done signal
   - clock
   - set start zero
   - display output
-endloop
-
+    endloop
 
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
```

### Comparing `python2verilog-0.0.4/README.md` & `python2verilog-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,104 @@
-![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
-![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+[![pypi](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)](https://pypi.org/project/python2verilog/)
+![py versions](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2FWorldofKerry%2FPython2Verilog%2Fmain%2F.github%2Fworkflows%2Fpytest.yml&query=%24.jobs.build.strategy.matrix%5B%22python-version%22%5D&label=python%20versions)
+[![pypi downloads](https://img.shields.io/pypi/dm/python2verilog)](https://pypi.org/project/python2verilog/)
+[![pytest](https://github.com/worldofkerry/python2verilog/actions/workflows/pytest.yml/badge.svg)](https://github.com/WorldofKerry/Python2Verilog/actions/workflows/pytest.yml)
+[![docs](https://github.com/worldofkerry/python2verilog/actions/workflows/sphinx.yml/badge.svg)](https://worldofkerry.github.io/Python2Verilog/)
 
-# Python 2 Verilog
+# python2verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench can also be generated and asserted against the Python outputs.
-
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
 
-**Warning**: Variables are treated as global and therefore no variable shadowing.
+A testbench can also be generated and asserted against the Python outputs.
+
+## Usage
 
-## Sample Usage
-`pip install python2verilog`
+`python3 -m pip install --upgrade pip`
+`python3 -m pip install python2verilog`
 
-### Basic Usage
-Create a python file containing a generator function with output type hints, named `<name>.py`.
+### Basics
 
-A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
+Create a python file containing a generator function with output type hints, named `python.py`.
 
-`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
+You can find a sample [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/happy_face/python.py), and a directory of samples [here](https://github.com/WorldofKerry/Python2Verilog/tree/main/tests/integration/data)
+
+Run `python3 -m python2verilog python.py` to generate a testbench file at `python.sv`.
+
+Use the arg `--help` for additional options, including outputting a testbench and running optimizers.
 
 ## Testing
 
 ### Requirements
 
-Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used for speed)
+
+Install required python libraries with `python3 -m pip install -r tests/requirements.txt`
+
+For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
+`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
 
-Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
-Python Libraries: `python3 -m pip install -r tests/requirements.txt`
+For most up-to-date information, refer to the pytest [github workflow](.github/workflows/python-package.yml).
 
 ### Creating New Test
 
 To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
-To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/integration/data/integration/<test-name>/`.
+To run tests, use `python3 -m pytest -sv`.
+
+Additional CLI flags can be found in [tests/conftest.py](tests/conftest.py).
 
 ## Tested Generations
 
-Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
+The Github Actions run all the tests with writing enabled.
+You may find its output as a [Github Artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/pytest/main/tests-data.zip).
 
 ## For Developers
 
-Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
-
-Architecture is based on [LLVM](https://llvm.org/).
-
 To setup pre-commit, run `pre-commit install`.
 
+[Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) is used for tracking.
+
 ### Epics
 
-- Support arrays
+- Support arrays (and their unrolling)
 - Mimic combinational logic with "regular" Python functions
-- Division approximations
+- Division approximations (and area/timing analysis)
 
 ## Docs
 
-- cd to `docs/`
-- `sphinx-apidoc -o . ../python2verilog/`
-- `make html`
+Uses sphinx.
+Run commands used by [Github Actions](.github/workflows/sphinx.yml).
 
 ## Random Planning, Design, and Notes
 
-## What needs to be duplicated in testbenches?
+### What needs to be duplicated in testbenches?
+
 declare I/O and other signals
 declare DUT
 start clock
 
 loop for each test case
+
 - start signal
 - while wait for done signal
   - clock
   - set start zero
   - display output
-endloop
-
+    endloop
 
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
```

### Comparing `python2verilog-0.0.4/pyproject.toml` & `python2verilog-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [project]
 name = "python2verilog"
-version = "0.0.4"
+version = "0.1.0"
 authors = [{ name = "Kerry Wang", email = "kerrywang369@gmail.com" }]
 description = "Converts a subset of python generator functions into synthesizable sequential SystemVerilog"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/WorldofKerry/Python2Verilog/"
 "Bug Tracker" = "https://github.com/WorldofKerry/Python2Verilog/issues"
 
-[[tool.mypy.overrides]]
-module = ["matplotlib", "matplotlib.pyplot"]
-ignore_missing_imports = true
+[tool.setuptools]
+"py-modules" = ["python2verilog"]
```

### Comparing `python2verilog-0.0.4/python2verilog.egg-info/PKG-INFO` & `python2verilog-0.1.0/python2verilog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,116 @@
 Metadata-Version: 2.1
 Name: python2verilog
-Version: 0.0.4
+Version: 0.1.0
 Summary: Converts a subset of python generator functions into synthesizable sequential SystemVerilog
 Author-email: Kerry Wang <kerrywang369@gmail.com>
 Project-URL: Homepage, https://github.com/WorldofKerry/Python2Verilog/
 Project-URL: Bug Tracker, https://github.com/WorldofKerry/Python2Verilog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-![Python Package](https://github.com/worldofkerry/python2verilog/actions/workflows/python-package.yml/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/python2verilog/badge/?version=latest)](https://python2verilog.readthedocs.io/en/latest/?badge=latest)
-![PyPI](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/python2verilog)
+[![pypi](https://img.shields.io/pypi/v/python2verilog?label=pypi%20package)](https://pypi.org/project/python2verilog/)
+![py versions](https://img.shields.io/badge/dynamic/yaml?url=https%3A%2F%2Fraw.githubusercontent.com%2FWorldofKerry%2FPython2Verilog%2Fmain%2F.github%2Fworkflows%2Fpytest.yml&query=%24.jobs.build.strategy.matrix%5B%22python-version%22%5D&label=python%20versions)
+[![pypi downloads](https://img.shields.io/pypi/dm/python2verilog)](https://pypi.org/project/python2verilog/)
+[![pytest](https://github.com/worldofkerry/python2verilog/actions/workflows/pytest.yml/badge.svg)](https://github.com/WorldofKerry/Python2Verilog/actions/workflows/pytest.yml)
+[![docs](https://github.com/worldofkerry/python2verilog/actions/workflows/sphinx.yml/badge.svg)](https://worldofkerry.github.io/Python2Verilog/)
 
-# Python 2 Verilog
+# python2verilog
 
 Converts a subset of python generator functions into synthesizable sequential SystemVerilog.
 
 A use case is for drawing shapes on grids (for VGA output), where the user may prototype the algorithm in python and then convert it to verilog for use in an FPGA.
 
-A testbench can also be generated and asserted against the Python outputs.
-
 Supports Python [Generator functions](https://wiki.python.org/moin/Generators) as well as the following block types:
 
 - `if`
 - `while`
 
-**Warning**: Variables are treated as global and therefore no variable shadowing.
+A testbench can also be generated and asserted against the Python outputs.
+
+## Usage
 
-## Sample Usage
-`pip install python2verilog`
+`python3 -m pip install --upgrade pip`
+`python3 -m pip install python2verilog`
 
-### Basic Usage
-Create a python file containing a generator function with output type hints, named `<name>.py`.
+### Basics
 
-A sample can be found [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/integration/circle_lines/python.py)
+Create a python file containing a generator function with output type hints, named `python.py`.
 
-`python3 -m python2verilog.convert <name>.py`. Use `--help` for additional options, including outputting a testbench.
+You can find a sample [here](https://github.com/WorldofKerry/Python2Verilog/blob/main/tests/integration/data/happy_face/python.py), and a directory of samples [here](https://github.com/WorldofKerry/Python2Verilog/tree/main/tests/integration/data)
+
+Run `python3 -m python2verilog python.py` to generate a testbench file at `python.sv`.
+
+Use the arg `--help` for additional options, including outputting a testbench and running optimizers.
 
 ## Testing
 
 ### Requirements
 
-Warning: may be outdated, refer to [github workflow](.github/workflows/python-package.yml) for most update-to-date information for Ubuntu.
+A Ubuntu environment (WSL2 works too, make sure to have the repo on the Ubuntu partition, as [`os.mkfifo`](https://docs.python.org/3/library/os.html#os.mkfifo) is used for speed)
+
+Install required python libraries with `python3 -m pip install -r tests/requirements.txt`
+
+For automatic Verilog simulation and testing, install [Icarus Verilog](https://github.com/steveicarus/iverilog) and its dependencies with
+`sudo apt-get install iverilog expected` (uses the `unbuffer` in `expected`).
 
-Verilog simulation: `sudo apt-get install iverilog expected` (uses the `unbuffer` app in `expected`). The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute, given that you paste the output into the "actual file" specified in the `config.ini` of the test.
+The online simulator [EDA Playground](https://edaplayground.com/) can be used as a subsitute if you manually copy-paste the module and testbench files to it.
 
-Python Libraries: `python3 -m pip install -r tests/requirements.txt`
+For most up-to-date information, refer to the pytest [github workflow](.github/workflows/python-package.yml).
 
 ### Creating New Test
 
 To create a new test case and set up configs, run `python3 tests/integration/new_test_case.py <test-name>`.
 
 ### Running Tests
 
-To run tests, use `python3 -m pytest --verbose` to generate the module, testbench, visualizations, dumps, and expected/actual outputs.
-Those files will be stored in `tests/integration/data/integration/<test-name>/`.
+To run tests, use `python3 -m pytest -sv`.
+
+Additional CLI flags can be found in [tests/conftest.py](tests/conftest.py).
 
 ## Tested Generations
 
-Outputs of tests in repo can be found as a [github workflow artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/python-package/main/tests-data.zip)
+The Github Actions run all the tests with writing enabled.
+You may find its output as a [Github Artifact](https://nightly.link/WorldofKerry/Python2Verilog/workflows/pytest/main/tests-data.zip).
 
 ## For Developers
 
-Based on my experimentation with a [C to Verilog converter](https://github.com/WorldofKerry/c2hdl).
-
-Architecture is based on [LLVM](https://llvm.org/).
-
 To setup pre-commit, run `pre-commit install`.
 
+[Github Issues](https://github.com/WorldofKerry/Python2Verilog/issues) is used for tracking.
+
 ### Epics
 
-- Support arrays
+- Support arrays (and their unrolling)
 - Mimic combinational logic with "regular" Python functions
-- Division approximations
+- Division approximations (and area/timing analysis)
 
 ## Docs
 
-- cd to `docs/`
-- `sphinx-apidoc -o . ../python2verilog/`
-- `make html`
+Uses sphinx.
+Run commands used by [Github Actions](.github/workflows/sphinx.yml).
 
 ## Random Planning, Design, and Notes
 
-## What needs to be duplicated in testbenches?
+### What needs to be duplicated in testbenches?
+
 declare I/O and other signals
 declare DUT
 start clock
 
 loop for each test case
+
 - start signal
 - while wait for done signal
   - clock
   - set start zero
   - display output
-endloop
-
+    endloop
 
 ### Potential API
 
 ```python
 import python2verilog as p2v
 import ast
```

