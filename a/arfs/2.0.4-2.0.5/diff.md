# Comparing `tmp/arfs-2.0.4.tar.gz` & `tmp/arfs-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arfs-2.0.4.tar", last modified: Wed Aug  2 19:55:11 2023, max compression
+gzip compressed data, was "arfs-2.0.5.tar", last modified: Sat Aug  5 22:07:15 2023, max compression
```

## Comparing `arfs-2.0.4.tar` & `arfs-2.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.885490 arfs-2.0.4/
--rw-rw-rw-   0        0        0     1091 2020-11-27 22:01:34.000000 arfs-2.0.4/LICENSE.md
--rw-rw-rw-   0        0        0    11944 2023-08-02 19:55:11.892488 arfs-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    11254 2023-07-31 13:58:34.000000 arfs-2.0.4/README.md
--rw-rw-rw-   0        0        0       82 2023-01-04 17:12:37.000000 arfs-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1386 2023-08-02 19:55:11.924489 arfs-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.190488 arfs-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.402520 arfs-2.0.4/src/arfs/
--rw-rw-rw-   0        0        0       92 2023-08-02 12:18:39.000000 arfs-2.0.4/src/arfs/__init__.py
--rw-rw-rw-   0        0        0    87156 2023-08-02 12:10:26.000000 arfs-2.0.4/src/arfs/association.py
--rw-rw-rw-   0        0        0     6829 2023-07-31 13:45:23.000000 arfs-2.0.4/src/arfs/benchmark.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.193487 arfs-2.0.4/src/arfs/dataset/
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.587488 arfs-2.0.4/src/arfs/dataset/data/
--rw-rw-rw-   0        0        0    77321 2023-01-06 14:48:50.000000 arfs-2.0.4/src/arfs/dataset/data/boston_bunch.joblib
--rw-rw-rw-   0        0        0   645468 2021-03-16 17:57:09.000000 arfs-2.0.4/src/arfs/dataset/data/housing.zip
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.769494 arfs-2.0.4/src/arfs/feature_selection/
--rw-rw-rw-   0        0        0      711 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0    96674 2023-08-02 12:14:27.000000 arfs-2.0.4/src/arfs/feature_selection/allrelevant.py
--rw-rw-rw-   0        0        0     5398 2023-07-31 13:36:41.000000 arfs-2.0.4/src/arfs/feature_selection/base.py
--rw-rw-rw-   0        0        0    22557 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/feature_selection/lasso.py
--rw-rw-rw-   0        0        0    13812 2023-07-31 13:37:06.000000 arfs-2.0.4/src/arfs/feature_selection/mrmr.py
--rw-rw-rw-   0        0        0     2473 2023-07-31 13:38:21.000000 arfs-2.0.4/src/arfs/feature_selection/summary.py
--rw-rw-rw-   0        0        0    16052 2023-07-31 13:40:30.000000 arfs-2.0.4/src/arfs/feature_selection/unsupervised.py
--rw-rw-rw-   0        0        0    15889 2023-07-31 13:42:08.000000 arfs-2.0.4/src/arfs/feature_selection/variable_importance.py
--rw-rw-rw-   0        0        0    21997 2023-07-31 13:49:08.000000 arfs-2.0.4/src/arfs/gbm.py
--rw-rw-rw-   0        0        0     5788 2023-08-02 08:27:06.000000 arfs-2.0.4/src/arfs/parallel.py
--rw-rw-rw-   0        0        0    38523 2023-08-02 12:10:25.000000 arfs-2.0.4/src/arfs/preprocessing.py
--rw-rw-rw-   0        0        0    15511 2023-07-31 13:53:23.000000 arfs-2.0.4/src/arfs/sampling.py
--rw-rw-rw-   0        0        0    25361 2023-07-31 13:53:40.000000 arfs-2.0.4/src/arfs/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.554489 arfs-2.0.4/src/arfs.egg-info/
--rw-rw-rw-   0        0        0    11944 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-04 17:19:39.000000 arfs-2.0.4/src/arfs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      362 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-02 19:55:11.000000 arfs-2.0.4/src/arfs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 19:55:11.805487 arfs-2.0.4/tests/
--rw-rw-rw-   0        0        0    10887 2023-05-15 12:20:31.000000 arfs-2.0.4/tests/test_allrelevant.py
--rw-rw-rw-   0        0        0    19605 2023-05-21 19:11:19.000000 arfs-2.0.4/tests/test_featselect.py
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.887258 arfs-2.0.5/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     1071 2023-05-08 18:32:07.000000 arfs-2.0.5/LICENSE.md
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    11798 2023-08-05 22:07:15.887258 arfs-2.0.5/PKG-INFO
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    11127 2023-08-05 17:05:12.000000 arfs-2.0.5/README.md
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)       80 2023-05-08 18:32:08.000000 arfs-2.0.5/pyproject.toml
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     1320 2023-08-05 22:07:15.891258 arfs-2.0.5/setup.cfg
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.855259 arfs-2.0.5/src/
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.867259 arfs-2.0.5/src/arfs/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)       88 2023-08-05 20:30:42.000000 arfs-2.0.5/src/arfs/__init__.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    84688 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/association.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     6639 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/benchmark.py
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.855259 arfs-2.0.5/src/arfs/dataset/
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.871259 arfs-2.0.5/src/arfs/dataset/data/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    77321 2023-05-08 18:32:08.000000 arfs-2.0.5/src/arfs/dataset/data/boston_bunch.joblib
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)   645468 2023-05-08 18:32:08.000000 arfs-2.0.5/src/arfs/dataset/data/housing.zip
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.883258 arfs-2.0.5/src/arfs/feature_selection/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      684 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/__init__.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    94060 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/allrelevant.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     5228 2023-08-05 20:09:36.000000 arfs-2.0.5/src/arfs/feature_selection/base.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    21930 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/lasso.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    13466 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/mrmr.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     2400 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/summary.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    15600 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/feature_selection/unsupervised.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    15596 2023-08-05 18:10:07.000000 arfs-2.0.5/src/arfs/feature_selection/variable_importance.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    21243 2023-08-05 20:24:10.000000 arfs-2.0.5/src/arfs/gbm.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)     5617 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/parallel.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    37504 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/preprocessing.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    15034 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/sampling.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    24489 2023-08-05 17:05:12.000000 arfs-2.0.5/src/arfs/utils.py
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.871259 arfs-2.0.5/src/arfs.egg-info/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    11798 2023-08-05 22:07:15.000000 arfs-2.0.5/src/arfs.egg-info/PKG-INFO
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      849 2023-08-05 22:07:15.000000 arfs-2.0.5/src/arfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)        1 2023-08-05 22:07:15.000000 arfs-2.0.5/src/arfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)        1 2023-05-08 18:35:39.000000 arfs-2.0.5/src/arfs.egg-info/not-zip-safe
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)      362 2023-08-05 22:07:15.000000 arfs-2.0.5/src/arfs.egg-info/requires.txt
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)        5 2023-08-05 22:07:15.000000 arfs-2.0.5/src/arfs.egg-info/top_level.txt
+drwxrwxr-x   0 bsatom    (1000) bsatom    (1000)        0 2023-08-05 22:07:15.887258 arfs-2.0.5/tests/
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    10620 2023-05-17 14:18:47.000000 arfs-2.0.5/tests/test_allrelevant.py
+-rw-rw-r--   0 bsatom    (1000) bsatom    (1000)    19261 2023-05-17 14:18:47.000000 arfs-2.0.5/tests/test_featselect.py
```

### Comparing `arfs-2.0.4/LICENSE.md` & `arfs-2.0.5/LICENSE.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [2020] [Thomas Bury]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [2020] [Thomas Bury]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `arfs-2.0.4/PKG-INFO` & `arfs-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: arfs
-Version: 2.0.4
-Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
-Author: ThomasBury
-Author-email: bury.thomas@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/ThomasBury/arfs
-Project-URL: Source, https://github.com/ThomasBury/arfs
-Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
-Project-URL: Download, https://pypi.org/project/arfs/
-Keywords: feature-selection,all-relevant,selection,MRmr
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE.md
-
-<img src="logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
-
-
-[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
-
-# All relevant feature selection
-
-All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
-
-This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
-
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
-
-Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
-
-## Installation
-
-`$ pip install arfs`
-
-## Example
-
-Working examples for:
-
- - [Preprocessing](./docs/notebooks/preprocessingipynb)
- - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
- - [Regression](./docs/notebooks/arfs_regression.ipynb)
- - [Classification](./docs/notebooks/arfs_classification.ipynb)
- - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
- - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
- - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
- - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
- - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
- - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
- - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
- - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
- - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
- - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
- - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
-
-For imbalanced classification:
- - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
- - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
-
-
-
-## Boruta
-
-The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
-
- * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
- * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
- * Combine the original ones with shuffled copies
- * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
- * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
- * Find the maximum Z score among shadow attributes (MZSA)
- * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
- * Tag the variables as 'important' when they have importance significantly higher than MZSA.
- * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
-
-At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-
-## BoostARoota
-
-BoostARoota follows closely the Boruta method but modifies a few things:
-
- * One-Hot-Encode the feature set
- * Double width of the data set, making a copy of all features in the original dataset
- * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
- * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
- * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
- * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
- * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
- * Go back to (2) until the number of features removed is less than ten per cent of the total.
- * Method returns the features remaining once completed.
-
-In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-## Modifications to Boruta and BoostARoota
-
- I forked both Boruta and BoostARoota and made the following changes (under PR):
-
-**Boruta --> Leshy**:
-
-  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
-  - Using lightGBM as the default speeds up by an order of magnitude the running time
-  - Work with Catboost, sklearn API
-  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
-  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
-
-**BoostARoota --> BoostAGroota**:
-
-  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
-  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
-  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
-  - Work with sample_weight, for Poisson or any application requiring a weighting.
-
-## GrootCV, a new method
-
-**New: GrootCV**:
-
-  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
-  - the feature importance is derived using SHAP importance
-  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
-  - Not based on a given percentage of cols needed to be deleted
-  - Plot method for var. imp
-
-
-## References
-
-**Theory**
-
- - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
- - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
-
-**Applications**
-
- - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
- - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
- - [BoostARoota](https://github.com/chasedehan/BoostARoota)
-
-
-
+Metadata-Version: 2.1
+Name: arfs
+Version: 2.0.5
+Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
+Author: ThomasBury
+Author-email: bury.thomas@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/ThomasBury/arfs
+Project-URL: Source, https://github.com/ThomasBury/arfs
+Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
+Project-URL: Download, https://pypi.org/project/arfs/
+Keywords: feature-selection,all-relevant,selection,MRmr
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE.md
+
+<img src="logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
+
+
+[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
+
+# All relevant feature selection
+
+All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
+
+This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
+
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
+
+## Installation
+
+`$ pip install arfs`
+
+## Example
+
+Working examples for:
+
+ - [Preprocessing](./docs/notebooks/preprocessingipynb)
+ - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
+ - [Regression](./docs/notebooks/arfs_regression.ipynb)
+ - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
+ - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
+ - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
+ - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
+ - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
+ - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
+ - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
+
+For imbalanced classification:
+ - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
+ - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
+
+
+
+## Boruta
+
+The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
+
+ * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
+ * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
+ * Combine the original ones with shuffled copies
+ * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
+ * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
+ * Find the maximum Z score among shadow attributes (MZSA)
+ * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
+ * Tag the variables as 'important' when they have importance significantly higher than MZSA.
+ * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
+
+At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+
+## BoostARoota
+
+BoostARoota follows closely the Boruta method but modifies a few things:
+
+ * One-Hot-Encode the feature set
+ * Double width of the data set, making a copy of all features in the original dataset
+ * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
+ * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
+ * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
+ * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
+ * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
+ * Go back to (2) until the number of features removed is less than ten per cent of the total.
+ * Method returns the features remaining once completed.
+
+In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+## Modifications to Boruta and BoostARoota
+
+ I forked both Boruta and BoostARoota and made the following changes (under PR):
+
+**Boruta --> Leshy**:
+
+  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
+  - Using lightGBM as the default speeds up by an order of magnitude the running time
+  - Work with Catboost, sklearn API
+  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
+  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
+
+**BoostARoota --> BoostAGroota**:
+
+  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
+  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
+  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
+  - Work with sample_weight, for Poisson or any application requiring a weighting.
+
+## GrootCV, a new method
+
+**New: GrootCV**:
+
+  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
+  - the feature importance is derived using SHAP importance
+  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
+  - Not based on a given percentage of cols needed to be deleted
+  - Plot method for var. imp
+
+
+## References
+
+**Theory**
+
+ - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
+ - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
+
+**Applications**
+
+ - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
+ - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
+ - [BoostARoota](https://github.com/chasedehan/BoostARoota)
+
+
+
```

### Comparing `arfs-2.0.4/README.md` & `arfs-2.0.5/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-<img src="logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
-
-
-[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
-
-# All relevant feature selection
-
-All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
-
-This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
-
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
-
-Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
-
-## Installation
-
-`$ pip install arfs`
-
-## Example
-
-Working examples for:
-
- - [Preprocessing](./docs/notebooks/preprocessingipynb)
- - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
- - [Regression](./docs/notebooks/arfs_regression.ipynb)
- - [Classification](./docs/notebooks/arfs_classification.ipynb)
- - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
- - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
- - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
- - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
- - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
- - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
- - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
- - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
- - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
- - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
- - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
-
-For imbalanced classification:
- - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
- - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
-
-
-
-## Boruta
-
-The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
-
- * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
- * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
- * Combine the original ones with shuffled copies
- * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
- * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
- * Find the maximum Z score among shadow attributes (MZSA)
- * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
- * Tag the variables as 'important' when they have importance significantly higher than MZSA.
- * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
-
-At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-
-## BoostARoota
-
-BoostARoota follows closely the Boruta method but modifies a few things:
-
- * One-Hot-Encode the feature set
- * Double width of the data set, making a copy of all features in the original dataset
- * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
- * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
- * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
- * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
- * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
- * Go back to (2) until the number of features removed is less than ten per cent of the total.
- * Method returns the features remaining once completed.
-
-In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-## Modifications to Boruta and BoostARoota
-
- I forked both Boruta and BoostARoota and made the following changes (under PR):
-
-**Boruta --> Leshy**:
-
-  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
-  - Using lightGBM as the default speeds up by an order of magnitude the running time
-  - Work with Catboost, sklearn API
-  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
-  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
-
-**BoostARoota --> BoostAGroota**:
-
-  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
-  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
-  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
-  - Work with sample_weight, for Poisson or any application requiring a weighting.
-
-## GrootCV, a new method
-
-**New: GrootCV**:
-
-  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
-  - the feature importance is derived using SHAP importance
-  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
-  - Not based on a given percentage of cols needed to be deleted
-  - Plot method for var. imp
-
-
-## References
-
-**Theory**
-
- - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
- - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
-
-**Applications**
-
- - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
- - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
- - [BoostARoota](https://github.com/chasedehan/BoostARoota)
-
-
-
+<img src="logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
+
+
+[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
+
+# All relevant feature selection
+
+All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
+
+This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
+
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
+
+## Installation
+
+`$ pip install arfs`
+
+## Example
+
+Working examples for:
+
+ - [Preprocessing](./docs/notebooks/preprocessingipynb)
+ - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
+ - [Regression](./docs/notebooks/arfs_regression.ipynb)
+ - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
+ - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
+ - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
+ - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
+ - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
+ - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
+ - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
+
+For imbalanced classification:
+ - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
+ - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
+
+
+
+## Boruta
+
+The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
+
+ * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
+ * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
+ * Combine the original ones with shuffled copies
+ * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
+ * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
+ * Find the maximum Z score among shadow attributes (MZSA)
+ * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
+ * Tag the variables as 'important' when they have importance significantly higher than MZSA.
+ * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
+
+At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+
+## BoostARoota
+
+BoostARoota follows closely the Boruta method but modifies a few things:
+
+ * One-Hot-Encode the feature set
+ * Double width of the data set, making a copy of all features in the original dataset
+ * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
+ * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
+ * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
+ * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
+ * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
+ * Go back to (2) until the number of features removed is less than ten per cent of the total.
+ * Method returns the features remaining once completed.
+
+In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+## Modifications to Boruta and BoostARoota
+
+ I forked both Boruta and BoostARoota and made the following changes (under PR):
+
+**Boruta --> Leshy**:
+
+  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
+  - Using lightGBM as the default speeds up by an order of magnitude the running time
+  - Work with Catboost, sklearn API
+  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
+  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
+
+**BoostARoota --> BoostAGroota**:
+
+  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
+  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
+  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
+  - Work with sample_weight, for Poisson or any application requiring a weighting.
+
+## GrootCV, a new method
+
+**New: GrootCV**:
+
+  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
+  - the feature importance is derived using SHAP importance
+  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
+  - Not based on a given percentage of cols needed to be deleted
+  - Plot method for var. imp
+
+
+## References
+
+**Theory**
+
+ - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
+ - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
+
+**Applications**
+
+ - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
+ - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
+ - [BoostARoota](https://github.com/chasedehan/BoostARoota)
+
+
+
```

### Comparing `arfs-2.0.4/src/arfs/association.py` & `arfs-2.0.5/src/arfs/association.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,2468 +1,2468 @@
-""" Parallelized Association and Correlation matrix
- 
-This module provides parallelized methods for computing associations.
-Namely, correlation, correlation ratio, Theil's U, Cramer's V
-
-They are the basis of the MRmr feature selection
-"""
-
-import math
-import warnings
-import matplotlib
-import numpy as np
-import gc
-import pandas as pd
-import scipy.stats as ss
-import matplotlib.pyplot as plt
-import scipy.cluster.hierarchy as sch
-import scipy.stats as ss
-
-
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-from sklearn.utils import as_float_array, safe_sqr, safe_mask
-from multiprocessing import cpu_count
-from itertools import combinations, permutations, product
-from pandas.api.types import is_numeric_dtype
-from scipy.stats import rankdata
-from functools import partial
-
-from .parallel import (
-    parallel_matrix_entries,
-    parallel_df,
-    _compute_series,
-    _compute_matrix_entries,
-)
-from .utils import create_dtype_dict
-
-_PRECISION = 1e-13
-
-########################
-# Redundancy measures
-########################
-
-# For computing the redundancy of all the columns with a given series
-# R(y, x_i) for i=1,..., N --> a series (y is a fixed, chosen column)
-# the main functions are:
-# - the series-series computation (two columns)
-# - the closure for applying the latter function to all columns of a dataframe
-# - the "series" version, using the closure for computing the redundancy with all the cols of the DF
-#
-# For computing the redundancy matrix all the cols combinations of columns
-# R(x_i, x_j) for i, j=1,..., N --> a data frame (either TRIUL if the measure is symmetric
-# or the full matrix if asymmetric)
-# - the series-series computation (two columns), same as for series case
-# - the function looping over a chunk of combinations
-# - the parallelization (sending different chunks to different cores and applying the latter function)
-
-##################
-# CAT-CAT
-##################
-
-
-def weighted_conditional_entropy(x, y, sample_weight=None):
-    """weighted_conditional_entropy computes the weighted conditional entropy between two
-    categorical predictors.
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The predictor vector
-    y : pd.Series of shape (n_samples,)
-        The target vector
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-
-    Returns
-    -------
-    float
-        weighted conditional entropy
-    """
-
-    if sample_weight is None:
-        sample_weight = np.ones(len(x))
-    elif np.count_nonzero(sample_weight) == 0:
-        raise ValueError(
-            "All elements in sample_weight are zero. Cannot divide by zero."
-        )
-
-    df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
-    tot_weight = df["sample_weight"].sum()
-    y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
-    y_counter = y_counter["sample_weight"]
-    xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
-    xy_counter = xy_counter["sample_weight"]
-    h_xy = 0.0
-    for xy in xy_counter.keys():
-        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
-        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
-        if p_xy != 0:
-            h_xy += p_xy * math.log(p_y / p_xy, math.e)
-    return h_xy
-
-
-def weighted_theils_u(x, y, sample_weight=None, as_frame=False):
-    """weighted_theils_u computes the weighted Theil's U statistic between two
-    categorical predictors.
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The predictor vector
-    y : pd.Series of shape (n_samples,)
-        The target vector
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-
-    Returns
-    -------
-    pd.DataFrame
-        predictor names and value of the Theil's U statistic
-    """
-
-    if sample_weight is None:
-        sample_weight = np.ones(len(x))
-
-    df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
-    tot_weight = df["sample_weight"].sum()
-    y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
-    y_counter = y_counter["sample_weight"]
-    x_counter = df[["x", "sample_weight"]].groupby("x").sum().to_dict()
-    x_counter = x_counter["sample_weight"]
-    p_x = list(map(lambda n: n / tot_weight, x_counter.values()))
-    h_x = ss.entropy(p_x)
-    xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
-    xy_counter = xy_counter["sample_weight"]
-    h_xy = 0.0
-    for xy in xy_counter.keys():
-        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
-        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
-        if p_xy != 0:
-            h_xy += p_xy * math.log(p_y / p_xy, math.e)
-
-    if h_x == 0:
-        return 1.0
-    else:
-        u = (h_x - h_xy) / h_x
-        if abs(u) < _PRECISION or abs(u - 1.0) < _PRECISION:
-            rounded_u = round(u)
-            warnings.warn(
-                f"Rounded U = {u} to {rounded_u}. This is probably due to floating point precision issues.",
-                RuntimeWarning,
-            )
-            u = rounded_u
-
-    if as_frame:
-        return pd.DataFrame({"row": x.name, "col": y.name, "val": u}, index=[0])
-    else:
-        return u
-
-
-def theils_u_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """theils_u_matrix theils_u_matrix computes the weighted Theil's U statistic for
-    categorical-categorical association. This is an asymmetric coefficient: U(x,y) != U(y,x)
-    U(x, y) means the uncertainty of x given y: value is on the range of [0,1] -
-    where 0 means y provides no information about x, and 1 means y provides full information about x
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X :  array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.DataFrame
-        The Theil's U matrix in a tidy (long) format.
-    """
-
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    # Cramer's V only for categorical columns
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-    cat_cols = dtypes_dic["cat"]
-
-    if cat_cols:
-        # explicitely store the unique 2-permutation of column names
-        # permutations and not combinations because U is asymmetric
-        comb_list = [comb for comb in permutations(cat_cols, 2)]
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(cat_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        # parallelize jobs
-        theil_u_matrix_entries = partial(
-            _compute_matrix_entries, func_xyw=weighted_theils_u
-        )
-        lst = parallel_matrix_entries(
-            func=theil_u_matrix_entries,
-            df=X,
-            comb_list=comb_list,
-            sample_weight=sample_weight,
-            n_jobs=-1,
-        )
-        return lst
-    else:
-        return None
-
-
-def theils_u_series(X, target, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """theils_u_series computes the weighted Theil's U statistic for
-    categorical-categorical association. This is an asymmetric coefficient: U(x,y) != U(y,x)
-    U(x, y) means the uncertainty of x given y: value is on the range of [0,1] -
-    where 0 means y provides no information about x, and 1 means y provides full information about x
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        The Theil's U series.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if col_dtypes_dic[target] != "cat":
-        raise TypeError("the target column is not categorical")
-
-    # Cramer's V only for categorical columns
-    cat_cols = dtypes_dic["cat"]
-
-    if cat_cols:
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(cat_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        # parallelize jobs
-        _theil_u = partial(_compute_series, func_xyw=weighted_theils_u)
-        lst = parallel_df(
-            func=_theil_u,
-            df=X[cat_cols],
-            series=X[target],
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-        return lst
-    else:
-        return None
-
-
-def cramer_v(x, y, sample_weight=None, as_frame=False):
-    """cramer_v computes the weighted V statistic of two
-    categorical predictors.
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The predictor vector, the first categorical predictor
-    y : pd.Series of shape (n_samples,)
-        second categorical predictor, order doesn't matter, symmetrical association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-
-    Returns
-    -------
-    pd.DataFrame
-        single row dataframe with the predictor names and the statistic value
-    """
-    tot_weight = sample_weight.sum()
-    weighted_tab = pd.crosstab(x, y, sample_weight, aggfunc=sum).fillna(0)
-    chi2 = ss.chi2_contingency(weighted_tab)[0]
-    phi2 = chi2 / tot_weight
-    r, k = weighted_tab.shape
-    phi2corr = max(0, phi2 - ((k - 1) * (r - 1)) / (tot_weight - 1))
-    rcorr = r - ((r - 1) ** 2) / (tot_weight - 1)
-    kcorr = k - ((k - 1) ** 2) / (tot_weight - 1)
-    v = np.sqrt(phi2corr / min((kcorr - 1), (rcorr - 1)))
-
-    if as_frame:
-        x_name = x.name if isinstance(x, pd.Series) else "var"
-        y_name = y.name if isinstance(y, pd.Series) else "target"
-        return pd.DataFrame(
-            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [v, v]}
-        )
-    else:
-        return v
-
-
-def cramer_v_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """cramer_v_matrix computes the weighted Cramer's V statistic for
-    categorical-categorical association. This is a symmetric coefficient: V(x,y) = V(y,x)
-
-    It uses the corrected Cramer's V statistics, itself based on the chi2 contingency
-    table. The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X :  array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.DataFrame
-        The Cramer's V matrix (lower triangular) in a tidy (long) format.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    # Cramer's V only for categorical columns
-    # in GLM supposed to be all the columns
-    cat_cols = dtypes_dic["cat"]
-
-    if cat_cols:
-        # explicitely store the unique 2-combinations of column names
-        comb_list = [comb for comb in combinations(cat_cols, 2)]
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(cat_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        _cramer_v_matrix_entries = partial(_compute_matrix_entries, func_xyw=cramer_v)
-        lst = parallel_matrix_entries(
-            func=_cramer_v_matrix_entries,
-            df=X,
-            comb_list=comb_list,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-        return lst
-    else:
-        return None
-
-
-def cramer_v_series(X, target, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """cramer_v_series computes the weighted Cramer's V statistic for
-    categorical-categorical association. This is a symmetric coefficient: V(x,y) = V(y,x)
-
-    It uses the corrected Cramer's V statistics, itself based on the chi2 contingency
-    table. The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        The Cramer's V series
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if col_dtypes_dic[target] != "cat":
-        raise TypeError("the target column is not categorical")
-
-    # Cramer's V only for categorical columns
-    cat_cols = dtypes_dic["cat"]
-
-    if cat_cols:
-        X = X[cat_cols]
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(cat_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        # parallelize jobs
-        _cramer_v = partial(_compute_series, func_xyw=cramer_v)
-        lst = parallel_df(
-            func=_cramer_v,
-            df=X[cat_cols],
-            series=X[target],
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-        # concatenate the results
-        # v_df_list = list(chain(*v_df_list))
-        return lst  # pd.concat(lst)
-    else:
-        return None
-
-
-def _weighted_correlation_ratio(*args):
-    """Calculates the Correlation Ratio (sometimes marked by the greek letter Eta)
-    for categorical-continuous association.
-    Answers the question - given a continuous value of a measurement, is it
-    possible to know which category is it associated with?
-    Value is in the range [0,1], where 0 means a category cannot be determined
-    by a continuous measurement, and 1 means a category can be determined with
-    absolute certainty.
-
-    Based on the scikit-learn implementation of the unweighted version.
-
-    Returns
-    -------
-    float
-        value of the correlation ratio
-    """
-    # how many levels (predictor)
-    n_classes = len(args)
-    # convert to float 2-uple d'array
-    args = [as_float_array(a) for a in args]
-    # compute the total weight per level
-    weight_per_class = np.array([a[1].sum() for a in args])
-    # total weight
-    tot_weight = np.sum(weight_per_class)
-    # weighted sum of squares
-    ss_alldata = sum((a[1] * safe_sqr(a[0])).sum(axis=0) for a in args)
-    # list of weighted sums
-    sums_args = [np.asarray((a[0] * a[1]).sum(axis=0)) for a in args]
-    square_of_sums_alldata = sum(sums_args) ** 2
-    square_of_sums_args = [s**2 for s in sums_args]
-    sstot = ss_alldata - square_of_sums_alldata / float(tot_weight)
-    ssbn = 0.0
-    for k, _ in enumerate(args):
-        ssbn += square_of_sums_args[k] / weight_per_class[k]
-    ssbn -= square_of_sums_alldata / float(tot_weight)
-    constant_features_idx = np.where(sstot == 0.0)[0]
-    if np.nonzero(ssbn)[0].size != ssbn.size and constant_features_idx.size:
-        warnings.warn("Features %s are constant." % constant_features_idx, UserWarning)
-    etasq = ssbn / sstot
-    # flatten matrix to vector in sparse case
-    etasq = np.asarray(etasq).ravel()
-    return np.sqrt(etasq)
-
-
-def correlation_ratio(x, y, sample_weight=None, as_frame=False):
-    """Compute the weighted correlation ratio. The association between a continuous predictor (y)
-    and a categorical predictor (x). It can be weighted.
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The categorical predictor vector
-    y : pd.Series of shape (n_samples,)
-        The continuous predictor
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-
-    Returns
-    -------
-    float
-        value of the correlation ratio
-    """
-    if sample_weight is None:
-        sample_weight = np.ones_like(y)
-
-    # one 2-uple per level of the categorical feature x
-    if x.dtype in ["category", "object", "bool"]:
-        args = [
-            (
-                y[safe_mask(y, x == k)],
-                sample_weight[safe_mask(sample_weight, x == k)],
-            )
-            for k in np.unique(x)
-        ]
-    elif y.dtype in ["category", "object", "bool"]:
-        args = [
-            (
-                x[safe_mask(x, y == k)],
-                sample_weight[safe_mask(sample_weight, y == k)],
-            )
-            for k in np.unique(y)
-        ]
-    else:
-        raise TypeError(
-            "one of the two series should be categorical/object and the other numerical"
-        )
-
-    if as_frame:
-        x_name = x.name if isinstance(x, pd.Series) else "var"
-        y_name = y.name if isinstance(y, pd.Series) else "target"
-        v = _weighted_correlation_ratio(*args)[0]
-        return pd.DataFrame(
-            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [v, v]}
-        )
-    else:
-        return _weighted_correlation_ratio(*args)[0]
-
-
-def correlation_ratio_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """correlation_ratio_matrix computes the weighted Correlation Ratio for
-    categorical-numerical association. This is a symmetric coefficient: CR(x,y) = CR(y,x)
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X :  array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.DataFrame
-        The correlation ratio matrix (lower triangular) in a tidy (long) format.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    # Cramer's V only for categorical columns
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-    cat_cols = dtypes_dic["cat"]
-    num_cols = dtypes_dic["num"]
-
-    if cat_cols and num_cols:
-        # explicitely store the unique 2-combinations of column names
-        # the first one should be the categorical predictor
-        comb_list = list(product(cat_cols, num_cols))
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(cat_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        # parallelize jobs
-        corr_ratio_matrix_entries = partial(
-            _compute_matrix_entries, func_xyw=correlation_ratio
-        )
-        lst = parallel_matrix_entries(
-            func=corr_ratio_matrix_entries,
-            df=X,
-            comb_list=comb_list,
-            sample_weight=sample_weight,
-            n_jobs=-1,
-        )
-        return lst
-    else:
-        return None
-
-
-def correlation_ratio_series(
-    X, target, sample_weight=None, n_jobs=-1, handle_na="drop"
-):
-    """correlation_ratio_series computes the weighted correlation ration for
-    categorical-numerical association. This is a symmetric coefficient: CR(x,y) = CR(y,x)
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format, a series.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        The Correlation ratio series (lower triangular) in a tidy (long) format.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if col_dtypes_dic[target] == "cat":
-        # if the target is categorical, pick only num predictors
-        pred_list = dtypes_dic["num"]
-    else:
-        # if the target is numerical, the 2nd pred should be categorical
-        pred_list = dtypes_dic["cat"]
-
-    if pred_list:
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(pred_list))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-        # parallelize jobs
-        _corr_ratio = partial(_compute_series, func_xyw=correlation_ratio)
-        lst = parallel_df(
-            func=_corr_ratio,
-            df=X[pred_list],
-            series=X[target],
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-        return lst
-    else:
-        return None
-
-
-def wm(x, w):
-    """wm computes the weighted mean
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples,)
-        the target array
-    w : array-like of shape (n_samples,)
-        the sample weights array
-
-    Returns
-    -------
-    float
-        weighted mean
-    """
-    return np.sum(x * w) / np.sum(w)
-
-
-def wcov(x, y, w):
-    """wcov computes the weighted covariance
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples,)
-        the perdictor 1 array
-    y : array-like of shape (n_samples,)
-        the perdictor 2 array
-    w : array-like of shape (n_samples,)
-        the sample weights array
-
-    Returns
-    -------
-    float
-        weighted covariance
-    """
-    return np.sum(w * (x - wm(x, w)) * (y - wm(y, w))) / np.sum(w)
-
-
-def wcorr(x, y, w):
-    """wcov computes the weighted Pearson correlation coefficient
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples,)
-        the perdictor 1 array
-    y : array-like of shape (n_samples,)
-        the perdictor 2 array
-    w : array-like of shape (n_samples,)
-        the sample weights array
-
-    Returns
-    -------
-    float
-        weighted correlation coefficient
-    """
-    return wcov(x, y, w) / np.sqrt(wcov(x, x, w) * wcov(y, y, w))
-
-
-def wrank(x, w):
-    """wrank computes the weighted rank
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples,)
-        the target array
-    w : array-like of shape (n_samples,)
-        the sample weights array
-
-    Returns
-    -------
-    float
-        weighted rank
-    """
-    (unique, arr_inv, counts) = np.unique(
-        rankdata(x), return_counts=True, return_inverse=True
-    )
-    a = np.bincount(arr_inv, w)
-    return (np.cumsum(a) - a)[arr_inv] + ((counts + 1) / 2 * (a / counts))[arr_inv]
-
-
-def wspearman(x, y, w):
-    """wcov computes the weighted Spearman correlation coefficient
-
-    Parameters
-    ----------
-    x : array-like of shape (n_samples,)
-        the perdictor 1 array
-    y : array-like of shape (n_samples,)
-        the perdictor 2 array
-    w : array-like of shape (n_samples,)
-        the sample weights array
-
-    Returns
-    -------
-    float
-        Spearman weighted correlation coefficient
-    """
-    return wcorr(wrank(x, w), wrank(y, w), w)
-
-
-def weighted_corr(x, y, sample_weight=None, as_frame=False, method="pearson"):
-    """weighted_corr computes the weighted correlation coefficient (Pearson or Spearman)
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The categorical predictor vector
-    y : pd.Series of shape (n_samples,)
-        The continuous predictor
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-    method : str
-        either "spearman" or "pearson", by default "pearson"
-
-    Returns
-    -------
-    float or pd.DataFrame
-        weighted correlation coefficient
-    """
-
-    if method == "pearson":
-        c = wcorr(x, y, sample_weight)
-    else:
-        c = wspearman(x, y, sample_weight)
-
-    if as_frame:
-        x_name = x.name if isinstance(x, pd.Series) else "var"
-        y_name = y.name if isinstance(y, pd.Series) else "target"
-        return pd.DataFrame(
-            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [c, c]}
-        )
-    else:
-        return c
-
-
-def wcorr_series(
-    X, target, sample_weight=None, n_jobs=-1, handle_na="drop", method="pearson"
-):
-    """wcorr_series computes the weighted correlation coefficient (Pearson or Spearman) for
-    continuous-continuous association. This is an symmetric coefficient: corr(x,y) = corr(y,x)
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    method : str
-        either "spearman" or "pearson", by default "pearson"
-
-    Returns
-    -------
-    pd.Series
-        The weighted correlation series.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if col_dtypes_dic[target] == "cat":
-        raise TypeError("the target column is categorical")
-
-    num_cols = dtypes_dic["num"]
-    y = X[target]
-
-    if num_cols:
-        _wcorr_method = partial(weighted_corr, method=method)
-        # parallelize jobs
-        _wcorr_method_series = partial(_compute_series, func_xyw=_wcorr_method)
-        return parallel_df(
-            func=_wcorr_method_series,
-            df=X[num_cols],
-            series=y,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-    else:
-        return None
-
-
-def wcorr_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop", method="pearson"):
-    """wcorr_matrix computes the weighted correlation statistic for
-    (Pearson or Spearman) for continuous-continuous association.
-    This is an symmetric coefficient: corr(x,y) = corr(y,x)
-
-    The computation is embarrassingly parallel and is distributed on available cores.
-    Moreover, the statistic is computed for the unique combinations only and returned in a
-    tidy (long) format.
-
-    Parameters
-    ----------
-    X :  array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    method : str
-        either "spearman" or "pearson"
-
-    Returns
-    -------
-    pd.DataFrame
-        The Cramer's V matrix (lower triangular) in a tidy (long) format.
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    num_cols = dtypes_dic["num"]
-    if num_cols:
-        # explicitely store the unique 2-combinations of column names
-        comb_list = [comb for comb in combinations(num_cols, 2)]
-        # define the number of cores
-        n_jobs = (
-            min(cpu_count(), len(num_cols))
-            if n_jobs == -1
-            else min(cpu_count(), n_jobs)
-        )
-
-        if (n_jobs > 1) or (method != "pearson"):
-            _wcorr_method = partial(weighted_corr, method=method)
-            _wcorr_method_entries = partial(
-                _compute_matrix_entries, func_xyw=_wcorr_method
-            )
-            lst = parallel_matrix_entries(
-                func=_wcorr_method_entries,
-                df=X,
-                comb_list=comb_list,
-                sample_weight=sample_weight,
-                n_jobs=-1,
-            )
-            return lst
-        else:
-            return (
-                matrix_to_xy(weighted_correlation_1cpu(X, sample_weight, handle_na))
-                .to_frame()
-                .reset_index()
-                .rename(columns={"level_0": "row", "level_1": "col", 0: "val"})
-            )
-    else:
-        return None
-
-
-def weighted_correlation_1cpu(X, sample_weight=None, handle_na="drop"):
-    """weighted_correlation computes the lower triangular weighted correlation matrix
-    using a single CPU, therefore using common numpy linear algebra
-
-    Parameters
-    ----------
-    X :  array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.DataFrame
-        the lower triangular weighted correlation matrix in long format
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-    # degree of freedom for the second moment estimator
-    ddof = 1
-
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    numeric_cols = dtypes_dic["num"]
-
-    if numeric_cols:
-        data = X[numeric_cols]
-        col_idx = data.columns
-        data = data.values
-        sum_weights = sample_weight.sum()
-        weighted_sum = np.dot(data.T, sample_weight)
-        weighted_mean = weighted_sum / sum_weights
-        demeaned = data - weighted_mean
-        sum_of_squares = np.dot((demeaned**2).T, sample_weight)
-        weighted_std = np.sqrt(sum_of_squares / (sum_weights - ddof))
-        weighted_cov = np.dot(sample_weight * demeaned.T, demeaned)
-        weighted_cov /= sum_weights - ddof
-        weighted_corcoef = pd.DataFrame(
-            weighted_cov / weighted_std / weighted_std[:, None],
-            index=col_idx,
-            columns=col_idx,
-        )
-        return weighted_corcoef
-    else:
-        return None
-
-
-#################################
-# association
-# cat-cat + cat-cont + cont-cont
-#################################
-
-
-def association_series(
-    X,
-    target,
-    features=None,
-    sample_weight=None,
-    nom_nom_assoc="theil",
-    num_num_assoc="pearson",
-    nom_num_assoc="correlation_ratio",
-    normalize=False,
-    n_jobs=-1,
-    handle_na="drop",
-):
-    """association_series computes the association matrix for cont-cont, cat-cont and cat-cat.
-    predictors. The weighted correlation matrix is used for the cont-cont predictors.
-    The correlation ratio is used between cont-cat predictors and either the Cramer's V or Theil's U
-    matrix for cat-cat predictors. The Pearson or Spearman correlation coefficient is used for
-    the cont-cont association.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    features : list of str, optional
-        list of features with which to compute the association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    nom_nom_assoc : str or callable
-        If callable, a function which receives two `pd.Series` (and optionally a weight array) and returns a single number.
-        If string, name of nominal-nominal (categorical-categorical) association to use.
-        Options are 'cramer' for Cramer's V or `theil` for Theil's U. If 'theil',
-        heat-map columns are the provided information (U = U(row|col)).
-    num_num_assoc : str or callable
-        If callable, a function which receives two `pd.Series` and returns a single number.
-        If string, name of numerical-numerical association to use. Options are 'pearson'
-        for Pearson's R, 'spearman' for Spearman's R.
-    nom_num_assoc : str or callable
-        If callable, a function which receives two `pd.Series` and returns a single number.
-        If string, name of nominal-numerical association to use. Options are 'correlation_ratio'
-        for correlation ratio
-    normalize : bool
-        either to normalize or not the scores
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        a series with all the association values with the target column
-
-    Raises
-    ------
-    TypeError
-        if features is not None and is not a list of strings
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    if features and is_list_of_str(features):
-        data = X[features + [target]]
-    elif features and (not is_list_of_str(features)):
-        raise TypeError("features is not a list of strings")
-    elif features is None:
-        data = X
-
-    dtypes_dic = create_dtype_dict(X)
-
-    # only numeric, NaN already checked, not repeating the process
-    if X.dtypes.map(is_numeric_dtype).all():
-        if callable(num_num_assoc):
-            return _callable_association_series_fn(
-                assoc_fn=num_num_assoc,
-                X=data,
-                target=target,
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-                kind="num-num",
-            )
-        else:
-            return wcorr_series(
-                data,
-                target,
-                sample_weight,
-                n_jobs,
-                handle_na=None,
-                method=num_num_assoc,
-            )
-
-    # only categorical (here understood as no numerical columns)
-    if not X.dtypes.map(is_numeric_dtype).any():
-        if callable(nom_nom_assoc):
-            return _callable_association_series_fn(
-                assoc_fn=nom_nom_assoc,
-                X=data,
-                target=target,
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-                kind="nom-nom",
-            )
-        elif nom_nom_assoc == "theil":
-            return theils_u_series(data, target, sample_weight, n_jobs, handle_na=None)
-        elif nom_nom_assoc == "cramer":
-            return cramer_v_series(data, target, sample_weight, n_jobs, handle_na=None)
-
-    # cat-num
-    if callable(nom_num_assoc):
-        assoc_series = _callable_association_series_fn(
-            assoc_fn=nom_num_assoc,
-            X=data,
-            target=target,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-            kind="nom-num",
-        )
-    else:
-        assoc_series = correlation_ratio_series(
-            data, target, sample_weight, n_jobs, handle_na=None
-        )
-
-    if normalize:
-        assoc_series = (assoc_series - assoc_series.min()) / np.ptp(assoc_series)
-
-    # cat-cat
-    if dtypes_dic[target] == "cat":
-        if callable(nom_nom_assoc):
-            assoc_series_complement = _callable_association_series_fn(
-                assoc_fn=nom_nom_assoc,
-                X=data,
-                target=target,
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-                kind="nom-nom",
-            )
-        elif nom_nom_assoc == "theil":
-            assoc_series_complement = theils_u_series(
-                data, target, sample_weight, n_jobs, handle_na=None
-            )
-        else:
-            assoc_series_complement = cramer_v_series(
-                data, target, sample_weight, n_jobs, handle_na=None
-            )
-
-        if normalize:
-            assoc_series_complement = (
-                assoc_series_complement - assoc_series_complement.min()
-            ) / np.ptp(assoc_series_complement)
-
-        assoc_series = pd.concat([assoc_series, assoc_series_complement])
-
-    # num-num
-    if dtypes_dic[target] == "num":
-        if callable(num_num_assoc):
-            assoc_series_complement = _callable_association_series_fn(
-                assoc_fn=num_num_assoc,
-                X=data,
-                target=target,
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-                kind="num-num",
-            )
-        else:
-            assoc_series_complement = wcorr_series(
-                data,
-                target,
-                sample_weight,
-                n_jobs,
-                handle_na=None,
-                method=num_num_assoc,
-            )
-
-        if normalize:
-            assoc_series_complement = (
-                assoc_series_complement - assoc_series_complement.min()
-            ) / np.ptp(assoc_series_complement)
-
-        assoc_series = pd.concat([assoc_series, assoc_series_complement])
-
-    return assoc_series.sort_values(ascending=False)
-
-
-def association_matrix(
-    X,
-    sample_weight=None,
-    nom_nom_assoc="theil",
-    num_num_assoc="pearson",
-    nom_num_assoc="correlation_ratio",
-    n_jobs=-1,
-    handle_na="drop",
-    nom_nom_comb=None,
-    num_num_comb=None,
-    nom_num_comb=None,
-):
-    """association_matrix computes the association matrix for cont-cont, cat-cont and cat-cat.
-    predictors. The weighted correlation matrix is used for the cont-cont predictors.
-    The correlation ratio is used between cont-cat predictors and either the Cramer's V or Theil's U
-    matrix for cat-cat predictors.
-
-    The association matrix is not symmetric is Theil is used. The obeservations might be weighted.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    nom_nom_assoc : str or callable
-        If callable, a function which receives two `pd.Series` (and optionally a weight array) and returns a single number.
-        If string, name of nominal-nominal (categorical-categorical) association to use.
-        Options are 'cramer' for Cramer's V or `theil` for Theil's U. If 'theil',
-        heat-map columns are the provided information (U = U(row|col)).
-    num_num_assoc : str or callable
-        If callable, a function which receives two `pd.Series` and returns a single number.
-        If string, name of numerical-numerical association to use. Options are 'pearson'
-        for Pearson's R, 'spearman' for Spearman's R.
-    nom_num_assoc : str or callable
-        If callable, a function which receives two `pd.Series` and returns a single number.
-        If string, name of nominal-numerical association to use. Options are 'correlation_ratio'
-        for correlation ratio
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-    nom_nom_comb_list : list of 2-uple of strings
-        Pairs of column names corresponding to the entries for nom_nom associations.
-        If asymmetrical association, take care of providing an exhaustive list of column name pairs.
-    num_num_comb_list : list of 2-uple of strings
-        Pairs of column names corresponding to the entries for num_num associations
-    nom_num_comb_list : list of 2-uple of strings
-        Pairs of column names corresponding to the entries for nom_num associations
-
-    Returns
-    -------
-    pd.DataFrame
-        the association matrix
-    """
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    # num-num, NaNs already checked above, not repeating the process
-    if callable(num_num_assoc):
-        w_num_num = _callable_association_matrix_fn(
-            assoc_fn=num_num_assoc,
-            cols_comb=num_num_comb,
-            kind="num-num",
-            X=X,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-    else:
-        w_num_num = wcorr_matrix(
-            X, sample_weight, n_jobs, handle_na=None, method=num_num_assoc
-        )
-
-    # nom-num
-    if callable(nom_num_assoc):
-        w_nom_num = _callable_association_matrix_fn(
-            assoc_fn=nom_num_assoc,
-            cols_comb=nom_num_comb,
-            kind="nom-num",
-            X=X,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-    else:
-        w_nom_num = correlation_ratio_matrix(X, sample_weight, n_jobs, handle_na=None)
-
-    # nom-nom
-    if callable(nom_nom_assoc):
-        w_nom_nom = _callable_association_matrix_fn(
-            assoc_fn=nom_nom_assoc,
-            cols_comb=nom_nom_comb,
-            kind="nom-nom",
-            X=X,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-    elif nom_nom_assoc == "cramer":
-        w_nom_nom = cramer_v_matrix(X, sample_weight, n_jobs, handle_na=None)
-    else:
-        w_nom_nom = theils_u_matrix(X, sample_weight, n_jobs, handle_na=None)
-
-    return pd.concat([w_num_num, w_nom_num, w_nom_nom], ignore_index=True)
-
-
-def _callable_association_series_fn(
-    assoc_fn, X, target, sample_weight=None, n_jobs=-1, kind="nom-nom"
-):
-    """_callable_association_series_fn private function, utility for computing association series
-    for a callable custom association
-
-    Parameters
-    ----------
-    assoc_fn : callable
-        a function which receives two `pd.Series` (and optionally a weight array) and returns a single number
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    target : str or int
-        the predictor name or index with which to compute association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    kind : str
-        kind of association, either 'num-num' or 'nom-nom' or 'nom-num'
-
-    Returns
-    -------
-    pd.Series
-        the association series
-
-    Raises
-    ------
-    ValueError
-        if kind is not 'num-num' or 'nom-nom' or 'nom-num'
-    """
-    col_dtypes_dic = create_dtype_dict(X)
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if kind == "nom-nom":
-        if col_dtypes_dic[target] != "cat":
-            raise TypeError("the target column is not categorical")
-        nom_cols = dtypes_dic["cat"]
-        if nom_cols:
-            # define the number of cores
-            n_jobs = (
-                min(cpu_count(), len(nom_cols))
-                if n_jobs == -1
-                else min(cpu_count(), n_jobs)
-            )
-            # parallelize jobs
-            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
-            return parallel_df(
-                func=_assoc_fn,
-                df=X[nom_cols],
-                series=X[target],
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-            )
-        else:
-            return None
-
-    elif kind == "nom-num":
-        if col_dtypes_dic[target] == "cat":
-            # if the target is categorical, pick only num predictors
-            pred_list = dtypes_dic["num"]
-        else:
-            # if the target is numerical, the 2nd pred should be categorical
-            pred_list = dtypes_dic["cat"]
-
-        if pred_list:
-            # define the number of cores
-            n_jobs = (
-                min(cpu_count(), len(pred_list))
-                if n_jobs == -1
-                else min(cpu_count(), n_jobs)
-            )
-            # parallelize jobs
-            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
-            return parallel_df(
-                func=_assoc_fn,
-                df=X[pred_list],
-                series=X[target],
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-            )
-        else:
-            return None
-
-    elif kind == "num-num":
-        num_cols = dtypes_dic["num"]
-        if num_cols:
-            # parallelize jobs
-            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
-            return parallel_df(
-                func=_assoc_fn,
-                df=X[num_cols],
-                series=X[target],
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-            )
-        else:
-            return None
-    else:
-        raise ValueError("kind can be 'num-num' or 'nom-num' or 'nom-nom'")
-
-
-def _callable_association_matrix_fn(
-    assoc_fn, X, sample_weight=None, n_jobs=-1, kind="nom-nom", cols_comb=None
-):
-    """_callable_association_matrix_fn private function, utility for computing association matrix
-    for a callable custom association
-
-    Parameters
-    ----------
-    assoc_fn : callable
-        a function which receives two `pd.Series` (and optionally a weight array) and returns a single number
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    kind : str
-        kind of association, either 'num-num' or 'nom-nom' or 'nom-num'
-    cols_comb : list of 2-uple of str, optional
-        combination of column names (list of 2-uples of strings)
-
-    Returns
-    -------
-    pd.DataFrame
-        the association matrix
-    """
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    if cols_comb is None:
-        if kind == "num-num":
-            selected_cols = dtypes_dic["num"]
-        elif kind == "nom-nom":
-            selected_cols = dtypes_dic["cat"]
-        elif kind == "nom-num":
-            cat_cols = dtypes_dic["cat"]
-            num_cols = dtypes_dic["num"]
-            if cat_cols and num_cols:
-                # explicitely store the unique 2-combinations of column names
-                # the first one should be the categorical predictor
-                selected_cols = list(product(cat_cols, num_cols))
-        else:
-            selected_cols = None
-
-        if selected_cols:
-            # explicitely store the unique 2-combinations of column names
-            cols_comb = [comb for comb in combinations(selected_cols, 2)]
-            _assoc_fn = partial(_compute_matrix_entries, func_xyw=assoc_fn)
-            assoc = parallel_matrix_entries(
-                func=_assoc_fn,
-                df=X,
-                comb_list=cols_comb,
-                sample_weight=sample_weight,
-                n_jobs=n_jobs,
-            )
-
-        else:
-            assoc = None
-    else:
-        _assoc_fn = partial(_compute_matrix_entries, func_xyw=assoc_fn)
-        assoc = parallel_matrix_entries(
-            func=_assoc_fn,
-            df=X,
-            comb_list=cols_comb,
-            sample_weight=sample_weight,
-            n_jobs=n_jobs,
-        )
-    return assoc
-
-
-################################
-# Association predictor-target
-################################
-
-
-def f_oneway_weighted(*args):
-    """
-    Calculate the weighted F-statistic for one-way ANOVA (continuous target, categorical predictor).
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples,)
-        The predictor dataframe.
-    y : array-like of shape (n_samples,)
-        The target vector.
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None.
-
-    Returns
-    -------
-    float
-        The value of the F-statistic.
-
-    Notes
-    -----
-    The F-statistic is calculated as:
-
-    .. math::
-        F(rf) = \\frac{\\sum_i (\\bar{Y}_{i \\bullet} - \\bar{Y})^2 / (K-1)}{\\sum_i \\sum_k (\\bar{Y}_{ij} - \\bar{Y}_{i\\bullet})^2 / (N - K)}
-    """
-    # how many levels (predictor)
-    n_classes = len(args)
-    # convert to float 2-uple d'array
-    args = [as_float_array(a) for a in args]
-    # compute the total weight per level
-    weight_per_class = np.array([a[1].sum() for a in args])
-    # total weight
-    tot_weight = np.sum(weight_per_class)
-    # weighted sum of squares
-    ss_alldata = sum((a[1] * safe_sqr(a[0])).sum(axis=0) for a in args)
-    # list of weighted sums
-    sums_args = [np.asarray((a[0] * a[1]).sum(axis=0)) for a in args]
-    square_of_sums_alldata = sum(sums_args) ** 2
-    square_of_sums_args = [s**2 for s in sums_args]
-    sstot = ss_alldata - square_of_sums_alldata / float(tot_weight)
-    ssbn = 0.0
-    for k, _ in enumerate(args):
-        ssbn += square_of_sums_args[k] / weight_per_class[k]
-    ssbn -= square_of_sums_alldata / float(tot_weight)
-    sswn = sstot - ssbn
-    dfbn = n_classes - 1
-    dfwn = tot_weight - n_classes
-    msb = ssbn / float(dfbn)
-    msw = sswn / float(dfwn)
-    constant_features_idx = np.where(msw == 0.0)[0]
-    if np.nonzero(msb)[0].size != msb.size and constant_features_idx.size:
-        warnings.warn("Features %s are constant." % constant_features_idx, UserWarning)
-    f = msb / msw
-    # flatten matrix to vector in sparse case
-    f = np.asarray(f).ravel()
-    return f
-
-
-def f_cat_regression(x, y, sample_weight=None, as_frame=False):
-    """f_cat_regression computes the weighted ANOVA F-value for the provided sample.
-    (continuous target, categorical predictor)
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The predictor vector, the first categorical predictor
-    y : pd.Series of shape (n_samples,)
-        second categorical predictor, order doesn't matter, symmetrical association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-
-    Returns
-    -------
-    float
-        value of the F-statistic
-    """
-    if sample_weight is None:
-        sample_weight = np.ones_like(y)
-
-    # one 2-uple per level of the categorical feature x
-    args = [
-        (
-            y[safe_mask(y, x == k)],
-            sample_weight[safe_mask(sample_weight, x == k)],
-        )
-        for k in np.unique(x)
-    ]
-
-    if as_frame:
-        x_name = x.name if isinstance(x, pd.Series) else "var"
-        y_name = y.name if isinstance(y, pd.Series) else "target"
-        return pd.DataFrame(
-            {"row": x_name, "col": y_name, "val": f_oneway_weighted(*args)[0]},
-            index=[0],
-        )
-    else:
-        return f_oneway_weighted(*args)[0]
-
-
-def f_cat_regression_parallel(X, y, sample_weight=None, n_jobs=-1, handle_na="drop"):
-    """f_cat_regression_parallel computes the weighted ANOVA F-value for the provided categorical predictors
-    using parallelization of the code (continuous target, categorical predictor).
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    y : array-like of shape (n_samples,)
-        The target vector
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        the value of the F-statistic for each predictor
-    """
-
-    # Cramer's V only for categorical columns
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    cat_cols = dtypes_dic["cat"]
-
-    if not isinstance(y, pd.Series):
-        y = pd.Series(y)
-        y.name = "target"
-
-    target = y.name
-    X[target] = y.values
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    y = X[target].copy()
-    X = X.drop(target, axis=1)
-
-    # define the number of cores
-    n_jobs = min(cpu_count(), X.shape[1]) if n_jobs == -1 else min(cpu_count(), n_jobs)
-    # parallelize jobs
-    _f_stat_cat = partial(_compute_series, func_xyw=f_cat_regression)
-    return parallel_df(
-        func=_f_stat_cat,
-        df=X[cat_cols],
-        series=y,
-        sample_weight=sample_weight,
-        n_jobs=n_jobs,
-    )
-
-
-def f_cont_regression_parallel(
-    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
-):
-    """Univariate linear regression tests returning F-statistic.
-
-    Quick linear model for testing the effect of a single regressor,
-    sequentially for many regressors.
-    This is done in 2 steps:
-    1. The cross-correlation between each regressor and the target is computed using:
-           E[(X[:, i] - mean(X[:, i])) * (y - mean(y))] / (std(X[:, i]) * std(y))
-    2. It is converted to an F score ranks features in the same order if all the features
-       are positively correlated with the target.
-    Note that it is therefore recommended as a feature selection criterion to identify
-    potentially predictive features for a downstream classifier, irrespective of
-    the sign of the association with the target variable.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        The predictor dataframe.
-    y : array-like of shape (n_samples,)
-        The target vector.
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None.
-    n_jobs : int, optional
-        The number of cores to use for the computation, by default -1.
-    handle_na : str, optional
-        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
-    force_finite : bool, optional
-        Whether or not to force the F-statistics and associated p-values to
-        be finite. There are two cases where the F-statistic is expected to not
-        be finite:
-        - when the target `y` or some features in `X` are constant. In this
-          case, the Pearson's R correlation is not defined leading to obtain
-          `np.nan` values in the F-statistic and p-value. When
-          `force_finite=True`, the F-statistic is set to `0.0` and the
-          associated p-value is set to `1.0`.
-        - when a feature in `X` is perfectly correlated (or
-          anti-correlated) with the target `y`. In this case, the F-statistic
-          is expected to be `np.inf`. When `force_finite=True`, the F-statistic
-          is set to `np.finfo(dtype).max`.
-
-    Returns
-    -------
-    f_statistic : array-like of shape (n_features,)
-        F-statistic for each feature.
-    """
-    if not isinstance(y, pd.Series):
-        y = pd.Series(y)
-        y.name = "target"
-
-    target = y.name
-    X[target] = y.values
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    correlation_coefficient = wcorr_series(X, target, sample_weight, n_jobs, handle_na)
-
-    deg_of_freedom = y.size - 2
-    corr_coef_squared = correlation_coefficient**2
-
-    with np.errstate(divide="ignore", invalid="ignore"):
-        f_statistic = corr_coef_squared / (1 - corr_coef_squared) * deg_of_freedom
-
-    if force_finite and not np.isfinite(f_statistic).all():
-        # case where there is a perfect (anti-)correlation
-        # f-statistics can be set to the maximum and p-values to zero
-        mask_inf = np.isinf(f_statistic)
-        f_statistic[mask_inf] = np.finfo(f_statistic.dtype).max
-        # case where the target or some features are constant
-        # f-statistics would be minimum and thus p-values large
-        mask_nan = np.isnan(f_statistic)
-        f_statistic[mask_nan] = 0.0
-
-    return f_statistic.drop(labels=[target]).sort_values(ascending=False)
-
-
-def f_stat_regression_parallel(
-    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
-):
-    """
-    Compute the weighted explained variance for the provided categorical and numerical predictors using parallelization.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        The predictor dataframe.
-    y : array-like of shape (n_samples,)
-        The target vector.
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None.
-    n_jobs : int, optional
-        The number of cores to use for the computation, by default -1.
-    handle_na : str, optional
-        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
-    force_finite : bool, optional
-        Whether or not to force the F-statistics and associated p-values to be finite.
-        There are two cases where the F-statistic is expected to not be finite:
-        - When the target `y` or some features in `X` are constant. In this case,
-          the Pearson's R correlation is not defined leading to obtain `np.nan`
-          values in the F-statistic and p-value. When `force_finite=True`, the
-          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
-        - When a feature in `X` is perfectly correlated (or anti-correlated)
-          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
-          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
-
-    Returns
-    -------
-    pd.Series
-        The value of the F-statistic for each predictor.
-    """
-    f_stat_cont_series = f_cont_regression_parallel(
-        X,
-        y,
-        sample_weight,
-        n_jobs,
-        force_finite=force_finite,
-        handle_na=handle_na,
-    )
-    f_stat_cat_series = f_cat_regression_parallel(
-        X, y, sample_weight, n_jobs, handle_na=handle_na
-    )
-
-    # normalize the scores
-    # correlation coefficient varies in the range [-1, 1]
-    # correlation ratio varies in the range [0, 1]
-    # Cramer's V varies in the range [0, 1]
-    # Theil's U varies in the range [0, 1]
-    # F-statistic varies in the range [0, +inf] but both kind of F stat are not necessary on the same scale
-    # in order to have a similar scale and compare both kind, one can studentize them
-    if X.shape[1] > 1:
-        f_stat_cont_series = (
-            f_stat_cont_series - f_stat_cont_series.mean()
-        ) / f_stat_cont_series.std()
-        f_stat_cat_series = (
-            f_stat_cat_series - f_stat_cat_series.mean()
-        ) / f_stat_cat_series.std()
-
-    return pd.concat([f_stat_cont_series, f_stat_cat_series]).sort_values(
-        ascending=False
-    )
-
-
-def f_cont_classification(x, y, sample_weight=None, as_frame=False):
-    """f_cont_classification computes the weighted ANOVA F-value for the provided sample.
-    Categorical target, continuous predictor.
-
-    Parameters
-    ----------
-    x : pd.Series of shape (n_samples,)
-        The predictor vector, the first categorical predictor
-    y : pd.Series of shape (n_samples,)
-        second categorical predictor, order doesn't matter, symmetrical association
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    as_frame: bool
-        return output as a dataframe or a float
-
-    Returns
-    -------
-    float :
-        value of the F-statistic
-    """
-    if sample_weight is None:
-        sample_weight = np.ones_like(y)
-
-    # one 2-uple per level of the categorical target y, continuous predictor x
-    args = [
-        (
-            x[safe_mask(x, y == k)],
-            sample_weight[safe_mask(sample_weight, y == k)],
-        )
-        for k in np.unique(y)
-    ]
-
-    if as_frame:
-        x_name = x.name if isinstance(x, pd.Series) else "var"
-        y_name = y.name if isinstance(y, pd.Series) else "target"
-        return pd.DataFrame(
-            {"row": x_name, "col": y_name, "val": f_oneway_weighted(*args)[0]},
-            index=[0],
-        )
-    else:
-        return f_oneway_weighted(*args)[0]
-
-
-def f_cont_classification_parallel(
-    X, y, sample_weight=None, n_jobs=-1, handle_na="drop"
-):
-    """f_cont_classification_parallel computes the weighted ANOVA F-value
-    for the provided categorical predictors using parallelization of the code.
-    Categorical target, continuous predictor.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        The set of regressors that will be tested sequentially
-    y : array-like of shape (n_samples,)
-        The target vector
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    pd.Series
-        the value of the F-statistic for each predictor
-    """
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-
-    num_cols = dtypes_dic["num"]
-
-    if not isinstance(y, pd.Series):
-        y = pd.Series(y)
-        y.name = "target"
-
-    target = y.name
-    X[target] = y.values
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    y = X[target].copy()
-    X = X.drop(target, axis=1)
-
-    # define the number of cores
-    n_jobs = min(cpu_count(), X.shape[1]) if n_jobs == -1 else min(cpu_count(), n_jobs)
-    # parallelize jobs
-    _f_stat_cont_clf = partial(_compute_series, func_xyw=f_cont_classification)
-    return parallel_df(
-        func=_f_stat_cont_clf,
-        df=X[num_cols],
-        series=y,
-        sample_weight=sample_weight,
-        n_jobs=n_jobs,
-    )
-
-
-def f_cat_classification_parallel(
-    X,
-    y,
-    sample_weight=None,
-    n_jobs=-1,
-    force_finite=True,
-    handle_na="drop",
-):
-    """
-    Univariate information dependence.
-
-    It ranks features in the same order if all the features are positively correlated with the target.
-    Note that it is therefore recommended as a feature selection criterion to identify
-    potentially predictive features for a downstream classifier, irrespective of
-    the sign of the association with the target variable.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        The predictor dataframe.
-    y : array-like of shape (n_samples,)
-        The target vector.
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None.
-    n_jobs : int, optional
-        The number of cores to use for the computation, by default -1.
-    handle_na : str, optional
-        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
-    force_finite : bool, optional
-        Whether or not to force the F-statistics and associated p-values to
-        be finite. There are two cases where the F-statistic is expected to not
-        be finite:
-            - when the target `y` or some features in `X` are constant. In this
-              case, the Pearson's R correlation is not defined leading to obtain
-              `np.nan` values in the F-statistic and p-value. When
-              `force_finite=True`, the F-statistic is set to `0.0` and the
-              associated p-value is set to `1.0`.
-            - when a feature in `X` is perfectly correlated (or
-              anti-correlated) with the target `y`. In this case, the F-statistic
-              is expected to be `np.inf`. When `force_finite=True`, the F-statistic
-              is set to `np.finfo(dtype).max`.
-
-    Returns
-    -------
-    f_statistic : array-like of shape (n_features,)
-        F-statistic for each feature.
-    """
-    if not isinstance(y, pd.Series):
-        y = pd.Series(y)
-        y.name = "target"
-
-    target = y.name
-    X[target] = y.values
-    # sanity checks
-    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
-
-    deg_of_freedom = y.size - 2
-
-    theils_u_coef = theils_u_series(X, target, sample_weight, n_jobs, handle_na)
-    theils_u_coef_squared = theils_u_coef**2
-
-    with np.errstate(divide="ignore", invalid="ignore"):
-        f_statistic = (
-            theils_u_coef_squared / (1 - theils_u_coef_squared) * deg_of_freedom
-        )
-
-    if force_finite and not np.isfinite(f_statistic).all():
-        # case where there is a perfect (anti-)correlation
-        # f-statistics can be set to the maximum and p-values to zero
-        mask_inf = np.isinf(f_statistic)
-        f_statistic[mask_inf] = np.finfo(f_statistic.dtype).max
-        # case where the target or some features are constant
-        # f-statistics would be minimum and thus p-values large
-        mask_nan = np.isnan(f_statistic)
-        f_statistic[mask_nan] = 0.0
-
-    return f_statistic.drop(labels=[target]).sort_values(ascending=False)
-
-
-def f_stat_classification_parallel(
-    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
-):
-    """
-    Compute the weighted ANOVA F-value for the provided categorical and numerical predictors using parallelization.
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        The predictor dataframe.
-    y : array-like of shape (n_samples,)
-        The target vector.
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None.
-    n_jobs : int, optional
-        The number of cores to use for the computation, by default -1.
-    handle_na : str, optional
-        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
-    force_finite : bool, optional
-        Whether or not to force the F-statistics and associated p-values to be finite.
-        There are two cases where the F-statistic is expected to not be finite:
-        - When the target `y` or some features in `X` are constant. In this case,
-          the Pearson's R correlation is not defined leading to obtain `np.nan`
-          values in the F-statistic and p-value. When `force_finite=True`, the
-          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
-        - When a feature in `X` is perfectly correlated (or anti-correlated)
-          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
-          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
-
-    Returns
-    -------
-    pd.Series
-        The value of the F-statistic for each predictor.
-    """
-    f_stat_cont_series = f_cont_classification_parallel(
-        X, y, sample_weight, n_jobs, handle_na=handle_na
-    )
-    f_stat_cat_series = f_cat_classification_parallel(
-        X,
-        y,
-        sample_weight,
-        n_jobs,
-        handle_na=handle_na,
-        force_finite=force_finite,
-    )
-
-    # normalize the scores
-    # correlation ratio varies in the range [0, 1]
-    # Cramer's V varies in the range [0, 1]
-    # Theil's U varies in the range [0, 1]
-    # F-statistic varies in the range [0, +inf]
-    # Both kind of F stat are not necessarily on the same scale
-    # one can studentize them
-    if X.shape[1] > 1:
-        f_stat_cont_series = (
-            f_stat_cont_series - f_stat_cont_series.mean()
-        ) / f_stat_cont_series.std()
-        f_stat_cat_series = (
-            f_stat_cat_series - f_stat_cat_series.mean()
-        ) / f_stat_cat_series.std()
-
-    return pd.concat([f_stat_cont_series, f_stat_cat_series]).sort_values(
-        ascending=False
-    )
-
-
-############
-# Utilities
-############
-
-
-def _check_association_input(X, sample_weight=None, handle_na="drop"):
-    """_check_association_input private function. Check the inputs,
-    convert X to a pd.DataFrame if needed, adds column names if non are provided.
-    Check if the sample_weight is None or of the right dimensionality and handle NA
-    according to the chosen methods (drop, fill, None).
-
-    Parameters
-    ----------
-    X : array-like of shape (n_samples, n_features)
-        predictor dataframe
-    sample_weight : array-like of shape (n_samples,), optional
-        The weight vector, by default None
-    handle_na : str, optional
-        either drop rows with na, fill na with 0 or do nothing, by default "drop"
-
-    Returns
-    -------
-    tuple
-        the dataframe and the sample weights
-
-    Raises
-    ------
-    ValueError
-        if sample_weight contains NA
-    """
-
-    if not isinstance(X, pd.DataFrame):
-        X = pd.DataFrame(X, columns=[f"pred_{i}" for i in range(X.shape[1])])
-
-    # sanity checks
-    if sample_weight is None:
-        sample_weight = np.ones(len(X))
-    elif ~np.isfinite(sample_weight).all():
-        raise ValueError("sample weights contains nans or nulls")
-
-    if isinstance(sample_weight, pd.Series):
-        sample_weight = sample_weight.to_numpy()
-
-    single_value_columns_set = set()
-    for c in X.columns:
-        if X[c].nunique() == 1:
-            single_value_columns_set.add(c)
-
-    if single_value_columns_set:
-        warnings.warn(
-            f"{single_value_columns_set} columns have been removed (single unique values)"
-        )
-
-    # handle nans
-    if handle_na is None:
-        pass
-    elif handle_na == "drop":
-        # mask the na
-        na_mask = (~X.isnull().any(axis=1)).values
-        if na_mask.any():
-            X, sample_weight = X.loc[na_mask, :], sample_weight[na_mask]
-    else:
-        X = X.fillna(0)
-    return X, sample_weight
-
-
-def is_list_of_str(str_list):
-    """Raise an exception if ``str_list`` is not a list of strings
-    Parameters
-    ----------
-    str_list : list
-        to list to be tested
-
-    Raises
-    ------
-    TypeError
-        if ``str_list`` is not a ``list[str]``
-    """
-    if str_list is not None:
-        if not (
-            isinstance(str_list, list) and all(isinstance(s, str) for s in str_list)
-        ):
-            return False
-        else:
-            return True
-
-
-def matrix_to_xy(df, columns=None, reset_index=False):
-    """matrix_to_xy wide to long format of the association matrix
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        the wide format of the association matrix
-    columns : list of str, optional
-        list of column names, by default None
-    reset_index : bool, optional
-        wether to reset_index or not, by default False
-
-    Returns
-    -------
-    pd.DataFrame
-        the long format of the association matrix
-    """
-    bool_index = np.tril(np.ones(df.shape), 0).astype(bool)
-    xy = (
-        df.where(bool_index).stack().reset_index()
-        if reset_index
-        else df.where(bool_index).stack()
-    )
-    if reset_index:
-        xy.columns = columns or ["row", "col", "val"]
-    return xy
-
-
-def xy_to_matrix(xy):
-    """xy_to_matrix long to wide format of the association matrix
-
-    Parameters
-    ----------
-    xy : pd.DataFrame
-        the long format of the association matrix, 3 columns.
-
-    Returns
-    -------
-    pd.DataFrame
-
-    """
-    xy = xy.pivot(index="row", columns="col").fillna(0)
-    xy.columns = xy.columns.droplevel(0)
-    return xy.rename_axis(None, axis=1).rename_axis(None, axis=0)
-
-
-###############
-# visualization
-###############
-
-
-def cluster_sq_matrix(sq_matrix, method="ward"):
-    """
-    Apply agglomerative clustering to sort a square correlation matrix.
-
-    Parameters
-    ----------
-    sq_matrix : pd.DataFrame
-        A square correlation matrix.
-    method : str, optional
-        The linkage method, by default "ward".
-
-    Returns
-    -------
-    pd.DataFrame
-        A sorted square matrix.
-
-    Example
-    -------
-    >>> from some_module import association_matrix, cluster_sq_matrix
-
-    >>> assoc = association_matrix(iris_df, plot=False)
-    >>> assoc_clustered = cluster_sq_matrix(assoc, method="complete")
-    """
-    d = sch.distance.pdist(sq_matrix.values)
-    L = sch.linkage(d, method=method)
-    ind = sch.fcluster(L, 0.5 * d.max(), "distance")
-    columns = [sq_matrix.columns.tolist()[i] for i in list((np.argsort(ind)))]
-    sq_matrix = sq_matrix.reindex(columns, axis=1)
-    sq_matrix = sq_matrix.reindex(columns, axis=0)
-    return sq_matrix
-
-
-def heatmap(
-    data, row_labels, col_labels, ax=None, cbar_kw=None, cbarlabel="", **kwargs
-):
-    """heatmap Create a heatmap from a numpy array and two lists of labels.
-
-    Parameters
-    ----------
-    data : array-like of shape (M, N)
-        matrix to plot
-    row_labels : array-like of shape (M,)
-        labels for the rows
-    col_labels : array-like of shape (N,)
-        labels for the columns
-    ax : matplotlib.axes.Axes, optional
-        A `matplotlib.axes.Axes` instance to which the heatmap is plotted.  If
-        not provided, use current axes or create a new one, by default None
-    cbar_kw : dict, optional
-         A dictionary with arguments to `matplotlib.Figure.colorbar`, by default None
-    cbarlabel : str, optional
-        The label for the colorbar, by default ""
-    kwargs : dict, optional
-        All other arguments are forwarded to `imshow`.
-
-    Returns
-    -------
-    tuple
-        imgshow and cbar objects
-    """
-
-    if ax is None:
-        ax = plt.gca()
-
-    if cbar_kw is None:
-        cbar_kw = {}
-
-    # Plot the heatmap
-    im = ax.imshow(data, **kwargs)
-
-    # Create colorbar
-    divider = make_axes_locatable(ax)
-
-    ax_cb = divider.append_axes("right", size="5%", pad=0.05)
-    fig = ax.get_figure()
-    fig.add_axes(ax_cb)
-
-    cbar = ax.figure.colorbar(im, cax=ax_cb, **cbar_kw)
-    cbar.ax.set_ylabel(cbarlabel, rotation=-90, va="bottom")
-
-    # Show all ticks and label them with the respective list entries.
-    ax.set_xticks(np.arange(data.shape[1]), labels=col_labels)
-    ax.set_yticks(np.arange(data.shape[0]), labels=row_labels)
-
-    # Let the horizontal axes labeling appear on top.
-    ax.tick_params(top=False, bottom=True, labeltop=False, labelbottom=True)
-
-    # Rotate the tick labels and set their alignment.
-    plt.setp(ax.get_xticklabels(), rotation=90, ha="right", rotation_mode="anchor")
-
-    # Turn spines off and create white grid.
-    ax.spines[:].set_visible(False)
-
-    ax.set_xticks(np.arange(data.shape[1] + 1) - 0.5, minor=True)
-    ax.set_yticks(np.arange(data.shape[0] + 1) - 0.5, minor=True)
-    ax.grid(which="minor", color="w", linestyle="-", linewidth=2)
-    ax.tick_params(which="minor", bottom=False, left=False)
-
-    return im, cbar
-
-
-def annotate_heatmap(
-    im,
-    data=None,
-    valfmt="{x:.2f}",
-    textcolors=("black", "white"),
-    threshold=None,
-    **textkw,
-):
-    """annotate_heatmap annotates a heatmap
-
-    Parameters
-    ----------
-    im : matplotlib.axes.Axes
-        The AxesImage to be labeled
-    data : array-like of shape (M, N), optional
-        data to illustrate, if none is provided the function retrieves
-        the array of the mlp obkect, by default None
-    valfmt : str, optional
-        annotation formating, by default "{x:.2f}"
-    textcolors : tuple, optional
-        A pair of colors.  The first is used for values below a threshold,
-        the second for those above, by default ("black", "white")
-    threshold : float, optional
-        Value in data units according to which the colors from textcolors are
-        applied.  If None (the default) uses the middle of the colormap as
-        separation, by default None
-    textkw : dict, optional
-        All other arguments are forwarded to mpl annotation.
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
-
-    if not isinstance(data, (list, np.ndarray)):
-        data = im.get_array()
-
-    # Normalize the threshold to the images color range.
-    if threshold is not None:
-        threshold = im.norm(threshold)
-    else:
-        threshold = im.norm(data.max()) / 2.0
-
-    # Set default alignment to center, but allow it to be
-    # overwritten by textkw.
-    kw = dict(horizontalalignment="center", verticalalignment="center")
-    kw.update(textkw)
-
-    # Get the formatter in case a string is supplied
-    if isinstance(valfmt, str):
-        valfmt = matplotlib.ticker.StrMethodFormatter(valfmt)
-
-    # Loop over the data and create a `Text` for each "pixel".
-    # Change the text's color depending on the data.
-    texts = []
-    for i in range(data.shape[0]):
-        for j in range(data.shape[1]):
-            kw.update(color=textcolors[int(im.norm(data[i, j]) > threshold)])
-            text = im.axes.text(j, i, valfmt(data[i, j], None), **kw)
-            texts.append(text)
-
-    return texts
-
-
-def plot_association_matrix(
-    assoc_mat,
-    suffix_dic=None,
-    ax=None,
-    cmap="PuOr",
-    cbarlabel=None,
-    figsize=None,
-    show=True,
-    cbar_kw=None,
-    imgshow_kw=None,
-    annotate=False,
-):
-    """plot_association_matrix renders the sorted associations/correlation matrix.
-    The sorting is done using hierarchical clustering,
-    very like in seaborn or other packages.
-    Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1.
-    The uncertainty coefficient is assymmetrical, (approximating how much the elements on the
-    left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical
-    correlations (Pearson's) from -1 to 1
-
-    Parameters
-    ----------
-    assoc_mat : pd.DataFrame
-        the square association frame
-    suffix_dic : Dict[str, str], optional
-        dictionary of data type for adding suffixes to column names
-        in the plotting utility for association matrix, by default None
-    ax : matplotlib.axes.Axes, optional
-        _description_, by default None
-    cmap : str, optional
-        the colormap. Please use a scientific colormap. See the ``scicomap`` package, by default "PuOr"
-    cbarlabel : str, optional
-        the colorbar label, by default None
-    figsize : Tuple[float, float], optional
-        figure size in inches, by default None
-    show : bool, optional
-        Whether or not to display the figure, by default True
-    cbar_kw : Dict, optional
-        colorbar kwargs, by default None
-    imgshow_kw : Dict, optional
-        imgshow kwargs, by default None
-    annotate : bool
-        Whether to annotate or not the colormap
-
-    Returns
-    -------
-    matplotlib.figure and matplotlib.axes.Axes
-        the figure and the axes
-    """
-    # default size if None
-    if figsize is None:
-        ncol = len(assoc_mat)
-        figsize = (ncol / 2.5, ncol / 2.5)
-
-    # provide default to the figure
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
-    else:
-        fig = ax.get_figure()
-    assoc_mat = cluster_sq_matrix(assoc_mat)
-
-    # provide default to imshow
-    if imgshow_kw is None:
-        imgshow_kw = {"vmin": -1, "vmax": 1}
-
-    # provide default to the colorbar
-    if cbar_kw is None:
-        cbar_kw = {"ticks": [-1, -0.5, 0, 0.5, 1]}
-
-    # rename the columns for keeping track of num vs cat columns
-    if suffix_dic is not None:
-        rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
-        assoc_mat = assoc_mat.rename(columns=rename_dic)
-        assoc_mat = assoc_mat.rename(index=rename_dic)
-
-    im, cbar = heatmap(
-        assoc_mat.values,
-        assoc_mat.columns,
-        assoc_mat.columns,
-        ax=ax,
-        cmap=cmap,
-        cbarlabel=cbarlabel,
-        cbar_kw=cbar_kw,
-        **imgshow_kw,
-    )
-
-    if annotate:
-        texts = annotate_heatmap(im, valfmt="{x:.1f}", textcolors=("white", "black"))
-
-    fig.tight_layout()
-    if show:
-        plt.show()
-    return fig, ax
-
-
-def plot_association_matrix_int(
-    assoc_mat, suffix_dic=None, cmap="PuOr", figsize=(800, 600), cluster_matrix=True
-):
-    """Plot the interactive sorted associations/correlation matrix.
-    The sorting is done using hierarchical clustering,
-    very like in seaborn or other packages.
-    Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1.
-    The uncertainty coefficient is assymmetrical, (approximating how much the elements on the
-    left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical
-    correlations (Pearson's) from -1 to 1
-
-    Parameters
-    ----------
-    assoc_mat : pd.DataFrame
-        the square association frame
-    suffix_dic : Dict[str, str], optional
-        dictionary of data type for adding suffixes to column names
-        in the plotting utility for association matrix, by default None
-    cmap : str, optional
-        the colormap. Please use a scientific colormap. See the ``scicomap`` package, by default "PuOr"
-    figsize : Tuple[float, float], optional
-        figure size in inches, by default None
-    cluster_matrix : bool
-        whether or not to cluster the square matrix, by default True
-
-    Returns
-    -------
-    panel.Column
-        the panel object
-    """
-    try:
-        import holoviews as hv
-    except ImportError:
-        raise ImportError(
-            "Holoviews is not installed. Please install it using 'pip install holoviews'."
-        )
-
-    try:
-        import panel as pn
-    except ImportError:
-        raise ImportError(
-            "Panel is not installed. Please install it using 'pip install panel'."
-        )
-
-    cmap = cmap if cmap is not None else "coolwarm"
-
-    # rename the columns for keeping track of num vs cat columns
-    if suffix_dic is not None:
-        rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
-        assoc_mat = assoc_mat.rename(columns=rename_dic)
-        assoc_mat = assoc_mat.rename(index=rename_dic)
-
-    if cluster_matrix:
-        assoc_mat = cluster_sq_matrix(assoc_mat)
-
-    heatmap = hv.HeatMap((assoc_mat.columns, assoc_mat.index, assoc_mat)).redim.range(
-        z=(-1, 1)
-    )
-
-    heatmap.opts(
-        tools=["tap", "hover"],
-        height=figsize[1],
-        width=figsize[0],
-        toolbar="left",
-        colorbar=True,
-        cmap=cmap,
-        fontsize={"title": 12, "ticks": 12, "minor_ticks": 12},
-        xrotation=90,
-        invert_xaxis=False,
-        invert_yaxis=True,
-        xlabel="",
-        ylabel="",
-    )
-    title_str = "**Continuous (con) and Categorical (nom) Associations **"
-    sub_title_str = (
-        "*Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1. The uncertainty "
-        "coefficient is assymmetrical, (approximating how much the elements on the "
-        "left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical "
-        "correlations (Pearson's) from -1 to 1*"
-    )
-    panel_layout = pn.Column(
-        pn.pane.Markdown(title_str, align="start", style={"color": "#575757"}),  # bold
-        pn.pane.Markdown(
-            sub_title_str, align="start", style={"color": "#575757"}
-        ),  # italic
-        heatmap,
-        background="#ebebeb",
-    )
-
-    gc.enable()
-    del assoc_mat
-    gc.collect()
-    return panel_layout
+""" Parallelized Association and Correlation matrix
+ 
+This module provides parallelized methods for computing associations.
+Namely, correlation, correlation ratio, Theil's U, Cramer's V
+
+They are the basis of the MRmr feature selection
+"""
+
+import math
+import warnings
+import matplotlib
+import numpy as np
+import gc
+import pandas as pd
+import scipy.stats as ss
+import matplotlib.pyplot as plt
+import scipy.cluster.hierarchy as sch
+import scipy.stats as ss
+
+
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+from sklearn.utils import as_float_array, safe_sqr, safe_mask
+from multiprocessing import cpu_count
+from itertools import combinations, permutations, product
+from pandas.api.types import is_numeric_dtype
+from scipy.stats import rankdata
+from functools import partial
+
+from .parallel import (
+    parallel_matrix_entries,
+    parallel_df,
+    _compute_series,
+    _compute_matrix_entries,
+)
+from .utils import create_dtype_dict
+
+_PRECISION = 1e-13
+
+########################
+# Redundancy measures
+########################
+
+# For computing the redundancy of all the columns with a given series
+# R(y, x_i) for i=1,..., N --> a series (y is a fixed, chosen column)
+# the main functions are:
+# - the series-series computation (two columns)
+# - the closure for applying the latter function to all columns of a dataframe
+# - the "series" version, using the closure for computing the redundancy with all the cols of the DF
+#
+# For computing the redundancy matrix all the cols combinations of columns
+# R(x_i, x_j) for i, j=1,..., N --> a data frame (either TRIUL if the measure is symmetric
+# or the full matrix if asymmetric)
+# - the series-series computation (two columns), same as for series case
+# - the function looping over a chunk of combinations
+# - the parallelization (sending different chunks to different cores and applying the latter function)
+
+##################
+# CAT-CAT
+##################
+
+
+def weighted_conditional_entropy(x, y, sample_weight=None):
+    """weighted_conditional_entropy computes the weighted conditional entropy between two
+    categorical predictors.
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The predictor vector
+    y : pd.Series of shape (n_samples,)
+        The target vector
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+
+    Returns
+    -------
+    float
+        weighted conditional entropy
+    """
+
+    if sample_weight is None:
+        sample_weight = np.ones(len(x))
+    elif np.count_nonzero(sample_weight) == 0:
+        raise ValueError(
+            "All elements in sample_weight are zero. Cannot divide by zero."
+        )
+
+    df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
+    tot_weight = df["sample_weight"].sum()
+    y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
+    y_counter = y_counter["sample_weight"]
+    xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
+    xy_counter = xy_counter["sample_weight"]
+    h_xy = 0.0
+    for xy in xy_counter.keys():
+        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
+        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
+        if p_xy != 0:
+            h_xy += p_xy * math.log(p_y / p_xy, math.e)
+    return h_xy
+
+
+def weighted_theils_u(x, y, sample_weight=None, as_frame=False):
+    """weighted_theils_u computes the weighted Theil's U statistic between two
+    categorical predictors.
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The predictor vector
+    y : pd.Series of shape (n_samples,)
+        The target vector
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+
+    Returns
+    -------
+    pd.DataFrame
+        predictor names and value of the Theil's U statistic
+    """
+
+    if sample_weight is None:
+        sample_weight = np.ones(len(x))
+
+    df = pd.DataFrame({"x": x, "y": y, "sample_weight": sample_weight})
+    tot_weight = df["sample_weight"].sum()
+    y_counter = df[["y", "sample_weight"]].groupby("y").sum().to_dict()
+    y_counter = y_counter["sample_weight"]
+    x_counter = df[["x", "sample_weight"]].groupby("x").sum().to_dict()
+    x_counter = x_counter["sample_weight"]
+    p_x = list(map(lambda n: n / tot_weight, x_counter.values()))
+    h_x = ss.entropy(p_x)
+    xy_counter = df[["x", "y", "sample_weight"]].groupby(["x", "y"]).sum().to_dict()
+    xy_counter = xy_counter["sample_weight"]
+    h_xy = 0.0
+    for xy in xy_counter.keys():
+        p_xy = xy_counter[xy] / tot_weight if tot_weight != 0 else 0
+        p_y = y_counter[xy[1]] / tot_weight if tot_weight != 0 else 0
+        if p_xy != 0:
+            h_xy += p_xy * math.log(p_y / p_xy, math.e)
+
+    if h_x == 0:
+        return 1.0
+    else:
+        u = (h_x - h_xy) / h_x
+        if abs(u) < _PRECISION or abs(u - 1.0) < _PRECISION:
+            rounded_u = round(u)
+            warnings.warn(
+                f"Rounded U = {u} to {rounded_u}. This is probably due to floating point precision issues.",
+                RuntimeWarning,
+            )
+            u = rounded_u
+
+    if as_frame:
+        return pd.DataFrame({"row": x.name, "col": y.name, "val": u}, index=[0])
+    else:
+        return u
+
+
+def theils_u_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """theils_u_matrix theils_u_matrix computes the weighted Theil's U statistic for
+    categorical-categorical association. This is an asymmetric coefficient: U(x,y) != U(y,x)
+    U(x, y) means the uncertainty of x given y: value is on the range of [0,1] -
+    where 0 means y provides no information about x, and 1 means y provides full information about x
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X :  array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.DataFrame
+        The Theil's U matrix in a tidy (long) format.
+    """
+
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    # Cramer's V only for categorical columns
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+    cat_cols = dtypes_dic["cat"]
+
+    if cat_cols:
+        # explicitely store the unique 2-permutation of column names
+        # permutations and not combinations because U is asymmetric
+        comb_list = [comb for comb in permutations(cat_cols, 2)]
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(cat_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        # parallelize jobs
+        theil_u_matrix_entries = partial(
+            _compute_matrix_entries, func_xyw=weighted_theils_u
+        )
+        lst = parallel_matrix_entries(
+            func=theil_u_matrix_entries,
+            df=X,
+            comb_list=comb_list,
+            sample_weight=sample_weight,
+            n_jobs=-1,
+        )
+        return lst
+    else:
+        return None
+
+
+def theils_u_series(X, target, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """theils_u_series computes the weighted Theil's U statistic for
+    categorical-categorical association. This is an asymmetric coefficient: U(x,y) != U(y,x)
+    U(x, y) means the uncertainty of x given y: value is on the range of [0,1] -
+    where 0 means y provides no information about x, and 1 means y provides full information about x
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        The Theil's U series.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if col_dtypes_dic[target] != "cat":
+        raise TypeError("the target column is not categorical")
+
+    # Cramer's V only for categorical columns
+    cat_cols = dtypes_dic["cat"]
+
+    if cat_cols:
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(cat_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        # parallelize jobs
+        _theil_u = partial(_compute_series, func_xyw=weighted_theils_u)
+        lst = parallel_df(
+            func=_theil_u,
+            df=X[cat_cols],
+            series=X[target],
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+        return lst
+    else:
+        return None
+
+
+def cramer_v(x, y, sample_weight=None, as_frame=False):
+    """cramer_v computes the weighted V statistic of two
+    categorical predictors.
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The predictor vector, the first categorical predictor
+    y : pd.Series of shape (n_samples,)
+        second categorical predictor, order doesn't matter, symmetrical association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+
+    Returns
+    -------
+    pd.DataFrame
+        single row dataframe with the predictor names and the statistic value
+    """
+    tot_weight = sample_weight.sum()
+    weighted_tab = pd.crosstab(x, y, sample_weight, aggfunc=sum).fillna(0)
+    chi2 = ss.chi2_contingency(weighted_tab)[0]
+    phi2 = chi2 / tot_weight
+    r, k = weighted_tab.shape
+    phi2corr = max(0, phi2 - ((k - 1) * (r - 1)) / (tot_weight - 1))
+    rcorr = r - ((r - 1) ** 2) / (tot_weight - 1)
+    kcorr = k - ((k - 1) ** 2) / (tot_weight - 1)
+    v = np.sqrt(phi2corr / min((kcorr - 1), (rcorr - 1)))
+
+    if as_frame:
+        x_name = x.name if isinstance(x, pd.Series) else "var"
+        y_name = y.name if isinstance(y, pd.Series) else "target"
+        return pd.DataFrame(
+            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [v, v]}
+        )
+    else:
+        return v
+
+
+def cramer_v_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """cramer_v_matrix computes the weighted Cramer's V statistic for
+    categorical-categorical association. This is a symmetric coefficient: V(x,y) = V(y,x)
+
+    It uses the corrected Cramer's V statistics, itself based on the chi2 contingency
+    table. The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X :  array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.DataFrame
+        The Cramer's V matrix (lower triangular) in a tidy (long) format.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    # Cramer's V only for categorical columns
+    # in GLM supposed to be all the columns
+    cat_cols = dtypes_dic["cat"]
+
+    if cat_cols:
+        # explicitely store the unique 2-combinations of column names
+        comb_list = [comb for comb in combinations(cat_cols, 2)]
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(cat_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        _cramer_v_matrix_entries = partial(_compute_matrix_entries, func_xyw=cramer_v)
+        lst = parallel_matrix_entries(
+            func=_cramer_v_matrix_entries,
+            df=X,
+            comb_list=comb_list,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+        return lst
+    else:
+        return None
+
+
+def cramer_v_series(X, target, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """cramer_v_series computes the weighted Cramer's V statistic for
+    categorical-categorical association. This is a symmetric coefficient: V(x,y) = V(y,x)
+
+    It uses the corrected Cramer's V statistics, itself based on the chi2 contingency
+    table. The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        The Cramer's V series
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if col_dtypes_dic[target] != "cat":
+        raise TypeError("the target column is not categorical")
+
+    # Cramer's V only for categorical columns
+    cat_cols = dtypes_dic["cat"]
+
+    if cat_cols:
+        X = X[cat_cols]
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(cat_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        # parallelize jobs
+        _cramer_v = partial(_compute_series, func_xyw=cramer_v)
+        lst = parallel_df(
+            func=_cramer_v,
+            df=X[cat_cols],
+            series=X[target],
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+        # concatenate the results
+        # v_df_list = list(chain(*v_df_list))
+        return lst  # pd.concat(lst)
+    else:
+        return None
+
+
+def _weighted_correlation_ratio(*args):
+    """Calculates the Correlation Ratio (sometimes marked by the greek letter Eta)
+    for categorical-continuous association.
+    Answers the question - given a continuous value of a measurement, is it
+    possible to know which category is it associated with?
+    Value is in the range [0,1], where 0 means a category cannot be determined
+    by a continuous measurement, and 1 means a category can be determined with
+    absolute certainty.
+
+    Based on the scikit-learn implementation of the unweighted version.
+
+    Returns
+    -------
+    float
+        value of the correlation ratio
+    """
+    # how many levels (predictor)
+    n_classes = len(args)
+    # convert to float 2-uple d'array
+    args = [as_float_array(a) for a in args]
+    # compute the total weight per level
+    weight_per_class = np.array([a[1].sum() for a in args])
+    # total weight
+    tot_weight = np.sum(weight_per_class)
+    # weighted sum of squares
+    ss_alldata = sum((a[1] * safe_sqr(a[0])).sum(axis=0) for a in args)
+    # list of weighted sums
+    sums_args = [np.asarray((a[0] * a[1]).sum(axis=0)) for a in args]
+    square_of_sums_alldata = sum(sums_args) ** 2
+    square_of_sums_args = [s**2 for s in sums_args]
+    sstot = ss_alldata - square_of_sums_alldata / float(tot_weight)
+    ssbn = 0.0
+    for k, _ in enumerate(args):
+        ssbn += square_of_sums_args[k] / weight_per_class[k]
+    ssbn -= square_of_sums_alldata / float(tot_weight)
+    constant_features_idx = np.where(sstot == 0.0)[0]
+    if np.nonzero(ssbn)[0].size != ssbn.size and constant_features_idx.size:
+        warnings.warn("Features %s are constant." % constant_features_idx, UserWarning)
+    etasq = ssbn / sstot
+    # flatten matrix to vector in sparse case
+    etasq = np.asarray(etasq).ravel()
+    return np.sqrt(etasq)
+
+
+def correlation_ratio(x, y, sample_weight=None, as_frame=False):
+    """Compute the weighted correlation ratio. The association between a continuous predictor (y)
+    and a categorical predictor (x). It can be weighted.
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The categorical predictor vector
+    y : pd.Series of shape (n_samples,)
+        The continuous predictor
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+
+    Returns
+    -------
+    float
+        value of the correlation ratio
+    """
+    if sample_weight is None:
+        sample_weight = np.ones_like(y)
+
+    # one 2-uple per level of the categorical feature x
+    if x.dtype in ["category", "object", "bool"]:
+        args = [
+            (
+                y[safe_mask(y, x == k)],
+                sample_weight[safe_mask(sample_weight, x == k)],
+            )
+            for k in np.unique(x)
+        ]
+    elif y.dtype in ["category", "object", "bool"]:
+        args = [
+            (
+                x[safe_mask(x, y == k)],
+                sample_weight[safe_mask(sample_weight, y == k)],
+            )
+            for k in np.unique(y)
+        ]
+    else:
+        raise TypeError(
+            "one of the two series should be categorical/object and the other numerical"
+        )
+
+    if as_frame:
+        x_name = x.name if isinstance(x, pd.Series) else "var"
+        y_name = y.name if isinstance(y, pd.Series) else "target"
+        v = _weighted_correlation_ratio(*args)[0]
+        return pd.DataFrame(
+            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [v, v]}
+        )
+    else:
+        return _weighted_correlation_ratio(*args)[0]
+
+
+def correlation_ratio_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """correlation_ratio_matrix computes the weighted Correlation Ratio for
+    categorical-numerical association. This is a symmetric coefficient: CR(x,y) = CR(y,x)
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X :  array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.DataFrame
+        The correlation ratio matrix (lower triangular) in a tidy (long) format.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    # Cramer's V only for categorical columns
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+    cat_cols = dtypes_dic["cat"]
+    num_cols = dtypes_dic["num"]
+
+    if cat_cols and num_cols:
+        # explicitely store the unique 2-combinations of column names
+        # the first one should be the categorical predictor
+        comb_list = list(product(cat_cols, num_cols))
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(cat_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        # parallelize jobs
+        corr_ratio_matrix_entries = partial(
+            _compute_matrix_entries, func_xyw=correlation_ratio
+        )
+        lst = parallel_matrix_entries(
+            func=corr_ratio_matrix_entries,
+            df=X,
+            comb_list=comb_list,
+            sample_weight=sample_weight,
+            n_jobs=-1,
+        )
+        return lst
+    else:
+        return None
+
+
+def correlation_ratio_series(
+    X, target, sample_weight=None, n_jobs=-1, handle_na="drop"
+):
+    """correlation_ratio_series computes the weighted correlation ration for
+    categorical-numerical association. This is a symmetric coefficient: CR(x,y) = CR(y,x)
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format, a series.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        The Correlation ratio series (lower triangular) in a tidy (long) format.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if col_dtypes_dic[target] == "cat":
+        # if the target is categorical, pick only num predictors
+        pred_list = dtypes_dic["num"]
+    else:
+        # if the target is numerical, the 2nd pred should be categorical
+        pred_list = dtypes_dic["cat"]
+
+    if pred_list:
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(pred_list))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+        # parallelize jobs
+        _corr_ratio = partial(_compute_series, func_xyw=correlation_ratio)
+        lst = parallel_df(
+            func=_corr_ratio,
+            df=X[pred_list],
+            series=X[target],
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+        return lst
+    else:
+        return None
+
+
+def wm(x, w):
+    """wm computes the weighted mean
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples,)
+        the target array
+    w : array-like of shape (n_samples,)
+        the sample weights array
+
+    Returns
+    -------
+    float
+        weighted mean
+    """
+    return np.sum(x * w) / np.sum(w)
+
+
+def wcov(x, y, w):
+    """wcov computes the weighted covariance
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples,)
+        the perdictor 1 array
+    y : array-like of shape (n_samples,)
+        the perdictor 2 array
+    w : array-like of shape (n_samples,)
+        the sample weights array
+
+    Returns
+    -------
+    float
+        weighted covariance
+    """
+    return np.sum(w * (x - wm(x, w)) * (y - wm(y, w))) / np.sum(w)
+
+
+def wcorr(x, y, w):
+    """wcov computes the weighted Pearson correlation coefficient
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples,)
+        the perdictor 1 array
+    y : array-like of shape (n_samples,)
+        the perdictor 2 array
+    w : array-like of shape (n_samples,)
+        the sample weights array
+
+    Returns
+    -------
+    float
+        weighted correlation coefficient
+    """
+    return wcov(x, y, w) / np.sqrt(wcov(x, x, w) * wcov(y, y, w))
+
+
+def wrank(x, w):
+    """wrank computes the weighted rank
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples,)
+        the target array
+    w : array-like of shape (n_samples,)
+        the sample weights array
+
+    Returns
+    -------
+    float
+        weighted rank
+    """
+    (unique, arr_inv, counts) = np.unique(
+        rankdata(x), return_counts=True, return_inverse=True
+    )
+    a = np.bincount(arr_inv, w)
+    return (np.cumsum(a) - a)[arr_inv] + ((counts + 1) / 2 * (a / counts))[arr_inv]
+
+
+def wspearman(x, y, w):
+    """wcov computes the weighted Spearman correlation coefficient
+
+    Parameters
+    ----------
+    x : array-like of shape (n_samples,)
+        the perdictor 1 array
+    y : array-like of shape (n_samples,)
+        the perdictor 2 array
+    w : array-like of shape (n_samples,)
+        the sample weights array
+
+    Returns
+    -------
+    float
+        Spearman weighted correlation coefficient
+    """
+    return wcorr(wrank(x, w), wrank(y, w), w)
+
+
+def weighted_corr(x, y, sample_weight=None, as_frame=False, method="pearson"):
+    """weighted_corr computes the weighted correlation coefficient (Pearson or Spearman)
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The categorical predictor vector
+    y : pd.Series of shape (n_samples,)
+        The continuous predictor
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+    method : str
+        either "spearman" or "pearson", by default "pearson"
+
+    Returns
+    -------
+    float or pd.DataFrame
+        weighted correlation coefficient
+    """
+
+    if method == "pearson":
+        c = wcorr(x, y, sample_weight)
+    else:
+        c = wspearman(x, y, sample_weight)
+
+    if as_frame:
+        x_name = x.name if isinstance(x, pd.Series) else "var"
+        y_name = y.name if isinstance(y, pd.Series) else "target"
+        return pd.DataFrame(
+            {"row": [x_name, y_name], "col": [y_name, x_name], "val": [c, c]}
+        )
+    else:
+        return c
+
+
+def wcorr_series(
+    X, target, sample_weight=None, n_jobs=-1, handle_na="drop", method="pearson"
+):
+    """wcorr_series computes the weighted correlation coefficient (Pearson or Spearman) for
+    continuous-continuous association. This is an symmetric coefficient: corr(x,y) = corr(y,x)
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+    method : str
+        either "spearman" or "pearson", by default "pearson"
+
+    Returns
+    -------
+    pd.Series
+        The weighted correlation series.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if col_dtypes_dic[target] == "cat":
+        raise TypeError("the target column is categorical")
+
+    num_cols = dtypes_dic["num"]
+    y = X[target]
+
+    if num_cols:
+        _wcorr_method = partial(weighted_corr, method=method)
+        # parallelize jobs
+        _wcorr_method_series = partial(_compute_series, func_xyw=_wcorr_method)
+        return parallel_df(
+            func=_wcorr_method_series,
+            df=X[num_cols],
+            series=y,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+    else:
+        return None
+
+
+def wcorr_matrix(X, sample_weight=None, n_jobs=-1, handle_na="drop", method="pearson"):
+    """wcorr_matrix computes the weighted correlation statistic for
+    (Pearson or Spearman) for continuous-continuous association.
+    This is an symmetric coefficient: corr(x,y) = corr(y,x)
+
+    The computation is embarrassingly parallel and is distributed on available cores.
+    Moreover, the statistic is computed for the unique combinations only and returned in a
+    tidy (long) format.
+
+    Parameters
+    ----------
+    X :  array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+    method : str
+        either "spearman" or "pearson"
+
+    Returns
+    -------
+    pd.DataFrame
+        The Cramer's V matrix (lower triangular) in a tidy (long) format.
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    num_cols = dtypes_dic["num"]
+    if num_cols:
+        # explicitely store the unique 2-combinations of column names
+        comb_list = [comb for comb in combinations(num_cols, 2)]
+        # define the number of cores
+        n_jobs = (
+            min(cpu_count(), len(num_cols))
+            if n_jobs == -1
+            else min(cpu_count(), n_jobs)
+        )
+
+        if (n_jobs > 1) or (method != "pearson"):
+            _wcorr_method = partial(weighted_corr, method=method)
+            _wcorr_method_entries = partial(
+                _compute_matrix_entries, func_xyw=_wcorr_method
+            )
+            lst = parallel_matrix_entries(
+                func=_wcorr_method_entries,
+                df=X,
+                comb_list=comb_list,
+                sample_weight=sample_weight,
+                n_jobs=-1,
+            )
+            return lst
+        else:
+            return (
+                matrix_to_xy(weighted_correlation_1cpu(X, sample_weight, handle_na))
+                .to_frame()
+                .reset_index()
+                .rename(columns={"level_0": "row", "level_1": "col", 0: "val"})
+            )
+    else:
+        return None
+
+
+def weighted_correlation_1cpu(X, sample_weight=None, handle_na="drop"):
+    """weighted_correlation computes the lower triangular weighted correlation matrix
+    using a single CPU, therefore using common numpy linear algebra
+
+    Parameters
+    ----------
+    X :  array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.DataFrame
+        the lower triangular weighted correlation matrix in long format
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+    # degree of freedom for the second moment estimator
+    ddof = 1
+
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    numeric_cols = dtypes_dic["num"]
+
+    if numeric_cols:
+        data = X[numeric_cols]
+        col_idx = data.columns
+        data = data.values
+        sum_weights = sample_weight.sum()
+        weighted_sum = np.dot(data.T, sample_weight)
+        weighted_mean = weighted_sum / sum_weights
+        demeaned = data - weighted_mean
+        sum_of_squares = np.dot((demeaned**2).T, sample_weight)
+        weighted_std = np.sqrt(sum_of_squares / (sum_weights - ddof))
+        weighted_cov = np.dot(sample_weight * demeaned.T, demeaned)
+        weighted_cov /= sum_weights - ddof
+        weighted_corcoef = pd.DataFrame(
+            weighted_cov / weighted_std / weighted_std[:, None],
+            index=col_idx,
+            columns=col_idx,
+        )
+        return weighted_corcoef
+    else:
+        return None
+
+
+#################################
+# association
+# cat-cat + cat-cont + cont-cont
+#################################
+
+
+def association_series(
+    X,
+    target,
+    features=None,
+    sample_weight=None,
+    nom_nom_assoc="theil",
+    num_num_assoc="pearson",
+    nom_num_assoc="correlation_ratio",
+    normalize=False,
+    n_jobs=-1,
+    handle_na="drop",
+):
+    """association_series computes the association matrix for cont-cont, cat-cont and cat-cat.
+    predictors. The weighted correlation matrix is used for the cont-cont predictors.
+    The correlation ratio is used between cont-cat predictors and either the Cramer's V or Theil's U
+    matrix for cat-cat predictors. The Pearson or Spearman correlation coefficient is used for
+    the cont-cont association.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    features : list of str, optional
+        list of features with which to compute the association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    nom_nom_assoc : str or callable
+        If callable, a function which receives two `pd.Series` (and optionally a weight array) and returns a single number.
+        If string, name of nominal-nominal (categorical-categorical) association to use.
+        Options are 'cramer' for Cramer's V or `theil` for Theil's U. If 'theil',
+        heat-map columns are the provided information (U = U(row|col)).
+    num_num_assoc : str or callable
+        If callable, a function which receives two `pd.Series` and returns a single number.
+        If string, name of numerical-numerical association to use. Options are 'pearson'
+        for Pearson's R, 'spearman' for Spearman's R.
+    nom_num_assoc : str or callable
+        If callable, a function which receives two `pd.Series` and returns a single number.
+        If string, name of nominal-numerical association to use. Options are 'correlation_ratio'
+        for correlation ratio
+    normalize : bool
+        either to normalize or not the scores
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        a series with all the association values with the target column
+
+    Raises
+    ------
+    TypeError
+        if features is not None and is not a list of strings
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    if features and is_list_of_str(features):
+        data = X[features + [target]]
+    elif features and (not is_list_of_str(features)):
+        raise TypeError("features is not a list of strings")
+    elif features is None:
+        data = X
+
+    dtypes_dic = create_dtype_dict(X)
+
+    # only numeric, NaN already checked, not repeating the process
+    if X.dtypes.map(is_numeric_dtype).all():
+        if callable(num_num_assoc):
+            return _callable_association_series_fn(
+                assoc_fn=num_num_assoc,
+                X=data,
+                target=target,
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+                kind="num-num",
+            )
+        else:
+            return wcorr_series(
+                data,
+                target,
+                sample_weight,
+                n_jobs,
+                handle_na=None,
+                method=num_num_assoc,
+            )
+
+    # only categorical (here understood as no numerical columns)
+    if not X.dtypes.map(is_numeric_dtype).any():
+        if callable(nom_nom_assoc):
+            return _callable_association_series_fn(
+                assoc_fn=nom_nom_assoc,
+                X=data,
+                target=target,
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+                kind="nom-nom",
+            )
+        elif nom_nom_assoc == "theil":
+            return theils_u_series(data, target, sample_weight, n_jobs, handle_na=None)
+        elif nom_nom_assoc == "cramer":
+            return cramer_v_series(data, target, sample_weight, n_jobs, handle_na=None)
+
+    # cat-num
+    if callable(nom_num_assoc):
+        assoc_series = _callable_association_series_fn(
+            assoc_fn=nom_num_assoc,
+            X=data,
+            target=target,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+            kind="nom-num",
+        )
+    else:
+        assoc_series = correlation_ratio_series(
+            data, target, sample_weight, n_jobs, handle_na=None
+        )
+
+    if normalize:
+        assoc_series = (assoc_series - assoc_series.min()) / np.ptp(assoc_series)
+
+    # cat-cat
+    if dtypes_dic[target] == "cat":
+        if callable(nom_nom_assoc):
+            assoc_series_complement = _callable_association_series_fn(
+                assoc_fn=nom_nom_assoc,
+                X=data,
+                target=target,
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+                kind="nom-nom",
+            )
+        elif nom_nom_assoc == "theil":
+            assoc_series_complement = theils_u_series(
+                data, target, sample_weight, n_jobs, handle_na=None
+            )
+        else:
+            assoc_series_complement = cramer_v_series(
+                data, target, sample_weight, n_jobs, handle_na=None
+            )
+
+        if normalize:
+            assoc_series_complement = (
+                assoc_series_complement - assoc_series_complement.min()
+            ) / np.ptp(assoc_series_complement)
+
+        assoc_series = pd.concat([assoc_series, assoc_series_complement])
+
+    # num-num
+    if dtypes_dic[target] == "num":
+        if callable(num_num_assoc):
+            assoc_series_complement = _callable_association_series_fn(
+                assoc_fn=num_num_assoc,
+                X=data,
+                target=target,
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+                kind="num-num",
+            )
+        else:
+            assoc_series_complement = wcorr_series(
+                data,
+                target,
+                sample_weight,
+                n_jobs,
+                handle_na=None,
+                method=num_num_assoc,
+            )
+
+        if normalize:
+            assoc_series_complement = (
+                assoc_series_complement - assoc_series_complement.min()
+            ) / np.ptp(assoc_series_complement)
+
+        assoc_series = pd.concat([assoc_series, assoc_series_complement])
+
+    return assoc_series.sort_values(ascending=False)
+
+
+def association_matrix(
+    X,
+    sample_weight=None,
+    nom_nom_assoc="theil",
+    num_num_assoc="pearson",
+    nom_num_assoc="correlation_ratio",
+    n_jobs=-1,
+    handle_na="drop",
+    nom_nom_comb=None,
+    num_num_comb=None,
+    nom_num_comb=None,
+):
+    """association_matrix computes the association matrix for cont-cont, cat-cont and cat-cat.
+    predictors. The weighted correlation matrix is used for the cont-cont predictors.
+    The correlation ratio is used between cont-cat predictors and either the Cramer's V or Theil's U
+    matrix for cat-cat predictors.
+
+    The association matrix is not symmetric is Theil is used. The obeservations might be weighted.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    nom_nom_assoc : str or callable
+        If callable, a function which receives two `pd.Series` (and optionally a weight array) and returns a single number.
+        If string, name of nominal-nominal (categorical-categorical) association to use.
+        Options are 'cramer' for Cramer's V or `theil` for Theil's U. If 'theil',
+        heat-map columns are the provided information (U = U(row|col)).
+    num_num_assoc : str or callable
+        If callable, a function which receives two `pd.Series` and returns a single number.
+        If string, name of numerical-numerical association to use. Options are 'pearson'
+        for Pearson's R, 'spearman' for Spearman's R.
+    nom_num_assoc : str or callable
+        If callable, a function which receives two `pd.Series` and returns a single number.
+        If string, name of nominal-numerical association to use. Options are 'correlation_ratio'
+        for correlation ratio
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+    nom_nom_comb_list : list of 2-uple of strings
+        Pairs of column names corresponding to the entries for nom_nom associations.
+        If asymmetrical association, take care of providing an exhaustive list of column name pairs.
+    num_num_comb_list : list of 2-uple of strings
+        Pairs of column names corresponding to the entries for num_num associations
+    nom_num_comb_list : list of 2-uple of strings
+        Pairs of column names corresponding to the entries for nom_num associations
+
+    Returns
+    -------
+    pd.DataFrame
+        the association matrix
+    """
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    # num-num, NaNs already checked above, not repeating the process
+    if callable(num_num_assoc):
+        w_num_num = _callable_association_matrix_fn(
+            assoc_fn=num_num_assoc,
+            cols_comb=num_num_comb,
+            kind="num-num",
+            X=X,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+    else:
+        w_num_num = wcorr_matrix(
+            X, sample_weight, n_jobs, handle_na=None, method=num_num_assoc
+        )
+
+    # nom-num
+    if callable(nom_num_assoc):
+        w_nom_num = _callable_association_matrix_fn(
+            assoc_fn=nom_num_assoc,
+            cols_comb=nom_num_comb,
+            kind="nom-num",
+            X=X,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+    else:
+        w_nom_num = correlation_ratio_matrix(X, sample_weight, n_jobs, handle_na=None)
+
+    # nom-nom
+    if callable(nom_nom_assoc):
+        w_nom_nom = _callable_association_matrix_fn(
+            assoc_fn=nom_nom_assoc,
+            cols_comb=nom_nom_comb,
+            kind="nom-nom",
+            X=X,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+    elif nom_nom_assoc == "cramer":
+        w_nom_nom = cramer_v_matrix(X, sample_weight, n_jobs, handle_na=None)
+    else:
+        w_nom_nom = theils_u_matrix(X, sample_weight, n_jobs, handle_na=None)
+
+    return pd.concat([w_num_num, w_nom_num, w_nom_nom], ignore_index=True)
+
+
+def _callable_association_series_fn(
+    assoc_fn, X, target, sample_weight=None, n_jobs=-1, kind="nom-nom"
+):
+    """_callable_association_series_fn private function, utility for computing association series
+    for a callable custom association
+
+    Parameters
+    ----------
+    assoc_fn : callable
+        a function which receives two `pd.Series` (and optionally a weight array) and returns a single number
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    target : str or int
+        the predictor name or index with which to compute association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    kind : str
+        kind of association, either 'num-num' or 'nom-nom' or 'nom-num'
+
+    Returns
+    -------
+    pd.Series
+        the association series
+
+    Raises
+    ------
+    ValueError
+        if kind is not 'num-num' or 'nom-nom' or 'nom-num'
+    """
+    col_dtypes_dic = create_dtype_dict(X)
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if kind == "nom-nom":
+        if col_dtypes_dic[target] != "cat":
+            raise TypeError("the target column is not categorical")
+        nom_cols = dtypes_dic["cat"]
+        if nom_cols:
+            # define the number of cores
+            n_jobs = (
+                min(cpu_count(), len(nom_cols))
+                if n_jobs == -1
+                else min(cpu_count(), n_jobs)
+            )
+            # parallelize jobs
+            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
+            return parallel_df(
+                func=_assoc_fn,
+                df=X[nom_cols],
+                series=X[target],
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+            )
+        else:
+            return None
+
+    elif kind == "nom-num":
+        if col_dtypes_dic[target] == "cat":
+            # if the target is categorical, pick only num predictors
+            pred_list = dtypes_dic["num"]
+        else:
+            # if the target is numerical, the 2nd pred should be categorical
+            pred_list = dtypes_dic["cat"]
+
+        if pred_list:
+            # define the number of cores
+            n_jobs = (
+                min(cpu_count(), len(pred_list))
+                if n_jobs == -1
+                else min(cpu_count(), n_jobs)
+            )
+            # parallelize jobs
+            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
+            return parallel_df(
+                func=_assoc_fn,
+                df=X[pred_list],
+                series=X[target],
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+            )
+        else:
+            return None
+
+    elif kind == "num-num":
+        num_cols = dtypes_dic["num"]
+        if num_cols:
+            # parallelize jobs
+            _assoc_fn = partial(_compute_series, func_xyw=assoc_fn)
+            return parallel_df(
+                func=_assoc_fn,
+                df=X[num_cols],
+                series=X[target],
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+            )
+        else:
+            return None
+    else:
+        raise ValueError("kind can be 'num-num' or 'nom-num' or 'nom-nom'")
+
+
+def _callable_association_matrix_fn(
+    assoc_fn, X, sample_weight=None, n_jobs=-1, kind="nom-nom", cols_comb=None
+):
+    """_callable_association_matrix_fn private function, utility for computing association matrix
+    for a callable custom association
+
+    Parameters
+    ----------
+    assoc_fn : callable
+        a function which receives two `pd.Series` (and optionally a weight array) and returns a single number
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    kind : str
+        kind of association, either 'num-num' or 'nom-nom' or 'nom-num'
+    cols_comb : list of 2-uple of str, optional
+        combination of column names (list of 2-uples of strings)
+
+    Returns
+    -------
+    pd.DataFrame
+        the association matrix
+    """
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    if cols_comb is None:
+        if kind == "num-num":
+            selected_cols = dtypes_dic["num"]
+        elif kind == "nom-nom":
+            selected_cols = dtypes_dic["cat"]
+        elif kind == "nom-num":
+            cat_cols = dtypes_dic["cat"]
+            num_cols = dtypes_dic["num"]
+            if cat_cols and num_cols:
+                # explicitely store the unique 2-combinations of column names
+                # the first one should be the categorical predictor
+                selected_cols = list(product(cat_cols, num_cols))
+        else:
+            selected_cols = None
+
+        if selected_cols:
+            # explicitely store the unique 2-combinations of column names
+            cols_comb = [comb for comb in combinations(selected_cols, 2)]
+            _assoc_fn = partial(_compute_matrix_entries, func_xyw=assoc_fn)
+            assoc = parallel_matrix_entries(
+                func=_assoc_fn,
+                df=X,
+                comb_list=cols_comb,
+                sample_weight=sample_weight,
+                n_jobs=n_jobs,
+            )
+
+        else:
+            assoc = None
+    else:
+        _assoc_fn = partial(_compute_matrix_entries, func_xyw=assoc_fn)
+        assoc = parallel_matrix_entries(
+            func=_assoc_fn,
+            df=X,
+            comb_list=cols_comb,
+            sample_weight=sample_weight,
+            n_jobs=n_jobs,
+        )
+    return assoc
+
+
+################################
+# Association predictor-target
+################################
+
+
+def f_oneway_weighted(*args):
+    """
+    Calculate the weighted F-statistic for one-way ANOVA (continuous target, categorical predictor).
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples,)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
+
+    Returns
+    -------
+    float
+        The value of the F-statistic.
+
+    Notes
+    -----
+    The F-statistic is calculated as:
+
+    .. math::
+        F(rf) = \\frac{\\sum_i (\\bar{Y}_{i \\bullet} - \\bar{Y})^2 / (K-1)}{\\sum_i \\sum_k (\\bar{Y}_{ij} - \\bar{Y}_{i\\bullet})^2 / (N - K)}
+    """
+    # how many levels (predictor)
+    n_classes = len(args)
+    # convert to float 2-uple d'array
+    args = [as_float_array(a) for a in args]
+    # compute the total weight per level
+    weight_per_class = np.array([a[1].sum() for a in args])
+    # total weight
+    tot_weight = np.sum(weight_per_class)
+    # weighted sum of squares
+    ss_alldata = sum((a[1] * safe_sqr(a[0])).sum(axis=0) for a in args)
+    # list of weighted sums
+    sums_args = [np.asarray((a[0] * a[1]).sum(axis=0)) for a in args]
+    square_of_sums_alldata = sum(sums_args) ** 2
+    square_of_sums_args = [s**2 for s in sums_args]
+    sstot = ss_alldata - square_of_sums_alldata / float(tot_weight)
+    ssbn = 0.0
+    for k, _ in enumerate(args):
+        ssbn += square_of_sums_args[k] / weight_per_class[k]
+    ssbn -= square_of_sums_alldata / float(tot_weight)
+    sswn = sstot - ssbn
+    dfbn = n_classes - 1
+    dfwn = tot_weight - n_classes
+    msb = ssbn / float(dfbn)
+    msw = sswn / float(dfwn)
+    constant_features_idx = np.where(msw == 0.0)[0]
+    if np.nonzero(msb)[0].size != msb.size and constant_features_idx.size:
+        warnings.warn("Features %s are constant." % constant_features_idx, UserWarning)
+    f = msb / msw
+    # flatten matrix to vector in sparse case
+    f = np.asarray(f).ravel()
+    return f
+
+
+def f_cat_regression(x, y, sample_weight=None, as_frame=False):
+    """f_cat_regression computes the weighted ANOVA F-value for the provided sample.
+    (continuous target, categorical predictor)
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The predictor vector, the first categorical predictor
+    y : pd.Series of shape (n_samples,)
+        second categorical predictor, order doesn't matter, symmetrical association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+
+    Returns
+    -------
+    float
+        value of the F-statistic
+    """
+    if sample_weight is None:
+        sample_weight = np.ones_like(y)
+
+    # one 2-uple per level of the categorical feature x
+    args = [
+        (
+            y[safe_mask(y, x == k)],
+            sample_weight[safe_mask(sample_weight, x == k)],
+        )
+        for k in np.unique(x)
+    ]
+
+    if as_frame:
+        x_name = x.name if isinstance(x, pd.Series) else "var"
+        y_name = y.name if isinstance(y, pd.Series) else "target"
+        return pd.DataFrame(
+            {"row": x_name, "col": y_name, "val": f_oneway_weighted(*args)[0]},
+            index=[0],
+        )
+    else:
+        return f_oneway_weighted(*args)[0]
+
+
+def f_cat_regression_parallel(X, y, sample_weight=None, n_jobs=-1, handle_na="drop"):
+    """f_cat_regression_parallel computes the weighted ANOVA F-value for the provided categorical predictors
+    using parallelization of the code (continuous target, categorical predictor).
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    y : array-like of shape (n_samples,)
+        The target vector
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        the value of the F-statistic for each predictor
+    """
+
+    # Cramer's V only for categorical columns
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    cat_cols = dtypes_dic["cat"]
+
+    if not isinstance(y, pd.Series):
+        y = pd.Series(y)
+        y.name = "target"
+
+    target = y.name
+    X[target] = y.values
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    y = X[target].copy()
+    X = X.drop(target, axis=1)
+
+    # define the number of cores
+    n_jobs = min(cpu_count(), X.shape[1]) if n_jobs == -1 else min(cpu_count(), n_jobs)
+    # parallelize jobs
+    _f_stat_cat = partial(_compute_series, func_xyw=f_cat_regression)
+    return parallel_df(
+        func=_f_stat_cat,
+        df=X[cat_cols],
+        series=y,
+        sample_weight=sample_weight,
+        n_jobs=n_jobs,
+    )
+
+
+def f_cont_regression_parallel(
+    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
+):
+    """Univariate linear regression tests returning F-statistic.
+
+    Quick linear model for testing the effect of a single regressor,
+    sequentially for many regressors.
+    This is done in 2 steps:
+    1. The cross-correlation between each regressor and the target is computed using:
+           E[(X[:, i] - mean(X[:, i])) * (y - mean(y))] / (std(X[:, i]) * std(y))
+    2. It is converted to an F score ranks features in the same order if all the features
+       are positively correlated with the target.
+    Note that it is therefore recommended as a feature selection criterion to identify
+    potentially predictive features for a downstream classifier, irrespective of
+    the sign of the association with the target variable.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
+    n_jobs : int, optional
+        The number of cores to use for the computation, by default -1.
+    handle_na : str, optional
+        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to
+        be finite. There are two cases where the F-statistic is expected to not
+        be finite:
+        - when the target `y` or some features in `X` are constant. In this
+          case, the Pearson's R correlation is not defined leading to obtain
+          `np.nan` values in the F-statistic and p-value. When
+          `force_finite=True`, the F-statistic is set to `0.0` and the
+          associated p-value is set to `1.0`.
+        - when a feature in `X` is perfectly correlated (or
+          anti-correlated) with the target `y`. In this case, the F-statistic
+          is expected to be `np.inf`. When `force_finite=True`, the F-statistic
+          is set to `np.finfo(dtype).max`.
+
+    Returns
+    -------
+    f_statistic : array-like of shape (n_features,)
+        F-statistic for each feature.
+    """
+    if not isinstance(y, pd.Series):
+        y = pd.Series(y)
+        y.name = "target"
+
+    target = y.name
+    X[target] = y.values
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    correlation_coefficient = wcorr_series(X, target, sample_weight, n_jobs, handle_na)
+
+    deg_of_freedom = y.size - 2
+    corr_coef_squared = correlation_coefficient**2
+
+    with np.errstate(divide="ignore", invalid="ignore"):
+        f_statistic = corr_coef_squared / (1 - corr_coef_squared) * deg_of_freedom
+
+    if force_finite and not np.isfinite(f_statistic).all():
+        # case where there is a perfect (anti-)correlation
+        # f-statistics can be set to the maximum and p-values to zero
+        mask_inf = np.isinf(f_statistic)
+        f_statistic[mask_inf] = np.finfo(f_statistic.dtype).max
+        # case where the target or some features are constant
+        # f-statistics would be minimum and thus p-values large
+        mask_nan = np.isnan(f_statistic)
+        f_statistic[mask_nan] = 0.0
+
+    return f_statistic.drop(labels=[target]).sort_values(ascending=False)
+
+
+def f_stat_regression_parallel(
+    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
+):
+    """
+    Compute the weighted explained variance for the provided categorical and numerical predictors using parallelization.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
+    n_jobs : int, optional
+        The number of cores to use for the computation, by default -1.
+    handle_na : str, optional
+        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to be finite.
+        There are two cases where the F-statistic is expected to not be finite:
+        - When the target `y` or some features in `X` are constant. In this case,
+          the Pearson's R correlation is not defined leading to obtain `np.nan`
+          values in the F-statistic and p-value. When `force_finite=True`, the
+          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
+        - When a feature in `X` is perfectly correlated (or anti-correlated)
+          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
+          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
+
+    Returns
+    -------
+    pd.Series
+        The value of the F-statistic for each predictor.
+    """
+    f_stat_cont_series = f_cont_regression_parallel(
+        X,
+        y,
+        sample_weight,
+        n_jobs,
+        force_finite=force_finite,
+        handle_na=handle_na,
+    )
+    f_stat_cat_series = f_cat_regression_parallel(
+        X, y, sample_weight, n_jobs, handle_na=handle_na
+    )
+
+    # normalize the scores
+    # correlation coefficient varies in the range [-1, 1]
+    # correlation ratio varies in the range [0, 1]
+    # Cramer's V varies in the range [0, 1]
+    # Theil's U varies in the range [0, 1]
+    # F-statistic varies in the range [0, +inf] but both kind of F stat are not necessary on the same scale
+    # in order to have a similar scale and compare both kind, one can studentize them
+    if X.shape[1] > 1:
+        f_stat_cont_series = (
+            f_stat_cont_series - f_stat_cont_series.mean()
+        ) / f_stat_cont_series.std()
+        f_stat_cat_series = (
+            f_stat_cat_series - f_stat_cat_series.mean()
+        ) / f_stat_cat_series.std()
+
+    return pd.concat([f_stat_cont_series, f_stat_cat_series]).sort_values(
+        ascending=False
+    )
+
+
+def f_cont_classification(x, y, sample_weight=None, as_frame=False):
+    """f_cont_classification computes the weighted ANOVA F-value for the provided sample.
+    Categorical target, continuous predictor.
+
+    Parameters
+    ----------
+    x : pd.Series of shape (n_samples,)
+        The predictor vector, the first categorical predictor
+    y : pd.Series of shape (n_samples,)
+        second categorical predictor, order doesn't matter, symmetrical association
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    as_frame: bool
+        return output as a dataframe or a float
+
+    Returns
+    -------
+    float :
+        value of the F-statistic
+    """
+    if sample_weight is None:
+        sample_weight = np.ones_like(y)
+
+    # one 2-uple per level of the categorical target y, continuous predictor x
+    args = [
+        (
+            x[safe_mask(x, y == k)],
+            sample_weight[safe_mask(sample_weight, y == k)],
+        )
+        for k in np.unique(y)
+    ]
+
+    if as_frame:
+        x_name = x.name if isinstance(x, pd.Series) else "var"
+        y_name = y.name if isinstance(y, pd.Series) else "target"
+        return pd.DataFrame(
+            {"row": x_name, "col": y_name, "val": f_oneway_weighted(*args)[0]},
+            index=[0],
+        )
+    else:
+        return f_oneway_weighted(*args)[0]
+
+
+def f_cont_classification_parallel(
+    X, y, sample_weight=None, n_jobs=-1, handle_na="drop"
+):
+    """f_cont_classification_parallel computes the weighted ANOVA F-value
+    for the provided categorical predictors using parallelization of the code.
+    Categorical target, continuous predictor.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        The set of regressors that will be tested sequentially
+    y : array-like of shape (n_samples,)
+        The target vector
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    pd.Series
+        the value of the F-statistic for each predictor
+    """
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+
+    num_cols = dtypes_dic["num"]
+
+    if not isinstance(y, pd.Series):
+        y = pd.Series(y)
+        y.name = "target"
+
+    target = y.name
+    X[target] = y.values
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    y = X[target].copy()
+    X = X.drop(target, axis=1)
+
+    # define the number of cores
+    n_jobs = min(cpu_count(), X.shape[1]) if n_jobs == -1 else min(cpu_count(), n_jobs)
+    # parallelize jobs
+    _f_stat_cont_clf = partial(_compute_series, func_xyw=f_cont_classification)
+    return parallel_df(
+        func=_f_stat_cont_clf,
+        df=X[num_cols],
+        series=y,
+        sample_weight=sample_weight,
+        n_jobs=n_jobs,
+    )
+
+
+def f_cat_classification_parallel(
+    X,
+    y,
+    sample_weight=None,
+    n_jobs=-1,
+    force_finite=True,
+    handle_na="drop",
+):
+    """
+    Univariate information dependence.
+
+    It ranks features in the same order if all the features are positively correlated with the target.
+    Note that it is therefore recommended as a feature selection criterion to identify
+    potentially predictive features for a downstream classifier, irrespective of
+    the sign of the association with the target variable.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
+    n_jobs : int, optional
+        The number of cores to use for the computation, by default -1.
+    handle_na : str, optional
+        Either drop rows with NaN, fill NaN with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to
+        be finite. There are two cases where the F-statistic is expected to not
+        be finite:
+            - when the target `y` or some features in `X` are constant. In this
+              case, the Pearson's R correlation is not defined leading to obtain
+              `np.nan` values in the F-statistic and p-value. When
+              `force_finite=True`, the F-statistic is set to `0.0` and the
+              associated p-value is set to `1.0`.
+            - when a feature in `X` is perfectly correlated (or
+              anti-correlated) with the target `y`. In this case, the F-statistic
+              is expected to be `np.inf`. When `force_finite=True`, the F-statistic
+              is set to `np.finfo(dtype).max`.
+
+    Returns
+    -------
+    f_statistic : array-like of shape (n_features,)
+        F-statistic for each feature.
+    """
+    if not isinstance(y, pd.Series):
+        y = pd.Series(y)
+        y.name = "target"
+
+    target = y.name
+    X[target] = y.values
+    # sanity checks
+    X, sample_weight = _check_association_input(X, sample_weight, handle_na)
+
+    deg_of_freedom = y.size - 2
+
+    theils_u_coef = theils_u_series(X, target, sample_weight, n_jobs, handle_na)
+    theils_u_coef_squared = theils_u_coef**2
+
+    with np.errstate(divide="ignore", invalid="ignore"):
+        f_statistic = (
+            theils_u_coef_squared / (1 - theils_u_coef_squared) * deg_of_freedom
+        )
+
+    if force_finite and not np.isfinite(f_statistic).all():
+        # case where there is a perfect (anti-)correlation
+        # f-statistics can be set to the maximum and p-values to zero
+        mask_inf = np.isinf(f_statistic)
+        f_statistic[mask_inf] = np.finfo(f_statistic.dtype).max
+        # case where the target or some features are constant
+        # f-statistics would be minimum and thus p-values large
+        mask_nan = np.isnan(f_statistic)
+        f_statistic[mask_nan] = 0.0
+
+    return f_statistic.drop(labels=[target]).sort_values(ascending=False)
+
+
+def f_stat_classification_parallel(
+    X, y, sample_weight=None, n_jobs=-1, force_finite=True, handle_na="drop"
+):
+    """
+    Compute the weighted ANOVA F-value for the provided categorical and numerical predictors using parallelization.
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        The predictor dataframe.
+    y : array-like of shape (n_samples,)
+        The target vector.
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None.
+    n_jobs : int, optional
+        The number of cores to use for the computation, by default -1.
+    handle_na : str, optional
+        Either drop rows with NA, fill NA with 0, or do nothing, by default "drop".
+    force_finite : bool, optional
+        Whether or not to force the F-statistics and associated p-values to be finite.
+        There are two cases where the F-statistic is expected to not be finite:
+        - When the target `y` or some features in `X` are constant. In this case,
+          the Pearson's R correlation is not defined leading to obtain `np.nan`
+          values in the F-statistic and p-value. When `force_finite=True`, the
+          F-statistic is set to `0.0` and the associated p-value is set to `1.0`.
+        - When a feature in `X` is perfectly correlated (or anti-correlated)
+          with the target `y`. In this case, the F-statistic is expected to be `np.inf`.
+          When `force_finite=True`, the F-statistic is set to `np.finfo(dtype).max`.
+
+    Returns
+    -------
+    pd.Series
+        The value of the F-statistic for each predictor.
+    """
+    f_stat_cont_series = f_cont_classification_parallel(
+        X, y, sample_weight, n_jobs, handle_na=handle_na
+    )
+    f_stat_cat_series = f_cat_classification_parallel(
+        X,
+        y,
+        sample_weight,
+        n_jobs,
+        handle_na=handle_na,
+        force_finite=force_finite,
+    )
+
+    # normalize the scores
+    # correlation ratio varies in the range [0, 1]
+    # Cramer's V varies in the range [0, 1]
+    # Theil's U varies in the range [0, 1]
+    # F-statistic varies in the range [0, +inf]
+    # Both kind of F stat are not necessarily on the same scale
+    # one can studentize them
+    if X.shape[1] > 1:
+        f_stat_cont_series = (
+            f_stat_cont_series - f_stat_cont_series.mean()
+        ) / f_stat_cont_series.std()
+        f_stat_cat_series = (
+            f_stat_cat_series - f_stat_cat_series.mean()
+        ) / f_stat_cat_series.std()
+
+    return pd.concat([f_stat_cont_series, f_stat_cat_series]).sort_values(
+        ascending=False
+    )
+
+
+############
+# Utilities
+############
+
+
+def _check_association_input(X, sample_weight=None, handle_na="drop"):
+    """_check_association_input private function. Check the inputs,
+    convert X to a pd.DataFrame if needed, adds column names if non are provided.
+    Check if the sample_weight is None or of the right dimensionality and handle NA
+    according to the chosen methods (drop, fill, None).
+
+    Parameters
+    ----------
+    X : array-like of shape (n_samples, n_features)
+        predictor dataframe
+    sample_weight : array-like of shape (n_samples,), optional
+        The weight vector, by default None
+    handle_na : str, optional
+        either drop rows with na, fill na with 0 or do nothing, by default "drop"
+
+    Returns
+    -------
+    tuple
+        the dataframe and the sample weights
+
+    Raises
+    ------
+    ValueError
+        if sample_weight contains NA
+    """
+
+    if not isinstance(X, pd.DataFrame):
+        X = pd.DataFrame(X, columns=[f"pred_{i}" for i in range(X.shape[1])])
+
+    # sanity checks
+    if sample_weight is None:
+        sample_weight = np.ones(len(X))
+    elif ~np.isfinite(sample_weight).all():
+        raise ValueError("sample weights contains nans or nulls")
+
+    if isinstance(sample_weight, pd.Series):
+        sample_weight = sample_weight.to_numpy()
+
+    single_value_columns_set = set()
+    for c in X.columns:
+        if X[c].nunique() == 1:
+            single_value_columns_set.add(c)
+
+    if single_value_columns_set:
+        warnings.warn(
+            f"{single_value_columns_set} columns have been removed (single unique values)"
+        )
+
+    # handle nans
+    if handle_na is None:
+        pass
+    elif handle_na == "drop":
+        # mask the na
+        na_mask = (~X.isnull().any(axis=1)).values
+        if na_mask.any():
+            X, sample_weight = X.loc[na_mask, :], sample_weight[na_mask]
+    else:
+        X = X.fillna(0)
+    return X, sample_weight
+
+
+def is_list_of_str(str_list):
+    """Raise an exception if ``str_list`` is not a list of strings
+    Parameters
+    ----------
+    str_list : list
+        to list to be tested
+
+    Raises
+    ------
+    TypeError
+        if ``str_list`` is not a ``list[str]``
+    """
+    if str_list is not None:
+        if not (
+            isinstance(str_list, list) and all(isinstance(s, str) for s in str_list)
+        ):
+            return False
+        else:
+            return True
+
+
+def matrix_to_xy(df, columns=None, reset_index=False):
+    """matrix_to_xy wide to long format of the association matrix
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        the wide format of the association matrix
+    columns : list of str, optional
+        list of column names, by default None
+    reset_index : bool, optional
+        wether to reset_index or not, by default False
+
+    Returns
+    -------
+    pd.DataFrame
+        the long format of the association matrix
+    """
+    bool_index = np.tril(np.ones(df.shape), 0).astype(bool)
+    xy = (
+        df.where(bool_index).stack().reset_index()
+        if reset_index
+        else df.where(bool_index).stack()
+    )
+    if reset_index:
+        xy.columns = columns or ["row", "col", "val"]
+    return xy
+
+
+def xy_to_matrix(xy):
+    """xy_to_matrix long to wide format of the association matrix
+
+    Parameters
+    ----------
+    xy : pd.DataFrame
+        the long format of the association matrix, 3 columns.
+
+    Returns
+    -------
+    pd.DataFrame
+
+    """
+    xy = xy.pivot(index="row", columns="col").fillna(0)
+    xy.columns = xy.columns.droplevel(0)
+    return xy.rename_axis(None, axis=1).rename_axis(None, axis=0)
+
+
+###############
+# visualization
+###############
+
+
+def cluster_sq_matrix(sq_matrix, method="ward"):
+    """
+    Apply agglomerative clustering to sort a square correlation matrix.
+
+    Parameters
+    ----------
+    sq_matrix : pd.DataFrame
+        A square correlation matrix.
+    method : str, optional
+        The linkage method, by default "ward".
+
+    Returns
+    -------
+    pd.DataFrame
+        A sorted square matrix.
+
+    Example
+    -------
+    >>> from some_module import association_matrix, cluster_sq_matrix
+
+    >>> assoc = association_matrix(iris_df, plot=False)
+    >>> assoc_clustered = cluster_sq_matrix(assoc, method="complete")
+    """
+    d = sch.distance.pdist(sq_matrix.values)
+    L = sch.linkage(d, method=method)
+    ind = sch.fcluster(L, 0.5 * d.max(), "distance")
+    columns = [sq_matrix.columns.tolist()[i] for i in list((np.argsort(ind)))]
+    sq_matrix = sq_matrix.reindex(columns, axis=1)
+    sq_matrix = sq_matrix.reindex(columns, axis=0)
+    return sq_matrix
+
+
+def heatmap(
+    data, row_labels, col_labels, ax=None, cbar_kw=None, cbarlabel="", **kwargs
+):
+    """heatmap Create a heatmap from a numpy array and two lists of labels.
+
+    Parameters
+    ----------
+    data : array-like of shape (M, N)
+        matrix to plot
+    row_labels : array-like of shape (M,)
+        labels for the rows
+    col_labels : array-like of shape (N,)
+        labels for the columns
+    ax : matplotlib.axes.Axes, optional
+        A `matplotlib.axes.Axes` instance to which the heatmap is plotted.  If
+        not provided, use current axes or create a new one, by default None
+    cbar_kw : dict, optional
+         A dictionary with arguments to `matplotlib.Figure.colorbar`, by default None
+    cbarlabel : str, optional
+        The label for the colorbar, by default ""
+    kwargs : dict, optional
+        All other arguments are forwarded to `imshow`.
+
+    Returns
+    -------
+    tuple
+        imgshow and cbar objects
+    """
+
+    if ax is None:
+        ax = plt.gca()
+
+    if cbar_kw is None:
+        cbar_kw = {}
+
+    # Plot the heatmap
+    im = ax.imshow(data, **kwargs)
+
+    # Create colorbar
+    divider = make_axes_locatable(ax)
+
+    ax_cb = divider.append_axes("right", size="5%", pad=0.05)
+    fig = ax.get_figure()
+    fig.add_axes(ax_cb)
+
+    cbar = ax.figure.colorbar(im, cax=ax_cb, **cbar_kw)
+    cbar.ax.set_ylabel(cbarlabel, rotation=-90, va="bottom")
+
+    # Show all ticks and label them with the respective list entries.
+    ax.set_xticks(np.arange(data.shape[1]), labels=col_labels)
+    ax.set_yticks(np.arange(data.shape[0]), labels=row_labels)
+
+    # Let the horizontal axes labeling appear on top.
+    ax.tick_params(top=False, bottom=True, labeltop=False, labelbottom=True)
+
+    # Rotate the tick labels and set their alignment.
+    plt.setp(ax.get_xticklabels(), rotation=90, ha="right", rotation_mode="anchor")
+
+    # Turn spines off and create white grid.
+    ax.spines[:].set_visible(False)
+
+    ax.set_xticks(np.arange(data.shape[1] + 1) - 0.5, minor=True)
+    ax.set_yticks(np.arange(data.shape[0] + 1) - 0.5, minor=True)
+    ax.grid(which="minor", color="w", linestyle="-", linewidth=2)
+    ax.tick_params(which="minor", bottom=False, left=False)
+
+    return im, cbar
+
+
+def annotate_heatmap(
+    im,
+    data=None,
+    valfmt="{x:.2f}",
+    textcolors=("black", "white"),
+    threshold=None,
+    **textkw,
+):
+    """annotate_heatmap annotates a heatmap
+
+    Parameters
+    ----------
+    im : matplotlib.axes.Axes
+        The AxesImage to be labeled
+    data : array-like of shape (M, N), optional
+        data to illustrate, if none is provided the function retrieves
+        the array of the mlp obkect, by default None
+    valfmt : str, optional
+        annotation formating, by default "{x:.2f}"
+    textcolors : tuple, optional
+        A pair of colors.  The first is used for values below a threshold,
+        the second for those above, by default ("black", "white")
+    threshold : float, optional
+        Value in data units according to which the colors from textcolors are
+        applied.  If None (the default) uses the middle of the colormap as
+        separation, by default None
+    textkw : dict, optional
+        All other arguments are forwarded to mpl annotation.
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+
+    if not isinstance(data, (list, np.ndarray)):
+        data = im.get_array()
+
+    # Normalize the threshold to the images color range.
+    if threshold is not None:
+        threshold = im.norm(threshold)
+    else:
+        threshold = im.norm(data.max()) / 2.0
+
+    # Set default alignment to center, but allow it to be
+    # overwritten by textkw.
+    kw = dict(horizontalalignment="center", verticalalignment="center")
+    kw.update(textkw)
+
+    # Get the formatter in case a string is supplied
+    if isinstance(valfmt, str):
+        valfmt = matplotlib.ticker.StrMethodFormatter(valfmt)
+
+    # Loop over the data and create a `Text` for each "pixel".
+    # Change the text's color depending on the data.
+    texts = []
+    for i in range(data.shape[0]):
+        for j in range(data.shape[1]):
+            kw.update(color=textcolors[int(im.norm(data[i, j]) > threshold)])
+            text = im.axes.text(j, i, valfmt(data[i, j], None), **kw)
+            texts.append(text)
+
+    return texts
+
+
+def plot_association_matrix(
+    assoc_mat,
+    suffix_dic=None,
+    ax=None,
+    cmap="PuOr",
+    cbarlabel=None,
+    figsize=None,
+    show=True,
+    cbar_kw=None,
+    imgshow_kw=None,
+    annotate=False,
+):
+    """plot_association_matrix renders the sorted associations/correlation matrix.
+    The sorting is done using hierarchical clustering,
+    very like in seaborn or other packages.
+    Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1.
+    The uncertainty coefficient is assymmetrical, (approximating how much the elements on the
+    left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical
+    correlations (Pearson's) from -1 to 1
+
+    Parameters
+    ----------
+    assoc_mat : pd.DataFrame
+        the square association frame
+    suffix_dic : Dict[str, str], optional
+        dictionary of data type for adding suffixes to column names
+        in the plotting utility for association matrix, by default None
+    ax : matplotlib.axes.Axes, optional
+        _description_, by default None
+    cmap : str, optional
+        the colormap. Please use a scientific colormap. See the ``scicomap`` package, by default "PuOr"
+    cbarlabel : str, optional
+        the colorbar label, by default None
+    figsize : Tuple[float, float], optional
+        figure size in inches, by default None
+    show : bool, optional
+        Whether or not to display the figure, by default True
+    cbar_kw : Dict, optional
+        colorbar kwargs, by default None
+    imgshow_kw : Dict, optional
+        imgshow kwargs, by default None
+    annotate : bool
+        Whether to annotate or not the colormap
+
+    Returns
+    -------
+    matplotlib.figure and matplotlib.axes.Axes
+        the figure and the axes
+    """
+    # default size if None
+    if figsize is None:
+        ncol = len(assoc_mat)
+        figsize = (ncol / 2.5, ncol / 2.5)
+
+    # provide default to the figure
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+    else:
+        fig = ax.get_figure()
+    assoc_mat = cluster_sq_matrix(assoc_mat)
+
+    # provide default to imshow
+    if imgshow_kw is None:
+        imgshow_kw = {"vmin": -1, "vmax": 1}
+
+    # provide default to the colorbar
+    if cbar_kw is None:
+        cbar_kw = {"ticks": [-1, -0.5, 0, 0.5, 1]}
+
+    # rename the columns for keeping track of num vs cat columns
+    if suffix_dic is not None:
+        rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
+        assoc_mat = assoc_mat.rename(columns=rename_dic)
+        assoc_mat = assoc_mat.rename(index=rename_dic)
+
+    im, cbar = heatmap(
+        assoc_mat.values,
+        assoc_mat.columns,
+        assoc_mat.columns,
+        ax=ax,
+        cmap=cmap,
+        cbarlabel=cbarlabel,
+        cbar_kw=cbar_kw,
+        **imgshow_kw,
+    )
+
+    if annotate:
+        texts = annotate_heatmap(im, valfmt="{x:.1f}", textcolors=("white", "black"))
+
+    fig.tight_layout()
+    if show:
+        plt.show()
+    return fig, ax
+
+
+def plot_association_matrix_int(
+    assoc_mat, suffix_dic=None, cmap="PuOr", figsize=(800, 600), cluster_matrix=True
+):
+    """Plot the interactive sorted associations/correlation matrix.
+    The sorting is done using hierarchical clustering,
+    very like in seaborn or other packages.
+    Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1.
+    The uncertainty coefficient is assymmetrical, (approximating how much the elements on the
+    left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical
+    correlations (Pearson's) from -1 to 1
+
+    Parameters
+    ----------
+    assoc_mat : pd.DataFrame
+        the square association frame
+    suffix_dic : Dict[str, str], optional
+        dictionary of data type for adding suffixes to column names
+        in the plotting utility for association matrix, by default None
+    cmap : str, optional
+        the colormap. Please use a scientific colormap. See the ``scicomap`` package, by default "PuOr"
+    figsize : Tuple[float, float], optional
+        figure size in inches, by default None
+    cluster_matrix : bool
+        whether or not to cluster the square matrix, by default True
+
+    Returns
+    -------
+    panel.Column
+        the panel object
+    """
+    try:
+        import holoviews as hv
+    except ImportError:
+        raise ImportError(
+            "Holoviews is not installed. Please install it using 'pip install holoviews'."
+        )
+
+    try:
+        import panel as pn
+    except ImportError:
+        raise ImportError(
+            "Panel is not installed. Please install it using 'pip install panel'."
+        )
+
+    cmap = cmap if cmap is not None else "coolwarm"
+
+    # rename the columns for keeping track of num vs cat columns
+    if suffix_dic is not None:
+        rename_dic = {c: f"{c}_{suffix_dic[c]}" for c in assoc_mat.columns}
+        assoc_mat = assoc_mat.rename(columns=rename_dic)
+        assoc_mat = assoc_mat.rename(index=rename_dic)
+
+    if cluster_matrix:
+        assoc_mat = cluster_sq_matrix(assoc_mat)
+
+    heatmap = hv.HeatMap((assoc_mat.columns, assoc_mat.index, assoc_mat)).redim.range(
+        z=(-1, 1)
+    )
+
+    heatmap.opts(
+        tools=["tap", "hover"],
+        height=figsize[1],
+        width=figsize[0],
+        toolbar="left",
+        colorbar=True,
+        cmap=cmap,
+        fontsize={"title": 12, "ticks": 12, "minor_ticks": 12},
+        xrotation=90,
+        invert_xaxis=False,
+        invert_yaxis=True,
+        xlabel="",
+        ylabel="",
+    )
+    title_str = "**Continuous (con) and Categorical (nom) Associations **"
+    sub_title_str = (
+        "*Categorical(nom): uncertainty coefficient & correlation ratio from 0 to 1. The uncertainty "
+        "coefficient is assymmetrical, (approximating how much the elements on the "
+        "left PROVIDE INFORMATION on elements in the row). Continuous(con): symmetrical numerical "
+        "correlations (Pearson's) from -1 to 1*"
+    )
+    panel_layout = pn.Column(
+        pn.pane.Markdown(title_str, align="start", style={"color": "#575757"}),  # bold
+        pn.pane.Markdown(
+            sub_title_str, align="start", style={"color": "#575757"}
+        ),  # italic
+        heatmap,
+        background="#ebebeb",
+    )
+
+    gc.enable()
+    del assoc_mat
+    gc.collect()
+    return panel_layout
```

### Comparing `arfs-2.0.4/src/arfs/benchmark.py` & `arfs-2.0.5/src/arfs/benchmark.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-"""Benchmark Feature Selection
-
-This module provides utilities for comparing and benchmarking feature selection methods
-
-Module Structure:
------------------
-- ``sklearn_pimp_bench``: function for comparing using the sklearn permutation importance
-- ``compare_varimp``: function for comparing using 3 kinds of var.imp.
-- ``highlight_tick``: function for highlighting specific (genuine or noise for instance) predictors in the importance chart
-"""
-
-from __future__ import print_function, division
-
-import itertools
-from matplotlib import pyplot as plt
-from sklearn.model_selection import train_test_split
-from sklearn.inspection import permutation_importance
-
-from sklearn.base import clone
-
-from .preprocessing import OrdinalEncoderPandas
-
-
-def sklearn_pimp_bench(model, X, y, task="regression", sample_weight=None):
-    """Benchmark using sklearn permutation importance, works for regression and classification.
-
-    Parameters
-    ----------
-    model: object
-        An estimator that has not been fitted, sklearn compatible.
-    X : ndarray or DataFrame, shape (n_samples, n_features)
-        Data on which permutation importance will be computed.
-    y : array-like or None, shape (n_samples, ) or (n_samples, n_classes)
-        Targets for supervised or None for unsupervised.
-    task : str, optional
-        kind of task, either 'regression' or 'classification", by default 'regression'
-    sample_weight : array-like of shape (n_samples,), optional
-        Sample weights, by default None
-
-    Returns
-    -------
-    plt.figure
-        the figure corresponding to the feature selection
-
-    Raises
-    ------
-    ValueError
-        if task is not 'regression' or 'classification'
-    """
-
-    # for lightGBM cat feat as contiguous int
-    # https://lightgbm.readthedocs.io/en/latest/Advanced-Topics.html
-    # same for Random Forest and XGBoost (OHE leads to deep and sparse trees).
-    # For illustrations, see
-    # https://towardsdatascience.com/one-hot-encoding-is-making-
-    # your-tree-based-ensembles-worse-heres-why-d64b282b5769
-
-    # X, cat_var_df, inv_mapper, mapper = cat_var(X)
-    X = OrdinalEncoderPandas().fit_transform(X)
-
-    if task == "regression":
-        stratify = None
-    elif task == "classification":
-        stratify = y
-    else:
-        raise ValueError("`task` should be either 'regression' or 'classification' ")
-
-    if sample_weight is not None:
-        X_train, X_test, y_train, y_test, w_train, w_test = train_test_split(
-            X, y, sample_weight, stratify=stratify, random_state=42
-        )
-    else:
-        X_train, X_test, y_train, y_test = train_test_split(
-            X, y, stratify=stratify, random_state=42
-        )
-        w_train, w_test = None, None
-
-    # lightgbm faster and better than RF
-
-    model.fit(X_train, y_train, sample_weight=w_train)
-    result = permutation_importance(
-        model,
-        X_test,
-        y_test,
-        n_repeats=10,
-        random_state=42,
-        n_jobs=2,
-        sample_weight=w_test,
-    )
-
-    sorted_idx = result.importances_mean.argsort()
-    # Plot (5 predictors per inch)
-    fig, ax = plt.subplots(figsize=(16, X.shape[1] / 5))
-    ax.boxplot(
-        result.importances[sorted_idx].T, vert=False, labels=X_test.columns[sorted_idx]
-    )
-    ax.set_title("Permutation Importances (test set)")
-    ax.tick_params(axis="both", which="major", labelsize=9)
-    fig.tight_layout()
-    indices = [i for i, s in enumerate(X_test.columns[sorted_idx]) if "random" in s]
-    [fig.gca().get_yticklabels()[idx].set_color("red") for idx in indices]
-    indices = [i for i, s in enumerate(X_test.columns[sorted_idx]) if "genuine" in s]
-    [fig.gca().get_yticklabels()[idx].set_color("green") for idx in indices]
-    plt.show()
-    return fig
-
-
-def compare_varimp(feat_selector, models, X, y, sample_weight=None):
-    """Utility function to compare the results for the three possible kind of feature importance
-
-    Parameters
-    ----------
-    feat_selector : object
-        an instance of either Leshy, BoostaGRoota or GrootCV
-    models : list of objects
-        list of tree based scikit-learn estimators
-    X : pd.DataFrame, shape (n_samples, n_features)
-        the predictors frame
-    y : pd.Series
-        the target (same length as X)
-    sample_weight : None or pd.Series, optional
-        sample weights if any, by default None
-    """
-
-    varimp_list = ["shap", "fastshap", "pimp", "native"]
-    for model, varimp in itertools.product(models, varimp_list):
-        print(
-            "=" * 20
-            + " "
-            + str(feat_selector.__class__.__name__)
-            + " - testing: {mod:>25} for var.imp: {vimp:<15} ".format(
-                mod=str(model.__class__.__name__), vimp=varimp
-            )
-            + "=" * 20
-        )
-        # change the varimp
-        feat_selector.importance = varimp
-        # change model
-        mod_clone = clone(model, safe=True)
-        feat_selector.estimator = mod_clone
-        # fit the feature selector
-        feat_selector.fit(X=X, y=y, sample_weight=sample_weight)
-        # print the results
-        print(feat_selector.selected_features_)
-        fig = feat_selector.plot_importance(n_feat_per_inch=5)
-
-        if fig is not None:
-            # highlight synthetic random variable
-            fig = highlight_tick(figure=fig, str_match="random")
-            fig = highlight_tick(figure=fig, str_match="genuine", color="green")
-            plt.show()
-
-
-def highlight_tick(str_match, figure, color="red", axis="y"):
-    """Highlight the x/y tick-labels if they contains a given string
-
-    Parameters
-    ----------
-    str_match : str
-        the substring to match
-    figure : object
-        the matplotlib figure
-    color : str, optional
-        the matplotlib color for highlighting tick-labels, by default 'red'
-    axis : str, optional
-        axis to use for highlighting, by default 'y'
-
-    Returns
-    -------
-    plt.figure
-        the modified matplotlib figure
-
-    Raises
-    ------
-    ValueError
-        if axis is not 'x' or 'y'
-    """
-
-    if axis == "y":
-        labels = [item.get_text() for item in figure.gca().get_yticklabels()]
-        indices = [i for i, s in enumerate(labels) if str_match in s]
-        [figure.gca().get_yticklabels()[idx].set_color(color) for idx in indices]
-    elif axis == "x":
-        labels = [item.get_text() for item in figure.gca().get_xticklabels()]
-        indices = [i for i, s in enumerate(labels) if str_match in s]
-        [figure.gca().get_xticklabels()[idx].set_color(color) for idx in indices]
-    else:
-        raise ValueError("`axis` should be a string, either 'y' or 'x'")
-
-    return figure
+"""Benchmark Feature Selection
+
+This module provides utilities for comparing and benchmarking feature selection methods
+
+Module Structure:
+-----------------
+- ``sklearn_pimp_bench``: function for comparing using the sklearn permutation importance
+- ``compare_varimp``: function for comparing using 3 kinds of var.imp.
+- ``highlight_tick``: function for highlighting specific (genuine or noise for instance) predictors in the importance chart
+"""
+
+from __future__ import print_function, division
+
+import itertools
+from matplotlib import pyplot as plt
+from sklearn.model_selection import train_test_split
+from sklearn.inspection import permutation_importance
+
+from sklearn.base import clone
+
+from .preprocessing import OrdinalEncoderPandas
+
+
+def sklearn_pimp_bench(model, X, y, task="regression", sample_weight=None):
+    """Benchmark using sklearn permutation importance, works for regression and classification.
+
+    Parameters
+    ----------
+    model: object
+        An estimator that has not been fitted, sklearn compatible.
+    X : ndarray or DataFrame, shape (n_samples, n_features)
+        Data on which permutation importance will be computed.
+    y : array-like or None, shape (n_samples, ) or (n_samples, n_classes)
+        Targets for supervised or None for unsupervised.
+    task : str, optional
+        kind of task, either 'regression' or 'classification", by default 'regression'
+    sample_weight : array-like of shape (n_samples,), optional
+        Sample weights, by default None
+
+    Returns
+    -------
+    plt.figure
+        the figure corresponding to the feature selection
+
+    Raises
+    ------
+    ValueError
+        if task is not 'regression' or 'classification'
+    """
+
+    # for lightGBM cat feat as contiguous int
+    # https://lightgbm.readthedocs.io/en/latest/Advanced-Topics.html
+    # same for Random Forest and XGBoost (OHE leads to deep and sparse trees).
+    # For illustrations, see
+    # https://towardsdatascience.com/one-hot-encoding-is-making-
+    # your-tree-based-ensembles-worse-heres-why-d64b282b5769
+
+    # X, cat_var_df, inv_mapper, mapper = cat_var(X)
+    X = OrdinalEncoderPandas().fit_transform(X)
+
+    if task == "regression":
+        stratify = None
+    elif task == "classification":
+        stratify = y
+    else:
+        raise ValueError("`task` should be either 'regression' or 'classification' ")
+
+    if sample_weight is not None:
+        X_train, X_test, y_train, y_test, w_train, w_test = train_test_split(
+            X, y, sample_weight, stratify=stratify, random_state=42
+        )
+    else:
+        X_train, X_test, y_train, y_test = train_test_split(
+            X, y, stratify=stratify, random_state=42
+        )
+        w_train, w_test = None, None
+
+    # lightgbm faster and better than RF
+
+    model.fit(X_train, y_train, sample_weight=w_train)
+    result = permutation_importance(
+        model,
+        X_test,
+        y_test,
+        n_repeats=10,
+        random_state=42,
+        n_jobs=2,
+        sample_weight=w_test,
+    )
+
+    sorted_idx = result.importances_mean.argsort()
+    # Plot (5 predictors per inch)
+    fig, ax = plt.subplots(figsize=(16, X.shape[1] / 5))
+    ax.boxplot(
+        result.importances[sorted_idx].T, vert=False, labels=X_test.columns[sorted_idx]
+    )
+    ax.set_title("Permutation Importances (test set)")
+    ax.tick_params(axis="both", which="major", labelsize=9)
+    fig.tight_layout()
+    indices = [i for i, s in enumerate(X_test.columns[sorted_idx]) if "random" in s]
+    [fig.gca().get_yticklabels()[idx].set_color("red") for idx in indices]
+    indices = [i for i, s in enumerate(X_test.columns[sorted_idx]) if "genuine" in s]
+    [fig.gca().get_yticklabels()[idx].set_color("green") for idx in indices]
+    plt.show()
+    return fig
+
+
+def compare_varimp(feat_selector, models, X, y, sample_weight=None):
+    """Utility function to compare the results for the three possible kind of feature importance
+
+    Parameters
+    ----------
+    feat_selector : object
+        an instance of either Leshy, BoostaGRoota or GrootCV
+    models : list of objects
+        list of tree based scikit-learn estimators
+    X : pd.DataFrame, shape (n_samples, n_features)
+        the predictors frame
+    y : pd.Series
+        the target (same length as X)
+    sample_weight : None or pd.Series, optional
+        sample weights if any, by default None
+    """
+
+    varimp_list = ["shap", "fastshap", "pimp", "native"]
+    for model, varimp in itertools.product(models, varimp_list):
+        print(
+            "=" * 20
+            + " "
+            + str(feat_selector.__class__.__name__)
+            + " - testing: {mod:>25} for var.imp: {vimp:<15} ".format(
+                mod=str(model.__class__.__name__), vimp=varimp
+            )
+            + "=" * 20
+        )
+        # change the varimp
+        feat_selector.importance = varimp
+        # change model
+        mod_clone = clone(model, safe=True)
+        feat_selector.estimator = mod_clone
+        # fit the feature selector
+        feat_selector.fit(X=X, y=y, sample_weight=sample_weight)
+        # print the results
+        print(feat_selector.selected_features_)
+        fig = feat_selector.plot_importance(n_feat_per_inch=5)
+
+        if fig is not None:
+            # highlight synthetic random variable
+            fig = highlight_tick(figure=fig, str_match="random")
+            fig = highlight_tick(figure=fig, str_match="genuine", color="green")
+            plt.show()
+
+
+def highlight_tick(str_match, figure, color="red", axis="y"):
+    """Highlight the x/y tick-labels if they contains a given string
+
+    Parameters
+    ----------
+    str_match : str
+        the substring to match
+    figure : object
+        the matplotlib figure
+    color : str, optional
+        the matplotlib color for highlighting tick-labels, by default 'red'
+    axis : str, optional
+        axis to use for highlighting, by default 'y'
+
+    Returns
+    -------
+    plt.figure
+        the modified matplotlib figure
+
+    Raises
+    ------
+    ValueError
+        if axis is not 'x' or 'y'
+    """
+
+    if axis == "y":
+        labels = [item.get_text() for item in figure.gca().get_yticklabels()]
+        indices = [i for i, s in enumerate(labels) if str_match in s]
+        [figure.gca().get_yticklabels()[idx].set_color(color) for idx in indices]
+    elif axis == "x":
+        labels = [item.get_text() for item in figure.gca().get_xticklabels()]
+        indices = [i for i, s in enumerate(labels) if str_match in s]
+        [figure.gca().get_xticklabels()[idx].set_color(color) for idx in indices]
+    else:
+        raise ValueError("`axis` should be a string, either 'y' or 'x'")
+
+    return figure
```

### Comparing `arfs-2.0.4/src/arfs/dataset/data/boston_bunch.joblib` & `arfs-2.0.5/src/arfs/dataset/data/boston_bunch.joblib`

 * *Files identical despite different names*

### Comparing `arfs-2.0.4/src/arfs/dataset/data/housing.zip` & `arfs-2.0.5/src/arfs/dataset/data/housing.zip`

 * *Files identical despite different names*

### Comparing `arfs-2.0.4/src/arfs/feature_selection/allrelevant.py` & `arfs-2.0.5/src/arfs/feature_selection/allrelevant.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,2614 +1,2614 @@
-"""This module provides 3 different methods to perform 'all relevant feature selection'
-
-
-Reference:
-----------
-NILSSON, Roland, PEÑA, José M., BJÖRKEGREN, Johan, et al.
-Consistent feature selection for pattern recognition in polynomial time.
-Journal of Machine Learning Research, 2007, vol. 8, no Mar, p. 589-612.
-
-KURSA, Miron B., RUDNICKI, Witold R., et al.
-Feature selection with the Boruta package.
-J Stat Softw, 2010, vol. 36, no 11, p. 1-13.
-
-https://github.com/chasedehan/BoostARoota
-
-The module structure
---------------------
-- The ``Leshy`` class, a heavy re-work of ``BorutaPy`` class
-  itself a modified version of Boruta, the pull request I submitted and still pending:
-  https://github.com/scikit-learn-contrib/boruta_py/pull/100
-
-- The ``BoostAGroota`` class, a modified version of BoostARoota, PR still to be submitted
-  https://github.com/chasedehan/BoostARoota
-
-- The ``GrootCV`` class for a new method for all relevant feature selection using a lightgGBM model,
-  cross-validated SHAP importances and shadowing.
-
-Original BorutaPy version
--------------------------
-Author: Daniel Homola <dani.homola@gmail.com>
-
-Original code and method by: Miron B Kursa, https://m2.icm.edu.pl/boruta/
-Modified by Thomas Bury, pull request:
-https://github.com/scikit-learn-contrib/boruta_py/pull/100
-Waiting for merging
-
-https://github.com/scikit-learn-contrib/boruta_py/pull/100
-is a new PR based on #77 making all the changes optional. Waiting for merge
-
-Leshy is a re-work of the PR I submitted.
-
-License: BSD 3 clause
-
-"""
-
-from __future__ import print_function, division
-import operator
-import warnings
-import time
-import shap
-import numpy as np
-import pandas as pd
-import lightgbm as lgb
-import matplotlib as mpl
-import matplotlib.pyplot as plt
-import scipy as sp
-
-from typing import Tuple
-from tqdm.auto import tqdm
-from sklearn.utils import check_random_state, check_X_y
-from sklearn.base import BaseEstimator, is_regressor, is_classifier, clone
-
-from sklearn.utils.validation import check_is_fitted
-from sklearn.feature_selection._base import SelectorMixin
-from sklearn.model_selection import RepeatedKFold, train_test_split
-from sklearn.inspection import permutation_importance
-from sklearn.utils.validation import _check_sample_weight
-from matplotlib.lines import Line2D
-from lightgbm import early_stopping
-
-
-from ..utils import (
-    check_if_tree_based,
-    is_lightgbm,
-    is_catboost,
-    create_dtype_dict,
-    get_pandas_cat_codes,
-    validate_sample_weight,
-)
-
-########################################################################################
-#
-# Main Classes and Methods
-# Provide a fit, transform and fit_transform method
-#
-########################################################################################
-# !/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-NO_FEATURE_SELECTED_WARNINGS = "No feature selected - No data to plot"
-ARFS_COLOR_LIST = [
-    "#000000",
-    "#7F3C8D",
-    "#11A579",
-    "#3969AC",
-    "#F2B701",
-    "#E73F74",
-    "#80BA5A",
-    "#E68310",
-    "#008695",
-    "#CF1C90",
-    "#F97B72",
-]
-BLUE = "#2590fa"
-YELLOW = "#f0be00"
-RED = "#b51204"
-BCKGRD_COLOR = "#f5f5f5"
-PLT_PARAMS = {
-    "axes.prop_cycle": plt.cycler(color=ARFS_COLOR_LIST),
-    "axes.facecolor": BCKGRD_COLOR,
-    "patch.edgecolor": BCKGRD_COLOR,
-    "figure.facecolor": BCKGRD_COLOR,
-    "axes.edgecolor": BCKGRD_COLOR,
-    "savefig.edgecolor": BCKGRD_COLOR,
-    "savefig.facecolor": BCKGRD_COLOR,
-    "grid.color": "#d2d2d2",
-    "lines.linewidth": 1.5,
-}
-PLOT_KWARGS = dict(
-    kind="box",
-    boxprops=dict(linestyle="-", linewidth=1.5, color="gray", facecolor="gray"),
-    flierprops=dict(linestyle="-", linewidth=1.5, color="gray"),
-    medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
-    whiskerprops=dict(linestyle="-", linewidth=1.5, color="gray"),
-    capprops=dict(linestyle="-", linewidth=1.5, color="gray"),
-    showfliers=False,
-    grid=True,
-    rot=0,
-    vert=False,
-    patch_artist=True,
-    fontsize=9,
-)
-
-
-class Leshy(SelectorMixin, BaseEstimator):
-    """This is an improved version of BorutaPy which itself is an
-    improved Python implementation of the Boruta R package.
-    Boruta is an all relevant feature selection method, while most other are
-    minimal optimal; this means it tries to find all features carrying
-    information usable for prediction, rather than finding a possibly compact
-    subset of features on which some estimator has a minimal error.
-    Why bother with all relevant feature selection?
-    When you try to understand the phenomenon that made your data, you should
-    care about all factors that contribute to it, not just the bluntest signs
-    of it in context of your methodology (minimal optimal set of features
-    by definition depends on your estimator choice).
-
-    Parameters
-    ----------
-    estimator : object
-        A supervised learning estimator, with a 'fit' method that returns the
-        ``feature_importances_`` attribute. Important features must correspond to
-        high absolute values in the ``feature_importances_``
-    n_estimators : int or string, default = 1000
-        If int sets the number of estimators in the chosen ensemble method.
-        If 'auto' this is determined automatically based on the size of the
-        dataset. The other parameters of the used estimators need to be set
-        with initialisation.
-    perc : int, default = 100
-        Instead of the max we use the percentile defined by the user, to pick
-        our threshold for comparison between shadow and real features. The max
-        tend to be too stringent. This provides a finer control over this. The
-        lower perc is the more false positives will be picked as relevant but
-        also the less relevant features will be left out. The usual trade-off.
-        The default is essentially the vanilla Boruta corresponding to the max.
-    alpha : float, default = 0.05
-        Level at which the corrected p-values will get rejected in both
-        correction steps.
-    importance : str, default = 'shap'
-        The kind of variable importance used to compare and discriminate original
-        vs shadow predictors. Note that the builtin tree importance (gini/impurity based
-        importance) is biased towards numerical and large cardinality predictors, even
-        if they are random. Shapley values and permutation imp. are robust w.r.t those predictors.
-        Possible values: 'shap' (Shapley values), 'fastshap' (FastTreeShap implementation),
-        'pimp' (permutation importance) and 'native' (Gini/impurity)
-    two_step : Boolean, default = True
-        If you want to use the original implementation of Boruta with Bonferroni
-        correction only set this to False.
-    max_iter : int, default = 100
-        The number of maximum iterations to perform.
-    random_state : int, RandomState instance or None; default=None
-        If int, random_state is the seed used by the random number generator;
-        If RandomState instance, random_state is the random number generator;
-        If None, the random number generator is the RandomState instance used
-        by `np.random`.
-    verbose : int, default=0
-        Controls verbosity of output. 0: no output, 1: displays iteration number,
-        2: which features have been selected already
-
-
-    Attributes
-    ----------
-    n_features_ : int
-        The number of selected features.
-    support_ : array of shape [n_features]
-        The mask of selected features - only confirmed ones are True.
-    support_weak_ : array of shape [n_features]
-        The mask of selected tentative features, which haven't gained enough
-        support during the max_iter number of iterations.
-    selected_features_ : list of str
-        the list of columns to keep
-    ranking_ : array of shape [n_features]
-        The feature ranking, such that ``ranking_[i]`` corresponds to the
-        ranking position of the i-th feature. Selected (i.e., estimated
-        best) features are assigned rank one and tentative features are assigned
-        rank 2.
-    ranking_absolutes_ : array of shape [n_features]
-        The absolute feature ranking as ordered by selection process. It does not guarantee
-        that this order is correct for all models. For a model agnostic ranking, see the
-        the attribute ``ranking``
-    cat_name : list of str
-        the name of the categorical columns
-    cat_idx : list of int
-        the index of the categorical columns
-    imp_real_hist : array
-        array of the historical feature importance of the real predictors
-    sha_max : float
-        the maximum feature importance of the shadow predictors
-    col_names : list of str
-        the names of the real predictors
-
-
-    Examples
-    --------
-    >>> import pandas as pd
-    >>> from sklearn.ensemble import RandomForestClassifier
-    >>> from boruta import BorutaPy
-    >>>
-    >>> # load X and y
-    >>> # NOTE BorutaPy accepts numpy arrays only, hence the .values attribute
-    >>> X = pd.read_csv('examples/test_X.csv', index_col=0).values
-    >>> y = pd.read_csv('examples/test_y.csv', header=None, index_col=0).values
-    >>> y = y.ravel()
-    >>>
-    >>> # define random forest classifier, with utilising all cores and
-    >>> # sampling in proportion to y labels
-    >>> rf = RandomForestClassifier(n_jobs=-1, class_weight='balanced', max_depth=5)
-    >>>
-    >>> # define Boruta feature selection method
-    >>> feat_selector = Leshy(rf, n_estimators='auto', verbose=2, random_state=1)
-    >>>
-    >>> # find all relevant features - 5 features should be selected
-    >>> feat_selector.fit(X, y)
-    >>>
-    >>> # check selected features - first 5 features are selected
-    >>> feat_selector.selected_features_
-    >>>
-    >>> # check ranking of features
-    >>> feat_selector.ranking_
-    >>>
-    >>> # call transform() on X to filter it down to selected features
-    >>> X_filtered = feat_selector.transform(X)
-
-    References
-    ----------
-    See the original paper [1]_ for more details.
-
-    ..[1] Kursa M., Rudnicki W., "Feature Selection with the Boruta Package"
-        Journal of Statistical Software, Vol. 36, Issue 11, Sep 2010
-
-    """
-
-    def __init__(
-        self,
-        estimator,
-        n_estimators=1000,
-        perc=90,
-        alpha=0.05,
-        importance="shap",
-        two_step=True,
-        max_iter=100,
-        random_state=None,
-        verbose=0,
-        keep_weak=False,
-    ):
-        self.estimator = estimator
-        self.n_estimators = n_estimators
-        self.perc = perc
-        self.alpha = alpha
-        self.two_step = two_step
-        self.max_iter = max_iter
-        self.random_state = random_state
-        self.random_state_instance = None
-        self.verbose = verbose
-        self.keep_weak = keep_weak
-        self.importance = importance
-        self.cat_name = None
-        self.cat_idx = None
-        # Catboost doesn't allow to change random seed after fitting
-        self.is_cat = is_catboost(estimator)
-        self.is_lgb = is_lightgbm(estimator)
-        # plotting
-        self.imp_real_hist = None
-        self.sha_max = None
-        self.n_features_ = 0
-        self.support_ = None
-        self.support_weak_ = None
-
-    def fit(self, X, y, sample_weight=None):
-        """Fits the Boruta feature selection with the provided estimator.
-
-        Parameters
-        ----------
-        X : array-like, shape = [n_samples, n_features]
-            The training input samples.
-        y : array-like, shape = [n_samples]
-            The target values.
-        sample_weight : array-like, shape = [n_samples], default=None
-            Individual weights for each sample
-
-        Returns
-        -------
-        self : object
-            Nothing but attributes
-
-        """
-        try:
-            from fasttreeshap import TreeExplainer as FastTreeExplainer
-        except ImportError:
-            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
-            self.importance = "shap"
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a dataframe")
-
-        self.imp_real_hist = np.empty((0, X.shape[1]), float)
-        self._fit(X, y, sample_weight=sample_weight)
-        self.selected_features_ = self.feature_names_in_[self.support_]
-        self.not_selected_features_ = self.feature_names_in_[~self.support_]
-
-        return self
-
-    def transform(self, X):
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    @mpl.rc_context(PLT_PARAMS)
-    def plot_importance(self, n_feat_per_inch=5):
-        """Boxplot of the variable importance, ordered by magnitude
-        The max shadow variable importance illustrated by the dashed line.
-        Requires to apply the fit method first.
-
-        Parameters
-        ----------
-        n_feat_per_inch : int, default=5
-            number of features to plot per inch (for scaling the figure)
-
-        Returns
-        -------
-        fig : plt.figure
-            the matplotlib figure object containing the boxplot
-        """
-
-        if self.imp_real_hist is None:
-            raise ValueError("Use the fit method first to compute the var.imp")
-
-        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
-        vimp_df = vimp_df.reindex(
-            vimp_df.mean().sort_values(ascending=True).index, axis=1
-        )
-
-        if vimp_df.dropna().empty:
-            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
-            return None
-        else:
-            fig, ax = plt.subplots(figsize=(16, vimp_df.shape[1] / n_feat_per_inch))
-            bp = vimp_df.plot(**PLOT_KWARGS, ax=ax)
-
-            n_strong = sum(self.support_)
-            n_weak = np.sum(self.support_weak_)
-            n_discarded = np.sum(~(self.support_ | self.support_weak_))
-            box_face_col = (
-                [BLUE] * n_strong + [YELLOW] * n_weak + ["gray"] * n_discarded
-            )
-            for c in range(len(box_face_col)):
-                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_facecolor(
-                    box_face_col[c]
-                )
-                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_color(
-                    box_face_col[c]
-                )
-
-            xrange = vimp_df.max(skipna=True).max(skipna=True) - vimp_df.min(
-                skipna=True
-            ).min(skipna=True)
-            bp.set_xlim(left=vimp_df.min(skipna=True).min(skipna=True) - 0.10 * xrange)
-
-            custom_lines = [
-                Line2D([0], [0], color=BLUE, lw=5),
-                Line2D([0], [0], color=YELLOW, lw=5),
-                Line2D([0], [0], color="gray", lw=5),
-                Line2D([0], [0], linestyle="--", color=RED, lw=2),
-            ]
-            bp.legend(
-                custom_lines,
-                ["confirmed", "tentative", "rejected", "sha. max"],
-                loc="lower right",
-            )
-            ax.axvline(x=self.sha_max, linestyle="--", color=RED)
-            ax.set_title("Leshy importance and selected predictors")
-            return fig
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def _more_tags(self):
-        return {"allow_nan": True, "requires_y": True}
-
-    def _fit(self, X_raw, y, sample_weight=None):
-        """Private method. See the methods overview in the documentation
-        for explanation of the process
-
-        Parameters
-        ----------
-        X_raw : array-like, shape = [n_samples, n_features]
-            The training input samples.
-        y : array-like, shape = [n_samples]
-            The target values.
-        sample_weight : array-like, shape = [n_samples], default=None
-            Individual weights for each sample
-
-        Returns
-        -------
-        self : object
-            Nothing but attributes
-        """
-
-        start_time = time.time()
-        # the basic cat features encoding
-        # is performed when getting importances
-        # because the columns are dynamically created/rejected
-        X = X_raw
-
-        # only sklearn requires to fillna data
-        # modern GBM implementations can handle this
-        # X = X.fillna(0)
-        y = pd.Series(y).fillna(0) if not isinstance(y, pd.Series) else y.fillna(0)
-
-        # check input params
-        self._check_params(X, y)
-        sample_weight = validate_sample_weight(sample_weight)
-        self.random_state = check_random_state(self.random_state)
-
-        # setup variables for Boruta
-        n_sample, n_feat = X.shape
-        _iter = 1
-        # holds the decision about each feature:
-        # 0  - default state = tentative in original code
-        # 1  - accepted in original code
-        # -1 - rejected in original code
-        dec_reg = np.zeros(n_feat, dtype=int)
-        # counts how many times a given feature was more important than
-        # the best of the shadow features
-        hit_reg = np.zeros(n_feat, dtype=int)
-        # these record the history of the iterations
-        imp_history = np.zeros(n_feat, dtype=float)
-        sha_max_history = []
-
-        # set n_estimators
-        if self.n_estimators != "auto":
-            self.estimator.set_params(n_estimators=self.n_estimators)
-
-        dec_reg, sha_max_history, imp_history, imp_sha_max = self.select_features(
-            X=X, y=y, sample_weight=sample_weight
-        )
-        confirmed, tentative = _get_confirmed_and_tentative(dec_reg)
-        tentative = _select_tentative(tentative, imp_history, sha_max_history)
-        self._calculate_support(confirmed, tentative, n_feat)
-
-        # for plotting
-        self.imp_real_hist = imp_history
-        self.sha_max = imp_sha_max
-
-        # absolute and relative ranking
-        self._calculate_absolute_ranking()
-        self._calculate_relative_ranking(
-            n_feat=n_feat,
-            tentative=tentative,
-            confirmed=confirmed,
-            imp_history=imp_history,
-        )
-        self._print_result(dec_reg, _iter, start_time)
-        return self
-
-    def _get_tree_num(self, n_feat):
-        """private method, get a good estimated for the number of trees
-           given the number of features
-
-        Parameters
-        ----------
-        n_feat : int
-            The number of features
-
-        Returns
-        -------
-        n_estimators : int
-            the number of trees
-        """
-        depth = (
-            self.estimator.get_params()["max_depth"]
-            if not self.is_cat
-            else self.estimator.get_param("max_depth")
-        )
-        if depth is None:
-            depth = 10
-        # how many times a feature should be considered on average
-        f_repr = 100
-        # n_feat * 2 because the training matrix is extended with n shadow features
-        multi = (n_feat * 2) / (np.sqrt(n_feat * 2) * depth)
-        n_estimators = int(multi * f_repr)
-        return n_estimators
-
-    def _add_shadows_get_imps(self, X, y, sample_weight, dec_reg):
-        """Add a shuffled copy of the columns (shadows) and get the feature
-        importance of the augmented data set
-
-        Parameters
-        ----------
-        X: pd.DataFrame of shape [n_samples, n_features]
-            predictor matrix
-        y: pd.series of shape [n_samples]
-            target
-        sample_weight: array-like, shape = [n_samples], default=None
-            Individual weights for each sample
-        dec_reg: array
-            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
-        Returns
-        -------
-         imp_real: array
-            feature importance of the real predictors
-         imp_sha: array
-            feature importance of the shadow predictors
-        """
-        # find features that are tentative still
-        x_cur_ind = np.where(dec_reg >= 0)[0]
-        x_cur = X.iloc[:, x_cur_ind].copy()
-        x_cur_w = x_cur.shape[1]
-        # deep copy the matrix for the shadow matrix
-        x_sha = x_cur.copy()
-        # make sure there's at least 5 columns in the shadow matrix for
-        while x_sha.shape[1] < 5:
-            x_sha = pd.concat([x_sha, x_sha], axis=1)
-        # shuffle xSha
-        x_sha = x_sha.apply(self.random_state.permutation, axis=0)
-        x_sha.columns = [f"Shadow_{i}" for i in range(x_sha.shape[1])]
-        # get importance of the merged matrix
-        if self.importance == "shap":
-            imp = _get_shap_imp(
-                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
-            )
-        elif self.importance == "fastshap":
-            imp = _get_shap_imp_fast(
-                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
-            )
-        elif self.importance == "pimp":
-            imp = _get_perm_imp(
-                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
-            )
-        else:
-            imp = _get_imp(
-                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
-            )
-
-        # separate importances of real and shadow features
-        imp_sha = imp[x_cur_w:]
-        imp_real = np.zeros(X.shape[1])
-        imp_real[:] = np.nan
-        imp_real[x_cur_ind] = imp[:x_cur_w]
-
-        return imp_real, imp_sha
-
-    @staticmethod
-    def _assign_hits(hit_reg, cur_imp, imp_sha_max):
-        """count how many times a given feature was more important than
-        the best of the shadow features
-
-        Parameters
-        ----------
-        hit_reg: array
-            count how many times a given feature was more important than the
-            best of the shadow features
-        cur_imp: array
-            current importance
-        imp_sha_max: array
-            importance of the best shadow predictor
-        Returns
-        -------
-        hit_reg : array
-            the how many times a given feature was more important than the
-            best of the shadow features
-        """
-        # register hits for features that did better than the best of shadows
-        cur_imp_no_nan = cur_imp[0]
-        cur_imp_no_nan[np.isnan(cur_imp_no_nan)] = 0
-        hits = np.where(cur_imp_no_nan > imp_sha_max)[0]
-        hit_reg[hits] += 1
-        return hit_reg
-
-    def _do_tests(self, dec_reg, hit_reg, _iter):
-        """Private method, Perform the rest if the feature should be tagget as relevant (confirmed), not relevant (rejected)
-        or undecided. The test is performed by considering the binomial tentatives over several attempts.
-        I.e. count how many times a given feature was more important than the best of the shadow features
-        and test if the associated probability to the z-score is below, between or above the rejection or
-        acceptance threshold.
-
-        Parameters
-        ----------
-        dec_reg : array
-            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
-        hit_reg : array
-            counts how many times a given feature was more important than the best of the shadow features
-        _iter : int
-            iteration number
-        Returns
-        -------
-        dec_reg : array
-            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
-
-        """
-        active_features = np.where(dec_reg >= 0)[0]
-        hits = hit_reg[active_features]
-        # get uncorrected p values based on hit_reg
-        to_accept_ps = sp.stats.binom.sf(hits - 1, _iter, 0.5).flatten()
-        to_reject_ps = sp.stats.binom.cdf(hits, _iter, 0.5).flatten()
-
-        if self.two_step:
-            # two step multicor process
-            # first we correct for testing several features in each round using FDR
-            to_accept = self._fdrcorrection(to_accept_ps, alpha=self.alpha)[0]
-            to_reject = self._fdrcorrection(to_reject_ps, alpha=self.alpha)[0]
-
-            # second we correct for testing the same feature over and over again
-            # using bonferroni
-            to_accept2 = to_accept_ps <= self.alpha / float(_iter)
-            to_reject2 = to_reject_ps <= self.alpha / float(_iter)
-
-            # combine the two multi corrections, and get indexes
-            to_accept *= to_accept2
-            to_reject *= to_reject2
-        else:
-            # as in th original Boruta, we simply do bonferroni correction
-            # with the total n_feat in each iteration
-            to_accept = to_accept_ps <= self.alpha / float(len(dec_reg))
-            to_reject = to_reject_ps <= self.alpha / float(len(dec_reg))
-
-        # find features which are 0 and have been rejected or accepted
-        to_accept = np.where((dec_reg[active_features] == 0) * to_accept)[0]
-        to_reject = np.where((dec_reg[active_features] == 0) * to_reject)[0]
-
-        # updating dec_reg
-        dec_reg[active_features[to_accept]] = 1
-        dec_reg[active_features[to_reject]] = -1
-        return dec_reg
-
-    @staticmethod
-    def _fdrcorrection(pvals, alpha=0.05):
-        """Benjamini/Hochberg p-value correction for false discovery rate, from
-        statsmodels package. Included here for decoupling dependency on statsmodels.
-
-        Parameters
-        ----------
-        pvals : array_like
-            set of p-values of the individual tests.
-        alpha : float
-            error rate
-        Returns
-        -------
-        rejected : array, bool
-            True if a hypothesis is rejected, False if not
-        pvalue-corrected : array
-            pvalues adjusted for multiple hypothesis testing to limit FDR
-        """
-        pvals = np.asarray(pvals)
-        pvals_sortind = np.argsort(pvals)
-        pvals_sorted = np.take(pvals, pvals_sortind)
-        nobs = len(pvals_sorted)
-        ecdffactor = np.arange(1, nobs + 1) / float(nobs)
-
-        reject = pvals_sorted <= ecdffactor * alpha
-        if reject.any():
-            rejectmax = max(np.nonzero(reject)[0])
-            reject[:rejectmax] = True
-
-        pvals_corrected_raw = pvals_sorted / ecdffactor
-        pvals_corrected = np.minimum.accumulate(pvals_corrected_raw[::-1])[::-1]
-        pvals_corrected[pvals_corrected > 1] = 1
-        # reorder p-values and rejection mask to original order of pvals
-        pvals_corrected_ = np.empty_like(pvals_corrected)
-        pvals_corrected_[pvals_sortind] = pvals_corrected
-        reject_ = np.empty_like(reject)
-        reject_[pvals_sortind] = reject
-        return reject_, pvals_corrected_
-
-    @staticmethod
-    def _nanrankdata(X, axis=1):
-        """Replaces bottleneck's nanrankdata with scipy and numpy alternative.
-
-        Parameters
-        ----------
-        X : array or pd.DataFrame
-            the data array
-        axis : int, optional
-            row-wise (0) or column-wise (1), by default 1
-
-        Returns
-        -------
-        ranks : array
-            the ranked array
-        """
-        ranks = sp.stats.mstats.rankdata(X, axis=axis)
-        ranks[np.isnan(X)] = np.nan
-        return ranks
-
-    def _check_params(self, X, y):
-        """Private method, Check hyperparameters as well as X and y before proceeding with fit.
-
-        Parameters
-        ----------
-        X : pd.DataFrame
-            predictor matrix
-        y : pd.series
-            target series
-
-        Raises
-        ------
-        ValueError
-            [description]
-        ValueError
-            [description]
-        """
-        # check X and y are consistent len, X is Array and y is column
-        X, y = check_X_y(X, y, dtype=None, force_all_finite=False)
-        if self.perc <= 0 or self.perc > 100:
-            raise ValueError("The percentile should be between 0 and 100.")
-
-        if self.alpha <= 0 or self.alpha > 1:
-            raise ValueError("Alpha should be between 0 and 1.")
-
-    def _print_results(self, dec_reg, _iter, flag):
-        """Private method, printing the result
-
-        Parameters
-        ----------
-        dec_reg: array
-            if the feature as been tagged as relevant (confirmed),
-            not relevant (rejected) or undecided
-        _iter: int
-            the iteration number
-        flag: int
-            is still in the feature selection process or not
-        Returns
-        -------
-         output: str
-            the output to be printed out
-        """
-        n_iter = str(_iter) + " / " + str(self.max_iter)
-        n_confirmed = np.where(dec_reg == 1)[0].shape[0]
-        n_rejected = np.where(dec_reg == -1)[0].shape[0]
-        cols = ["Iteration: ", "Confirmed: ", "Tentative: ", "Rejected: "]
-
-        # still in feature selection
-        if flag == 0:
-            n_tentative = np.where(dec_reg == 0)[0].shape[0]
-            content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
-            if self.verbose == 1:
-                output = cols[0] + n_iter
-            elif self.verbose > 1:
-                output = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
-
-        # Boruta finished running and tentatives have been filtered
-        else:
-            n_tentative = np.sum(self.support_weak_)
-            n_rejected = np.sum(~(self.support_ | self.support_weak_))
-            content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
-            result = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
-            if self.importance in ["shap", "pimp"]:
-                vimp = str(self.importance)
-            else:
-                vimp = "native"
-            output = (
-                "\n\nLeshy finished running using " + vimp + " var. imp.\n\n" + result
-            )
-        print(output)
-
-    def _update_estimator(self):
-        """
-        Update the estimator with a new random state, if applicable.
-
-        If the dataset is not categorical, the estimator's `random_state` parameter is updated
-        with a new random state generated by the `random_state` attribute of the Leshy object.
-        If the estimator is a LightGBM model, the random state value is generated between 0 and 10000.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        None
-        """
-        if self.is_cat is False:
-            if self.is_lgb:
-                self.estimator.set_params(
-                    random_state=self.random_state.randint(0, 10000)
-                )
-            else:
-                self.estimator.set_params(random_state=self.random_state)
-
-    def _update_tree_num(self, dec_reg):
-        """Update the number of trees in the estimator based on the number of selected features.
-
-        Parameters
-        ----------
-        dec_reg : array-like of shape (n_features,)
-            The decision rule for each feature, where negative values indicate that the feature should be rejected
-            and non-negative values indicate that the feature should be selected.
-
-        Returns
-        -------
-        None
-
-        Notes
-        -----
-        This function updates the `n_estimators` parameter of the estimator if it is set to "auto". The number of trees is
-        determined based on the number of selected features. Specifically, the number of trees is set to the value returned
-        by the `_get_tree_num` method, which takes as input the number of selected features that are not rejected.
-
-        If `n_estimators` is not set to "auto", this function does nothing.
-        """
-        if self.n_estimators == "auto":
-            # number of features that aren't rejected
-            not_rejected = np.where(dec_reg >= 0)[0].shape[0]
-            n_tree = self._get_tree_num(not_rejected)
-            self.estimator.set_params(n_estimators=n_tree)
-
-    def _run_iteration(
-        self, X, y, sample_weight, dec_reg, sha_max_history, imp_history, hit_reg, _iter
-    ):
-        """
-        Run an iteration of the Gradient Boosting algorithm.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            The input samples.
-
-        y : array-like of shape (n_samples,)
-            The target values.
-
-        sample_weight : array-like of shape (n_samples,), default=None
-            Sample weights. If None, then samples are equally weighted.
-
-        dec_reg : array-like of shape (n_samples,)
-            Decision function of the estimator.
-
-        sha_max_history : list of floats
-            List of the maximum shadow importance value at each iteration.
-
-        imp_history : array-like of shape (n_iterations, n_features)
-            Matrix of feature importances at each iteration.
-
-        hit_reg : array-like of shape (n_samples,)
-            Array of hit counts for each sample.
-
-        _iter : int
-            The current iteration number.
-
-        Returns
-        -------
-        dec_reg : array-like of shape (n_samples,)
-            Updated decision function of the estimator.
-
-        sha_max_history : list of floats
-            List of the maximum shadow importance value at each iteration.
-
-        imp_history : array-like of shape (n_iterations, n_features)
-            Matrix of feature importances at each iteration.
-
-        hit_reg : array-like of shape (n_samples,)
-            Array of hit counts for each sample.
-
-        imp_sha_max : float
-            The maximum shadow importance value for this iteration.
-        """
-        cur_imp = self._add_shadows_get_imps(X, y, sample_weight, dec_reg)
-        imp_sha_max = np.percentile(cur_imp[1], self.perc)
-        sha_max_history.append(imp_sha_max)
-        imp_history = np.vstack((imp_history, cur_imp[0]))
-        hit_reg = self._assign_hits(hit_reg, cur_imp, imp_sha_max)
-        dec_reg = self._do_tests(dec_reg, hit_reg, _iter)
-        return dec_reg, sha_max_history, imp_history, hit_reg, imp_sha_max
-
-    def select_features(self, X, y, sample_weight=None):
-        """
-        Select features using the Leshy algorithm.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            The input data.
-        y : array-like of shape (n_samples,)
-            The target values.
-        sample_weight : array-like of shape (n_samples,), default=None
-            Individual weights for each sample.
-
-        Returns
-        -------
-        dec_reg : ndarray of shape (n_features,)
-            The decision rule. 1 means the feature is selected, 0 means the feature is not selected.
-        sha_max_history : list
-            List of the maximum shadow importances per iteration.
-        imp_history : ndarray of shape (n_iterations, n_features)
-            Array containing the feature importances per iteration.
-        imp_sha_max : float
-            Maximum shadow importance value.
-        """
-        pbar = tqdm(total=self.max_iter, desc="Leshy iteration")
-        dec_reg = np.zeros(X.shape[1])
-        hit_reg = np.zeros(X.shape[1])
-        sha_max_history = []
-        imp_history = np.empty((0, X.shape[1]))
-
-        for _iter in range(1, self.max_iter):
-            if not np.any(dec_reg == 0):
-                break
-            self._update_tree_num(dec_reg)
-            self._update_estimator()
-            (
-                dec_reg,
-                sha_max_history,
-                imp_history,
-                hit_reg,
-                imp_sha_max,
-            ) = self._run_iteration(
-                X,
-                y,
-                sample_weight,
-                dec_reg,
-                sha_max_history,
-                imp_history,
-                hit_reg,
-                _iter,
-            )
-            _iter += 1
-            pbar.update(1)
-
-        pbar.close()
-        return dec_reg, sha_max_history, imp_history, imp_sha_max
-
-    def _calculate_support(self, confirmed, tentative, n_feat):
-        """
-        Calculate the feature support arrays.
-
-        Parameters
-        ----------
-        confirmed : array-like of shape (n_confirmed,)
-            Indices of confirmed features.
-        tentative : array-like of shape (n_tentative,)
-            Indices of tentative features.
-        n_feat : int
-            Total number of features.
-
-        Returns
-        -------
-        None
-            The function populates the following class attributes:
-            - n_features_ : int
-                Number of selected features.
-            - support_ : ndarray of shape (n_feat,)
-                Boolean array indicating the selected features.
-            - support_weak_ : ndarray of shape (n_feat,)
-                Boolean array indicating the tentatively selected features.
-        """
-        # basic result variables
-        self.n_features_ = confirmed.shape[0]
-        self.support_ = np.zeros(n_feat, dtype=bool)
-        self.support_weak_ = np.zeros(n_feat, dtype=bool)
-        self.support_[confirmed] = 1
-        self.support_weak_ = np.zeros(n_feat, dtype=bool)
-        self.support_weak_[tentative] = 1
-        if self.keep_weak:
-            self.support_[tentative] = 1
-
-    def _calculate_absolute_ranking(self):
-        """
-        Compute feature importance scores using SHAP values.
-
-        Parameters
-        ----------
-        new_x_tr : numpy.ndarray
-            The training dataset after being processed.
-        shap_matrix : numpy.ndarray
-            The matrix containing SHAP values computed by a LightGBM model.
-        param : dict
-            A dictionary containing the parameters for a LightGBM model.
-        objective : str
-            The objective function of the LightGBM model.
-
-        Returns
-        -------
-        list
-            A list of tuples containing feature names and their corresponding importance scores.
-        """
-        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
-        self.ranking_absolutes_ = list(
-            vimp_df.mean().sort_values(ascending=False).index
-        )
-
-    def _calculate_relative_ranking(self, n_feat, tentative, confirmed, imp_history):
-        """
-        Calculates the relative ranking of features based on their importance history.
-
-        Parameters
-        ----------
-        n_feat : int
-            The total number of features.
-        tentative : ndarray of shape (n_tentative_features,)
-            An array containing the indices of tentative features.
-        confirmed : ndarray of shape (n_confirmed_features,)
-            An array containing the indices of confirmed features.
-        imp_history : ndarray of shape (n_iterations + 1, n_features)
-            An array containing the feature importances for each iteration.
-
-        Returns
-        -------
-        None
-
-        """
-        # ranking, confirmed variables are rank 1
-        self.ranking_ = np.ones(n_feat, dtype=int)
-        # tentative variables are rank 2
-        self.ranking_[tentative] = 2
-        selected = np.hstack((confirmed, tentative))
-        # all rejected features are sorted by importance history
-        not_selected = np.setdiff1d(np.arange(n_feat), selected)
-        # large importance values should rank higher = lower ranks -> *(-1)
-        imp_history_rejected = imp_history[1:, not_selected] * -1
-
-        # update rank for not_selected features
-        if not_selected.shape[0] > 0:
-            # calculate ranks in each iteration, then median of ranks across feats
-            iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
-            rank_medians = np.nanmedian(iter_ranks, axis=0)
-            ranks = self._nanrankdata(rank_medians, axis=0)
-
-            # set smallest rank to 3 if there are tentative feats
-            if tentative.shape[0] > 0:
-                ranks = ranks - np.min(ranks) + 3
-            else:
-                # and 2 otherwise
-                ranks = ranks - np.min(ranks) + 2
-            self.ranking_[not_selected] = ranks
-        else:
-            # all are selected, thus we set feature supports to True
-            self.support_ = np.ones(n_feat, dtype=bool)
-
-    def _print_result(self, dec_reg, _iter, start_time):
-        """
-        Print the results of feature selection.
-
-        Parameters
-        ----------
-        dec_reg : bool
-            Decision on whether to proceed with another round of feature selection.
-        _iter : int
-            Current iteration number.
-        start_time : float
-            Time when the feature selection process started.
-
-        Returns
-        -------
-        None
-            The function prints the relevant results and running time.
-        """
-        if self.verbose > 0:
-            self._print_results(dec_reg, _iter, 1)
-        self.running_time = time.time() - start_time
-        hours, rem = divmod(self.running_time, 3600)
-        minutes, seconds = divmod(rem, 60)
-        print(
-            "All relevant predictors selected in {:0>2}:{:0>2}:{:05.2f}".format(
-                int(hours), int(minutes), seconds
-            )
-        )
-
-
-def _get_confirmed_and_tentative(dec_reg):
-    """Extracts the confirmed and tentative features from dec_reg."""
-    confirmed = np.where(dec_reg == 1)[0]
-    tentative = np.where(dec_reg == 0)[0]
-    return confirmed, tentative
-
-
-def _select_tentative(tentative, imp_history, sha_max_history):
-    """
-    Select tentative features based on median importance values.
-
-    Parameters
-    ----------
-    tentative: array-like of shape (n_tentative,)
-        Array of indices representing tentative features.
-    imp_history: array-like of shape (n_iterations + 1, n_features)
-        Importance values for each feature in each iteration.
-    sha_max_history: array-like of shape (n_iterations + 1,)
-        The history of the highest stability scores.
-
-    Returns
-    -------
-    tentative: array-like of shape (n_tentative_confirmed,)
-        The confirmed tentative features based on their median importance values.
-    """
-    # ignore the first row of zeros
-    tentative_median = np.median(imp_history[1:, tentative], axis=0)
-    # which tentative to keep
-    tentative_confirmed = np.where(tentative_median > np.median(sha_max_history))[0]
-    tentative = tentative[tentative_confirmed]
-    return tentative
-
-
-def _split_fit_estimator(estimator, X, y, sample_weight=None, cat_feature=None):
-    """Private function, split the train, test and fit the model
-
-    Parameters
-    ----------
-    estimator : estimator object implementing 'fit' and 'predict'
-        The object to use to fit the data.
-    X : pd.DataFrame of shape [n_samples, n_features]
-        predictor matrix
-    y : pd.series of shape [n_samples]
-        target
-    sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample
-    cat_feature : list of int or None
-        the list of integers, cols loc, of the categrocial predictors. Avoids to detect and encode
-        each iteration if the exact same columns are passed to the selection methods.
-    Returns
-    -------
-     model :
-        fitted model
-     X_tt : array [n_samples, n_features]
-        the test split, predictors
-     y_tt : array [n_samples]
-        the test split, target
-    """
-    if cat_feature is None:
-        # detect, store and encode categorical predictors
-        X, _, cat_idx = get_pandas_cat_codes(X)
-    else:
-        cat_idx = cat_feature
-
-    if sample_weight is not None:
-        w = sample_weight
-        if is_regressor(estimator):
-            X_tr, X_tt, y_tr, y_tt, w_tr, w_tt = train_test_split(
-                X, y, w, random_state=42
-            )
-        else:
-            X_tr, X_tt, y_tr, y_tt, w_tr, w_tt = train_test_split(
-                X, y, w, stratify=y, random_state=42
-            )
-    else:
-        if is_regressor(estimator):
-            X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, random_state=42)
-        else:
-            X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, stratify=y, random_state=42)
-        w_tr, w_tt = None, None
-
-    if check_if_tree_based(estimator):
-        try:
-            # handle cat features if supported by the fit method
-            if is_catboost(estimator) or (
-                "cat_feature" in estimator.fit.__code__.co_varnames
-            ):
-                model = estimator.fit(
-                    X_tr, y_tr, sample_weight=w_tr, cat_features=cat_idx
-                )
-            else:
-                model = estimator.fit(X_tr, y_tr, sample_weight=w_tr)
-
-        except Exception as e:
-            raise ValueError(
-                "Please check your X and y variable. The provided "
-                "estimator cannot be fitted to your data.\n" + str(e)
-            )
-    else:
-        raise ValueError("Not a tree based model")
-
-    return model, X_tt, y_tt, w_tt
-
-
-def _get_shap_imp(estimator, X, y, sample_weight=None, cat_feature=None):
-    """Get the SHAP feature importance
-
-    Parameters
-    ----------
-    estimator : estimator object
-        An estimator object implementing `fit` and `predict` methods.
-    X : pd.DataFrame of shape [n_samples, n_features]
-        Predictor matrix.
-    y : pd.Series of shape [n_samples]
-        Target variable.
-    sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample.
-    cat_feature : list of int or None, default=None
-        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
-        each iteration if the exact same columns are passed to the selection methods.
-
-    Returns
-    -------
-    shap_imp : array
-        The SHAP importance array.
-    """
-    # Clone the estimator to avoid modifying the original one
-    estimator = clone(estimator)
-
-    # Split the data into train and test sets and fit the model
-    model, X_tt, y_tt, w_tt = _split_fit_estimator(
-        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
-    )
-    # Compute the SHAP values
-    if is_lightgbm(estimator):
-        # For LightGBM models use the built-in SHAP method
-        shap_matrix = model.predict(X_tt, pred_contrib=True)
-
-        # The shape of the shap_matrix depends on whether the estimator is a classifier or a regressor
-        if is_classifier(estimator) and (len(np.unique(y_tt)) > 2):
-            # For multi-class classifiers, reshape the shap_matrix
-            n_features = X_tt.shape[1]
-            shap_matrix = np.delete(
-                shap_matrix,
-                list(range(n_features, shap_matrix.shape[1], n_features + 1)),
-                axis=1,
-            )
-            shap_imp = np.mean(np.abs(shap_matrix), axis=0)
-        else:
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
-    else:
-        # For other tree-based models, use the shap.TreeExplainer method to compute SHAP values
-        explainer = shap.TreeExplainer(
-            model, feature_perturbation="tree_path_dependent"
-        )
-        shap_values = explainer.shap_values(X_tt)
-        # For multi-class classifiers, reshape the shap_values
-        if is_classifier(estimator):
-            if isinstance(shap_values, list):
-                # For LightGBM classifier in sklearn API, SHAP returns a list of arrays
-                # https://github.com/slundberg/shap/issues/526
-                shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_values], axis=0)
-            else:
-                shap_imp = np.abs(shap_values).mean(0)
-        else:
-            shap_imp = np.abs(shap_values).mean(0)
-    return shap_imp
-
-
-def _get_shap_imp_fast(estimator, X, y, sample_weight=None, cat_feature=None):
-    """Get the SHAP feature importance using the fasttreeshap implementation
-
-    Parameters
-    ----------
-    estimator : estimator object
-        An estimator object implementing `fit` and `predict` methods.
-    X : pd.DataFrame of shape [n_samples, n_features]
-        Predictor matrix.
-    y : pd.Series of shape [n_samples]
-        Target variable.
-    sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample.
-    cat_feature : list of int or None, default=None
-        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
-        each iteration if the exact same columns are passed to the selection methods.
-
-    Returns
-    -------
-    shap_imp : array
-        The SHAP importance array.
-    """
-    try:
-        from fasttreeshap import TreeExplainer as FastTreeExplainer
-    except ImportError:
-        ImportError("fasttreeshap is not installed")
-    
-    # Clone the estimator to avoid modifying the original one
-    estimator = clone(estimator)
-
-    # Split the data into train and test sets and fit the model
-    model, X_tt, y_tt, w_tt = _split_fit_estimator(
-        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
-    )
-    explainer = FastTreeExplainer(
-        model,
-        algorithm="auto",
-        shortcut=False,
-        feature_perturbation="tree_path_dependent",
-    )
-    shap_matrix = explainer.shap_values(X_tt)
-    # multiclass returns a list
-    # for binary and for some models, shap is still returning a list
-    if is_classifier(estimator):
-        if isinstance(shap_matrix, list):
-            # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
-            # https://github.com/slundberg/shap/issues/526
-            shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_matrix], axis=0)
-        else:
-            shap_imp = np.abs(shap_matrix).mean(0)
-    else:
-        shap_imp = np.abs(shap_matrix).mean(0)
-    return shap_imp
-
-
-def _get_perm_imp(estimator, X, y, sample_weight, cat_feature=None):
-    """Private function, Get the SHAP feature importance
-
-    Parameters
-    ----------
-    estimator: sklearn estimator
-    X : pd.DataFrame of shape [n_samples, n_features]
-        predictor matrix
-    y : pd.series of shape [n_samples]
-        target
-    sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample
-    cat_feature : list of int or None
-        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
-        each iteration if the exact same columns are passed to the selection methods.
-    Returns
-    -------
-    imp : array
-        the permutation importance array
-    """
-    # be sure to use an non-fitted estimator
-    estimator = clone(estimator)
-
-    model, X_tt, y_tt, w_tt = _split_fit_estimator(
-        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
-    )
-    perm_imp = permutation_importance(
-        model, X_tt, y_tt, n_repeats=5, random_state=42, n_jobs=-1
-    )
-    imp = perm_imp.importances_mean.ravel()
-    return imp
-
-
-def _get_imp(estimator, X, y, sample_weight=None, cat_feature=None):
-    """Private function, Get the native feature importance (impurity based for instance)
-
-    Notes
-    -----
-    This is know to return biased and uninformative results.
-    e.g.
-    https://scikit-learn.org/stable/auto_examples/inspection/
-    plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py
-
-    or
-
-    https://explained.ai/rf-importance/
-
-    Parameters
-    ----------
-    X : array-like, shape = [n_samples, n_features]
-        The training input samples.
-    y : array-like, shape = [n_samples]
-        The target values.
-    sample_weight : array-like, shape = [n_samples], default=None
-        Individual weights for each sample
-    cat_feature: list of int or None
-        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
-        each iteration if the exact same columns are passed to the selection methods.
-    Returns
-    -------
-    imp : array
-        the permutation importance array
-    """
-    # be sure to use an non-fitted estimator
-    estimator = clone(estimator)
-
-    try:
-        if cat_feature is None:
-            X, _, cat_idx = get_pandas_cat_codes(X)
-        else:
-            cat_idx = cat_feature
-
-        # handle catboost and cat features
-        if is_catboost(estimator) or (
-            "cat_feature" in estimator.fit.__code__.co_varnames
-        ):
-            X = pd.DataFrame(X)
-            estimator.fit(X, y, sample_weight=sample_weight, cat_features=cat_idx)
-        else:
-            estimator.fit(X, y, sample_weight=sample_weight)
-
-    except Exception as e:
-        raise ValueError(
-            "Please check your X and y variable. The provided "
-            "estimator cannot be fitted to your data.\n" + str(e)
-        )
-    try:
-        imp = estimator.feature_importances_
-    except Exception:
-        raise ValueError(
-            "Only methods with feature_importance_ attribute "
-            "are currently supported in BorutaPy."
-        )
-    return imp
-
-
-###################################
-#
-# BoostAGroota
-#
-###################################
-class BoostAGroota(SelectorMixin, BaseEstimator):  # (object):
-    """
-    BoostAGroota is an all-relevant feature selection method, while most others are minimal optimal.
-    It tries to find all features carrying information usable for prediction, rather than finding a possibly compact
-    subset of features on which some estimator has a minimal error.
-
-    Why bother with all-relevant feature selection?
-    When you try to understand the phenomenon that made your data, you should
-    care about all factors that contribute to it, not just the bluntest signs
-    of it in the context of your methodology (minimal optimal set of features
-    by definition depends on your estimator choice).
-
-    Parameters
-    ----------
-    estimator : scikit-learn estimator
-        The model to train, lightGBM recommended, see the reduce lightgbm method.
-    cutoff : float
-        The value by which the max of shadow imp is divided, to compare to real importance.
-    iters : int (>0)
-        The number of iterations to average for the feature importance (on the same split),
-        to reduce the variance.
-    max_rounds : int (>0)
-        The number of times the core BoostAGroota algorithm will run.
-        Each round eliminates more and more features.
-    delta : float (0 < delta <= 1)
-        Stopping criteria for whether another round is started.
-    silent : bool
-        Set to True if you don't want to see the BoostAGroota output printed.
-    importance : str, default='shap'
-        The kind of feature importance to use. Possible values: 'shap' (Shapley values),
-        'pimp' (permutation importance), and 'native' (Gini/impurity).
-
-    Attributes
-    ----------
-    selected_features_ : list of str
-        The list of columns to keep.
-    ranking_ : array of shape [n_features]
-        The feature ranking, such that ``ranking_[i]`` corresponds to the
-        ranking position of the i-th feature. Selected (i.e., estimated
-        best) features are assigned rank 1, and tentative features are assigned
-        rank 2.
-    ranking_absolutes_ : array of shape [n_features]
-        The absolute feature ranking as ordered by the selection process. It does not guarantee
-        that this order is correct for all models. For a model-agnostic ranking, see the
-        attribute ``ranking``.
-    sha_cutoff_df : dataframe
-        Feature importance of the real+shadow predictors over iterations.
-    mean_shadow : float
-        The threshold below which the predictors are rejected.
-
-    Examples
-    --------
-    >>> X = df[filtered_features].copy()
-    >>> y = df['target'].copy()
-    >>> w = df['weight'].copy()
-    >>> model = LGBMRegressor(n_jobs=-1, n_estimators=100, objective='rmse', random_state=42, verbose=0)
-    >>> feat_selector = BoostAGroota(estimator=model, cutoff=1, iters=10, max_rounds=10, delta=0.1, importance='shap')
-    >>> feat_selector.fit(X, y, sample_weight=None)
-    >>> print(feat_selector.selected_features_)
-    >>> feat_selector.plot_importance(n_feat_per_inch=5)
-    """
-
-    def __init__(
-        self,
-        estimator=None,
-        cutoff=4,
-        iters=10,
-        max_rounds=500,
-        delta=0.1,
-        silent=True,
-        importance="shap",
-    ):
-        self.estimator = estimator
-        self.cutoff = cutoff
-        self.iters = iters
-        self.max_rounds = max_rounds
-        self.delta = delta
-        self.silent = silent
-        self.importance = importance
-        self.sha_cutoff_df = None
-        self.mean_shadow = None
-        self.ranking_absolutes_ = None
-        self.ranking_ = None
-
-        # Throw errors if the inputted parameters don't meet the necessary criteria
-        if cutoff <= 0:
-            raise ValueError(
-                "cutoff should be greater than 0. You entered" + str(cutoff)
-            )
-        if iters <= 0:
-            raise ValueError("iters should be greater than 0. You entered" + str(iters))
-        if (delta <= 0) | (delta > 1):
-            raise ValueError("delta should be between 0 and 1, was " + str(delta))
-
-        # Issue warnings for parameters to still let it run
-        if delta < 0.02:
-            warnings.warn(
-                "WARNING: Setting a delta below 0.02 may not converge on a solution."
-            )
-        if max_rounds < 1:
-            warnings.warn(
-                "WARNING: Setting max_rounds below 1 will automatically be set to 1."
-            )
-
-        if importance == "native":
-            warnings.warn(
-                "[BoostAGroota]: using native variable importance might break the FS"
-            )
-
-    def __repr__(self):
-        s = (
-            "BoostARoota(est={est}, \n"
-            "                cutoff={cutoff},\n"
-            "                iters={iters},\n"
-            "                max_rounds={mr},\n"
-            "                delta={delta},\n"
-            "                silent={silent}, \n"
-            '                importance="{importance}")'.format(
-                estimator=self.estimator,
-                cutoff=self.cutoff,
-                iters=self.iters,
-                mr=self.max_rounds,
-                delta=self.delta,
-                silent=self.silent,
-                importance=self.importance,
-            )
-        )
-        return s
-
-    def fit(self, X, y, sample_weight=None):
-        """Fit the BoostAGroota transformer with the provided estimator.
-        Parameters
-        ----------
-        X : pd.DataFrame
-            the predictors matrix
-        y : pd.Series
-            the target
-        sample_weight : pd.series
-            sample_weight, if any
-        """
-        try:
-            from fasttreeshap import TreeExplainer as FastTreeExplainer
-        except ImportError:
-            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
-            self.importance = "shap"
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a dataframe")
-
-        if sample_weight is not None:
-            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
-
-        # crit, keep_vars, df_vimp, mean_shadow
-        _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _boostaroota(
-            X,
-            y,
-            # metric=self.metric,
-            estimator=self.estimator,
-            cutoff=self.cutoff,
-            iters=self.iters,
-            max_rounds=self.max_rounds,
-            delta=self.delta,
-            silent=self.silent,
-            weight=sample_weight,
-            imp=self.importance,
-        )
-        self.selected_features_ = self.selected_features_.values
-        self.support_ = np.asarray(
-            [c in self.selected_features_ for c in self.feature_names_in_]
-        )
-        self.ranking_absolutes_ = list(
-            self.sha_cutoff_df.iloc[:, : int(self.sha_cutoff_df.shape[1] / 2)]
-            .mean()
-            .sort_values(ascending=False)
-            .index
-        )
-        self.ranking_ = np.where(self.support_, 2, 1)
-        return self
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def transform(self, X):
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    def _more_tags(self):
-        return {"allow_nan": True, "requires_y": True}
-
-    @mpl.rc_context(PLT_PARAMS)
-    def plot_importance(self, n_feat_per_inch=5):
-        """
-        Boxplot of the variable importance, ordered by magnitude.
-        The max shadow variable importance illustrated by the dashed line.
-        Requires to apply the fit method first.
-
-        Parameters
-        ----------
-        n_feat_per_inch : int, default=5
-            Number of features to plot per inch (for scaling the figure).
-
-        Returns
-        -------
-        fig : plt.figure or None
-            The matplotlib figure object containing the boxplot, or None if there are no selected features.
-        """
-        if self.mean_shadow is None:
-            raise ValueError("Apply fit method first")
-
-        b_df = self.sha_cutoff_df
-        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
-
-        real_df = real_df.reindex(
-            real_df.mean().sort_values(ascending=True).index, axis=1
-        )
-
-        if real_df.dropna().empty:
-            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
-            return None
-
-        fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
-        bp = real_df.plot(**PLOT_KWARGS, ax=ax)
-        bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
-
-        for c in range(len(self.selected_features_)):
-            patch = bp.findobj(mpl.patches.Patch)[real_df.shape[1] - c - 1]
-            patch.set_facecolor(BLUE)
-            patch.set_color(BLUE)
-
-        custom_lines = [
-            Line2D([0], [0], color=BLUE, lw=5),
-            Line2D([0], [0], color="gray", lw=5),
-            Line2D([0], [0], linestyle="--", color=RED, lw=2),
-        ]
-        bp.legend(
-            custom_lines, ["confirmed", "rejected", "sha. max"], loc="lower right"
-        )
-
-        ax.axvline(x=self.mean_shadow, linestyle="--", color=RED)
-        ax.set_title("BoostAGroota importance of selected predictors")
-
-        return fig
-
-
-############################################
-# Helper Functions to do the Heavy Lifting
-############################################
-
-
-def _create_shadow(X_train):
-    """Create shadow features by making copies of all X variables and randomly shuffling them.
-
-    Parameters
-    ----------
-    X_train : pd.DataFrame
-        The dataframe to create shadow features on.
-
-    Returns
-    -------
-    pd.DataFrame
-        A dataframe that is twice the width of X_train and contains the shadow features, along with a list of the shadow feature names.
-    """
-    X_shadow = X_train.copy()
-    for c in X_shadow.columns:
-        np.random.shuffle(X_shadow[c].values)
-    # Rename the shadow variables
-    shadow_names = [f"ShadowVar{i+1}" for i in range(X_train.shape[1])]
-    X_shadow.columns = shadow_names
-    # Combine to make one new dataframe
-    new_x = pd.concat([X_train, X_shadow], axis=1)
-    return new_x, shadow_names
-
-
-########################################################################################
-# BoostARoota. In principle, you cannot/don't need to access those methods (reason of
-# the _ in front of the function name, they're internal functions)
-########################################################################################
-
-
-def _reduce_vars_sklearn(
-    X,
-    y,
-    estimator,
-    this_round,
-    cutoff,
-    n_iterations,
-    delta,
-    silent,
-    weight,
-    imp_kind,
-    cat_feature,
-):
-    """
-    Private function, reduce the number of predictors using a sklearn estimator
-
-    Parameters
-    ----------
-    x : pd.DataFrame
-        the dataframe to create shadow features on
-    y : pd.Series
-        the target
-    estimator : sklearn estimator
-        the model to train, lightGBM recommended
-    this_round : int
-        The number of times the core BoostARoota algorithm will run.
-        Each round eliminates more and more features
-    cutoff : float
-        the value by which the max of shadow imp is divided, to compare to real importance
-    n_iterations : int
-        The number of iterations to average for the feature importance (on the same split),
-        to reduce the variance
-    delta : float (0 < delta <= 1)
-        Stopping criteria for whether another round is started
-    silent : bool
-        Set to True if don't want to see the BoostARoota output printed.
-        Will still show any errors or warnings that may occur
-    weight : pd.series
-        sample_weight, if any
-    imp_kind : str
-        whether if native, shap, fastshap or permutation importance should be used
-    cat_feature : list of int or None
-        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
-        each iteration if the exact same columns are passed to the selection methods.
-
-    Returns
-    -------
-    criteria : bool
-        if the criteria has been reached or not
-    real_vars['feature'] : pd.dataframe
-        feature importance of the real predictors over iter
-    df : pd.DataFrame
-        feature importance of the real+shadow predictors over iter
-    mean_shadow : float
-        the feature importance threshold, to reject or not the predictors
-
-    Raises
-    ------
-    ValueError
-        error if the feature importance type is not
-    """
-    # Set up the parameters for running the model in XGBoost - split is on multi log loss
-    for i in range(1, n_iterations + 1):
-        # Create the shadow variables and run the model to obtain importances
-        new_x, shadow_names = _create_shadow(X)
-        imp_func = {
-            "shap": _get_shap_imp,
-            "fastshap": _get_shap_imp,
-            "pimp": _get_perm_imp,
-            "native": _get_imp,
-        }
-        importance = imp_func[imp_kind](
-            estimator, new_x, y, sample_weight=weight, cat_feature=cat_feature
-        )
-
-        # Create a dataframe to store the feature importances
-        if i == 1:
-            df = pd.DataFrame({"feature": new_x.columns})
-            df2 = df.copy()
-
-        # Store the feature importances in df2
-        try:
-            # Normalize the feature importances
-            df2["fscore" + str(i)] = importance / importance.sum()
-        except ValueError:
-            print("Only Sklearn tree based methods allowed")
-
-        # Merge the current feature importances with the existing ones in df
-        df = pd.merge(
-            df, df2, on="feature", how="outer", suffixes=("_x" + str(i), "_y" + str(i))
-        )
-
-        # Print the iteration number if not silent
-        if not silent:
-            print("Round: ", this_round, " iteration: ", i)
-
-    df["Mean"] = df.select_dtypes(include=[np.number]).mean(axis=1, skipna=True)
-    # Split them back out
-    real_vars = df.loc[~df["feature"].isin(shadow_names)]
-    shadow_vars = df.loc[df["feature"].isin(shadow_names)]
-
-    # Get mean value from the shadows (max, like in Boruta, median to mitigate variance)
-    mean_shadow = (
-        shadow_vars.select_dtypes(include=[np.number])
-        .max(skipna=True)
-        .mean(skipna=True)
-        / cutoff
-    )
-    real_vars = real_vars[(real_vars.Mean >= mean_shadow)]
-
-    # Check for the stopping criteria
-    # Compute the fraction of features selected in this round
-    selected_frac = len(real_vars) / len(X.columns)
-
-    # Check if we should stop feature selection
-    # make sure we are removing at least delta % of the variables
-    criteria = len(X.columns) == 0 or selected_frac == 0 or selected_frac > 1 - delta
-
-    return criteria, real_vars["feature"], df, mean_shadow
-
-
-def _boostaroota(
-    X, y, estimator, cutoff, iters, max_rounds, delta, silent, weight, imp
-):
-    """
-    Private function, reduces the number of predictors using a sklearn estimator.
-
-    Parameters
-    ----------
-    x : pd.DataFrame
-        The dataframe to create shadow features on.
-    y : pd.Series
-        The target.
-    estimator : scikit-learn estimator
-        The model to train, lightGBM recommended, see the reduce lightgbm method.
-    cutoff : float
-        The value by which the max of shadow imp is divided, to compare to real importance.
-    iters : int (>0)
-        The number of iterations to average for the feature importances (on the same split),
-        to reduce the variance.
-    max_rounds : int (>0)
-        The number of times the core BoostARoota algorithm will run.
-        Each round eliminates more and more features.
-    delta : float (0 < delta <= 1)
-        Stopping criteria for whether another round is started.
-    silent : bool
-        Set to True if you don't want to see the BoostARoota output printed.
-        Will still show any errors or warnings that may occur.
-    weight : pd.Series, optional
-        Sample weights, if any.
-
-    Returns
-    -------
-    crit : bool
-        If the criteria have been reached or not.
-    keep_vars : pd.DataFrame
-        Feature importance of the real predictors over iterations.
-    df_vimp : pd.DataFrame
-        Feature importance of the real+shadow predictors over iterations.
-    mean_shadow : float
-        The feature importance threshold to reject or not the predictors.
-    """
-    start_time = time.time()
-    new_x = X.copy()
-
-    # extract the categorical names for the first time, store it for next iterations
-    # In the below while loop this list will be update only once some of the predictors
-    # are removed. This way the encoding is done only every predictors update and not
-    # every iteration. The code will then be much faster since the encoding is done only once.
-    new_x, obj_feat, cat_idx = get_pandas_cat_codes(X)
-
-    # Run through loop until "crit" changes
-    i = 0
-    imp_dic = {}
-    with tqdm(total=max_rounds, desc="BoostaGRoota round") as pbar:
-        while True:
-            # Inside this loop we reduce the dataset on each iteration exiting with keep_vars
-            i += 1
-            crit, keep_vars, df_vimp, mean_shadow = _reduce_vars_sklearn(
-                new_x,
-                y,
-                estimator=estimator,
-                this_round=i,
-                cutoff=cutoff,
-                n_iterations=iters,
-                delta=delta,
-                silent=silent,
-                weight=weight,
-                imp_kind=imp,
-                cat_feature=cat_idx,
-            )
-
-            b_df = df_vimp.T.iloc[1:-1].astype(float)
-            b_df.columns = df_vimp.T.iloc[0].values
-            imp_dic.update(b_df.to_dict())
-
-            if crit or i >= max_rounds or len(keep_vars) == 0:
-                break
-            else:
-                new_x = new_x[keep_vars].copy()
-                _, _, cat_idx = get_pandas_cat_codes(new_x)
-
-                pbar.update(1)
-
-    elapsed = (time.time() - start_time) / 60
-    if not silent:
-        print(f"BoostARoota ran successfully! Algorithm went through {i} rounds.")
-        print(f"The feature selection BoostARoota running time is {elapsed:8.2f} min")
-
-    df_vimp = pd.DataFrame.from_dict(imp_dic)
-
-    return crit, keep_vars, df_vimp, mean_shadow
-
-
-###################################
-#
-# GrootCV
-#
-###################################
-
-
-class GrootCV(SelectorMixin, BaseEstimator):
-    """
-    GrootCV is a feature selection method based on cross-validation with lightGBM.
-
-    A shuffled copy of the predictors matrix is added (shadows) to the original set of predictors.
-    The lightGBM is fitted using repeated cross-validation, the feature importance
-    is extracted each time and averaged to smooth out the noise.
-    If the feature importance is larger than the average shadow feature importance then the predictors are rejected, the others are kept.
-        - Cross-validated feature importance to smooth out the noise, based on lightGBM only
-          (which is, most of the time, the fastest and more accurate Boosting).
-        - the feature importance is derived using SHAP importance
-        - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
-          it improves the convergence (needs less evaluation to find a threshold)
-        - Not based on a given percentage of cols needed to be deleted
-        - Plot method for var. imp
-
-    Parameters
-    ----------
-    objective : str or callable, default=None
-        The objective function to use in lightGBM. If None, it uses the objective specified in `lgbm_params`.
-    cutoff : float, default=1
-        The value by which the max of shadow imp is divided, to compare to real importance.
-    n_folds : int, default=5
-        The number of folds for cross-validation.
-    n_iter : int, default=5
-        The number of iterations to average for the feature importance (on the same split), to reduce variance.
-    silent : bool, default=True
-        Set to True if you don't want to see the GrootCV output printed.
-    rf : bool, default=False
-        If True, use random forest for calculating feature importances; otherwise, use lightGBM.
-    fastshap : bool, default=False
-        If True, use fastSHAP for calculating feature importances; otherwise, use SHAP.
-    n_jobs : int, default=0
-        The number of jobs to run in parallel. If 0, no parallelism is used.
-    lgbm_params : dict, default=None
-        The parameters for the lightGBM model.
-
-    Attributes
-    ----------
-    selected_features_ : ndarray
-        The list of columns to keep as selected features.
-    cv_df : pd.DataFrame
-        DataFrame containing feature importance values for each fold and iteration.
-    sha_cutoff : float
-        The threshold below which the predictors are rejected.
-    ranking_absolutes_ : list
-        The absolute feature ranking as ordered by the selection process.
-    ranking_ : ndarray
-        The feature ranking, where 2 corresponds to selected features and 1 to tentative features.
-
-    Methods
-    -------
-    fit(X, y, sample_weight=None)
-        Fit the GrootCV on the input data.
-    transform(X)
-        Apply the fitted GrootCV on new data.
-    plot_importance(n_feat_per_inch=5)
-        Plot the feature importance of the fitted GrootCV.
-
-    Warnings
-    --------
-    If `sha_cutoff` is None, you should apply the fit method first.
-    Examples
-    -------
-    >>> X = df[filtered_features].copy()
-    >>> y = df['target'].copy()
-    >>> w = df['weight'].copy()
-    >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
-    >>> feat_selector.fit(X, y, sample_weight=None)
-    >>> feat_selector.plot_importance(n_feat_per_inch=5)
-    """
-
-    def __init__(
-        self,
-        objective=None,
-        cutoff=1,
-        n_folds=5,
-        n_iter=5,
-        silent=True,
-        rf=False,
-        fastshap=False,
-        n_jobs=0,
-        lgbm_params=None,
-    ):
-        self.objective = objective
-        self.cutoff = cutoff
-        self.n_folds = n_folds
-        self.n_iter = n_iter
-        self.silent = silent
-        self.rf = rf
-        self.fastshap = fastshap
-        self.cv_df = None
-        self.sha_cutoff = None
-        self.ranking_absolutes_ = None
-        self.ranking_ = None
-        self.lgbm_params = lgbm_params
-        self.n_jobs = n_jobs
-
-        # Throw errors if the inputted parameters don't meet the necessary criteria
-        # Ensure parameters meet necessary criteria
-        if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
-            raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
-
-    def fit(self, X, y, sample_weight=None):
-        """
-        Fit the GrootCV on the input data.
-
-        Parameters
-        ----------
-        X : pd.DataFrame of shape (n_samples, n_features)
-            The predictor dataframe.
-        y : array-like of shape (n_samples,)
-            The target vector.
-        sample_weight : array-like of shape (n_samples,), optional
-            The weight vector, by default None.
-
-        Returns
-        -------
-        self : object
-            Returns self.
-        """
-
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a pandas DataFrame")
-
-        self.feature_names_in_ = X.columns.to_numpy()
-        y = pd.Series(y) if not isinstance(y, pd.Series) else y
-
-        if sample_weight is not None:
-            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
-
-        # internal encoding (ordinal encoding)
-        X, obj_feat, cat_idx = get_pandas_cat_codes(X)
-
-        self.selected_features_, self.cv_df, self.sha_cutoff = _reduce_vars_lgb_cv(
-            X,
-            y,
-            objective=self.objective,
-            cutoff=self.cutoff,
-            n_folds=self.n_folds,
-            n_iter=self.n_iter,
-            silent=self.silent,
-            weight=sample_weight,
-            rf=self.rf,
-            fastshap=self.fastshap,
-            lgbm_params=self.lgbm_params,
-            n_jobs=self.n_jobs,
-        )
-
-        self.selected_features_ = self.selected_features_.values
-        self.support_ = np.asarray(
-            [c in self.selected_features_ for c in self.feature_names_in_]
-        )
-        self.ranking_ = np.where(self.support_, 2, 1)
-
-        b_df = self.cv_df.T.copy()
-        b_df.columns = b_df.iloc[0]
-        b_df = b_df.drop(b_df.index[0])
-        b_df = b_df.drop(b_df.index[-1])
-        b_df = b_df.convert_dtypes()
-        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
-        self.ranking_absolutes_ = list(
-            real_df.mean().sort_values(ascending=False).index
-        )
-        return self
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def transform(self, X):
-        """
-        Apply the fitted GrootCV on new data.
-
-        Parameters
-        ----------
-        X : pd.DataFrame of shape (n_samples, n_features)
-            The predictor dataframe.
-
-        Returns
-        -------
-        X_selected : pd.DataFrame of shape (n_samples, n_selected_features)
-            The selected features from the input dataframe.
-        """
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    def _more_tags(self):
-        return {"allow_nan": True, "requires_y": True}
-
-    @mpl.rc_context(PLT_PARAMS)
-    def plot_importance(self, n_feat_per_inch=5):
-        """
-        Plot the feature importance of the fitted GrootCV.
-
-        Parameters
-        ----------
-        n_feat_per_inch : int, default=5
-            The number of features per inch in the plot.
-
-        Returns
-        -------
-        fig : matplotlib.figure.Figure or None
-            The matplotlib figure containing the plot or None if no feature is selected.
-        """
-
-        if self.sha_cutoff is None:
-            raise ValueError("Apply fit method first")
-
-        b_df = self.cv_df.T.copy()
-        b_df.columns = b_df.iloc[0]
-        b_df = b_df.drop(b_df.index[0])
-        b_df = b_df.drop(b_df.index[-1])
-        b_df = b_df.convert_dtypes()
-        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
-        sha_df = b_df.iloc[:, int(b_df.shape[1] / 2) :].copy()
-
-        real_df = real_df.reindex(
-            real_df.select_dtypes(include=[np.number])
-            .mean()
-            .sort_values(ascending=True)
-            .index,
-            axis=1,
-        )
-
-        if real_df.dropna().empty:
-            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
-            return None
-        else:
-            fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
-            bp = real_df.plot(**PLOT_KWARGS, ax=ax)
-            col_idx = np.argwhere(real_df.columns.isin(self.selected_features_)).ravel()
-
-            for c in range(real_df.shape[1]):
-                bp.findobj(mpl.patches.Patch)[c].set_facecolor("gray")
-                bp.findobj(mpl.patches.Patch)[c].set_color("gray")
-
-            for c in col_idx:
-                bp.findobj(mpl.patches.Patch)[c].set_facecolor(BLUE)
-                bp.findobj(mpl.patches.Patch)[c].set_color(BLUE)
-
-            ax.axvline(x=self.sha_cutoff, linestyle="--", color=RED)
-            bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
-            custom_lines = [
-                Line2D([0], [0], color=BLUE, lw=5),
-                Line2D([0], [0], color="gray", lw=5),
-                Line2D([0], [0], linestyle="--", color=RED, lw=2),
-            ]
-            bp.legend(
-                custom_lines, ["confirmed", "rejected", "threshold"], loc="lower right"
-            )
-            ax.set_title("Groot CV importance and selected predictors")
-
-            return fig
-
-
-########################################################################################
-#
-# GrootCV. In principle, you cannot/don't need to access those methods (reason of
-# the _ in front of the function name, they're internal functions)
-#
-########################################################################################
-
-
-def _reduce_vars_lgb_cv(
-    X,
-    y,
-    objective,
-    n_folds,
-    cutoff,
-    n_iter,
-    silent,
-    weight,
-    rf,
-    fastshap,
-    lgbm_params=None,
-    n_jobs=0,
-):
-    """
-    Reduce the number of predictors using a lightgbm (python API)
-
-    Parameters
-    ----------
-    X : pd.DataFrame
-            the dataframe to create shadow features on
-    y : pd.Series
-            the target
-    objective : str
-            the lightGBM objective
-    cutoff : float
-            the value by which the max of shadow imp is divided, to compare to real importance
-    n_iter : int
-            The number of repetition of the cross-validation, smooth out the feature importance noise
-    silent : bool
-            Set to True if don't want to see the BoostARoota output printed.
-            Will still show any errors or warnings that may occur
-    weight : pd.series
-            sample_weight, if any
-    rf : bool, default=False
-            the lightGBM implementation of the random forest
-    fastshap : bool
-            enable or not the fasttreeshap implementation
-    lgbm_params : dict, optional
-            dictionary of lightgbm parameters
-    n_jobs: int, default 0
-        0 means default number of threads in OpenMP
-        for the best speed, set this to the number of real CPU cores, not the number of threads
-
-    Returns
-    -------
-    real_vars['feature'] : pd.dataframe
-            feature importance of the real predictors over iter
-    df : pd.DataFrame
-            feature importance of the real+shadow predictors over iter
-    cutoff_shadow : float
-            the feature importance threshold, to reject or not the predictors
-    """
-
-    params = _set_lgb_parameters(
-        X=X,
-        y=y,
-        objective=objective,
-        rf=rf,
-        silent=silent,
-        n_jobs=n_jobs,
-        lgbm_params=lgbm_params,
-    )
-
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-    category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
-    cat_idx = [X.columns.get_loc(col) for col in category_cols]
-
-    rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
-    iter = 0
-    df = pd.DataFrame({"feature": X.columns})
-    for tridx, validx in tqdm(
-        rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
-    ):
-        X_train, X_val, y_train, y_val, weight_tr, weight_val = _split_data(
-            X, y, tridx, validx, weight
-        )
-
-        # Create the shadow variables and run the model to obtain importances
-        new_x_tr, shadow_names = _create_shadow(X_train)
-        new_x_val, _ = _create_shadow(X_val)
-
-        bst, shap_matrix, bst.best_iteration = _train_lgb_model(
-            new_x_tr,
-            y_train,
-            weight_tr,
-            new_x_val,
-            y_val,
-            weight_val,
-            category_cols=category_cols,
-            early_stopping_rounds=20,
-            fastshap=fastshap,
-            **params,
-        )
-
-        importance = _compute_importance(
-            new_x_tr, shap_matrix, params, objective, fastshap
-        )
-        df = _merge_importance_df(
-            df=df,
-            importance=importance,
-            iter=iter,
-            n_folds=n_folds,
-            column_names=new_x_tr.columns,
-            silent=silent,
-        )
-        iter += 1
-
-    df["Med"] = df.select_dtypes(include=[np.number]).mean(axis=1)
-    # Split them back out
-    real_vars = df[~df["feature"].isin(shadow_names)]
-    shadow_vars = df[df["feature"].isin(shadow_names)]
-
-    # Get median value from the shadows, comparing predictor by predictor. Not the same criteria
-    # max().max() like in Boruta but max of the median to mitigate.
-    # Otherwise too conservative (reject too often)
-    cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
-    real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
-
-    return real_vars["feature"], df, cutoff_shadow
-
-
-def _set_lgb_parameters(
-    X: np.ndarray,
-    y: np.ndarray,
-    objective: str,
-    rf: bool,
-    silent: bool,
-    n_jobs: int = 0,
-    lgbm_params: dict = None,
-) -> dict:
-    """Set parameters for a LightGBM model based on the input features and the objective.
-
-    Parameters
-    ----------
-    X : numpy array or pandas DataFrame
-        The feature matrix of the training data.
-    y : numpy array or pandas Series
-        The target variable of the training data.
-    objective : str
-        The objective function to optimize during training.
-    rf : bool, default False
-        Whether to use random forest boosting.
-    silent : bool, default True
-        Whether to print messages during parameter setting.
-    n_jobs: int, default 0
-        0 means default number of threads in OpenMP
-        for the best speed, set this to the number of real CPU cores, not the number of threads
-
-    Returns
-    -------
-    dict
-        The dictionary of LightGBM parameters.
-
-    """
-
-    n_feat = X.shape[1]
-
-    params = lgbm_params if lgbm_params is not None else {}
-
-    params["objective"] = objective
-    params["verbosity"] = -1
-    if objective == "softmax":
-        params["num_class"] = len(np.unique(y))
-
-    if rf:
-        feat_frac = (
-            np.sqrt(n_feat) / n_feat
-            if objective in ["softmax", "binary"]
-            else n_feat / (3 * n_feat)
-        )
-        params.update(
-            {
-                "boosting_type": "rf",
-                "bagging_fraction": 0.7,
-                "feature_fraction": feat_frac,
-                "bagging_freq": 1,
-            }
-        )
-
-    clf_losses = [
-        "binary",
-        "softmax",
-        "multi_logloss",
-        "multiclassova",
-        "multiclass",
-        "multiclass_ova",
-        "ova",
-        "ovr",
-        "binary_logloss",
-    ]
-    if objective in clf_losses:
-        y = y.astype(int)
-        y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
-        n_classes = y_freq_table.size
-        if n_classes > 2 and objective != "softmax":
-            params["objective"] = "softmax"
-            params["num_class"] = len(np.unique(y))
-            if not silent:
-                print("Multi-class task, setting objective to softmax")
-        main_class = y_freq_table[0]
-        if not silent:
-            print("GrootCV: classification with unbalance classes")
-        if main_class > 0.8:
-            params.update({"is_unbalance": True})
-
-    params.update({"num_threads": n_jobs})
-
-    # we are using early_stopping
-    # we prevent the overridding of it by popping the n_iterations
-    keys_to_pop = [
-        "num_iterations",
-        "num_iteration",
-        "n_iter",
-        "num_tree",
-        "num_trees",
-        "num_round",
-        "num_rounds",
-        "nrounds",
-        "num_boost_round",
-        "n_estimators",
-        "max_iter",
-    ]
-    for key in keys_to_pop:
-        params.pop(key, None)
-
-    return params
-
-
-def _split_data(X, y, tridx, validx, weight=None):
-    """
-    Split data into train and validation sets based on provided indices.
-
-    Parameters
-    ----------
-    X : pandas.DataFrame
-        Features.
-    y : pandas.Series
-        Target variable.
-    tridx : list
-        Indices to be used for training.
-    validx : list
-        Indices to be used for validation.
-    weight : pandas.Series, optional
-        Weights for each sample, by default None.
-
-    Returns
-    -------
-    tuple of pandas.DataFrame and pandas.Series
-        X_train, X_val, y_train, y_val, weight_tr, weight_val
-    """
-    if weight is not None:
-        X_train, y_train, weight_tr = (
-            X.iloc[tridx, :],
-            y.iloc[tridx],
-            weight.iloc[tridx],
-        )
-        X_val, y_val, weight_val = (
-            X.iloc[validx, :],
-            y.iloc[validx],
-            weight.iloc[validx],
-        )
-    else:
-        X_train, y_train = X.iloc[tridx, :], y.iloc[tridx]
-        X_val, y_val = X.iloc[validx, :], y.iloc[validx]
-        weight_tr = None
-        weight_val = None
-    return X_train, X_val, y_train, y_val, weight_tr, weight_val
-
-
-def _train_lgb_model(
-    X_train,
-    y_train,
-    weight_train,
-    X_val,
-    y_val,
-    weight_val,
-    category_cols=None,
-    early_stopping_rounds=20,
-    fastshap=True,
-    **params,
-):
-    """
-    Train a LightGBM model with the given training data and hyperparameters and return the trained model and its SHAP values.
-
-    Parameters
-    ----------
-    X_train : array-like of shape (n_samples, n_features)
-        The input training data.
-    y_train : array-like of shape (n_samples,)
-        The target training data.
-    weight_train : array-like of shape (n_samples,)
-        The sample weights for training data.
-    X_val : array-like of shape (n_val_samples, n_features)
-        The input validation data.
-    y_val : array-like of shape (n_val_samples,)
-        The target validation data.
-    weight_val : array-like of shape (n_val_samples,)
-        The sample weights for validation data.
-    category_cols : array-like or None, optional (default=None)
-        The indices of categorical columns. If None, no categorical columns will be considered.
-    early_stopping_rounds : int, optional (default=20)
-        Activates early stopping. Validation metric needs to improve at least once in every early_stopping_rounds
-        round(s) to continue training._train_lgb_model
-    fastshap : bool
-        enable or not fasttreeshap implementation
-    **params : dict
-        Other parameters passed to the LightGBM model.
-
-    Returns
-    -------
-    tuple of (Booster, numpy.ndarray, int)
-        The trained LightGBM model, its SHAP values for X_train, and the best iteration reached during training.
-    """
-
-    d_train = lgb.Dataset(
-        X_train, label=y_train, weight=weight_train, categorical_feature=category_cols
-    )
-    d_valid = lgb.Dataset(
-        X_val, label=y_val, weight=weight_val, categorical_feature=category_cols
-    )
-    watchlist = [d_train, d_valid]
-
-    bst = lgb.train(
-        params,
-        train_set=d_train,
-        num_boost_round=10000,
-        valid_sets=watchlist,
-        categorical_feature=category_cols,
-        callbacks=[early_stopping(early_stopping_rounds, False, False)],
-    )
-
-    if fastshap:
-        try:
-            from fasttreeshap import TreeExplainer as FastTreeExplainer
-        except ImportError:
-            raise ImportError(
-                "fasttreeshap is not installed. Please install it using 'pip/conda install fasttreeshap'."
-            )
-
-        explainer = FastTreeExplainer(
-            bst,
-            algorithm="auto",
-            shortcut=False,
-            feature_perturbation="tree_path_dependent",
-        )
-        shap_matrix = explainer.shap_values(X_train)
-    else:
-        shap_matrix = bst.predict(X_train, pred_contrib=True)
-
-    return bst, shap_matrix, bst.best_iteration
-
-
-def _compute_importance(new_x_tr, shap_matrix, param, objective, fastshap):
-    """Compute feature importance scores using SHAP values.
-
-    Parameters
-    ----------
-    new_x_tr : numpy.ndarray
-        The training dataset after being processed.
-    shap_matrix : numpy.ndarray
-        The matrix containing SHAP values computed by a LightGBM model.
-    param : dict
-        A dictionary containing the parameters for a LightGBM model.
-    objective : str
-        The objective function of the LightGBM model.
-
-    Returns
-    -------
-    list
-        A list of tuples containing feature names and their corresponding importance scores.
-    """
-    if fastshap:
-        if objective == "softmax":
-            shap_matrix = np.abs(np.concatenate(shap_matrix, axis=1))
-        shap_imp = np.mean(np.abs(shap_matrix), axis=0)
-    else:
-        if objective == "softmax":
-            n_feat = new_x_tr.shape[1]
-            shap_matrix = np.delete(
-                shap_matrix,
-                list(range(n_feat, (n_feat + 1) * param["num_class"], n_feat + 1)),
-                axis=1,
-            )
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
-        else:
-            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
-    importance = dict(zip(new_x_tr.columns, shap_imp))
-    return sorted(importance.items(), key=operator.itemgetter(1))
-
-
-def _merge_importance_df(df, importance, iter, n_folds, column_names, silent=True):
-    """
-    Merge the feature importance dataframe `df` with the importance
-    information for the current iteration of a cross-validation loop.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        The current feature importance dataframe.
-    importance : dict
-        A dictionary with the feature importance information for
-        the current iteration.
-    i : int
-        The index of the current iteration.
-    n_folds : int
-        The number of folds used in the cross-validation loop.
-    silent : bool, optional
-        If True, suppress output.
-
-    Returns
-    -------
-    pandas.DataFrame
-        The updated feature importance dataframe.
-    """
-
-    df2 = pd.DataFrame(importance, columns=["feature", "fscore" + str(iter)])
-    df2["fscore" + str(iter)] = (
-        df2["fscore" + str(iter)] / df2["fscore" + str(iter)].sum()
-    )
-    df = pd.merge(df, df2, on="feature", how="outer")
-    nit = divmod(iter, n_folds)[0]
-    nf = divmod(iter, n_folds)[1]
-    if not silent:
-        if nf == 0:
-            print("Groot iteration: ", nit, " with " + str(n_folds) + " folds")
-    return df
+"""This module provides 3 different methods to perform 'all relevant feature selection'
+
+
+Reference:
+----------
+NILSSON, Roland, PEÑA, José M., BJÖRKEGREN, Johan, et al.
+Consistent feature selection for pattern recognition in polynomial time.
+Journal of Machine Learning Research, 2007, vol. 8, no Mar, p. 589-612.
+
+KURSA, Miron B., RUDNICKI, Witold R., et al.
+Feature selection with the Boruta package.
+J Stat Softw, 2010, vol. 36, no 11, p. 1-13.
+
+https://github.com/chasedehan/BoostARoota
+
+The module structure
+--------------------
+- The ``Leshy`` class, a heavy re-work of ``BorutaPy`` class
+  itself a modified version of Boruta, the pull request I submitted and still pending:
+  https://github.com/scikit-learn-contrib/boruta_py/pull/100
+
+- The ``BoostAGroota`` class, a modified version of BoostARoota, PR still to be submitted
+  https://github.com/chasedehan/BoostARoota
+
+- The ``GrootCV`` class for a new method for all relevant feature selection using a lightgGBM model,
+  cross-validated SHAP importances and shadowing.
+
+Original BorutaPy version
+-------------------------
+Author: Daniel Homola <dani.homola@gmail.com>
+
+Original code and method by: Miron B Kursa, https://m2.icm.edu.pl/boruta/
+Modified by Thomas Bury, pull request:
+https://github.com/scikit-learn-contrib/boruta_py/pull/100
+Waiting for merging
+
+https://github.com/scikit-learn-contrib/boruta_py/pull/100
+is a new PR based on #77 making all the changes optional. Waiting for merge
+
+Leshy is a re-work of the PR I submitted.
+
+License: BSD 3 clause
+
+"""
+
+from __future__ import print_function, division
+import operator
+import warnings
+import time
+import shap
+import numpy as np
+import pandas as pd
+import lightgbm as lgb
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import scipy as sp
+
+from typing import Tuple
+from tqdm.auto import tqdm
+from sklearn.utils import check_random_state, check_X_y
+from sklearn.base import BaseEstimator, is_regressor, is_classifier, clone
+
+from sklearn.utils.validation import check_is_fitted
+from sklearn.feature_selection._base import SelectorMixin
+from sklearn.model_selection import RepeatedKFold, train_test_split
+from sklearn.inspection import permutation_importance
+from sklearn.utils.validation import _check_sample_weight
+from matplotlib.lines import Line2D
+from lightgbm import early_stopping
+
+
+from ..utils import (
+    check_if_tree_based,
+    is_lightgbm,
+    is_catboost,
+    create_dtype_dict,
+    get_pandas_cat_codes,
+    validate_sample_weight,
+)
+
+########################################################################################
+#
+# Main Classes and Methods
+# Provide a fit, transform and fit_transform method
+#
+########################################################################################
+# !/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+NO_FEATURE_SELECTED_WARNINGS = "No feature selected - No data to plot"
+ARFS_COLOR_LIST = [
+    "#000000",
+    "#7F3C8D",
+    "#11A579",
+    "#3969AC",
+    "#F2B701",
+    "#E73F74",
+    "#80BA5A",
+    "#E68310",
+    "#008695",
+    "#CF1C90",
+    "#F97B72",
+]
+BLUE = "#2590fa"
+YELLOW = "#f0be00"
+RED = "#b51204"
+BCKGRD_COLOR = "#f5f5f5"
+PLT_PARAMS = {
+    "axes.prop_cycle": plt.cycler(color=ARFS_COLOR_LIST),
+    "axes.facecolor": BCKGRD_COLOR,
+    "patch.edgecolor": BCKGRD_COLOR,
+    "figure.facecolor": BCKGRD_COLOR,
+    "axes.edgecolor": BCKGRD_COLOR,
+    "savefig.edgecolor": BCKGRD_COLOR,
+    "savefig.facecolor": BCKGRD_COLOR,
+    "grid.color": "#d2d2d2",
+    "lines.linewidth": 1.5,
+}
+PLOT_KWARGS = dict(
+    kind="box",
+    boxprops=dict(linestyle="-", linewidth=1.5, color="gray", facecolor="gray"),
+    flierprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    medianprops=dict(linestyle="-", linewidth=1.5, color="#000000"),
+    whiskerprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    capprops=dict(linestyle="-", linewidth=1.5, color="gray"),
+    showfliers=False,
+    grid=True,
+    rot=0,
+    vert=False,
+    patch_artist=True,
+    fontsize=9,
+)
+
+
+class Leshy(SelectorMixin, BaseEstimator):
+    """This is an improved version of BorutaPy which itself is an
+    improved Python implementation of the Boruta R package.
+    Boruta is an all relevant feature selection method, while most other are
+    minimal optimal; this means it tries to find all features carrying
+    information usable for prediction, rather than finding a possibly compact
+    subset of features on which some estimator has a minimal error.
+    Why bother with all relevant feature selection?
+    When you try to understand the phenomenon that made your data, you should
+    care about all factors that contribute to it, not just the bluntest signs
+    of it in context of your methodology (minimal optimal set of features
+    by definition depends on your estimator choice).
+
+    Parameters
+    ----------
+    estimator : object
+        A supervised learning estimator, with a 'fit' method that returns the
+        ``feature_importances_`` attribute. Important features must correspond to
+        high absolute values in the ``feature_importances_``
+    n_estimators : int or string, default = 1000
+        If int sets the number of estimators in the chosen ensemble method.
+        If 'auto' this is determined automatically based on the size of the
+        dataset. The other parameters of the used estimators need to be set
+        with initialisation.
+    perc : int, default = 100
+        Instead of the max we use the percentile defined by the user, to pick
+        our threshold for comparison between shadow and real features. The max
+        tend to be too stringent. This provides a finer control over this. The
+        lower perc is the more false positives will be picked as relevant but
+        also the less relevant features will be left out. The usual trade-off.
+        The default is essentially the vanilla Boruta corresponding to the max.
+    alpha : float, default = 0.05
+        Level at which the corrected p-values will get rejected in both
+        correction steps.
+    importance : str, default = 'shap'
+        The kind of variable importance used to compare and discriminate original
+        vs shadow predictors. Note that the builtin tree importance (gini/impurity based
+        importance) is biased towards numerical and large cardinality predictors, even
+        if they are random. Shapley values and permutation imp. are robust w.r.t those predictors.
+        Possible values: 'shap' (Shapley values), 'fastshap' (FastTreeShap implementation),
+        'pimp' (permutation importance) and 'native' (Gini/impurity)
+    two_step : Boolean, default = True
+        If you want to use the original implementation of Boruta with Bonferroni
+        correction only set this to False.
+    max_iter : int, default = 100
+        The number of maximum iterations to perform.
+    random_state : int, RandomState instance or None; default=None
+        If int, random_state is the seed used by the random number generator;
+        If RandomState instance, random_state is the random number generator;
+        If None, the random number generator is the RandomState instance used
+        by `np.random`.
+    verbose : int, default=0
+        Controls verbosity of output. 0: no output, 1: displays iteration number,
+        2: which features have been selected already
+
+
+    Attributes
+    ----------
+    n_features_ : int
+        The number of selected features.
+    support_ : array of shape [n_features]
+        The mask of selected features - only confirmed ones are True.
+    support_weak_ : array of shape [n_features]
+        The mask of selected tentative features, which haven't gained enough
+        support during the max_iter number of iterations.
+    selected_features_ : list of str
+        the list of columns to keep
+    ranking_ : array of shape [n_features]
+        The feature ranking, such that ``ranking_[i]`` corresponds to the
+        ranking position of the i-th feature. Selected (i.e., estimated
+        best) features are assigned rank one and tentative features are assigned
+        rank 2.
+    ranking_absolutes_ : array of shape [n_features]
+        The absolute feature ranking as ordered by selection process. It does not guarantee
+        that this order is correct for all models. For a model agnostic ranking, see the
+        the attribute ``ranking``
+    cat_name : list of str
+        the name of the categorical columns
+    cat_idx : list of int
+        the index of the categorical columns
+    imp_real_hist : array
+        array of the historical feature importance of the real predictors
+    sha_max : float
+        the maximum feature importance of the shadow predictors
+    col_names : list of str
+        the names of the real predictors
+
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> from sklearn.ensemble import RandomForestClassifier
+    >>> from boruta import BorutaPy
+    >>>
+    >>> # load X and y
+    >>> # NOTE BorutaPy accepts numpy arrays only, hence the .values attribute
+    >>> X = pd.read_csv('examples/test_X.csv', index_col=0).values
+    >>> y = pd.read_csv('examples/test_y.csv', header=None, index_col=0).values
+    >>> y = y.ravel()
+    >>>
+    >>> # define random forest classifier, with utilising all cores and
+    >>> # sampling in proportion to y labels
+    >>> rf = RandomForestClassifier(n_jobs=-1, class_weight='balanced', max_depth=5)
+    >>>
+    >>> # define Boruta feature selection method
+    >>> feat_selector = Leshy(rf, n_estimators='auto', verbose=2, random_state=1)
+    >>>
+    >>> # find all relevant features - 5 features should be selected
+    >>> feat_selector.fit(X, y)
+    >>>
+    >>> # check selected features - first 5 features are selected
+    >>> feat_selector.selected_features_
+    >>>
+    >>> # check ranking of features
+    >>> feat_selector.ranking_
+    >>>
+    >>> # call transform() on X to filter it down to selected features
+    >>> X_filtered = feat_selector.transform(X)
+
+    References
+    ----------
+    See the original paper [1]_ for more details.
+
+    ..[1] Kursa M., Rudnicki W., "Feature Selection with the Boruta Package"
+        Journal of Statistical Software, Vol. 36, Issue 11, Sep 2010
+
+    """
+
+    def __init__(
+        self,
+        estimator,
+        n_estimators=1000,
+        perc=90,
+        alpha=0.05,
+        importance="shap",
+        two_step=True,
+        max_iter=100,
+        random_state=None,
+        verbose=0,
+        keep_weak=False,
+    ):
+        self.estimator = estimator
+        self.n_estimators = n_estimators
+        self.perc = perc
+        self.alpha = alpha
+        self.two_step = two_step
+        self.max_iter = max_iter
+        self.random_state = random_state
+        self.random_state_instance = None
+        self.verbose = verbose
+        self.keep_weak = keep_weak
+        self.importance = importance
+        self.cat_name = None
+        self.cat_idx = None
+        # Catboost doesn't allow to change random seed after fitting
+        self.is_cat = is_catboost(estimator)
+        self.is_lgb = is_lightgbm(estimator)
+        # plotting
+        self.imp_real_hist = None
+        self.sha_max = None
+        self.n_features_ = 0
+        self.support_ = None
+        self.support_weak_ = None
+
+    def fit(self, X, y, sample_weight=None):
+        """Fits the Boruta feature selection with the provided estimator.
+
+        Parameters
+        ----------
+        X : array-like, shape = [n_samples, n_features]
+            The training input samples.
+        y : array-like, shape = [n_samples]
+            The target values.
+        sample_weight : array-like, shape = [n_samples], default=None
+            Individual weights for each sample
+
+        Returns
+        -------
+        self : object
+            Nothing but attributes
+
+        """
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
+            self.importance = "shap"
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+        else:
+            raise TypeError("X is not a dataframe")
+
+        self.imp_real_hist = np.empty((0, X.shape[1]), float)
+        self._fit(X, y, sample_weight=sample_weight)
+        self.selected_features_ = self.feature_names_in_[self.support_]
+        self.not_selected_features_ = self.feature_names_in_[~self.support_]
+
+        return self
+
+    def transform(self, X):
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    @mpl.rc_context(PLT_PARAMS)
+    def plot_importance(self, n_feat_per_inch=5):
+        """Boxplot of the variable importance, ordered by magnitude
+        The max shadow variable importance illustrated by the dashed line.
+        Requires to apply the fit method first.
+
+        Parameters
+        ----------
+        n_feat_per_inch : int, default=5
+            number of features to plot per inch (for scaling the figure)
+
+        Returns
+        -------
+        fig : plt.figure
+            the matplotlib figure object containing the boxplot
+        """
+
+        if self.imp_real_hist is None:
+            raise ValueError("Use the fit method first to compute the var.imp")
+
+        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
+        vimp_df = vimp_df.reindex(
+            vimp_df.mean().sort_values(ascending=True).index, axis=1
+        )
+
+        if vimp_df.dropna().empty:
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
+            return None
+        else:
+            fig, ax = plt.subplots(figsize=(16, vimp_df.shape[1] / n_feat_per_inch))
+            bp = vimp_df.plot(**PLOT_KWARGS, ax=ax)
+
+            n_strong = sum(self.support_)
+            n_weak = np.sum(self.support_weak_)
+            n_discarded = np.sum(~(self.support_ | self.support_weak_))
+            box_face_col = (
+                [BLUE] * n_strong + [YELLOW] * n_weak + ["gray"] * n_discarded
+            )
+            for c in range(len(box_face_col)):
+                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_facecolor(
+                    box_face_col[c]
+                )
+                bp.findobj(mpl.patches.Patch)[len(self.support_) - c - 1].set_color(
+                    box_face_col[c]
+                )
+
+            xrange = vimp_df.max(skipna=True).max(skipna=True) - vimp_df.min(
+                skipna=True
+            ).min(skipna=True)
+            bp.set_xlim(left=vimp_df.min(skipna=True).min(skipna=True) - 0.10 * xrange)
+
+            custom_lines = [
+                Line2D([0], [0], color=BLUE, lw=5),
+                Line2D([0], [0], color=YELLOW, lw=5),
+                Line2D([0], [0], color="gray", lw=5),
+                Line2D([0], [0], linestyle="--", color=RED, lw=2),
+            ]
+            bp.legend(
+                custom_lines,
+                ["confirmed", "tentative", "rejected", "sha. max"],
+                loc="lower right",
+            )
+            ax.axvline(x=self.sha_max, linestyle="--", color=RED)
+            ax.set_title("Leshy importance and selected predictors")
+            return fig
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def _more_tags(self):
+        return {"allow_nan": True, "requires_y": True}
+
+    def _fit(self, X_raw, y, sample_weight=None):
+        """Private method. See the methods overview in the documentation
+        for explanation of the process
+
+        Parameters
+        ----------
+        X_raw : array-like, shape = [n_samples, n_features]
+            The training input samples.
+        y : array-like, shape = [n_samples]
+            The target values.
+        sample_weight : array-like, shape = [n_samples], default=None
+            Individual weights for each sample
+
+        Returns
+        -------
+        self : object
+            Nothing but attributes
+        """
+
+        start_time = time.time()
+        # the basic cat features encoding
+        # is performed when getting importances
+        # because the columns are dynamically created/rejected
+        X = X_raw
+
+        # only sklearn requires to fillna data
+        # modern GBM implementations can handle this
+        # X = X.fillna(0)
+        y = pd.Series(y).fillna(0) if not isinstance(y, pd.Series) else y.fillna(0)
+
+        # check input params
+        self._check_params(X, y)
+        sample_weight = validate_sample_weight(sample_weight)
+        self.random_state = check_random_state(self.random_state)
+
+        # setup variables for Boruta
+        n_sample, n_feat = X.shape
+        _iter = 1
+        # holds the decision about each feature:
+        # 0  - default state = tentative in original code
+        # 1  - accepted in original code
+        # -1 - rejected in original code
+        dec_reg = np.zeros(n_feat, dtype=int)
+        # counts how many times a given feature was more important than
+        # the best of the shadow features
+        hit_reg = np.zeros(n_feat, dtype=int)
+        # these record the history of the iterations
+        imp_history = np.zeros(n_feat, dtype=float)
+        sha_max_history = []
+
+        # set n_estimators
+        if self.n_estimators != "auto":
+            self.estimator.set_params(n_estimators=self.n_estimators)
+
+        dec_reg, sha_max_history, imp_history, imp_sha_max = self.select_features(
+            X=X, y=y, sample_weight=sample_weight
+        )
+        confirmed, tentative = _get_confirmed_and_tentative(dec_reg)
+        tentative = _select_tentative(tentative, imp_history, sha_max_history)
+        self._calculate_support(confirmed, tentative, n_feat)
+
+        # for plotting
+        self.imp_real_hist = imp_history
+        self.sha_max = imp_sha_max
+
+        # absolute and relative ranking
+        self._calculate_absolute_ranking()
+        self._calculate_relative_ranking(
+            n_feat=n_feat,
+            tentative=tentative,
+            confirmed=confirmed,
+            imp_history=imp_history,
+        )
+        self._print_result(dec_reg, _iter, start_time)
+        return self
+
+    def _get_tree_num(self, n_feat):
+        """private method, get a good estimated for the number of trees
+           given the number of features
+
+        Parameters
+        ----------
+        n_feat : int
+            The number of features
+
+        Returns
+        -------
+        n_estimators : int
+            the number of trees
+        """
+        depth = (
+            self.estimator.get_params()["max_depth"]
+            if not self.is_cat
+            else self.estimator.get_param("max_depth")
+        )
+        if depth is None:
+            depth = 10
+        # how many times a feature should be considered on average
+        f_repr = 100
+        # n_feat * 2 because the training matrix is extended with n shadow features
+        multi = (n_feat * 2) / (np.sqrt(n_feat * 2) * depth)
+        n_estimators = int(multi * f_repr)
+        return n_estimators
+
+    def _add_shadows_get_imps(self, X, y, sample_weight, dec_reg):
+        """Add a shuffled copy of the columns (shadows) and get the feature
+        importance of the augmented data set
+
+        Parameters
+        ----------
+        X: pd.DataFrame of shape [n_samples, n_features]
+            predictor matrix
+        y: pd.series of shape [n_samples]
+            target
+        sample_weight: array-like, shape = [n_samples], default=None
+            Individual weights for each sample
+        dec_reg: array
+            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
+        Returns
+        -------
+         imp_real: array
+            feature importance of the real predictors
+         imp_sha: array
+            feature importance of the shadow predictors
+        """
+        # find features that are tentative still
+        x_cur_ind = np.where(dec_reg >= 0)[0]
+        x_cur = X.iloc[:, x_cur_ind].copy()
+        x_cur_w = x_cur.shape[1]
+        # deep copy the matrix for the shadow matrix
+        x_sha = x_cur.copy()
+        # make sure there's at least 5 columns in the shadow matrix for
+        while x_sha.shape[1] < 5:
+            x_sha = pd.concat([x_sha, x_sha], axis=1)
+        # shuffle xSha
+        x_sha = x_sha.apply(self.random_state.permutation, axis=0)
+        x_sha.columns = [f"Shadow_{i}" for i in range(x_sha.shape[1])]
+        # get importance of the merged matrix
+        if self.importance == "shap":
+            imp = _get_shap_imp(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
+        elif self.importance == "fastshap":
+            imp = _get_shap_imp_fast(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
+        elif self.importance == "pimp":
+            imp = _get_perm_imp(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
+        else:
+            imp = _get_imp(
+                self.estimator, pd.concat([x_cur, x_sha], axis=1), y, sample_weight
+            )
+
+        # separate importances of real and shadow features
+        imp_sha = imp[x_cur_w:]
+        imp_real = np.zeros(X.shape[1])
+        imp_real[:] = np.nan
+        imp_real[x_cur_ind] = imp[:x_cur_w]
+
+        return imp_real, imp_sha
+
+    @staticmethod
+    def _assign_hits(hit_reg, cur_imp, imp_sha_max):
+        """count how many times a given feature was more important than
+        the best of the shadow features
+
+        Parameters
+        ----------
+        hit_reg: array
+            count how many times a given feature was more important than the
+            best of the shadow features
+        cur_imp: array
+            current importance
+        imp_sha_max: array
+            importance of the best shadow predictor
+        Returns
+        -------
+        hit_reg : array
+            the how many times a given feature was more important than the
+            best of the shadow features
+        """
+        # register hits for features that did better than the best of shadows
+        cur_imp_no_nan = cur_imp[0]
+        cur_imp_no_nan[np.isnan(cur_imp_no_nan)] = 0
+        hits = np.where(cur_imp_no_nan > imp_sha_max)[0]
+        hit_reg[hits] += 1
+        return hit_reg
+
+    def _do_tests(self, dec_reg, hit_reg, _iter):
+        """Private method, Perform the rest if the feature should be tagget as relevant (confirmed), not relevant (rejected)
+        or undecided. The test is performed by considering the binomial tentatives over several attempts.
+        I.e. count how many times a given feature was more important than the best of the shadow features
+        and test if the associated probability to the z-score is below, between or above the rejection or
+        acceptance threshold.
+
+        Parameters
+        ----------
+        dec_reg : array
+            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
+        hit_reg : array
+            counts how many times a given feature was more important than the best of the shadow features
+        _iter : int
+            iteration number
+        Returns
+        -------
+        dec_reg : array
+            holds the decision about each feature 1, 0, -1 (accepted, undecided, rejected)
+
+        """
+        active_features = np.where(dec_reg >= 0)[0]
+        hits = hit_reg[active_features]
+        # get uncorrected p values based on hit_reg
+        to_accept_ps = sp.stats.binom.sf(hits - 1, _iter, 0.5).flatten()
+        to_reject_ps = sp.stats.binom.cdf(hits, _iter, 0.5).flatten()
+
+        if self.two_step:
+            # two step multicor process
+            # first we correct for testing several features in each round using FDR
+            to_accept = self._fdrcorrection(to_accept_ps, alpha=self.alpha)[0]
+            to_reject = self._fdrcorrection(to_reject_ps, alpha=self.alpha)[0]
+
+            # second we correct for testing the same feature over and over again
+            # using bonferroni
+            to_accept2 = to_accept_ps <= self.alpha / float(_iter)
+            to_reject2 = to_reject_ps <= self.alpha / float(_iter)
+
+            # combine the two multi corrections, and get indexes
+            to_accept *= to_accept2
+            to_reject *= to_reject2
+        else:
+            # as in th original Boruta, we simply do bonferroni correction
+            # with the total n_feat in each iteration
+            to_accept = to_accept_ps <= self.alpha / float(len(dec_reg))
+            to_reject = to_reject_ps <= self.alpha / float(len(dec_reg))
+
+        # find features which are 0 and have been rejected or accepted
+        to_accept = np.where((dec_reg[active_features] == 0) * to_accept)[0]
+        to_reject = np.where((dec_reg[active_features] == 0) * to_reject)[0]
+
+        # updating dec_reg
+        dec_reg[active_features[to_accept]] = 1
+        dec_reg[active_features[to_reject]] = -1
+        return dec_reg
+
+    @staticmethod
+    def _fdrcorrection(pvals, alpha=0.05):
+        """Benjamini/Hochberg p-value correction for false discovery rate, from
+        statsmodels package. Included here for decoupling dependency on statsmodels.
+
+        Parameters
+        ----------
+        pvals : array_like
+            set of p-values of the individual tests.
+        alpha : float
+            error rate
+        Returns
+        -------
+        rejected : array, bool
+            True if a hypothesis is rejected, False if not
+        pvalue-corrected : array
+            pvalues adjusted for multiple hypothesis testing to limit FDR
+        """
+        pvals = np.asarray(pvals)
+        pvals_sortind = np.argsort(pvals)
+        pvals_sorted = np.take(pvals, pvals_sortind)
+        nobs = len(pvals_sorted)
+        ecdffactor = np.arange(1, nobs + 1) / float(nobs)
+
+        reject = pvals_sorted <= ecdffactor * alpha
+        if reject.any():
+            rejectmax = max(np.nonzero(reject)[0])
+            reject[:rejectmax] = True
+
+        pvals_corrected_raw = pvals_sorted / ecdffactor
+        pvals_corrected = np.minimum.accumulate(pvals_corrected_raw[::-1])[::-1]
+        pvals_corrected[pvals_corrected > 1] = 1
+        # reorder p-values and rejection mask to original order of pvals
+        pvals_corrected_ = np.empty_like(pvals_corrected)
+        pvals_corrected_[pvals_sortind] = pvals_corrected
+        reject_ = np.empty_like(reject)
+        reject_[pvals_sortind] = reject
+        return reject_, pvals_corrected_
+
+    @staticmethod
+    def _nanrankdata(X, axis=1):
+        """Replaces bottleneck's nanrankdata with scipy and numpy alternative.
+
+        Parameters
+        ----------
+        X : array or pd.DataFrame
+            the data array
+        axis : int, optional
+            row-wise (0) or column-wise (1), by default 1
+
+        Returns
+        -------
+        ranks : array
+            the ranked array
+        """
+        ranks = sp.stats.mstats.rankdata(X, axis=axis)
+        ranks[np.isnan(X)] = np.nan
+        return ranks
+
+    def _check_params(self, X, y):
+        """Private method, Check hyperparameters as well as X and y before proceeding with fit.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            predictor matrix
+        y : pd.series
+            target series
+
+        Raises
+        ------
+        ValueError
+            [description]
+        ValueError
+            [description]
+        """
+        # check X and y are consistent len, X is Array and y is column
+        X, y = check_X_y(X, y, dtype=None, force_all_finite=False)
+        if self.perc <= 0 or self.perc > 100:
+            raise ValueError("The percentile should be between 0 and 100.")
+
+        if self.alpha <= 0 or self.alpha > 1:
+            raise ValueError("Alpha should be between 0 and 1.")
+
+    def _print_results(self, dec_reg, _iter, flag):
+        """Private method, printing the result
+
+        Parameters
+        ----------
+        dec_reg: array
+            if the feature as been tagged as relevant (confirmed),
+            not relevant (rejected) or undecided
+        _iter: int
+            the iteration number
+        flag: int
+            is still in the feature selection process or not
+        Returns
+        -------
+         output: str
+            the output to be printed out
+        """
+        n_iter = str(_iter) + " / " + str(self.max_iter)
+        n_confirmed = np.where(dec_reg == 1)[0].shape[0]
+        n_rejected = np.where(dec_reg == -1)[0].shape[0]
+        cols = ["Iteration: ", "Confirmed: ", "Tentative: ", "Rejected: "]
+
+        # still in feature selection
+        if flag == 0:
+            n_tentative = np.where(dec_reg == 0)[0].shape[0]
+            content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
+            if self.verbose == 1:
+                output = cols[0] + n_iter
+            elif self.verbose > 1:
+                output = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
+
+        # Boruta finished running and tentatives have been filtered
+        else:
+            n_tentative = np.sum(self.support_weak_)
+            n_rejected = np.sum(~(self.support_ | self.support_weak_))
+            content = map(str, [n_iter, n_confirmed, n_tentative, n_rejected])
+            result = "\n".join([x[0] + "\t" + x[1] for x in zip(cols, content)])
+            if self.importance in ["shap", "pimp"]:
+                vimp = str(self.importance)
+            else:
+                vimp = "native"
+            output = (
+                "\n\nLeshy finished running using " + vimp + " var. imp.\n\n" + result
+            )
+        print(output)
+
+    def _update_estimator(self):
+        """
+        Update the estimator with a new random state, if applicable.
+
+        If the dataset is not categorical, the estimator's `random_state` parameter is updated
+        with a new random state generated by the `random_state` attribute of the Leshy object.
+        If the estimator is a LightGBM model, the random state value is generated between 0 and 10000.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+        if self.is_cat is False:
+            if self.is_lgb:
+                self.estimator.set_params(
+                    random_state=self.random_state.randint(0, 10000)
+                )
+            else:
+                self.estimator.set_params(random_state=self.random_state)
+
+    def _update_tree_num(self, dec_reg):
+        """Update the number of trees in the estimator based on the number of selected features.
+
+        Parameters
+        ----------
+        dec_reg : array-like of shape (n_features,)
+            The decision rule for each feature, where negative values indicate that the feature should be rejected
+            and non-negative values indicate that the feature should be selected.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        This function updates the `n_estimators` parameter of the estimator if it is set to "auto". The number of trees is
+        determined based on the number of selected features. Specifically, the number of trees is set to the value returned
+        by the `_get_tree_num` method, which takes as input the number of selected features that are not rejected.
+
+        If `n_estimators` is not set to "auto", this function does nothing.
+        """
+        if self.n_estimators == "auto":
+            # number of features that aren't rejected
+            not_rejected = np.where(dec_reg >= 0)[0].shape[0]
+            n_tree = self._get_tree_num(not_rejected)
+            self.estimator.set_params(n_estimators=n_tree)
+
+    def _run_iteration(
+        self, X, y, sample_weight, dec_reg, sha_max_history, imp_history, hit_reg, _iter
+    ):
+        """
+        Run an iteration of the Gradient Boosting algorithm.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input samples.
+
+        y : array-like of shape (n_samples,)
+            The target values.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples are equally weighted.
+
+        dec_reg : array-like of shape (n_samples,)
+            Decision function of the estimator.
+
+        sha_max_history : list of floats
+            List of the maximum shadow importance value at each iteration.
+
+        imp_history : array-like of shape (n_iterations, n_features)
+            Matrix of feature importances at each iteration.
+
+        hit_reg : array-like of shape (n_samples,)
+            Array of hit counts for each sample.
+
+        _iter : int
+            The current iteration number.
+
+        Returns
+        -------
+        dec_reg : array-like of shape (n_samples,)
+            Updated decision function of the estimator.
+
+        sha_max_history : list of floats
+            List of the maximum shadow importance value at each iteration.
+
+        imp_history : array-like of shape (n_iterations, n_features)
+            Matrix of feature importances at each iteration.
+
+        hit_reg : array-like of shape (n_samples,)
+            Array of hit counts for each sample.
+
+        imp_sha_max : float
+            The maximum shadow importance value for this iteration.
+        """
+        cur_imp = self._add_shadows_get_imps(X, y, sample_weight, dec_reg)
+        imp_sha_max = np.percentile(cur_imp[1], self.perc)
+        sha_max_history.append(imp_sha_max)
+        imp_history = np.vstack((imp_history, cur_imp[0]))
+        hit_reg = self._assign_hits(hit_reg, cur_imp, imp_sha_max)
+        dec_reg = self._do_tests(dec_reg, hit_reg, _iter)
+        return dec_reg, sha_max_history, imp_history, hit_reg, imp_sha_max
+
+    def select_features(self, X, y, sample_weight=None):
+        """
+        Select features using the Leshy algorithm.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The input data.
+        y : array-like of shape (n_samples,)
+            The target values.
+        sample_weight : array-like of shape (n_samples,), default=None
+            Individual weights for each sample.
+
+        Returns
+        -------
+        dec_reg : ndarray of shape (n_features,)
+            The decision rule. 1 means the feature is selected, 0 means the feature is not selected.
+        sha_max_history : list
+            List of the maximum shadow importances per iteration.
+        imp_history : ndarray of shape (n_iterations, n_features)
+            Array containing the feature importances per iteration.
+        imp_sha_max : float
+            Maximum shadow importance value.
+        """
+        pbar = tqdm(total=self.max_iter, desc="Leshy iteration")
+        dec_reg = np.zeros(X.shape[1])
+        hit_reg = np.zeros(X.shape[1])
+        sha_max_history = []
+        imp_history = np.empty((0, X.shape[1]))
+
+        for _iter in range(1, self.max_iter):
+            if not np.any(dec_reg == 0):
+                break
+            self._update_tree_num(dec_reg)
+            self._update_estimator()
+            (
+                dec_reg,
+                sha_max_history,
+                imp_history,
+                hit_reg,
+                imp_sha_max,
+            ) = self._run_iteration(
+                X,
+                y,
+                sample_weight,
+                dec_reg,
+                sha_max_history,
+                imp_history,
+                hit_reg,
+                _iter,
+            )
+            _iter += 1
+            pbar.update(1)
+
+        pbar.close()
+        return dec_reg, sha_max_history, imp_history, imp_sha_max
+
+    def _calculate_support(self, confirmed, tentative, n_feat):
+        """
+        Calculate the feature support arrays.
+
+        Parameters
+        ----------
+        confirmed : array-like of shape (n_confirmed,)
+            Indices of confirmed features.
+        tentative : array-like of shape (n_tentative,)
+            Indices of tentative features.
+        n_feat : int
+            Total number of features.
+
+        Returns
+        -------
+        None
+            The function populates the following class attributes:
+            - n_features_ : int
+                Number of selected features.
+            - support_ : ndarray of shape (n_feat,)
+                Boolean array indicating the selected features.
+            - support_weak_ : ndarray of shape (n_feat,)
+                Boolean array indicating the tentatively selected features.
+        """
+        # basic result variables
+        self.n_features_ = confirmed.shape[0]
+        self.support_ = np.zeros(n_feat, dtype=bool)
+        self.support_weak_ = np.zeros(n_feat, dtype=bool)
+        self.support_[confirmed] = 1
+        self.support_weak_ = np.zeros(n_feat, dtype=bool)
+        self.support_weak_[tentative] = 1
+        if self.keep_weak:
+            self.support_[tentative] = 1
+
+    def _calculate_absolute_ranking(self):
+        """
+        Compute feature importance scores using SHAP values.
+
+        Parameters
+        ----------
+        new_x_tr : numpy.ndarray
+            The training dataset after being processed.
+        shap_matrix : numpy.ndarray
+            The matrix containing SHAP values computed by a LightGBM model.
+        param : dict
+            A dictionary containing the parameters for a LightGBM model.
+        objective : str
+            The objective function of the LightGBM model.
+
+        Returns
+        -------
+        list
+            A list of tuples containing feature names and their corresponding importance scores.
+        """
+        vimp_df = pd.DataFrame(self.imp_real_hist, columns=self.feature_names_in_)
+        self.ranking_absolutes_ = list(
+            vimp_df.mean().sort_values(ascending=False).index
+        )
+
+    def _calculate_relative_ranking(self, n_feat, tentative, confirmed, imp_history):
+        """
+        Calculates the relative ranking of features based on their importance history.
+
+        Parameters
+        ----------
+        n_feat : int
+            The total number of features.
+        tentative : ndarray of shape (n_tentative_features,)
+            An array containing the indices of tentative features.
+        confirmed : ndarray of shape (n_confirmed_features,)
+            An array containing the indices of confirmed features.
+        imp_history : ndarray of shape (n_iterations + 1, n_features)
+            An array containing the feature importances for each iteration.
+
+        Returns
+        -------
+        None
+
+        """
+        # ranking, confirmed variables are rank 1
+        self.ranking_ = np.ones(n_feat, dtype=int)
+        # tentative variables are rank 2
+        self.ranking_[tentative] = 2
+        selected = np.hstack((confirmed, tentative))
+        # all rejected features are sorted by importance history
+        not_selected = np.setdiff1d(np.arange(n_feat), selected)
+        # large importance values should rank higher = lower ranks -> *(-1)
+        imp_history_rejected = imp_history[1:, not_selected] * -1
+
+        # update rank for not_selected features
+        if not_selected.shape[0] > 0:
+            # calculate ranks in each iteration, then median of ranks across feats
+            iter_ranks = self._nanrankdata(imp_history_rejected, axis=1)
+            rank_medians = np.nanmedian(iter_ranks, axis=0)
+            ranks = self._nanrankdata(rank_medians, axis=0)
+
+            # set smallest rank to 3 if there are tentative feats
+            if tentative.shape[0] > 0:
+                ranks = ranks - np.min(ranks) + 3
+            else:
+                # and 2 otherwise
+                ranks = ranks - np.min(ranks) + 2
+            self.ranking_[not_selected] = ranks
+        else:
+            # all are selected, thus we set feature supports to True
+            self.support_ = np.ones(n_feat, dtype=bool)
+
+    def _print_result(self, dec_reg, _iter, start_time):
+        """
+        Print the results of feature selection.
+
+        Parameters
+        ----------
+        dec_reg : bool
+            Decision on whether to proceed with another round of feature selection.
+        _iter : int
+            Current iteration number.
+        start_time : float
+            Time when the feature selection process started.
+
+        Returns
+        -------
+        None
+            The function prints the relevant results and running time.
+        """
+        if self.verbose > 0:
+            self._print_results(dec_reg, _iter, 1)
+        self.running_time = time.time() - start_time
+        hours, rem = divmod(self.running_time, 3600)
+        minutes, seconds = divmod(rem, 60)
+        print(
+            "All relevant predictors selected in {:0>2}:{:0>2}:{:05.2f}".format(
+                int(hours), int(minutes), seconds
+            )
+        )
+
+
+def _get_confirmed_and_tentative(dec_reg):
+    """Extracts the confirmed and tentative features from dec_reg."""
+    confirmed = np.where(dec_reg == 1)[0]
+    tentative = np.where(dec_reg == 0)[0]
+    return confirmed, tentative
+
+
+def _select_tentative(tentative, imp_history, sha_max_history):
+    """
+    Select tentative features based on median importance values.
+
+    Parameters
+    ----------
+    tentative: array-like of shape (n_tentative,)
+        Array of indices representing tentative features.
+    imp_history: array-like of shape (n_iterations + 1, n_features)
+        Importance values for each feature in each iteration.
+    sha_max_history: array-like of shape (n_iterations + 1,)
+        The history of the highest stability scores.
+
+    Returns
+    -------
+    tentative: array-like of shape (n_tentative_confirmed,)
+        The confirmed tentative features based on their median importance values.
+    """
+    # ignore the first row of zeros
+    tentative_median = np.median(imp_history[1:, tentative], axis=0)
+    # which tentative to keep
+    tentative_confirmed = np.where(tentative_median > np.median(sha_max_history))[0]
+    tentative = tentative[tentative_confirmed]
+    return tentative
+
+
+def _split_fit_estimator(estimator, X, y, sample_weight=None, cat_feature=None):
+    """Private function, split the train, test and fit the model
+
+    Parameters
+    ----------
+    estimator : estimator object implementing 'fit' and 'predict'
+        The object to use to fit the data.
+    X : pd.DataFrame of shape [n_samples, n_features]
+        predictor matrix
+    y : pd.series of shape [n_samples]
+        target
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample
+    cat_feature : list of int or None
+        the list of integers, cols loc, of the categrocial predictors. Avoids to detect and encode
+        each iteration if the exact same columns are passed to the selection methods.
+    Returns
+    -------
+     model :
+        fitted model
+     X_tt : array [n_samples, n_features]
+        the test split, predictors
+     y_tt : array [n_samples]
+        the test split, target
+    """
+    if cat_feature is None:
+        # detect, store and encode categorical predictors
+        X, _, cat_idx = get_pandas_cat_codes(X)
+    else:
+        cat_idx = cat_feature
+
+    if sample_weight is not None:
+        w = sample_weight
+        if is_regressor(estimator):
+            X_tr, X_tt, y_tr, y_tt, w_tr, w_tt = train_test_split(
+                X, y, w, random_state=42
+            )
+        else:
+            X_tr, X_tt, y_tr, y_tt, w_tr, w_tt = train_test_split(
+                X, y, w, stratify=y, random_state=42
+            )
+    else:
+        if is_regressor(estimator):
+            X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, random_state=42)
+        else:
+            X_tr, X_tt, y_tr, y_tt = train_test_split(X, y, stratify=y, random_state=42)
+        w_tr, w_tt = None, None
+
+    if check_if_tree_based(estimator):
+        try:
+            # handle cat features if supported by the fit method
+            if is_catboost(estimator) or (
+                "cat_feature" in estimator.fit.__code__.co_varnames
+            ):
+                model = estimator.fit(
+                    X_tr, y_tr, sample_weight=w_tr, cat_features=cat_idx
+                )
+            else:
+                model = estimator.fit(X_tr, y_tr, sample_weight=w_tr)
+
+        except Exception as e:
+            raise ValueError(
+                "Please check your X and y variable. The provided "
+                "estimator cannot be fitted to your data.\n" + str(e)
+            )
+    else:
+        raise ValueError("Not a tree based model")
+
+    return model, X_tt, y_tt, w_tt
+
+
+def _get_shap_imp(estimator, X, y, sample_weight=None, cat_feature=None):
+    """Get the SHAP feature importance
+
+    Parameters
+    ----------
+    estimator : estimator object
+        An estimator object implementing `fit` and `predict` methods.
+    X : pd.DataFrame of shape [n_samples, n_features]
+        Predictor matrix.
+    y : pd.Series of shape [n_samples]
+        Target variable.
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample.
+    cat_feature : list of int or None, default=None
+        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
+        each iteration if the exact same columns are passed to the selection methods.
+
+    Returns
+    -------
+    shap_imp : array
+        The SHAP importance array.
+    """
+    # Clone the estimator to avoid modifying the original one
+    estimator = clone(estimator)
+
+    # Split the data into train and test sets and fit the model
+    model, X_tt, y_tt, w_tt = _split_fit_estimator(
+        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
+    )
+    # Compute the SHAP values
+    if is_lightgbm(estimator):
+        # For LightGBM models use the built-in SHAP method
+        shap_matrix = model.predict(X_tt, pred_contrib=True)
+
+        # The shape of the shap_matrix depends on whether the estimator is a classifier or a regressor
+        if is_classifier(estimator) and (len(np.unique(y_tt)) > 2):
+            # For multi-class classifiers, reshape the shap_matrix
+            n_features = X_tt.shape[1]
+            shap_matrix = np.delete(
+                shap_matrix,
+                list(range(n_features, shap_matrix.shape[1], n_features + 1)),
+                axis=1,
+            )
+            shap_imp = np.mean(np.abs(shap_matrix), axis=0)
+        else:
+            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    else:
+        # For other tree-based models, use the shap.TreeExplainer method to compute SHAP values
+        explainer = shap.TreeExplainer(
+            model, feature_perturbation="tree_path_dependent"
+        )
+        shap_values = explainer.shap_values(X_tt)
+        # For multi-class classifiers, reshape the shap_values
+        if is_classifier(estimator):
+            if isinstance(shap_values, list):
+                # For LightGBM classifier in sklearn API, SHAP returns a list of arrays
+                # https://github.com/slundberg/shap/issues/526
+                shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_values], axis=0)
+            else:
+                shap_imp = np.abs(shap_values).mean(0)
+        else:
+            shap_imp = np.abs(shap_values).mean(0)
+    return shap_imp
+
+
+def _get_shap_imp_fast(estimator, X, y, sample_weight=None, cat_feature=None):
+    """Get the SHAP feature importance using the fasttreeshap implementation
+
+    Parameters
+    ----------
+    estimator : estimator object
+        An estimator object implementing `fit` and `predict` methods.
+    X : pd.DataFrame of shape [n_samples, n_features]
+        Predictor matrix.
+    y : pd.Series of shape [n_samples]
+        Target variable.
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample.
+    cat_feature : list of int or None, default=None
+        The list of integers, columns loc, of the categorical predictors. Avoids detecting and encoding
+        each iteration if the exact same columns are passed to the selection methods.
+
+    Returns
+    -------
+    shap_imp : array
+        The SHAP importance array.
+    """
+    try:
+        from fasttreeshap import TreeExplainer as FastTreeExplainer
+    except ImportError:
+        ImportError("fasttreeshap is not installed")
+    
+    # Clone the estimator to avoid modifying the original one
+    estimator = clone(estimator)
+
+    # Split the data into train and test sets and fit the model
+    model, X_tt, y_tt, w_tt = _split_fit_estimator(
+        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
+    )
+    explainer = FastTreeExplainer(
+        model,
+        algorithm="auto",
+        shortcut=False,
+        feature_perturbation="tree_path_dependent",
+    )
+    shap_matrix = explainer.shap_values(X_tt)
+    # multiclass returns a list
+    # for binary and for some models, shap is still returning a list
+    if is_classifier(estimator):
+        if isinstance(shap_matrix, list):
+            # For LightGBM classifier, RF, in sklearn API, SHAP returns a list of arrays
+            # https://github.com/slundberg/shap/issues/526
+            shap_imp = np.mean([np.abs(sv).mean(0) for sv in shap_matrix], axis=0)
+        else:
+            shap_imp = np.abs(shap_matrix).mean(0)
+    else:
+        shap_imp = np.abs(shap_matrix).mean(0)
+    return shap_imp
+
+
+def _get_perm_imp(estimator, X, y, sample_weight, cat_feature=None):
+    """Private function, Get the SHAP feature importance
+
+    Parameters
+    ----------
+    estimator: sklearn estimator
+    X : pd.DataFrame of shape [n_samples, n_features]
+        predictor matrix
+    y : pd.series of shape [n_samples]
+        target
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample
+    cat_feature : list of int or None
+        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
+        each iteration if the exact same columns are passed to the selection methods.
+    Returns
+    -------
+    imp : array
+        the permutation importance array
+    """
+    # be sure to use an non-fitted estimator
+    estimator = clone(estimator)
+
+    model, X_tt, y_tt, w_tt = _split_fit_estimator(
+        estimator, X, y, sample_weight=sample_weight, cat_feature=cat_feature
+    )
+    perm_imp = permutation_importance(
+        model, X_tt, y_tt, n_repeats=5, random_state=42, n_jobs=-1
+    )
+    imp = perm_imp.importances_mean.ravel()
+    return imp
+
+
+def _get_imp(estimator, X, y, sample_weight=None, cat_feature=None):
+    """Private function, Get the native feature importance (impurity based for instance)
+
+    Notes
+    -----
+    This is know to return biased and uninformative results.
+    e.g.
+    https://scikit-learn.org/stable/auto_examples/inspection/
+    plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py
+
+    or
+
+    https://explained.ai/rf-importance/
+
+    Parameters
+    ----------
+    X : array-like, shape = [n_samples, n_features]
+        The training input samples.
+    y : array-like, shape = [n_samples]
+        The target values.
+    sample_weight : array-like, shape = [n_samples], default=None
+        Individual weights for each sample
+    cat_feature: list of int or None
+        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
+        each iteration if the exact same columns are passed to the selection methods.
+    Returns
+    -------
+    imp : array
+        the permutation importance array
+    """
+    # be sure to use an non-fitted estimator
+    estimator = clone(estimator)
+
+    try:
+        if cat_feature is None:
+            X, _, cat_idx = get_pandas_cat_codes(X)
+        else:
+            cat_idx = cat_feature
+
+        # handle catboost and cat features
+        if is_catboost(estimator) or (
+            "cat_feature" in estimator.fit.__code__.co_varnames
+        ):
+            X = pd.DataFrame(X)
+            estimator.fit(X, y, sample_weight=sample_weight, cat_features=cat_idx)
+        else:
+            estimator.fit(X, y, sample_weight=sample_weight)
+
+    except Exception as e:
+        raise ValueError(
+            "Please check your X and y variable. The provided "
+            "estimator cannot be fitted to your data.\n" + str(e)
+        )
+    try:
+        imp = estimator.feature_importances_
+    except Exception:
+        raise ValueError(
+            "Only methods with feature_importance_ attribute "
+            "are currently supported in BorutaPy."
+        )
+    return imp
+
+
+###################################
+#
+# BoostAGroota
+#
+###################################
+class BoostAGroota(SelectorMixin, BaseEstimator):  # (object):
+    """
+    BoostAGroota is an all-relevant feature selection method, while most others are minimal optimal.
+    It tries to find all features carrying information usable for prediction, rather than finding a possibly compact
+    subset of features on which some estimator has a minimal error.
+
+    Why bother with all-relevant feature selection?
+    When you try to understand the phenomenon that made your data, you should
+    care about all factors that contribute to it, not just the bluntest signs
+    of it in the context of your methodology (minimal optimal set of features
+    by definition depends on your estimator choice).
+
+    Parameters
+    ----------
+    estimator : scikit-learn estimator
+        The model to train, lightGBM recommended, see the reduce lightgbm method.
+    cutoff : float
+        The value by which the max of shadow imp is divided, to compare to real importance.
+    iters : int (>0)
+        The number of iterations to average for the feature importance (on the same split),
+        to reduce the variance.
+    max_rounds : int (>0)
+        The number of times the core BoostAGroota algorithm will run.
+        Each round eliminates more and more features.
+    delta : float (0 < delta <= 1)
+        Stopping criteria for whether another round is started.
+    silent : bool
+        Set to True if you don't want to see the BoostAGroota output printed.
+    importance : str, default='shap'
+        The kind of feature importance to use. Possible values: 'shap' (Shapley values),
+        'pimp' (permutation importance), and 'native' (Gini/impurity).
+
+    Attributes
+    ----------
+    selected_features_ : list of str
+        The list of columns to keep.
+    ranking_ : array of shape [n_features]
+        The feature ranking, such that ``ranking_[i]`` corresponds to the
+        ranking position of the i-th feature. Selected (i.e., estimated
+        best) features are assigned rank 1, and tentative features are assigned
+        rank 2.
+    ranking_absolutes_ : array of shape [n_features]
+        The absolute feature ranking as ordered by the selection process. It does not guarantee
+        that this order is correct for all models. For a model-agnostic ranking, see the
+        attribute ``ranking``.
+    sha_cutoff_df : dataframe
+        Feature importance of the real+shadow predictors over iterations.
+    mean_shadow : float
+        The threshold below which the predictors are rejected.
+
+    Examples
+    --------
+    >>> X = df[filtered_features].copy()
+    >>> y = df['target'].copy()
+    >>> w = df['weight'].copy()
+    >>> model = LGBMRegressor(n_jobs=-1, n_estimators=100, objective='rmse', random_state=42, verbose=0)
+    >>> feat_selector = BoostAGroota(estimator=model, cutoff=1, iters=10, max_rounds=10, delta=0.1, importance='shap')
+    >>> feat_selector.fit(X, y, sample_weight=None)
+    >>> print(feat_selector.selected_features_)
+    >>> feat_selector.plot_importance(n_feat_per_inch=5)
+    """
+
+    def __init__(
+        self,
+        estimator=None,
+        cutoff=4,
+        iters=10,
+        max_rounds=500,
+        delta=0.1,
+        silent=True,
+        importance="shap",
+    ):
+        self.estimator = estimator
+        self.cutoff = cutoff
+        self.iters = iters
+        self.max_rounds = max_rounds
+        self.delta = delta
+        self.silent = silent
+        self.importance = importance
+        self.sha_cutoff_df = None
+        self.mean_shadow = None
+        self.ranking_absolutes_ = None
+        self.ranking_ = None
+
+        # Throw errors if the inputted parameters don't meet the necessary criteria
+        if cutoff <= 0:
+            raise ValueError(
+                "cutoff should be greater than 0. You entered" + str(cutoff)
+            )
+        if iters <= 0:
+            raise ValueError("iters should be greater than 0. You entered" + str(iters))
+        if (delta <= 0) | (delta > 1):
+            raise ValueError("delta should be between 0 and 1, was " + str(delta))
+
+        # Issue warnings for parameters to still let it run
+        if delta < 0.02:
+            warnings.warn(
+                "WARNING: Setting a delta below 0.02 may not converge on a solution."
+            )
+        if max_rounds < 1:
+            warnings.warn(
+                "WARNING: Setting max_rounds below 1 will automatically be set to 1."
+            )
+
+        if importance == "native":
+            warnings.warn(
+                "[BoostAGroota]: using native variable importance might break the FS"
+            )
+
+    def __repr__(self):
+        s = (
+            "BoostARoota(est={est}, \n"
+            "                cutoff={cutoff},\n"
+            "                iters={iters},\n"
+            "                max_rounds={mr},\n"
+            "                delta={delta},\n"
+            "                silent={silent}, \n"
+            '                importance="{importance}")'.format(
+                estimator=self.estimator,
+                cutoff=self.cutoff,
+                iters=self.iters,
+                mr=self.max_rounds,
+                delta=self.delta,
+                silent=self.silent,
+                importance=self.importance,
+            )
+        )
+        return s
+
+    def fit(self, X, y, sample_weight=None):
+        """Fit the BoostAGroota transformer with the provided estimator.
+        Parameters
+        ----------
+        X : pd.DataFrame
+            the predictors matrix
+        y : pd.Series
+            the target
+        sample_weight : pd.series
+            sample_weight, if any
+        """
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            warnings.warn("fasttreeshap is not installed. Fallback to shap.")
+            self.importance = "shap"
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+        else:
+            raise TypeError("X is not a dataframe")
+
+        if sample_weight is not None:
+            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
+
+        # crit, keep_vars, df_vimp, mean_shadow
+        _, self.selected_features_, self.sha_cutoff_df, self.mean_shadow = _boostaroota(
+            X,
+            y,
+            # metric=self.metric,
+            estimator=self.estimator,
+            cutoff=self.cutoff,
+            iters=self.iters,
+            max_rounds=self.max_rounds,
+            delta=self.delta,
+            silent=self.silent,
+            weight=sample_weight,
+            imp=self.importance,
+        )
+        self.selected_features_ = self.selected_features_.values
+        self.support_ = np.asarray(
+            [c in self.selected_features_ for c in self.feature_names_in_]
+        )
+        self.ranking_absolutes_ = list(
+            self.sha_cutoff_df.iloc[:, : int(self.sha_cutoff_df.shape[1] / 2)]
+            .mean()
+            .sort_values(ascending=False)
+            .index
+        )
+        self.ranking_ = np.where(self.support_, 2, 1)
+        return self
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def transform(self, X):
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    def _more_tags(self):
+        return {"allow_nan": True, "requires_y": True}
+
+    @mpl.rc_context(PLT_PARAMS)
+    def plot_importance(self, n_feat_per_inch=5):
+        """
+        Boxplot of the variable importance, ordered by magnitude.
+        The max shadow variable importance illustrated by the dashed line.
+        Requires to apply the fit method first.
+
+        Parameters
+        ----------
+        n_feat_per_inch : int, default=5
+            Number of features to plot per inch (for scaling the figure).
+
+        Returns
+        -------
+        fig : plt.figure or None
+            The matplotlib figure object containing the boxplot, or None if there are no selected features.
+        """
+        if self.mean_shadow is None:
+            raise ValueError("Apply fit method first")
+
+        b_df = self.sha_cutoff_df
+        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
+
+        real_df = real_df.reindex(
+            real_df.mean().sort_values(ascending=True).index, axis=1
+        )
+
+        if real_df.dropna().empty:
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
+            return None
+
+        fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
+        bp = real_df.plot(**PLOT_KWARGS, ax=ax)
+        bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
+
+        for c in range(len(self.selected_features_)):
+            patch = bp.findobj(mpl.patches.Patch)[real_df.shape[1] - c - 1]
+            patch.set_facecolor(BLUE)
+            patch.set_color(BLUE)
+
+        custom_lines = [
+            Line2D([0], [0], color=BLUE, lw=5),
+            Line2D([0], [0], color="gray", lw=5),
+            Line2D([0], [0], linestyle="--", color=RED, lw=2),
+        ]
+        bp.legend(
+            custom_lines, ["confirmed", "rejected", "sha. max"], loc="lower right"
+        )
+
+        ax.axvline(x=self.mean_shadow, linestyle="--", color=RED)
+        ax.set_title("BoostAGroota importance of selected predictors")
+
+        return fig
+
+
+############################################
+# Helper Functions to do the Heavy Lifting
+############################################
+
+
+def _create_shadow(X_train):
+    """Create shadow features by making copies of all X variables and randomly shuffling them.
+
+    Parameters
+    ----------
+    X_train : pd.DataFrame
+        The dataframe to create shadow features on.
+
+    Returns
+    -------
+    pd.DataFrame
+        A dataframe that is twice the width of X_train and contains the shadow features, along with a list of the shadow feature names.
+    """
+    X_shadow = X_train.copy()
+    for c in X_shadow.columns:
+        np.random.shuffle(X_shadow[c].values)
+    # Rename the shadow variables
+    shadow_names = [f"ShadowVar{i+1}" for i in range(X_train.shape[1])]
+    X_shadow.columns = shadow_names
+    # Combine to make one new dataframe
+    new_x = pd.concat([X_train, X_shadow], axis=1)
+    return new_x, shadow_names
+
+
+########################################################################################
+# BoostARoota. In principle, you cannot/don't need to access those methods (reason of
+# the _ in front of the function name, they're internal functions)
+########################################################################################
+
+
+def _reduce_vars_sklearn(
+    X,
+    y,
+    estimator,
+    this_round,
+    cutoff,
+    n_iterations,
+    delta,
+    silent,
+    weight,
+    imp_kind,
+    cat_feature,
+):
+    """
+    Private function, reduce the number of predictors using a sklearn estimator
+
+    Parameters
+    ----------
+    x : pd.DataFrame
+        the dataframe to create shadow features on
+    y : pd.Series
+        the target
+    estimator : sklearn estimator
+        the model to train, lightGBM recommended
+    this_round : int
+        The number of times the core BoostARoota algorithm will run.
+        Each round eliminates more and more features
+    cutoff : float
+        the value by which the max of shadow imp is divided, to compare to real importance
+    n_iterations : int
+        The number of iterations to average for the feature importance (on the same split),
+        to reduce the variance
+    delta : float (0 < delta <= 1)
+        Stopping criteria for whether another round is started
+    silent : bool
+        Set to True if don't want to see the BoostARoota output printed.
+        Will still show any errors or warnings that may occur
+    weight : pd.series
+        sample_weight, if any
+    imp_kind : str
+        whether if native, shap, fastshap or permutation importance should be used
+    cat_feature : list of int or None
+        the list of integers, cols loc, of the categorical predictors. Avoids to detect and encode
+        each iteration if the exact same columns are passed to the selection methods.
+
+    Returns
+    -------
+    criteria : bool
+        if the criteria has been reached or not
+    real_vars['feature'] : pd.dataframe
+        feature importance of the real predictors over iter
+    df : pd.DataFrame
+        feature importance of the real+shadow predictors over iter
+    mean_shadow : float
+        the feature importance threshold, to reject or not the predictors
+
+    Raises
+    ------
+    ValueError
+        error if the feature importance type is not
+    """
+    # Set up the parameters for running the model in XGBoost - split is on multi log loss
+    for i in range(1, n_iterations + 1):
+        # Create the shadow variables and run the model to obtain importances
+        new_x, shadow_names = _create_shadow(X)
+        imp_func = {
+            "shap": _get_shap_imp,
+            "fastshap": _get_shap_imp,
+            "pimp": _get_perm_imp,
+            "native": _get_imp,
+        }
+        importance = imp_func[imp_kind](
+            estimator, new_x, y, sample_weight=weight, cat_feature=cat_feature
+        )
+
+        # Create a dataframe to store the feature importances
+        if i == 1:
+            df = pd.DataFrame({"feature": new_x.columns})
+            df2 = df.copy()
+
+        # Store the feature importances in df2
+        try:
+            # Normalize the feature importances
+            df2["fscore" + str(i)] = importance / importance.sum()
+        except ValueError:
+            print("Only Sklearn tree based methods allowed")
+
+        # Merge the current feature importances with the existing ones in df
+        df = pd.merge(
+            df, df2, on="feature", how="outer", suffixes=("_x" + str(i), "_y" + str(i))
+        )
+
+        # Print the iteration number if not silent
+        if not silent:
+            print("Round: ", this_round, " iteration: ", i)
+
+    df["Mean"] = df.select_dtypes(include=[np.number]).mean(axis=1, skipna=True)
+    # Split them back out
+    real_vars = df.loc[~df["feature"].isin(shadow_names)]
+    shadow_vars = df.loc[df["feature"].isin(shadow_names)]
+
+    # Get mean value from the shadows (max, like in Boruta, median to mitigate variance)
+    mean_shadow = (
+        shadow_vars.select_dtypes(include=[np.number])
+        .max(skipna=True)
+        .mean(skipna=True)
+        / cutoff
+    )
+    real_vars = real_vars[(real_vars.Mean >= mean_shadow)]
+
+    # Check for the stopping criteria
+    # Compute the fraction of features selected in this round
+    selected_frac = len(real_vars) / len(X.columns)
+
+    # Check if we should stop feature selection
+    # make sure we are removing at least delta % of the variables
+    criteria = len(X.columns) == 0 or selected_frac == 0 or selected_frac > 1 - delta
+
+    return criteria, real_vars["feature"], df, mean_shadow
+
+
+def _boostaroota(
+    X, y, estimator, cutoff, iters, max_rounds, delta, silent, weight, imp
+):
+    """
+    Private function, reduces the number of predictors using a sklearn estimator.
+
+    Parameters
+    ----------
+    x : pd.DataFrame
+        The dataframe to create shadow features on.
+    y : pd.Series
+        The target.
+    estimator : scikit-learn estimator
+        The model to train, lightGBM recommended, see the reduce lightgbm method.
+    cutoff : float
+        The value by which the max of shadow imp is divided, to compare to real importance.
+    iters : int (>0)
+        The number of iterations to average for the feature importances (on the same split),
+        to reduce the variance.
+    max_rounds : int (>0)
+        The number of times the core BoostARoota algorithm will run.
+        Each round eliminates more and more features.
+    delta : float (0 < delta <= 1)
+        Stopping criteria for whether another round is started.
+    silent : bool
+        Set to True if you don't want to see the BoostARoota output printed.
+        Will still show any errors or warnings that may occur.
+    weight : pd.Series, optional
+        Sample weights, if any.
+
+    Returns
+    -------
+    crit : bool
+        If the criteria have been reached or not.
+    keep_vars : pd.DataFrame
+        Feature importance of the real predictors over iterations.
+    df_vimp : pd.DataFrame
+        Feature importance of the real+shadow predictors over iterations.
+    mean_shadow : float
+        The feature importance threshold to reject or not the predictors.
+    """
+    start_time = time.time()
+    new_x = X.copy()
+
+    # extract the categorical names for the first time, store it for next iterations
+    # In the below while loop this list will be update only once some of the predictors
+    # are removed. This way the encoding is done only every predictors update and not
+    # every iteration. The code will then be much faster since the encoding is done only once.
+    new_x, obj_feat, cat_idx = get_pandas_cat_codes(X)
+
+    # Run through loop until "crit" changes
+    i = 0
+    imp_dic = {}
+    with tqdm(total=max_rounds, desc="BoostaGRoota round") as pbar:
+        while True:
+            # Inside this loop we reduce the dataset on each iteration exiting with keep_vars
+            i += 1
+            crit, keep_vars, df_vimp, mean_shadow = _reduce_vars_sklearn(
+                new_x,
+                y,
+                estimator=estimator,
+                this_round=i,
+                cutoff=cutoff,
+                n_iterations=iters,
+                delta=delta,
+                silent=silent,
+                weight=weight,
+                imp_kind=imp,
+                cat_feature=cat_idx,
+            )
+
+            b_df = df_vimp.T.iloc[1:-1].astype(float)
+            b_df.columns = df_vimp.T.iloc[0].values
+            imp_dic.update(b_df.to_dict())
+
+            if crit or i >= max_rounds or len(keep_vars) == 0:
+                break
+            else:
+                new_x = new_x[keep_vars].copy()
+                _, _, cat_idx = get_pandas_cat_codes(new_x)
+
+                pbar.update(1)
+
+    elapsed = (time.time() - start_time) / 60
+    if not silent:
+        print(f"BoostARoota ran successfully! Algorithm went through {i} rounds.")
+        print(f"The feature selection BoostARoota running time is {elapsed:8.2f} min")
+
+    df_vimp = pd.DataFrame.from_dict(imp_dic)
+
+    return crit, keep_vars, df_vimp, mean_shadow
+
+
+###################################
+#
+# GrootCV
+#
+###################################
+
+
+class GrootCV(SelectorMixin, BaseEstimator):
+    """
+    GrootCV is a feature selection method based on cross-validation with lightGBM.
+
+    A shuffled copy of the predictors matrix is added (shadows) to the original set of predictors.
+    The lightGBM is fitted using repeated cross-validation, the feature importance
+    is extracted each time and averaged to smooth out the noise.
+    If the feature importance is larger than the average shadow feature importance then the predictors are rejected, the others are kept.
+        - Cross-validated feature importance to smooth out the noise, based on lightGBM only
+          (which is, most of the time, the fastest and more accurate Boosting).
+        - the feature importance is derived using SHAP importance
+        - Taking the max of median of the shadow var. imp over folds otherwise not enough conservative and
+          it improves the convergence (needs less evaluation to find a threshold)
+        - Not based on a given percentage of cols needed to be deleted
+        - Plot method for var. imp
+
+    Parameters
+    ----------
+    objective : str or callable, default=None
+        The objective function to use in lightGBM. If None, it uses the objective specified in `lgbm_params`.
+    cutoff : float, default=1
+        The value by which the max of shadow imp is divided, to compare to real importance.
+    n_folds : int, default=5
+        The number of folds for cross-validation.
+    n_iter : int, default=5
+        The number of iterations to average for the feature importance (on the same split), to reduce variance.
+    silent : bool, default=True
+        Set to True if you don't want to see the GrootCV output printed.
+    rf : bool, default=False
+        If True, use random forest for calculating feature importances; otherwise, use lightGBM.
+    fastshap : bool, default=False
+        If True, use fastSHAP for calculating feature importances; otherwise, use SHAP.
+    n_jobs : int, default=0
+        The number of jobs to run in parallel. If 0, no parallelism is used.
+    lgbm_params : dict, default=None
+        The parameters for the lightGBM model.
+
+    Attributes
+    ----------
+    selected_features_ : ndarray
+        The list of columns to keep as selected features.
+    cv_df : pd.DataFrame
+        DataFrame containing feature importance values for each fold and iteration.
+    sha_cutoff : float
+        The threshold below which the predictors are rejected.
+    ranking_absolutes_ : list
+        The absolute feature ranking as ordered by the selection process.
+    ranking_ : ndarray
+        The feature ranking, where 2 corresponds to selected features and 1 to tentative features.
+
+    Methods
+    -------
+    fit(X, y, sample_weight=None)
+        Fit the GrootCV on the input data.
+    transform(X)
+        Apply the fitted GrootCV on new data.
+    plot_importance(n_feat_per_inch=5)
+        Plot the feature importance of the fitted GrootCV.
+
+    Warnings
+    --------
+    If `sha_cutoff` is None, you should apply the fit method first.
+    Examples
+    -------
+    >>> X = df[filtered_features].copy()
+    >>> y = df['target'].copy()
+    >>> w = df['weight'].copy()
+    >>> feat_selector = arfsgroot.GrootCV(objective='rmse', cutoff = 1, n_folds=5, n_iter=5)
+    >>> feat_selector.fit(X, y, sample_weight=None)
+    >>> feat_selector.plot_importance(n_feat_per_inch=5)
+    """
+
+    def __init__(
+        self,
+        objective=None,
+        cutoff=1,
+        n_folds=5,
+        n_iter=5,
+        silent=True,
+        rf=False,
+        fastshap=False,
+        n_jobs=0,
+        lgbm_params=None,
+    ):
+        self.objective = objective
+        self.cutoff = cutoff
+        self.n_folds = n_folds
+        self.n_iter = n_iter
+        self.silent = silent
+        self.rf = rf
+        self.fastshap = fastshap
+        self.cv_df = None
+        self.sha_cutoff = None
+        self.ranking_absolutes_ = None
+        self.ranking_ = None
+        self.lgbm_params = lgbm_params
+        self.n_jobs = n_jobs
+
+        # Throw errors if the inputted parameters don't meet the necessary criteria
+        # Ensure parameters meet necessary criteria
+        if cutoff <= 0 or n_iter <= 0 or n_folds <= 0:
+            raise ValueError("cutoff, n_iter, and n_folds should be greater than 0.")
+
+    def fit(self, X, y, sample_weight=None):
+        """
+        Fit the GrootCV on the input data.
+
+        Parameters
+        ----------
+        X : pd.DataFrame of shape (n_samples, n_features)
+            The predictor dataframe.
+        y : array-like of shape (n_samples,)
+            The target vector.
+        sample_weight : array-like of shape (n_samples,), optional
+            The weight vector, by default None.
+
+        Returns
+        -------
+        self : object
+            Returns self.
+        """
+
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a pandas DataFrame")
+
+        self.feature_names_in_ = X.columns.to_numpy()
+        y = pd.Series(y) if not isinstance(y, pd.Series) else y
+
+        if sample_weight is not None:
+            sample_weight = pd.Series(_check_sample_weight(sample_weight, X))
+
+        # internal encoding (ordinal encoding)
+        X, obj_feat, cat_idx = get_pandas_cat_codes(X)
+
+        self.selected_features_, self.cv_df, self.sha_cutoff = _reduce_vars_lgb_cv(
+            X,
+            y,
+            objective=self.objective,
+            cutoff=self.cutoff,
+            n_folds=self.n_folds,
+            n_iter=self.n_iter,
+            silent=self.silent,
+            weight=sample_weight,
+            rf=self.rf,
+            fastshap=self.fastshap,
+            lgbm_params=self.lgbm_params,
+            n_jobs=self.n_jobs,
+        )
+
+        self.selected_features_ = self.selected_features_.values
+        self.support_ = np.asarray(
+            [c in self.selected_features_ for c in self.feature_names_in_]
+        )
+        self.ranking_ = np.where(self.support_, 2, 1)
+
+        b_df = self.cv_df.T.copy()
+        b_df.columns = b_df.iloc[0]
+        b_df = b_df.drop(b_df.index[0])
+        b_df = b_df.drop(b_df.index[-1])
+        b_df = b_df.convert_dtypes()
+        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
+        self.ranking_absolutes_ = list(
+            real_df.mean().sort_values(ascending=False).index
+        )
+        return self
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def transform(self, X):
+        """
+        Apply the fitted GrootCV on new data.
+
+        Parameters
+        ----------
+        X : pd.DataFrame of shape (n_samples, n_features)
+            The predictor dataframe.
+
+        Returns
+        -------
+        X_selected : pd.DataFrame of shape (n_samples, n_selected_features)
+            The selected features from the input dataframe.
+        """
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    def _more_tags(self):
+        return {"allow_nan": True, "requires_y": True}
+
+    @mpl.rc_context(PLT_PARAMS)
+    def plot_importance(self, n_feat_per_inch=5):
+        """
+        Plot the feature importance of the fitted GrootCV.
+
+        Parameters
+        ----------
+        n_feat_per_inch : int, default=5
+            The number of features per inch in the plot.
+
+        Returns
+        -------
+        fig : matplotlib.figure.Figure or None
+            The matplotlib figure containing the plot or None if no feature is selected.
+        """
+
+        if self.sha_cutoff is None:
+            raise ValueError("Apply fit method first")
+
+        b_df = self.cv_df.T.copy()
+        b_df.columns = b_df.iloc[0]
+        b_df = b_df.drop(b_df.index[0])
+        b_df = b_df.drop(b_df.index[-1])
+        b_df = b_df.convert_dtypes()
+        real_df = b_df.iloc[:, : int(b_df.shape[1] / 2)].copy()
+        sha_df = b_df.iloc[:, int(b_df.shape[1] / 2) :].copy()
+
+        real_df = real_df.reindex(
+            real_df.select_dtypes(include=[np.number])
+            .mean()
+            .sort_values(ascending=True)
+            .index,
+            axis=1,
+        )
+
+        if real_df.dropna().empty:
+            warnings.warn(NO_FEATURE_SELECTED_WARNINGS)
+            return None
+        else:
+            fig, ax = plt.subplots(figsize=(16, real_df.shape[1] / n_feat_per_inch))
+            bp = real_df.plot(**PLOT_KWARGS, ax=ax)
+            col_idx = np.argwhere(real_df.columns.isin(self.selected_features_)).ravel()
+
+            for c in range(real_df.shape[1]):
+                bp.findobj(mpl.patches.Patch)[c].set_facecolor("gray")
+                bp.findobj(mpl.patches.Patch)[c].set_color("gray")
+
+            for c in col_idx:
+                bp.findobj(mpl.patches.Patch)[c].set_facecolor(BLUE)
+                bp.findobj(mpl.patches.Patch)[c].set_color(BLUE)
+
+            ax.axvline(x=self.sha_cutoff, linestyle="--", color=RED)
+            bp.set_xlim(left=real_df.min(skipna=True).min(skipna=True) - 0.025)
+            custom_lines = [
+                Line2D([0], [0], color=BLUE, lw=5),
+                Line2D([0], [0], color="gray", lw=5),
+                Line2D([0], [0], linestyle="--", color=RED, lw=2),
+            ]
+            bp.legend(
+                custom_lines, ["confirmed", "rejected", "threshold"], loc="lower right"
+            )
+            ax.set_title("Groot CV importance and selected predictors")
+
+            return fig
+
+
+########################################################################################
+#
+# GrootCV. In principle, you cannot/don't need to access those methods (reason of
+# the _ in front of the function name, they're internal functions)
+#
+########################################################################################
+
+
+def _reduce_vars_lgb_cv(
+    X,
+    y,
+    objective,
+    n_folds,
+    cutoff,
+    n_iter,
+    silent,
+    weight,
+    rf,
+    fastshap,
+    lgbm_params=None,
+    n_jobs=0,
+):
+    """
+    Reduce the number of predictors using a lightgbm (python API)
+
+    Parameters
+    ----------
+    X : pd.DataFrame
+            the dataframe to create shadow features on
+    y : pd.Series
+            the target
+    objective : str
+            the lightGBM objective
+    cutoff : float
+            the value by which the max of shadow imp is divided, to compare to real importance
+    n_iter : int
+            The number of repetition of the cross-validation, smooth out the feature importance noise
+    silent : bool
+            Set to True if don't want to see the BoostARoota output printed.
+            Will still show any errors or warnings that may occur
+    weight : pd.series
+            sample_weight, if any
+    rf : bool, default=False
+            the lightGBM implementation of the random forest
+    fastshap : bool
+            enable or not the fasttreeshap implementation
+    lgbm_params : dict, optional
+            dictionary of lightgbm parameters
+    n_jobs: int, default 0
+        0 means default number of threads in OpenMP
+        for the best speed, set this to the number of real CPU cores, not the number of threads
+
+    Returns
+    -------
+    real_vars['feature'] : pd.dataframe
+            feature importance of the real predictors over iter
+    df : pd.DataFrame
+            feature importance of the real+shadow predictors over iter
+    cutoff_shadow : float
+            the feature importance threshold, to reject or not the predictors
+    """
+
+    params = _set_lgb_parameters(
+        X=X,
+        y=y,
+        objective=objective,
+        rf=rf,
+        silent=silent,
+        n_jobs=n_jobs,
+        lgbm_params=lgbm_params,
+    )
+
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+    category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
+    cat_idx = [X.columns.get_loc(col) for col in category_cols]
+
+    rkf = RepeatedKFold(n_splits=n_folds, n_repeats=n_iter, random_state=2652124)
+    iter = 0
+    df = pd.DataFrame({"feature": X.columns})
+    for tridx, validx in tqdm(
+        rkf.split(X, y), total=rkf.get_n_splits(), desc="Repeated k-fold"
+    ):
+        X_train, X_val, y_train, y_val, weight_tr, weight_val = _split_data(
+            X, y, tridx, validx, weight
+        )
+
+        # Create the shadow variables and run the model to obtain importances
+        new_x_tr, shadow_names = _create_shadow(X_train)
+        new_x_val, _ = _create_shadow(X_val)
+
+        bst, shap_matrix, bst.best_iteration = _train_lgb_model(
+            new_x_tr,
+            y_train,
+            weight_tr,
+            new_x_val,
+            y_val,
+            weight_val,
+            category_cols=category_cols,
+            early_stopping_rounds=20,
+            fastshap=fastshap,
+            **params,
+        )
+
+        importance = _compute_importance(
+            new_x_tr, shap_matrix, params, objective, fastshap
+        )
+        df = _merge_importance_df(
+            df=df,
+            importance=importance,
+            iter=iter,
+            n_folds=n_folds,
+            column_names=new_x_tr.columns,
+            silent=silent,
+        )
+        iter += 1
+
+    df["Med"] = df.select_dtypes(include=[np.number]).mean(axis=1)
+    # Split them back out
+    real_vars = df[~df["feature"].isin(shadow_names)]
+    shadow_vars = df[df["feature"].isin(shadow_names)]
+
+    # Get median value from the shadows, comparing predictor by predictor. Not the same criteria
+    # max().max() like in Boruta but max of the median to mitigate.
+    # Otherwise too conservative (reject too often)
+    cutoff_shadow = shadow_vars.select_dtypes(include=[np.number]).max().mean() / cutoff
+    real_vars = real_vars[(real_vars.Med.values >= cutoff_shadow)]
+
+    return real_vars["feature"], df, cutoff_shadow
+
+
+def _set_lgb_parameters(
+    X: np.ndarray,
+    y: np.ndarray,
+    objective: str,
+    rf: bool,
+    silent: bool,
+    n_jobs: int = 0,
+    lgbm_params: dict = None,
+) -> dict:
+    """Set parameters for a LightGBM model based on the input features and the objective.
+
+    Parameters
+    ----------
+    X : numpy array or pandas DataFrame
+        The feature matrix of the training data.
+    y : numpy array or pandas Series
+        The target variable of the training data.
+    objective : str
+        The objective function to optimize during training.
+    rf : bool, default False
+        Whether to use random forest boosting.
+    silent : bool, default True
+        Whether to print messages during parameter setting.
+    n_jobs: int, default 0
+        0 means default number of threads in OpenMP
+        for the best speed, set this to the number of real CPU cores, not the number of threads
+
+    Returns
+    -------
+    dict
+        The dictionary of LightGBM parameters.
+
+    """
+
+    n_feat = X.shape[1]
+
+    params = lgbm_params if lgbm_params is not None else {}
+
+    params["objective"] = objective
+    params["verbosity"] = -1
+    if objective == "softmax":
+        params["num_class"] = len(np.unique(y))
+
+    if rf:
+        feat_frac = (
+            np.sqrt(n_feat) / n_feat
+            if objective in ["softmax", "binary"]
+            else n_feat / (3 * n_feat)
+        )
+        params.update(
+            {
+                "boosting_type": "rf",
+                "bagging_fraction": 0.7,
+                "feature_fraction": feat_frac,
+                "bagging_freq": 1,
+            }
+        )
+
+    clf_losses = [
+        "binary",
+        "softmax",
+        "multi_logloss",
+        "multiclassova",
+        "multiclass",
+        "multiclass_ova",
+        "ova",
+        "ovr",
+        "binary_logloss",
+    ]
+    if objective in clf_losses:
+        y = y.astype(int)
+        y_freq_table = pd.Series(y.fillna(0)).value_counts(normalize=True)
+        n_classes = y_freq_table.size
+        if n_classes > 2 and objective != "softmax":
+            params["objective"] = "softmax"
+            params["num_class"] = len(np.unique(y))
+            if not silent:
+                print("Multi-class task, setting objective to softmax")
+        main_class = y_freq_table[0]
+        if not silent:
+            print("GrootCV: classification with unbalance classes")
+        if main_class > 0.8:
+            params.update({"is_unbalance": True})
+
+    params.update({"num_threads": n_jobs})
+
+    # we are using early_stopping
+    # we prevent the overridding of it by popping the n_iterations
+    keys_to_pop = [
+        "num_iterations",
+        "num_iteration",
+        "n_iter",
+        "num_tree",
+        "num_trees",
+        "num_round",
+        "num_rounds",
+        "nrounds",
+        "num_boost_round",
+        "n_estimators",
+        "max_iter",
+    ]
+    for key in keys_to_pop:
+        params.pop(key, None)
+
+    return params
+
+
+def _split_data(X, y, tridx, validx, weight=None):
+    """
+    Split data into train and validation sets based on provided indices.
+
+    Parameters
+    ----------
+    X : pandas.DataFrame
+        Features.
+    y : pandas.Series
+        Target variable.
+    tridx : list
+        Indices to be used for training.
+    validx : list
+        Indices to be used for validation.
+    weight : pandas.Series, optional
+        Weights for each sample, by default None.
+
+    Returns
+    -------
+    tuple of pandas.DataFrame and pandas.Series
+        X_train, X_val, y_train, y_val, weight_tr, weight_val
+    """
+    if weight is not None:
+        X_train, y_train, weight_tr = (
+            X.iloc[tridx, :],
+            y.iloc[tridx],
+            weight.iloc[tridx],
+        )
+        X_val, y_val, weight_val = (
+            X.iloc[validx, :],
+            y.iloc[validx],
+            weight.iloc[validx],
+        )
+    else:
+        X_train, y_train = X.iloc[tridx, :], y.iloc[tridx]
+        X_val, y_val = X.iloc[validx, :], y.iloc[validx]
+        weight_tr = None
+        weight_val = None
+    return X_train, X_val, y_train, y_val, weight_tr, weight_val
+
+
+def _train_lgb_model(
+    X_train,
+    y_train,
+    weight_train,
+    X_val,
+    y_val,
+    weight_val,
+    category_cols=None,
+    early_stopping_rounds=20,
+    fastshap=True,
+    **params,
+):
+    """
+    Train a LightGBM model with the given training data and hyperparameters and return the trained model and its SHAP values.
+
+    Parameters
+    ----------
+    X_train : array-like of shape (n_samples, n_features)
+        The input training data.
+    y_train : array-like of shape (n_samples,)
+        The target training data.
+    weight_train : array-like of shape (n_samples,)
+        The sample weights for training data.
+    X_val : array-like of shape (n_val_samples, n_features)
+        The input validation data.
+    y_val : array-like of shape (n_val_samples,)
+        The target validation data.
+    weight_val : array-like of shape (n_val_samples,)
+        The sample weights for validation data.
+    category_cols : array-like or None, optional (default=None)
+        The indices of categorical columns. If None, no categorical columns will be considered.
+    early_stopping_rounds : int, optional (default=20)
+        Activates early stopping. Validation metric needs to improve at least once in every early_stopping_rounds
+        round(s) to continue training._train_lgb_model
+    fastshap : bool
+        enable or not fasttreeshap implementation
+    **params : dict
+        Other parameters passed to the LightGBM model.
+
+    Returns
+    -------
+    tuple of (Booster, numpy.ndarray, int)
+        The trained LightGBM model, its SHAP values for X_train, and the best iteration reached during training.
+    """
+
+    d_train = lgb.Dataset(
+        X_train, label=y_train, weight=weight_train, categorical_feature=category_cols
+    )
+    d_valid = lgb.Dataset(
+        X_val, label=y_val, weight=weight_val, categorical_feature=category_cols
+    )
+    watchlist = [d_train, d_valid]
+
+    bst = lgb.train(
+        params,
+        train_set=d_train,
+        num_boost_round=10000,
+        valid_sets=watchlist,
+        categorical_feature=category_cols,
+        callbacks=[early_stopping(early_stopping_rounds, False, False)],
+    )
+
+    if fastshap:
+        try:
+            from fasttreeshap import TreeExplainer as FastTreeExplainer
+        except ImportError:
+            raise ImportError(
+                "fasttreeshap is not installed. Please install it using 'pip/conda install fasttreeshap'."
+            )
+
+        explainer = FastTreeExplainer(
+            bst,
+            algorithm="auto",
+            shortcut=False,
+            feature_perturbation="tree_path_dependent",
+        )
+        shap_matrix = explainer.shap_values(X_train)
+    else:
+        shap_matrix = bst.predict(X_train, pred_contrib=True)
+
+    return bst, shap_matrix, bst.best_iteration
+
+
+def _compute_importance(new_x_tr, shap_matrix, param, objective, fastshap):
+    """Compute feature importance scores using SHAP values.
+
+    Parameters
+    ----------
+    new_x_tr : numpy.ndarray
+        The training dataset after being processed.
+    shap_matrix : numpy.ndarray
+        The matrix containing SHAP values computed by a LightGBM model.
+    param : dict
+        A dictionary containing the parameters for a LightGBM model.
+    objective : str
+        The objective function of the LightGBM model.
+
+    Returns
+    -------
+    list
+        A list of tuples containing feature names and their corresponding importance scores.
+    """
+    if fastshap:
+        if objective == "softmax":
+            shap_matrix = np.abs(np.concatenate(shap_matrix, axis=1))
+        shap_imp = np.mean(np.abs(shap_matrix), axis=0)
+    else:
+        if objective == "softmax":
+            n_feat = new_x_tr.shape[1]
+            shap_matrix = np.delete(
+                shap_matrix,
+                list(range(n_feat, (n_feat + 1) * param["num_class"], n_feat + 1)),
+                axis=1,
+            )
+            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+        else:
+            shap_imp = np.mean(np.abs(shap_matrix[:, :-1]), axis=0)
+    importance = dict(zip(new_x_tr.columns, shap_imp))
+    return sorted(importance.items(), key=operator.itemgetter(1))
+
+
+def _merge_importance_df(df, importance, iter, n_folds, column_names, silent=True):
+    """
+    Merge the feature importance dataframe `df` with the importance
+    information for the current iteration of a cross-validation loop.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        The current feature importance dataframe.
+    importance : dict
+        A dictionary with the feature importance information for
+        the current iteration.
+    i : int
+        The index of the current iteration.
+    n_folds : int
+        The number of folds used in the cross-validation loop.
+    silent : bool, optional
+        If True, suppress output.
+
+    Returns
+    -------
+    pandas.DataFrame
+        The updated feature importance dataframe.
+    """
+
+    df2 = pd.DataFrame(importance, columns=["feature", "fscore" + str(iter)])
+    df2["fscore" + str(iter)] = (
+        df2["fscore" + str(iter)] / df2["fscore" + str(iter)].sum()
+    )
+    df = pd.merge(df, df2, on="feature", how="outer")
+    nit = divmod(iter, n_folds)[0]
+    nf = divmod(iter, n_folds)[1]
+    if not silent:
+        if nf == 0:
+            print("Groot iteration: ", nit, " with " + str(n_folds) + " folds")
+    return df
```

### Comparing `arfs-2.0.4/src/arfs/feature_selection/base.py` & `arfs-2.0.5/src/arfs/feature_selection/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-"""Base Submodule
-
-This module provides a base class for selector using a statistic and a threshold
-
-Module Structure:
------------------
-- ``BaseThresholdSelector``: parent class for the "treshold-based" selectors
-
-"""
-
-# Settings and libraries
-from __future__ import print_function
-
-# pandas
-import pandas as pd
-
-# numpy
-import numpy as np
-
-# sklearn
-
-from sklearn.utils.validation import check_is_fitted
-from sklearn.base import BaseEstimator
-from sklearn.feature_selection._base import SelectorMixin
-
-
-# fix random seed for reproducibility
-np.random.seed(7)
-
-
-class BaseThresholdSelector(SelectorMixin, BaseEstimator):
-    """Base class for threshold-based feature selection
-
-    Parameters
-    ----------
-    threshold : float, .05
-        Features with a training-set missing greater/lower (geq/leq) than this threshold will be removed
-    statistic_fn : callable, optional
-        The function for computing the statistic series. The index should be the column names and the
-        the values the computed statistic
-    greater_than_threshold : bool, False
-        Whether or not to reject the features if lower or greater than threshold
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    support_ : list of bool
-        the list of the selected X-columns
-    selected_features_ : list of str
-        the list of names of selected features
-    not_selected_features_ : list of str
-        the list of names of rejected features
-
-    """
-
-    def __init__(
-        self,
-        threshold=0.05,
-        statistic_fn=None,
-        greater_than_threshold=False,
-    ):
-        self.threshold = threshold
-        self.statistic_fn = statistic_fn
-        self.greater_than_threshold = greater_than_threshold
-
-    def fit(self, X, y=None, sample_weight=None):
-        """Learn empirical statistics from X.
-
-        Parameters
-        ----------
-        X : pd.DataFrame, shape (n_samples, n_features)
-            Data from which to compute variances, where `n_samples` is
-            the number of samples and `n_features` is the number of features.
-        y : any, default=None
-            Ignored. This parameter exists only for compatibility with
-            sklearn.pipeline.Pipeline.
-        sample_weight : pd.Series, optional, shape (n_samples,)
-            weights for computing the statistics (e.g. weighted average)
-
-        Returns
-        -------
-        self : object
-            Returns the instance itself.
-        """
-
-        # Calculate the fraction of missing in each column
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a dataframe")
-
-        self.statistic_series_ = self.statistic_fn(X)
-        self.statistic_df_ = pd.DataFrame(self.statistic_series_).rename(
-            columns={"index": "feature", 0: "statistic"}
-        )
-
-        # Sort with highest number of missing values on top
-        self.statistic_df_ = self.statistic_df_.sort_values(
-            "statistic", ascending=False
-        )
-        if self.greater_than_threshold:
-            self.support_ = self.statistic_series_.values >= self.threshold
-        else:
-            self.support_ = self.statistic_series_.values <= self.threshold
-
-        self.selected_features_ = self.feature_names_in_[self.support_]
-        self.not_selected_features_ = self.feature_names_in_[~self.support_]
-
-        return self
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def transform(self, X):
-        """
-        Transform the data, returns a transformed version of `X`.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-
-        Returns
-        -------
-        X_new : ndarray array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    def fit_transform(self, X, y=None, sample_weight=None, **fit_params):
-        """
-        Fit to data, then transform it.
-        Fits transformer to `X` and `y` with optional parameters `fit_params`
-        and returns a transformed version of `X`.
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            Target values (None for unsupervised transformations).
-        sample_weight :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            sample weight values.
-        **fit_params : dict
-            Additional fit parameters.
-        Returns
-        -------
-        X_new : ndarray array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        return self.fit(X=X, y=y, sample_weight=sample_weight, **fit_params).transform(
-            X
-        )
-
-    def _more_tags(self):
-        return {"allow_nan": True}
+"""Base Submodule
+
+This module provides a base class for selector using a statistic and a threshold
+
+Module Structure:
+-----------------
+- ``BaseThresholdSelector``: parent class for the "treshold-based" selectors
+
+"""
+
+# Settings and libraries
+from __future__ import print_function
+
+# pandas
+import pandas as pd
+
+# numpy
+import numpy as np
+
+# sklearn
+
+from sklearn.utils.validation import check_is_fitted
+from sklearn.base import BaseEstimator
+from sklearn.feature_selection._base import SelectorMixin
+
+
+# fix random seed for reproducibility
+np.random.seed(7)
+
+
+class BaseThresholdSelector(SelectorMixin, BaseEstimator):
+    """Base class for threshold-based feature selection
+
+    Parameters
+    ----------
+    threshold : float, .05
+        Features with a training-set missing greater/lower (geq/leq) than this threshold will be removed
+    statistic_fn : callable, optional
+        The function for computing the statistic series. The index should be the column names and the
+        the values the computed statistic
+    greater_than_threshold : bool, False
+        Whether or not to reject the features if lower or greater than threshold
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    support_ : list of bool
+        the list of the selected X-columns
+    selected_features_ : list of str
+        the list of names of selected features
+    not_selected_features_ : list of str
+        the list of names of rejected features
+
+    """
+
+    def __init__(
+        self,
+        threshold=0.05,
+        statistic_fn=None,
+        greater_than_threshold=False,
+    ):
+        self.threshold = threshold
+        self.statistic_fn = statistic_fn
+        self.greater_than_threshold = greater_than_threshold
+
+    def fit(self, X, y=None, sample_weight=None):
+        """Learn empirical statistics from X.
+
+        Parameters
+        ----------
+        X : pd.DataFrame, shape (n_samples, n_features)
+            Data from which to compute variances, where `n_samples` is
+            the number of samples and `n_features` is the number of features.
+        y : any, default=None
+            Ignored. This parameter exists only for compatibility with
+            sklearn.pipeline.Pipeline.
+        sample_weight : pd.Series, optional, shape (n_samples,)
+            weights for computing the statistics (e.g. weighted average)
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
+        """
+
+        # Calculate the fraction of missing in each column
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+        else:
+            raise TypeError("X is not a dataframe")
+
+        self.statistic_series_ = self.statistic_fn(X)
+        self.statistic_df_ = pd.DataFrame(self.statistic_series_).rename(
+            columns={"index": "feature", 0: "statistic"}
+        )
+
+        # Sort with highest number of missing values on top
+        self.statistic_df_ = self.statistic_df_.sort_values(
+            "statistic", ascending=False
+        )
+        if self.greater_than_threshold:
+            self.support_ = self.statistic_series_.values > self.threshold
+        else:
+            self.support_ = self.statistic_series_.values < self.threshold
+
+        self.selected_features_ = self.feature_names_in_[self.support_]
+        self.not_selected_features_ = self.feature_names_in_[~self.support_]
+
+        return self
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def transform(self, X):
+        """
+        Transform the data, returns a transformed version of `X`.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    def fit_transform(self, X, y=None, sample_weight=None, **fit_params):
+        """
+        Fit to data, then transform it.
+        Fits transformer to `X` and `y` with optional parameters `fit_params`
+        and returns a transformed version of `X`.
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            Target values (None for unsupervised transformations).
+        sample_weight :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            sample weight values.
+        **fit_params : dict
+            Additional fit parameters.
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        return self.fit(X=X, y=y, sample_weight=sample_weight, **fit_params).transform(
+            X
+        )
+
+    def _more_tags(self):
+        return {"allow_nan": True}
```

### Comparing `arfs-2.0.4/src/arfs/feature_selection/lasso.py` & `arfs-2.0.5/src/arfs/feature_selection/lasso.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,627 +1,627 @@
-"""LassoFeatureSelection Submodule
-
-This module provides LASSO-based feature selection, specifically designed for use with Generalized Linear Models (GLM). 
-The Lasso Regularized GLM introduces an L1 regularization penalty (Lasso regularization), 
-encouraging some coefficients to become exactly zero during the model fitting process. 
-This regularization effectively removes irrelevant features from the model, making it a 
-powerful tool for feature selection, particularly in datasets with numerous variables.
-
-Module Structure:
------------------
-- `EnetGLM`: class serves as a scikit-learn wrapper for the regularized statsmodels GLM, providing seamless integration with scikit-learn's ecosystem.
-- `weighted_cross_val_score`: function allows users to pass weights to the model and define a custom scoring metric.
-- `grid_search_cv`: function performs a weighted LASSO grid search to find the best Lasso parameter for the model.
-- `LassoFeatureSelection`: class is the core feature selection class, estimating the Lasso parameter through 
-    the grid search process, enabling efficient and effective feature selection.
-
-With this submodule, users can easily leverage Lasso Regularized GLMs and conduct feature selection, 
-improving model performance and interpretability in various datasets.
-"""
-
-import pandas as pd
-import numpy as np
-import statsmodels.api as sm
-from sklearn.base import BaseEstimator, TransformerMixin, RegressorMixin
-from sklearn.base import clone
-from sklearn.utils import check_array
-from sklearn.model_selection import StratifiedKFold, KFold
-from joblib import Parallel, delayed
-from typing import Union, Optional
-
-
-def _map_family_link(family: str = "gaussian", link: Optional[str] = None):
-    family_mapping = {
-        "gaussian": sm.families.Gaussian,
-        "binomial": sm.families.Binomial,
-        "poisson": sm.families.Poisson,
-        "gamma": sm.families.Gamma,
-        "negativebinomial": sm.families.NegativeBinomial,
-        "tweedie": sm.families.Tweedie,
-    }
-    link_mapping = {
-        "identity": sm.genmod.families.links.Identity(),
-        "log": sm.genmod.families.links.Log(),
-        "logit": sm.genmod.families.links.Logit(),
-        "probit": sm.genmod.families.links.Probit(),
-        "cloglog": sm.genmod.families.links.CLogLog(),
-        "inverse_squared": sm.genmod.families.links.InverseSquared(),
-    }
-    if link is not None:
-        objective = family_mapping[family](link_mapping[link])
-    else:
-        objective = family_mapping[family]()
-    return objective
-
-
-class EnetGLM(BaseEstimator, RegressorMixin):
-    """
-    Elastic Net Generalized Linear Model.
-
-    Parameters
-    ----------
-    family : statsmodels.family object, optional (default=sm.families.Gaussian())
-        The distributional assumption of the model.
-    alpha : float, optional (default=0.0)
-        The elastic net mixing parameter. 0 <= alpha <= 1.
-        alpha = 0 is equivalent to ridge regression, alpha = 1 is equivalent to lasso regression.
-    L1_wt : float, optional (default=0.0)
-        The weight of the L1 penalty term. 0 <= L1_wt <= 1.
-        L1_wt = 0 is equivalent to ridge regression, L1_wt = 1 is equivalent to lasso regression.
-    fit_intercept : bool, optional (default=True)
-        Whether to fit an intercept term in the model.
-    """
-
-    def __init__(
-        self,
-        family: str = "gaussian",
-        link: Optional[str] = None,
-        alpha: float = 0.0,
-        L1_wt: float = 1e-6,
-        fit_intercept: bool = True,
-    ):
-        """
-        Initialize self.
-
-        Parameters
-        ----------
-        family :
-            The distributional assumption of the model.
-        link:
-            the GLM link function
-        alpha :
-            The penalty weight. If a scalar, the same penalty weight applies to all variables in the model.
-            If a vector, it must have the same length as params, and contains a penalty weight for each coefficient.
-        L1_wt :
-            The `L1_wt` parameter represents the weight of the L1 penalty term in the model and
-            should be within the range 0 to 1. A value of 0 corresponds to ridge regression,
-            while a value of 1 corresponds to lasso regression. However, for obtaining statistics,
-            `L1_wt` should be set to a value greater than 0. If it is set to 0.0, statsmodels returns
-            a ridge regularized wrapper without refitting the model, making the statistics unavailable
-            and breaking the class. Nevertheless, you can set `L1_wt` to a very small value, such as 1e-9,
-            to obtain close-to-ridge behavior while still obtaining the necessary statistics.
-
-        fit_intercept :
-            Whether to fit an intercept term in the model.
-        """
-        self.family = family
-        self.link = link
-        self.alpha = alpha
-        self.L1_wt = L1_wt
-        self.model = None
-        self.result = None
-        self.fit_intercept = fit_intercept
-        self.objective = _map_family_link(family=family, link=link)
-
-    def fit(
-        self,
-        X: pd.DataFrame,
-        y: Union[np.ndarray, pd.Series],
-        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
-    ):
-        """
-        Fit the model to the data.
-
-        Notes
-        -----
-        In statsmodels and GLMs in general, you can use either an offset or a weight to account for
-        differences in exposure between observations. However, if you choose to use an offset,
-        you need to pass the number of cases (ncl) instead of the frequency and set the offset to
-        the logarithm of the exposure due to the log link function. It is recommended to use the frequency
-        and the weights instead of the offset because this ensures that all models have the same inputs.
-        To use the frequency and the weights, you can fit the model using the following code:
-
-        ```python
-        self.model = sm.GLM(endog=y, exog=X, var_weights=sample_weight, family=self.family)
-        ```
-
-        This is equivalent to using the exposure and the log of the exposure internally, which can be done using the following code:
-
-        ```python
-        self.model = sm.GLM(endog=y, exog=sm.add_constant(X), exposure=sample_weight, family=sm.families.Poisson())
-        self.result = self.model.fit()
-        ```
-
-        Parameters
-        ----------
-        X :
-            array-like, shape (n_samples, n_features)
-            The input data.
-        y :
-            array-like, shape (n_samples,)
-            The target values.
-        sample_weight : array-like, shape (n_samples,), optional (default=None)
-            Sample weights.
-
-        Returns
-        -------
-        self : object
-            Returns self.
-        """
-
-        # see the if kwargs.get("L1_wt", 1) == 0 condition in
-        # https://www.statsmodels.org/dev/_modules/statsmodels/genmod/generalized_linear_model.html#GLM.fit_regularized
-        # workaround to get the statistics
-        if self.alpha == 0.0:
-            self.alpha = 1e-9
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-
-        if self.fit_intercept:
-            X = sm.add_constant(X)
-            X = X.rename(columns={"const": "Intercept"})
-        else:
-            X = drop_existing_sm_constant_from_df(X)
-
-        self.n_features_in_ = X.shape[1]
-
-        self.model = sm.GLM(
-            endog=y,
-            exog=X,
-            var_weights=sample_weight,
-            family=self.objective,
-        )
-
-        self.result = self.model.fit_regularized(
-            method="elastic_net", alpha=self.alpha, L1_wt=self.L1_wt, refit=True
-        )
-        self.coef_ = self.result.params
-        self.bse_ = self.result.bse
-        self.deviance_ = self.result.deviance
-        self.pseudo_rsquared_ = self.result.pseudo_rsquared()
-        self.aic_ = self.result.aic
-        self.bic_ = self.result.bic_llf
-        self.pvalues_ = self.result.pvalues
-        self.tvalues_ = self.result.tvalues
-        self.pearson_chi2_ = self.result.pearson_chi2
-
-    def predict(self, X):
-        """
-        Predict using the fitted model.
-
-        Parameters
-        ----------
-        X :
-            array-like, shape (n_samples, n_features)
-            The input data.
-
-        Returns
-        -------
-        y : array-like, shape (n_samples,)
-            The predicted target values.
-
-        Raises
-        ------
-        ValueError
-            If the model has not been fit.
-        """
-        if self.model is None:
-            raise ValueError("Fit the model first.")
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-
-        if self.fit_intercept:
-            X = sm.add_constant(X)
-            X = X.rename(columns={"const": "Intercept"})
-
-        return self.result.predict(X)
-
-    def get_coef(self):
-        """
-        Get the estimated coefficients of the fitted model.
-
-        Returns
-        -------
-        coef_ : array-like, shape (n_features,)
-            The estimated coefficients of the fitted model.
-        """
-        return self.coef_
-
-    def score(
-        self,
-        X: pd.DataFrame,
-        y: pd.Series,
-        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
-    ):
-        """
-        Return the deviance of the fitted model.
-
-        Parameters
-        ----------
-        X :
-            array-like, shape (n_samples, n_features)
-            The input data.
-        sample_weight : array-like, shape (n_samples,), optional (default=None)
-            Sample weights.
-
-        Returns
-        -------
-        deviance : float
-            The deviance of the fitted model.
-        """
-        mu = self.objective.link.inverse(self.predict(X))
-
-        var_weights = sample_weight if sample_weight is not None else 1.0
-        return self.objective.deviance(endog=y, mu=mu, var_weights=var_weights)
-
-    def summary(self):
-        """
-        Print a summary of the fitted model.
-
-        Returns
-        -------
-        summary : str
-            The summary of the fitted model.
-        """
-        return self.result.summary()
-
-
-def weighted_cross_val_score(estimator, X, y, sample_weight=None, cv=5, n_jobs=-1):
-    """
-    Perform cross-validation for a scikit-learn estimator with a score function that requires sample_weight.
-
-    Parameters
-    ----------
-    estimator : estimator
-        The scikit-learn estimator object.
-    X : array-like of shape (n_samples, n_features)
-        The input features.
-    y : array-like of shape (n_samples,)
-        The target variable.
-    sample_weight : array-like of shape (n_samples,), optional
-        The sample weights for each data point.
-    cv : int, default=5
-        The number of cross-validation folds.
-    n_jobs:
-        the number of processes
-
-    Returns
-    -------
-    scores : array of shape (cv,)
-        The list of scores for each fold.
-    average_score : float
-        The average score across all folds.
-
-    """
-
-    # logging.info("Starting cross-validation...")
-
-    splitter = (
-        KFold(n_splits=cv) if len(np.unique(y)) > 2 else StratifiedKFold(n_splits=cv)
-    )
-
-    if not hasattr(estimator, "score") or not callable(getattr(estimator, "score")):
-        raise ValueError(
-            "The estimator does not have a score method that takes a sample_weight argument."
-        )
-
-    with Parallel(n_jobs=-1) as parallel:
-        scores = parallel(
-            delayed(_fit_and_score)(
-                estimator, X, y, train_index, test_index, sample_weight
-            )
-            for train_index, test_index in splitter.split(X)
-        )
-
-    # logging.info("Finished cross-validation.")
-    return scores
-
-
-def _fit_and_score(
-    estimator: BaseEstimator,
-    X: Union[pd.DataFrame, np.ndarray],
-    y: Union[pd.Series, np.ndarray],
-    train_index: np.ndarray,
-    test_index: np.ndarray,
-    sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
-) -> float:
-    """
-    Fit and score an estimator on a specified train-test split.
-
-    Parameters
-    ----------
-    estimator : BaseEstimator
-        The estimator object implementing the scikit-learn estimator interface.
-    X : Union[pd.DataFrame, np.ndarray]
-        The input features, can be either a pandas DataFrame or a numpy array.
-    y : Union[pd.Series, np.ndarray]
-        The target values, can be either a pandas Series or a numpy array.
-    train_index : np.ndarray
-        Array of indices representing the training data.
-    test_index : np.ndarray
-        Array of indices representing the test data.
-    sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
-        Sample weights to be used during training. Can be either a pandas Series or a numpy array.
-
-    Returns
-    -------
-    float
-        The score of the estimator on the test data.
-
-    Raises
-    ------
-    ValueError
-        If the input data is not of the correct format.
-    """
-    # X = X.values if isinstance(X, pd.DataFrame) else X
-    y = y.values if isinstance(y, pd.Series) else y
-    X_train, X_test = X.iloc[train_index, :], X.iloc[test_index, :]
-    y_train, y_test = y[train_index], y[test_index]
-
-    if sample_weight is not None:
-        sample_weight = (
-            sample_weight.values
-            if isinstance(sample_weight, pd.Series)
-            else sample_weight
-        )
-        sample_weight_train = sample_weight[train_index]
-        sample_weight_test = sample_weight[test_index]
-        estimator.fit(X_train, y_train, sample_weight=sample_weight_train)
-        score = estimator.score(X_test, y_test, sample_weight=sample_weight_test)
-    else:
-        estimator.fit(X_train, y_train)
-        score = estimator.score(X_test, y_test)
-
-    return score
-
-
-def grid_search_cv(
-    X: Union[pd.DataFrame, np.ndarray],
-    y: Union[pd.Series, np.ndarray],
-    sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
-    n_iterations: int = 10,
-    family: str = "gaussian",
-    score: str = "bic",
-    fit_intercept: bool = True,
-) -> EnetGLM:
-    """
-    Perform grid search cross-validation for an Elastic Net Generalized Linear Model (EnetGLM).
-
-    Parameters
-    ----------
-    X : Union[pd.DataFrame, np.ndarray]
-        The input features, can be either a pandas DataFrame or a numpy array.
-    y : Union[pd.Series, np.ndarray]
-        The target values, can be either a pandas Series or a numpy array.
-    sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
-        Sample weights to be used during training. Can be either a pandas Series or a numpy array.
-    n_iterations : int, default=10
-        Number of iterations for the grid search.
-    family : str, default="gaussian"
-        The family of the GLM. Options: "gaussian", "poisson", "gamma", "negativebinomial", "binomial", "tweedie".
-    score : str, default="bic"
-        The score to use for model selection. Options: "bic" (Bayesian Information Criterion) or "mean_cv" (mean cross-validation score).
-
-    Returns
-    -------
-    EnetGLM
-        The best estimator found after grid search cross-validation.
-
-    Raises
-    ------
-    ValueError
-        If the input data is not of the correct format or if an invalid family or score value is provided.
-    """
-    estimator = EnetGLM(family=family, L1_wt=1.0, fit_intercept=fit_intercept)
-
-    # Check if X and y are pandas DataFrames/Series and convert them to numpy arrays if necessary
-    # X = check_array(X, accept_sparse=True, force_all_finite=False)
-    y = check_array(y, ensure_2d=False, force_all_finite=False)
-
-    if score not in ["bic", "deviance"]:
-        raise ValueError("Invalid score value. Options are: 'bic' or 'deviance'.")
-
-    grid = np.logspace(-3, 3, n_iterations)
-    param_score = []
-
-    for param in grid:
-        estimator = clone(estimator)
-        estimator.set_params(
-            **{
-                "alpha": param,
-                "L1_wt": 1.0,
-                "fit_intercept": fit_intercept,
-                "family": family,
-            }
-        )
-
-        if score == "bic":
-            estimator.fit(X=X, y=y, sample_weight=sample_weight)
-            param_score.append(estimator.bic_)
-        else:
-            scores = weighted_cross_val_score(
-                estimator, X, y, sample_weight=sample_weight, cv=5, n_jobs=-1
-            )
-            param_score.append(np.mean(scores))
-    # min deviance or min BIC
-    best_alpha_value = grid[np.argmin(param_score)]
-    best_estimator = clone(estimator)
-    best_estimator.set_params(
-        **{
-            "alpha": best_alpha_value,
-            "L1_wt": 1.0,
-            "fit_intercept": fit_intercept,
-            "family": family,
-        }
-    )
-    best_estimator.fit(X, y, sample_weight=sample_weight)
-
-    return best_estimator
-
-
-class LassoFeatureSelection(BaseEstimator, TransformerMixin):
-    """
-    LassoFeatureSelection performs feature selection using GLM Lasso regularization.
-
-    Parameters
-    ----------
-    family : str, default="gaussian"
-        The family of the GLM. Options: "gaussian", "poisson", "gamma", "negativebinomial", "binomial", "tweedie".
-    n_iterations : int, default=10
-        Number of iterations for the grid search.
-    score : str, default="bic"
-        The score to use for model selection. Options: "bic" (Bayesian Information Criterion) or "mean_cv" (mean cross-validation score).
-
-    Attributes
-    ----------
-    family : str
-        The family of the GLM.
-    n_iterations : int
-        Number of iterations for the grid search.
-    best_estimator_ : EnetGLM
-        The best estimator found after grid search cross-validation.
-    selected_features_ : ndarray
-        The selected feature names.
-    support_ : ndarray
-        The support of selected features (True for selected, False otherwise).
-    feature_names_in_ : ndarray
-        The input feature names.
-    score : str
-        The score used for model selection.
-
-    Methods
-    -------
-    fit(X, y=None, sample_weight=None)
-        Fit the LassoFeatureSelection model and select the best features.
-    transform(X)
-        Transform the input data to keep only the selected features.
-    get_feature_names_out()
-        Get the names of the selected features.
-
-    """
-
-    def __init__(
-        self,
-        family: str = "gaussian",
-        n_iterations: int = 10,
-        score: str = "bic",
-        fit_intercept: bool = True,
-    ):
-        self.family = family
-        self.n_iterations = n_iterations
-        self.best_estimator_ = None
-        self.selected_features_ = None
-        self.support_ = None
-        self.feature_names_in_ = None
-        self.score = score
-        self.fit_intercept = fit_intercept
-
-    def fit(
-        self,
-        X: Union[pd.DataFrame, np.ndarray],
-        y: Optional[Union[pd.Series, np.ndarray]] = None,
-        sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
-    ):
-        """
-        Fit the LassoFeatureSelection model and select the best features.
-
-        Parameters
-        ----------
-        X : Union[pd.DataFrame, np.ndarray]
-            The input features, can be either a pandas DataFrame or a numpy array.
-        y : Optional[Union[pd.Series, np.ndarray]], default=None
-            The target values, can be either a pandas Series or a numpy array.
-        sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
-            Sample weights to be used during training. Can be either a pandas Series or a numpy array.
-
-        Returns
-        -------
-        LassoFeatureSelection
-            The fitted LassoFeatureSelection model.
-
-        """
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-
-        if not self.fit_intercept:
-            X = drop_existing_sm_constant_from_df(X)
-
-        self.feature_names_in_ = (
-            X.columns.insert(0, "Intercept")
-            if self.fit_intercept and "Intercept" not in X.columns
-            else X.columns
-        )
-
-        self.best_estimator_ = grid_search_cv(
-            family=self.family,
-            X=X,
-            y=y,
-            sample_weight=sample_weight,
-            n_iterations=self.n_iterations,
-            score=self.score,
-            fit_intercept=self.fit_intercept,
-        )
-        self.support_ = self.best_estimator_.coef_ != 0
-        self.selected_features_ = self.feature_names_in_[self.support_]
-        return self
-
-    def transform(self, X: Union[pd.DataFrame, np.ndarray]) -> pd.DataFrame:
-        """
-        Transform the input data to keep only the selected features.
-
-        Parameters
-        ----------
-        X : Union[pd.DataFrame, np.ndarray]
-            The input features, can be either a pandas DataFrame or a numpy array.
-
-        Returns
-        -------
-        Union[pd.DataFrame, np.ndarray]
-            The transformed data with only the selected features.
-
-        """
-
-        if self.fit_intercept:
-            X = sm.add_constant(X)
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-            # if not a DF, assuming the col orders is
-            # the same, as required anyway
-            X.columns = self.feature_names_in_
-
-        X = X.rename(columns={"const": "Intercept"}) if "const" in X.columns else X
-        return X[self.selected_features_]
-
-    def get_feature_names_out(self) -> np.ndarray:
-        """
-        Get the names of the selected features.
-
-        Returns
-        -------
-        np.ndarray
-            The names of the selected features.
-
-        """
-        return self.feature_names_in_[self.support_]
-
-
-def drop_existing_sm_constant_from_df(X):
-    X = X.drop(columns=["Intercept"]) if "Intercept" in X.columns else X
-    X = X.drop(columns=["const"]) if "const" in X.columns else X
-    X = X.drop(columns=["intercept"]) if "intercept" in X.columns else X
-    return X
+"""LassoFeatureSelection Submodule
+
+This module provides LASSO-based feature selection, specifically designed for use with Generalized Linear Models (GLM). 
+The Lasso Regularized GLM introduces an L1 regularization penalty (Lasso regularization), 
+encouraging some coefficients to become exactly zero during the model fitting process. 
+This regularization effectively removes irrelevant features from the model, making it a 
+powerful tool for feature selection, particularly in datasets with numerous variables.
+
+Module Structure:
+-----------------
+- `EnetGLM`: class serves as a scikit-learn wrapper for the regularized statsmodels GLM, providing seamless integration with scikit-learn's ecosystem.
+- `weighted_cross_val_score`: function allows users to pass weights to the model and define a custom scoring metric.
+- `grid_search_cv`: function performs a weighted LASSO grid search to find the best Lasso parameter for the model.
+- `LassoFeatureSelection`: class is the core feature selection class, estimating the Lasso parameter through 
+    the grid search process, enabling efficient and effective feature selection.
+
+With this submodule, users can easily leverage Lasso Regularized GLMs and conduct feature selection, 
+improving model performance and interpretability in various datasets.
+"""
+
+import pandas as pd
+import numpy as np
+import statsmodels.api as sm
+from sklearn.base import BaseEstimator, TransformerMixin, RegressorMixin
+from sklearn.base import clone
+from sklearn.utils import check_array
+from sklearn.model_selection import StratifiedKFold, KFold
+from joblib import Parallel, delayed
+from typing import Union, Optional
+
+
+def _map_family_link(family: str = "gaussian", link: Optional[str] = None):
+    family_mapping = {
+        "gaussian": sm.families.Gaussian,
+        "binomial": sm.families.Binomial,
+        "poisson": sm.families.Poisson,
+        "gamma": sm.families.Gamma,
+        "negativebinomial": sm.families.NegativeBinomial,
+        "tweedie": sm.families.Tweedie,
+    }
+    link_mapping = {
+        "identity": sm.genmod.families.links.Identity(),
+        "log": sm.genmod.families.links.Log(),
+        "logit": sm.genmod.families.links.Logit(),
+        "probit": sm.genmod.families.links.Probit(),
+        "cloglog": sm.genmod.families.links.CLogLog(),
+        "inverse_squared": sm.genmod.families.links.InverseSquared(),
+    }
+    if link is not None:
+        objective = family_mapping[family](link_mapping[link])
+    else:
+        objective = family_mapping[family]()
+    return objective
+
+
+class EnetGLM(BaseEstimator, RegressorMixin):
+    """
+    Elastic Net Generalized Linear Model.
+
+    Parameters
+    ----------
+    family : statsmodels.family object, optional (default=sm.families.Gaussian())
+        The distributional assumption of the model.
+    alpha : float, optional (default=0.0)
+        The elastic net mixing parameter. 0 <= alpha <= 1.
+        alpha = 0 is equivalent to ridge regression, alpha = 1 is equivalent to lasso regression.
+    L1_wt : float, optional (default=0.0)
+        The weight of the L1 penalty term. 0 <= L1_wt <= 1.
+        L1_wt = 0 is equivalent to ridge regression, L1_wt = 1 is equivalent to lasso regression.
+    fit_intercept : bool, optional (default=True)
+        Whether to fit an intercept term in the model.
+    """
+
+    def __init__(
+        self,
+        family: str = "gaussian",
+        link: Optional[str] = None,
+        alpha: float = 0.0,
+        L1_wt: float = 1e-6,
+        fit_intercept: bool = True,
+    ):
+        """
+        Initialize self.
+
+        Parameters
+        ----------
+        family :
+            The distributional assumption of the model.
+        link:
+            the GLM link function
+        alpha :
+            The penalty weight. If a scalar, the same penalty weight applies to all variables in the model.
+            If a vector, it must have the same length as params, and contains a penalty weight for each coefficient.
+        L1_wt :
+            The `L1_wt` parameter represents the weight of the L1 penalty term in the model and
+            should be within the range 0 to 1. A value of 0 corresponds to ridge regression,
+            while a value of 1 corresponds to lasso regression. However, for obtaining statistics,
+            `L1_wt` should be set to a value greater than 0. If it is set to 0.0, statsmodels returns
+            a ridge regularized wrapper without refitting the model, making the statistics unavailable
+            and breaking the class. Nevertheless, you can set `L1_wt` to a very small value, such as 1e-9,
+            to obtain close-to-ridge behavior while still obtaining the necessary statistics.
+
+        fit_intercept :
+            Whether to fit an intercept term in the model.
+        """
+        self.family = family
+        self.link = link
+        self.alpha = alpha
+        self.L1_wt = L1_wt
+        self.model = None
+        self.result = None
+        self.fit_intercept = fit_intercept
+        self.objective = _map_family_link(family=family, link=link)
+
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: Union[np.ndarray, pd.Series],
+        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
+    ):
+        """
+        Fit the model to the data.
+
+        Notes
+        -----
+        In statsmodels and GLMs in general, you can use either an offset or a weight to account for
+        differences in exposure between observations. However, if you choose to use an offset,
+        you need to pass the number of cases (ncl) instead of the frequency and set the offset to
+        the logarithm of the exposure due to the log link function. It is recommended to use the frequency
+        and the weights instead of the offset because this ensures that all models have the same inputs.
+        To use the frequency and the weights, you can fit the model using the following code:
+
+        ```python
+        self.model = sm.GLM(endog=y, exog=X, var_weights=sample_weight, family=self.family)
+        ```
+
+        This is equivalent to using the exposure and the log of the exposure internally, which can be done using the following code:
+
+        ```python
+        self.model = sm.GLM(endog=y, exog=sm.add_constant(X), exposure=sample_weight, family=sm.families.Poisson())
+        self.result = self.model.fit()
+        ```
+
+        Parameters
+        ----------
+        X :
+            array-like, shape (n_samples, n_features)
+            The input data.
+        y :
+            array-like, shape (n_samples,)
+            The target values.
+        sample_weight : array-like, shape (n_samples,), optional (default=None)
+            Sample weights.
+
+        Returns
+        -------
+        self : object
+            Returns self.
+        """
+
+        # see the if kwargs.get("L1_wt", 1) == 0 condition in
+        # https://www.statsmodels.org/dev/_modules/statsmodels/genmod/generalized_linear_model.html#GLM.fit_regularized
+        # workaround to get the statistics
+        if self.alpha == 0.0:
+            self.alpha = 1e-9
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
+
+        if self.fit_intercept:
+            X = sm.add_constant(X)
+            X = X.rename(columns={"const": "Intercept"})
+        else:
+            X = drop_existing_sm_constant_from_df(X)
+
+        self.n_features_in_ = X.shape[1]
+
+        self.model = sm.GLM(
+            endog=y,
+            exog=X,
+            var_weights=sample_weight,
+            family=self.objective,
+        )
+
+        self.result = self.model.fit_regularized(
+            method="elastic_net", alpha=self.alpha, L1_wt=self.L1_wt, refit=True
+        )
+        self.coef_ = self.result.params
+        self.bse_ = self.result.bse
+        self.deviance_ = self.result.deviance
+        self.pseudo_rsquared_ = self.result.pseudo_rsquared()
+        self.aic_ = self.result.aic
+        self.bic_ = self.result.bic_llf
+        self.pvalues_ = self.result.pvalues
+        self.tvalues_ = self.result.tvalues
+        self.pearson_chi2_ = self.result.pearson_chi2
+
+    def predict(self, X):
+        """
+        Predict using the fitted model.
+
+        Parameters
+        ----------
+        X :
+            array-like, shape (n_samples, n_features)
+            The input data.
+
+        Returns
+        -------
+        y : array-like, shape (n_samples,)
+            The predicted target values.
+
+        Raises
+        ------
+        ValueError
+            If the model has not been fit.
+        """
+        if self.model is None:
+            raise ValueError("Fit the model first.")
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
+
+        if self.fit_intercept:
+            X = sm.add_constant(X)
+            X = X.rename(columns={"const": "Intercept"})
+
+        return self.result.predict(X)
+
+    def get_coef(self):
+        """
+        Get the estimated coefficients of the fitted model.
+
+        Returns
+        -------
+        coef_ : array-like, shape (n_features,)
+            The estimated coefficients of the fitted model.
+        """
+        return self.coef_
+
+    def score(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        sample_weight: Optional[Union[np.ndarray, pd.Series]] = None,
+    ):
+        """
+        Return the deviance of the fitted model.
+
+        Parameters
+        ----------
+        X :
+            array-like, shape (n_samples, n_features)
+            The input data.
+        sample_weight : array-like, shape (n_samples,), optional (default=None)
+            Sample weights.
+
+        Returns
+        -------
+        deviance : float
+            The deviance of the fitted model.
+        """
+        mu = self.objective.link.inverse(self.predict(X))
+
+        var_weights = sample_weight if sample_weight is not None else 1.0
+        return self.objective.deviance(endog=y, mu=mu, var_weights=var_weights)
+
+    def summary(self):
+        """
+        Print a summary of the fitted model.
+
+        Returns
+        -------
+        summary : str
+            The summary of the fitted model.
+        """
+        return self.result.summary()
+
+
+def weighted_cross_val_score(estimator, X, y, sample_weight=None, cv=5, n_jobs=-1):
+    """
+    Perform cross-validation for a scikit-learn estimator with a score function that requires sample_weight.
+
+    Parameters
+    ----------
+    estimator : estimator
+        The scikit-learn estimator object.
+    X : array-like of shape (n_samples, n_features)
+        The input features.
+    y : array-like of shape (n_samples,)
+        The target variable.
+    sample_weight : array-like of shape (n_samples,), optional
+        The sample weights for each data point.
+    cv : int, default=5
+        The number of cross-validation folds.
+    n_jobs:
+        the number of processes
+
+    Returns
+    -------
+    scores : array of shape (cv,)
+        The list of scores for each fold.
+    average_score : float
+        The average score across all folds.
+
+    """
+
+    # logging.info("Starting cross-validation...")
+
+    splitter = (
+        KFold(n_splits=cv) if len(np.unique(y)) > 2 else StratifiedKFold(n_splits=cv)
+    )
+
+    if not hasattr(estimator, "score") or not callable(getattr(estimator, "score")):
+        raise ValueError(
+            "The estimator does not have a score method that takes a sample_weight argument."
+        )
+
+    with Parallel(n_jobs=-1) as parallel:
+        scores = parallel(
+            delayed(_fit_and_score)(
+                estimator, X, y, train_index, test_index, sample_weight
+            )
+            for train_index, test_index in splitter.split(X)
+        )
+
+    # logging.info("Finished cross-validation.")
+    return scores
+
+
+def _fit_and_score(
+    estimator: BaseEstimator,
+    X: Union[pd.DataFrame, np.ndarray],
+    y: Union[pd.Series, np.ndarray],
+    train_index: np.ndarray,
+    test_index: np.ndarray,
+    sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
+) -> float:
+    """
+    Fit and score an estimator on a specified train-test split.
+
+    Parameters
+    ----------
+    estimator : BaseEstimator
+        The estimator object implementing the scikit-learn estimator interface.
+    X : Union[pd.DataFrame, np.ndarray]
+        The input features, can be either a pandas DataFrame or a numpy array.
+    y : Union[pd.Series, np.ndarray]
+        The target values, can be either a pandas Series or a numpy array.
+    train_index : np.ndarray
+        Array of indices representing the training data.
+    test_index : np.ndarray
+        Array of indices representing the test data.
+    sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
+        Sample weights to be used during training. Can be either a pandas Series or a numpy array.
+
+    Returns
+    -------
+    float
+        The score of the estimator on the test data.
+
+    Raises
+    ------
+    ValueError
+        If the input data is not of the correct format.
+    """
+    # X = X.values if isinstance(X, pd.DataFrame) else X
+    y = y.values if isinstance(y, pd.Series) else y
+    X_train, X_test = X.iloc[train_index, :], X.iloc[test_index, :]
+    y_train, y_test = y[train_index], y[test_index]
+
+    if sample_weight is not None:
+        sample_weight = (
+            sample_weight.values
+            if isinstance(sample_weight, pd.Series)
+            else sample_weight
+        )
+        sample_weight_train = sample_weight[train_index]
+        sample_weight_test = sample_weight[test_index]
+        estimator.fit(X_train, y_train, sample_weight=sample_weight_train)
+        score = estimator.score(X_test, y_test, sample_weight=sample_weight_test)
+    else:
+        estimator.fit(X_train, y_train)
+        score = estimator.score(X_test, y_test)
+
+    return score
+
+
+def grid_search_cv(
+    X: Union[pd.DataFrame, np.ndarray],
+    y: Union[pd.Series, np.ndarray],
+    sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
+    n_iterations: int = 10,
+    family: str = "gaussian",
+    score: str = "bic",
+    fit_intercept: bool = True,
+) -> EnetGLM:
+    """
+    Perform grid search cross-validation for an Elastic Net Generalized Linear Model (EnetGLM).
+
+    Parameters
+    ----------
+    X : Union[pd.DataFrame, np.ndarray]
+        The input features, can be either a pandas DataFrame or a numpy array.
+    y : Union[pd.Series, np.ndarray]
+        The target values, can be either a pandas Series or a numpy array.
+    sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
+        Sample weights to be used during training. Can be either a pandas Series or a numpy array.
+    n_iterations : int, default=10
+        Number of iterations for the grid search.
+    family : str, default="gaussian"
+        The family of the GLM. Options: "gaussian", "poisson", "gamma", "negativebinomial", "binomial", "tweedie".
+    score : str, default="bic"
+        The score to use for model selection. Options: "bic" (Bayesian Information Criterion) or "mean_cv" (mean cross-validation score).
+
+    Returns
+    -------
+    EnetGLM
+        The best estimator found after grid search cross-validation.
+
+    Raises
+    ------
+    ValueError
+        If the input data is not of the correct format or if an invalid family or score value is provided.
+    """
+    estimator = EnetGLM(family=family, L1_wt=1.0, fit_intercept=fit_intercept)
+
+    # Check if X and y are pandas DataFrames/Series and convert them to numpy arrays if necessary
+    # X = check_array(X, accept_sparse=True, force_all_finite=False)
+    y = check_array(y, ensure_2d=False, force_all_finite=False)
+
+    if score not in ["bic", "deviance"]:
+        raise ValueError("Invalid score value. Options are: 'bic' or 'deviance'.")
+
+    grid = np.logspace(-3, 3, n_iterations)
+    param_score = []
+
+    for param in grid:
+        estimator = clone(estimator)
+        estimator.set_params(
+            **{
+                "alpha": param,
+                "L1_wt": 1.0,
+                "fit_intercept": fit_intercept,
+                "family": family,
+            }
+        )
+
+        if score == "bic":
+            estimator.fit(X=X, y=y, sample_weight=sample_weight)
+            param_score.append(estimator.bic_)
+        else:
+            scores = weighted_cross_val_score(
+                estimator, X, y, sample_weight=sample_weight, cv=5, n_jobs=-1
+            )
+            param_score.append(np.mean(scores))
+    # min deviance or min BIC
+    best_alpha_value = grid[np.argmin(param_score)]
+    best_estimator = clone(estimator)
+    best_estimator.set_params(
+        **{
+            "alpha": best_alpha_value,
+            "L1_wt": 1.0,
+            "fit_intercept": fit_intercept,
+            "family": family,
+        }
+    )
+    best_estimator.fit(X, y, sample_weight=sample_weight)
+
+    return best_estimator
+
+
+class LassoFeatureSelection(BaseEstimator, TransformerMixin):
+    """
+    LassoFeatureSelection performs feature selection using GLM Lasso regularization.
+
+    Parameters
+    ----------
+    family : str, default="gaussian"
+        The family of the GLM. Options: "gaussian", "poisson", "gamma", "negativebinomial", "binomial", "tweedie".
+    n_iterations : int, default=10
+        Number of iterations for the grid search.
+    score : str, default="bic"
+        The score to use for model selection. Options: "bic" (Bayesian Information Criterion) or "mean_cv" (mean cross-validation score).
+
+    Attributes
+    ----------
+    family : str
+        The family of the GLM.
+    n_iterations : int
+        Number of iterations for the grid search.
+    best_estimator_ : EnetGLM
+        The best estimator found after grid search cross-validation.
+    selected_features_ : ndarray
+        The selected feature names.
+    support_ : ndarray
+        The support of selected features (True for selected, False otherwise).
+    feature_names_in_ : ndarray
+        The input feature names.
+    score : str
+        The score used for model selection.
+
+    Methods
+    -------
+    fit(X, y=None, sample_weight=None)
+        Fit the LassoFeatureSelection model and select the best features.
+    transform(X)
+        Transform the input data to keep only the selected features.
+    get_feature_names_out()
+        Get the names of the selected features.
+
+    """
+
+    def __init__(
+        self,
+        family: str = "gaussian",
+        n_iterations: int = 10,
+        score: str = "bic",
+        fit_intercept: bool = True,
+    ):
+        self.family = family
+        self.n_iterations = n_iterations
+        self.best_estimator_ = None
+        self.selected_features_ = None
+        self.support_ = None
+        self.feature_names_in_ = None
+        self.score = score
+        self.fit_intercept = fit_intercept
+
+    def fit(
+        self,
+        X: Union[pd.DataFrame, np.ndarray],
+        y: Optional[Union[pd.Series, np.ndarray]] = None,
+        sample_weight: Optional[Union[pd.Series, np.ndarray]] = None,
+    ):
+        """
+        Fit the LassoFeatureSelection model and select the best features.
+
+        Parameters
+        ----------
+        X : Union[pd.DataFrame, np.ndarray]
+            The input features, can be either a pandas DataFrame or a numpy array.
+        y : Optional[Union[pd.Series, np.ndarray]], default=None
+            The target values, can be either a pandas Series or a numpy array.
+        sample_weight : Optional[Union[pd.Series, np.ndarray]], default=None
+            Sample weights to be used during training. Can be either a pandas Series or a numpy array.
+
+        Returns
+        -------
+        LassoFeatureSelection
+            The fitted LassoFeatureSelection model.
+
+        """
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
+
+        if not self.fit_intercept:
+            X = drop_existing_sm_constant_from_df(X)
+
+        self.feature_names_in_ = (
+            X.columns.insert(0, "Intercept")
+            if self.fit_intercept and "Intercept" not in X.columns
+            else X.columns
+        )
+
+        self.best_estimator_ = grid_search_cv(
+            family=self.family,
+            X=X,
+            y=y,
+            sample_weight=sample_weight,
+            n_iterations=self.n_iterations,
+            score=self.score,
+            fit_intercept=self.fit_intercept,
+        )
+        self.support_ = self.best_estimator_.coef_ != 0
+        self.selected_features_ = self.feature_names_in_[self.support_]
+        return self
+
+    def transform(self, X: Union[pd.DataFrame, np.ndarray]) -> pd.DataFrame:
+        """
+        Transform the input data to keep only the selected features.
+
+        Parameters
+        ----------
+        X : Union[pd.DataFrame, np.ndarray]
+            The input features, can be either a pandas DataFrame or a numpy array.
+
+        Returns
+        -------
+        Union[pd.DataFrame, np.ndarray]
+            The transformed data with only the selected features.
+
+        """
+
+        if self.fit_intercept:
+            X = sm.add_constant(X)
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            # if not a DF, assuming the col orders is
+            # the same, as required anyway
+            X.columns = self.feature_names_in_
+
+        X = X.rename(columns={"const": "Intercept"}) if "const" in X.columns else X
+        return X[self.selected_features_]
+
+    def get_feature_names_out(self) -> np.ndarray:
+        """
+        Get the names of the selected features.
+
+        Returns
+        -------
+        np.ndarray
+            The names of the selected features.
+
+        """
+        return self.feature_names_in_[self.support_]
+
+
+def drop_existing_sm_constant_from_df(X):
+    X = X.drop(columns=["Intercept"]) if "Intercept" in X.columns else X
+    X = X.drop(columns=["const"]) if "const" in X.columns else X
+    X = X.drop(columns=["intercept"]) if "intercept" in X.columns else X
+    return X
```

### Comparing `arfs-2.0.4/src/arfs/feature_selection/mrmr.py` & `arfs-2.0.5/src/arfs/feature_selection/mrmr.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,346 +1,346 @@
-"""MRMR Feature Selection Module
-
-This module provides MinRedundancyMaxRelevance (MRMR) feature selection for classification or regression tasks. 
-In a classification task, the target should be of object or pandas category dtype, while in a regression task, 
-the target should be of numpy categorical dtype. The predictors can be categorical or numerical without requiring encoding, 
-as the appropriate method (correlation, correlation ratio, or Theil's U) will be automatically selected based on the data type.
-
-Module Structure:
------------------
-- ``MinRedundancyMaxRelevance``: MRMR feature selection class for classification or regression tasks.
-"""
-
-import functools
-import numpy as np
-import pandas as pd
-from sklearn.base import BaseEstimator
-from sklearn.utils.validation import check_is_fitted
-from tqdm.auto import tqdm
-from sklearn.feature_selection._base import SelectorMixin
-from ..association import (
-    f_stat_classification_parallel,
-    f_stat_regression_parallel,
-    association_series,
-)
-
-FLOOR = 0.001
-
-
-class MinRedundancyMaxRelevance(SelectorMixin, BaseEstimator):
-    """MRMR feature selection for a classification or a regression task
-    For a classification task, the target should be of object or pandas category
-    dtype. For a regression task, the target should be of numpy categorical dtype.
-    The predictors can be categorical or numerical, there is no encoding required.
-    The dtype will be automatically detected and the right method applied (either
-    correlation, correlation ration or Theil's U)
-
-
-    Parameters
-    ----------
-    n_features_to_select: int
-        Number of features to select.
-    relevance_func: callable, optional
-        relevance function having arguments "X", "y", "sample_weight" and returning a pd.Series
-        containing a score of relevance for each feature
-    redundancy: callable, optional
-        Redundancy method.
-        If callable, it should take "X", "sample_weight" as input and return a pandas.Series
-        containing a score of redundancy for each feature.
-    denominator: str or callable (optional, default='mean')
-        Synthesis function to apply to the denominator of MRMR score.
-        If string, name of method. Supported: 'max', 'mean'.
-        If callable, it should take an iterable as input and return a scalar.
-    task: str
-        either "regression" or "classifiction"
-    only_same_domain: bool (optional, default=False)
-        If False, all the necessary correlation coefficients are computed.
-        If True, only features belonging to the same domain are compared.
-        Domain is defined by the string preceding the first underscore:
-        for instance "cusinfo_age" and "cusinfo_income" belong to the same domain, whereas "age" and "income" don't.
-    return_scores: bool (optional, default=False)
-        If False, only the list of selected features is returned.
-        If True, a tuple containing (list of selected features, relevance, redundancy) is returned.
-    n_jobs: int (optional, default=-1)
-        Maximum number of workers to use. Only used when relevance = "f" or redundancy = "corr".
-        If -1, use as many workers as min(cpu count, number of features).
-    show_progress: bool (optional, default=True)
-        If False, no progress bar is displayed.
-        If True, a TQDM progress bar shows the number of features processed.
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    ranking_ : pd.DataFrame
-        name and scores for the selected features
-    support_ : list of bool
-        the list of the selected X-columns
-    Example
-    -------
-    >>> from sklearn.datasets import make_classification, make_regression
-    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
-    >>> X = pd.DataFrame(X)
-    >>> y = pd.Series(y)
-    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
-    >>> X.columns = pred_name
-    >>> y.name = "target"
-    >>> fs_mrmr = MinRedundancyMaxRelevance(n_features_to_select=5,
-    >>>                  relevance_func=None,
-    >>>                  redundancy_func=None,
-    >>>                  task= "regression",#"classification",
-    >>>                  denominator_func=np.mean,
-    >>>                  only_same_domain=False,
-    >>>                  return_scores=False,
-    >>>                  show_progress=True)
-    >>> #fs_mrmr.fit(X=X, y=y.astype(str), sample_weight=None)
-    >>> fs_mrmr.fit(X=X, y=y, sample_weight=None)
-    """
-
-    def __init__(
-        self,
-        n_features_to_select,
-        relevance_func=None,
-        redundancy_func=None,
-        task="regression",
-        denominator_func=np.mean,
-        only_same_domain=False,
-        return_scores=False,
-        n_jobs=-1,
-        show_progress=True,
-    ):
-        self.n_features_to_select = n_features_to_select
-        self.relevance_func = relevance_func
-        self.redundancy_func = redundancy_func
-        self.denominator_func = denominator_func
-        self.only_same_domain = only_same_domain
-        self.return_scores = return_scores
-        self.show_progress = show_progress
-        self.n_jobs = n_jobs
-        self.task = task
-
-        if self.relevance_func is None:
-            if self.task == "regression":
-                self.relevance_func = functools.partial(
-                    f_stat_regression_parallel, n_jobs=self.n_jobs
-                )
-            else:
-                self.relevance_func = functools.partial(
-                    f_stat_classification_parallel, n_jobs=self.n_jobs
-                )
-
-        if self.redundancy_func is None:
-            self.redundancy_func = functools.partial(
-                association_series, n_jobs=self.n_jobs, normalize=True
-            )
-
-    def fit(self, X, y, sample_weight=None):
-        """fit the MRmr selector by learning the associations
-
-        Parameters
-        ----------
-        X : pd.DataFrame, shape (n_samples, n_features)
-            Data from which to compute variances, where `n_samples` is
-            the number of samples and `n_features` is the number of features.
-        y : any, default=None
-            Ignored. This parameter exists only for compatibility with
-            sklearn.pipeline.Pipeline.
-        sample_weight : pd.Series, optional, shape (n_samples,)
-            weights for computing the statistics (e.g. weighted average)
-
-        Returns
-        -------
-        self : object
-            Returns the instance itself.
-        """
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a pd.DataFrame")
-
-        if not isinstance(y, pd.Series):
-            y = pd.Series(y)
-
-        y.name = "target"
-
-        target = y.copy()
-        if self.task == "classification":
-            target = target.astype("category")
-
-        self.relevance_args = {"X": X, "y": target, "sample_weight": sample_weight}
-        self.redundancy_args = {"X": X, "sample_weight": sample_weight}
-
-        self.relevance = self.relevance_func(**self.relevance_args)
-        self.features = self.relevance[~self.relevance.isna()].index.to_list()
-        self.relevance = self.relevance.loc[self.features]
-        self.redundancy = pd.DataFrame(
-            FLOOR, index=self.features, columns=self.features
-        )
-        self.n_features_to_select = min(self.n_features_to_select, len(self.features))
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-
-        self.n_features_in_ = len(self.features)
-
-        self.selected_features = []
-        self.not_selected_features = self.features.copy()
-        self.ranking_ = pd.Series(
-            dtype="float64"
-        )  # pd.DataFrame(columns=['var_name', 'mrmr', 'relevancy', 'redundancy'])
-        self.redundancy_ = pd.Series(dtype="float64")
-        self.run_feature_selection()
-
-        # store the output in the sklearn flavour
-        self.relevance_ = self.relevance
-        self.ranking_ = pd.concat(
-            [self.ranking_, self.relevance_, self.redundancy_], axis=1
-        )
-        self.ranking_.columns = ["mrmr", "relevance", "redundancy"]
-        self.ranking_ = self.ranking_.iloc[: self.n_features_to_select, :]
-
-        # Set back the mrmr score to Inf for the first selected feature to avoid dividing by zero
-        self.ranking_.iloc[0, 0] = float("Inf")
-
-        self.selected_features_ = self.selected_features
-        self.support_ = np.asarray(
-            [x in self.selected_features for x in self.feature_names_in_]
-        )
-        self.not_selected_features_ = self.not_selected_features
-        return self
-
-    def transform(self, X):
-        """
-        Transform the data, returns a transformed version of `X`.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-
-        Returns
-        -------
-        X_new : ndarray array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    def fit_transform(self, X, y, sample_weight=None):
-        """
-        Fit to data, then transform it.
-        Fits transformer to `X` and `y` and optionally sample_weight
-        with optional parameters `fit_params`
-        and returns a transformed version of `X`.
-        
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            Target values (None for unsupervised transformations).
-        sample_weight :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            sample weight values.
-        **fit_params : dict
-            Additional fit parameters.
-            
-        Returns
-        -------
-        X_new : ndarray array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        return self.fit(X=X, y=y, sample_weight=sample_weight).transform(X)
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def _more_tags(self):
-        return {"allow_nan": True}
-
-    def select_next_feature(
-        self, not_selected_features, selected_features, relevance, redundancy
-    ):
-        score_numerator = relevance.loc[not_selected_features]
-
-        if len(selected_features) > 0:
-            last_selected_feature = selected_features[-1]
-
-            if self.only_same_domain:
-                not_selected_features_sub = [
-                    c
-                    for c in not_selected_features
-                    if c.split("_")[0] == last_selected_feature.split("_")[0]
-                ]
-            else:
-                not_selected_features_sub = not_selected_features
-
-            if not_selected_features_sub:
-                redundancy.loc[not_selected_features_sub, last_selected_feature] = (
-                    self.redundancy_func(
-                        target=last_selected_feature,
-                        features=not_selected_features_sub,
-                        **self.redundancy_args,
-                    )
-                    .fillna(FLOOR)
-                    .abs()
-                    .clip(FLOOR)
-                )
-                score_denominator = (
-                    redundancy.loc[not_selected_features, selected_features]
-                    .apply(self.denominator_func, axis=1)
-                    .replace(1.0, float("Inf"))
-                )
-
-            else:
-                score_denominator = pd.Series(1, index=self.features)
-
-        else:
-            score_denominator = pd.Series(1, index=self.features)
-
-        score = score_numerator / score_denominator
-        score = score.sort_values(ascending=False)
-        best_feature = score.index[score.argmax()]
-
-        return best_feature, score, score_denominator
-
-    def update_ranks(self, best_feature, score, score_denominator):
-        self.ranking_ = pd.concat(
-            [
-                self.ranking_,
-                pd.Series({best_feature: score.loc[best_feature]}, dtype="float64"),
-            ]
-        )
-        self.redundancy_ = pd.concat(
-            [
-                self.redundancy_,
-                pd.Series(
-                    {best_feature: score_denominator.loc[best_feature]},
-                    dtype="float64",
-                ),
-            ]
-        )
-        # the first selected feature has a default denominator (redundancy) = 1 to avoid dividing by zero
-        # I set it back to zero
-        self.redundancy_ = self.redundancy_.replace(1.0, 0.0)
-        self.selected_features.append(best_feature)
-        self.not_selected_features.remove(best_feature)
-
-    def run_feature_selection(self):
-        for i in tqdm(range(self.n_features_to_select), disable=not self.show_progress):
-            best_feature, score, score_denominator = self.select_next_feature(
-                self.not_selected_features,
-                self.selected_features,
-                self.relevance,
-                self.redundancy,
-            )
-            self.update_ranks(best_feature, score, score_denominator)
+"""MRMR Feature Selection Module
+
+This module provides MinRedundancyMaxRelevance (MRMR) feature selection for classification or regression tasks. 
+In a classification task, the target should be of object or pandas category dtype, while in a regression task, 
+the target should be of numpy categorical dtype. The predictors can be categorical or numerical without requiring encoding, 
+as the appropriate method (correlation, correlation ratio, or Theil's U) will be automatically selected based on the data type.
+
+Module Structure:
+-----------------
+- ``MinRedundancyMaxRelevance``: MRMR feature selection class for classification or regression tasks.
+"""
+
+import functools
+import numpy as np
+import pandas as pd
+from sklearn.base import BaseEstimator
+from sklearn.utils.validation import check_is_fitted
+from tqdm.auto import tqdm
+from sklearn.feature_selection._base import SelectorMixin
+from ..association import (
+    f_stat_classification_parallel,
+    f_stat_regression_parallel,
+    association_series,
+)
+
+FLOOR = 0.001
+
+
+class MinRedundancyMaxRelevance(SelectorMixin, BaseEstimator):
+    """MRMR feature selection for a classification or a regression task
+    For a classification task, the target should be of object or pandas category
+    dtype. For a regression task, the target should be of numpy categorical dtype.
+    The predictors can be categorical or numerical, there is no encoding required.
+    The dtype will be automatically detected and the right method applied (either
+    correlation, correlation ration or Theil's U)
+
+
+    Parameters
+    ----------
+    n_features_to_select: int
+        Number of features to select.
+    relevance_func: callable, optional
+        relevance function having arguments "X", "y", "sample_weight" and returning a pd.Series
+        containing a score of relevance for each feature
+    redundancy: callable, optional
+        Redundancy method.
+        If callable, it should take "X", "sample_weight" as input and return a pandas.Series
+        containing a score of redundancy for each feature.
+    denominator: str or callable (optional, default='mean')
+        Synthesis function to apply to the denominator of MRMR score.
+        If string, name of method. Supported: 'max', 'mean'.
+        If callable, it should take an iterable as input and return a scalar.
+    task: str
+        either "regression" or "classifiction"
+    only_same_domain: bool (optional, default=False)
+        If False, all the necessary correlation coefficients are computed.
+        If True, only features belonging to the same domain are compared.
+        Domain is defined by the string preceding the first underscore:
+        for instance "cusinfo_age" and "cusinfo_income" belong to the same domain, whereas "age" and "income" don't.
+    return_scores: bool (optional, default=False)
+        If False, only the list of selected features is returned.
+        If True, a tuple containing (list of selected features, relevance, redundancy) is returned.
+    n_jobs: int (optional, default=-1)
+        Maximum number of workers to use. Only used when relevance = "f" or redundancy = "corr".
+        If -1, use as many workers as min(cpu count, number of features).
+    show_progress: bool (optional, default=True)
+        If False, no progress bar is displayed.
+        If True, a TQDM progress bar shows the number of features processed.
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    ranking_ : pd.DataFrame
+        name and scores for the selected features
+    support_ : list of bool
+        the list of the selected X-columns
+    Example
+    -------
+    >>> from sklearn.datasets import make_classification, make_regression
+    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
+    >>> X = pd.DataFrame(X)
+    >>> y = pd.Series(y)
+    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
+    >>> X.columns = pred_name
+    >>> y.name = "target"
+    >>> fs_mrmr = MinRedundancyMaxRelevance(n_features_to_select=5,
+    >>>                  relevance_func=None,
+    >>>                  redundancy_func=None,
+    >>>                  task= "regression",#"classification",
+    >>>                  denominator_func=np.mean,
+    >>>                  only_same_domain=False,
+    >>>                  return_scores=False,
+    >>>                  show_progress=True)
+    >>> #fs_mrmr.fit(X=X, y=y.astype(str), sample_weight=None)
+    >>> fs_mrmr.fit(X=X, y=y, sample_weight=None)
+    """
+
+    def __init__(
+        self,
+        n_features_to_select,
+        relevance_func=None,
+        redundancy_func=None,
+        task="regression",
+        denominator_func=np.mean,
+        only_same_domain=False,
+        return_scores=False,
+        n_jobs=-1,
+        show_progress=True,
+    ):
+        self.n_features_to_select = n_features_to_select
+        self.relevance_func = relevance_func
+        self.redundancy_func = redundancy_func
+        self.denominator_func = denominator_func
+        self.only_same_domain = only_same_domain
+        self.return_scores = return_scores
+        self.show_progress = show_progress
+        self.n_jobs = n_jobs
+        self.task = task
+
+        if self.relevance_func is None:
+            if self.task == "regression":
+                self.relevance_func = functools.partial(
+                    f_stat_regression_parallel, n_jobs=self.n_jobs
+                )
+            else:
+                self.relevance_func = functools.partial(
+                    f_stat_classification_parallel, n_jobs=self.n_jobs
+                )
+
+        if self.redundancy_func is None:
+            self.redundancy_func = functools.partial(
+                association_series, n_jobs=self.n_jobs, normalize=True
+            )
+
+    def fit(self, X, y, sample_weight=None):
+        """fit the MRmr selector by learning the associations
+
+        Parameters
+        ----------
+        X : pd.DataFrame, shape (n_samples, n_features)
+            Data from which to compute variances, where `n_samples` is
+            the number of samples and `n_features` is the number of features.
+        y : any, default=None
+            Ignored. This parameter exists only for compatibility with
+            sklearn.pipeline.Pipeline.
+        sample_weight : pd.Series, optional, shape (n_samples,)
+            weights for computing the statistics (e.g. weighted average)
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
+        """
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+        else:
+            raise TypeError("X is not a pd.DataFrame")
+
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y)
+
+        y.name = "target"
+
+        target = y.copy()
+        if self.task == "classification":
+            target = target.astype("category")
+
+        self.relevance_args = {"X": X, "y": target, "sample_weight": sample_weight}
+        self.redundancy_args = {"X": X, "sample_weight": sample_weight}
+
+        self.relevance = self.relevance_func(**self.relevance_args)
+        self.features = self.relevance[~self.relevance.isna()].index.to_list()
+        self.relevance = self.relevance.loc[self.features]
+        self.redundancy = pd.DataFrame(
+            FLOOR, index=self.features, columns=self.features
+        )
+        self.n_features_to_select = min(self.n_features_to_select, len(self.features))
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+
+        self.n_features_in_ = len(self.features)
+
+        self.selected_features = []
+        self.not_selected_features = self.features.copy()
+        self.ranking_ = pd.Series(
+            dtype="float64"
+        )  # pd.DataFrame(columns=['var_name', 'mrmr', 'relevancy', 'redundancy'])
+        self.redundancy_ = pd.Series(dtype="float64")
+        self.run_feature_selection()
+
+        # store the output in the sklearn flavour
+        self.relevance_ = self.relevance
+        self.ranking_ = pd.concat(
+            [self.ranking_, self.relevance_, self.redundancy_], axis=1
+        )
+        self.ranking_.columns = ["mrmr", "relevance", "redundancy"]
+        self.ranking_ = self.ranking_.iloc[: self.n_features_to_select, :]
+
+        # Set back the mrmr score to Inf for the first selected feature to avoid dividing by zero
+        self.ranking_.iloc[0, 0] = float("Inf")
+
+        self.selected_features_ = self.selected_features
+        self.support_ = np.asarray(
+            [x in self.selected_features for x in self.feature_names_in_]
+        )
+        self.not_selected_features_ = self.not_selected_features
+        return self
+
+    def transform(self, X):
+        """
+        Transform the data, returns a transformed version of `X`.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    def fit_transform(self, X, y, sample_weight=None):
+        """
+        Fit to data, then transform it.
+        Fits transformer to `X` and `y` and optionally sample_weight
+        with optional parameters `fit_params`
+        and returns a transformed version of `X`.
+        
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            Target values (None for unsupervised transformations).
+        sample_weight :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            sample weight values.
+        **fit_params : dict
+            Additional fit parameters.
+            
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        return self.fit(X=X, y=y, sample_weight=sample_weight).transform(X)
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def _more_tags(self):
+        return {"allow_nan": True}
+
+    def select_next_feature(
+        self, not_selected_features, selected_features, relevance, redundancy
+    ):
+        score_numerator = relevance.loc[not_selected_features]
+
+        if len(selected_features) > 0:
+            last_selected_feature = selected_features[-1]
+
+            if self.only_same_domain:
+                not_selected_features_sub = [
+                    c
+                    for c in not_selected_features
+                    if c.split("_")[0] == last_selected_feature.split("_")[0]
+                ]
+            else:
+                not_selected_features_sub = not_selected_features
+
+            if not_selected_features_sub:
+                redundancy.loc[not_selected_features_sub, last_selected_feature] = (
+                    self.redundancy_func(
+                        target=last_selected_feature,
+                        features=not_selected_features_sub,
+                        **self.redundancy_args,
+                    )
+                    .fillna(FLOOR)
+                    .abs()
+                    .clip(FLOOR)
+                )
+                score_denominator = (
+                    redundancy.loc[not_selected_features, selected_features]
+                    .apply(self.denominator_func, axis=1)
+                    .replace(1.0, float("Inf"))
+                )
+
+            else:
+                score_denominator = pd.Series(1, index=self.features)
+
+        else:
+            score_denominator = pd.Series(1, index=self.features)
+
+        score = score_numerator / score_denominator
+        score = score.sort_values(ascending=False)
+        best_feature = score.index[score.argmax()]
+
+        return best_feature, score, score_denominator
+
+    def update_ranks(self, best_feature, score, score_denominator):
+        self.ranking_ = pd.concat(
+            [
+                self.ranking_,
+                pd.Series({best_feature: score.loc[best_feature]}, dtype="float64"),
+            ]
+        )
+        self.redundancy_ = pd.concat(
+            [
+                self.redundancy_,
+                pd.Series(
+                    {best_feature: score_denominator.loc[best_feature]},
+                    dtype="float64",
+                ),
+            ]
+        )
+        # the first selected feature has a default denominator (redundancy) = 1 to avoid dividing by zero
+        # I set it back to zero
+        self.redundancy_ = self.redundancy_.replace(1.0, 0.0)
+        self.selected_features.append(best_feature)
+        self.not_selected_features.remove(best_feature)
+
+    def run_feature_selection(self):
+        for i in tqdm(range(self.n_features_to_select), disable=not self.show_progress):
+            best_feature, score, score_denominator = self.select_next_feature(
+                self.not_selected_features,
+                self.selected_features,
+                self.relevance,
+                self.redundancy,
+            )
+            self.update_ranks(best_feature, score, score_denominator)
```

### Comparing `arfs-2.0.4/src/arfs/feature_selection/unsupervised.py` & `arfs-2.0.5/src/arfs/feature_selection/unsupervised.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,452 +1,452 @@
-"""Unsupervised Feature Selection
-
-This module provides selectors using unsupervised statistics and a threshold
-
-Module Structure:
------------------
-- ``MissingValueThreshold``: child class of the ``BaseThresholdSelector``, filter out columns with too many missing values
-- ``UniqueValuesThreshold`` child of the ``BaseThresholdSelector``, filter out columns with zero variance
-- ``CardinalityThreshold`` child of the ``BaseThresholdSelector``, filter out categorical columns with too many levels  
-- ``CollinearityThreshold`` child of the ``BaseThresholdSelector``, filter out collinear columns
-"""
-
-from __future__ import print_function
-from tqdm.auto import trange
-
-# pandas
-import pandas as pd
-
-# numpy
-import numpy as np
-
-# sklearn
-from sklearn.utils.validation import check_is_fitted
-from sklearn.base import BaseEstimator
-from sklearn.feature_selection._base import SelectorMixin
-
-# ARFS
-from .base import BaseThresholdSelector
-from ..utils import create_dtype_dict
-from ..association import association_matrix, xy_to_matrix, plot_association_matrix
-from ..preprocessing import OrdinalEncoderPandas
-
-
-# fix random seed for reproducibility
-np.random.seed(7)
-
-
-def _missing_ratio(df):
-    if not isinstance(df, pd.DataFrame):
-        raise TypeError("df should be a pandas DataFrame")
-    numeric_columns = df.select_dtypes(np.number).columns
-    n_samples = len(df)
-
-    missing_counts = {}
-    for column in df.columns:
-        if column in numeric_columns:
-            missing_counts[column] = (
-                df[column].isnull().sum() + np.isinf(df[column]).sum()
-            ) / n_samples
-        else:
-            missing_counts[column] = df[column].isnull().sum() / n_samples
-    return pd.Series(missing_counts)
-
-
-class MissingValueThreshold(BaseThresholdSelector):
-    """Feature selector that removes all high missing percentage features.
-    This feature selection algorithm looks only at the features (X),
-    not the desired outputs (y), and can thus be used for unsupervised learning.
-
-
-    Parameters
-    ----------
-    threshold: float, default = .05
-        Features with a training-set missing larger than this threshold will be removed.
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    support_ : list of bool
-        the list of the selected X-columns
-    selected_features_ : list of str
-        the list of names of selected features
-    not_selected_features_ : list of str
-        the list of names of rejected features
-
-    Example
-    -------
-    >>> from sklearn.datasets import make_classification, make_regression
-    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
-    >>> X = pd.DataFrame(X)
-    >>> y = pd.Series(y)
-    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
-    >>> X.columns = pred_name
-    >>> selector = MissingValueThreshold(0.05)
-    >>> selector.fit_transform(X)
-    """
-
-    def __init__(self, threshold=0.05):
-        super().__init__(
-            threshold=threshold,
-            statistic_fn=_missing_ratio,
-            greater_than_threshold=False,
-        )
-
-
-def _pandas_count_unique_values(X):
-    if not isinstance(X, pd.DataFrame):
-        raise TypeError("X should be a pandas DataFrame")
-    return X.nunique()
-
-
-class UniqueValuesThreshold(BaseThresholdSelector):
-    """Feature selector that removes all features with zero variance (single unique values)
-    or remove columns with less unique values than threshold
-    This feature selection algorithm looks only at the features (X),
-    not the desired outputs (y), and can thus be used for unsupervised learning.
-
-    Parameters
-    ----------
-    threshold: int, default = 1
-        Features with a training-set missing larger than this threshold will be removed.
-        The thresold should be >= 1
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    support_ : list of bool
-        the list of the selected X-columns
-    selected_features_ : list of str
-        the list of names of selected features
-    not_selected_features_ : list of str
-        the list of names of rejected features
-
-    Example
-    -------
-    >>> from sklearn.datasets import make_classification, make_regression
-    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
-    >>> X = pd.DataFrame(X)
-    >>> y = pd.Series(y)
-    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
-    >>> X.columns = pred_name
-    >>> selector = UniqueValuesThreshold(1)
-    >>> selector.fit_transform(X)
-    """
-
-    def __init__(self, threshold=1):
-        super().__init__(
-            threshold=threshold,
-            statistic_fn=_pandas_count_unique_values,
-            greater_than_threshold=True,
-        )
-
-
-def _pandas_count_unique_values_cat_features(X):
-    """
-    Counts the number of unique values in categorical features of a pandas DataFrame.
-
-    Parameters
-    ----------
-    X : pandas DataFrame
-        The input data.
-
-    Returns
-    -------
-    pandas Series
-        The number of unique values in each categorical feature.
-
-    Raises
-    ------
-    TypeError
-        If the input data is not a pandas DataFrame.
-    """
-    if not isinstance(X, pd.DataFrame):
-        raise TypeError("X should be a pandas DataFrame")
-    count_series = pd.Series(data=0, index=X.columns)
-    dtype_dic = create_dtype_dict(X, dic_keys="dtypes")
-    for c in dtype_dic["cat"]:
-        count_series[c] = X[c].nunique()
-    return count_series
-
-
-class CardinalityThreshold(BaseThresholdSelector):
-    """Feature selector that removes all categorical features with more unique values than threshold
-    This feature selection algorithm looks only at the features (X),
-    not the desired outputs (y), and can thus be used for unsupervised learning.
-
-    Parameters
-    ----------
-    threshold: int, default = 1000
-        Features with a training-set missing larger than this threshold will be removed.
-        The thresold should be >= 1
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    support_ : list of bool
-        the list of the selected X-columns
-    selected_features_ : list of str
-        the list of names of selected features
-    not_selected_features_ : list of str
-        the list of names of rejected features
-
-    Example
-    -------
-    >>> from sklearn.datasets import make_classification, make_regression
-    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
-    >>> X = pd.DataFrame(X)
-    >>> y = pd.Series(y)
-    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
-    >>> X.columns = pred_name
-    >>> selector = CardinalityThreshold(100)
-    >>> selector.fit_transform(X)
-    """
-
-    def __init__(self, threshold=1000):
-        super().__init__(
-            threshold=threshold,
-            statistic_fn=_pandas_count_unique_values_cat_features,
-            greater_than_threshold=False,
-        )
-
-
-class CollinearityThreshold(SelectorMixin, BaseEstimator):
-    """Feature selector that removes collinear features.
-    This feature selection algorithm looks only at the features (X),
-    not the desired outputs (y), and can thus be used for unsupervised learning.
-    It computes the association between features (continuous or categorical),
-    store the pairs of collinear features and remove one of them for all pairs having
-    an association value above the threshold.
-
-    The association measures are the Spearman correlation coefficient, correlation ratio
-    and Theil's U. The association matrix is not necessarily symmetrical.
-
-    By changing the method to "correlation", data will be encoded as integer
-    and the Spearman correlation coefficient will be used instead. Faster but not
-    a best practice because the categorical variables are considered as numeric.
-
-    Parameters
-    ----------
-    threshold : float, default = .8
-        Features with a training-set missing larger than this threshold will be removed
-        The thresold should be > 0 and =< 1
-    method : str, default = "association"
-        method for computing the association matrix. Either "association" or "correlation".
-        Correlation leads to encoding of categorical variables as numeric
-    n_jobs : int, default = -1
-        the number of threads, -1 uses all the threads for computating the association matrix
-    nom_nom_assoc : str or callable, default = "theil"
-        the categorical-categorical association measure, by default Theil's U, not symmetrical!
-    num_num_assoc : str or callable, default = "spearman"
-        the numeric-numeric association measure
-    nom_num_assoc : str or callable, default = "correlation_ratio"
-        the numeric-categorical association measure
-
-    Returns
-    -------
-    selected_features: list of str
-        List of selected features.
-
-    Attributes
-    ----------
-    n_features_in_ : int
-        number of input predictors
-    assoc_matrix_ : pd.DataFrame
-        the square association matrix
-    collinearity_summary_ : pd.DataFrame
-        the pairs of collinear features and the association values
-    support_ : list of bool
-        the list of the selected X-columns
-    selected_features_ : list of str
-        the list of names of selected features
-    not_selected_features_ : list of str
-        the list of names of rejected features
-
-    Example
-    -------
-    >>> from sklearn.datasets import make_classification, make_regression
-    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
-    >>> X = pd.DataFrame(X)
-    >>> y = pd.Series(y)
-    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
-    >>> X.columns = pred_name
-    >>> selector = CollinearityThreshold(threshold=0.75)
-    >>> selector.fit_transform(X)
-    """
-
-    def __init__(
-        self,
-        threshold=0.80,
-        method="association",
-        n_jobs=-1,
-        nom_nom_assoc="theil",
-        num_num_assoc="spearman",
-        nom_num_assoc="correlation_ratio",
-    ):
-        self.threshold = threshold
-        self.method = method
-        self.n_jobs = n_jobs
-        self.nom_nom_assoc = nom_nom_assoc
-        self.num_num_assoc = num_num_assoc
-        self.nom_num_assoc = nom_num_assoc
-
-        if self.method not in ["association", "correlation"]:
-            raise ValueError("``method`` should be 'association' or 'correlation'")
-
-        if (self.threshold > 1.0) or (self.threshold < 0.0):
-            raise ValueError("``threshold`` should be larger than 0 and smaller than 1")
-
-    def fit(self, X, y=None, sample_weight=None):
-        """Learn empirical associtions from X.
-
-        Parameters
-        ----------
-        X : pd.DataFrame, shape (n_samples, n_features)
-            Data from which to compute variances, where `n_samples` is
-            the number of samples and `n_features` is the number of features.
-        y : any, default=None
-            Ignored. This parameter exists only for compatibility with
-            sklearn.pipeline.Pipeline.
-        sample_weight : pd.Series, optional, shape (n_samples,)
-            weights for computing the statistics (e.g. weighted average)
-
-        Returns
-        -------
-        self : object
-            Returns the instance itself.
-        """
-
-        if isinstance(X, pd.DataFrame):
-            self.feature_names_in_ = X.columns.to_numpy()
-        else:
-            raise TypeError("X is not a dataframe")
-
-        self.suffix_dic = create_dtype_dict(X)
-
-        if self.method == "correlation":
-            encoder = OrdinalEncoderPandas()
-            X = encoder.fit_transform(X)
-            del encoder
-
-        assoc_matrix = association_matrix(
-            X=X,
-            sample_weight=sample_weight,
-            n_jobs=self.n_jobs,
-            nom_nom_assoc=self.nom_nom_assoc,
-            num_num_assoc=self.num_num_assoc,
-            nom_num_assoc=self.nom_num_assoc,
-        )
-        self.assoc_matrix_ = xy_to_matrix(assoc_matrix)
-
-        to_drop = _recursive_collinear_elimination(self.assoc_matrix_, self.threshold)
-
-        self.support_ = np.asarray(
-            [True if c not in to_drop else False for c in X.columns]
-        )
-        self.selected_features_ = self.feature_names_in_[self.support_]
-        self.not_selected_features_ = self.feature_names_in_[~self.support_]
-
-        return self
-
-    def _get_support_mask(self):
-        check_is_fitted(self)
-
-        return self.support_
-
-    def transform(self, X):
-        if not isinstance(X, pd.DataFrame):
-            raise TypeError("X is not a dataframe")
-        return X[self.selected_features_]
-
-    def _more_tags(self):
-        return {"allow_nan": True}
-
-    def plot_association(
-        self, ax=None, cmap="PuOr", figsize=None, cbar_kw=None, imgshow_kw=None
-    ):
-        """plot_association plots the association matrix
-
-        Parameters
-        ----------
-        ax : matplotlib.axes.Axes, optional
-            the mpl axes if the figure object exists already, by default None
-        cmap : str, optional
-            colormap name, by default "PuOr"
-        figsize : tuple of float, optional
-            figure size, by default None
-        cbar_kw : dict, optional
-            colorbar kwargs, by default None
-        imgshow_kw : dict, optional
-            imgshow kwargs, by default None
-        """
-
-        if figsize is None:
-            figsize = (self.assoc_matrix_.shape[0] / 3, self.assoc_matrix_.shape[0] / 3)
-
-        f, ax = plot_association_matrix(
-            assoc_mat=self.assoc_matrix_,
-            suffix_dic=self.suffix_dic,
-            ax=ax,
-            cmap=cmap,
-            cbarlabel="association value",
-            figsize=figsize,
-            show=True,
-            cbar_kw=cbar_kw,
-            imgshow_kw=imgshow_kw,
-        )
-
-        return f
-
-
-def _most_collinear(association_matrix, threshold):
-    cols_to_drop = [
-        column
-        for column in association_matrix.columns
-        if any(association_matrix.loc[:, column].abs() > threshold)
-    ]
-    rows_to_drop = [
-        row
-        for row in association_matrix.index
-        if any(association_matrix.loc[row, :].abs() > threshold)
-    ]
-    to_drop = list(set(cols_to_drop).union(set(rows_to_drop)))
-    most_collinear_series = (
-        association_matrix[to_drop].abs().sum(axis=1).sort_values(ascending=False)
-    )
-    most_collinear_series += (
-        association_matrix[to_drop].abs().sum(axis=0).sort_values(ascending=False)
-    )
-    most_collinear_series /= 2
-    return most_collinear_series.index[0], to_drop
-
-
-def _recursive_collinear_elimination(association_matrix, threshold):
-    dum = association_matrix.copy()
-    most_collinear_features = []
-    most_collinear_feature, to_drop = _most_collinear(association_matrix, threshold)
-    most_collinear_features.append(most_collinear_feature)
-    dum = dum.drop(columns=most_collinear_feature, index=most_collinear_feature)
-
-    while len(to_drop) > 1:
-        most_collinear_feature, to_drop = _most_collinear(dum, 0.75)
-        most_collinear_features.append(most_collinear_feature)
-        dum = dum.drop(columns=most_collinear_feature, index=most_collinear_feature)
-    return most_collinear_features
+"""Unsupervised Feature Selection
+
+This module provides selectors using unsupervised statistics and a threshold
+
+Module Structure:
+-----------------
+- ``MissingValueThreshold``: child class of the ``BaseThresholdSelector``, filter out columns with too many missing values
+- ``UniqueValuesThreshold`` child of the ``BaseThresholdSelector``, filter out columns with zero variance
+- ``CardinalityThreshold`` child of the ``BaseThresholdSelector``, filter out categorical columns with too many levels  
+- ``CollinearityThreshold`` child of the ``BaseThresholdSelector``, filter out collinear columns
+"""
+
+from __future__ import print_function
+from tqdm.auto import trange
+
+# pandas
+import pandas as pd
+
+# numpy
+import numpy as np
+
+# sklearn
+from sklearn.utils.validation import check_is_fitted
+from sklearn.base import BaseEstimator
+from sklearn.feature_selection._base import SelectorMixin
+
+# ARFS
+from .base import BaseThresholdSelector
+from ..utils import create_dtype_dict
+from ..association import association_matrix, xy_to_matrix, plot_association_matrix
+from ..preprocessing import OrdinalEncoderPandas
+
+
+# fix random seed for reproducibility
+np.random.seed(7)
+
+
+def _missing_ratio(df):
+    if not isinstance(df, pd.DataFrame):
+        raise TypeError("df should be a pandas DataFrame")
+    numeric_columns = df.select_dtypes(np.number).columns
+    n_samples = len(df)
+
+    missing_counts = {}
+    for column in df.columns:
+        if column in numeric_columns:
+            missing_counts[column] = (
+                df[column].isnull().sum() + np.isinf(df[column]).sum()
+            ) / n_samples
+        else:
+            missing_counts[column] = df[column].isnull().sum() / n_samples
+    return pd.Series(missing_counts)
+
+
+class MissingValueThreshold(BaseThresholdSelector):
+    """Feature selector that removes all high missing percentage features.
+    This feature selection algorithm looks only at the features (X),
+    not the desired outputs (y), and can thus be used for unsupervised learning.
+
+
+    Parameters
+    ----------
+    threshold: float, default = .05
+        Features with a training-set missing larger than this threshold will be removed.
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    support_ : list of bool
+        the list of the selected X-columns
+    selected_features_ : list of str
+        the list of names of selected features
+    not_selected_features_ : list of str
+        the list of names of rejected features
+
+    Example
+    -------
+    >>> from sklearn.datasets import make_classification, make_regression
+    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
+    >>> X = pd.DataFrame(X)
+    >>> y = pd.Series(y)
+    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
+    >>> X.columns = pred_name
+    >>> selector = MissingValueThreshold(0.05)
+    >>> selector.fit_transform(X)
+    """
+
+    def __init__(self, threshold=0.05):
+        super().__init__(
+            threshold=threshold,
+            statistic_fn=_missing_ratio,
+            greater_than_threshold=False,
+        )
+
+
+def _pandas_count_unique_values(X):
+    if not isinstance(X, pd.DataFrame):
+        raise TypeError("X should be a pandas DataFrame")
+    return X.nunique()
+
+
+class UniqueValuesThreshold(BaseThresholdSelector):
+    """Feature selector that removes all features with zero variance (single unique values)
+    or remove columns with less unique values than threshold
+    This feature selection algorithm looks only at the features (X),
+    not the desired outputs (y), and can thus be used for unsupervised learning.
+
+    Parameters
+    ----------
+    threshold: int, default = 1
+        Features with a training-set missing larger than this threshold will be removed.
+        The thresold should be >= 1
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    support_ : list of bool
+        the list of the selected X-columns
+    selected_features_ : list of str
+        the list of names of selected features
+    not_selected_features_ : list of str
+        the list of names of rejected features
+
+    Example
+    -------
+    >>> from sklearn.datasets import make_classification, make_regression
+    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
+    >>> X = pd.DataFrame(X)
+    >>> y = pd.Series(y)
+    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
+    >>> X.columns = pred_name
+    >>> selector = UniqueValuesThreshold(1)
+    >>> selector.fit_transform(X)
+    """
+
+    def __init__(self, threshold=1):
+        super().__init__(
+            threshold=threshold,
+            statistic_fn=_pandas_count_unique_values,
+            greater_than_threshold=True,
+        )
+
+
+def _pandas_count_unique_values_cat_features(X):
+    """
+    Counts the number of unique values in categorical features of a pandas DataFrame.
+
+    Parameters
+    ----------
+    X : pandas DataFrame
+        The input data.
+
+    Returns
+    -------
+    pandas Series
+        The number of unique values in each categorical feature.
+
+    Raises
+    ------
+    TypeError
+        If the input data is not a pandas DataFrame.
+    """
+    if not isinstance(X, pd.DataFrame):
+        raise TypeError("X should be a pandas DataFrame")
+    count_series = pd.Series(data=0, index=X.columns)
+    dtype_dic = create_dtype_dict(X, dic_keys="dtypes")
+    for c in dtype_dic["cat"]:
+        count_series[c] = X[c].nunique()
+    return count_series
+
+
+class CardinalityThreshold(BaseThresholdSelector):
+    """Feature selector that removes all categorical features with more unique values than threshold
+    This feature selection algorithm looks only at the features (X),
+    not the desired outputs (y), and can thus be used for unsupervised learning.
+
+    Parameters
+    ----------
+    threshold: int, default = 1000
+        Features with a training-set missing larger than this threshold will be removed.
+        The thresold should be >= 1
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    support_ : list of bool
+        the list of the selected X-columns
+    selected_features_ : list of str
+        the list of names of selected features
+    not_selected_features_ : list of str
+        the list of names of rejected features
+
+    Example
+    -------
+    >>> from sklearn.datasets import make_classification, make_regression
+    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
+    >>> X = pd.DataFrame(X)
+    >>> y = pd.Series(y)
+    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
+    >>> X.columns = pred_name
+    >>> selector = CardinalityThreshold(100)
+    >>> selector.fit_transform(X)
+    """
+
+    def __init__(self, threshold=1000):
+        super().__init__(
+            threshold=threshold,
+            statistic_fn=_pandas_count_unique_values_cat_features,
+            greater_than_threshold=False,
+        )
+
+
+class CollinearityThreshold(SelectorMixin, BaseEstimator):
+    """Feature selector that removes collinear features.
+    This feature selection algorithm looks only at the features (X),
+    not the desired outputs (y), and can thus be used for unsupervised learning.
+    It computes the association between features (continuous or categorical),
+    store the pairs of collinear features and remove one of them for all pairs having
+    an association value above the threshold.
+
+    The association measures are the Spearman correlation coefficient, correlation ratio
+    and Theil's U. The association matrix is not necessarily symmetrical.
+
+    By changing the method to "correlation", data will be encoded as integer
+    and the Spearman correlation coefficient will be used instead. Faster but not
+    a best practice because the categorical variables are considered as numeric.
+
+    Parameters
+    ----------
+    threshold : float, default = .8
+        Features with a training-set missing larger than this threshold will be removed
+        The thresold should be > 0 and =< 1
+    method : str, default = "association"
+        method for computing the association matrix. Either "association" or "correlation".
+        Correlation leads to encoding of categorical variables as numeric
+    n_jobs : int, default = -1
+        the number of threads, -1 uses all the threads for computating the association matrix
+    nom_nom_assoc : str or callable, default = "theil"
+        the categorical-categorical association measure, by default Theil's U, not symmetrical!
+    num_num_assoc : str or callable, default = "spearman"
+        the numeric-numeric association measure
+    nom_num_assoc : str or callable, default = "correlation_ratio"
+        the numeric-categorical association measure
+
+    Returns
+    -------
+    selected_features: list of str
+        List of selected features.
+
+    Attributes
+    ----------
+    n_features_in_ : int
+        number of input predictors
+    assoc_matrix_ : pd.DataFrame
+        the square association matrix
+    collinearity_summary_ : pd.DataFrame
+        the pairs of collinear features and the association values
+    support_ : list of bool
+        the list of the selected X-columns
+    selected_features_ : list of str
+        the list of names of selected features
+    not_selected_features_ : list of str
+        the list of names of rejected features
+
+    Example
+    -------
+    >>> from sklearn.datasets import make_classification, make_regression
+    >>> X, y = make_regression(n_samples = 1000, n_features = 50, n_informative = 5, shuffle=False) # , n_redundant = 5
+    >>> X = pd.DataFrame(X)
+    >>> y = pd.Series(y)
+    >>> pred_name = [f"pred_{i}" for i in range(X.shape[1])]
+    >>> X.columns = pred_name
+    >>> selector = CollinearityThreshold(threshold=0.75)
+    >>> selector.fit_transform(X)
+    """
+
+    def __init__(
+        self,
+        threshold=0.80,
+        method="association",
+        n_jobs=-1,
+        nom_nom_assoc="theil",
+        num_num_assoc="spearman",
+        nom_num_assoc="correlation_ratio",
+    ):
+        self.threshold = threshold
+        self.method = method
+        self.n_jobs = n_jobs
+        self.nom_nom_assoc = nom_nom_assoc
+        self.num_num_assoc = num_num_assoc
+        self.nom_num_assoc = nom_num_assoc
+
+        if self.method not in ["association", "correlation"]:
+            raise ValueError("``method`` should be 'association' or 'correlation'")
+
+        if (self.threshold > 1.0) or (self.threshold < 0.0):
+            raise ValueError("``threshold`` should be larger than 0 and smaller than 1")
+
+    def fit(self, X, y=None, sample_weight=None):
+        """Learn empirical associtions from X.
+
+        Parameters
+        ----------
+        X : pd.DataFrame, shape (n_samples, n_features)
+            Data from which to compute variances, where `n_samples` is
+            the number of samples and `n_features` is the number of features.
+        y : any, default=None
+            Ignored. This parameter exists only for compatibility with
+            sklearn.pipeline.Pipeline.
+        sample_weight : pd.Series, optional, shape (n_samples,)
+            weights for computing the statistics (e.g. weighted average)
+
+        Returns
+        -------
+        self : object
+            Returns the instance itself.
+        """
+
+        if isinstance(X, pd.DataFrame):
+            self.feature_names_in_ = X.columns.to_numpy()
+        else:
+            raise TypeError("X is not a dataframe")
+
+        self.suffix_dic = create_dtype_dict(X)
+
+        if self.method == "correlation":
+            encoder = OrdinalEncoderPandas()
+            X = encoder.fit_transform(X)
+            del encoder
+
+        assoc_matrix = association_matrix(
+            X=X,
+            sample_weight=sample_weight,
+            n_jobs=self.n_jobs,
+            nom_nom_assoc=self.nom_nom_assoc,
+            num_num_assoc=self.num_num_assoc,
+            nom_num_assoc=self.nom_num_assoc,
+        )
+        self.assoc_matrix_ = xy_to_matrix(assoc_matrix)
+
+        to_drop = _recursive_collinear_elimination(self.assoc_matrix_, self.threshold)
+
+        self.support_ = np.asarray(
+            [True if c not in to_drop else False for c in X.columns]
+        )
+        self.selected_features_ = self.feature_names_in_[self.support_]
+        self.not_selected_features_ = self.feature_names_in_[~self.support_]
+
+        return self
+
+    def _get_support_mask(self):
+        check_is_fitted(self)
+
+        return self.support_
+
+    def transform(self, X):
+        if not isinstance(X, pd.DataFrame):
+            raise TypeError("X is not a dataframe")
+        return X[self.selected_features_]
+
+    def _more_tags(self):
+        return {"allow_nan": True}
+
+    def plot_association(
+        self, ax=None, cmap="PuOr", figsize=None, cbar_kw=None, imgshow_kw=None
+    ):
+        """plot_association plots the association matrix
+
+        Parameters
+        ----------
+        ax : matplotlib.axes.Axes, optional
+            the mpl axes if the figure object exists already, by default None
+        cmap : str, optional
+            colormap name, by default "PuOr"
+        figsize : tuple of float, optional
+            figure size, by default None
+        cbar_kw : dict, optional
+            colorbar kwargs, by default None
+        imgshow_kw : dict, optional
+            imgshow kwargs, by default None
+        """
+
+        if figsize is None:
+            figsize = (self.assoc_matrix_.shape[0] / 3, self.assoc_matrix_.shape[0] / 3)
+
+        f, ax = plot_association_matrix(
+            assoc_mat=self.assoc_matrix_,
+            suffix_dic=self.suffix_dic,
+            ax=ax,
+            cmap=cmap,
+            cbarlabel="association value",
+            figsize=figsize,
+            show=True,
+            cbar_kw=cbar_kw,
+            imgshow_kw=imgshow_kw,
+        )
+
+        return f
+
+
+def _most_collinear(association_matrix, threshold):
+    cols_to_drop = [
+        column
+        for column in association_matrix.columns
+        if any(association_matrix.loc[:, column].abs() > threshold)
+    ]
+    rows_to_drop = [
+        row
+        for row in association_matrix.index
+        if any(association_matrix.loc[row, :].abs() > threshold)
+    ]
+    to_drop = list(set(cols_to_drop).union(set(rows_to_drop)))
+    most_collinear_series = (
+        association_matrix[to_drop].abs().sum(axis=1).sort_values(ascending=False)
+    )
+    most_collinear_series += (
+        association_matrix[to_drop].abs().sum(axis=0).sort_values(ascending=False)
+    )
+    most_collinear_series /= 2
+    return most_collinear_series.index[0], to_drop
+
+
+def _recursive_collinear_elimination(association_matrix, threshold):
+    dum = association_matrix.copy()
+    most_collinear_features = []
+    most_collinear_feature, to_drop = _most_collinear(association_matrix, threshold)
+    most_collinear_features.append(most_collinear_feature)
+    dum = dum.drop(columns=most_collinear_feature, index=most_collinear_feature)
+
+    while len(to_drop) > 1:
+        most_collinear_feature, to_drop = _most_collinear(dum, 0.75)
+        most_collinear_features.append(most_collinear_feature)
+        dum = dum.drop(columns=most_collinear_feature, index=most_collinear_feature)
+    return most_collinear_features
```

### Comparing `arfs-2.0.4/src/arfs/gbm.py` & `arfs-2.0.5/src/arfs/gbm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,610 +1,604 @@
-"""GBM Wrapper
-
-This module offers a class to train base LightGBM and CatBoost models, with early stopping as the default behavior. 
-The target variable can be finite discrete (classification) or continuous (regression). 
-Additionally, the model allows boosting from an initial score (also known as a baseline for CatBoost) and accepts sample weights as input.
-
-Module Structure:
------------------
-- ``GradientBoosting``: main class to train a lightGBM  or catboost with early stopping
-
-"""
-
-from sklearn.model_selection import (
-    ShuffleSplit,
-    StratifiedShuffleSplit,
-    GroupShuffleSplit,
-)
-import lightgbm as lgb
-from lightgbm import early_stopping, log_evaluation, record_evaluation
-import pandas as pd
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-import numpy as np
-import joblib
-from datetime import date
-import warnings
-import gc
-import os
-from pathlib import Path
-from arfs.utils import create_dtype_dict
-
-QUAL_COLORS = [
-    (0.188235, 0.635294, 0.854902),
-    (0.898039, 0.682353, 0.219608),
-    (0.988235, 0.309804, 0.188235),
-    (0.427451, 0.564706, 0.309804),
-]
-BCKGRND_COLOR = "#f5f5f5"
-
-MPL_PARAMS = {
-    "figure.figsize": (5, 3),
-    "axes.prop_cycle": plt.cycler(color=QUAL_COLORS),
-    "axes.facecolor": BCKGRND_COLOR,
-    "patch.edgecolor": BCKGRND_COLOR,
-    "figure.facecolor": BCKGRND_COLOR,
-    "axes.edgecolor": BCKGRND_COLOR,
-    "savefig.edgecolor": BCKGRND_COLOR,
-    "savefig.facecolor": BCKGRND_COLOR,
-    "grid.color": "#d2d2d2",
-    "lines.linewidth": 2,
-    "grid.alpha": 0.5,
-}
-
-
-class GradientBoosting:
-    """Performs the training of a base lightGBM/CatBoost using early stopping. It works for any of the
-    supported loss function (lightGBM/CatBoost), so for regression and classification you can use an instance of
-    this class. For the early stopping process, 20% of the data set is used and a fix seed is used for
-    reproducibility.
-
-    The resulting model can be saved at the desired location.
-    Last, you can pass relevant lightGBM/Catboost parameters and/or sample weights (exposure, etc.) if needed.
-
-    Init score of Booster to start from, if required (like for GLM residuals modelling using GBM).
-
-
-    Parameters
-    ----------
-    cat_feat : List[str], 'auto' or None,
-        The list of column names of the categorical predictors. For catboost, much more efficient if those columns
-        are of dtype pd.Categorical. For lightGBM, most of the time better to integer encode and NOT consider
-        them as categorical (set this parameter as None).
-    params : dict, default=None
-        you can pass the parameters that you want to lightGBM/Catboost, as long as they are valid.
-        If None, default parameters are passed.
-    stratified : bool, default=False
-        stratified shuffle split for the early stopping process. For classification problem, it guarantees
-        the same proportion
-    show_learning_curve : bool, default=True
-        if show or not the learning curve
-    verbose_eval : int, default=50
-        period for printing the train and validation results. If < 1, no output
-
-    Attributes
-    ----------
-    cat_feat : Union[str, List[str], None]
-        The list of categorical predictors after pre-processing
-    model_params : Dict
-        the dictionary of model parameters
-    learning_curve : plt.figure
-        the learning curve
-    is_init_score :  bool
-        boosted from an initial score or not
-    stratified : bool
-        either if stratified shuffle split was used or not for the early stopping process
-
-    Example
-    -------
-    >>> # set up the trainer
-    >>> save_path = "C:/Users/mtpl_bi_pp/base/"
-    >>> gbm_model = GradientBoosting(cat_feat='auto',
-    >>>                              stratified=False,
-    >>>                              params={
-    >>>                                 'objective': 'tweedie',
-    >>>                                 'tweedie_variance_power': 1.1
-    >>>                             })
-    >>>
-    >>> # train the model
-    >>> gbm_model.fit(X=X_tr,y=y_tr,sample_weight=exp_tr)
-    >>>
-    >>> # predict new values (test set)
-    >>> y_bt = gbm_model.predict(X_tt)
-    >>>
-    >>> # save the model
-    >>> gbm_model.save(save_path='C:/models/', name="my_fancy_model")
-
-    """
-
-    def __init__(
-        self,
-        cat_feat="auto",
-        params=None,
-        stratified=False,
-        show_learning_curve=True,
-        verbose_eval=50,
-        return_valid_features=False,
-    ):
-        self.model = None
-        self.cat_feat = cat_feat
-        self.model_params = None
-        self.params = params
-        self.learning_curve = None
-        self.is_init_score = False
-        self.stratified = stratified
-        self.show_learning_curve = show_learning_curve
-        self.verbose_eval = verbose_eval
-        self.return_valid_features = return_valid_features
-        self.valid_features = None
-
-    def __repr__(self):
-        s = (
-            "GradientBoosting(cat_feat={cat_feat},\n"
-            "                 params={params})".format(
-                cat_feat=self.cat_feat, params=self.params
-            )
-        )
-        return s
-
-    def fit(
-        self,
-        X,
-        y,
-        sample_weight=None,
-        init_score=None,
-        groups=None,
-    ):
-        """Fit the lightGBM/Catboost either using the python API and early stopping
-
-        Parameters
-        ----------
-        X : pd.DataFrame or np.ndarray
-            the predictors' matrix
-        y : pd.Series or np.ndarray
-            the target series/array
-        sample_weight : pd.Series or np.ndarray, optional
-            the sample_weight series/array, if relevant. If not None, it should be of the same length as the
-            target (default ``None``)
-        init_score : pd.Series or np.ndarray, optional
-            the initial score to boost from (series/array), if relevant. If not None,
-            it should be of the same length as the target (default ``None``)
-        groups : pd.Series or np.ndarray, optional
-            the groups (e.g. polID) for robust cross validation.
-            The same group will not appear in two different folds.
-
-        """
-        if (self.params is not None) and (not isinstance(self.params, dict)):
-            raise TypeError(
-                "params should be either None or a dictionary of lightgbm params"
-            )
-        elif (isinstance(self.params, dict)) and (
-            "objective" not in self.params.keys()
-        ):
-            raise KeyError("Provide the objective in the params dict")
-
-        if self.cat_feat == "auto":
-            dtypes_dic = create_dtype_dict(df=X, dic_keys="dtypes")
-            category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
-            self.cat_feat = category_cols if category_cols else None
-
-        if not isinstance(X, (pd.Series, pd.DataFrame)):
-            X = pd.DataFrame(X)
-
-        if not isinstance(y, pd.Series):
-            y = pd.Series(y)
-
-        if sample_weight is not None:
-            if not isinstance(sample_weight, pd.Series):
-                sample_weight = pd.Series(sample_weight)
-
-        if init_score is not None:
-            self.is_init_score = True
-            if not isinstance(init_score, pd.Series):
-                init_score = pd.Series(init_score)
-
-        output = _fit_early_stopped_lgb(
-            X=X,
-            y=y,
-            sample_weight=sample_weight,
-            params=self.params,
-            init_score=init_score,
-            cat_feat=self.cat_feat,
-            stratified=self.stratified,
-            groups=groups,
-            learning_curve=self.show_learning_curve,
-            verbose_eval=self.verbose_eval,
-            return_valid_features=self.return_valid_features,
-        )
-
-        if self.show_learning_curve:
-            if self.return_valid_features:
-                self.model, self.valid_features, self.learning_curve = (
-                    output[0],
-                    output[1],
-                    output[2],
-                )
-            else:
-                self.model, self.learning_curve = output[0], output[1]
-        else:
-            if self.return_valid_features:
-                self.model, self.valid_features = output[0], output[1]
-            else:
-                self.model = output
-
-        self.model_params = self.model.params
-
-    def predict(self, X, predict_proba=False):
-        """Predict the new values using the fitted model.
-
-        Parameters
-        ----------
-        X : pd.DataFrame or np.ndarray
-            the predictors' matrix
-        predict_proba : bool, default=False
-            returns probabilities (only for classification) (default ``False``)
-        """
-        if self.is_init_score:
-            raise AttributeError(
-                "The model is fitted from an initial score, use the `predict_raw` method instead\n"
-                "Please also check what is returned by the predicted method, for the raw version\n"
-                "you might have to apply `exp`"
-            )
-
-        obj_fn = self.model_params["objective"]
-        # self.params['objective']
-        # LightGBM
-
-        if not predict_proba and ("binary" in obj_fn):
-            # rounding the values and convert to integer
-            return self.model.predict(X).round(0).astype(int)
-        elif not predict_proba and ("multi" in obj_fn):
-            y_pred = self.model.predict(X)
-            # find the class using the argmax function
-            # one proba per class and pick the largest prob
-            return np.array([np.argmax(line) for line in y_pred])
-        else:
-            return self.model.predict(X)
-
-    def predict_raw(self, X, **kwargs):
-        """The native predict method, if you need raw_score, etc.
-
-
-        Parameters
-        ----------
-        X : pd.DataFrame or np.ndarray
-            the predictors' matrix
-
-        **kwargs : dict, optional
-            optional dictionary of other parameters for the prediction.
-            See the ``lightgbm`` and ``catboost`` documentation for details.
-
-        Raises
-        ------
-        Exception
-            "method not found" if the method specified in the init differs from "lgb" or "cat"
-
-        """
-        return self.model.predict(X, **kwargs)
-
-    def save(self, save_path=None, name=None):
-        """Save method, saves the model as pkl file in the specified folder as name.pkl
-        If the path is None, then the model is saved in the current working directory.
-        If the name is not specified, the model is saved as 'gbm_base_model_[TIMESTAMP].pkl
-
-        Parameters
-        ----------
-        save_path : str, optional
-            folder where to save the model, as a pickle/joblib file
-        name : str, optional
-            name of the model name
-
-        Returns
-        -------
-        str
-            where the pkl file is saved
-
-        """
-        if name:
-            file_name = f"{str(name)}.joblib"
-            fig_name = f"{str(name)}_learning_curve.png"
-        else:
-            file_name = f"gbm_base_model_{str(self.params['objective'])}.joblib"
-            fig_name = f"gbm_base_model_learning_curve_{str(date.today())}.png"
-
-        if save_path:
-            file_path = os.path.join(save_path, file_name)
-            fig_path = os.path.join(save_path, fig_name)
-        else:
-            file_path = file_name
-            fig_path = fig_name
-        print(f"Saving model as: {file_path}")
-        joblib.dump(self.model, file_path)
-
-        self.learning_curve.savefig(
-            fig_path, bbox_inches="tight"
-        )  # save the figure to file
-        return file_path
-
-    def load(self, model_path):
-        if Path(model_path).is_file():
-            # load model and update method
-            self.model = joblib.load(model_path)
-            self.model_params = self.model.params
-
-            self.cat_feat = self.model.params
-        else:
-            raise ValueError("The model file does not exist, please check the path")
-
-
-def _fit_early_stopped_lgb(
-    X,
-    y,
-    sample_weight=None,
-    groups=None,
-    init_score=None,
-    params=None,
-    cat_feat=None,
-    stratified=False,
-    learning_curve=True,
-    verbose_eval=0,
-    return_valid_features=False,
-):
-    """convenience function, early stopping for lightGBM, using dataset and setting categorical feature, sample weights
-    and baseline (init_score), if any. User defined params can be passed.
-    It works for classification and regression.
-
-    Parameters
-    ----------
-    X : pd.DataFrame or np.ndarray
-        the predictors' matrix
-    y : pd.Series or np.ndarray
-        the target series/array
-    sample_weight : pd.Series or np.ndarray, optional
-        the sample_weight series/array, if relevant. If not None, it should be of the same length as the
-        target (default ``None``)
-    groups : pd.Series or np.ndarray, optional
-        the groups (e.g. polID) for robust cross validation.
-        The same group will not appear in two different folds.
-    params : dict, optional
-        you can pass the parameters that you want to lightGBM/Catboost, as long as they are valid.
-        If None, default parameters are passed.
-    init_score : pd.Series or np.ndarray, optional
-        the initial score to boost from (series/array), if relevant. If not None,
-        it should be of the same length as the target (default ``None``)
-    cat_feat : str or list of strings, optional
-        Categorical features. If list of int, interpreted as indices. If list of strings, interpreted as feature names
-        (need to specify ``feature_name`` as well). If 'auto' and data is pandas DataFrame, pandas unordered categorical
-        columns are used. All values in categorical features should be less than int32 max value (2147483647). Large
-        values could be memory consuming. Consider using consecutive integers starting from zero. All negative values
-        in categorical features will be treated as missing values. The output cannot be monotonically constrained with
-        respect to a categorical feature (default ``None``)
-    stratified : bool, default = False
-        stratified shuffle split for the early stopping process. For classification problem, it guarantees
-        the same proportion
-    learning_curve : bool, default = False
-        if show or not the learning curve
-    verbose_eval : int, default = 0
-        period for printing the train and validation results. If < 1, no output
-    return_valid_features : bool, default = False
-        Whether or not to return validation features
-
-    Returns
-    -------
-    model : object
-        model object
-    fig : plt.figure
-        the learning curves, matplotlib figure object
-
-    """
-    (
-        X_train,
-        y_train,
-        X_val,
-        y_val,
-        sample_weight_val,
-        sample_weight_train,
-        init_score_val,
-        init_score_train,
-    ) = _make_split(
-        X=X,
-        y=y,
-        sample_weight=sample_weight,
-        init_score=init_score,
-        groups=groups,
-        stratified=stratified,
-        test_size=0.2,
-    )
-
-    col_list = list(X.columns)
-    d_train = lgb.Dataset(
-        X_train, label=y_train, categorical_feature=cat_feat, free_raw_data=False
-    )
-    d_valid = lgb.Dataset(
-        X_val,
-        label=y_val,
-        categorical_feature=cat_feat,
-        reference=d_train,
-        free_raw_data=False,
-    )
-    # set weight if any
-    if sample_weight is not None:
-        d_train = d_train.set_weight(sample_weight_train)
-        d_valid = d_valid.set_weight(sample_weight_val)
-
-    # set initial score if any
-    if init_score is not None:
-        d_train = d_train.set_init_score(init_score_train)
-        d_valid = d_valid.set_init_score(init_score_val)
-
-    # check that if the params argument is not None, it is a dictionary
-    if params is None:
-        warnings.warn("No params dictionary provided, using RMSE as default")
-        params = {"objective": "rmse", "metric": "rmse", "num_boost_round": 10_000}
-    elif not isinstance(params, dict):
-        raise TypeError(
-            "params should be either None or a dictionary of lightgbm params"
-        )
-
-    if "num_boost_round" not in params:
-        # a very large number of trees, to guarantee early stopping and convergence
-        params["num_boost_round"] = 10_000
-    # Check if the objective is passed as an argument, dictionary key or both
-    if "objective" not in params:
-        raise KeyError("No objective provided in the params dictionary")
-    # if no metric provided --> set to same as objective (early stopping)
-    # requires a metric
-    if "metric" not in params and not callable(params["objective"]):
-        params["metric"] = params["objective"]
-    elif "metric" not in params and callable(params["objective"]):
-        raise KeyError(
-            "No metric provided for early stopping and could not set objective as metric (scoring)\n"
-            "because the objective is user defined"
-        )
-
-    if "metric" in params:
-        if isinstance(params["metric"], str):
-            feval_call = None
-        else:
-            feval_call = params["metric"]
-            params["metric"] = "custom"
-    else:
-        feval_call = None
-
-    if callable(params["objective"]):
-        fobj_call = params["objective"]
-        params.pop("objective")
-    else:
-        fobj_call = None
-
-    watchlist = [d_train, d_valid]
-    evals_result = {}
-    params["verbosity"] = -1
-
-    n_trees = params["num_boost_round"] if "num_boost_round" in params else 10_000
-    # remove key if exists to avoid LGB userwarnings
-    params.pop("num_boost_round", None)
-
-    model = lgb.train(
-        params,
-        num_boost_round=n_trees,
-        train_set=d_train,
-        valid_sets=watchlist,
-        feval=feval_call,
-        fobj=fobj_call,
-        callbacks=[
-            early_stopping(10, verbose=False),
-            log_evaluation(verbose_eval),
-            record_evaluation(eval_result=evals_result),
-        ],
-    )
-
-    if learning_curve:
-        with mpl.rc_context(MPL_PARAMS):
-            fig, ax = plt.subplots()
-            ax = lgb.plot_metric(evals_result, ax=ax)
-            up_lim = model.best_iteration + 50
-            ax.axvline(
-                x=model.best_iteration, color="grey", linestyle="--", label="best_iter"
-            )
-            ax.set_xlim([0, up_lim])
-
-        del d_train
-        del d_valid
-        gc.enable()
-        gc.collect()
-        if return_valid_features:
-            return model, X_val, fig
-        else:
-            return model, fig
-    else:
-        if return_valid_features:
-            return model, X_val
-        else:
-            return model
-
-
-def _make_split(
-    X,
-    y,
-    sample_weight=None,
-    init_score=None,
-    groups=None,
-    stratified=False,
-    test_size=0.2,
-):
-    """_make_split is a private function for splitting the dataset according to the task
-
-    Parameters
-    ----------
-    X : pd.DataFrame or np.ndarray
-        the predictors' matrix
-    y : pd.Series or np.ndarray
-        the target series/array
-    sample_weight : pd.Series or np.ndarray, optional
-        the sample_weight series/array, if relevant. If not None, it should be of the same length as the
-        target (default ``None``)
-    groups : pd.Series or np.ndarray, optional
-        the groups (e.g. polID) for robust cross validation.
-        The same group will not appear in two different folds.
-    stratified : bool, default False
-        stratified shuffle split for the early stopping process. For classification problem, it guarantees
-        the same proportion
-    test_size : float, default 0.2
-        test set size, percentage of the total number of rows, by default .2
-
-    Returns
-    -------
-    Tuple[Union[pd.DataFrame, pd.Series]]
-        the split data, target, weights and initial scores (if any)
-    """
-
-    if stratified:
-        rs = StratifiedShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
-        splitter = rs.split(X, y)
-    elif (not stratified) and (groups is not None):
-        rs = GroupShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
-        splitter = rs.split(X, y, groups)
-    else:
-        rs = ShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
-        splitter = rs.split(X, y)
-
-    for train_index, test_index in splitter:
-        X_val, y_val = X.iloc[test_index], y.iloc[test_index]
-        X_train, y_train = X.iloc[train_index], y.iloc[train_index]
-        if sample_weight is not None:
-            sample_weight_val, sample_weight_train = (
-                sample_weight.iloc[test_index],
-                sample_weight.iloc[train_index],
-            )
-        else:
-            sample_weight_val, sample_weight_train = None, None
-
-        if init_score is not None:
-            init_score_val, init_score_train = (
-                init_score.iloc[test_index],
-                init_score.iloc[train_index],
-            )
-        else:
-            init_score_val, init_score_train = None, None
-
-    return (
-        X_train,
-        y_train,
-        X_val,
-        y_val,
-        sample_weight_val,
-        sample_weight_train,
-        init_score_val,
-        init_score_train,
-    )
-
-
-def gbm_flavour(estimator):
-    model_str = str(type(estimator))
-    if "lightgbm" in model_str:
-        method = "lgb"
-    elif "catboost" in model_str:
-        method = "cat"
-    else:
-        method = "unknown"
-    return method
+"""GBM Wrapper
+
+This module offers a class to train base LightGBM and CatBoost models, with early stopping as the default behavior. 
+The target variable can be finite discrete (classification) or continuous (regression). 
+Additionally, the model allows boosting from an initial score (also known as a baseline for CatBoost) and accepts sample weights as input.
+
+Module Structure:
+-----------------
+- ``GradientBoosting``: main class to train a lightGBM  or catboost with early stopping
+
+"""
+
+from sklearn.model_selection import (
+    ShuffleSplit,
+    StratifiedShuffleSplit,
+    GroupShuffleSplit,
+)
+import lightgbm as lgb
+from lightgbm import early_stopping, log_evaluation, record_evaluation
+import pandas as pd
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+import numpy as np
+import joblib
+from datetime import date
+import warnings
+import gc
+import os
+from pathlib import Path
+from arfs.utils import create_dtype_dict
+
+QUAL_COLORS = [
+    (0.188235, 0.635294, 0.854902),
+    (0.898039, 0.682353, 0.219608),
+    (0.988235, 0.309804, 0.188235),
+    (0.427451, 0.564706, 0.309804),
+]
+BCKGRND_COLOR = "#f5f5f5"
+
+MPL_PARAMS = {
+    "figure.figsize": (5, 3),
+    "axes.prop_cycle": plt.cycler(color=QUAL_COLORS),
+    "axes.facecolor": BCKGRND_COLOR,
+    "patch.edgecolor": BCKGRND_COLOR,
+    "figure.facecolor": BCKGRND_COLOR,
+    "axes.edgecolor": BCKGRND_COLOR,
+    "savefig.edgecolor": BCKGRND_COLOR,
+    "savefig.facecolor": BCKGRND_COLOR,
+    "grid.color": "#d2d2d2",
+    "lines.linewidth": 2,
+    "grid.alpha": 0.5,
+}
+
+
+class GradientBoosting:
+    """Performs the training of a base lightGBM/CatBoost using early stopping. It works for any of the
+    supported loss function (lightGBM/CatBoost), so for regression and classification you can use an instance of
+    this class. For the early stopping process, 20% of the data set is used and a fix seed is used for
+    reproducibility.
+
+    The resulting model can be saved at the desired location.
+    Last, you can pass relevant lightGBM/Catboost parameters and/or sample weights (exposure, etc.) if needed.
+
+    Init score of Booster to start from, if required (like for GLM residuals modelling using GBM).
+
+
+    Parameters
+    ----------
+    cat_feat : List[str], 'auto' or None,
+        The list of column names of the categorical predictors. For catboost, much more efficient if those columns
+        are of dtype pd.Categorical. For lightGBM, most of the time better to integer encode and NOT consider
+        them as categorical (set this parameter as None).
+    params : dict, default=None
+        you can pass the parameters that you want to lightGBM/Catboost, as long as they are valid.
+        If None, default parameters are passed.
+    stratified : bool, default=False
+        stratified shuffle split for the early stopping process. For classification problem, it guarantees
+        the same proportion
+    show_learning_curve : bool, default=True
+        if show or not the learning curve
+    verbose_eval : int, default=50
+        period for printing the train and validation results. If < 1, no output
+
+    Attributes
+    ----------
+    cat_feat : Union[str, List[str], None]
+        The list of categorical predictors after pre-processing
+    model_params : Dict
+        the dictionary of model parameters
+    learning_curve : plt.figure
+        the learning curve
+    is_init_score :  bool
+        boosted from an initial score or not
+    stratified : bool
+        either if stratified shuffle split was used or not for the early stopping process
+
+    Example
+    -------
+    >>> # set up the trainer
+    >>> save_path = "C:/Users/mtpl_bi_pp/base/"
+    >>> gbm_model = GradientBoosting(cat_feat='auto',
+    >>>                              stratified=False,
+    >>>                              params={
+    >>>                                 'objective': 'tweedie',
+    >>>                                 'tweedie_variance_power': 1.1
+    >>>                             })
+    >>>
+    >>> # train the model
+    >>> gbm_model.fit(X=X_tr,y=y_tr,sample_weight=exp_tr)
+    >>>
+    >>> # predict new values (test set)
+    >>> y_bt = gbm_model.predict(X_tt)
+    >>>
+    >>> # save the model
+    >>> gbm_model.save(save_path='C:/models/', name="my_fancy_model")
+
+    """
+
+    def __init__(
+        self,
+        cat_feat="auto",
+        params=None,
+        stratified=False,
+        show_learning_curve=True,
+        verbose_eval=50,
+        return_valid_features=False,
+    ):
+        self.model = None
+        self.cat_feat = cat_feat
+        self.model_params = None
+        self.params = params
+        self.learning_curve = None
+        self.is_init_score = False
+        self.stratified = stratified
+        self.show_learning_curve = show_learning_curve
+        self.verbose_eval = verbose_eval
+        self.return_valid_features = return_valid_features
+        self.valid_features = None
+
+    def __repr__(self):
+        s = (
+            "GradientBoosting(cat_feat={cat_feat},\n"
+            "                 params={params})".format(
+                cat_feat=self.cat_feat, params=self.params
+            )
+        )
+        return s
+
+    def fit(
+        self,
+        X,
+        y,
+        sample_weight=None,
+        init_score=None,
+        groups=None,
+    ):
+        """Fit the lightGBM/Catboost either using the python API and early stopping
+
+        Parameters
+        ----------
+        X : pd.DataFrame or np.ndarray
+            the predictors' matrix
+        y : pd.Series or np.ndarray
+            the target series/array
+        sample_weight : pd.Series or np.ndarray, optional
+            the sample_weight series/array, if relevant. If not None, it should be of the same length as the
+            target (default ``None``)
+        init_score : pd.Series or np.ndarray, optional
+            the initial score to boost from (series/array), if relevant. If not None,
+            it should be of the same length as the target (default ``None``)
+        groups : pd.Series or np.ndarray, optional
+            the groups (e.g. polID) for robust cross validation.
+            The same group will not appear in two different folds.
+
+        """
+        if (self.params is not None) and (not isinstance(self.params, dict)):
+            raise TypeError(
+                "params should be either None or a dictionary of lightgbm params"
+            )
+        elif (isinstance(self.params, dict)) and (
+            "objective" not in self.params.keys()
+        ):
+            raise KeyError("Provide the objective in the params dict")
+
+        if self.cat_feat == "auto":
+            dtypes_dic = create_dtype_dict(df=X, dic_keys="dtypes")
+            category_cols = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
+            self.cat_feat = category_cols if category_cols else None
+
+        if not isinstance(X, (pd.Series, pd.DataFrame)):
+            X = pd.DataFrame(X)
+
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y)
+
+        if sample_weight is not None:
+            if not isinstance(sample_weight, pd.Series):
+                sample_weight = pd.Series(sample_weight)
+
+        if init_score is not None:
+            self.is_init_score = True
+            if not isinstance(init_score, pd.Series):
+                init_score = pd.Series(init_score)
+
+        output = _fit_early_stopped_lgb(
+            X=X,
+            y=y,
+            sample_weight=sample_weight,
+            params=self.params,
+            init_score=init_score,
+            cat_feat=self.cat_feat,
+            stratified=self.stratified,
+            groups=groups,
+            learning_curve=self.show_learning_curve,
+            verbose_eval=self.verbose_eval,
+            return_valid_features=self.return_valid_features,
+        )
+
+        if self.show_learning_curve:
+            if self.return_valid_features:
+                self.model, self.valid_features, self.learning_curve = (
+                    output[0],
+                    output[1],
+                    output[2],
+                )
+            else:
+                self.model, self.learning_curve = output[0], output[1]
+        else:
+            if self.return_valid_features:
+                self.model, self.valid_features = output[0], output[1]
+            else:
+                self.model = output
+
+        self.model_params = self.model.params
+
+    def predict(self, X, predict_proba=False):
+        """Predict the new values using the fitted model.
+
+        Parameters
+        ----------
+        X : pd.DataFrame or np.ndarray
+            the predictors' matrix
+        predict_proba : bool, default=False
+            returns probabilities (only for classification) (default ``False``)
+        """
+        if self.is_init_score:
+            raise AttributeError(
+                "The model is fitted from an initial score, use the `predict_raw` method instead\n"
+                "Please also check what is returned by the predicted method, for the raw version\n"
+                "you might have to apply `exp`"
+            )
+
+        obj_fn = self.model_params["objective"]
+        # self.params['objective']
+        # LightGBM
+
+        if not predict_proba and ("binary" in obj_fn):
+            # rounding the values and convert to integer
+            return self.model.predict(X).round(0).astype(int)
+        elif not predict_proba and ("multi" in obj_fn):
+            y_pred = self.model.predict(X)
+            # find the class using the argmax function
+            # one proba per class and pick the largest prob
+            return np.array([np.argmax(line) for line in y_pred])
+        else:
+            return self.model.predict(X)
+
+    def predict_raw(self, X, **kwargs):
+        """The native predict method, if you need raw_score, etc.
+
+
+        Parameters
+        ----------
+        X : pd.DataFrame or np.ndarray
+            the predictors' matrix
+
+        **kwargs : dict, optional
+            optional dictionary of other parameters for the prediction.
+            See the ``lightgbm`` and ``catboost`` documentation for details.
+
+        Raises
+        ------
+        Exception
+            "method not found" if the method specified in the init differs from "lgb" or "cat"
+
+        """
+        return self.model.predict(X, **kwargs)
+
+    def save(self, save_path=None, name=None):
+        """Save method, saves the model as pkl file in the specified folder as name.pkl
+        If the path is None, then the model is saved in the current working directory.
+        If the name is not specified, the model is saved as 'gbm_base_model_[TIMESTAMP].pkl
+
+        Parameters
+        ----------
+        save_path : str, optional
+            folder where to save the model, as a pickle/joblib file
+        name : str, optional
+            name of the model name
+
+        Returns
+        -------
+        str
+            where the pkl file is saved
+
+        """
+        if name:
+            file_name = f"{str(name)}.joblib"
+            fig_name = f"{str(name)}_learning_curve.png"
+        else:
+            file_name = f"gbm_base_model_{str(self.params['objective'])}.joblib"
+            fig_name = f"gbm_base_model_learning_curve_{str(date.today())}.png"
+
+        if save_path:
+            file_path = os.path.join(save_path, file_name)
+            fig_path = os.path.join(save_path, fig_name)
+        else:
+            file_path = file_name
+            fig_path = fig_name
+        print(f"Saving model as: {file_path}")
+        joblib.dump(self.model, file_path)
+
+        self.learning_curve.savefig(
+            fig_path, bbox_inches="tight"
+        )  # save the figure to file
+        return file_path
+
+    def load(self, model_path):
+        if Path(model_path).is_file():
+            # load model and update method
+            self.model = joblib.load(model_path)
+            self.model_params = self.model.params
+
+            self.cat_feat = self.model.params
+        else:
+            raise ValueError("The model file does not exist, please check the path")
+
+
+def _fit_early_stopped_lgb(
+    X,
+    y,
+    sample_weight=None,
+    groups=None,
+    init_score=None,
+    params=None,
+    cat_feat=None,
+    stratified=False,
+    learning_curve=True,
+    verbose_eval=0,
+    return_valid_features=False,
+):
+    """convenience function, early stopping for lightGBM, using dataset and setting categorical feature, sample weights
+    and baseline (init_score), if any. User defined params can be passed.
+    It works for classification and regression.
+
+    Parameters
+    ----------
+    X : pd.DataFrame or np.ndarray
+        the predictors' matrix
+    y : pd.Series or np.ndarray
+        the target series/array
+    sample_weight : pd.Series or np.ndarray, optional
+        the sample_weight series/array, if relevant. If not None, it should be of the same length as the
+        target (default ``None``)
+    groups : pd.Series or np.ndarray, optional
+        the groups (e.g. polID) for robust cross validation.
+        The same group will not appear in two different folds.
+    params : dict, optional
+        you can pass the parameters that you want to lightGBM/Catboost, as long as they are valid.
+        If None, default parameters are passed.
+    init_score : pd.Series or np.ndarray, optional
+        the initial score to boost from (series/array), if relevant. If not None,
+        it should be of the same length as the target (default ``None``)
+    cat_feat : str or list of strings, optional
+        Categorical features. If list of int, interpreted as indices. If list of strings, interpreted as feature names
+        (need to specify ``feature_name`` as well). If 'auto' and data is pandas DataFrame, pandas unordered categorical
+        columns are used. All values in categorical features should be less than int32 max value (2147483647). Large
+        values could be memory consuming. Consider using consecutive integers starting from zero. All negative values
+        in categorical features will be treated as missing values. The output cannot be monotonically constrained with
+        respect to a categorical feature (default ``None``)
+    stratified : bool, default = False
+        stratified shuffle split for the early stopping process. For classification problem, it guarantees
+        the same proportion
+    learning_curve : bool, default = False
+        if show or not the learning curve
+    verbose_eval : int, default = 0
+        period for printing the train and validation results. If < 1, no output
+    return_valid_features : bool, default = False
+        Whether or not to return validation features
+
+    Returns
+    -------
+    model : object
+        model object
+    fig : plt.figure
+        the learning curves, matplotlib figure object
+
+    """
+    (
+        X_train,
+        y_train,
+        X_val,
+        y_val,
+        sample_weight_val,
+        sample_weight_train,
+        init_score_val,
+        init_score_train,
+    ) = _make_split(
+        X=X,
+        y=y,
+        sample_weight=sample_weight,
+        init_score=init_score,
+        groups=groups,
+        stratified=stratified,
+        test_size=0.2,
+    )
+
+    col_list = list(X.columns)
+    d_train = lgb.Dataset(
+        X_train, label=y_train, categorical_feature=cat_feat, free_raw_data=False
+    )
+    d_valid = lgb.Dataset(
+        X_val,
+        label=y_val,
+        categorical_feature=cat_feat,
+        reference=d_train,
+        free_raw_data=False,
+    )
+    # set weight if any
+    if sample_weight is not None:
+        d_train = d_train.set_weight(sample_weight_train)
+        d_valid = d_valid.set_weight(sample_weight_val)
+
+    # set initial score if any
+    if init_score is not None:
+        d_train = d_train.set_init_score(init_score_train)
+        d_valid = d_valid.set_init_score(init_score_val)
+
+    # check that if the params argument is not None, it is a dictionary
+    if params is None:
+        warnings.warn("No params dictionary provided, using RMSE as default")
+        params = {"objective": "rmse", "metric": "rmse", "num_boost_round": 10_000}
+    elif not isinstance(params, dict):
+        raise TypeError(
+            "params should be either None or a dictionary of lightgbm params"
+        )
+
+    if "num_boost_round" not in params:
+        # a very large number of trees, to guarantee early stopping and convergence
+        params["num_boost_round"] = 10_000
+    # Check if the objective is passed as an argument, dictionary key or both
+    if "objective" not in params:
+        raise KeyError("No objective provided in the params dictionary")
+    # if no metric provided --> set to same as objective (early stopping)
+    # requires a metric
+    if "metric" not in params and not callable(params["objective"]):
+        params["metric"] = params["objective"]
+    elif "metric" not in params and callable(params["objective"]):
+        raise KeyError(
+            "No metric provided for early stopping and could not set objective as metric (scoring)\n"
+            "because the objective is user defined"
+        )
+
+    if "metric" in params:
+        if isinstance(params["metric"], str):
+            feval_call = None
+        else:
+            feval_call = params["metric"]
+            params["metric"] = "custom"
+    else:
+        feval_call = None
+
+    watchlist = [d_train, d_valid]
+    evals_result = {}
+    params["verbosity"] = -1
+
+    n_trees = params["num_boost_round"] if "num_boost_round" in params else 10_000
+    # remove key if exists to avoid LGB userwarnings
+    params.pop("num_boost_round", None)
+
+    model = lgb.train(
+        params,
+        num_boost_round=n_trees,
+        train_set=d_train,
+        valid_sets=watchlist,
+        feval=feval_call,
+        # fobj=fobj_call,
+        callbacks=[
+            early_stopping(10, verbose=False),
+            log_evaluation(verbose_eval),
+            record_evaluation(eval_result=evals_result),
+        ],
+    )
+
+    if learning_curve:
+        with mpl.rc_context(MPL_PARAMS):
+            fig, ax = plt.subplots()
+            ax = lgb.plot_metric(evals_result, ax=ax)
+            up_lim = model.best_iteration + 50
+            ax.axvline(
+                x=model.best_iteration, color="grey", linestyle="--", label="best_iter"
+            )
+            ax.set_xlim([0, up_lim])
+
+        del d_train
+        del d_valid
+        gc.enable()
+        gc.collect()
+        if return_valid_features:
+            return model, X_val, fig
+        else:
+            return model, fig
+    else:
+        if return_valid_features:
+            return model, X_val
+        else:
+            return model
+
+
+def _make_split(
+    X,
+    y,
+    sample_weight=None,
+    init_score=None,
+    groups=None,
+    stratified=False,
+    test_size=0.2,
+):
+    """_make_split is a private function for splitting the dataset according to the task
+
+    Parameters
+    ----------
+    X : pd.DataFrame or np.ndarray
+        the predictors' matrix
+    y : pd.Series or np.ndarray
+        the target series/array
+    sample_weight : pd.Series or np.ndarray, optional
+        the sample_weight series/array, if relevant. If not None, it should be of the same length as the
+        target (default ``None``)
+    groups : pd.Series or np.ndarray, optional
+        the groups (e.g. polID) for robust cross validation.
+        The same group will not appear in two different folds.
+    stratified : bool, default False
+        stratified shuffle split for the early stopping process. For classification problem, it guarantees
+        the same proportion
+    test_size : float, default 0.2
+        test set size, percentage of the total number of rows, by default .2
+
+    Returns
+    -------
+    Tuple[Union[pd.DataFrame, pd.Series]]
+        the split data, target, weights and initial scores (if any)
+    """
+
+    if stratified:
+        rs = StratifiedShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
+        splitter = rs.split(X, y)
+    elif (not stratified) and (groups is not None):
+        rs = GroupShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
+        splitter = rs.split(X, y, groups)
+    else:
+        rs = ShuffleSplit(n_splits=1, test_size=test_size, random_state=42)
+        splitter = rs.split(X, y)
+
+    for train_index, test_index in splitter:
+        X_val, y_val = X.iloc[test_index], y.iloc[test_index]
+        X_train, y_train = X.iloc[train_index], y.iloc[train_index]
+        if sample_weight is not None:
+            sample_weight_val, sample_weight_train = (
+                sample_weight.iloc[test_index],
+                sample_weight.iloc[train_index],
+            )
+        else:
+            sample_weight_val, sample_weight_train = None, None
+
+        if init_score is not None:
+            init_score_val, init_score_train = (
+                init_score.iloc[test_index],
+                init_score.iloc[train_index],
+            )
+        else:
+            init_score_val, init_score_train = None, None
+
+    return (
+        X_train,
+        y_train,
+        X_val,
+        y_val,
+        sample_weight_val,
+        sample_weight_train,
+        init_score_val,
+        init_score_train,
+    )
+
+
+def gbm_flavour(estimator):
+    model_str = str(type(estimator))
+    if "lightgbm" in model_str:
+        method = "lgb"
+    elif "catboost" in model_str:
+        method = "cat"
+    else:
+        method = "unknown"
+    return method
```

### Comparing `arfs-2.0.4/src/arfs/parallel.py` & `arfs-2.0.5/src/arfs/parallel.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-"""Parallelize Pandas
-
-This module provides utilities for parallelizing operations on pd.DataFrame
-
-Module Structure:
------------------
-- ``parallel_matrix_entries`` for parallelizing operations returning a matrix (2D) (apply on pairs of columns)
-- ``parallel_df`` for parallelizing operations returning a series (1D) (apply on a single column at a time)
-"""
-
-import numpy as np
-import pandas as pd
-from joblib import Parallel, delayed
-from multiprocessing import cpu_count
-from itertools import chain
-
-
-def parallel_matrix_entries(func, df, comb_list, sample_weight=None, n_jobs=-1):
-    """parallel_matrix_entries applies a function to each chunk of
-    combinaison of columns of the dataframe, distributed by cores.
-    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
-
-
-    Parameters
-    ----------
-    func : callable
-        function to be applied to each column
-    df : pd.DataFrame
-        the dataframe on which to apply the function
-    comb_list : list of tuples of str
-        Pairs of column names corresponding to the entries
-    sample_weight : pd.Series or np.array, optional
-        The weight vector, if any, of shape (n_samples,), by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-
-    Returns
-    -------
-    pd.DataFrame
-        concatenated results into a single pandas DF
-    """
-
-    if n_jobs == 1:
-        return func(X=df, sample_weight=sample_weight, comb_list=comb_list)
-
-    n_jobs = (
-        min(cpu_count(), len(df.columns)) if n_jobs == -1 else min(cpu_count(), n_jobs)
-    )
-    comb_chunks = np.array_split(comb_list, n_jobs)
-    lst = Parallel(n_jobs=n_jobs)(
-        delayed(func)(X=df, sample_weight=sample_weight, comb_list=comb_chunk)
-        for comb_chunk in comb_chunks
-    )
-    # return flatten list of pandas DF
-    return pd.concat(list(chain(*lst)), ignore_index=True)
-
-
-def parallel_df(func, df, series, sample_weight=None, n_jobs=-1):
-    """parallel_df apply a function to each column of the dataframe, distributed by cores.
-    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
-
-    Parameters
-    ----------
-    func : callable
-        function to be applied to each column
-    df : pd.DataFrame
-        the dataframe on which to apply the function
-    series : pd.Series
-        series (target) used by the function
-    sample_weight : pd.Series or np.array, optional
-        The weight vector, if any, of shape (n_samples,), by default None
-    n_jobs : int, optional
-        the number of cores to use for the computation, by default -1
-
-    Returns
-    -------
-    pd.DataFrame
-        concatenated results into a single pandas DF
-    """
-
-    if n_jobs == 1:
-        return func(df, series, sample_weight).sort_values(ascending=False)
-
-    n_jobs = (
-        min(cpu_count(), len(df.columns)) if n_jobs == -1 else min(cpu_count(), n_jobs)
-    )
-    col_chunks = np.array_split(range(len(df.columns)), n_jobs)
-    lst = Parallel(n_jobs=n_jobs)(
-        delayed(func)(df.iloc[:, col_chunk], series, sample_weight)
-        for col_chunk in col_chunks
-    )
-    return pd.concat(lst).sort_values(ascending=False)
-
-
-def _compute_series(
-    X,
-    y,
-    sample_weight=None,
-    func_xyw=None,
-):
-    """_compute_series is a utility function for computing the series
-    resulting of the ``apply``
-
-    Parameters
-    ----------
-    X : pd.DataFrame, of shape (n_samples, n_features)
-        The set of regressors that will be tested sequentially
-    y : pd.Series or np.array, of shape (n_samples,)
-        The target vector
-    sample_weight : pd.Series or np.array, of shape (n_samples,), optional
-        The weight vector, if any, by default None
-    func_xyw : callable, optional
-        callable (function) for computing the individual elements of the series
-        takes two mandatory inputs (x and y) and an optional input w, sample_weights
-    """
-
-    def _closure_compute_series(x, y, sample_weight):
-        x_not_na = ~x.isna()
-        if x_not_na.sum() == 0:
-            return 0
-        return func_xyw(
-            x=x[x_not_na],
-            y=y[x_not_na],
-            sample_weight=sample_weight[x_not_na],
-            as_frame=False,
-        )
-
-    return X.apply(
-        lambda col: _closure_compute_series(x=col, y=y, sample_weight=sample_weight)
-    ).fillna(0.0)
-
-
-def _compute_matrix_entries(
-    X,
-    comb_list,
-    sample_weight=None,
-    func_xyw=None,
-):
-    """base closure for computing matrix entries appling a function to each chunk of
-    combinaison of columns of the dataframe, distributed by cores.
-    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
-
-    Parameters
-    ----------
-    X : pd.DataFrame, of shape (n_samples, n_features)
-        The set of regressors that will be tested sequentially
-    sample_weight : pd.Series or np.array, of shape (n_samples,), optional
-        The weight vector, if any, by default None
-    func_xyw : callable, optional
-        callable (function) for computing the individual elements of the matrix
-        takes two mandatory inputs (x and y) and an optional input w, sample_weights
-    comb_list : list of 2-uple of str
-        Pairs of column names corresponding to the entries
-
-    Returns
-    -------
-    pd.DataFrame
-        concatenated results into a single pandas DF
-    """
-    v_df_list = []
-    for comb in comb_list:
-        v_df_list.append(
-            func_xyw(
-                x=X[comb[0]],
-                y=X[comb[1]],
-                sample_weight=sample_weight,
-                as_frame=True,
-            )
-        )
-
-    return v_df_list
+"""Parallelize Pandas
+
+This module provides utilities for parallelizing operations on pd.DataFrame
+
+Module Structure:
+-----------------
+- ``parallel_matrix_entries`` for parallelizing operations returning a matrix (2D) (apply on pairs of columns)
+- ``parallel_df`` for parallelizing operations returning a series (1D) (apply on a single column at a time)
+"""
+
+import numpy as np
+import pandas as pd
+from joblib import Parallel, delayed
+from multiprocessing import cpu_count
+from itertools import chain
+
+
+def parallel_matrix_entries(func, df, comb_list, sample_weight=None, n_jobs=-1):
+    """parallel_matrix_entries applies a function to each chunk of
+    combinaison of columns of the dataframe, distributed by cores.
+    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
+
+
+    Parameters
+    ----------
+    func : callable
+        function to be applied to each column
+    df : pd.DataFrame
+        the dataframe on which to apply the function
+    comb_list : list of tuples of str
+        Pairs of column names corresponding to the entries
+    sample_weight : pd.Series or np.array, optional
+        The weight vector, if any, of shape (n_samples,), by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+
+    Returns
+    -------
+    pd.DataFrame
+        concatenated results into a single pandas DF
+    """
+
+    if n_jobs == 1:
+        return func(X=df, sample_weight=sample_weight, comb_list=comb_list)
+
+    n_jobs = (
+        min(cpu_count(), len(df.columns)) if n_jobs == -1 else min(cpu_count(), n_jobs)
+    )
+    comb_chunks = np.array_split(comb_list, n_jobs)
+    lst = Parallel(n_jobs=n_jobs)(
+        delayed(func)(X=df, sample_weight=sample_weight, comb_list=comb_chunk)
+        for comb_chunk in comb_chunks
+    )
+    # return flatten list of pandas DF
+    return pd.concat(list(chain(*lst)), ignore_index=True)
+
+
+def parallel_df(func, df, series, sample_weight=None, n_jobs=-1):
+    """parallel_df apply a function to each column of the dataframe, distributed by cores.
+    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
+
+    Parameters
+    ----------
+    func : callable
+        function to be applied to each column
+    df : pd.DataFrame
+        the dataframe on which to apply the function
+    series : pd.Series
+        series (target) used by the function
+    sample_weight : pd.Series or np.array, optional
+        The weight vector, if any, of shape (n_samples,), by default None
+    n_jobs : int, optional
+        the number of cores to use for the computation, by default -1
+
+    Returns
+    -------
+    pd.DataFrame
+        concatenated results into a single pandas DF
+    """
+
+    if n_jobs == 1:
+        return func(df, series, sample_weight).sort_values(ascending=False)
+
+    n_jobs = (
+        min(cpu_count(), len(df.columns)) if n_jobs == -1 else min(cpu_count(), n_jobs)
+    )
+    col_chunks = np.array_split(range(len(df.columns)), n_jobs)
+    lst = Parallel(n_jobs=n_jobs)(
+        delayed(func)(df.iloc[:, col_chunk], series, sample_weight)
+        for col_chunk in col_chunks
+    )
+    return pd.concat(lst).sort_values(ascending=False)
+
+
+def _compute_series(
+    X,
+    y,
+    sample_weight=None,
+    func_xyw=None,
+):
+    """_compute_series is a utility function for computing the series
+    resulting of the ``apply``
+
+    Parameters
+    ----------
+    X : pd.DataFrame, of shape (n_samples, n_features)
+        The set of regressors that will be tested sequentially
+    y : pd.Series or np.array, of shape (n_samples,)
+        The target vector
+    sample_weight : pd.Series or np.array, of shape (n_samples,), optional
+        The weight vector, if any, by default None
+    func_xyw : callable, optional
+        callable (function) for computing the individual elements of the series
+        takes two mandatory inputs (x and y) and an optional input w, sample_weights
+    """
+
+    def _closure_compute_series(x, y, sample_weight):
+        x_not_na = ~x.isna()
+        if x_not_na.sum() == 0:
+            return 0
+        return func_xyw(
+            x=x[x_not_na],
+            y=y[x_not_na],
+            sample_weight=sample_weight[x_not_na],
+            as_frame=False,
+        )
+
+    return X.apply(
+        lambda col: _closure_compute_series(x=col, y=y, sample_weight=sample_weight)
+    ).fillna(0.0)
+
+
+def _compute_matrix_entries(
+    X,
+    comb_list,
+    sample_weight=None,
+    func_xyw=None,
+):
+    """base closure for computing matrix entries appling a function to each chunk of
+    combinaison of columns of the dataframe, distributed by cores.
+    This is similar to https://github.com/smazzanti/mrmr/mrmr/pandas.py
+
+    Parameters
+    ----------
+    X : pd.DataFrame, of shape (n_samples, n_features)
+        The set of regressors that will be tested sequentially
+    sample_weight : pd.Series or np.array, of shape (n_samples,), optional
+        The weight vector, if any, by default None
+    func_xyw : callable, optional
+        callable (function) for computing the individual elements of the matrix
+        takes two mandatory inputs (x and y) and an optional input w, sample_weights
+    comb_list : list of 2-uple of str
+        Pairs of column names corresponding to the entries
+
+    Returns
+    -------
+    pd.DataFrame
+        concatenated results into a single pandas DF
+    """
+    v_df_list = []
+    for comb in comb_list:
+        v_df_list.append(
+            func_xyw(
+                x=X[comb[0]],
+                y=X[comb[1]],
+                sample_weight=sample_weight,
+                as_frame=True,
+            )
+        )
+
+    return v_df_list
```

### Comparing `arfs-2.0.4/src/arfs/preprocessing.py` & `arfs-2.0.5/src/arfs/preprocessing.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,1019 +1,1019 @@
-"""
-This module provides preprocessing classes
-
-Module Structure:
------------------
-- ``OrdinalEncoderPandas``: main class for ordinal encoding, takes in a DF and returns a DF of the same shape
-- ``dtype_column_selector``: for standardizing selection of columns based on their dtypes
-- ``TreeDiscretizer``: class for discretizing continuous columns and auto-group levels of categorical columns
-- ``IntervalToMidpoint``: class for converting pandas numerical intervals into their float midpoint
-- ``PatsyTransformer``: class for encoding data for (generalized) linear models, leveraging Patsy
-"""
-
-# Settings and libraries
-from __future__ import print_function
-from tqdm.auto import tqdm
-
-# pandas
-import pandas as pd
-from pandas.api.types import IntervalDtype
-
-# numpy
-import numpy as np
-
-# regular expression
-import re
-
-# sklearn
-from sklearn.preprocessing import OrdinalEncoder
-from sklearn.base import BaseEstimator, TransformerMixin
-
-# patsy
-from patsy import dmatrix, EvalEnvironment, ModelDesc, INTERCEPT
-
-# typing
-from typing import Any, Callable, Union, List, Tuple, Optional, Dict
-
-# ARFS
-from .gbm import GradientBoosting
-from .utils import create_dtype_dict
-
-
-# fix random seed for reproducibility
-np.random.seed(7)
-
-
-class OrdinalEncoderPandas(OrdinalEncoder):
-    # class OrdinalEncoderPandas(BaseEstimator, TransformerMixin):
-    """Encode categorical features as an integer array and returns a pandas DF.
-    The features are converted to ordinal integers. This results in
-    a single column of integers (0 to n_categories - 1) per feature.
-    Read more in the scikit-learn OrdinalEncoder documentation
-
-    Parameters
-    ----------
-    pattern : str, default=None
-        Name of columns containing this regex pattern will be included. If
-        None, column selection will not be selected based on pattern.
-    dtype_include : column dtype or list of column dtypes, default=None
-        A selection of dtypes to include. For more details, see
-        `pandas.DataFrame.select_dtypes`.
-    dtype_exclude : column dtype or list of column dtypes, default=None
-        A selection of dtypes to exclude. For more details, see
-        `pandas.DataFrame.select_dtypes`.
-    exclude_cols : list of str, optional
-        columns to not encode
-    output_dtype : number type, default np.float64
-        Desired dtype of output.
-    handle_unknown : {'error', 'use_encoded_value'}, default='error'
-        When set to 'error' an error will be raised in case an unknown
-        categorical feature is present during transform. When set to
-        'use_encoded_value', the encoded value of unknown categories will be
-        set to the value given for the parameter `unknown_value`. In
-        `inverse_transform`, an unknown category will be denoted as None.
-    unknown_value : int or np.nan, default=None
-        When the parameter handle_unknown is set to 'use_encoded_value', this
-        parameter is required and will set the encoded value of unknown
-        categories. It has to be distinct from the values used to encode any of
-        the categories in `fit`. If set to np.nan, the `dtype` parameter must
-        be a float dtype.
-    encoded_missing_value : int or np.nan, default=np.nan
-        Encoded value of missing categories. If set to `np.nan`, then the `dtype`
-        parameter must be a float dtype.
-    return_pandas_categorical : bool, defult=False
-        return encoded columns as pandas category dtype or as float
-
-    Attributes
-    ----------
-    categories_ : list of arrays
-        The categories of each feature determined during ``fit`` (in order of
-        the features in X and corresponding with the output of ``transform``).
-        This does not include categories that weren't seen during ``fit``.
-    feature_names_in_ : ndarray of shape (`n_features_in_`,)
-        Names of features seen during :term:`fit`. Defined only when `X`
-        has feature names that are all strings.
-
-    Examples
-    --------
-    Given a dataset with two features, we let the encoder find the unique
-    values per feature and transform the data to an ordinal encoding.
-    >>> ord_enc = OrdinalEncoderPandas(exclude_cols=["PARENT1", "SEX"])
-    >>> X_enc = ord_enc.fit_transform(X)
-    >>> X_original = ord_enc.inverse_transform(X_enc)
-    """
-
-    def __init__(
-        self,
-        dtype_include=["category", "object", "bool"],
-        dtype_exclude=[np.number],
-        pattern=None,
-        exclude_cols=None,
-        output_dtype=np.float64,
-        handle_unknown="use_encoded_value",
-        unknown_value=np.nan,
-        encoded_missing_value=np.nan,
-        return_pandas_categorical=False,
-    ):
-        self.dtype_include = dtype_include
-        self.dtype_exclude = dtype_exclude
-        self.pattern = pattern
-        self.exclude_cols = exclude_cols
-        self.output_dtype = output_dtype
-        self.handle_unknown = handle_unknown
-        self.unknown_value = unknown_value
-        self.encoded_missing_value = encoded_missing_value
-        self.return_pandas_categorical = return_pandas_categorical
-
-        super().__init__(
-            categories="auto",
-            dtype=self.output_dtype,
-            handle_unknown=self.handle_unknown,
-            unknown_value=self.unknown_value,
-            encoded_missing_value=self.encoded_missing_value,
-        )
-
-    def fit(self, X, y=None):
-        """
-        Fit the OrdinalEncoder to X.
-
-        Parameters
-        ----------
-        X : pd.DataFrame, of shape (n_samples, n_features)
-            The data to determine the categories of each feature.
-        y : Ignored. This parameter exists only for compatibility with
-            :class:`~sklearn.pipeline.Pipeline`.
-
-        Returns
-        -------
-        self :
-            Fitted encoder.
-        """
-
-        cat_features_selector = dtype_column_selector(
-            dtype_include=self.dtype_include,
-            dtype_exclude=self.dtype_exclude,
-            pattern=self.pattern,
-            exclude_cols=self.exclude_cols,
-        )
-
-        self.feature_names_in_ = X.columns.to_numpy()
-        self.categorical_features_ = cat_features_selector(X)
-
-        super(OrdinalEncoderPandas, self).fit(X[self.categorical_features_])
-        # self.feature_names_in_ = X.columns.to_numpy()
-        return self
-
-    def transform(self, X, y=None, sample_weight=None):
-        """
-        Transform X to ordinal codes.
-
-        Parameters
-        ----------
-        X : pd.DataFrame of shape (n_samples, n_features)
-            The data to encode.
-
-        Returns
-        -------
-        X_out : pd.DataFrame (n_samples, n_features)
-            Transformed input.
-        """
-        X_trans = X.copy()
-        X_trans[self.categorical_features_] = super(
-            OrdinalEncoderPandas, self
-        ).transform(X_trans[self.categorical_features_])
-
-        if self.return_pandas_categorical:
-            X_trans[self.categorical_features_] = X_trans[
-                self.categorical_features_
-            ].astype("category")
-        return X_trans
-
-    def fit_transform(self, X, y=None, sample_weight=None, **fit_params):
-        """
-        Fit to data, then transform it.
-        Fits transformer to `X` and `y` with optional parameters `fit_params`
-        and returns a transformed version of `X`.
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input samples.
-        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
-                default=None
-            Target values (None for unsupervised transformations).
-        **fit_params : dict
-            Additional fit parameters.
-        Returns
-        -------
-        X_new : ndarray array of shape (n_samples, n_features_new)
-            Transformed array.
-        """
-        self = self.fit(X)
-        return self.transform(X)
-
-    def inverse_transform(self, X):
-        """
-        Convert the data back to the original representation.
-        When unknown categories are encountered (all zeros in the
-        one-hot encoding), ``None`` is used to represent this category. If the
-        feature with the unknown category has a dropped category, the dropped
-        category will be its inverse.
-        For a given input feature, if there is an infrequent category,
-        'infrequent_sklearn' will be used to represent the infrequent category.
-
-        Parameters
-        ----------
-        X : pd.DataFrame of shape (n_samples, n_encoded_features)
-            The transformed data.
-        Returns
-        -------
-        X_tr : pd.Dataframe of shape (n_samples, n_features)
-            Inverse transformed array.
-        """
-
-        X[self.categorical_features_] = super(
-            OrdinalEncoderPandas, self
-        ).inverse_transform(X[self.categorical_features_])
-        return X
-
-
-class dtype_column_selector:
-    """Create a callable to select columns to be used with
-    :class:`ColumnTransformer`.
-    :func:`dtype_column_selector` can select columns based on datatype or the
-    columns name with a regex. When using multiple selection criteria, **all**
-    criteria must match for a column to be selected.
-
-    Parameters
-    ----------
-    pattern : str, default=None
-        Name of columns containing this regex pattern will be included. If
-        None, column selection will not be selected based on pattern.
-    dtype_include : column dtype or list of column dtypes, default=None
-        A selection of dtypes to include. For more details, see
-        :meth:`pandas.DataFrame.select_dtypes`.
-    dtype_exclude : column dtype or list of column dtypes, default=None
-        A selection of dtypes to exclude. For more details, see
-        :meth:`pandas.DataFrame.select_dtypes`.
-    exclude_cols : list of column names, default=None
-        A selection of columns to exclude
-
-    Returns
-    -------
-    selector : callable
-        Callable for column selection to be used by a
-        :class:`ColumnTransformer`.
-
-    See Also
-    --------
-    ColumnTransformer : Class that allows combining the
-        outputs of multiple transformer objects used on column subsets
-        of the data into a single feature space.
-
-    Examples
-    --------
-    >>> from sklearn.preprocessing import StandardScaler, OneHotEncoder
-    >>> from sklearn.compose import make_column_transformer
-    >>> from arfs.preprocessing import dtype_column_selector
-    >>> import numpy as np
-    >>> import pandas as pd  # doctest: +SKIP
-    >>> X = pd.DataFrame({'city': ['London', 'London', 'Paris', 'Sallisaw'],
-    ...                   'rating': [5, 3, 4, 5]})  # doctest: +SKIP
-    >>> ct = make_column_transformer(
-    ...       (StandardScaler(),
-    ...        dtype_column_selector(dtype_include=np.number)),  # rating
-    ...       (OneHotEncoder(),
-    ...        dtype_column_selector(dtype_include=object)))  # city
-    >>> ct.fit_transform(X)
-    array([[ 0.90453403,  1.        ,  0.        ,  0.        ],
-           [-1.50755672,  1.        ,  0.        ,  0.        ],
-           [-0.30151134,  0.        ,  1.        ,  0.        ],
-           [ 0.90453403,  0.        ,  0.        ,  1.        ]])
-    """
-
-    def __init__(
-        self, pattern=None, *, dtype_include=None, dtype_exclude=None, exclude_cols=None
-    ):
-        self.pattern = pattern
-        self.dtype_include = dtype_include
-        self.dtype_exclude = dtype_exclude
-        self.exclude_cols = exclude_cols
-
-    def __call__(self, df):
-        """Callable for column selection to be used by a
-        :class:`ColumnTransformer`.
-        Parameters
-        ----------
-        df : pd.DataFrame of shape (n_features, n_samples)
-            DataFrame to select columns from.
-        """
-        if not hasattr(df, "iloc"):
-            raise ValueError(
-                "make_column_selector can only be applied to pandas dataframes"
-            )
-        df_row = df.iloc[:1]
-        if self.dtype_include is not None or self.dtype_exclude is not None:
-            df_row = df_row.select_dtypes(
-                include=self.dtype_include, exclude=self.dtype_exclude
-            )
-        cols = df_row.columns
-        if self.pattern is not None:
-            cols = cols[cols.str.contains(self.pattern, regex=True)]
-
-        if self.exclude_cols is not None:
-            cols = cols[~cols.isin(self.exclude_cols)]
-
-        return cols.tolist()
-
-
-def cat_var(data, col_excl=None, return_cat=True):
-    """Ad hoc categorical encoding (as integer). Automatically detect the non-numerical columns,
-    save the index and name of those columns, encode them as integer,
-    save the direct and inverse mappers as
-    dictionaries.
-    Return the data-set with the encoded columns with a data type either int or pandas categorical.
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        the dataset
-    col_excl: list of str, default=None
-        the list of columns names not being encoded (e.g. the ID column)
-    return_cat: bool, default=True
-        return encoded object columns as pandas categoricals or not.
-
-    Returns
-    -------
-    df: pd.DataFrame
-        the dataframe with encoded columns
-    cat_var_df: pd.DataFrame
-        the dataframe with the indices and names of the categorical columns
-    inv_mapper: dict
-        the dictionary to map integer --> category
-    mapper: dict
-        the dictionary to map category --> integer
-    """
-    df = data.copy()
-    if col_excl is None:
-        non_num_cols = list(
-            set(list(df.columns)) - set(list(df.select_dtypes(include=[np.number])))
-        )
-    else:
-        non_num_cols = list(
-            set(list(df.columns))
-            - set(list(df.select_dtypes(include=[np.number])))
-            - set(col_excl)
-        )
-    cat_var_index = [df.columns.get_loc(c) for c in non_num_cols if c in df]
-    cat_var_df = pd.DataFrame({"cat_ind": cat_var_index, "cat_name": non_num_cols})
-    # avoid having datetime objects as keys in the mapping dic
-    date_cols = [s for s in list(df) if "date" in s]
-    df.loc[:, date_cols] = df.loc[:, date_cols].astype(str)
-    cols_need_mapped = cat_var_df.cat_name.to_list()
-    inv_mapper = {
-        col: dict(enumerate(df[col].astype("category").cat.categories))
-        for col in df[cols_need_mapped]
-    }
-    mapper = {
-        col: {v: k for k, v in inv_mapper[col].items()} for col in df[cols_need_mapped]
-    }
-    progress_bar = tqdm(cols_need_mapped)
-    for c in progress_bar:
-        progress_bar.set_description("Processing {0:<30}".format(c))
-        df.loc[:, c] = df.loc[:, c].map(mapper[c]).fillna(0).astype(int)
-        # I could have use df[c].update(df[c].map(mapper[c])) while slower,
-        # prevents values not included in an incomplete map from being changed to nans.
-        # But then I could have outputs
-        # with mixed types in the case of different dtypes mapping (like str -> int).
-        # This would eventually break any flow.
-        # Map is faster than replace
-    if return_cat:
-        df.loc[:, non_num_cols] = df.loc[:, non_num_cols].astype("category")
-    return df, cat_var_df, inv_mapper, mapper
-
-
-class TreeDiscretizer(BaseEstimator, TransformerMixin):
-    """
-    Discretize continuous and/or categorical data using univariate regularized trees, returning a pandas DataFrame.
-    The TreeDiscretizer is designed to support regression and binary classification tasks.
-    Discretization, also known as quantization or binning, allows for the partitioning of continuous features into discrete values.
-    In certain datasets with continuous attributes, discretization can be beneficial as it transforms the dataset into one with only nominal attributes.
-    Additionally, for categorical predictors, grouping levels can help reduce overfitting and create meaningful clusters.
-
-    By encoding discretized features, a model can become more expressive while maintaining interpretability.
-    For example, preprocessing with a discretizer can introduce nonlinearity to linear models.
-    For more advanced possibilities, particularly smooth ones, you can refer to the section on generating polynomial features.
-    The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned.
-    It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns.
-    This approach groups similar levels together, reducing dimensionality and regularizing the model.
-
-    TreeDiscretizer handles missing values for both numerical and categorical predictors,
-    eliminating the need for encoding categorical predictors separately.
-
-    Notes
-    -----
-    This is a substitution to proper regularization schemes such as:
-    - GroupLasso: Categorical predictors, which are usually encoded as multiple dummy variables,
-                  are considered together rather than separately.
-    - FusedLasso: Takes into account the ordering of the features.
-
-    Parameters
-    ----------
-    bin_features : List of string or None
-        The list of names of the variable that has to be binned, or "all", "numerical" or "categorical"
-        for splitting and grouping all, only numerical or only categorical columns.
-    n_bins : int
-        The number of bins that has to be created while binning the variables in the "bin_features" list.
-    n_bins_max : int, optional
-        The maximum number of levels that a categorical column can have to avoid being binned.
-    num_bins_as_category: bool, default=False
-        Save the numeric bins as pandas category or as pandas interval.
-    boost_params : dict
-        The boosting parameters dictionary.
-    raw : bool
-        Returns raw levels (non-human-interpretable) or levels matching the original ones.
-    task : str
-        Either regression or classification (binary).
-
-    Attributes
-    ----------
-    tree_dic : dict
-        The dictionary keys are binned column names and items are the univariate trees.
-    bin_upper_bound_dic : dict
-        The upper bound of the numerical intervals.
-    cat_bin_dict : dict
-        The mapping dictionary for the categorical columns.
-    tree_imputer : dict
-        The missing values are split by the tree and lead to similar splits and are mapped to this value.
-    ordinal_encoder_dic : dict
-        Dictionary with the fitted encoder, if any.
-    cat_features : list
-        Names of the found categorical columns.
-
-    Methods
-    -------
-    fit(X, y, sample_weight=None)
-        Fit the transformer object on data.
-    transform(X)
-        Apply the fitted transformer object on new data.
-    fit_transform(X)
-        Fit and apply the transformer object on data.
-
-    Example
-    -------
-    >>> lgb_params = {'min_split_gain': 5}
-    >>> disc = TreeDiscretizer(bin_features='all', n_bins=10)
-    >>> disc.fit(X=df[predictors], y=df['Frequency'], sample_weight=df['Exposure'])
-    """
-
-    def __init__(
-        self,
-        bin_features="all",
-        n_bins=10,
-        n_bins_max=None,
-        num_bins_as_category=False,
-        boost_params=None,
-        raw=False,
-        task="regression",
-    ):
-        if (boost_params is not None) & (not isinstance(boost_params, dict)):
-            raise TypeError("boost_kwargs should be a dictionary")
-
-        self.bin_features = bin_features
-        self.n_bins = n_bins
-        self.n_bins_max = n_bins_max
-        self.num_bins_as_category = num_bins_as_category
-        self.boost_params = {}
-        self.raw = raw
-        self.task = task
-        if boost_params is not None:
-            self.boost_params = boost_params
-
-        # force some params
-        if self.task == "regression":
-            self.boost_params["objective"] = "RMSE"
-        elif self.task == "classification":
-            self.boost_params["objective"] = "binary"
-
-        self.boost_params["num_boost_round"] = 1
-        self.boost_params["max_leaf"] = self.n_bins
-        self.tree_dic = {}
-        self.bin_upper_bound_dic = {}
-        self.cat_bin_dict = {}
-        self.tree_imputer = {}
-        self.ordinal_encoder_dic = {}
-        self.cat_features = None
-
-    def fit(self, X, y, sample_weight=None):
-        """
-        Fit the TreeDiscretizer on the input data.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            The predictor dataframe.
-        y : array-like of shape (n_samples,)
-            The target vector.
-        sample_weight : array-like of shape (n_samples,), optional
-            The weight vector, by default None.
-
-        Returns
-        -------
-        self : object
-            Returns self.
-        """
-        X = X.copy()
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
-
-        self.feature_names_in_ = X.columns.to_numpy()
-
-        if self.bin_features is None:
-            self.bin_features = list(X.select_dtypes("number").columns)
-            self.cat_features = []
-        elif isinstance(self.bin_features, list):
-            self.cat_features = list(
-                set(self.bin_features)
-                - set(list(X[self.bin_features].select_dtypes("number").columns))
-            )
-        elif isinstance(self.bin_features, str) and (self.bin_features == "all"):
-            self.bin_features = list(X.columns)
-            self.cat_features = list(
-                set(self.bin_features) - set(list(X.select_dtypes("number").columns))
-            )
-        elif isinstance(self.bin_features, str) and (self.bin_features == "numerical"):
-            self.bin_features = list(X.select_dtypes("number").columns)
-        elif isinstance(self.bin_features, str) and (
-            self.bin_features == "categorical"
-        ):
-            self.bin_features = list(X.select_dtypes(["category", "object"]).columns)
-            self.cat_features = self.bin_features
-
-        self.n_unique_table_ = X[self.bin_features].nunique()
-        # transform only the columns with more than n_bins_max
-        self.bin_features = (
-            self.n_unique_table_[self.n_unique_table_ > self.n_bins_max].index.to_list()
-            if self.n_bins_max
-            else self.bin_features
-        )
-
-        for col in self.bin_features:
-            is_categorical = (self.cat_features is not None) and (
-                col in self.cat_features
-            )
-            if is_categorical:
-                encoder = OrdinalEncoder(
-                    handle_unknown="use_encoded_value", unknown_value=np.nan
-                )
-                # create a category for missing
-                X[col] = (
-                    X[col]
-                    .astype("category")
-                    .cat.add_categories("missing_added")
-                    .fillna("missing_added")
-                )
-                # encode
-                self.ordinal_encoder_dic[col] = encoder.fit(X[[col]])
-                dum = encoder.transform(X[[col]])
-                if isinstance(dum, pd.DataFrame):
-                    X[col] = dum.values.ravel()
-                else:
-                    X[col] = dum.ravel()
-
-            else:
-                encoder = None
-
-            gbm_param = self.boost_params.copy()
-            tree = GradientBoosting(
-                cat_feat=None, params=gbm_param, show_learning_curve=False
-            )
-            tree.fit(X[[col]], y, sample_weight=sample_weight)
-
-            # store each fitted tree in a dictionary
-            self.tree_dic[col] = tree
-
-            # create the bins series
-            # predict, group by original values
-            # create monotonicly increasing bin for pd.cut
-            X[f"{col}_g"] = tree.predict(X[[col]])
-
-            if is_categorical:
-                # retrieve original values
-                dum = encoder.inverse_transform(X[[col]])
-                if isinstance(dum, pd.DataFrame):
-                    X[col] = dum.values.ravel()
-                else:
-                    X[col] = dum.ravel()
-
-                self.cat_bin_dict[col] = (
-                    X[[f"{col}_g", col]]
-                    .groupby(f"{col}_g")
-                    .apply(lambda x: " / ".join(map(str, x[col].unique())))
-                    .to_dict()
-                )
-            else:
-                bin_array = (
-                    X[[f"{col}_g", col]]
-                    .groupby(f"{col}_g")
-                    .aggregate(max)
-                    .sort_values(col)
-                    .values.ravel()
-                )
-                # overwrite max for handling unseen larger values than max val on the train set
-                bin_array = np.delete(bin_array, [np.argmax(bin_array)])
-                # append -Inf and Inf for covering the whole interval, as in KBinsDiscretizer
-                bin_array = np.unique(np.append(bin_array, [-np.Inf, np.Inf]))
-                self.bin_upper_bound_dic[col] = bin_array
-                # the tree imputer: if nan is passed, the predicted value will be the
-                # same than another non-missing value and nan should fall into this bin
-                # the predicted value of a NaN
-                nan_pred_val = tree.predict(np.expand_dims([np.nan], axis=1))[0]
-                # the closest predicted value for non NaN inputs
-                non_nan_values = X[col].dropna().unique()
-                pred_values = tree.predict(np.expand_dims(non_nan_values, axis=1))
-                # store the value for knowing the bin into which the NaN should fall
-                self.tree_imputer[col] = non_nan_values.flat[
-                    np.abs(pred_values - nan_pred_val).argmin()
-                ]
-
-            del tree
-
-        return self
-
-    def transform(self, X):
-        """
-        Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
-            `n_features` is the number of features.
-
-        Returns
-        -------
-        X : pd.DataFrame
-            DataFrame with the binned and grouped columns.
-        """
-        X = X.copy()
-
-        for col in self.bin_features:
-            if self.raw:
-                # predict each univariate tree
-                X[col] = self.tree_dic[col].predict(X[[col]])
-            else:
-                if (self.cat_features is not None) and (col in self.cat_features):
-                    # apply the systematic imputation (missing might be grouped
-                    # with other categories depending on the results of the tree
-                    # splitting)
-                    X[col] = (
-                        X[col]
-                        .astype("category")
-                        .cat.add_categories("missing_added")
-                        .fillna("missing_added")
-                    )
-                    dum = self.ordinal_encoder_dic[col].transform(X[[col]])
-                    X[col] = self.tree_dic[col].predict(dum)
-                    X[col] = X[col].map(self.cat_bin_dict[col])
-                else:
-                    # retrieve the association the tree learnt for missing values
-                    X[col].fillna(self.tree_imputer[col], inplace=True)
-                    # apply the binning
-                    X[col] = pd.cut(
-                        X[col],
-                        bins=self.bin_upper_bound_dic[col],
-                        include_lowest=True,
-                        precision=2,
-                    )
-
-                    if not self.num_bins_as_category:
-                        X[col] = X[col].astype(IntervalDtype())
-        return X
-
-
-def highlight_discarded(s):
-    """
-    highlight X in red and V in green.
-
-    Parameters
-    ----------
-    s : np.arrays
-
-    Returns
-    -------
-    list
-
-    """
-    is_X = s == 0
-    return [
-        "background-color: #d65f5f" if v else "background-color: #33a654" for v in is_X
-    ]
-
-
-class IntervalToMidpoint(BaseEstimator, TransformerMixin):
-    """
-    IntervalToMidpoint is a transformer that converts numerical intervals in a pandas DataFrame to their midpoints.
-
-    Parameters
-    ----------
-    cols : list of str or str, default "all"
-        The column(s) to transform. If "all", all columns with numerical intervals will be transformed.
-
-    Attributes
-    ----------
-    cols : list of str or str
-        The column(s) to transform.
-    float_interval_cols_ : list of str
-        The columns with numerical interval data types in the input DataFrame.
-    columns_to_transform_ : list of str
-        The columns to be transformed based on the specified `cols` attribute.
-
-    Methods
-    -------
-    fit(X, y=None)
-        Fit the transformer on the input data.
-    transform(X)
-        Transform the input data by converting numerical intervals to midpoints.
-    inverse_transform(X)
-        Inverse transform is not implemented for this transformer.
-    """
-
-    def __init__(self, cols: Union[List[str], str] = "all"):
-        self.cols = cols
-
-    def fit(self, X: pd.DataFrame = None, y: pd.Series = None):
-        """
-        Fit the transformer on the input data.
-
-        Parameters
-        ----------
-        X :
-            The input data to fit the transformer on.
-        y :
-            Ignored parameter.
-
-        Returns
-        -------
-        self : IntervalToMidpoint
-            The fitted transformer object.
-        """
-        data = X.copy()
-
-        if self.cols == "all":
-            self.cols = data.columns
-
-        self.float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")[
-            "num_interval"
-        ]
-        self.columns_to_transform_ = list(
-            set(self.cols).intersection(set(self.float_interval_cols_))
-        )
-        return self
-
-    def transform(self, X: pd.DataFrame):
-        """
-        Transform the input data by converting numerical intervals to midpoints.
-
-        Parameters
-        ----------
-        X : pd.DataFrame
-            The input data to transform.
-
-        Returns
-        -------
-        X : pd.DataFrame
-            The transformed data with numerical intervals replaced by their midpoints.
-        """
-        X = X.copy()
-        for c in self.columns_to_transform_:
-            X.loc[:, c] = find_interval_midpoint(X[c])
-            X.loc[:, c] = X[c].astype(float)
-        return X
-
-    def inverse_transform(self, X: pd.DataFrame):
-        """
-        Inverse transform is not implemented for this transformer.
-
-        Parameters
-        ----------
-        X : pd.DataFrame
-            The input data to perform inverse transform on.
-
-        Raises
-        ------
-        NotImplementedError
-            Raised since inverse transform is not implemented for this transformer.
-        """
-        raise NotImplementedError(
-            "inverse_transform is not implemented for this transformer."
-        )
-
-
-def transform_interval_to_midpoint(
-    X: pd.DataFrame, cols: Union[List[str], str] = "all"
-) -> pd.DataFrame:
-    """
-    Transforms interval columns in a pandas DataFrame to their midpoint values.
-
-    Notes
-    -----
-    Equivalent function to ``IntervalToMidpoint`` without the estimator API
-
-    Parameters
-    ----------
-    X : pd.DataFrame
-        The input DataFrame containing the data to be transformed.
-    cols : list of str or str
-        The columns to be transformed. Defaults to "all" which transforms all columns.
-
-    Returns
-    -------
-    pd.DataFrame :
-        The transformed DataFrame with interval columns replaced by their midpoint values.
-
-    Raises
-    ------
-    TypeError :
-        If the input data is not a pandas DataFrame.
-    """
-    if cols == "all":
-        cols = X.columns
-
-    X = X.copy()
-    float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
-    columns_to_transform_ = list(set(cols).intersection(set(float_interval_cols_)))
-    for c in columns_to_transform_:
-        X.loc[:, c] = find_interval_midpoint(X[c])
-    return X
-
-
-def find_interval_midpoint(interval_series: pd.Series) -> np.ndarray:
-    """Find the midpoint (or left/right bound if the interval contains Inf).
-
-    Parameters
-    ----------
-    interval_series : pd.Series
-        series of pandas intervals.
-
-    Returns
-    -------
-    np.ndarray
-        Array of midpoints or bounds of the intervals.
-    """
-    left = interval_series.array.left
-    right = interval_series.array.right
-    mid = interval_series.array.mid
-    left_inf = np.isinf(left)
-    right_inf = np.isinf(right)
-
-    return np.where(
-        left_inf & right_inf,
-        np.inf,
-        np.where(left_inf, right, np.where(right_inf, left, mid)),
-    )
-
-
-class PatsyTransformer(BaseEstimator, TransformerMixin):
-    """Transformer using patsy-formulas.
-
-    PatsyTransformer transforms a pandas DataFrame (or dict-like)
-    according to the formula and produces a numpy array.
-
-    Parameters
-    ----------
-    formula : string or formula-like
-        Pasty formula used to transform the data.
-
-    add_intercept : boolean, default=False
-        Wether to add an intersept. By default scikit-learn has built-in
-        intercepts for all models, so we don't add an intercept to the data,
-        even if one is specified in the formula.
-
-    eval_env : environment or int, default=0
-        Envirionment in which to evalute the formula.
-        Defaults to the scope in which PatsyModel was instantiated.
-
-    NA_action : string or NAAction, default="drop"
-        What to do with rows that contain missing values. You can ``"drop"``
-        them, ``"raise"`` an error, or for customization, pass an `NAAction`
-        object.  See ``patsy.NAAction`` for details on what values count as
-        'missing' (and how to alter this).
-
-    Attributes
-    ----------
-    feature_names_ : list of string
-        Column names / keys of training data.
-
-    return_type : string, default="dataframe"
-        data type that transform method will return. Default is ``"dataframe"``
-        for numpy array, but if you would like to get Pandas dataframe (for
-        example for using it in scikit transformers with dataframe as input
-        use ``"dataframe"`` and if numpy array use ``"ndarray"``
-
-    Note
-    ----
-    PastyTransformer does by default not add an intercept, even if you
-    specified it in the formula. You need to set add_intercept=True.
-
-    As scikit-learn transformers can not ouput y, the formula
-    should not contain a left hand side.  If you need to transform both
-    features and targets, use PatsyModel.
-    """
-
-    def __init__(
-        self,
-        formula=None,
-        add_intercept=True,
-        eval_env=0,
-        NA_action="drop",
-        return_type="dataframe",
-    ):
-        self.formula = formula
-        self.eval_env = eval_env
-        self.add_intercept = add_intercept
-        self.NA_action = NA_action
-        self.return_type = return_type
-
-    def fit(self, data, y=None):
-        """Fit the scikit-learn model using the formula.
-
-        Parameters
-        ----------
-        data : dict-like (pandas dataframe)
-            Input data. Column names need to match variables in formula.
-        """
-        self._fit_transform(data, y)
-        return self
-
-    def fit_transform(self, data, y=None):
-        """Fit the scikit-learn model using the formula and transform it.
-
-        Parameters
-        ----------
-        data : dict-like (pandas dataframe)
-            Input data. Column names need to match variables in formula.
-
-        Returns
-        -------
-        X_transform : ndarray
-            Transformed data
-        """
-        return self._fit_transform(data, y)
-
-    def _fit_transform(self, data, y=None):
-        if not isinstance(data, pd.DataFrame):
-            data = pd.DataFrame(data)
-            data.columns = [f"pred_{i}" for i in range(data.shape[1])]
-
-        if not isinstance(y, pd.Series):
-            y = pd.Series(y)
-            y.name = "target"
-
-        target_name = y.name if y is not None else "y"
-        self.formula = self.formula or " + ".join(
-            data.columns.difference([target_name])
-        )
-        eval_env = EvalEnvironment.capture(self.eval_env, reference=2)
-        # self.formula = _drop_intercept(self.formula, self.add_intercept)
-
-        design = dmatrix(
-            self.formula,
-            data,
-            NA_action=self.NA_action,
-            return_type="dataframe",
-            eval_env=eval_env,
-        )
-        self.design_ = design.design_info
-
-        if self.return_type == "dataframe":
-            return design
-        else:
-            return np.array(design)
-
-    def transform(self, data):
-        """Transform with estimator using formula.
-
-        Transform the data using formula, then transform it
-        using the estimator.
-
-        Parameters
-        ----------
-        data : dict-like (pandas dataframe)
-            Input data. Column names need to match variables in formula.
-        """
-        if self.return_type == "dataframe":
-            return dmatrix(self.design_, data, return_type="dataframe")
-        else:
-            return np.array(dmatrix(self.design_, data))
-
-
-def _drop_intercept(formula, add_intercept):
-    """Drop the intercept from formula if not add_intercept"""
-    if not add_intercept:
-        if not isinstance(formula, ModelDesc):
-            formula = ModelDesc.from_formula(formula)
-        if INTERCEPT in formula.rhs_termlist:
-            formula.rhs_termlist.remove(INTERCEPT)
-        return formula
-    return formula
+"""
+This module provides preprocessing classes
+
+Module Structure:
+-----------------
+- ``OrdinalEncoderPandas``: main class for ordinal encoding, takes in a DF and returns a DF of the same shape
+- ``dtype_column_selector``: for standardizing selection of columns based on their dtypes
+- ``TreeDiscretizer``: class for discretizing continuous columns and auto-group levels of categorical columns
+- ``IntervalToMidpoint``: class for converting pandas numerical intervals into their float midpoint
+- ``PatsyTransformer``: class for encoding data for (generalized) linear models, leveraging Patsy
+"""
+
+# Settings and libraries
+from __future__ import print_function
+from tqdm.auto import tqdm
+
+# pandas
+import pandas as pd
+from pandas.api.types import IntervalDtype
+
+# numpy
+import numpy as np
+
+# regular expression
+import re
+
+# sklearn
+from sklearn.preprocessing import OrdinalEncoder
+from sklearn.base import BaseEstimator, TransformerMixin
+
+# patsy
+from patsy import dmatrix, EvalEnvironment, ModelDesc, INTERCEPT
+
+# typing
+from typing import Any, Callable, Union, List, Tuple, Optional, Dict
+
+# ARFS
+from .gbm import GradientBoosting
+from .utils import create_dtype_dict
+
+
+# fix random seed for reproducibility
+np.random.seed(7)
+
+
+class OrdinalEncoderPandas(OrdinalEncoder):
+    # class OrdinalEncoderPandas(BaseEstimator, TransformerMixin):
+    """Encode categorical features as an integer array and returns a pandas DF.
+    The features are converted to ordinal integers. This results in
+    a single column of integers (0 to n_categories - 1) per feature.
+    Read more in the scikit-learn OrdinalEncoder documentation
+
+    Parameters
+    ----------
+    pattern : str, default=None
+        Name of columns containing this regex pattern will be included. If
+        None, column selection will not be selected based on pattern.
+    dtype_include : column dtype or list of column dtypes, default=None
+        A selection of dtypes to include. For more details, see
+        `pandas.DataFrame.select_dtypes`.
+    dtype_exclude : column dtype or list of column dtypes, default=None
+        A selection of dtypes to exclude. For more details, see
+        `pandas.DataFrame.select_dtypes`.
+    exclude_cols : list of str, optional
+        columns to not encode
+    output_dtype : number type, default np.float64
+        Desired dtype of output.
+    handle_unknown : {'error', 'use_encoded_value'}, default='error'
+        When set to 'error' an error will be raised in case an unknown
+        categorical feature is present during transform. When set to
+        'use_encoded_value', the encoded value of unknown categories will be
+        set to the value given for the parameter `unknown_value`. In
+        `inverse_transform`, an unknown category will be denoted as None.
+    unknown_value : int or np.nan, default=None
+        When the parameter handle_unknown is set to 'use_encoded_value', this
+        parameter is required and will set the encoded value of unknown
+        categories. It has to be distinct from the values used to encode any of
+        the categories in `fit`. If set to np.nan, the `dtype` parameter must
+        be a float dtype.
+    encoded_missing_value : int or np.nan, default=np.nan
+        Encoded value of missing categories. If set to `np.nan`, then the `dtype`
+        parameter must be a float dtype.
+    return_pandas_categorical : bool, defult=False
+        return encoded columns as pandas category dtype or as float
+
+    Attributes
+    ----------
+    categories_ : list of arrays
+        The categories of each feature determined during ``fit`` (in order of
+        the features in X and corresponding with the output of ``transform``).
+        This does not include categories that weren't seen during ``fit``.
+    feature_names_in_ : ndarray of shape (`n_features_in_`,)
+        Names of features seen during :term:`fit`. Defined only when `X`
+        has feature names that are all strings.
+
+    Examples
+    --------
+    Given a dataset with two features, we let the encoder find the unique
+    values per feature and transform the data to an ordinal encoding.
+    >>> ord_enc = OrdinalEncoderPandas(exclude_cols=["PARENT1", "SEX"])
+    >>> X_enc = ord_enc.fit_transform(X)
+    >>> X_original = ord_enc.inverse_transform(X_enc)
+    """
+
+    def __init__(
+        self,
+        dtype_include=["category", "object", "bool"],
+        dtype_exclude=[np.number],
+        pattern=None,
+        exclude_cols=None,
+        output_dtype=np.float64,
+        handle_unknown="use_encoded_value",
+        unknown_value=np.nan,
+        encoded_missing_value=np.nan,
+        return_pandas_categorical=False,
+    ):
+        self.dtype_include = dtype_include
+        self.dtype_exclude = dtype_exclude
+        self.pattern = pattern
+        self.exclude_cols = exclude_cols
+        self.output_dtype = output_dtype
+        self.handle_unknown = handle_unknown
+        self.unknown_value = unknown_value
+        self.encoded_missing_value = encoded_missing_value
+        self.return_pandas_categorical = return_pandas_categorical
+
+        super().__init__(
+            categories="auto",
+            dtype=self.output_dtype,
+            handle_unknown=self.handle_unknown,
+            unknown_value=self.unknown_value,
+            encoded_missing_value=self.encoded_missing_value,
+        )
+
+    def fit(self, X, y=None):
+        """
+        Fit the OrdinalEncoder to X.
+
+        Parameters
+        ----------
+        X : pd.DataFrame, of shape (n_samples, n_features)
+            The data to determine the categories of each feature.
+        y : Ignored. This parameter exists only for compatibility with
+            :class:`~sklearn.pipeline.Pipeline`.
+
+        Returns
+        -------
+        self :
+            Fitted encoder.
+        """
+
+        cat_features_selector = dtype_column_selector(
+            dtype_include=self.dtype_include,
+            dtype_exclude=self.dtype_exclude,
+            pattern=self.pattern,
+            exclude_cols=self.exclude_cols,
+        )
+
+        self.feature_names_in_ = X.columns.to_numpy()
+        self.categorical_features_ = cat_features_selector(X)
+
+        super(OrdinalEncoderPandas, self).fit(X[self.categorical_features_])
+        # self.feature_names_in_ = X.columns.to_numpy()
+        return self
+
+    def transform(self, X, y=None, sample_weight=None):
+        """
+        Transform X to ordinal codes.
+
+        Parameters
+        ----------
+        X : pd.DataFrame of shape (n_samples, n_features)
+            The data to encode.
+
+        Returns
+        -------
+        X_out : pd.DataFrame (n_samples, n_features)
+            Transformed input.
+        """
+        X_trans = X.copy()
+        X_trans[self.categorical_features_] = super(
+            OrdinalEncoderPandas, self
+        ).transform(X_trans[self.categorical_features_])
+
+        if self.return_pandas_categorical:
+            X_trans[self.categorical_features_] = X_trans[
+                self.categorical_features_
+            ].astype("category")
+        return X_trans
+
+    def fit_transform(self, X, y=None, sample_weight=None, **fit_params):
+        """
+        Fit to data, then transform it.
+        Fits transformer to `X` and `y` with optional parameters `fit_params`
+        and returns a transformed version of `X`.
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input samples.
+        y :  array-like of shape (n_samples,) or (n_samples, n_outputs), \
+                default=None
+            Target values (None for unsupervised transformations).
+        **fit_params : dict
+            Additional fit parameters.
+        Returns
+        -------
+        X_new : ndarray array of shape (n_samples, n_features_new)
+            Transformed array.
+        """
+        self = self.fit(X)
+        return self.transform(X)
+
+    def inverse_transform(self, X):
+        """
+        Convert the data back to the original representation.
+        When unknown categories are encountered (all zeros in the
+        one-hot encoding), ``None`` is used to represent this category. If the
+        feature with the unknown category has a dropped category, the dropped
+        category will be its inverse.
+        For a given input feature, if there is an infrequent category,
+        'infrequent_sklearn' will be used to represent the infrequent category.
+
+        Parameters
+        ----------
+        X : pd.DataFrame of shape (n_samples, n_encoded_features)
+            The transformed data.
+        Returns
+        -------
+        X_tr : pd.Dataframe of shape (n_samples, n_features)
+            Inverse transformed array.
+        """
+
+        X[self.categorical_features_] = super(
+            OrdinalEncoderPandas, self
+        ).inverse_transform(X[self.categorical_features_])
+        return X
+
+
+class dtype_column_selector:
+    """Create a callable to select columns to be used with
+    :class:`ColumnTransformer`.
+    :func:`dtype_column_selector` can select columns based on datatype or the
+    columns name with a regex. When using multiple selection criteria, **all**
+    criteria must match for a column to be selected.
+
+    Parameters
+    ----------
+    pattern : str, default=None
+        Name of columns containing this regex pattern will be included. If
+        None, column selection will not be selected based on pattern.
+    dtype_include : column dtype or list of column dtypes, default=None
+        A selection of dtypes to include. For more details, see
+        :meth:`pandas.DataFrame.select_dtypes`.
+    dtype_exclude : column dtype or list of column dtypes, default=None
+        A selection of dtypes to exclude. For more details, see
+        :meth:`pandas.DataFrame.select_dtypes`.
+    exclude_cols : list of column names, default=None
+        A selection of columns to exclude
+
+    Returns
+    -------
+    selector : callable
+        Callable for column selection to be used by a
+        :class:`ColumnTransformer`.
+
+    See Also
+    --------
+    ColumnTransformer : Class that allows combining the
+        outputs of multiple transformer objects used on column subsets
+        of the data into a single feature space.
+
+    Examples
+    --------
+    >>> from sklearn.preprocessing import StandardScaler, OneHotEncoder
+    >>> from sklearn.compose import make_column_transformer
+    >>> from arfs.preprocessing import dtype_column_selector
+    >>> import numpy as np
+    >>> import pandas as pd  # doctest: +SKIP
+    >>> X = pd.DataFrame({'city': ['London', 'London', 'Paris', 'Sallisaw'],
+    ...                   'rating': [5, 3, 4, 5]})  # doctest: +SKIP
+    >>> ct = make_column_transformer(
+    ...       (StandardScaler(),
+    ...        dtype_column_selector(dtype_include=np.number)),  # rating
+    ...       (OneHotEncoder(),
+    ...        dtype_column_selector(dtype_include=object)))  # city
+    >>> ct.fit_transform(X)
+    array([[ 0.90453403,  1.        ,  0.        ,  0.        ],
+           [-1.50755672,  1.        ,  0.        ,  0.        ],
+           [-0.30151134,  0.        ,  1.        ,  0.        ],
+           [ 0.90453403,  0.        ,  0.        ,  1.        ]])
+    """
+
+    def __init__(
+        self, pattern=None, *, dtype_include=None, dtype_exclude=None, exclude_cols=None
+    ):
+        self.pattern = pattern
+        self.dtype_include = dtype_include
+        self.dtype_exclude = dtype_exclude
+        self.exclude_cols = exclude_cols
+
+    def __call__(self, df):
+        """Callable for column selection to be used by a
+        :class:`ColumnTransformer`.
+        Parameters
+        ----------
+        df : pd.DataFrame of shape (n_features, n_samples)
+            DataFrame to select columns from.
+        """
+        if not hasattr(df, "iloc"):
+            raise ValueError(
+                "make_column_selector can only be applied to pandas dataframes"
+            )
+        df_row = df.iloc[:1]
+        if self.dtype_include is not None or self.dtype_exclude is not None:
+            df_row = df_row.select_dtypes(
+                include=self.dtype_include, exclude=self.dtype_exclude
+            )
+        cols = df_row.columns
+        if self.pattern is not None:
+            cols = cols[cols.str.contains(self.pattern, regex=True)]
+
+        if self.exclude_cols is not None:
+            cols = cols[~cols.isin(self.exclude_cols)]
+
+        return cols.tolist()
+
+
+def cat_var(data, col_excl=None, return_cat=True):
+    """Ad hoc categorical encoding (as integer). Automatically detect the non-numerical columns,
+    save the index and name of those columns, encode them as integer,
+    save the direct and inverse mappers as
+    dictionaries.
+    Return the data-set with the encoded columns with a data type either int or pandas categorical.
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        the dataset
+    col_excl: list of str, default=None
+        the list of columns names not being encoded (e.g. the ID column)
+    return_cat: bool, default=True
+        return encoded object columns as pandas categoricals or not.
+
+    Returns
+    -------
+    df: pd.DataFrame
+        the dataframe with encoded columns
+    cat_var_df: pd.DataFrame
+        the dataframe with the indices and names of the categorical columns
+    inv_mapper: dict
+        the dictionary to map integer --> category
+    mapper: dict
+        the dictionary to map category --> integer
+    """
+    df = data.copy()
+    if col_excl is None:
+        non_num_cols = list(
+            set(list(df.columns)) - set(list(df.select_dtypes(include=[np.number])))
+        )
+    else:
+        non_num_cols = list(
+            set(list(df.columns))
+            - set(list(df.select_dtypes(include=[np.number])))
+            - set(col_excl)
+        )
+    cat_var_index = [df.columns.get_loc(c) for c in non_num_cols if c in df]
+    cat_var_df = pd.DataFrame({"cat_ind": cat_var_index, "cat_name": non_num_cols})
+    # avoid having datetime objects as keys in the mapping dic
+    date_cols = [s for s in list(df) if "date" in s]
+    df.loc[:, date_cols] = df.loc[:, date_cols].astype(str)
+    cols_need_mapped = cat_var_df.cat_name.to_list()
+    inv_mapper = {
+        col: dict(enumerate(df[col].astype("category").cat.categories))
+        for col in df[cols_need_mapped]
+    }
+    mapper = {
+        col: {v: k for k, v in inv_mapper[col].items()} for col in df[cols_need_mapped]
+    }
+    progress_bar = tqdm(cols_need_mapped)
+    for c in progress_bar:
+        progress_bar.set_description("Processing {0:<30}".format(c))
+        df.loc[:, c] = df.loc[:, c].map(mapper[c]).fillna(0).astype(int)
+        # I could have use df[c].update(df[c].map(mapper[c])) while slower,
+        # prevents values not included in an incomplete map from being changed to nans.
+        # But then I could have outputs
+        # with mixed types in the case of different dtypes mapping (like str -> int).
+        # This would eventually break any flow.
+        # Map is faster than replace
+    if return_cat:
+        df.loc[:, non_num_cols] = df.loc[:, non_num_cols].astype("category")
+    return df, cat_var_df, inv_mapper, mapper
+
+
+class TreeDiscretizer(BaseEstimator, TransformerMixin):
+    """
+    Discretize continuous and/or categorical data using univariate regularized trees, returning a pandas DataFrame.
+    The TreeDiscretizer is designed to support regression and binary classification tasks.
+    Discretization, also known as quantization or binning, allows for the partitioning of continuous features into discrete values.
+    In certain datasets with continuous attributes, discretization can be beneficial as it transforms the dataset into one with only nominal attributes.
+    Additionally, for categorical predictors, grouping levels can help reduce overfitting and create meaningful clusters.
+
+    By encoding discretized features, a model can become more expressive while maintaining interpretability.
+    For example, preprocessing with a discretizer can introduce nonlinearity to linear models.
+    For more advanced possibilities, particularly smooth ones, you can refer to the section on generating polynomial features.
+    The TreeDiscretizer function utilizes univariate regularized trees, with one tree per column to be binned.
+    It finds the optimal partition and returns numerical intervals for numerical continuous columns and pd.Categorical for categorical columns.
+    This approach groups similar levels together, reducing dimensionality and regularizing the model.
+
+    TreeDiscretizer handles missing values for both numerical and categorical predictors,
+    eliminating the need for encoding categorical predictors separately.
+
+    Notes
+    -----
+    This is a substitution to proper regularization schemes such as:
+    - GroupLasso: Categorical predictors, which are usually encoded as multiple dummy variables,
+                  are considered together rather than separately.
+    - FusedLasso: Takes into account the ordering of the features.
+
+    Parameters
+    ----------
+    bin_features : List of string or None
+        The list of names of the variable that has to be binned, or "all", "numerical" or "categorical"
+        for splitting and grouping all, only numerical or only categorical columns.
+    n_bins : int
+        The number of bins that has to be created while binning the variables in the "bin_features" list.
+    n_bins_max : int, optional
+        The maximum number of levels that a categorical column can have to avoid being binned.
+    num_bins_as_category: bool, default=False
+        Save the numeric bins as pandas category or as pandas interval.
+    boost_params : dict
+        The boosting parameters dictionary.
+    raw : bool
+        Returns raw levels (non-human-interpretable) or levels matching the original ones.
+    task : str
+        Either regression or classification (binary).
+
+    Attributes
+    ----------
+    tree_dic : dict
+        The dictionary keys are binned column names and items are the univariate trees.
+    bin_upper_bound_dic : dict
+        The upper bound of the numerical intervals.
+    cat_bin_dict : dict
+        The mapping dictionary for the categorical columns.
+    tree_imputer : dict
+        The missing values are split by the tree and lead to similar splits and are mapped to this value.
+    ordinal_encoder_dic : dict
+        Dictionary with the fitted encoder, if any.
+    cat_features : list
+        Names of the found categorical columns.
+
+    Methods
+    -------
+    fit(X, y, sample_weight=None)
+        Fit the transformer object on data.
+    transform(X)
+        Apply the fitted transformer object on new data.
+    fit_transform(X)
+        Fit and apply the transformer object on data.
+
+    Example
+    -------
+    >>> lgb_params = {'min_split_gain': 5}
+    >>> disc = TreeDiscretizer(bin_features='all', n_bins=10)
+    >>> disc.fit(X=df[predictors], y=df['Frequency'], sample_weight=df['Exposure'])
+    """
+
+    def __init__(
+        self,
+        bin_features="all",
+        n_bins=10,
+        n_bins_max=None,
+        num_bins_as_category=False,
+        boost_params=None,
+        raw=False,
+        task="regression",
+    ):
+        if (boost_params is not None) & (not isinstance(boost_params, dict)):
+            raise TypeError("boost_kwargs should be a dictionary")
+
+        self.bin_features = bin_features
+        self.n_bins = n_bins
+        self.n_bins_max = n_bins_max
+        self.num_bins_as_category = num_bins_as_category
+        self.boost_params = {}
+        self.raw = raw
+        self.task = task
+        if boost_params is not None:
+            self.boost_params = boost_params
+
+        # force some params
+        if self.task == "regression":
+            self.boost_params["objective"] = "RMSE"
+        elif self.task == "classification":
+            self.boost_params["objective"] = "binary"
+
+        self.boost_params["num_boost_round"] = 1
+        self.boost_params["max_leaf"] = self.n_bins
+        self.tree_dic = {}
+        self.bin_upper_bound_dic = {}
+        self.cat_bin_dict = {}
+        self.tree_imputer = {}
+        self.ordinal_encoder_dic = {}
+        self.cat_features = None
+
+    def fit(self, X, y, sample_weight=None):
+        """
+        Fit the TreeDiscretizer on the input data.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            The predictor dataframe.
+        y : array-like of shape (n_samples,)
+            The target vector.
+        sample_weight : array-like of shape (n_samples,), optional
+            The weight vector, by default None.
+
+        Returns
+        -------
+        self : object
+            Returns self.
+        """
+        X = X.copy()
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+            X.columns = [f"pred_{i}" for i in range(X.shape[1])]
+
+        self.feature_names_in_ = X.columns.to_numpy()
+
+        if self.bin_features is None:
+            self.bin_features = list(X.select_dtypes("number").columns)
+            self.cat_features = []
+        elif isinstance(self.bin_features, list):
+            self.cat_features = list(
+                set(self.bin_features)
+                - set(list(X[self.bin_features].select_dtypes("number").columns))
+            )
+        elif isinstance(self.bin_features, str) and (self.bin_features == "all"):
+            self.bin_features = list(X.columns)
+            self.cat_features = list(
+                set(self.bin_features) - set(list(X.select_dtypes("number").columns))
+            )
+        elif isinstance(self.bin_features, str) and (self.bin_features == "numerical"):
+            self.bin_features = list(X.select_dtypes("number").columns)
+        elif isinstance(self.bin_features, str) and (
+            self.bin_features == "categorical"
+        ):
+            self.bin_features = list(X.select_dtypes(["category", "object"]).columns)
+            self.cat_features = self.bin_features
+
+        self.n_unique_table_ = X[self.bin_features].nunique()
+        # transform only the columns with more than n_bins_max
+        self.bin_features = (
+            self.n_unique_table_[self.n_unique_table_ > self.n_bins_max].index.to_list()
+            if self.n_bins_max
+            else self.bin_features
+        )
+
+        for col in self.bin_features:
+            is_categorical = (self.cat_features is not None) and (
+                col in self.cat_features
+            )
+            if is_categorical:
+                encoder = OrdinalEncoder(
+                    handle_unknown="use_encoded_value", unknown_value=np.nan
+                )
+                # create a category for missing
+                X[col] = (
+                    X[col]
+                    .astype("category")
+                    .cat.add_categories("missing_added")
+                    .fillna("missing_added")
+                )
+                # encode
+                self.ordinal_encoder_dic[col] = encoder.fit(X[[col]])
+                dum = encoder.transform(X[[col]])
+                if isinstance(dum, pd.DataFrame):
+                    X[col] = dum.values.ravel()
+                else:
+                    X[col] = dum.ravel()
+
+            else:
+                encoder = None
+
+            gbm_param = self.boost_params.copy()
+            tree = GradientBoosting(
+                cat_feat=None, params=gbm_param, show_learning_curve=False
+            )
+            tree.fit(X[[col]], y, sample_weight=sample_weight)
+
+            # store each fitted tree in a dictionary
+            self.tree_dic[col] = tree
+
+            # create the bins series
+            # predict, group by original values
+            # create monotonicly increasing bin for pd.cut
+            X[f"{col}_g"] = tree.predict(X[[col]])
+
+            if is_categorical:
+                # retrieve original values
+                dum = encoder.inverse_transform(X[[col]])
+                if isinstance(dum, pd.DataFrame):
+                    X[col] = dum.values.ravel()
+                else:
+                    X[col] = dum.ravel()
+
+                self.cat_bin_dict[col] = (
+                    X[[f"{col}_g", col]]
+                    .groupby(f"{col}_g")
+                    .apply(lambda x: " / ".join(map(str, x[col].unique())))
+                    .to_dict()
+                )
+            else:
+                bin_array = (
+                    X[[f"{col}_g", col]]
+                    .groupby(f"{col}_g")
+                    .aggregate(max)
+                    .sort_values(col)
+                    .values.ravel()
+                )
+                # overwrite max for handling unseen larger values than max val on the train set
+                bin_array = np.delete(bin_array, [np.argmax(bin_array)])
+                # append -Inf and Inf for covering the whole interval, as in KBinsDiscretizer
+                bin_array = np.unique(np.append(bin_array, [-np.Inf, np.Inf]))
+                self.bin_upper_bound_dic[col] = bin_array
+                # the tree imputer: if nan is passed, the predicted value will be the
+                # same than another non-missing value and nan should fall into this bin
+                # the predicted value of a NaN
+                nan_pred_val = tree.predict(np.expand_dims([np.nan], axis=1))[0]
+                # the closest predicted value for non NaN inputs
+                non_nan_values = X[col].dropna().unique()
+                pred_values = tree.predict(np.expand_dims(non_nan_values, axis=1))
+                # store the value for knowing the bin into which the NaN should fall
+                self.tree_imputer[col] = non_nan_values.flat[
+                    np.abs(pred_values - nan_pred_val).argmin()
+                ]
+
+            del tree
+
+        return self
+
+    def transform(self, X):
+        """
+        Apply the discretizer on `X`. Only the columns with more than n_bins_max unique values will be transformed.
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Input data with shape (n_samples, n_features), where `n_samples` is the number of samples and
+            `n_features` is the number of features.
+
+        Returns
+        -------
+        X : pd.DataFrame
+            DataFrame with the binned and grouped columns.
+        """
+        X = X.copy()
+
+        for col in self.bin_features:
+            if self.raw:
+                # predict each univariate tree
+                X[col] = self.tree_dic[col].predict(X[[col]])
+            else:
+                if (self.cat_features is not None) and (col in self.cat_features):
+                    # apply the systematic imputation (missing might be grouped
+                    # with other categories depending on the results of the tree
+                    # splitting)
+                    X[col] = (
+                        X[col]
+                        .astype("category")
+                        .cat.add_categories("missing_added")
+                        .fillna("missing_added")
+                    )
+                    dum = self.ordinal_encoder_dic[col].transform(X[[col]])
+                    X[col] = self.tree_dic[col].predict(dum)
+                    X[col] = X[col].map(self.cat_bin_dict[col])
+                else:
+                    # retrieve the association the tree learnt for missing values
+                    X[col].fillna(self.tree_imputer[col], inplace=True)
+                    # apply the binning
+                    X[col] = pd.cut(
+                        X[col],
+                        bins=self.bin_upper_bound_dic[col],
+                        include_lowest=True,
+                        precision=2,
+                    )
+
+                    if not self.num_bins_as_category:
+                        X[col] = X[col].astype(IntervalDtype())
+        return X
+
+
+def highlight_discarded(s):
+    """
+    highlight X in red and V in green.
+
+    Parameters
+    ----------
+    s : np.arrays
+
+    Returns
+    -------
+    list
+
+    """
+    is_X = s == 0
+    return [
+        "background-color: #d65f5f" if v else "background-color: #33a654" for v in is_X
+    ]
+
+
+class IntervalToMidpoint(BaseEstimator, TransformerMixin):
+    """
+    IntervalToMidpoint is a transformer that converts numerical intervals in a pandas DataFrame to their midpoints.
+
+    Parameters
+    ----------
+    cols : list of str or str, default "all"
+        The column(s) to transform. If "all", all columns with numerical intervals will be transformed.
+
+    Attributes
+    ----------
+    cols : list of str or str
+        The column(s) to transform.
+    float_interval_cols_ : list of str
+        The columns with numerical interval data types in the input DataFrame.
+    columns_to_transform_ : list of str
+        The columns to be transformed based on the specified `cols` attribute.
+
+    Methods
+    -------
+    fit(X, y=None)
+        Fit the transformer on the input data.
+    transform(X)
+        Transform the input data by converting numerical intervals to midpoints.
+    inverse_transform(X)
+        Inverse transform is not implemented for this transformer.
+    """
+
+    def __init__(self, cols: Union[List[str], str] = "all"):
+        self.cols = cols
+
+    def fit(self, X: pd.DataFrame = None, y: pd.Series = None):
+        """
+        Fit the transformer on the input data.
+
+        Parameters
+        ----------
+        X :
+            The input data to fit the transformer on.
+        y :
+            Ignored parameter.
+
+        Returns
+        -------
+        self : IntervalToMidpoint
+            The fitted transformer object.
+        """
+        data = X.copy()
+
+        if self.cols == "all":
+            self.cols = data.columns
+
+        self.float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")[
+            "num_interval"
+        ]
+        self.columns_to_transform_ = list(
+            set(self.cols).intersection(set(self.float_interval_cols_))
+        )
+        return self
+
+    def transform(self, X: pd.DataFrame):
+        """
+        Transform the input data by converting numerical intervals to midpoints.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            The input data to transform.
+
+        Returns
+        -------
+        X : pd.DataFrame
+            The transformed data with numerical intervals replaced by their midpoints.
+        """
+        X = X.copy()
+        for c in self.columns_to_transform_:
+            X.loc[:, c] = find_interval_midpoint(X[c])
+            X.loc[:, c] = X[c].astype(float)
+        return X
+
+    def inverse_transform(self, X: pd.DataFrame):
+        """
+        Inverse transform is not implemented for this transformer.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            The input data to perform inverse transform on.
+
+        Raises
+        ------
+        NotImplementedError
+            Raised since inverse transform is not implemented for this transformer.
+        """
+        raise NotImplementedError(
+            "inverse_transform is not implemented for this transformer."
+        )
+
+
+def transform_interval_to_midpoint(
+    X: pd.DataFrame, cols: Union[List[str], str] = "all"
+) -> pd.DataFrame:
+    """
+    Transforms interval columns in a pandas DataFrame to their midpoint values.
+
+    Notes
+    -----
+    Equivalent function to ``IntervalToMidpoint`` without the estimator API
+
+    Parameters
+    ----------
+    X : pd.DataFrame
+        The input DataFrame containing the data to be transformed.
+    cols : list of str or str
+        The columns to be transformed. Defaults to "all" which transforms all columns.
+
+    Returns
+    -------
+    pd.DataFrame :
+        The transformed DataFrame with interval columns replaced by their midpoint values.
+
+    Raises
+    ------
+    TypeError :
+        If the input data is not a pandas DataFrame.
+    """
+    if cols == "all":
+        cols = X.columns
+
+    X = X.copy()
+    float_interval_cols_ = create_dtype_dict(X, dic_keys="dtypes")["num_interval"]
+    columns_to_transform_ = list(set(cols).intersection(set(float_interval_cols_)))
+    for c in columns_to_transform_:
+        X.loc[:, c] = find_interval_midpoint(X[c])
+    return X
+
+
+def find_interval_midpoint(interval_series: pd.Series) -> np.ndarray:
+    """Find the midpoint (or left/right bound if the interval contains Inf).
+
+    Parameters
+    ----------
+    interval_series : pd.Series
+        series of pandas intervals.
+
+    Returns
+    -------
+    np.ndarray
+        Array of midpoints or bounds of the intervals.
+    """
+    left = interval_series.array.left
+    right = interval_series.array.right
+    mid = interval_series.array.mid
+    left_inf = np.isinf(left)
+    right_inf = np.isinf(right)
+
+    return np.where(
+        left_inf & right_inf,
+        np.inf,
+        np.where(left_inf, right, np.where(right_inf, left, mid)),
+    )
+
+
+class PatsyTransformer(BaseEstimator, TransformerMixin):
+    """Transformer using patsy-formulas.
+
+    PatsyTransformer transforms a pandas DataFrame (or dict-like)
+    according to the formula and produces a numpy array.
+
+    Parameters
+    ----------
+    formula : string or formula-like
+        Pasty formula used to transform the data.
+
+    add_intercept : boolean, default=False
+        Wether to add an intersept. By default scikit-learn has built-in
+        intercepts for all models, so we don't add an intercept to the data,
+        even if one is specified in the formula.
+
+    eval_env : environment or int, default=0
+        Envirionment in which to evalute the formula.
+        Defaults to the scope in which PatsyModel was instantiated.
+
+    NA_action : string or NAAction, default="drop"
+        What to do with rows that contain missing values. You can ``"drop"``
+        them, ``"raise"`` an error, or for customization, pass an `NAAction`
+        object.  See ``patsy.NAAction`` for details on what values count as
+        'missing' (and how to alter this).
+
+    Attributes
+    ----------
+    feature_names_ : list of string
+        Column names / keys of training data.
+
+    return_type : string, default="dataframe"
+        data type that transform method will return. Default is ``"dataframe"``
+        for numpy array, but if you would like to get Pandas dataframe (for
+        example for using it in scikit transformers with dataframe as input
+        use ``"dataframe"`` and if numpy array use ``"ndarray"``
+
+    Note
+    ----
+    PastyTransformer does by default not add an intercept, even if you
+    specified it in the formula. You need to set add_intercept=True.
+
+    As scikit-learn transformers can not ouput y, the formula
+    should not contain a left hand side.  If you need to transform both
+    features and targets, use PatsyModel.
+    """
+
+    def __init__(
+        self,
+        formula=None,
+        add_intercept=True,
+        eval_env=0,
+        NA_action="drop",
+        return_type="dataframe",
+    ):
+        self.formula = formula
+        self.eval_env = eval_env
+        self.add_intercept = add_intercept
+        self.NA_action = NA_action
+        self.return_type = return_type
+
+    def fit(self, data, y=None):
+        """Fit the scikit-learn model using the formula.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+        """
+        self._fit_transform(data, y)
+        return self
+
+    def fit_transform(self, data, y=None):
+        """Fit the scikit-learn model using the formula and transform it.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+
+        Returns
+        -------
+        X_transform : ndarray
+            Transformed data
+        """
+        return self._fit_transform(data, y)
+
+    def _fit_transform(self, data, y=None):
+        if not isinstance(data, pd.DataFrame):
+            data = pd.DataFrame(data)
+            data.columns = [f"pred_{i}" for i in range(data.shape[1])]
+
+        if not isinstance(y, pd.Series):
+            y = pd.Series(y)
+            y.name = "target"
+
+        target_name = y.name if y is not None else "y"
+        self.formula = self.formula or " + ".join(
+            data.columns.difference([target_name])
+        )
+        eval_env = EvalEnvironment.capture(self.eval_env, reference=2)
+        # self.formula = _drop_intercept(self.formula, self.add_intercept)
+
+        design = dmatrix(
+            self.formula,
+            data,
+            NA_action=self.NA_action,
+            return_type="dataframe",
+            eval_env=eval_env,
+        )
+        self.design_ = design.design_info
+
+        if self.return_type == "dataframe":
+            return design
+        else:
+            return np.array(design)
+
+    def transform(self, data):
+        """Transform with estimator using formula.
+
+        Transform the data using formula, then transform it
+        using the estimator.
+
+        Parameters
+        ----------
+        data : dict-like (pandas dataframe)
+            Input data. Column names need to match variables in formula.
+        """
+        if self.return_type == "dataframe":
+            return dmatrix(self.design_, data, return_type="dataframe")
+        else:
+            return np.array(dmatrix(self.design_, data))
+
+
+def _drop_intercept(formula, add_intercept):
+    """Drop the intercept from formula if not add_intercept"""
+    if not add_intercept:
+        if not isinstance(formula, ModelDesc):
+            formula = ModelDesc.from_formula(formula)
+        if INTERCEPT in formula.rhs_termlist:
+            formula.rhs_termlist.remove(INTERCEPT)
+        return formula
+    return formula
```

### Comparing `arfs-2.0.4/src/arfs/sampling.py` & `arfs-2.0.5/src/arfs/sampling.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,477 +1,477 @@
-"""This module provide methods for sampling large datasets for reducing the running time
-"""
-import numpy as np
-import pandas as pd
-from scipy.sparse import issparse
-from collections import Counter
-from sklearn.cluster import AgglomerativeClustering
-from sklearn.ensemble import IsolationForest
-from scipy.stats import ks_2samp
-from .utils import is_list_of_str, is_list_of_bool, is_list_of_int
-
-
-def sample(df, n=1000, sample_weight=None, method="gower"):
-    """Sampling rows from a dataframe when random sampling is not
-    enough for reducing the number of rows.
-    The strategies are either using hierarchical clustering
-    based on the Gower distance or using isolation forest for identifying
-    the most similar elements.
-    For the clustering algorithm, clusters are determined using the Gower distance
-    (mixed type data) and the dataset is shrunk from n_samples to n_clusters.
-
-    For the isolation forest algorithm, samples are added till a suffisant 2-samples
-    KS statistics is reached or if the number iteration reached the max number (20)
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        the dataframe to sample, with or without the target
-    n : int, optional
-        the number of clusters if method is ``"gower"``, by default 100
-    sample_weight : pd.Series or np.array, optional
-        sample weights, by default None
-    method : str, optional
-        the strategy to use for sampling the rows. Either ``"gower"`` or ``"isoforest"``, by default 'gower'
-
-    Returns
-    -------
-    pd.DataFrame
-        the sampled dataframe
-
-    """
-    assert isinstance(df, pd.DataFrame), "X should be a DataFrame"
-    X = df.copy()
-    num_cols = list(X.select_dtypes(include=[np.number]))
-    non_num_cols = list(set(list(X.columns)) - set(num_cols))
-
-    if method == "gower":
-        # basic imputation
-        if non_num_cols:
-            X[non_num_cols] = X[non_num_cols].fillna(X[non_num_cols].mode().iloc[0])
-        if num_cols:
-            X[num_cols] = X[num_cols].fillna(X[num_cols].mean().iloc[0])
-
-        # no need for scaling, it is built-in the computation of the Gower distance
-        gd = gower_matrix(X, cat_features=non_num_cols, weight=sample_weight)
-
-        labels = AgglomerativeClustering(
-            n_clusters=n, affinity="precomputed", linkage="complete"
-        ).fit_predict(gd)
-        X["label"] = labels
-        X["label"] = "clus_" + X["label"].astype(str)
-        X_num = X.groupby("label")[num_cols].agg("mean")
-        if non_num_cols:
-            X_nonnum = X.groupby("label")[non_num_cols].agg(get_most_common)
-            X_sampled = X_num.join(X_nonnum)
-        else:
-            X_sampled = X_num
-        X_sampled = X_sampled.reindex(X.columns, axis=1)
-        return X_sampled
-    elif method == "isoforest":
-        X[non_num_cols] = X[non_num_cols].astype("str").astype("category")
-        for col in non_num_cols:
-            X[col] = X[col].astype("category").cat.codes
-        idx = isof_find_sample(X, sample_weight=None)
-        return X.iloc[idx, :]
-    else:
-        NotImplementedError(f"{method} not implemented")
-
-
-def get_most_common(srs):
-    x = list(srs)
-    my_counter = Counter(x)
-    return my_counter.most_common(1)[0][0]
-
-
-def gower_matrix(
-    data_x,
-    data_y=None,
-    weight=None,
-    cat_features="auto",
-):
-    """Computes the gower distances between X and Y
-
-    Gower is a similarity measure for categorical, boolean and numerical mixed
-    data.
-
-    Parameters
-    ----------
-    data_x : np.array or pd.DataFrame
-        The data for computing the Gower distance
-    data_y : np.array or pd.DataFrame or pd.Series, optional
-        The reference matrix or vector to compare with, optional
-    weight : np.array or pd.Series, optional
-        sample weight, optional
-    cat_features : list of str or bool or int, optional
-        auto-detect cat features or a list of cat features, by default 'auto'
-
-    Returns
-    -------
-    np.array
-        The Gower distance matrix, shape (n_samples, n_samples)
-
-    Notes
-    -----
-    The non-numeric features, and numeric feature ranges are determined from X and not Y.
-
-    Raises
-    ------
-    TypeError
-        If two dataframes are passed but have different number of columns
-    TypeError
-        If two arrays are passed but have different number of columns
-    TypeError
-        Sparse matrices are not supported
-    TypeError
-        if a list of categorical columns is passed, it should be a list of strings or integers or boolean values
-    """
-    # function checks
-    X = data_x
-    if data_y is None:
-        Y = data_x
-    else:
-        Y = data_y
-    if not isinstance(X, np.ndarray):
-        y_col = Y.columns if isinstance(Y, pd.DataFrame) else Y.index
-        if not np.array_equal(X.columns, y_col):
-            raise TypeError("X and Y must have same columns!")
-    else:
-        if not X.shape[1] == Y.shape[1]:
-            raise TypeError("X and Y must have same y-dim!")
-    if issparse(X) or issparse(Y):
-        raise TypeError("Sparse matrices are not supported!")
-
-    x_n_rows, x_n_cols = X.shape
-    y_n_rows, y_n_cols = Y.shape
-
-    if cat_features == "auto":
-        if not isinstance(X, np.ndarray):
-            is_number = np.vectorize(lambda x: not np.issubdtype(x, np.number))
-            cat_features = is_number(X.dtypes)
-        else:
-            cat_features = np.zeros(x_n_cols, dtype=bool)
-            for col in range(x_n_cols):
-                if not np.issubdtype(type(X[0, col]), np.number):
-                    cat_features[col] = True
-    else:
-        # force categorical columns (if integer encoded for instance)
-        if is_list_of_str(cat_features):
-            cat_feat = [True if c in cat_features else False for c in X.columns]
-            cat_features = np.array(cat_feat)
-        elif is_list_of_bool(cat_features):
-            cat_features = np.array(cat_features)
-        elif is_list_of_int(cat_features):
-            cat_feat = [
-                True if c in cat_features else False for c in range(len(X.columns))
-            ]
-            cat_features = np.array(cat_feat)
-        else:
-            raise TypeError(
-                "If not 'auto' cat_features should be a list of strings, integers or Booleans"
-            )
-
-    # print(cat_features)
-
-    if not isinstance(X, np.ndarray):
-        X = np.asarray(X)
-    if not isinstance(Y, np.ndarray):
-        Y = np.asarray(Y)
-
-    Z = np.concatenate((X, Y))
-
-    x_index = range(0, x_n_rows)
-    y_index = range(x_n_rows, x_n_rows + y_n_rows)
-
-    Z_num = Z[:, np.logical_not(cat_features)]
-
-    num_cols = Z_num.shape[1]
-    num_ranges = np.zeros(num_cols)
-    num_max = np.zeros(num_cols)
-
-    for col in range(num_cols):
-        col_array = Z_num[:, col].astype(np.float32)
-        max_ = np.nanmax(col_array)
-        min_ = np.nanmin(col_array)
-
-        if np.isnan(max_):
-            max_ = 0.0
-        if np.isnan(min_):
-            min_ = 0.0
-        num_max[col] = max_
-        num_ranges[col] = (1 - min_ / max_) if (max_ != 0) else 0.0
-
-    # This is to normalize the numeric values between 0 and 1.
-    Z_num = np.divide(
-        Z_num.astype(float),
-        num_max.astype(float),
-        out=np.zeros_like(Z_num).astype(float),
-        where=num_max != 0,
-    )
-    Z_cat = Z[:, cat_features]
-
-    if weight is None:
-        weight = np.ones(Z.shape[1])
-
-    # print(weight)
-
-    weight_cat = weight[cat_features]
-    weight_num = weight[np.logical_not(cat_features)]
-
-    out = np.zeros((x_n_rows, y_n_rows), dtype=np.float32)
-
-    weight_sum = weight.sum()
-
-    X_cat = Z_cat[x_index,]
-    X_num = Z_num[x_index,]
-    Y_cat = Z_cat[y_index,]
-    Y_num = Z_num[y_index,]
-
-    # print(X_cat,X_num,Y_cat,Y_num)
-
-    for i in range(x_n_rows):
-        j_start = i
-        if x_n_rows != y_n_rows:
-            j_start = 0
-        # call the main function
-        res = _gower_distance_row(
-            X_cat[i, :],
-            X_num[i, :],
-            Y_cat[j_start:y_n_rows, :],
-            Y_num[j_start:y_n_rows, :],
-            weight_cat,
-            weight_num,
-            weight_sum,
-            num_ranges,
-        )
-        # print(res)
-        out[i, j_start:] = res
-        if x_n_rows == y_n_rows:
-            out[i:, j_start] = res
-
-    return out
-
-
-def _gower_distance_row(
-    xi_cat,
-    xi_num,
-    xj_cat,
-    xj_num,
-    feature_weight_cat,
-    feature_weight_num,
-    feature_weight_sum,
-    ranges_of_numeric,
-):
-    """Compute a row of the Gower matrix
-
-    Parameters
-    ----------
-    xi_cat : np.array
-        categorical row of the X matrix
-    xi_num : np.array
-        numerical row of the X matrix
-    xj_cat : np.array
-        categorical row of the X matrix
-    xj_num : np.array
-        numerical row of the X matrix
-    feature_weight_cat : np.array
-        weight vector for the categorical features
-    feature_weight_num : np.array
-        weight vector for the numerical features
-    feature_weight_sum : float
-        The sum of the wieghts
-    ranges_of_numeric : np.array
-        range of the scaled numerical features (between 0 and 1)
-
-    Returns
-    -------
-    np.array : array
-        a row vector of the Gower distance
-    """
-    # categorical columns
-    sij_cat = np.where(xi_cat == xj_cat, np.zeros_like(xi_cat), np.ones_like(xi_cat))
-    sum_cat = np.multiply(feature_weight_cat, sij_cat).sum(axis=1)
-
-    # numerical columns
-    abs_delta = np.absolute(xi_num - xj_num)
-    sij_num = np.divide(
-        abs_delta,
-        ranges_of_numeric,
-        out=np.zeros_like(abs_delta),
-        where=ranges_of_numeric != 0,
-    )
-
-    sum_num = np.multiply(feature_weight_num, sij_num).sum(axis=1)
-    sums = np.add(sum_cat, sum_num)
-    sum_sij = np.divide(sums, feature_weight_sum)
-
-    return sum_sij
-
-
-def smallest_indices(ary, n):
-    """Returns the n largest indices from a numpy array.
-
-    Parameters
-    ----------
-    ary : np.array
-        the array for which to return largest indices
-    n : int
-        the number of indices to return
-
-    Returns
-    -------
-    dict
-        the dictionary of indices and values of the largest elements
-    """
-    # n += 1
-    flat = np.nan_to_num(ary.flatten(), nan=999)
-    indices = np.argpartition(-flat, -n)[-n:]
-    indices = indices[np.argsort(flat[indices])]
-    # indices = np.delete(indices,0,0)
-    values = flat[indices]
-    return {"index": indices, "values": values}
-
-
-def gower_topn(
-    data_x,
-    data_y=None,
-    weight=None,
-    cat_features="auto",
-    n=5,
-    key=None,
-):
-    """Get the n most similar elements
-
-    Parameters
-    ----------
-    data_x : np.array or pd.DataFrame
-        The data for the look up
-    data_y : np.array or pd.DataFrame or pd.Series, optional
-        elements for which to return the most similar elements, should be a single row
-    weight : np.array or pd.Series, optional
-        sample weight, by default None
-    cat_features : list of str or bool or int, optional
-        auto detection of cat features or a list of strings, booleans or integers, by default 'auto'
-    n : int, optional
-        the number of neighbors/similar rows to find, by default 5
-    key : str, optional
-        identifier key. If several rows refer to the same id, this column
-        will be used for finding the nearest neighbors with a
-        different id, by default None
-
-    Returns
-    -------
-    dict
-        the dictionary of indices and values of the closest elements
-
-    Raises
-    ------
-    TypeError
-        if the reference element is not a single row
-    """
-
-    if data_y.shape[0] >= 2:
-        raise TypeError("Only support `data_y` of 1 row. ")
-    if key is None:
-        dm = gower_matrix(data_y, data_x, weight, cat_features)
-    else:
-        X = data_x.drop(key, axis=1)
-        Y = data_x.drop(key, axis=1)
-        dm = gower_matrix(Y, X, weight, cat_features)
-
-    if key is not None:
-        idx = smallest_indices(np.nan_to_num(dm[0], nan=1), n)["index"]
-        val = smallest_indices(np.nan_to_num(dm[0], nan=1), n)["values"]
-        unique_id = data_x.iloc[idx, :]
-        unique_id = unique_id[key]
-        nunique_id = unique_id.nunique()
-        mul = 1
-        # continue looking for the closest n unique records with a different id
-        while nunique_id < n:
-            idx = smallest_indices(np.nan_to_num(dm[0], nan=1), mul * n)["index"]
-            val = smallest_indices(np.nan_to_num(dm[0], nan=1), mul * n)["values"]
-            unique_id = data_x.iloc[idx, :].reset_index()
-            unique_id = unique_id[key]
-            nunique_id = unique_id.nunique()
-            mul += 1
-
-        # find the indices of the unique id
-        _, idx_n = np.unique(unique_id, return_index=True)
-        # select only the rows corresponding to unique id
-        val = val[idx_n]
-        idx = idx[idx_n]
-        # sort them from the closest to the farthest, according to the Gower metrics
-        idx_n = np.argsort(val)
-        # return the n closest records, with a different id
-        return {"index": idx[idx_n[:n]], "values": val[idx_n[:n]]}
-    else:
-        return smallest_indices(np.nan_to_num(dm[0], nan=1), n)
-
-
-def get_5_percent_splits(length):
-    """splits dataframe into 5% intervals
-
-    Parameters
-    ----------
-    length : int
-        array length
-
-    Returns
-    -------
-    array
-        vector of sizes
-    """
-
-    five_percent = round(5 / 100 * length)
-    return np.arange(five_percent, length, five_percent)
-
-
-def isolation_forest(X, sample_weight=None):
-    """fits isloation forest to the dataset and gives an anomally score to every sample
-
-    Parameters
-    ----------
-    X : pd.DataFrame or np.array
-        the predictors matrix
-    sample_weight : pd.Series or np.array, optional
-        the sample weights, if any, by default None
-    """
-    clf = IsolationForest().fit(X, sample_weight=sample_weight)
-    return clf.score_samples(X)
-
-
-def isof_find_sample(X, sample_weight=None):
-    """Finds a sample by comparing the distributions of the anomally scores between the sample and the original
-    distribution using the KS-test. Starts of a 5% howver will increase to 10% and then 15% etc. if a significant sample can not be found
-
-    References
-    ----------
-    Sampling method taken from boruta_shap, author: https://github.com/Ekeany
-
-    Parameters
-    ----------
-    X : pd.DataFrame
-        the predictors matrix
-    sample_weight : pd.Series or np.array, optional
-        the sample weights, if any, by default None
-
-    Returns
-    -------
-    array
-        the indices for reducing the shadow predictors matrix
-    """
-    loop = True
-    iteration = 0
-    size = get_5_percent_splits(length=X.shape[0])
-    element = 1
-    preds = isolation_forest(X, sample_weight)
-    while loop:
-        sample_indices = np.random.choice(
-            np.arange(preds.size), size=size[element], replace=False
-        )
-        sample = np.take(preds, sample_indices)
-        if ks_2samp(preds, sample).pvalue > 0.95:
-            break
-        if iteration == 20:
-            element += 1
-            iteration = 0
-    return sample_indices
+"""This module provide methods for sampling large datasets for reducing the running time
+"""
+import numpy as np
+import pandas as pd
+from scipy.sparse import issparse
+from collections import Counter
+from sklearn.cluster import AgglomerativeClustering
+from sklearn.ensemble import IsolationForest
+from scipy.stats import ks_2samp
+from .utils import is_list_of_str, is_list_of_bool, is_list_of_int
+
+
+def sample(df, n=1000, sample_weight=None, method="gower"):
+    """Sampling rows from a dataframe when random sampling is not
+    enough for reducing the number of rows.
+    The strategies are either using hierarchical clustering
+    based on the Gower distance or using isolation forest for identifying
+    the most similar elements.
+    For the clustering algorithm, clusters are determined using the Gower distance
+    (mixed type data) and the dataset is shrunk from n_samples to n_clusters.
+
+    For the isolation forest algorithm, samples are added till a suffisant 2-samples
+    KS statistics is reached or if the number iteration reached the max number (20)
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        the dataframe to sample, with or without the target
+    n : int, optional
+        the number of clusters if method is ``"gower"``, by default 100
+    sample_weight : pd.Series or np.array, optional
+        sample weights, by default None
+    method : str, optional
+        the strategy to use for sampling the rows. Either ``"gower"`` or ``"isoforest"``, by default 'gower'
+
+    Returns
+    -------
+    pd.DataFrame
+        the sampled dataframe
+
+    """
+    assert isinstance(df, pd.DataFrame), "X should be a DataFrame"
+    X = df.copy()
+    num_cols = list(X.select_dtypes(include=[np.number]))
+    non_num_cols = list(set(list(X.columns)) - set(num_cols))
+
+    if method == "gower":
+        # basic imputation
+        if non_num_cols:
+            X[non_num_cols] = X[non_num_cols].fillna(X[non_num_cols].mode().iloc[0])
+        if num_cols:
+            X[num_cols] = X[num_cols].fillna(X[num_cols].mean().iloc[0])
+
+        # no need for scaling, it is built-in the computation of the Gower distance
+        gd = gower_matrix(X, cat_features=non_num_cols, weight=sample_weight)
+
+        labels = AgglomerativeClustering(
+            n_clusters=n, affinity="precomputed", linkage="complete"
+        ).fit_predict(gd)
+        X["label"] = labels
+        X["label"] = "clus_" + X["label"].astype(str)
+        X_num = X.groupby("label")[num_cols].agg("mean")
+        if non_num_cols:
+            X_nonnum = X.groupby("label")[non_num_cols].agg(get_most_common)
+            X_sampled = X_num.join(X_nonnum)
+        else:
+            X_sampled = X_num
+        X_sampled = X_sampled.reindex(X.columns, axis=1)
+        return X_sampled
+    elif method == "isoforest":
+        X[non_num_cols] = X[non_num_cols].astype("str").astype("category")
+        for col in non_num_cols:
+            X[col] = X[col].astype("category").cat.codes
+        idx = isof_find_sample(X, sample_weight=None)
+        return X.iloc[idx, :]
+    else:
+        NotImplementedError(f"{method} not implemented")
+
+
+def get_most_common(srs):
+    x = list(srs)
+    my_counter = Counter(x)
+    return my_counter.most_common(1)[0][0]
+
+
+def gower_matrix(
+    data_x,
+    data_y=None,
+    weight=None,
+    cat_features="auto",
+):
+    """Computes the gower distances between X and Y
+
+    Gower is a similarity measure for categorical, boolean and numerical mixed
+    data.
+
+    Parameters
+    ----------
+    data_x : np.array or pd.DataFrame
+        The data for computing the Gower distance
+    data_y : np.array or pd.DataFrame or pd.Series, optional
+        The reference matrix or vector to compare with, optional
+    weight : np.array or pd.Series, optional
+        sample weight, optional
+    cat_features : list of str or bool or int, optional
+        auto-detect cat features or a list of cat features, by default 'auto'
+
+    Returns
+    -------
+    np.array
+        The Gower distance matrix, shape (n_samples, n_samples)
+
+    Notes
+    -----
+    The non-numeric features, and numeric feature ranges are determined from X and not Y.
+
+    Raises
+    ------
+    TypeError
+        If two dataframes are passed but have different number of columns
+    TypeError
+        If two arrays are passed but have different number of columns
+    TypeError
+        Sparse matrices are not supported
+    TypeError
+        if a list of categorical columns is passed, it should be a list of strings or integers or boolean values
+    """
+    # function checks
+    X = data_x
+    if data_y is None:
+        Y = data_x
+    else:
+        Y = data_y
+    if not isinstance(X, np.ndarray):
+        y_col = Y.columns if isinstance(Y, pd.DataFrame) else Y.index
+        if not np.array_equal(X.columns, y_col):
+            raise TypeError("X and Y must have same columns!")
+    else:
+        if not X.shape[1] == Y.shape[1]:
+            raise TypeError("X and Y must have same y-dim!")
+    if issparse(X) or issparse(Y):
+        raise TypeError("Sparse matrices are not supported!")
+
+    x_n_rows, x_n_cols = X.shape
+    y_n_rows, y_n_cols = Y.shape
+
+    if cat_features == "auto":
+        if not isinstance(X, np.ndarray):
+            is_number = np.vectorize(lambda x: not np.issubdtype(x, np.number))
+            cat_features = is_number(X.dtypes)
+        else:
+            cat_features = np.zeros(x_n_cols, dtype=bool)
+            for col in range(x_n_cols):
+                if not np.issubdtype(type(X[0, col]), np.number):
+                    cat_features[col] = True
+    else:
+        # force categorical columns (if integer encoded for instance)
+        if is_list_of_str(cat_features):
+            cat_feat = [True if c in cat_features else False for c in X.columns]
+            cat_features = np.array(cat_feat)
+        elif is_list_of_bool(cat_features):
+            cat_features = np.array(cat_features)
+        elif is_list_of_int(cat_features):
+            cat_feat = [
+                True if c in cat_features else False for c in range(len(X.columns))
+            ]
+            cat_features = np.array(cat_feat)
+        else:
+            raise TypeError(
+                "If not 'auto' cat_features should be a list of strings, integers or Booleans"
+            )
+
+    # print(cat_features)
+
+    if not isinstance(X, np.ndarray):
+        X = np.asarray(X)
+    if not isinstance(Y, np.ndarray):
+        Y = np.asarray(Y)
+
+    Z = np.concatenate((X, Y))
+
+    x_index = range(0, x_n_rows)
+    y_index = range(x_n_rows, x_n_rows + y_n_rows)
+
+    Z_num = Z[:, np.logical_not(cat_features)]
+
+    num_cols = Z_num.shape[1]
+    num_ranges = np.zeros(num_cols)
+    num_max = np.zeros(num_cols)
+
+    for col in range(num_cols):
+        col_array = Z_num[:, col].astype(np.float32)
+        max_ = np.nanmax(col_array)
+        min_ = np.nanmin(col_array)
+
+        if np.isnan(max_):
+            max_ = 0.0
+        if np.isnan(min_):
+            min_ = 0.0
+        num_max[col] = max_
+        num_ranges[col] = (1 - min_ / max_) if (max_ != 0) else 0.0
+
+    # This is to normalize the numeric values between 0 and 1.
+    Z_num = np.divide(
+        Z_num.astype(float),
+        num_max.astype(float),
+        out=np.zeros_like(Z_num).astype(float),
+        where=num_max != 0,
+    )
+    Z_cat = Z[:, cat_features]
+
+    if weight is None:
+        weight = np.ones(Z.shape[1])
+
+    # print(weight)
+
+    weight_cat = weight[cat_features]
+    weight_num = weight[np.logical_not(cat_features)]
+
+    out = np.zeros((x_n_rows, y_n_rows), dtype=np.float32)
+
+    weight_sum = weight.sum()
+
+    X_cat = Z_cat[x_index,]
+    X_num = Z_num[x_index,]
+    Y_cat = Z_cat[y_index,]
+    Y_num = Z_num[y_index,]
+
+    # print(X_cat,X_num,Y_cat,Y_num)
+
+    for i in range(x_n_rows):
+        j_start = i
+        if x_n_rows != y_n_rows:
+            j_start = 0
+        # call the main function
+        res = _gower_distance_row(
+            X_cat[i, :],
+            X_num[i, :],
+            Y_cat[j_start:y_n_rows, :],
+            Y_num[j_start:y_n_rows, :],
+            weight_cat,
+            weight_num,
+            weight_sum,
+            num_ranges,
+        )
+        # print(res)
+        out[i, j_start:] = res
+        if x_n_rows == y_n_rows:
+            out[i:, j_start] = res
+
+    return out
+
+
+def _gower_distance_row(
+    xi_cat,
+    xi_num,
+    xj_cat,
+    xj_num,
+    feature_weight_cat,
+    feature_weight_num,
+    feature_weight_sum,
+    ranges_of_numeric,
+):
+    """Compute a row of the Gower matrix
+
+    Parameters
+    ----------
+    xi_cat : np.array
+        categorical row of the X matrix
+    xi_num : np.array
+        numerical row of the X matrix
+    xj_cat : np.array
+        categorical row of the X matrix
+    xj_num : np.array
+        numerical row of the X matrix
+    feature_weight_cat : np.array
+        weight vector for the categorical features
+    feature_weight_num : np.array
+        weight vector for the numerical features
+    feature_weight_sum : float
+        The sum of the wieghts
+    ranges_of_numeric : np.array
+        range of the scaled numerical features (between 0 and 1)
+
+    Returns
+    -------
+    np.array : array
+        a row vector of the Gower distance
+    """
+    # categorical columns
+    sij_cat = np.where(xi_cat == xj_cat, np.zeros_like(xi_cat), np.ones_like(xi_cat))
+    sum_cat = np.multiply(feature_weight_cat, sij_cat).sum(axis=1)
+
+    # numerical columns
+    abs_delta = np.absolute(xi_num - xj_num)
+    sij_num = np.divide(
+        abs_delta,
+        ranges_of_numeric,
+        out=np.zeros_like(abs_delta),
+        where=ranges_of_numeric != 0,
+    )
+
+    sum_num = np.multiply(feature_weight_num, sij_num).sum(axis=1)
+    sums = np.add(sum_cat, sum_num)
+    sum_sij = np.divide(sums, feature_weight_sum)
+
+    return sum_sij
+
+
+def smallest_indices(ary, n):
+    """Returns the n largest indices from a numpy array.
+
+    Parameters
+    ----------
+    ary : np.array
+        the array for which to return largest indices
+    n : int
+        the number of indices to return
+
+    Returns
+    -------
+    dict
+        the dictionary of indices and values of the largest elements
+    """
+    # n += 1
+    flat = np.nan_to_num(ary.flatten(), nan=999)
+    indices = np.argpartition(-flat, -n)[-n:]
+    indices = indices[np.argsort(flat[indices])]
+    # indices = np.delete(indices,0,0)
+    values = flat[indices]
+    return {"index": indices, "values": values}
+
+
+def gower_topn(
+    data_x,
+    data_y=None,
+    weight=None,
+    cat_features="auto",
+    n=5,
+    key=None,
+):
+    """Get the n most similar elements
+
+    Parameters
+    ----------
+    data_x : np.array or pd.DataFrame
+        The data for the look up
+    data_y : np.array or pd.DataFrame or pd.Series, optional
+        elements for which to return the most similar elements, should be a single row
+    weight : np.array or pd.Series, optional
+        sample weight, by default None
+    cat_features : list of str or bool or int, optional
+        auto detection of cat features or a list of strings, booleans or integers, by default 'auto'
+    n : int, optional
+        the number of neighbors/similar rows to find, by default 5
+    key : str, optional
+        identifier key. If several rows refer to the same id, this column
+        will be used for finding the nearest neighbors with a
+        different id, by default None
+
+    Returns
+    -------
+    dict
+        the dictionary of indices and values of the closest elements
+
+    Raises
+    ------
+    TypeError
+        if the reference element is not a single row
+    """
+
+    if data_y.shape[0] >= 2:
+        raise TypeError("Only support `data_y` of 1 row. ")
+    if key is None:
+        dm = gower_matrix(data_y, data_x, weight, cat_features)
+    else:
+        X = data_x.drop(key, axis=1)
+        Y = data_x.drop(key, axis=1)
+        dm = gower_matrix(Y, X, weight, cat_features)
+
+    if key is not None:
+        idx = smallest_indices(np.nan_to_num(dm[0], nan=1), n)["index"]
+        val = smallest_indices(np.nan_to_num(dm[0], nan=1), n)["values"]
+        unique_id = data_x.iloc[idx, :]
+        unique_id = unique_id[key]
+        nunique_id = unique_id.nunique()
+        mul = 1
+        # continue looking for the closest n unique records with a different id
+        while nunique_id < n:
+            idx = smallest_indices(np.nan_to_num(dm[0], nan=1), mul * n)["index"]
+            val = smallest_indices(np.nan_to_num(dm[0], nan=1), mul * n)["values"]
+            unique_id = data_x.iloc[idx, :].reset_index()
+            unique_id = unique_id[key]
+            nunique_id = unique_id.nunique()
+            mul += 1
+
+        # find the indices of the unique id
+        _, idx_n = np.unique(unique_id, return_index=True)
+        # select only the rows corresponding to unique id
+        val = val[idx_n]
+        idx = idx[idx_n]
+        # sort them from the closest to the farthest, according to the Gower metrics
+        idx_n = np.argsort(val)
+        # return the n closest records, with a different id
+        return {"index": idx[idx_n[:n]], "values": val[idx_n[:n]]}
+    else:
+        return smallest_indices(np.nan_to_num(dm[0], nan=1), n)
+
+
+def get_5_percent_splits(length):
+    """splits dataframe into 5% intervals
+
+    Parameters
+    ----------
+    length : int
+        array length
+
+    Returns
+    -------
+    array
+        vector of sizes
+    """
+
+    five_percent = round(5 / 100 * length)
+    return np.arange(five_percent, length, five_percent)
+
+
+def isolation_forest(X, sample_weight=None):
+    """fits isloation forest to the dataset and gives an anomally score to every sample
+
+    Parameters
+    ----------
+    X : pd.DataFrame or np.array
+        the predictors matrix
+    sample_weight : pd.Series or np.array, optional
+        the sample weights, if any, by default None
+    """
+    clf = IsolationForest().fit(X, sample_weight=sample_weight)
+    return clf.score_samples(X)
+
+
+def isof_find_sample(X, sample_weight=None):
+    """Finds a sample by comparing the distributions of the anomally scores between the sample and the original
+    distribution using the KS-test. Starts of a 5% howver will increase to 10% and then 15% etc. if a significant sample can not be found
+
+    References
+    ----------
+    Sampling method taken from boruta_shap, author: https://github.com/Ekeany
+
+    Parameters
+    ----------
+    X : pd.DataFrame
+        the predictors matrix
+    sample_weight : pd.Series or np.array, optional
+        the sample weights, if any, by default None
+
+    Returns
+    -------
+    array
+        the indices for reducing the shadow predictors matrix
+    """
+    loop = True
+    iteration = 0
+    size = get_5_percent_splits(length=X.shape[0])
+    element = 1
+    preds = isolation_forest(X, sample_weight)
+    while loop:
+        sample_indices = np.random.choice(
+            np.arange(preds.size), size=size[element], replace=False
+        )
+        sample = np.take(preds, sample_indices)
+        if ks_2samp(preds, sample).pvalue > 0.95:
+            break
+        if iteration == 20:
+            element += 1
+            iteration = 0
+    return sample_indices
```

### Comparing `arfs-2.0.4/src/arfs/utils.py` & `arfs-2.0.5/src/arfs/utils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,872 +1,872 @@
-"""Utility and validation functions
-"""
-
-from __future__ import print_function, division
-
-import lightgbm as lgb
-import matplotlib as mpl
-import numpy as np
-import pandas as pd
-
-from pkg_resources import resource_filename
-from matplotlib import pyplot as plt
-from sklearn.impute import SimpleImputer
-from sklearn.compose import make_column_transformer
-from sklearn.pipeline import make_pipeline
-from sklearn.datasets import fetch_openml
-from sklearn.datasets import load_breast_cancer
-from sklearn.utils import Bunch
-import joblib
-
-qualitative_colors = [
-    "#7F3C8D",
-    "#11A579",
-    "#3969AC",
-    "#F2B701",
-    "#E73F74",
-    "#80BA5A",
-    "#E68310",
-    "#008695",
-    "#CF1C90",
-    "#F97B72",
-]
-
-#####################
-#                   #
-#     Utilities     #
-#                   #
-#####################
-
-
-def reset_plot():
-    """Reset plot style"""
-    # plt.rcParams = plt.rcParamsDefault
-    mpl.rcParams.update(plt.rcParamsDefault)
-
-
-def set_my_plt_style(height=3, width=5, linewidth=2):
-    """This set the style of matplotlib to fivethirtyeight with some modifications (colours, axes)
-
-    Parameters
-    ----------
-    linewidth: int, default=2
-        line width
-    height: int, default=3
-        fig height in inches (yeah they're still struggling with the metric system)
-    width: int, default=5
-        fig width in inches (yeah they're still struggling with the metric system)
-
-    """
-    plt.style.use("fivethirtyeight")
-    my_colors_list = qualitative_colors
-    myorder = [2, 3, 4, 1, 0, 6, 5, 8, 9, 7]
-    my_colors_list = [my_colors_list[i] for i in myorder]
-    bckgnd_color = "#f5f5f5"
-    params = {
-        "figure.figsize": (width, height),
-        "axes.prop_cycle": plt.cycler(color=my_colors_list),
-        "axes.facecolor": bckgnd_color,
-        "patch.edgecolor": bckgnd_color,
-        "figure.facecolor": bckgnd_color,
-        "axes.edgecolor": bckgnd_color,
-        "savefig.edgecolor": bckgnd_color,
-        "savefig.facecolor": bckgnd_color,
-        "grid.color": "#9e9e9e",
-        "lines.linewidth": linewidth,
-    }  # plt.cycler(color=my_colors_list)
-    mpl.rcParams.update(params)
-
-
-def create_dtype_dict(df: pd.DataFrame, dic_keys: str = "col_names") -> dict:
-    """Create a custom dictionary of data type for adding suffixes
-    to column names in the plotting utility for association matrix.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        The dataframe used for computing the association matrix.
-    dic_keys : str
-        Either "col_names" or "dtypes" for returning either a dictionary
-        with column names or dtypes as keys.
-
-    Returns
-    -------
-    dict
-        A dictionary with either column names or dtypes as keys.
-
-    Raises
-    ------
-    ValueError
-        If `dic_keys` is not either "col_names" or "dtypes".
-    """
-    if not isinstance(df, pd.DataFrame):
-        raise TypeError("df should be a pandas DataFrame")
-
-    categorical_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
-    time_cols = df.select_dtypes(
-        include=["datetime", "timedelta", "datetimetz"]
-    ).columns
-    numerical_interval_cols = df.select_dtypes(
-        ["Interval[float]", "Interval[int]"]
-    ).columns
-    numerical_cols = df.select_dtypes(include=np.number).columns
-    remaining_cols = (
-        df.columns.difference(categorical_cols)
-        .difference(numerical_cols)
-        .difference(time_cols)
-        .difference(numerical_interval_cols)
-    )
-
-    if dic_keys == "col_names":
-        cat_dict = dict.fromkeys(categorical_cols, "cat")
-        num_dict = dict.fromkeys(numerical_cols, "num")
-        num_interval_dict = dict.fromkeys(numerical_interval_cols, "num_interval")
-        time_dict = dict.fromkeys(time_cols, "time")
-        remaining_dict = dict.fromkeys(remaining_cols, "unk")
-        return {
-            **cat_dict,
-            **num_dict,
-            **num_interval_dict,
-            **time_dict,
-            **remaining_dict,
-        }
-
-    if dic_keys == "dtypes":
-        return {
-            "cat": categorical_cols.tolist(),
-            "num": numerical_cols.tolist(),
-            "num_interval": numerical_interval_cols.tolist(),
-            "time": time_cols.tolist(),
-            "unk": remaining_cols.tolist(),
-        }
-
-    raise ValueError("dic_keys should be either 'col_names' or 'dtypes'")
-
-
-def get_pandas_cat_codes(X):
-    """
-    Converts categorical and time features in a pandas DataFrame into numerical codes.
-
-    Parameters
-    ----------
-    X : pandas DataFrame
-        The input DataFrame containing categorical and/or time features.
-
-    Returns
-    -------
-    X : pandas DataFrame
-        The modified input DataFrame with categorical and time features replaced by numerical codes.
-    obj_feat : list or None
-        List of column names that were converted to numerical codes. Returns None if no categorical or time features found.
-    cat_idx : list or None
-        List of column indices for the columns in obj_feat. Returns None if no categorical or time features found.
-    """
-    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
-    obj_feat = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
-
-    if obj_feat:
-        for obj_column in obj_feat:
-            column = X[obj_column].astype("str").astype("category")
-            # performs label encoding
-            _, inverse = np.unique(column, return_inverse=True)
-            X[obj_column] = inverse
-        cat_idx = [X.columns.get_loc(col) for col in obj_feat]
-    else:
-        obj_feat = None
-        cat_idx = None
-
-    return X, obj_feat, cat_idx
-
-
-def validate_sample_weight(sample_weight):
-    """Ensures sample_weight parameter is a numpy array."""
-    if isinstance(sample_weight, pd.Series):
-        return sample_weight.values
-    elif isinstance(sample_weight, np.ndarray):
-        return sample_weight
-    elif sample_weight is None:
-        return None
-    else:
-        raise ValueError("sample_weight must be an array-like object or None.")
-
-
-def validate_sample_weight(sample_weight):
-    """
-    Validate the sample_weight parameter.
-
-    Parameters
-    ----------
-    sample_weight : array-like or None
-        Input sample weights.
-
-    Returns
-    -------
-    np.ndarray or None
-        If sample_weight is a Pandas Series, its values are returned as a
-        numpy array. If sample_weight is already a numpy array, it is
-        returned unmodified. If sample_weight is None, None is returned.
-
-    Raises
-    ------
-    ValueError
-        If sample_weight is not an array-like object or None.
-    """
-    if isinstance(sample_weight, pd.Series):
-        return sample_weight.values
-    elif isinstance(sample_weight, np.ndarray):
-        return sample_weight
-    elif sample_weight is None:
-        return None
-    else:
-        raise ValueError("sample_weight must be an array-like object or None.")
-
-
-def validate_pandas_input(arg):
-    """Validate if pandas or numpy arrays are provided
-    Parameters
-    ----------
-    arg : pd.DataFrame or np.array
-        the object to validate
-    Raises
-    ------
-    TypeError
-        error if pandas or numpy arrays are not provided
-    """
-    try:
-        return arg.values
-    except AttributeError:
-        raise TypeError("input needs to be a numpy array or pandas data frame.")
-
-
-def check_if_tree_based(model):
-    """check if estimator is tree based
-
-    Parameters
-    ----------
-    model : object
-        the estimator to check
-
-    Returns
-    -------
-    condition : boolean
-        if tree based or not
-    """
-    tree_based_models = [
-        "lightgbm",
-        "lgbm",
-        "xgboost",
-        "xgb",
-        "catboost",
-        "forest",
-        "boosting",
-        "tree",
-    ]
-    return any(m in model.__class__.__name__.lower() for m in tree_based_models)
-
-
-def is_lightgbm(estimator):
-    """check if estimator is lightgbm
-
-    Parameters
-    ----------
-    model : object
-        the estimator to check
-
-    Returns
-    -------
-    condition : boolean
-        if lgbm based or not
-    """
-    is_lgb = "lgbm" in estimator.__class__.__name__.lower()
-    return is_lgb
-
-
-def is_catboost(estimator):
-    """check if estimator is catboost
-
-    Parameters
-    ----------
-    model : object
-        the estimator to check
-
-    Returns
-    -------
-    condition : boolean
-        if catboost based or not
-    """
-    is_cat = "catboost" in estimator.__class__.__name__.lower()
-    return is_cat
-
-
-def is_xgboost(estimator):
-    """check if estimator is xgboost
-
-    Parameters
-    ----------
-    model : object
-        the estimator to check
-
-    Returns
-    -------
-    condition : boolean
-        if xgboost based or not
-    """
-    is_xgb = "xgb" in estimator.__class__.__name__.lower()
-    return is_xgb
-
-
-def LightForestRegressor(n_feat, n_estimators=10):
-    """lightGBM implementation of the Random Forest regressor with the
-    ideal number of features, according to Elements of statistical learning
-
-    Parameters
-    ----------
-    n_feat: int
-        the number of predictors (nbr of columns of the X matrix)
-    n_estimators : int, optional
-        the number of trees/estimators, by default 10
-
-    Returns
-    -------
-    lightgbm regressor
-        sklearn random forest estimator based on lightgbm
-    """
-
-    feat_frac = n_feat / (3 * n_feat)
-    return lgb.LGBMRegressor(
-        verbose=-1,
-        force_col_wise=True,
-        n_estimators=n_estimators,
-        subsample=0.632,
-        colsample_bytree=feat_frac,
-        boosting_type="rf",
-        subsample_freq=1,
-    )
-
-
-def LightForestClassifier(n_feat, n_estimators=10):
-    """lightGBM implementation of the Random Forest classifier with the
-    ideal number of features, according to Elements of statistical learning
-
-    Parameters
-    ----------
-    n_feat: int
-        the number of predictors (nbr of columns of the X matrix)
-    n_estimators : int, optional
-        the number of trees/estimators, by default 10
-
-    Returns
-    -------
-    lightgbm classifier
-        sklearn random forest estimator based on lightgbm
-    """
-    feat_frac = np.sqrt(n_feat) / n_feat
-    return lgb.LGBMClassifier(
-        verbose=-1,
-        force_col_wise=True,
-        n_estimators=n_estimators,
-        subsample=0.632,
-        colsample_bytree=feat_frac,
-        boosting_type="rf",
-        subsample_freq=1,
-    )
-
-
-def is_list_of_str(str_list):
-    """Check if ``str_list`` is a list of strings.
-
-    Parameters
-    ----------
-    str_list : list or None
-        The list to check.
-
-    Returns
-    -------
-    bool
-        True if the list is a list of strings, False otherwise.
-    """
-    if (
-        str_list is not None
-        and isinstance(str_list, list)
-        and all(isinstance(s, str) for s in str_list)
-    ):
-        return True
-    else:
-        return False
-
-
-def is_list_of_bool(bool_list):
-    """Check if ``bool_list`` is not a list of Booleans
-
-    Parameters
-    ----------
-    bool_list : list of bool
-        the list we want to check for
-
-    Returns
-    -------
-    bool
-        True if list of Booleans, else False
-    """
-    if (
-        bool_list is not None
-        and isinstance(bool_list, list)
-        and all(isinstance(s, bool) for s in bool_list)
-    ):
-        return True
-    else:
-        return False
-
-
-def is_list_of_int(int_list):
-    """Check if ``int_list`` is not a list of integers
-
-    Parameters
-    ----------
-    int_list : list of int
-        the list we want to check for
-
-    Returns
-    -------
-    bool
-        True if list of integers, else False
-    """
-    if (
-        int_list is not None
-        and isinstance(int_list, list)
-        and all(isinstance(s, int) for s in int_list)
-    ):
-        return True
-    else:
-        return False
-
-
-def _get_titanic_data():
-    """Load Titanic data and add dummies (random predictors, numeric and categorical) and
-    a genuine one, for benchmarking purpose. Classification (binary)
-
-    Returns
-    -------
-    object
-        Bunch sklearn, extension of dictionary
-    """
-    # Fetch Titanic data and add random cat and numbers
-    # Example taken from https://scikit-learn.org/stable/auto_examples/inspection/
-    # plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py
-    X, y = fetch_openml("titanic", version=1, as_frame=True, return_X_y=True)
-    rng = np.random.RandomState(seed=42)
-    nice_guys = ["Rick", "Bender", "Cartman", "Morty", "Fry", "Vador", "Thanos"]
-    X["random_cat"] = np.random.choice(nice_guys, X.shape[0])
-    X["random_num"] = rng.randn(X.shape[0])
-    X["family_size"] = X["parch"] + X["sibsp"]
-    X.drop(["parch", "sibsp"], axis=1, inplace=True)
-    X["is_alone"] = np.where(X["family_size"] > 1, 0, 1)
-    X["title"] = (
-        X["name"].str.split(", ", expand=True)[1].str.split(".", expand=True)[0]
-    )
-    X.loc[X["title"] == "Miss", "title"] = "Mrs"
-    title_counts = X["title"].value_counts()
-    rare_titles = title_counts[title_counts < 10].index
-    X.loc[X["title"].isin(rare_titles), "title"] = "rare"
-    categorical_columns = [
-        "pclass",
-        "sex",
-        "embarked",
-        "random_cat",
-        "is_alone",
-        "title",
-    ]
-    numerical_columns = ["age", "family_size", "fare", "random_num"]
-    X = X[categorical_columns + numerical_columns]
-
-    # Preprocessing
-    categorical_pipe = make_pipeline(
-        SimpleImputer(strategy="constant", fill_value="missing")
-    )
-    numerical_pipe = make_pipeline(SimpleImputer(strategy="mean"))
-    preprocessor = make_column_transformer(
-        (categorical_pipe, categorical_columns),
-        (numerical_pipe, numerical_columns),
-    )
-    X = preprocessor.fit_transform(X)
-
-    # Encode categorical variables
-    X = pd.DataFrame(X, columns=categorical_columns + numerical_columns)
-    X[categorical_columns] = X[categorical_columns].astype(str)
-    X[numerical_columns] = X[numerical_columns].astype(float)
-
-    # Create sample weights
-    sample_weight = np.random.uniform(0, 1, len(y))
-
-    return Bunch(
-        data=X,
-        target=y,
-        sample_weight=sample_weight,
-        categorical=categorical_columns,
-    )
-
-
-def _get_cancer_data():
-    """Load breast cancer data and add dummies (random predictors) and a genuine one, for benchmarking purpose
-    Classification (binary)
-
-    Returns
-    -------
-    object
-        Bunch sklearn, extension of dictionary
-    """
-
-    rng = np.random.RandomState(seed=42)
-    data = load_breast_cancer()
-    X, y = data.data, data.target
-    X = pd.DataFrame(X)
-    X.columns = data.feature_names
-    X["random_num1"] = rng.randn(X.shape[0])
-    X["random_num2"] = np.random.poisson(1, X.shape[0])
-    z = y.astype(int)
-    X["genuine_num"] = z * np.abs(
-        np.random.normal(0, 0.1, X.shape[0])
-    ) + np.random.normal(0, 0.1, X.shape[0])
-    y = pd.Series(y)
-    return Bunch(data=X, target=y, sample_weight=None, categorical=None)
-
-
-def _load_boston_data():
-    """Load Boston data and add dummies (random predictors, numeric and categorical) and
-    a genuine one, for benchmarking purpose. Regression (positive domain).
-
-    Returns
-    -------
-    object
-        Bunch sklearn, extension of dictionary
-    """
-
-    data_file_name = resource_filename(__name__, "dataset/data/boston_bunch.joblib")
-    return joblib.load(data_file_name)
-
-
-def _load_housing(as_frame: bool = False):
-    """Load the California housing data. See here
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html
-    for the downloadable version.
-
-    Parameters
-    ----------
-    as_frame :
-        return a pandas dataframe? if not then a "Bunch" (enhanced dictionary) is returned (default ``True``)
-
-    Returns
-    -------
-    pd.DataFrame or Bunch
-        the dataset
-
-    """
-    fdescr_name = resource_filename(__name__, "dataset/descr/housing.rst")
-    with open(fdescr_name) as f:
-        descr_text = f.read()
-
-    data_file_name = resource_filename(__name__, "dataset/data/housing.zip")
-    data = pd.read_csv(data_file_name)
-    feature_names = [
-        "MedInc",
-        "HouseAge",
-        "AveRooms",
-        "AveBedrms",
-        "Population",
-        "AveOccup",
-        "Latitude",
-        "Longitude",
-    ]
-
-    if as_frame:
-        return data
-    else:
-        return Bunch(
-            data=data[feature_names].values,
-            target=data["target"].values,
-            feature_names=feature_names,
-            DESCR=descr_text,
-            filename=data_file_name,
-        )
-
-
-def plot_y_vs_X(X, y, ncols=2, figsize=(10, 10)):
-    """Plot target vs relevant and non-relevant predictors
-
-    Parameters
-    ----------
-    X : pd.DataFrame
-        The DataFrame of the predictors.
-    y : np.array
-        The target.
-    ncols : int, optional
-        The number of columns in the facet plot. Default is 2.
-    figsize : tuple, optional
-        The figure size. Default is (10, 10).
-
-    Returns
-    -------
-    plt.figure
-        The univariate plots y vs pred_i.
-    """
-    n_cols_to_plot = X.shape[1]
-    n_rows = int(np.ceil(n_cols_to_plot / ncols))
-
-    # Create figure and axes
-    f, axs = plt.subplots(nrows=n_rows, ncols=ncols, figsize=figsize)
-
-    for i, col in enumerate(X.columns):
-        row = i // ncols
-        col = i % ncols
-        axs[row, col].scatter(X[col], y, alpha=0.1)
-        axs[row, col].set_title(col)
-
-    # Hide unused subplots
-    for i in range(n_cols_to_plot, n_rows * ncols):
-        row = i // ncols
-        col = i % ncols
-        axs[row, col].set_axis_off()
-
-    # Adjust spacing between subplots
-    plt.tight_layout()
-
-    return f
-
-
-def load_data(name="Titanic"):
-    """Load some toy data set to test the All Relevant Feature Selection methods.
-    Dummies (random) predictors are added and ARFS should be able to filter them out.
-    The Titanic predictors are encoded (needed for scikit estimators).
-
-    Titanic and cancer are for binary classification, they contain synthetic random (dummies) predictors and a
-    noisy but genuine synthetic predictor. Hopefully, a good All Relevant FS should be able to detect all the
-    predictors genuinely related to the target.
-
-    Boston is for regression, this data set contains
-
-    Parameters
-    ----------
-    name : str, optional
-        the name of the data set. Titanic is for classification with sample_weight,
-        Boston for regression and cancer for classification (without sample weight), by default 'Titanic'
-
-    Returns
-    -------
-    Bunch
-        extension of dictionary, accessible by key
-
-    Raises
-    ------
-    ValueError
-        if the dataset name is invalid
-    """
-
-    if name == "Titanic":
-        return _get_titanic_data()
-    elif name == "Boston":
-        return _load_boston_data()
-    elif name == "cancer":
-        return _get_cancer_data()
-    elif name == "housing":
-        return _load_housing(as_frame=False)
-    else:
-        raise ValueError(
-            "`name should be in ['Titanic', 'Boston', 'cancer', 'housing']`"
-        )
-
-
-def _make_corr_dataset_regression(size=1000):
-    """Generate an artificial dataset for regression tasks with columns that
-    are correlated, have no variance, large cardinality, numerical and categorical.
-
-    Parameters
-    ----------
-    size : int, optional
-        number of rows to generate, by default 1000
-
-    Returns
-    -------
-    pd.DataFrame, pd.Series, pd.Series
-        the predictors matrix, the target and the weights
-    """
-    # generate weights
-    w = np.random.beta(a=1, b=0.5, size=size)
-
-    # set seed for reproducibility
-    np.random.seed(42)
-
-    # generate target variable
-    sigma = 0.2
-    y = np.random.normal(1, sigma, size)
-
-    # generate correlated features
-    z = y - np.random.normal(1, sigma / 5, size) + np.random.normal(1, sigma / 5, size)
-    X = pd.DataFrame(
-        {
-            "var0": z,
-            "var1": y * np.abs(np.random.normal(0, sigma * 2, size))
-            + np.random.normal(0, sigma / 10, size),
-            "var2": -y + np.random.normal(0, sigma, size),
-            "var3": y**2 + np.random.normal(0, sigma, size),
-            "var4": np.sqrt(y) + np.random.gamma(1, 0.2, size),
-            "var5": np.random.normal(0, 1, size),
-            "var6": np.random.poisson(1, size),
-            "var7": np.random.binomial(1, 0.3, size),
-            "var8": np.random.normal(0, 1, size),
-            "var9": np.random.poisson(1, size),
-            "var10": np.ones(size),
-            "var11": np.concatenate(
-                [
-                    np.arange(start=0, stop=int(size / 2), step=1),
-                    np.arange(start=0, stop=int(size / 2), step=1),
-                ]
-            ),
-            "var12": y**3 + np.abs(np.random.normal(0, 1, size)),
-        }
-    )
-
-    # introduce missing values
-    idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
-    X.loc[idx_nan, "var12"] = np.nan
-
-    # set column names and types
-    X.columns = ["var" + str(i) for i in range(13)]
-    X["var11"] = X["var11"].astype("category")
-    X["nice_guys"] = np.random.choice(
-        [
-            "Rick",
-            "Bender",
-            "Cartman",
-            "Morty",
-            "Fry",
-            "Vador",
-            "Thanos",
-            "Bejita",
-            "Cell",
-            "Tinkywinky",
-            "Lecter",
-            "Alien",
-            "Terminator",
-            "Drago",
-            "Dracula",
-            "Krueger",
-            "Geoffrey",
-            "Goldfinder",
-            "Blackbeard",
-            "Excel",
-            "SAS",
-            "Bias",
-            "Variance",
-            "Scrum",
-            "Human",
-            "Garry",
-            "Coldplay",
-            "Imaginedragons",
-            "Platist",
-            "Creationist",
-            "Gruber",
-            "KeyserSoze",
-            "Luthor",
-            "Klaue",
-            "Bane",
-            "MarkZ",
-        ],
-        size,
-    )
-
-    return X, y, w
-
-
-def _make_corr_dataset_classification(size=1000):
-    """
-    Generate an artificial dataset for classification tasks. Some columns are correlated,
-    have no variance, large cardinality, numerical and categorical.
-
-    Parameters:
-        size (int): The number of rows to generate. Default is 1000.
-
-    Returns:
-        tuple: A tuple containing the predictors matrix, the target, and the weights.
-    """
-    # Generate weights
-    w = np.random.beta(a=1, b=0.5, size=size)
-
-    # Fix the seed and generate the target
-    np.random.seed(42)
-    y = np.random.binomial(1, 0.5, size)
-
-    # Generate the predictors matrix
-    X = np.zeros((size, 13))
-
-    z = y - np.random.binomial(1, 0.1, size) + np.random.binomial(1, 0.1, size)
-    z[z == -1] = 0
-    z[z == 2] = 1
-
-    # Generate 5 relevant features, with positive and negative correlation to the target
-    X[:, 0] = z
-    X[:, 1] = y * np.abs(np.random.normal(0, 1, size)) + np.random.normal(0, 0.1, size)
-    X[:, 2] = -y + np.random.normal(0, 1, size)
-    X[:, 3] = y**2 + np.random.normal(0, 1, size)
-    X[:, 4] = np.sqrt(y) + np.random.binomial(2, 0.1, size)
-
-    # Generate 5 irrelevant features
-    X[:, 5:10] = np.random.normal(0, 1, size=(size, 5))
-
-    # Generate a column with zero variance
-    X[:, 10] = np.ones(size)
-
-    # Generate a column with high cardinality
-    X[:, 11] = np.arange(start=0, stop=size, step=1)
-
-    # Generate a column with a lot of missing values
-    idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
-    X[:, 12] = y**3 + np.abs(np.random.normal(0, 1, size))
-    X[idx_nan, 12] = np.nan
-
-    # Make the predictors matrix a pandas DataFrame
-    column_names = ["var" + str(i) for i in range(13)]
-    column_names[11] = "dummy"
-    X = pd.DataFrame(X, columns=column_names)
-    X["dummy"] = X["dummy"].astype("category")
-
-    # Add a column of random values from a list
-    nice_guys = [
-        "Rick",
-        "Bender",
-        "Cartman",
-        "Morty",
-        "Fry",
-        "Vador",
-        "Thanos",
-        "Bejita",
-        "Cell",
-        "Tinkywinky",
-        "Lecter",
-        "Alien",
-        "Terminator",
-        "Drago",
-        "Dracula",
-        "Krueger",
-        "Geoffrey",
-        "Goldfinder",
-        "Blackbeard",
-        "Excel",
-        "SAS",
-        "Bias",
-        "Variance",
-        "Scrum",
-        "Human",
-        "Garry",
-        "Coldplay",
-        "Imaginedragons",
-        "Platist",
-        "Creationist",
-        "Gruber",
-        "KeyserSoze",
-        "Luthor",
-        "Klaue",
-        "Bane",
-        "MarkZ",
-    ]
-
-    return X, y, w
+"""Utility and validation functions
+"""
+
+from __future__ import print_function, division
+
+import lightgbm as lgb
+import matplotlib as mpl
+import numpy as np
+import pandas as pd
+
+from pkg_resources import resource_filename
+from matplotlib import pyplot as plt
+from sklearn.impute import SimpleImputer
+from sklearn.compose import make_column_transformer
+from sklearn.pipeline import make_pipeline
+from sklearn.datasets import fetch_openml
+from sklearn.datasets import load_breast_cancer
+from sklearn.utils import Bunch
+import joblib
+
+qualitative_colors = [
+    "#7F3C8D",
+    "#11A579",
+    "#3969AC",
+    "#F2B701",
+    "#E73F74",
+    "#80BA5A",
+    "#E68310",
+    "#008695",
+    "#CF1C90",
+    "#F97B72",
+]
+
+#####################
+#                   #
+#     Utilities     #
+#                   #
+#####################
+
+
+def reset_plot():
+    """Reset plot style"""
+    # plt.rcParams = plt.rcParamsDefault
+    mpl.rcParams.update(plt.rcParamsDefault)
+
+
+def set_my_plt_style(height=3, width=5, linewidth=2):
+    """This set the style of matplotlib to fivethirtyeight with some modifications (colours, axes)
+
+    Parameters
+    ----------
+    linewidth: int, default=2
+        line width
+    height: int, default=3
+        fig height in inches (yeah they're still struggling with the metric system)
+    width: int, default=5
+        fig width in inches (yeah they're still struggling with the metric system)
+
+    """
+    plt.style.use("fivethirtyeight")
+    my_colors_list = qualitative_colors
+    myorder = [2, 3, 4, 1, 0, 6, 5, 8, 9, 7]
+    my_colors_list = [my_colors_list[i] for i in myorder]
+    bckgnd_color = "#f5f5f5"
+    params = {
+        "figure.figsize": (width, height),
+        "axes.prop_cycle": plt.cycler(color=my_colors_list),
+        "axes.facecolor": bckgnd_color,
+        "patch.edgecolor": bckgnd_color,
+        "figure.facecolor": bckgnd_color,
+        "axes.edgecolor": bckgnd_color,
+        "savefig.edgecolor": bckgnd_color,
+        "savefig.facecolor": bckgnd_color,
+        "grid.color": "#9e9e9e",
+        "lines.linewidth": linewidth,
+    }  # plt.cycler(color=my_colors_list)
+    mpl.rcParams.update(params)
+
+
+def create_dtype_dict(df: pd.DataFrame, dic_keys: str = "col_names") -> dict:
+    """Create a custom dictionary of data type for adding suffixes
+    to column names in the plotting utility for association matrix.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        The dataframe used for computing the association matrix.
+    dic_keys : str
+        Either "col_names" or "dtypes" for returning either a dictionary
+        with column names or dtypes as keys.
+
+    Returns
+    -------
+    dict
+        A dictionary with either column names or dtypes as keys.
+
+    Raises
+    ------
+    ValueError
+        If `dic_keys` is not either "col_names" or "dtypes".
+    """
+    if not isinstance(df, pd.DataFrame):
+        raise TypeError("df should be a pandas DataFrame")
+
+    categorical_cols = df.select_dtypes(include=["object", "category", "bool"]).columns
+    time_cols = df.select_dtypes(
+        include=["datetime", "timedelta", "datetimetz"]
+    ).columns
+    numerical_interval_cols = df.select_dtypes(
+        ["Interval[float]", "Interval[int]"]
+    ).columns
+    numerical_cols = df.select_dtypes(include=np.number).columns
+    remaining_cols = (
+        df.columns.difference(categorical_cols)
+        .difference(numerical_cols)
+        .difference(time_cols)
+        .difference(numerical_interval_cols)
+    )
+
+    if dic_keys == "col_names":
+        cat_dict = dict.fromkeys(categorical_cols, "cat")
+        num_dict = dict.fromkeys(numerical_cols, "num")
+        num_interval_dict = dict.fromkeys(numerical_interval_cols, "num_interval")
+        time_dict = dict.fromkeys(time_cols, "time")
+        remaining_dict = dict.fromkeys(remaining_cols, "unk")
+        return {
+            **cat_dict,
+            **num_dict,
+            **num_interval_dict,
+            **time_dict,
+            **remaining_dict,
+        }
+
+    if dic_keys == "dtypes":
+        return {
+            "cat": categorical_cols.tolist(),
+            "num": numerical_cols.tolist(),
+            "num_interval": numerical_interval_cols.tolist(),
+            "time": time_cols.tolist(),
+            "unk": remaining_cols.tolist(),
+        }
+
+    raise ValueError("dic_keys should be either 'col_names' or 'dtypes'")
+
+
+def get_pandas_cat_codes(X):
+    """
+    Converts categorical and time features in a pandas DataFrame into numerical codes.
+
+    Parameters
+    ----------
+    X : pandas DataFrame
+        The input DataFrame containing categorical and/or time features.
+
+    Returns
+    -------
+    X : pandas DataFrame
+        The modified input DataFrame with categorical and time features replaced by numerical codes.
+    obj_feat : list or None
+        List of column names that were converted to numerical codes. Returns None if no categorical or time features found.
+    cat_idx : list or None
+        List of column indices for the columns in obj_feat. Returns None if no categorical or time features found.
+    """
+    dtypes_dic = create_dtype_dict(X, dic_keys="dtypes")
+    obj_feat = dtypes_dic["cat"] + dtypes_dic["time"] + dtypes_dic["unk"]
+
+    if obj_feat:
+        for obj_column in obj_feat:
+            column = X[obj_column].astype("str").astype("category")
+            # performs label encoding
+            _, inverse = np.unique(column, return_inverse=True)
+            X[obj_column] = inverse
+        cat_idx = [X.columns.get_loc(col) for col in obj_feat]
+    else:
+        obj_feat = None
+        cat_idx = None
+
+    return X, obj_feat, cat_idx
+
+
+def validate_sample_weight(sample_weight):
+    """Ensures sample_weight parameter is a numpy array."""
+    if isinstance(sample_weight, pd.Series):
+        return sample_weight.values
+    elif isinstance(sample_weight, np.ndarray):
+        return sample_weight
+    elif sample_weight is None:
+        return None
+    else:
+        raise ValueError("sample_weight must be an array-like object or None.")
+
+
+def validate_sample_weight(sample_weight):
+    """
+    Validate the sample_weight parameter.
+
+    Parameters
+    ----------
+    sample_weight : array-like or None
+        Input sample weights.
+
+    Returns
+    -------
+    np.ndarray or None
+        If sample_weight is a Pandas Series, its values are returned as a
+        numpy array. If sample_weight is already a numpy array, it is
+        returned unmodified. If sample_weight is None, None is returned.
+
+    Raises
+    ------
+    ValueError
+        If sample_weight is not an array-like object or None.
+    """
+    if isinstance(sample_weight, pd.Series):
+        return sample_weight.values
+    elif isinstance(sample_weight, np.ndarray):
+        return sample_weight
+    elif sample_weight is None:
+        return None
+    else:
+        raise ValueError("sample_weight must be an array-like object or None.")
+
+
+def validate_pandas_input(arg):
+    """Validate if pandas or numpy arrays are provided
+    Parameters
+    ----------
+    arg : pd.DataFrame or np.array
+        the object to validate
+    Raises
+    ------
+    TypeError
+        error if pandas or numpy arrays are not provided
+    """
+    try:
+        return arg.values
+    except AttributeError:
+        raise TypeError("input needs to be a numpy array or pandas data frame.")
+
+
+def check_if_tree_based(model):
+    """check if estimator is tree based
+
+    Parameters
+    ----------
+    model : object
+        the estimator to check
+
+    Returns
+    -------
+    condition : boolean
+        if tree based or not
+    """
+    tree_based_models = [
+        "lightgbm",
+        "lgbm",
+        "xgboost",
+        "xgb",
+        "catboost",
+        "forest",
+        "boosting",
+        "tree",
+    ]
+    return any(m in model.__class__.__name__.lower() for m in tree_based_models)
+
+
+def is_lightgbm(estimator):
+    """check if estimator is lightgbm
+
+    Parameters
+    ----------
+    model : object
+        the estimator to check
+
+    Returns
+    -------
+    condition : boolean
+        if lgbm based or not
+    """
+    is_lgb = "lgbm" in estimator.__class__.__name__.lower()
+    return is_lgb
+
+
+def is_catboost(estimator):
+    """check if estimator is catboost
+
+    Parameters
+    ----------
+    model : object
+        the estimator to check
+
+    Returns
+    -------
+    condition : boolean
+        if catboost based or not
+    """
+    is_cat = "catboost" in estimator.__class__.__name__.lower()
+    return is_cat
+
+
+def is_xgboost(estimator):
+    """check if estimator is xgboost
+
+    Parameters
+    ----------
+    model : object
+        the estimator to check
+
+    Returns
+    -------
+    condition : boolean
+        if xgboost based or not
+    """
+    is_xgb = "xgb" in estimator.__class__.__name__.lower()
+    return is_xgb
+
+
+def LightForestRegressor(n_feat, n_estimators=10):
+    """lightGBM implementation of the Random Forest regressor with the
+    ideal number of features, according to Elements of statistical learning
+
+    Parameters
+    ----------
+    n_feat: int
+        the number of predictors (nbr of columns of the X matrix)
+    n_estimators : int, optional
+        the number of trees/estimators, by default 10
+
+    Returns
+    -------
+    lightgbm regressor
+        sklearn random forest estimator based on lightgbm
+    """
+
+    feat_frac = n_feat / (3 * n_feat)
+    return lgb.LGBMRegressor(
+        verbose=-1,
+        force_col_wise=True,
+        n_estimators=n_estimators,
+        subsample=0.632,
+        colsample_bytree=feat_frac,
+        boosting_type="rf",
+        subsample_freq=1,
+    )
+
+
+def LightForestClassifier(n_feat, n_estimators=10):
+    """lightGBM implementation of the Random Forest classifier with the
+    ideal number of features, according to Elements of statistical learning
+
+    Parameters
+    ----------
+    n_feat: int
+        the number of predictors (nbr of columns of the X matrix)
+    n_estimators : int, optional
+        the number of trees/estimators, by default 10
+
+    Returns
+    -------
+    lightgbm classifier
+        sklearn random forest estimator based on lightgbm
+    """
+    feat_frac = np.sqrt(n_feat) / n_feat
+    return lgb.LGBMClassifier(
+        verbose=-1,
+        force_col_wise=True,
+        n_estimators=n_estimators,
+        subsample=0.632,
+        colsample_bytree=feat_frac,
+        boosting_type="rf",
+        subsample_freq=1,
+    )
+
+
+def is_list_of_str(str_list):
+    """Check if ``str_list`` is a list of strings.
+
+    Parameters
+    ----------
+    str_list : list or None
+        The list to check.
+
+    Returns
+    -------
+    bool
+        True if the list is a list of strings, False otherwise.
+    """
+    if (
+        str_list is not None
+        and isinstance(str_list, list)
+        and all(isinstance(s, str) for s in str_list)
+    ):
+        return True
+    else:
+        return False
+
+
+def is_list_of_bool(bool_list):
+    """Check if ``bool_list`` is not a list of Booleans
+
+    Parameters
+    ----------
+    bool_list : list of bool
+        the list we want to check for
+
+    Returns
+    -------
+    bool
+        True if list of Booleans, else False
+    """
+    if (
+        bool_list is not None
+        and isinstance(bool_list, list)
+        and all(isinstance(s, bool) for s in bool_list)
+    ):
+        return True
+    else:
+        return False
+
+
+def is_list_of_int(int_list):
+    """Check if ``int_list`` is not a list of integers
+
+    Parameters
+    ----------
+    int_list : list of int
+        the list we want to check for
+
+    Returns
+    -------
+    bool
+        True if list of integers, else False
+    """
+    if (
+        int_list is not None
+        and isinstance(int_list, list)
+        and all(isinstance(s, int) for s in int_list)
+    ):
+        return True
+    else:
+        return False
+
+
+def _get_titanic_data():
+    """Load Titanic data and add dummies (random predictors, numeric and categorical) and
+    a genuine one, for benchmarking purpose. Classification (binary)
+
+    Returns
+    -------
+    object
+        Bunch sklearn, extension of dictionary
+    """
+    # Fetch Titanic data and add random cat and numbers
+    # Example taken from https://scikit-learn.org/stable/auto_examples/inspection/
+    # plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py
+    X, y = fetch_openml("titanic", version=1, as_frame=True, return_X_y=True)
+    rng = np.random.RandomState(seed=42)
+    nice_guys = ["Rick", "Bender", "Cartman", "Morty", "Fry", "Vador", "Thanos"]
+    X["random_cat"] = np.random.choice(nice_guys, X.shape[0])
+    X["random_num"] = rng.randn(X.shape[0])
+    X["family_size"] = X["parch"] + X["sibsp"]
+    X.drop(["parch", "sibsp"], axis=1, inplace=True)
+    X["is_alone"] = np.where(X["family_size"] > 1, 0, 1)
+    X["title"] = (
+        X["name"].str.split(", ", expand=True)[1].str.split(".", expand=True)[0]
+    )
+    X.loc[X["title"] == "Miss", "title"] = "Mrs"
+    title_counts = X["title"].value_counts()
+    rare_titles = title_counts[title_counts < 10].index
+    X.loc[X["title"].isin(rare_titles), "title"] = "rare"
+    categorical_columns = [
+        "pclass",
+        "sex",
+        "embarked",
+        "random_cat",
+        "is_alone",
+        "title",
+    ]
+    numerical_columns = ["age", "family_size", "fare", "random_num"]
+    X = X[categorical_columns + numerical_columns]
+
+    # Preprocessing
+    categorical_pipe = make_pipeline(
+        SimpleImputer(strategy="constant", fill_value="missing")
+    )
+    numerical_pipe = make_pipeline(SimpleImputer(strategy="mean"))
+    preprocessor = make_column_transformer(
+        (categorical_pipe, categorical_columns),
+        (numerical_pipe, numerical_columns),
+    )
+    X = preprocessor.fit_transform(X)
+
+    # Encode categorical variables
+    X = pd.DataFrame(X, columns=categorical_columns + numerical_columns)
+    X[categorical_columns] = X[categorical_columns].astype(str)
+    X[numerical_columns] = X[numerical_columns].astype(float)
+
+    # Create sample weights
+    sample_weight = np.random.uniform(0, 1, len(y))
+
+    return Bunch(
+        data=X,
+        target=y,
+        sample_weight=sample_weight,
+        categorical=categorical_columns,
+    )
+
+
+def _get_cancer_data():
+    """Load breast cancer data and add dummies (random predictors) and a genuine one, for benchmarking purpose
+    Classification (binary)
+
+    Returns
+    -------
+    object
+        Bunch sklearn, extension of dictionary
+    """
+
+    rng = np.random.RandomState(seed=42)
+    data = load_breast_cancer()
+    X, y = data.data, data.target
+    X = pd.DataFrame(X)
+    X.columns = data.feature_names
+    X["random_num1"] = rng.randn(X.shape[0])
+    X["random_num2"] = np.random.poisson(1, X.shape[0])
+    z = y.astype(int)
+    X["genuine_num"] = z * np.abs(
+        np.random.normal(0, 0.1, X.shape[0])
+    ) + np.random.normal(0, 0.1, X.shape[0])
+    y = pd.Series(y)
+    return Bunch(data=X, target=y, sample_weight=None, categorical=None)
+
+
+def _load_boston_data():
+    """Load Boston data and add dummies (random predictors, numeric and categorical) and
+    a genuine one, for benchmarking purpose. Regression (positive domain).
+
+    Returns
+    -------
+    object
+        Bunch sklearn, extension of dictionary
+    """
+
+    data_file_name = resource_filename(__name__, "dataset/data/boston_bunch.joblib")
+    return joblib.load(data_file_name)
+
+
+def _load_housing(as_frame: bool = False):
+    """Load the California housing data. See here
+    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html
+    for the downloadable version.
+
+    Parameters
+    ----------
+    as_frame :
+        return a pandas dataframe? if not then a "Bunch" (enhanced dictionary) is returned (default ``True``)
+
+    Returns
+    -------
+    pd.DataFrame or Bunch
+        the dataset
+
+    """
+    fdescr_name = resource_filename(__name__, "dataset/descr/housing.rst")
+    with open(fdescr_name) as f:
+        descr_text = f.read()
+
+    data_file_name = resource_filename(__name__, "dataset/data/housing.zip")
+    data = pd.read_csv(data_file_name)
+    feature_names = [
+        "MedInc",
+        "HouseAge",
+        "AveRooms",
+        "AveBedrms",
+        "Population",
+        "AveOccup",
+        "Latitude",
+        "Longitude",
+    ]
+
+    if as_frame:
+        return data
+    else:
+        return Bunch(
+            data=data[feature_names].values,
+            target=data["target"].values,
+            feature_names=feature_names,
+            DESCR=descr_text,
+            filename=data_file_name,
+        )
+
+
+def plot_y_vs_X(X, y, ncols=2, figsize=(10, 10)):
+    """Plot target vs relevant and non-relevant predictors
+
+    Parameters
+    ----------
+    X : pd.DataFrame
+        The DataFrame of the predictors.
+    y : np.array
+        The target.
+    ncols : int, optional
+        The number of columns in the facet plot. Default is 2.
+    figsize : tuple, optional
+        The figure size. Default is (10, 10).
+
+    Returns
+    -------
+    plt.figure
+        The univariate plots y vs pred_i.
+    """
+    n_cols_to_plot = X.shape[1]
+    n_rows = int(np.ceil(n_cols_to_plot / ncols))
+
+    # Create figure and axes
+    f, axs = plt.subplots(nrows=n_rows, ncols=ncols, figsize=figsize)
+
+    for i, col in enumerate(X.columns):
+        row = i // ncols
+        col = i % ncols
+        axs[row, col].scatter(X[col], y, alpha=0.1)
+        axs[row, col].set_title(col)
+
+    # Hide unused subplots
+    for i in range(n_cols_to_plot, n_rows * ncols):
+        row = i // ncols
+        col = i % ncols
+        axs[row, col].set_axis_off()
+
+    # Adjust spacing between subplots
+    plt.tight_layout()
+
+    return f
+
+
+def load_data(name="Titanic"):
+    """Load some toy data set to test the All Relevant Feature Selection methods.
+    Dummies (random) predictors are added and ARFS should be able to filter them out.
+    The Titanic predictors are encoded (needed for scikit estimators).
+
+    Titanic and cancer are for binary classification, they contain synthetic random (dummies) predictors and a
+    noisy but genuine synthetic predictor. Hopefully, a good All Relevant FS should be able to detect all the
+    predictors genuinely related to the target.
+
+    Boston is for regression, this data set contains
+
+    Parameters
+    ----------
+    name : str, optional
+        the name of the data set. Titanic is for classification with sample_weight,
+        Boston for regression and cancer for classification (without sample weight), by default 'Titanic'
+
+    Returns
+    -------
+    Bunch
+        extension of dictionary, accessible by key
+
+    Raises
+    ------
+    ValueError
+        if the dataset name is invalid
+    """
+
+    if name == "Titanic":
+        return _get_titanic_data()
+    elif name == "Boston":
+        return _load_boston_data()
+    elif name == "cancer":
+        return _get_cancer_data()
+    elif name == "housing":
+        return _load_housing(as_frame=False)
+    else:
+        raise ValueError(
+            "`name should be in ['Titanic', 'Boston', 'cancer', 'housing']`"
+        )
+
+
+def _make_corr_dataset_regression(size=1000):
+    """Generate an artificial dataset for regression tasks with columns that
+    are correlated, have no variance, large cardinality, numerical and categorical.
+
+    Parameters
+    ----------
+    size : int, optional
+        number of rows to generate, by default 1000
+
+    Returns
+    -------
+    pd.DataFrame, pd.Series, pd.Series
+        the predictors matrix, the target and the weights
+    """
+    # generate weights
+    w = np.random.beta(a=1, b=0.5, size=size)
+
+    # set seed for reproducibility
+    np.random.seed(42)
+
+    # generate target variable
+    sigma = 0.2
+    y = np.random.normal(1, sigma, size)
+
+    # generate correlated features
+    z = y - np.random.normal(1, sigma / 5, size) + np.random.normal(1, sigma / 5, size)
+    X = pd.DataFrame(
+        {
+            "var0": z,
+            "var1": y * np.abs(np.random.normal(0, sigma * 2, size))
+            + np.random.normal(0, sigma / 10, size),
+            "var2": -y + np.random.normal(0, sigma, size),
+            "var3": y**2 + np.random.normal(0, sigma, size),
+            "var4": np.sqrt(y) + np.random.gamma(1, 0.2, size),
+            "var5": np.random.normal(0, 1, size),
+            "var6": np.random.poisson(1, size),
+            "var7": np.random.binomial(1, 0.3, size),
+            "var8": np.random.normal(0, 1, size),
+            "var9": np.random.poisson(1, size),
+            "var10": np.ones(size),
+            "var11": np.concatenate(
+                [
+                    np.arange(start=0, stop=int(size / 2), step=1),
+                    np.arange(start=0, stop=int(size / 2), step=1),
+                ]
+            ),
+            "var12": y**3 + np.abs(np.random.normal(0, 1, size)),
+        }
+    )
+
+    # introduce missing values
+    idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
+    X.loc[idx_nan, "var12"] = np.nan
+
+    # set column names and types
+    X.columns = ["var" + str(i) for i in range(13)]
+    X["var11"] = X["var11"].astype("category")
+    X["nice_guys"] = np.random.choice(
+        [
+            "Rick",
+            "Bender",
+            "Cartman",
+            "Morty",
+            "Fry",
+            "Vador",
+            "Thanos",
+            "Bejita",
+            "Cell",
+            "Tinkywinky",
+            "Lecter",
+            "Alien",
+            "Terminator",
+            "Drago",
+            "Dracula",
+            "Krueger",
+            "Geoffrey",
+            "Goldfinder",
+            "Blackbeard",
+            "Excel",
+            "SAS",
+            "Bias",
+            "Variance",
+            "Scrum",
+            "Human",
+            "Garry",
+            "Coldplay",
+            "Imaginedragons",
+            "Platist",
+            "Creationist",
+            "Gruber",
+            "KeyserSoze",
+            "Luthor",
+            "Klaue",
+            "Bane",
+            "MarkZ",
+        ],
+        size,
+    )
+
+    return X, y, w
+
+
+def _make_corr_dataset_classification(size=1000):
+    """
+    Generate an artificial dataset for classification tasks. Some columns are correlated,
+    have no variance, large cardinality, numerical and categorical.
+
+    Parameters:
+        size (int): The number of rows to generate. Default is 1000.
+
+    Returns:
+        tuple: A tuple containing the predictors matrix, the target, and the weights.
+    """
+    # Generate weights
+    w = np.random.beta(a=1, b=0.5, size=size)
+
+    # Fix the seed and generate the target
+    np.random.seed(42)
+    y = np.random.binomial(1, 0.5, size)
+
+    # Generate the predictors matrix
+    X = np.zeros((size, 13))
+
+    z = y - np.random.binomial(1, 0.1, size) + np.random.binomial(1, 0.1, size)
+    z[z == -1] = 0
+    z[z == 2] = 1
+
+    # Generate 5 relevant features, with positive and negative correlation to the target
+    X[:, 0] = z
+    X[:, 1] = y * np.abs(np.random.normal(0, 1, size)) + np.random.normal(0, 0.1, size)
+    X[:, 2] = -y + np.random.normal(0, 1, size)
+    X[:, 3] = y**2 + np.random.normal(0, 1, size)
+    X[:, 4] = np.sqrt(y) + np.random.binomial(2, 0.1, size)
+
+    # Generate 5 irrelevant features
+    X[:, 5:10] = np.random.normal(0, 1, size=(size, 5))
+
+    # Generate a column with zero variance
+    X[:, 10] = np.ones(size)
+
+    # Generate a column with high cardinality
+    X[:, 11] = np.arange(start=0, stop=size, step=1)
+
+    # Generate a column with a lot of missing values
+    idx_nan = np.random.choice(size, int(round(size / 2)), replace=False)
+    X[:, 12] = y**3 + np.abs(np.random.normal(0, 1, size))
+    X[idx_nan, 12] = np.nan
+
+    # Make the predictors matrix a pandas DataFrame
+    column_names = ["var" + str(i) for i in range(13)]
+    column_names[11] = "dummy"
+    X = pd.DataFrame(X, columns=column_names)
+    X["dummy"] = X["dummy"].astype("category")
+
+    # Add a column of random values from a list
+    nice_guys = [
+        "Rick",
+        "Bender",
+        "Cartman",
+        "Morty",
+        "Fry",
+        "Vador",
+        "Thanos",
+        "Bejita",
+        "Cell",
+        "Tinkywinky",
+        "Lecter",
+        "Alien",
+        "Terminator",
+        "Drago",
+        "Dracula",
+        "Krueger",
+        "Geoffrey",
+        "Goldfinder",
+        "Blackbeard",
+        "Excel",
+        "SAS",
+        "Bias",
+        "Variance",
+        "Scrum",
+        "Human",
+        "Garry",
+        "Coldplay",
+        "Imaginedragons",
+        "Platist",
+        "Creationist",
+        "Gruber",
+        "KeyserSoze",
+        "Luthor",
+        "Klaue",
+        "Bane",
+        "MarkZ",
+    ]
+
+    return X, y, w
```

### Comparing `arfs-2.0.4/src/arfs.egg-info/PKG-INFO` & `arfs-2.0.5/src/arfs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-Metadata-Version: 2.1
-Name: arfs
-Version: 2.0.4
-Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
-Author: ThomasBury
-Author-email: bury.thomas@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/ThomasBury/arfs
-Project-URL: Source, https://github.com/ThomasBury/arfs
-Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
-Project-URL: Download, https://pypi.org/project/arfs/
-Keywords: feature-selection,all-relevant,selection,MRmr
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE.md
-
-<img src="logo.png" alt="drawing" width="200"/>
-
-[buy me caffeine](https://ko-fi.com/V7V72SOHX)
-
-[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
-
-
-[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
-
-# All relevant feature selection
-
-All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
-
-This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
-
-Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
-
-Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
-
-## Installation
-
-`$ pip install arfs`
-
-## Example
-
-Working examples for:
-
- - [Preprocessing](./docs/notebooks/preprocessingipynb)
- - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
- - [Regression](./docs/notebooks/arfs_regression.ipynb)
- - [Classification](./docs/notebooks/arfs_classification.ipynb)
- - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
- - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
- - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
- - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
- - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
- - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
- - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
- - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
- - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
- - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
- - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
-
-For imbalanced classification:
- - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
- - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
-
-
-
-## Boruta
-
-The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
-
- * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
- * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
- * Combine the original ones with shuffled copies
- * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
- * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
- * Find the maximum Z score among shadow attributes (MZSA)
- * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
- * Tag the variables as 'important' when they have importance significantly higher than MZSA.
- * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
-
-At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-
-## BoostARoota
-
-BoostARoota follows closely the Boruta method but modifies a few things:
-
- * One-Hot-Encode the feature set
- * Double width of the data set, making a copy of all features in the original dataset
- * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
- * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
- * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
- * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
- * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
- * Go back to (2) until the number of features removed is less than ten per cent of the total.
- * Method returns the features remaining once completed.
-
-In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
-
-## Modifications to Boruta and BoostARoota
-
- I forked both Boruta and BoostARoota and made the following changes (under PR):
-
-**Boruta --> Leshy**:
-
-  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
-  - Using lightGBM as the default speeds up by an order of magnitude the running time
-  - Work with Catboost, sklearn API
-  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
-  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
-
-**BoostARoota --> BoostAGroota**:
-
-  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
-  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
-  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
-  - Work with sample_weight, for Poisson or any application requiring a weighting.
-
-## GrootCV, a new method
-
-**New: GrootCV**:
-
-  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
-  - the feature importance is derived using SHAP importance
-  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
-  - Not based on a given percentage of cols needed to be deleted
-  - Plot method for var. imp
-
-
-## References
-
-**Theory**
-
- - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
- - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
-
-**Applications**
-
- - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
- - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
- - [BoostARoota](https://github.com/chasedehan/BoostARoota)
-
-
-
+Metadata-Version: 2.1
+Name: arfs
+Version: 2.0.5
+Summary: All Relevant Feature Selection and Maximal Relevant minimal redundancy FS
+Author: ThomasBury
+Author-email: bury.thomas@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/ThomasBury/arfs
+Project-URL: Source, https://github.com/ThomasBury/arfs
+Project-URL: Tracker, https://github.com/ThomasBury/arfs/issues
+Project-URL: Download, https://pypi.org/project/arfs/
+Keywords: feature-selection,all-relevant,selection,MRmr
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE.md
+
+<img src="logo.png" alt="drawing" width="200"/>
+
+[buy me caffeine](https://ko-fi.com/V7V72SOHX)
+
+[![PyPI version](https://badge.fury.io/py/arfs.svg)](https://badge.fury.io/py/arfs) [![Downloads](https://static.pepy.tech/personalized-badge/arfs?period=total&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads)](https://pepy.tech/project/arfs) [![Documentation Status](https://readthedocs.org/projects/arfs/badge/?version=latest)](https://arfs.readthedocs.io/en/latest/?badge=latest) [![Code Style](https://img.shields.io/badge/code%20style-black-black)](https://img.shields.io/badge/code%20style-black-black)
+
+
+[ARFS readthedocs](https://arfs.readthedocs.io/en/latest/#)
+
+# All relevant feature selection
+
+All relevant feature selection means trying to find all features carrying information usable for prediction, rather than finding a possibly compact subset of features on which some particular model has a minimal error. This might include redundant predictors. All relevant feature selection is model agnostic in the sense that it doesn't optimize a scoring function for a *specific* model but rather tries to select all the predictors which are related to the response. 
+
+This package implements 3 different methods (Leshy is an evolution of Boruta, BoostAGroota is an evolution of BoostARoota and GrootCV is a new one). They are sklearn compatible. See hereunder for details about those methods. You can use any sklearn compatible estimator with Leshy and BoostAGroota but I recommend lightGBM. It's fast, accurate and has SHAP values builtin. It also provides a module for performing preprocessing and perform basic feature selection (autobinning, remove columns with too many missing values, zero variance, high-cardinality, highly correlated, etc.). Examples and detailled methods hereunder.
+
+Moreover, as an alternative to the all relevant problem, the ARFS package provides a MRmr feature selection which, theoretically, returns a subset of the predictors selected by an arfs method. ARFS also provides a `LASSO` feature selection which works especially well for (G)LMs and GAMs. You can combine Lasso with the `TreeDiscretizer` for introducing non-linearities into linear models and perform feature selection.
+
+Please note that one limitation of the lasso is that it treats the levels of a categorical predictor individually. However, this issue can be addressed by utilizing the `TreeDiscretizer`, which automatically bins numerical variables and groups the levels of categorical variables.
+
+## Installation
+
+`$ pip install arfs`
+
+## Example
+
+Working examples for:
+
+ - [Preprocessing](./docs/notebooks/preprocessingipynb)
+ - [Basic FS (best before ARFS)](./docs/notebooks/basic_feature_selection.ipynb)
+ - [Regression](./docs/notebooks/arfs_regression.ipynb)
+ - [Classification](./docs/notebooks/arfs_classification.ipynb)
+ - [LASSO and (G)LM feature selection](./docs/notebooks/lasso_feature_selection.ipynb)
+ - [Passing custom params](./docs/notebooks/arfs_grootcv_custom_params.ipynb)
+ - [Non-normal loss and sample weights](./docs/notebooks/arfs_non_normal_loss_and_sample_weight.ipynb)
+ - [ARFS on GPU](./docs/notebooks/arfs_on_GPU.ipynb)
+ - [Fast Shap](./docs/notebooks/arfs_shap_vs_fastshap.ipynb)
+ - [Categoricals](./docs/notebooks/issue_categoricals.ipynb)
+ - [Collinearity](./docs/notebooks/issue_collinearity.ipynb)
+ - [Reducing run time for large data](./docs/notebooks/arfs_large_data_sampling.ipynb)
+ - [Comparison to Boruta and BorutaShap](./docs/notebooks/arfs_boruta_borutaShap_comparison.ipynb)
+ - [MRmr alternative](./docs/notebooks/mrmr_feature_selection.ipynb)
+ - [MRmr vs ARFS](./docs/notebooks/mrmr_fs_VS_arfs.ipynb)
+
+For imbalanced classification:
+ - GrootCV will automatically detect imbalanced data and set the lightGBM `'is_unbalance' = True`
+ - For Leshy and BoostAGroota, you can pass the estimator with the relevant parameter (e.g. `class_weight = 'balanced'`)
+
+
+
+## Boruta
+
+The Boruta algorithm tries to capture all the important features you might have in your dataset with respect to an outcome variable. The procedure is the following:
+
+ * Create duplicate copies of all independent variables. When the number of independent variables in the original data is less than 5, create at least 5 copies using existing variables.
+ * Shuffle the values of added duplicate copies to remove their correlations with the target variable. It is called shadow features or permuted copies.
+ * Combine the original ones with shuffled copies
+ * Run a random forest classifier on the combined dataset and performs a variable importance measure (the default is Mean Decrease Accuracy) to evaluate the importance of each variable where higher means more important.
+ * Then Z score is computed. It means mean of accuracy loss divided by the standard deviation of accuracy loss.
+ * Find the maximum Z score among shadow attributes (MZSA)
+ * Tag the variables as 'unimportant' when they have importance significantly lower than MZSA. Then we permanently remove them from the process.
+ * Tag the variables as 'important' when they have importance significantly higher than MZSA.
+ * Repeat the above steps for a predefined number of iterations (random forest runs), or until all attributes are either tagged 'unimportant' or 'important', whichever comes first.
+
+At every iteration, the algorithm compares the Z-scores of the shuffled copies of the features and the original features to see if the latter performed better than the former. If it does, the algorithm will mark the feature as important. In essence, the algorithm is trying to validate the importance of the feature by comparing with randomly shuffled copies, which increases the robustness. This is done by simply comparing the number of times a feature did better with the shadow features using a binomial distribution. Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+
+## BoostARoota
+
+BoostARoota follows closely the Boruta method but modifies a few things:
+
+ * One-Hot-Encode the feature set
+ * Double width of the data set, making a copy of all features in the original dataset
+ * Randomly shuffle the new features created in (2). These duplicated and shuffled features are referred to as "shadow features"
+ * Run XGBoost classifier on the entire data set ten times. Running it ten times allows for random noise to be smoothed, resulting in more robust estimates of importance. The number of repeats is a parameter than can be changed.
+ * Obtain importance values for each feature. This is a simple importance metric that sums up how many times the particular feature was split on in the XGBoost algorithm.
+ * Compute "cutoff": the average feature importance value for all shadow features and divide by four. Shadow importance values are divided by four (parameter can be changed) to make it more difficult for the variables to be removed. With values lower than this, features are removed at too high of a rate.
+ * Remove features with average importance across the ten iterations that is less than the cutoff specified in (6)
+ * Go back to (2) until the number of features removed is less than ten per cent of the total.
+ * Method returns the features remaining once completed.
+
+In the spirit, the same heuristic than Boruta but using Boosting (originally Boruta was supporting only random forest). The validation of the importance is done by comparing to the maximum of the median var. imp of the shadow predictors (in Boruta, a statistical test is performed using the Z-score). Since the whole process is done on the same train-test split, the variance of the variable importance comes only from the different re-fit of the model over the different iterations.
+
+## Modifications to Boruta and BoostARoota
+
+ I forked both Boruta and BoostARoota and made the following changes (under PR):
+
+**Boruta --> Leshy**:
+
+  - The categorical features (they are detected, encoded. The tree-based models are working better with integer encoding rather than with OHE, which leads to deep and unstable trees). If Catboost is used, then the cat.pred (if any) are set up
+  - Using lightGBM as the default speeds up by an order of magnitude the running time
+  - Work with Catboost, sklearn API
+  - Allow using sample_weight, for applications like Poisson regression or any requiring weights
+  - Supports 3 different feature importances: native, SHAP and permutation. Native being the least consistent(because of the imp. biased towards numerical and large cardinality categorical) but the fastest of the 3. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py))
+
+**BoostARoota --> BoostAGroota**:
+
+  - Replace XGBoost with LightGBM, you can still use tree-based scikitlearn models
+  - Replace native var.imp by SHAP var.imp. Indeed, the impurity var.imp. are biased en sensitive to large cardinality (see [scikit demo](https://scikit-learn.org/stable/auto_examples/inspection/plot_permutation_importance.html#sphx-glr-auto-examples-inspection-plot-permutation-importance-py)). Moreover, the native var. imp are computed on the train set, here the data are split (internally) in train and test, var. imp computed on the test set.
+  - Handling categorical predictors. Cat. predictors should NOT be one-hot encoded, it leads to deep unstable trees. Instead, it's better to use the native method of lightGBM or CatBoost. A preprocessing step is needed to encode (ligthGBM and CatBoost use integer encoding and reference to categorical columns. The splitting strategies are different then, see official doc).
+  - Work with sample_weight, for Poisson or any application requiring a weighting.
+
+## GrootCV, a new method
+
+**New: GrootCV**:
+
+  - Cross-validated feature importance to smooth out the noise, based on lightGBM only (which is, most of the time, the fastest and more accurate Boosting).
+  - the feature importance is derived using SHAP importance
+  - Taking the max of the median of the shadow var. imp over folds otherwise not enough conservative and it improves the convergence (needs less evaluation to find a threshold)
+  - Not based on a given percentage of cols needed to be deleted
+  - Plot method for var. imp
+
+
+## References
+
+**Theory**
+
+ - [Consistent feature selection for pattern recognition in polynomial time](https://www.jmlr.org/papers/volume8/nilsson07a/nilsson07a.pdf)
+ - [Maximum Relevance and Minimum Redundancy Feature Selection Methods for a Marketing Machine Learning Platform](https://eng.uber.com/research/maximum-relevance-and-minimum-redundancy-feature-selection-methods-for-a-marketing-machine-learning-platform/)
+
+**Applications**
+
+ - [The Boruta paper](https://www.jstatsoft.org/article/view/v036i11/v36i11.pdf)
+ - [The python implementation](https://github.com/scikit-learn-contrib/boruta_py)
+ - [BoostARoota](https://github.com/chasedehan/BoostARoota)
+
+
+
```

### Comparing `arfs-2.0.4/src/arfs.egg-info/SOURCES.txt` & `arfs-2.0.5/src/arfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arfs-2.0.4/tests/test_allrelevant.py` & `arfs-2.0.5/tests/test_allrelevant.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-import pytest
-import numpy as np
-import lightgbm as lgb
-from arfs.feature_selection.allrelevant import Leshy, BoostAGroota, GrootCV
-from arfs.utils import (
-    _generated_corr_dataset_regr,
-    _generated_corr_dataset_classification,
-)
-from arfs.utils import LightForestClassifier, LightForestRegressor
-
-
-class TestLeshy:
-    """
-    Test suite for all-relevant FS boruta-like method: Leshy
-    """
-
-    def test_borutaPy_vs_leshy_with_rfc_and_native_feature_importance(self):
-        # too slow for circleci to run them in a reasonable time
-        # takes 2 min on laptop, 1h or more on circleci
-        # sklearn random forest implementation
-        # X, y, w = _generated_corr_dataset_classification()
-        # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
-        # bt = BorutaPy(rfc)
-        # bt.fit(X.values, y)
-        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
-
-        # lightGBM random forest implementation
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = _generated_corr_dataset_classification(size=100)
-        n_feat = X.shape[1]
-        rfc = LightForestClassifier(n_feat)
-        # RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100) # --> too slow
-        arfs = Leshy(rfc, verbose=0, max_iter=10, random_state=42, importance="native")
-        arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
-        assert bool(
-            set(baseline_list) & set(leshy_rfc_list)
-        ), "expect non-empty intersection"
-
-    def test_borutaPy_vs_leshy_with_rfr_and_native_feature_importance(self):
-        # too slow for circleci to run them in a reasonable time
-        # takes 2 min on laptop, 1h or more on circleci
-        # # sklearn random forest implementation
-        # X, y, w = _generated_corr_dataset_regr()
-        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
-        # bt = BorutaPy(rfr)
-        # bt.fit(X.values, y)
-        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
-
-        # lightGBM random forest implementation
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = _generated_corr_dataset_regr(size=100)
-        n_feat = X.shape[1]
-        rfr = LightForestRegressor(n_feat)
-        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=10)
-        arfs = Leshy(rfr, verbose=0, max_iter=10, random_state=42, importance="native")
-        arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
-        assert bool(
-            set(baseline_list) & set(leshy_rfc_list)
-        ), "expect non-empty intersection"
-
-    def test_borutaPy_vs_leshy_with_rfc_and_shap_feature_importance(self):
-        # too slow for circleci to run them in a reasonable time
-        # takes 2 min on laptop, 1h or more on circleci
-        # # sklearn random forest implementation
-        # X, y, w = _generated_corr_dataset_classification()
-        # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
-        # bt = BorutaPy(rfc)
-        # bt.fit(X.values, y)
-        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
-
-        # lightGBM random forest implementation
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = _generated_corr_dataset_classification(size=100)
-        n_feat = X.shape[1]
-        model = LightForestClassifier(n_feat)
-        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
-        arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
-        assert bool(
-            set(baseline_list) & set(leshy_rfc_list)
-        ), "expect non-empty intersection"
-
-    def test_borutaPy_vs_leshy_with_rfr_and_shap_feature_importance(self):
-        # too slow for circleci to run them in a reasonable time
-        # takes 2 min on laptop, 1h or more on circleci
-        # # sklearn random forest implementation
-        # X, y, w = _generated_corr_dataset_regr()
-        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
-        # bt = BorutaPy(rfr)
-        # bt.fit(X.values, y)
-        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
-
-        # lightGBM random forest implementation
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-        X, y, w = _generated_corr_dataset_regr(size=500)
-        n_feat = X.shape[1]
-        model = LightForestRegressor(n_feat)
-        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
-        arfs.fit(X, y)
-        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
-        assert bool(
-            set(baseline_list) & set(leshy_rfc_list)
-        ), "expect non-empty intersection"
-
-    def test_leshy_clf_with_lgb_and_shap_feature_importance_and_sample_weight(self):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-
-        X, y, w = _generated_corr_dataset_classification(size=500)
-        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-    def test_leshy_regr_with_lgb_and_shap_feature_importance_and_sample_weight(self):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
-
-        X, y, w = _generated_corr_dataset_classification(size=500)
-        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-
-class TestBoostAGroota:
-    """
-    Test suite for all-relevant FS boruta-like method: Leshy
-    """
-
-    def test_boostagroota_clf_with_lgb_and_shap_feature_importance_and_sample_weight(
-        self,
-    ):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-
-        X, y, w = _generated_corr_dataset_classification(size=500)
-        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = BoostAGroota(
-            est=model,
-            cutoff=1,
-            iters=3,
-            max_rounds=3,
-            delta=0.1,
-            silent=False,
-            importance="shap",
-        )
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-    def test_boostagroota_clf_with_lgb_and_pimp_feature_importance_and_sample_weight(
-        self,
-    ):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-
-        X, y, w = _generated_corr_dataset_classification(size=500)
-        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = BoostAGroota(
-            est=model,
-            cutoff=1,
-            iters=3,
-            max_rounds=3,
-            delta=0.1,
-            silent=False,
-            importance="pimp",
-        )
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-    def test_boostagroota_rgr_with_lgb_and_shap_feature_importance_and_sample_weight(
-        self,
-    ):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
-
-        X, y, w = _generated_corr_dataset_regr(size=500)
-        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = BoostAGroota(
-            est=model,
-            cutoff=1,
-            iters=3,
-            max_rounds=3,
-            delta=0.1,
-            silent=False,
-            importance="shap",
-        )
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-    def test_boostagroota_regr_with_lgb_and_pimp_feature_importance_and_sample_weight(
-        self,
-    ):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
-
-        X, y, w = _generated_corr_dataset_regr(size=500)
-        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
-        arfs = BoostAGroota(
-            est=model,
-            cutoff=1,
-            iters=3,
-            max_rounds=3,
-            delta=0.1,
-            silent=False,
-            importance="pimp",
-        )
-        arfs.fit(X, y, w)
-        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(leshy_list)
-        ), "expect non-empty intersection"
-
-
-class TestGrootCV:
-    """
-    Test suite for all-relevant FS boruta-like method: Leshy
-    """
-
-    def test_grootcv_classification_with_and_sample_weight(self):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
-
-        X, y, w = _generated_corr_dataset_classification(size=100)
-        arfs = GrootCV(objective="binary", cutoff=1, n_folds=3, n_iter=3, silent=False)
-        arfs.fit(X, y, w)
-        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(grootcv_list)
-        ), "expect non-empty intersection"
-
-    def test_grootcv_regression_with_and_sample_weight(self):
-        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
-
-        X, y, w = _generated_corr_dataset_regr(size=100)
-        arfs = GrootCV(objective="l2", cutoff=1, n_folds=3, n_iter=3, silent=False)
-        arfs.fit(X, y, w)
-        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
-
-        assert bool(
-            set(baseline_list) & set(grootcv_list)
-        ), "expect non-empty intersection"
+import pytest
+import numpy as np
+import lightgbm as lgb
+from arfs.feature_selection.allrelevant import Leshy, BoostAGroota, GrootCV
+from arfs.utils import (
+    _generated_corr_dataset_regr,
+    _generated_corr_dataset_classification,
+)
+from arfs.utils import LightForestClassifier, LightForestRegressor
+
+
+class TestLeshy:
+    """
+    Test suite for all-relevant FS boruta-like method: Leshy
+    """
+
+    def test_borutaPy_vs_leshy_with_rfc_and_native_feature_importance(self):
+        # too slow for circleci to run them in a reasonable time
+        # takes 2 min on laptop, 1h or more on circleci
+        # sklearn random forest implementation
+        # X, y, w = _generated_corr_dataset_classification()
+        # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
+        # bt = BorutaPy(rfc)
+        # bt.fit(X.values, y)
+        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
+
+        # lightGBM random forest implementation
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+        X, y, w = _generated_corr_dataset_classification(size=100)
+        n_feat = X.shape[1]
+        rfc = LightForestClassifier(n_feat)
+        # RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100) # --> too slow
+        arfs = Leshy(rfc, verbose=0, max_iter=10, random_state=42, importance="native")
+        arfs.fit(X, y)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
+        assert bool(
+            set(baseline_list) & set(leshy_rfc_list)
+        ), "expect non-empty intersection"
+
+    def test_borutaPy_vs_leshy_with_rfr_and_native_feature_importance(self):
+        # too slow for circleci to run them in a reasonable time
+        # takes 2 min on laptop, 1h or more on circleci
+        # # sklearn random forest implementation
+        # X, y, w = _generated_corr_dataset_regr()
+        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
+        # bt = BorutaPy(rfr)
+        # bt.fit(X.values, y)
+        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
+
+        # lightGBM random forest implementation
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+        X, y, w = _generated_corr_dataset_regr(size=100)
+        n_feat = X.shape[1]
+        rfr = LightForestRegressor(n_feat)
+        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=10)
+        arfs = Leshy(rfr, verbose=0, max_iter=10, random_state=42, importance="native")
+        arfs.fit(X, y)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
+        assert bool(
+            set(baseline_list) & set(leshy_rfc_list)
+        ), "expect non-empty intersection"
+
+    def test_borutaPy_vs_leshy_with_rfc_and_shap_feature_importance(self):
+        # too slow for circleci to run them in a reasonable time
+        # takes 2 min on laptop, 1h or more on circleci
+        # # sklearn random forest implementation
+        # X, y, w = _generated_corr_dataset_classification()
+        # rfc = RandomForestClassifier(max_features='sqrt', max_samples=0.632, n_estimators=100)
+        # bt = BorutaPy(rfc)
+        # bt.fit(X.values, y)
+        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
+
+        # lightGBM random forest implementation
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+        X, y, w = _generated_corr_dataset_classification(size=100)
+        n_feat = X.shape[1]
+        model = LightForestClassifier(n_feat)
+        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
+        arfs.fit(X, y)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
+        assert bool(
+            set(baseline_list) & set(leshy_rfc_list)
+        ), "expect non-empty intersection"
+
+    def test_borutaPy_vs_leshy_with_rfr_and_shap_feature_importance(self):
+        # too slow for circleci to run them in a reasonable time
+        # takes 2 min on laptop, 1h or more on circleci
+        # # sklearn random forest implementation
+        # X, y, w = _generated_corr_dataset_regr()
+        # rfr = RandomForestRegressor(max_features=0.3, max_samples=0.632, n_estimators=100)
+        # bt = BorutaPy(rfr)
+        # bt.fit(X.values, y)
+        # borutapy_rfc_list = sorted(list(X.columns[bt.support_]))
+
+        # lightGBM random forest implementation
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+        X, y, w = _generated_corr_dataset_regr(size=500)
+        n_feat = X.shape[1]
+        model = LightForestRegressor(n_feat)
+        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
+        arfs.fit(X, y)
+        leshy_rfc_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        # assert borutapy_rfc_list == leshy_rfc_list, "same selected features are expected"
+        assert bool(
+            set(baseline_list) & set(leshy_rfc_list)
+        ), "expect non-empty intersection"
+
+    def test_leshy_clf_with_lgb_and_shap_feature_importance_and_sample_weight(self):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+
+        X, y, w = _generated_corr_dataset_classification(size=500)
+        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+    def test_leshy_regr_with_lgb_and_shap_feature_importance_and_sample_weight(self):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
+
+        X, y, w = _generated_corr_dataset_classification(size=500)
+        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = Leshy(model, verbose=0, max_iter=10, random_state=42, importance="shap")
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+
+class TestBoostAGroota:
+    """
+    Test suite for all-relevant FS boruta-like method: Leshy
+    """
+
+    def test_boostagroota_clf_with_lgb_and_shap_feature_importance_and_sample_weight(
+        self,
+    ):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+
+        X, y, w = _generated_corr_dataset_classification(size=500)
+        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = BoostAGroota(
+            est=model,
+            cutoff=1,
+            iters=3,
+            max_rounds=3,
+            delta=0.1,
+            silent=False,
+            importance="shap",
+        )
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+    def test_boostagroota_clf_with_lgb_and_pimp_feature_importance_and_sample_weight(
+        self,
+    ):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+
+        X, y, w = _generated_corr_dataset_classification(size=500)
+        model = lgb.LGBMClassifier(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = BoostAGroota(
+            est=model,
+            cutoff=1,
+            iters=3,
+            max_rounds=3,
+            delta=0.1,
+            silent=False,
+            importance="pimp",
+        )
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+    def test_boostagroota_rgr_with_lgb_and_shap_feature_importance_and_sample_weight(
+        self,
+    ):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
+
+        X, y, w = _generated_corr_dataset_regr(size=500)
+        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = BoostAGroota(
+            est=model,
+            cutoff=1,
+            iters=3,
+            max_rounds=3,
+            delta=0.1,
+            silent=False,
+            importance="shap",
+        )
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+    def test_boostagroota_regr_with_lgb_and_pimp_feature_importance_and_sample_weight(
+        self,
+    ):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
+
+        X, y, w = _generated_corr_dataset_regr(size=500)
+        model = lgb.LGBMRegressor(verbose=-1, force_col_wise=True, n_estimators=10)
+        arfs = BoostAGroota(
+            est=model,
+            cutoff=1,
+            iters=3,
+            max_rounds=3,
+            delta=0.1,
+            silent=False,
+            importance="pimp",
+        )
+        arfs.fit(X, y, w)
+        leshy_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(leshy_list)
+        ), "expect non-empty intersection"
+
+
+class TestGrootCV:
+    """
+    Test suite for all-relevant FS boruta-like method: Leshy
+    """
+
+    def test_grootcv_classification_with_and_sample_weight(self):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4"]
+
+        X, y, w = _generated_corr_dataset_classification(size=100)
+        arfs = GrootCV(objective="binary", cutoff=1, n_folds=3, n_iter=3, silent=False)
+        arfs.fit(X, y, w)
+        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(grootcv_list)
+        ), "expect non-empty intersection"
+
+    def test_grootcv_regression_with_and_sample_weight(self):
+        baseline_list = ["var0", "var1", "var2", "var3", "var4", "var5"]
+
+        X, y, w = _generated_corr_dataset_regr(size=100)
+        arfs = GrootCV(objective="l2", cutoff=1, n_folds=3, n_iter=3, silent=False)
+        arfs.fit(X, y, w)
+        grootcv_list = sorted(arfs.feature_names_in_[arfs.support_])
+
+        assert bool(
+            set(baseline_list) & set(grootcv_list)
+        ), "expect non-empty intersection"
```

### Comparing `arfs-2.0.4/tests/test_featselect.py` & `arfs-2.0.5/tests/test_featselect.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-import pytest
-import numpy as np
-import pandas as pd
-from arfs.feature_selection import (
-    MissingValueThreshold,
-    UniqueValuesThreshold,
-    CardinalityThreshold,
-    CollinearityThreshold,
-)
-from arfs.utils import (
-    _generated_corr_dataset_regr,
-    _generated_corr_dataset_classification,
-)
-
-
-class TestFeatSelectMissing:
-    """
-    Test suite for FeatureSelector, missing values
-    """
-
-    def test_identify_missing_for_classification(self):
-        # not task dependent (same for clf and regr)
-        X, y, w = _generated_corr_dataset_classification(size=10)
-        fs = MissingValueThreshold(threshold=0.01)
-        fs.fit(X)
-        message = "Expected: {0}, Actual: {1}".format(
-            "var12", fs.not_selected_features_
-        )
-        assert fs.not_selected_features_ == ["var12"], message
-
-
-class TestFeatSelectZeroVariance:
-    """
-    Test suite for FeatureSelector, missing values
-    """
-
-    def test_identify_single_unique_classification(self):
-        # not task dependent (same for clf and regr)
-        X, y, w = _generated_corr_dataset_classification(size=10)
-        fs = UniqueValuesThreshold(threshold=2)
-        fs.fit(X)
-        message = "Expected: {0}, Actual: {1}".format(
-            "var10", fs.not_selected_features_
-        )
-        assert fs.not_selected_features_ == ["var10"], message
-
-
-class TestFeatSelectHighCardinality:
-    """
-    Test suite for FeatureSelector, high cardinality
-    """
-
-    def test_identify_high_cardinality_classification(self):
-        # not task dependent (same for clf and regr)
-        X, y, w = _generated_corr_dataset_classification(size=100)
-        fs = CardinalityThreshold(threshold=5)
-        fs.fit(X)
-        expected = sorted(["dummy", "nice_guys"])
-        actual = sorted(list(fs.not_selected_features_))
-        message = "Expected: {0}, Actual: {1}".format(expected, actual)
-        assert actual == expected, message
-
-
-# class TestFeatSelectCollinearity:
-#     """
-#     test suite for FeatureSelector, high cardinality
-#     """
-
-#     def test_identify_collinear_spearman_no_encoding(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_collinear(correlation_threshold=0.5, encode=False, method='spearman')
-#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var4', 'var12'], fs.ops['collinear'])
-#         assert fs.ops['collinear'] == ['var2', 'var3', 'var4', 'var12'], message
-
-#     def test_identify_collinear_pearson_no_encoding(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_collinear(correlation_threshold=0.5, encode=False, method='pearson')
-#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var12'], fs.ops['collinear'])
-#         assert fs.ops['collinear'] == ['var2', 'var3', 'var12'], message
-
-#     def test_identify_collinear_spearman_with_encoding(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_collinear(correlation_threshold=0.5, encode=True, method='spearman')
-#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var4', 'var12'], fs.ops['collinear'])
-#         assert fs.ops['collinear'] == ['var2', 'var3', 'var4', 'var12'], message
-
-#     def test_identify_collinear_pearson_with_encoding(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_collinear(correlation_threshold=0.5, encode=True, method='pearson')
-#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var12'], fs.ops['collinear'])
-#         assert fs.ops['collinear'] == ['var2', 'var3', 'var12'], message
-
-
-# class TestFeatSelectZeroImportance:
-#     """
-#     test suite for FeatureSelector, high cardinality
-#     """
-
-#     def test_identify_zero_importance_for_regression_with_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_regression_with_early_stopping_no_eval_metric(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric=None, objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_regression_with_early_stopping_no_eval_metric_no_objective(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric=None, objective=None, n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_regression_with_early_stopping_wrong_task(self):
-#         X, y, w = _generated_corr_dataset_regr(size=10)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric='l2', objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     def test_identify_zero_importance_for_regression_without_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
-#                                     early_stopping=False)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     def test_identify_zero_importance_for_regression_without_early_stopping_no_objective(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', n_iterations=2,
-#                                     early_stopping=False)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     def test_identify_zero_importance_for_classification_with_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='classification', eval_metric='auc', n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_classification_with_early_stopping_no_eval_metric(self):
-#         X, y, w = _generated_corr_dataset_classification(size=10)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric=None, n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_classification_with_early_stopping_no_eval_metric_no_objective(self):
-#         X, y, w = _generated_corr_dataset_classification(size=10)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric=None, objective=None, n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     @pytest.mark.xfail
-#     def test_identify_zero_importance_for_classification_with_early_stopping_wrong_task(self):
-#         X, y, w = _generated_corr_dataset_classification(size=10)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric='auc', objective='cross-entropy', n_iterations=2,
-#                                     early_stopping=True)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     def test_identify_zero_importance_for_classification_without_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='classification', objective='binary', n_iterations=2,
-#                                     early_stopping=False)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-#     def test_identify_zero_importance_for_classification_without_early_stopping_no_objective(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='classification', n_iterations=2,
-#                                     early_stopping=False)
-#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
-#         assert 'var10' in fs.ops['zero_importance'], message
-
-
-# class TestFeatSelectLowImportance:
-#     """
-#     test suite for FeatureSelector, high cardinality
-#     """
-
-#     def test_identify_low_importance_for_regression_with_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_regression_with_early_stopping_no_eval_metric(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric=None, objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_regression_with_early_stopping_no_eval_metric_no_objective(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric=None, objective=None, n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_regression_with_early_stopping_wrong_task(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric='l2', objective='l2', n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     def test_identify_low_importance_for_regression_without_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', objective='l2', n_iterations=2, early_stopping=False)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     def test_identify_low_importance_for_regression_without_early_stopping_no_objective(self):
-#         X, y, w = _generated_corr_dataset_regr(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='regression', n_iterations=2, early_stopping=False)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     def test_identify_low_importance_for_classification_with_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='classification', eval_metric='auc', n_iterations=2, early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_classification_with_early_stopping_no_eval_metric(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric=None, n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_classification_with_early_stopping_no_eval_metric_no_objective(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='classification', eval_metric=None, objective=None, n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     @pytest.mark.xfail
-#     def test_identify_low_importance_for_classification_with_early_stopping_wrong_task(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         # Xfail: expected to fail because the eval metric is not provided
-#         fs.identify_zero_importance(task='regression', eval_metric='auc', objective='cross-entropy', n_iterations=2,
-#                                     early_stopping=True)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
-
-#     def test_identify_low_importance_for_classification_without_early_stopping(self):
-#         X, y, w = _generated_corr_dataset_classification(size=100)
-#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
-#         fs.identify_zero_importance(task='classification', n_iterations=2, early_stopping=False)
-#         cum_imp_threshold = 0.95
-#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
-#         expected = 1
-#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
-#         assert len(fs.ops['low_importance']) >= expected, message
+import pytest
+import numpy as np
+import pandas as pd
+from arfs.feature_selection import (
+    MissingValueThreshold,
+    UniqueValuesThreshold,
+    CardinalityThreshold,
+    CollinearityThreshold,
+)
+from arfs.utils import (
+    _generated_corr_dataset_regr,
+    _generated_corr_dataset_classification,
+)
+
+
+class TestFeatSelectMissing:
+    """
+    Test suite for FeatureSelector, missing values
+    """
+
+    def test_identify_missing_for_classification(self):
+        # not task dependent (same for clf and regr)
+        X, y, w = _generated_corr_dataset_classification(size=10)
+        fs = MissingValueThreshold(threshold=0.01)
+        fs.fit(X)
+        message = "Expected: {0}, Actual: {1}".format(
+            "var12", fs.not_selected_features_
+        )
+        assert fs.not_selected_features_ == ["var12"], message
+
+
+class TestFeatSelectZeroVariance:
+    """
+    Test suite for FeatureSelector, missing values
+    """
+
+    def test_identify_single_unique_classification(self):
+        # not task dependent (same for clf and regr)
+        X, y, w = _generated_corr_dataset_classification(size=10)
+        fs = UniqueValuesThreshold(threshold=2)
+        fs.fit(X)
+        message = "Expected: {0}, Actual: {1}".format(
+            "var10", fs.not_selected_features_
+        )
+        assert fs.not_selected_features_ == ["var10"], message
+
+
+class TestFeatSelectHighCardinality:
+    """
+    Test suite for FeatureSelector, high cardinality
+    """
+
+    def test_identify_high_cardinality_classification(self):
+        # not task dependent (same for clf and regr)
+        X, y, w = _generated_corr_dataset_classification(size=100)
+        fs = CardinalityThreshold(threshold=5)
+        fs.fit(X)
+        expected = sorted(["dummy", "nice_guys"])
+        actual = sorted(list(fs.not_selected_features_))
+        message = "Expected: {0}, Actual: {1}".format(expected, actual)
+        assert actual == expected, message
+
+
+# class TestFeatSelectCollinearity:
+#     """
+#     test suite for FeatureSelector, high cardinality
+#     """
+
+#     def test_identify_collinear_spearman_no_encoding(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_collinear(correlation_threshold=0.5, encode=False, method='spearman')
+#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var4', 'var12'], fs.ops['collinear'])
+#         assert fs.ops['collinear'] == ['var2', 'var3', 'var4', 'var12'], message
+
+#     def test_identify_collinear_pearson_no_encoding(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_collinear(correlation_threshold=0.5, encode=False, method='pearson')
+#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var12'], fs.ops['collinear'])
+#         assert fs.ops['collinear'] == ['var2', 'var3', 'var12'], message
+
+#     def test_identify_collinear_spearman_with_encoding(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_collinear(correlation_threshold=0.5, encode=True, method='spearman')
+#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var4', 'var12'], fs.ops['collinear'])
+#         assert fs.ops['collinear'] == ['var2', 'var3', 'var4', 'var12'], message
+
+#     def test_identify_collinear_pearson_with_encoding(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_collinear(correlation_threshold=0.5, encode=True, method='pearson')
+#         message = "Expected: {0}, Actual: {1}".format(['var2', 'var3', 'var12'], fs.ops['collinear'])
+#         assert fs.ops['collinear'] == ['var2', 'var3', 'var12'], message
+
+
+# class TestFeatSelectZeroImportance:
+#     """
+#     test suite for FeatureSelector, high cardinality
+#     """
+
+#     def test_identify_zero_importance_for_regression_with_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_regression_with_early_stopping_no_eval_metric(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric=None, objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_regression_with_early_stopping_no_eval_metric_no_objective(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric=None, objective=None, n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_regression_with_early_stopping_wrong_task(self):
+#         X, y, w = _generated_corr_dataset_regr(size=10)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric='l2', objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     def test_identify_zero_importance_for_regression_without_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
+#                                     early_stopping=False)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     def test_identify_zero_importance_for_regression_without_early_stopping_no_objective(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', n_iterations=2,
+#                                     early_stopping=False)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     def test_identify_zero_importance_for_classification_with_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='classification', eval_metric='auc', n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_classification_with_early_stopping_no_eval_metric(self):
+#         X, y, w = _generated_corr_dataset_classification(size=10)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric=None, n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_classification_with_early_stopping_no_eval_metric_no_objective(self):
+#         X, y, w = _generated_corr_dataset_classification(size=10)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric=None, objective=None, n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     @pytest.mark.xfail
+#     def test_identify_zero_importance_for_classification_with_early_stopping_wrong_task(self):
+#         X, y, w = _generated_corr_dataset_classification(size=10)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric='auc', objective='cross-entropy', n_iterations=2,
+#                                     early_stopping=True)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     def test_identify_zero_importance_for_classification_without_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='classification', objective='binary', n_iterations=2,
+#                                     early_stopping=False)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+#     def test_identify_zero_importance_for_classification_without_early_stopping_no_objective(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='classification', n_iterations=2,
+#                                     early_stopping=False)
+#         message = "Expected: {0}, Actual: {1}".format(['var10'], fs.ops['zero_importance'])
+#         assert 'var10' in fs.ops['zero_importance'], message
+
+
+# class TestFeatSelectLowImportance:
+#     """
+#     test suite for FeatureSelector, high cardinality
+#     """
+
+#     def test_identify_low_importance_for_regression_with_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', eval_metric='l2', objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_regression_with_early_stopping_no_eval_metric(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric=None, objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_regression_with_early_stopping_no_eval_metric_no_objective(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric=None, objective=None, n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_regression_with_early_stopping_wrong_task(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric='l2', objective='l2', n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     def test_identify_low_importance_for_regression_without_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', objective='l2', n_iterations=2, early_stopping=False)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     def test_identify_low_importance_for_regression_without_early_stopping_no_objective(self):
+#         X, y, w = _generated_corr_dataset_regr(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='regression', n_iterations=2, early_stopping=False)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     def test_identify_low_importance_for_classification_with_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='classification', eval_metric='auc', n_iterations=2, early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_classification_with_early_stopping_no_eval_metric(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric=None, n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_classification_with_early_stopping_no_eval_metric_no_objective(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='classification', eval_metric=None, objective=None, n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     @pytest.mark.xfail
+#     def test_identify_low_importance_for_classification_with_early_stopping_wrong_task(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         # Xfail: expected to fail because the eval metric is not provided
+#         fs.identify_zero_importance(task='regression', eval_metric='auc', objective='cross-entropy', n_iterations=2,
+#                                     early_stopping=True)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
+
+#     def test_identify_low_importance_for_classification_without_early_stopping(self):
+#         X, y, w = _generated_corr_dataset_classification(size=100)
+#         fs = FeatureSelector(X=X, y=y, sample_weight=w)
+#         fs.identify_zero_importance(task='classification', n_iterations=2, early_stopping=False)
+#         cum_imp_threshold = 0.95
+#         fs.identify_low_importance(cumulative_importance=cum_imp_threshold)
+#         expected = 1
+#         message = "Expected at least one predictor ruled out, Actual: {0}".format(sorted(fs.ops['low_importance']))
+#         assert len(fs.ops['low_importance']) >= expected, message
```

