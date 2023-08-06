# Comparing `tmp/cmnemoi_learn-0.1.0.tar.gz` & `tmp/cmnemoi_learn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmnemoi_learn-0.1.0.tar", max compression
+gzip compressed data, was "cmnemoi_learn-0.2.0.tar", max compression
```

## Comparing `cmnemoi_learn-0.1.0.tar` & `cmnemoi_learn-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1085 2023-08-05 21:38:51.404085 cmnemoi_learn-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      917 2023-08-05 21:38:51.404085 cmnemoi_learn-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-05 21:38:51.404085 cmnemoi_learn-0.1.0/cmnemoi_learn/__init__.py
--rw-r--r--   0        0        0     1016 2023-08-05 21:38:51.404085 cmnemoi_learn-0.1.0/cmnemoi_learn/linear_regression.py
--rw-r--r--   0        0        0      555 2023-08-05 21:38:51.404085 cmnemoi_learn-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 cmnemoi_learn-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1090 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/cmnemoi_learn/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/cmnemoi_learn/linear_regression.py
+-rw-r--r--   0        0        0      555 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 cmnemoi_learn-0.2.0/PKG-INFO
```

### Comparing `cmnemoi_learn-0.1.0/LICENSE.md` & `cmnemoi_learn-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmnemoi_learn-0.1.0/README.md` & `cmnemoi_learn-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # cmnemoi-learn - Machine Learning from scratch by Charles-Meldhine Madi Mnemoi
 
 Repository in which I will implement some of the machine learning models described in Elements Of Statistical Learning by Hastie, Tibshirani and Friedman from scratch (using only `numpy`) in form of a Python package.
 
 The implementations will be unit tested against popular implementation (Scikit-learn, PyTorch) with `pytest`.
 The quality of the code will be checked using `black`, `pylint` and `mypy` at each commit through a GitHub Action CI pipeline.
+The package will be published on PyPI at each push to the `main` branch through a GitHub Action CD pipeline.
 
-# Installing
+# Install the package
+
+```bash
+pip install cmnemoi-learn
+```
+
+# Contributing
 
 Clone the repo :
 ```bash
 git clone https://github.com/cmnemoi/cmnemoi-learn.git
 cd cmnemoi-learn
 ```
```

### Comparing `cmnemoi_learn-0.1.0/pyproject.toml` & `cmnemoi_learn-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmnemoi-learn"
-version = "0.1.0"
+version = "0.2.0"
 description = "Machine Learning from scratch by Charles-Meldhine Madi Mnemoi"
 authors = ["Charles-Meldhine Madi Mnemoi <charlesmeldhine.madimnemoi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cmnemoi_learn"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cmnemoi_learn-0.1.0/PKG-INFO` & `cmnemoi_learn-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmnemoi-learn
-Version: 0.1.0
+Version: 0.2.0
 Summary: Machine Learning from scratch by Charles-Meldhine Madi Mnemoi
 License: MIT
 Author: Charles-Meldhine Madi Mnemoi
 Author-email: charlesmeldhine.madimnemoi@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,23 @@
 
 # cmnemoi-learn - Machine Learning from scratch by Charles-Meldhine Madi Mnemoi
 
 Repository in which I will implement some of the machine learning models described in Elements Of Statistical Learning by Hastie, Tibshirani and Friedman from scratch (using only `numpy`) in form of a Python package.
 
 The implementations will be unit tested against popular implementation (Scikit-learn, PyTorch) with `pytest`.
 The quality of the code will be checked using `black`, `pylint` and `mypy` at each commit through a GitHub Action CI pipeline.
+The package will be published on PyPI at each push to the `main` branch through a GitHub Action CD pipeline.
 
-# Installing
+# Install the package
+
+```bash
+pip install cmnemoi-learn
+```
+
+# Contributing
 
 Clone the repo :
 ```bash
 git clone https://github.com/cmnemoi/cmnemoi-learn.git
 cd cmnemoi-learn
 ```
```

