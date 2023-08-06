# Comparing `tmp/cmnemoi_learn-0.2.0.tar.gz` & `tmp/cmnemoi_learn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmnemoi_learn-0.2.0.tar", max compression
+gzip compressed data, was "cmnemoi_learn-0.2.1.tar", max compression
```

## Comparing `cmnemoi_learn-0.2.0.tar` & `cmnemoi_learn-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1085 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1090 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/cmnemoi_learn/__init__.py
--rw-r--r--   0        0        0     1815 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/cmnemoi_learn/linear_regression.py
--rw-r--r--   0        0        0      555 2023-08-06 01:10:01.468937 cmnemoi_learn-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 cmnemoi_learn-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     1604 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/cmnemoi_learn/__init__.py
+-rw-r--r--   0        0        0     1207 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/cmnemoi_learn/abstract_model.py
+-rw-r--r--   0        0        0        0 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/cmnemoi_learn/regression/__init__.py
+-rw-r--r--   0        0        0      773 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/cmnemoi_learn/regression/abstract_regressor.py
+-rw-r--r--   0        0        0     1879 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/cmnemoi_learn/regression/linear_regression.py
+-rw-r--r--   0        0        0      653 2023-08-06 21:21:07.047763 cmnemoi_learn-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 cmnemoi_learn-0.2.1/PKG-INFO
```

### Comparing `cmnemoi_learn-0.2.0/LICENSE.md` & `cmnemoi_learn-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmnemoi_learn-0.2.0/cmnemoi_learn/linear_regression.py` & `cmnemoi_learn-0.2.1/cmnemoi_learn/regression/linear_regression.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """
 File defining a Linear Regression model.
 """
 
 from typing import Self
 import numpy as np
-from numpy.linalg import inv
+from numpy.linalg import pinv
 
+from cmnemoi_learn.regression.abstract_regressor import AbstractRegressor
 
-class LinearRegression:
+
+class LinearRegression(AbstractRegressor):
     """
     Linear Regression model.
     `y = X.theta` where `theta` are the parameters of the model.
     """
 
     def __init__(self) -> None:
-        self.X = np.array([])
-        self.y = np.array([])
+        super().__init__()
         self.theta = np.array([])
 
     def fit(self, X: np.ndarray, y: np.ndarray) -> Self:
         """Fit the Linear Regression model with normal equations solution.
 
-        The optimal parameters `theta` of the model are the ones which minimize 
+        The optimal parameters `theta` of the model are the ones which minimize
         Residuals Sum of Squares : `RSS = Sum(y - X.theta)**2`.
 
         Args:
             X (np.ndarray): Inputs
             y (np.ndarray): Output
 
         Returns:
             LinearRegression: Fitted Linear Regression model.
         """
         self.X = self._get_inputs_with_bias_column(X)
         self.y = y
-        self.theta = inv(self.X.T @ self.X) @ (self.X.T @ self.y)
+
+        self.theta = pinv(self.X.T @ self.X) @ (self.X.T @ self.y)
+
         return self
 
     def predict(self, X: np.ndarray) -> np.ndarray:
         """Predict new values with the Linear Regression model for the inputs given on argument.
 
         Args:
             X (np.ndarray): New inputs on which to predict.
```

### Comparing `cmnemoi_learn-0.2.0/pyproject.toml` & `cmnemoi_learn-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmnemoi-learn"
-version = "0.2.0"
+version = "0.2.1"
 description = "Machine Learning from scratch by Charles-Meldhine Madi Mnemoi"
 authors = ["Charles-Meldhine Madi Mnemoi <charlesmeldhine.madimnemoi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cmnemoi_learn"}]
 
 [tool.poetry.dependencies]
@@ -12,11 +12,15 @@
 numpy = "^1.25.2"
 scikit-learn = "^1.3.0"
 pytest = "^7.4.0"
 jupyter = "^1.0.0"
 black = "^23.7.0"
 pylint = "^2.17.5"
 mypy = "^1.4.1"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[project.urls]
+Repository = "https://github.com/cmnemoi/cmnemoi-learn.git"
```

### Comparing `cmnemoi_learn-0.2.0/PKG-INFO` & `cmnemoi_learn-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: cmnemoi-learn
-Version: 0.2.0
+Version: 0.2.1
 Summary: Machine Learning from scratch by Charles-Meldhine Madi Mnemoi
 License: MIT
 Author: Charles-Meldhine Madi Mnemoi
 Author-email: charlesmeldhine.madimnemoi@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.7.0,<24.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: pylint (>=2.17.5,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmnemoi-learn - Machine Learning from scratch by Charles-Meldhine Madi Mnemoi
 
+![CI Status](https://github.com/cmnemoi/cmnemoi-learn/actions/workflows/continous_integration.yaml/badge.svg?branch=main)
+![CD Status](https://github.com/cmnemoi/cmnemoi-learn/actions/workflows/create_github_release.yaml/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/cmnemoi/cmnemoi-learn/badge.svg?branch=main)](https://coveralls.io/github/cmnemoi/cmnemoi-learn?branch=main) 
+[![PyPI version](https://badge.fury.io/py/cmnemoi-learn.svg)](https://badge.fury.io/py/cmnemoi-learn) 
+
 Repository in which I will implement some of the machine learning models described in Elements Of Statistical Learning by Hastie, Tibshirani and Friedman from scratch (using only `numpy`) in form of a Python package.
 
 The implementations will be unit tested against popular implementation (Scikit-learn, PyTorch) with `pytest`.
+
 The quality of the code will be checked using `black`, `pylint` and `mypy` at each commit through a GitHub Action CI pipeline.
+
 The package will be published on PyPI at each push to the `main` branch through a GitHub Action CD pipeline.
 
 # Install the package
 
 ```bash
 pip install cmnemoi-learn
 ```
```

