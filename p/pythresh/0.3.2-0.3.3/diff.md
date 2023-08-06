# Comparing `tmp/pythresh-0.3.2.tar.gz` & `tmp/pythresh-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythresh-0.3.2.tar", last modified: Sun Jul  2 07:18:36 2023, max compression
+gzip compressed data, was "pythresh-0.3.3.tar", last modified: Sun Aug  6 15:26:21 2023, max compression
```

## Comparing `pythresh-0.3.2.tar` & `pythresh-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.580541 pythresh-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-02 07:18:20.000000 pythresh-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-02 07:18:20.000000 pythresh-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28627 2023-07-02 07:18:36.580541 pythresh-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-07-02 07:18:20.000000 pythresh-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.564540 pythresh-0.3.2/pythresh/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.568540 pythresh-0.3.2/pythresh/models/
--rw-r--r--   0 runner    (1001) docker     (123)   141564 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNB.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   141284 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNBC.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   165531 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_GNBM.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  3181480 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/models/meta_model_LIN.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.580541 pythresh-0.3.2/pythresh/thresholds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/aucp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/chau.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/clf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/clust.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/comb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/cpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/dsn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/eb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/fgd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/fwfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/gesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/iqr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3447 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/karch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mcst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/moll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/mtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/ocsvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/qmcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/regr.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/thresh_utility.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10061 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/vae.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/yj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 07:18:20.000000 pythresh-0.3.2/pythresh/thresholds/zscore.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-02 07:18:21.000000 pythresh-0.3.2/pythresh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:18:36.568540 pythresh-0.3.2/pythresh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28627 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 07:18:36.000000 pythresh-0.3.2/pythresh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 07:18:20.000000 pythresh-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 07:18:36.580541 pythresh-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-02 07:18:20.000000 pythresh-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:26:21.008719 pythresh-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-06 15:25:07.000000 pythresh-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-06 15:25:07.000000 pythresh-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-08-06 15:26:21.008719 pythresh-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28936 2023-08-06 15:25:07.000000 pythresh-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:26:20.996717 pythresh-0.3.3/pythresh/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:26:21.000718 pythresh-0.3.3/pythresh/models/
+-rw-r--r--   0 runner    (1001) docker     (123)   141564 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/models/meta_model_GNB.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   141284 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/models/meta_model_GNBC.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   165531 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/models/meta_model_GNBM.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  3181480 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/models/meta_model_LIN.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:26:21.008719 pythresh-0.3.3/pythresh/thresholds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/aucp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/chau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/clf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/clust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/comb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/cpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/dsn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/eb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/fgd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5276 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/fwfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/gamgmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/gesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/iqr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/karch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/mad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/mcst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/moll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/mtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/ocsvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/qmcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/thresh_utility.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10154 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/yj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/thresholds/zscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-06 15:25:07.000000 pythresh-0.3.3/pythresh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:26:20.996717 pythresh-0.3.3/pythresh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-08-06 15:26:20.000000 pythresh-0.3.3/pythresh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-06 15:26:20.000000 pythresh-0.3.3/pythresh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:26:20.000000 pythresh-0.3.3/pythresh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-06 15:26:20.000000 pythresh-0.3.3/pythresh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 15:26:20.000000 pythresh-0.3.3/pythresh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-06 15:25:07.000000 pythresh-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-06 15:26:21.008719 pythresh-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-06 15:25:07.000000 pythresh-0.3.3/setup.py
```

### Comparing `pythresh-0.3.2/LICENSE` & `pythresh-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.2/PKG-INFO` & `pythresh-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythresh
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python Toolbox for Outlier Detection Thresholding
 Home-page: https://github.com/KulikDM/pythresh
 Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
 Author: D Kulik
 Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
 Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,27 +71,28 @@
 .. image:: https://zenodo.org/badge/497683169.svg
    :target: https://zenodo.org/badge/latestdoi/497683169
    :alt: Zenodo DOI
 
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
-**thresholding outlier detection scores** in univariate/multivariate
-data. It has been writen to work in tandem with PyOD and has similar
-syntax and data structures. However, it is not limited to this single
-library. PyThresh is meant to threshold scores generated by an outlier
-detection. It thresholds scores without the need to set a contamination
-level or have the user guess the amount of outliers that may exist in
-the dataset beforehand. These non-parametric methods were written to
-reduce the user's input/guess work and rather rely on statistics instead
-to threshold outlier scores. For thresholding to be applied correctly,
-the outlier detection scores must follow this rule: the higher the
-score, the higher the probability that it is an outlier in the dataset.
-All threshold functions return a binary array where inliers and outliers
-are represented by a 0 and 1 respectively.
+**thresholding outlier detection likelihood scores** in
+univariate/multivariate data. It has been written to work in tandem with
+PyOD and has similar syntax and data structures. However, it is not
+limited to this single library. PyThresh is meant to threshold
+likelihood scores generated by an outlier detector. It thresholds these
+likelihood scores and replaces the need to set a contamination level or
+have the user guess the amount of outliers that may exist in the dataset
+beforehand. These non-parametric methods were written to reduce the
+user's input/guess work and rather rely on statistics instead to
+threshold outlier likelihood scores. For thresholding to be applied
+correctly, the outlier detection likelihood scores must follow this
+rule: the higher the score, the higher the probability that it is an
+outlier in the dataset. All threshold functions return a binary array
+where inliers and outliers are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
 ************************
  Documentation & Citing
@@ -121,14 +122,35 @@
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
    thres = FILTER()
    labels = thres.eval(decision_scores)
 
+or using multiple outlier detection score sets
+
+.. code:: python
+
+   # train multiple detectors
+   from pyod.models.knn import KNN
+   from pyod.models.pca import PCA
+   from pyod.models.iforest import IForest
+   from pythresh.thresholds.filter import FILTER
+
+   clfs = [KNN(), IForest(), PCA()]
+
+   # get outlier scores for each detector
+   scores = [clf.fit(X_train).decision_scores_ for clf in clfs]
+
+   scores = np.vstack(scores).T
+
+   # get outlier labels
+   thres = FILTER()
+   labels = thres.eval(scores)
+
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
 
 .. code:: bash
@@ -174,41 +196,45 @@
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
 
 ****************
  API Cheatsheet
 ****************
 
--  **eval(score)**: evaluate outlier score.
+-  **eval(score)**: evaluate a single outlier or multiple outlier
+   detection likelihood score sets.
 
 Key Attributes of threshold:
 
 -  **thresh_**: Return the threshold value that separates inliers from
    outliers. Outliers are considered all values above this threshold
-   value. Note the threshold value has been derived from normalized
-   scores.
+   value. Note the threshold value has been derived from likelihood
+   scores normalized between 0 and 1.
 
 -  **confidence_interval_**: Return the lower and upper confidence
    interval of the contamination level. Only applies to the COMB
    thresholder
 
+-  **dscores_**: 1D array of the TruncatedSVD decomposed decision scores
+   if multiple outlier detector score sets are passed
+
 ************************
  External Feature Cases
 ************************
 
 **Towards Data Science**: `Thresholding Outlier Detection Scores with
 PyThresh
 <https://towardsdatascience.com/thresholding-outlier-detection-scores-with-pythresh-f26299d14fa>`_
 
 **Towards Data Science**: `When Outliers are Significant: Weighted
 Linear Regression
 <https://towardsdatascience.com/when-outliers-are-significant-weighted-linear-regression-bcdc8389ab10>`_
 
 **ArXiv**: `Estimating the Contamination Factor's Distribution in
-Unsupervised Anomaly Detection <https://arxiv.org/abs/2210.10487>`_
+Unsupervised Anomaly Detection. <https://arxiv.org/abs/2210.10487>`_
 
 ***********************************
  Available Thresholding Algorithms
 ***********************************
 
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Abbr      | Description                               | References         | Documentation                                                                                                                                          |
@@ -233,14 +259,16 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FGD       | Fixed Gradient Descent                    | [#fgd1]_           | `pythresh.thresholds.fgd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fgd>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FILTER    | Filtering Based                           | [#filter1]_        | `pythresh.thresholds.filter module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.filter>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FWFM      | Full Width at Full Minimum                | [#fwfm1]_          | `pythresh.thresholds.fwfm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fwfm>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
+| GAMGMM    | Bayesian Gamma GMM                        | [#gamgmm1]_        | `pythresh.thresholds.gamgmm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gamgmm>`_            |
++-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | GESD      | Generalized Extreme Studentized Deviate   | [#gesd1]_          | `pythresh.thresholds.gesd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gesd>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | HIST      | Histogram Based                           | [#hist1]_          | `pythresh.thresholds.hist module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.hist>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | IQR       | Inter-Quartile Region                     | [#iqr1]_           | `pythresh.thresholds.iqr module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.iqr>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | KARCH     | Karcher mean (Riemannian Center of Mass)  | [#karch1]_         | `pythresh.thresholds.karch module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.karch>`_              |
@@ -401,14 +429,19 @@
    <https://ieeexplore.ieee.org/document/9029258/>`_
 
 .. [#fwfm1]
 
    `Sparse Auto-Regressive: Robust Estimation of AR Parameters
    <https://arxiv.org/abs/1306.3317>`_
 
+.. [#gamgmm1]
+
+   `Estimating the Contamination Factor's Distribution in Unsupervised
+   Anomaly Detection <https://proceedings.mlr.press/v202/perini23a.html>`_
+
 .. [#gesd1]
 
    `An adjusted Grubbs' and generalized extreme studentized deviation
    <https://www.degruyter.com/document/doi/10.1515/dema-2021-0041/html?lang=en>`_
 
 .. [#hist1]
```

### Comparing `pythresh-0.3.2/README.rst` & `pythresh-0.3.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -47,27 +47,28 @@
 .. image:: https://zenodo.org/badge/497683169.svg
    :target: https://zenodo.org/badge/latestdoi/497683169
    :alt: Zenodo DOI
 
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
-**thresholding outlier detection scores** in univariate/multivariate
-data. It has been writen to work in tandem with PyOD and has similar
-syntax and data structures. However, it is not limited to this single
-library. PyThresh is meant to threshold scores generated by an outlier
-detection. It thresholds scores without the need to set a contamination
-level or have the user guess the amount of outliers that may exist in
-the dataset beforehand. These non-parametric methods were written to
-reduce the user's input/guess work and rather rely on statistics instead
-to threshold outlier scores. For thresholding to be applied correctly,
-the outlier detection scores must follow this rule: the higher the
-score, the higher the probability that it is an outlier in the dataset.
-All threshold functions return a binary array where inliers and outliers
-are represented by a 0 and 1 respectively.
+**thresholding outlier detection likelihood scores** in
+univariate/multivariate data. It has been written to work in tandem with
+PyOD and has similar syntax and data structures. However, it is not
+limited to this single library. PyThresh is meant to threshold
+likelihood scores generated by an outlier detector. It thresholds these
+likelihood scores and replaces the need to set a contamination level or
+have the user guess the amount of outliers that may exist in the dataset
+beforehand. These non-parametric methods were written to reduce the
+user's input/guess work and rather rely on statistics instead to
+threshold outlier likelihood scores. For thresholding to be applied
+correctly, the outlier detection likelihood scores must follow this
+rule: the higher the score, the higher the probability that it is an
+outlier in the dataset. All threshold functions return a binary array
+where inliers and outliers are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
 ************************
  Documentation & Citing
@@ -97,14 +98,35 @@
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
    thres = FILTER()
    labels = thres.eval(decision_scores)
 
+or using multiple outlier detection score sets
+
+.. code:: python
+
+   # train multiple detectors
+   from pyod.models.knn import KNN
+   from pyod.models.pca import PCA
+   from pyod.models.iforest import IForest
+   from pythresh.thresholds.filter import FILTER
+
+   clfs = [KNN(), IForest(), PCA()]
+
+   # get outlier scores for each detector
+   scores = [clf.fit(X_train).decision_scores_ for clf in clfs]
+
+   scores = np.vstack(scores).T
+
+   # get outlier labels
+   thres = FILTER()
+   labels = thres.eval(scores)
+
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
 
 .. code:: bash
@@ -150,41 +172,45 @@
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
 
 ****************
  API Cheatsheet
 ****************
 
--  **eval(score)**: evaluate outlier score.
+-  **eval(score)**: evaluate a single outlier or multiple outlier
+   detection likelihood score sets.
 
 Key Attributes of threshold:
 
 -  **thresh_**: Return the threshold value that separates inliers from
    outliers. Outliers are considered all values above this threshold
-   value. Note the threshold value has been derived from normalized
-   scores.
+   value. Note the threshold value has been derived from likelihood
+   scores normalized between 0 and 1.
 
 -  **confidence_interval_**: Return the lower and upper confidence
    interval of the contamination level. Only applies to the COMB
    thresholder
 
+-  **dscores_**: 1D array of the TruncatedSVD decomposed decision scores
+   if multiple outlier detector score sets are passed
+
 ************************
  External Feature Cases
 ************************
 
 **Towards Data Science**: `Thresholding Outlier Detection Scores with
 PyThresh
 <https://towardsdatascience.com/thresholding-outlier-detection-scores-with-pythresh-f26299d14fa>`_
 
 **Towards Data Science**: `When Outliers are Significant: Weighted
 Linear Regression
 <https://towardsdatascience.com/when-outliers-are-significant-weighted-linear-regression-bcdc8389ab10>`_
 
 **ArXiv**: `Estimating the Contamination Factor's Distribution in
-Unsupervised Anomaly Detection <https://arxiv.org/abs/2210.10487>`_
+Unsupervised Anomaly Detection. <https://arxiv.org/abs/2210.10487>`_
 
 ***********************************
  Available Thresholding Algorithms
 ***********************************
 
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Abbr      | Description                               | References         | Documentation                                                                                                                                          |
@@ -209,14 +235,16 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FGD       | Fixed Gradient Descent                    | [#fgd1]_           | `pythresh.thresholds.fgd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fgd>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FILTER    | Filtering Based                           | [#filter1]_        | `pythresh.thresholds.filter module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.filter>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FWFM      | Full Width at Full Minimum                | [#fwfm1]_          | `pythresh.thresholds.fwfm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fwfm>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
+| GAMGMM    | Bayesian Gamma GMM                        | [#gamgmm1]_        | `pythresh.thresholds.gamgmm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gamgmm>`_            |
++-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | GESD      | Generalized Extreme Studentized Deviate   | [#gesd1]_          | `pythresh.thresholds.gesd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gesd>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | HIST      | Histogram Based                           | [#hist1]_          | `pythresh.thresholds.hist module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.hist>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | IQR       | Inter-Quartile Region                     | [#iqr1]_           | `pythresh.thresholds.iqr module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.iqr>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | KARCH     | Karcher mean (Riemannian Center of Mass)  | [#karch1]_         | `pythresh.thresholds.karch module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.karch>`_              |
@@ -377,14 +405,19 @@
    <https://ieeexplore.ieee.org/document/9029258/>`_
 
 .. [#fwfm1]
 
    `Sparse Auto-Regressive: Robust Estimation of AR Parameters
    <https://arxiv.org/abs/1306.3317>`_
 
+.. [#gamgmm1]
+
+   `Estimating the Contamination Factor's Distribution in Unsupervised
+   Anomaly Detection <https://proceedings.mlr.press/v202/perini23a.html>`_
+
 .. [#gesd1]
 
    `An adjusted Grubbs' and generalized extreme studentized deviation
    <https://www.degruyter.com/document/doi/10.1515/dema-2021-0041/html?lang=en>`_
 
 .. [#hist1]
```

### Comparing `pythresh-0.3.2/pythresh/models/meta_model_GNB.pkl` & `pythresh-0.3.3/pythresh/models/meta_model_GNB.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.2/pythresh/models/meta_model_GNBC.pkl` & `pythresh-0.3.3/pythresh/models/meta_model_GNBC.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.2/pythresh/models/meta_model_GNBM.pkl` & `pythresh-0.3.3/pythresh/models/meta_model_GNBM.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.2/pythresh/models/meta_model_LIN.pkl` & `pythresh-0.3.3/pythresh/models/meta_model_LIN.pkl`

 * *Files identical despite different names*

### Comparing `pythresh-0.3.2/pythresh/thresholds/aucp.py` & `pythresh-0.3.3/pythresh/thresholds/aucp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import numpy as np
 from sklearn.metrics import auc
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_kde, normalize
 
 
 class AUCP(BaseThresholder):
     r"""AUCP class for Area Under Curve Precentage thresholder.
 
        Use the area under the curve to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond where the auc of the kde is less
        than the (mean + abs(mean-median)) percent of the total kde auc.
        See :cite:`ren2018aucp` for details
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The area under the curve (AUC) is defined as follows:
 
        .. math::
 
@@ -45,39 +50,42 @@
 
        The first AUC that is greater than the total AUC of the pdf multiplied by the
        :math:`\mathrm{lim}` is set as the threshold between inliers and outliers.
 
 
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        pass
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Generate KDE
         val, dat_range = gen_kde(decision, 0, 1, len(decision)*2)
         val = normalize(val)
 
         # Get the total area under the curve
         tot_area = auc(dat_range, val)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/base.py` & `pythresh-0.3.3/pythresh/thresholds/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,35 @@
        Parameters
        ----------
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
+
+       confidence_interval_ : lower and upper confidence interval of the contamination level
+
+       dscores_ : 1D array of decomposed decision scores
     """
 
     @abc.abstractmethod
     def __init__(self):
 
         self.thresh_ = None
         self.confidence_interval_ = None
+        self.dscores_ = None
 
     @abc.abstractmethod
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/boot.py` & `pythresh-0.3.3/pythresh/thresholds/boot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class BOOT(BaseThresholder):
     r"""BOOT class for Bootstrapping thresholder.
 
        Use a bootstrapping based method to find a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -20,14 +19,16 @@
             Random seed for bootstrapping a confidence interval. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The two sided bias-corrected and accelerated bootstrap confidence interval
        is calculated with a confidence level of 0.95. The statistic calculating
        the confidence interval is the standard deviation of the decision
        scores, with the statistic treating corresponding elements of the
@@ -35,16 +36,16 @@
 
        The returned upper and lower confidence intervals are used to threshold
        the decision scores. Outliers are set to any value above the mean of the
        upper and lower confidence intervals.
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -70,29 +71,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         limit1, limit2 = stats.bootstrap(
             decision.reshape(1, -1),
             np.std,
             paired=True,
             random_state=self.random_state
         ).confidence_interval
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/chau.py` & `pythresh-0.3.3/pythresh/thresholds/chau.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import scipy.stats as stats
 from scipy.special import erfc
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class CHAU(BaseThresholder):
     r"""CHAU class for Chauvenet's criterion thresholder.
 
        Use the Chauvenet's criterion to evaluate a non-parametric
        means to threshold scores generated by the decision_scores
@@ -21,19 +20,25 @@
        method : {'mean', 'median', 'gmean'}, optional (default='mean')
             Calculate the area normal to distance using a scaler
 
             - 'mean':  Construct a scaler with the the mean of the scores
             - 'median: Construct a scaler with the the median of the scores
             - 'gmean': Construct a scaler with the geometric mean of the scores
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The Chauvenet's criterion for a one tail of a distribution is defined
        as follows:
 
        .. math::
@@ -69,41 +74,45 @@
        replaced with the geometric mean or the median.
 
        Any z-score greater than the Chauvenet's criterion is considered an outlier.
 
 
     """
 
-    def __init__(self, method='mean'):
+    def __init__(self, method='mean', random_state=1234):
 
         super().__init__()
         stat = {'mean': np.mean, 'median': np.median, 'gmean': stats.gmean}
         self.method = stat[method]
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Calculate Chauvenet's criterion for one tail
         Pz = 1/(4*len(decision))
         criterion = 1/abs(stats.norm.ppf(Pz))
 
         # Get area normal to distance
         prob = erfc(np.abs(decision-self.method(decision)) /
                     decision.std()/2.0**0.5)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/clf.py` & `pythresh-0.3.3/pythresh/thresholds/clf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from scipy.stats import gaussian_kde
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import normalize
+from .thresh_utility import check_scores, normalize
 
 
 class CLF(BaseThresholder):
     r"""CLF class for Trained Classifier thresholder.
 
        Use the trained linear classifier to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -18,68 +17,78 @@
 
        method : {'simple', 'complex'}, optional (default='complex')
             Type of linear model
 
             - 'simple':  Uses only the scores
             - 'complex': Uses the scores, log of the scores, and the scores' PDF
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The classifier was trained using a linear stochastic gradient decent method.
        A warm start was assigned to the classifier was partially fit with the decision
        scores and true labels from multiple outlier detection methods available in `PyOD`.
        The :code:`generate_data` function from `PyOD` was used to create the outlier data,
        and the contaminations and random states were randomized each iterative step.
 
 
     """
 
-    def __init__(self, method='complex'):
+    def __init__(self, method='complex', random_state=1234):
 
         if method == 'complex':
 
             self.m1 = 7.115947536708103
             self.m2 = -5.934885742167458
             self.m3 = -3.416078337348704
             self.c = 2.5731351150980992
 
         else:
 
             self.m = 4.0581548062264075
             self.c = -1.5357998356223497
 
         self.method = method
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Calculate expected y
         if self.method == 'complex':
 
             kde = gaussian_kde(decision)
             pdf = normalize(kde.pdf(decision))
             pdf = normalize(pdf**(1/10))
             log = normalize(np.log(decision + 1))
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/clust.py` & `pythresh-0.3.3/pythresh/thresholds/clust.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     SpectralClustering,
     estimate_bandwidth
 )
 from sklearn.mixture import BayesianGaussianMixture
 from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import normalize
+from .thresh_utility import check_scores, normalize
 
 
 class CLUST(BaseThresholder):
     """CLUST class for clustering type thresholders.
 
        Use the clustering methods to evaluate a non-parametric means to
        threshold scores generated by the decision_scores where outliers
@@ -57,18 +57,20 @@
             also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -104,28 +106,34 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
         decision = check_array(decision, ensure_2d=False)
 
-        decision = normalize(decision).reshape(-1, 1)
+        decision = normalize(decision)
+
+        if decision.ndim == 1:
+            decision = np.atleast_2d(decision).T
+
+        self.dscores_ = None
 
         labels = self.method_funcs[str(self.method)](decision)
 
         self.thresh_ = None
 
         return labels
 
@@ -134,27 +142,27 @@
 
         cl.process()
 
         pred = np.squeeze(np.array(cl.get_clusters(), dtype=object))
 
         pred = np.array(pred[0]) if type(pred[0]) == list else pred
 
-        labels = np.ones(len(decision))
+        labels = np.ones(len(decision), dtype=int)
         labels[pred.astype(int)] = 0
 
         # Flip if outliers were clustered
         labels = 1-labels if sum(labels) > np.ceil(len(decision)/2) else labels
 
         return labels
 
     def _sklearn_eval(self, cl, decision):
         """Evaluate cluster labels from sklearn methods."""
 
         cl.fit(decision)
-        labels = cl.labels_
+        labels = cl.labels_.astype(int)
 
         # Flip if outliers were clustered
         labels = 1-labels if sum(labels) > np.ceil(len(decision)/2) else labels
 
         return labels
 
     def _AGG_clust(self, decision):
@@ -246,21 +254,23 @@
 
         return self._pyclust_eval(cl, decision)
 
     def _MSHIFT_clust(self, decision):
         """Mean shift algorithm for cluster analysis."""
 
         # Get quantile value for bandwidth estimation
-        dat = np.squeeze(decision)
+        cscores = check_scores(decision,
+                               random_state=self.random_state)
+        dat = np.squeeze(cscores)
         q = cityblock(dat, np.sort(dat))/np.sum(dat)
 
         q = max(0.25, min(q, 1.0))
 
         # Estimate bandwidth
-        bw = estimate_bandwidth(decision, quantile=q)
+        bw = estimate_bandwidth(dat.reshape(-1, 1), quantile=q)
 
         cl = MeanShift(bandwidth=bw, cluster_all=True, max_iter=500)
         cl.fit(decision)
         lbls = cl.labels_
 
         mode = np.bincount(lbls).argmax()
         labels = np.ones(len(lbls))
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/comb.py` & `pythresh-0.3.3/pythresh/thresholds/comb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
 import scipy.stats as stats
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.ensemble import BaggingClassifier, StackingClassifier
 from sklearn.linear_model import RidgeClassifier
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class COMB(BaseThresholder):
     """COMB class for Combined thresholder.
 
        Use multiple thresholders as a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -45,14 +44,16 @@
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        confidence_interval_ : lower and upper confidence interval of the contamination level
+
+       dscores_ : 1D array of decomposed decision scores
     """
 
     def __init__(self, thresholders='default', max_contam=0.5, method='stacked', random_state=1234):
 
         self.thresholders = thresholders
         self.max_contam = max_contam
         func = {'mean': np.mean, 'median': np.median,
@@ -64,29 +65,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Initialize thresholders
         if self.thresholders == 'default':
             from .dsn import DSN
             from .filter import FILTER
             from .ocsvm import OCSVM
 
             self.thresholders = [DSN(random_state=self.random_state), FILTER(),
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/cpd.py` & `pythresh-0.3.3/pythresh/thresholds/cpd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import ruptures as rpt
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_cdf, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_cdf, gen_kde, normalize
 
 
 class CPD(BaseThresholder):
     r"""CPD class for Change Point Detection thresholder.
 
        Use change point detection to find a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -26,49 +25,59 @@
 
        transform : {'cdf', 'kde'}, optional (default='cdf')
             Data transformation method prior to fit
 
             - 'cdf': Use the cumulative distribution function
             - 'kde': Use the kernel density estimation
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
-       thres_ : threshold value that seperates inliers from outliers
+       thres_ : threshold value that separates inliers from outliers
+
+       dscores_ : 1D array of decomposed decision scores
 
     """
 
-    def __init__(self, method='Dynp', transform='cdf'):
+    def __init__(self, method='Dynp', transform='cdf', random_state=1234):
 
         self.method = method
         self.transform = transform
         self.method_func = {'Dynp': rpt.Dynp(), 'KernelCPD': rpt.KernelCPD(kernel='rbf'),
                             'Binseg': rpt.Binseg(), 'BottomUp': rpt.BottomUp()}
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Transform data prior to fit
         if self.transform == 'cdf':
             val_data, data_range = gen_cdf(decision, 0, 1, len(decision)*3)
         else:
             val_data, data_range = gen_kde(decision, 0, 1, len(decision)*3)
 
         # Change point detection
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/decomp.py` & `pythresh-0.3.3/pythresh/thresholds/decomp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
 from sklearn.decomposition import NMF, PCA
 from sklearn.random_projection import (
     GaussianRandomProjection,
     SparseRandomProjection
 )
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_cdf, normalize
+from .thresh_utility import check_scores, cut, gen_cdf, normalize
 
 
 class DECOMP(BaseThresholder):
     """DECOMP class for Decomposition based thresholders.
 
        Use decomposition to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -35,18 +34,20 @@
             Random seed for the decomposition algorithm. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -71,36 +72,40 @@
         self.method = method
         self.method_funcs = {'NMF': NMF(random_state=random_state),
                              'PCA': PCA(random_state=random_state),
                              'GRP': GaussianRandomProjection(n_components=2,
                                                              random_state=random_state),
                              'SRP': SparseRandomProjection(n_components=3,
                                                            random_state=random_state)}
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Generate a CDF of the decision scores
         val, dat_range = gen_cdf(decision, 0, 1, len(decision)*3)
         val = normalize(val)
 
         # Apply decomposition
         dec = self.method_funcs[str(self.method)].fit_transform(
             val.reshape(-1, 1))
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/dsn.py` & `pythresh-0.3.3/pythresh/thresholds/dsn.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import numpy as np
 import scipy.spatial.distance as distance
 import scipy.special as special
 import scipy.stats as stats
 from scipy import interpolate
 from scipy.integrate import simpson
 from sklearn.covariance import MinCovDet
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_cdf, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_cdf, gen_kde, normalize
 
 
 class DSN(BaseThresholder):
     """DSN class for Distance Shift from Normal thresholder.
 
        Use the distance shift from normal to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -46,18 +45,20 @@
             Random seed for the normal distribution. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -92,29 +93,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Create a normal distribution and normalize
         size = min(len(decision), 1500)
         norm = stats.norm.rvs(size=size, loc=0.0, scale=1.0,
                               random_state=self.random_state)
         self.norm = normalize(norm)
 
         n = 3 if self.metric != 'LP' else 1
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/eb.py` & `pythresh-0.3.3/pythresh/thresholds/eb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import numpy as np
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class EB(BaseThresholder):
     r"""EB class for Elliptical Boundary thresholder.
 
        Use pseudo-random elliptical boundaries to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond a pseudo-random elliptical boundary set
        between inliers and outliers. See :cite:`friendly2013eb` for details.
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        Pseudo-random eccentricities are used to generate elliptical boundaries
        and threshold the decision scores. This is done by using the farthest
        point on the perimeter of an ellipse from its center and is defined as:
 
@@ -41,41 +46,44 @@
        This is repeated with Monte Carlo simulations and the median number of inliers
        is selected from these thresholds. The pseudo-random eccentricity that produces
        a threshold that is closest to median sampled inlier count is applied as the
        output threshold.
 
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        pass
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Generate random set of eccentricities to test
-        r = np.random.RandomState(1234)
+        r = np.random.RandomState(self.random_state)
         rnd = r.uniform(0, 1, 5000)
 
         # Create pseudo-random elliptical boundaries using each eccentricity
         # and compute the inlier/outlier labels
         counts = []  # Get number of inliers
         for i in range(5000):
             e = rnd[i]
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/fgd.py` & `pythresh-0.3.3/pythresh/thresholds/fwfm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-import numpy as np
-from sklearn.utils import check_array
+from scipy.signal import find_peaks, peak_widths
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_kde, normalize
 
 
-class FGD(BaseThresholder):
-    """FGD class for Fixed Gradient Descent thresholder.
+class FWFM(BaseThresholder):
+    """FWFM class for Full Width at Full Minimum thresholder.
 
-       Use the fixed gradient descent to evaluate a non-parametric means
-       to threshold scores generated by the decision_scores where outliers
-       are set to any value beyond where the first derivative of the kde
-       with respect to the decision scores passes the mean of the first
-       and second inflection points. See :cite:`qi2021fgd` for details.
+       Use the full width at full minimum (aka base width) to evaluate
+       a non-parametric means to threshold scores generated by the
+       decision_scores where outliers are set to any value beyond the base
+       width. See :cite:`joneidi2013fwfm` for details.
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
-       A probability distribution of the decision scores is generated using
-       kernel density estimation. The first derivative of the pdf is
-       calculated, and the threshold is set as the middle point between the
-       first and second inflection points starting from the left side of the
-       data range.
+       The outlier detection scores are assumed to be a mixture of Gaussian
+       distributions. The probability density function of this Gaussian mixture
+       is approximated using kernel density estimation. The highest peak within the
+       PDF is used to find the base width of the mixture and the threshold is set
+       to the base width divided by the number of scores.
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        pass
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Generate KDE
-        val, dat_range = gen_kde(decision, 0, 1, len(decision)*3)
+        val, _ = gen_kde(decision, -1, 1, len(decision)*3)
+        val = normalize(val)
+
+        # Find the greatest peak of the KDE
+        peaks, _ = find_peaks(val, prominence=0.75)
+
+        # Find the base width of the peak
+        base_width = peak_widths(val, peaks, rel_height=0.99)[0]
 
-        # Calculate the first derivative of the KDE with respect
-        # to the data range
-        deriv = np.gradient(val, dat_range[1]-dat_range[0])
-
-        count = 0
-        ind = []
-
-        # Find the first two inflection points
-        for i in range(len(deriv)-1):
-
-            if (deriv[i] > 0) & (deriv[i+1] <= 0):
-                count += 1
-                ind.append(i)
-                if count == 2:
-                    break
+        # Normalize and set limit
+        limit = base_width/len(val) if len(base_width) > 0 else 1.1
 
-        limit = ((dat_range[ind[0]]+dat_range[ind[1]])/2 if
-                 len(ind) > 1 else 1.1)
         self.thresh_ = limit
 
         return cut(decision, limit)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/filter.py` & `pythresh-0.3.3/pythresh/thresholds/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from scipy import signal
 from scipy.ndimage import gaussian_filter
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class FILTER(BaseThresholder):
     """FILTER class for Filtering based thresholders.
 
        Use the filtering based methods to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -37,52 +36,62 @@
             - 'savgol':   savgol filter window size
             - 'hilbert':  number of Fourier components
             - 'medfilt:   kernel size
             - 'decimate': downsampling factor
             - 'detrend':  number of break points
             - 'resample': resampling window size
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
+
+       dscores_ : 1D array of decomposed decision scores
     """
 
-    def __init__(self, method='savgol', sigma='auto'):
+    def __init__(self, method='savgol', sigma='auto', random_state=1234):
 
         super().__init__()
         self.method = method
         self.method_funcs = {'gaussian': self._GAU_fltr, 'savgol': self._SAV_fltr,
                              'hilbert': self._HIL_fltr, 'wiener': self._WIE_fltr,
                              'medfilt': self._MED_fltr, 'decimate': self._DEC_fltr,
                              'detrend': self._DET_fltr, 'resample': self._RES_fltr}
 
         self.sigma = sigma
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Get sigma variables for various applications for each filter
         sig = (len(decision)*np.std(decision) if self.sigma == 'auto'
                else self.sigma)
 
         # Filter scores
         fltr = self.method_funcs[str(self.method)](decision, sig)
         limit = np.max(fltr)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/fwfm.py` & `pythresh-0.3.3/pythresh/thresholds/zscore.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,84 @@
-from scipy.signal import find_peaks, peak_widths
-from sklearn.utils import check_array
+import numpy as np
+import scipy.stats as stats
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, normalize
 
 
-class FWFM(BaseThresholder):
-    """FWFM class for Full Width at Full Minimum thresholder.
+class ZSCORE(BaseThresholder):
+    r"""ZSCORE class for ZSCORE thresholder.
 
-       Use the full width at full minimum (aka base width) to evaluate
-       a non-parametric means to threshold scores generated by the
-       decision_scores where outliers are set to any value beyond the base
-       width. See :cite:`joneidi2013fwfm` for details.
+       Use the zscore to evaluate a non-parametric means to threshold
+       scores generated by the decision_scores where outliers are set
+       to any value beyond a zscore of one.
+       See :cite:`bagdonavicius2020zscore` for details.
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
-       The outlier detection scores are assumed to be a mixture of Gaussian
-       distributions. The probability density function of this Gaussian mixture
-       is approximated using kernel density estimation. The highest peak within the
-       PDF is used to find the base width of the mixture and the threshold is set
-       to the base width divided by the number of scores.
+       The z-score can be calculated as follows:
+
+       .. math::
+
+           Z = \frac{x-\bar{x}}{\sigma} \mathrm{,}
+
+       where :math:`\bar{x}` and :math:`\sigma` are the mean and the
+       standard deviation of the decision scores respectively. The threshold
+       is set that any value beyond an absolute z-score of 1 is considered
+       and outlier.
+
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        super().__init__()
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
-        # Generate KDE
-        val, _ = gen_kde(decision, -1, 1, len(decision)*3)
-        val = normalize(val)
-
-        # Find the greatest peak of the KDE
-        peaks, _ = find_peaks(val, prominence=0.75)
+        self.dscores_ = decision
 
-        # Find the base width of the peak
-        base_width = peak_widths(val, peaks, rel_height=0.99)[0]
+        # Get the zscore of the decision scores
+        zscore = np.abs(stats.zscore(decision))
 
-        # Normalize and set limit
-        limit = base_width/len(val) if len(base_width) > 0 else 1.1
+        # Set the limit to where the zscore is 1
+        scores = np.zeros(len(decision), dtype=int)
+        mask = np.where(zscore >= 1.0)
+        scores[mask] = 1
 
-        self.thresh_ = limit
+        self.thresh_ = None
 
-        return cut(decision, limit)
+        return scores
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/gesd.py` & `pythresh-0.3.3/pythresh/thresholds/gesd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 # https://github.com/bhattbhavesh91/outlier-detection-grubbs-test-and-generalized-esd-test-python/blob/master/generalized-esd-test-for-outliers.ipynb
 
 
 class GESD(BaseThresholder):
     r"""GESD class for Generalized Extreme Studentized Deviate thresholder.
 
@@ -22,19 +21,25 @@
        max_outliers : int, optional (default='auto')
             maximum number of outliers that the dataset may have. Default sets
             max_outliers to be half the size of the dataset
 
        alpha : float, optional (default=0.05)
             significance level
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The generalized extreme studentized deviate is defined for the
        hypothesis:
 
        H0: There are no outliers in the decision scores
@@ -67,40 +72,44 @@
            p = 1-\frac{\alpha}{2(n-i+1)} \mathrm{.}
 
        The threshold for the decision scores is set to the smallest score that
        fulfills the condition :math:`R_i>\lambda_i`.
 
     """
 
-    def __init__(self, max_outliers='auto', alpha=0.05):
+    def __init__(self, max_outliers='auto', alpha=0.05, random_state=1234):
 
         self.max_outliers = max_outliers
         self.alpha = alpha
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         arr = decision.copy()
 
         limit = 1.1
 
         if self.max_outliers == 'auto':
             self.max_outliers = len(decision) // 2
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/hist.py` & `pythresh-0.3.3/pythresh/thresholds/hist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from scipy import ndimage as ndi
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import normalize
+from .thresh_utility import check_scores, normalize
 
 # https://github.com/scikit-image/scikit-image/blob/v0.19.2/skimage/filters/thresholding.py
 
 
 class HIST(BaseThresholder):
     """HIST class for Histogram based thresholders.
 
@@ -29,51 +28,61 @@
             - 'otsu':     OTSU's method for filtering
             - 'yen':      Yen's method for filtering
             - 'isodata':  Ridler-Calvard or inter-means method for filtering
             - 'li':       Li's iterative Minimum Cross Entropy method for filtering
             - 'minimum':  Minimum between two maxima via smoothing method for filtering
             - 'triangle': Triangle algorithm method for filtering
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
+
+       dscores_ : 1D array of decomposed decision scores
     """
 
-    def __init__(self, method='triangle', nbins='auto'):
+    def __init__(self, method='triangle', nbins='auto', random_state=1234):
 
         super().__init__()
         self.nbins = nbins
         self.method = method
         self.method_funcs = {'otsu': self._OTSU_thres, 'yen': self._YEN_thres,
                              'isodata': self._ISODATA_thres, 'li': self._LI_thres,
                              'minimum': self._Minimum_thres,
                              'triangle': self._Triangle_thres}
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         #  Set adaptive default if bins are None
         if self.nbins == 'auto':
             self.nbins = int(len(decision)**0.7)
 
         # Generate histogram
         bin_centers, counts = self._histogram(decision, self.nbins)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/iqr.py` & `pythresh-0.3.3/pythresh/thresholds/iqr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import inspect
 
 import numpy as np
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class IQR(BaseThresholder):
     r"""IQR class for Inter-Qaurtile Region thresholder.
 
        Use the inter-quartile region to evaluate a non-parametric
        means to threshold scores generated by the decision_scores
        where outliers are set to any value beyond the third quartile
        plus 1.5 times the inter-quartile region.
        See :cite:`bardet2015iqr` for details.
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The inter-quartile region is given as:
 
        .. math::
 
@@ -38,39 +43,42 @@
 
        .. math::
 
            t = Q_3 + 1.5 IQR
 
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        super().__init__()
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         arg_map = {'old': 'interpolation', 'new': 'method'}
         arg_name = (arg_map['new'] if 'method' in
                     inspect.signature(np.percentile).parameters
                     else arg_map['old'])
 
         # First quartile (Q1)
         P1 = np.percentile(decision, 25, **{arg_name: 'midpoint'})
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/karch.py` & `pythresh-0.3.3/pythresh/thresholds/karch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from geomstats.geometry.euclidean import Euclidean
 from geomstats.learning.frechet_mean import FrechetMean
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_kde, normalize
 
 
 class KARCH(BaseThresholder):
     r"""KARCH class for Riemannian Center of Mass thresholder.
 
        Use the Karcher mean (Riemannian Center of Mass) to evaluate a
        non-parametric means to threshold scores generated by the
@@ -24,61 +23,71 @@
 
        method : {'simple', 'complex'}, optional (default='complex')
             Method for computing the Karcher mean
 
             - 'simple':  Compute the Karcher mean using the 1D array of scores
             - 'complex': Compute the Karcher mean between a 2D array dot product of the scores and the sorted scores arrays
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The non-weighted Karcher mean which is also the Riemannian center of
        mass or the Riemannian geometric mean is defined to be a minimizer of:
 
        .. math::
 
            f(x) = \sum_{i=1}^n \delta^2(A,x) \mathrm{,}
 
-       where :math:`A` is a member of a special orthoganal group where the group qualities are
+       where :math:`A` is a member of a special orthogonal group where the group qualities are
        :math:`\left(X \in \mathbb{R}^{n \times n} \vert X^{\top}X=I \text{,} \mathrm{det}X=1 \right)`
        such that the group is a Lie group.
 
     """
 
-    def __init__(self, ndim=2, method='complex'):
+    def __init__(self, ndim=2, method='complex', random_state=1234):
 
         self.ndim = ndim
         self.method = method
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Create euclidean manifold and find Karcher mean
         manifold = Euclidean(dim=self.ndim)
         estimator = FrechetMean(metric=manifold.metric)
 
         if self.method == 'complex':
 
             # Create kde of scores
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/mcst.py` & `pythresh-0.3.3/pythresh/thresholds/mcst.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class MCST(BaseThresholder):
     r"""MCST class for Monte Carlo Shapiro Tests thresholder.
 
        Use uniform random sampling and statistical testing to evaluate a
        non-parametric means to threshold scores generated by the decision_scores
@@ -24,14 +23,16 @@
             Random seed for the uniform distribution. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The Shapiro-Wilk test is a frequentist statistical test for normality.
        It is used to test the null-hypothesis that the decision scores came
        from a normal distribution. This test statistic is defined as:
 
@@ -55,16 +56,16 @@
        between 0-1 are inserted into the normalized decision scores and p-values are
        calculated. if the p-value is higher than the initial p-value, the initial p-value
        is set to this value and the random value is stored. The minimum stored random
        value is set as the threshold as it is the minimum found outlier.
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -90,29 +91,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Get Baseline Shapiro-Wilk test p-value
         p_std = stats.shapiro(decision).pvalue
 
         # Create random dataset to insert and test p-values
         rnd = stats.uniform.rvs(loc=0, scale=1, size=len(
             decision), random_state=self.random_state)
         rnd = normalize(rnd)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/meta.py` & `pythresh-0.3.3/pythresh/thresholds/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 import joblib
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 from numba import njit, prange
 from sklearn.preprocessing import MinMaxScaler
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import normalize
+from .thresh_utility import check_scores, normalize
 
 
 class META(BaseThresholder):
     r"""META class for Meta-modelling thresholder.
 
        Use a trained meta-model to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -28,19 +27,25 @@
            select
 
            - 'LIN':  RidgeCV trained linear classifier meta-model on true labels
            - 'GNB':  Gaussian Naive Bayes trained classifier meta-model on true labels
            - 'GNBC': Gaussian Naive Bayes trained classifier meta-model on best contamination
            - 'GNBM': Gaussian Naive Bayes multivariate trained classifier meta-model
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        Meta-modelling is the creation of a model of models. If a dataset
        that contains only the explanatory variables (X), yet no response
        variable (y), it can still be predicted by using a meta-model. This
        is done by modelling datasets with known response variables that
@@ -55,39 +60,43 @@
        vowels, Waveform,  WBC, WDBC, Wilt, wine, WPBC, yeast`` available at
        `ADBench dataset <https://github.com/Minqi824/ADBench/tree/main/datasets/Classical>`_.
        META uses a majority vote of all the trained models to determine the
        inlier/outlier labels.
 
     """
 
-    def __init__(self, method='GNBM'):
+    def __init__(self, method='GNBM', random_state=1234):
 
         self.method = method
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         if self.method == 'LIN':
             clf = 'meta_model_LIN.pkl'
         elif self.method == 'GNB':
             clf = 'meta_model_GNB.pkl'
         elif self.method == 'GNBC':
             clf = 'meta_model_GNBC.pkl'
         else:
@@ -110,15 +119,15 @@
             qmcd = normalize(qmcd)
             if len(qmcd[qmcd > 0.5]) > 0.5*len(qmcd):
                 qmcd = 1 - qmcd
 
             kde = stats.gaussian_kde(decision)
             pdf = normalize(kde.pdf(decision))
 
-        for i in range(380):
+        for i in range(len(model.groups_)):
 
             df = pd.DataFrame()
             df['scores'] = decision
             df['groups'] = i
 
             if self.method == 'GNBM':
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/moll.py` & `pythresh-0.3.3/pythresh/thresholds/moll.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import scipy.signal as signal
 from scipy import integrate
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 # https://github.com/geomdata/gda-public/blob/master/timeseries/curve_geometry.pyx
 
 
 class MOLL(BaseThresholder):
     r"""MOLL class for Friedrichs' mollifier thresholder.
 
@@ -21,14 +20,16 @@
        ----------
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        Friedrichs' mollifier is a smoothing function that is applied to create sequences
        of smooth functions. These functions can be used to approximate generalized functions
        that may be non-smooth. The decision scores are assumed to be a part of a generalized
        function with a non-smooth nature in terms of the interval space between the scores
@@ -51,37 +52,44 @@
 
        The mollifier is inserted into a discrete convolution operator and the smoothed
        scores are returned. The threshold is set at one minus the maximum of the smoothed
        scores.
 
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        pass
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
+        decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
+                   which are the decision scores from a
+                   outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
-        dat_range = np.linspace(0, 1, len(decision))
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
+        dat_range = np.linspace(0, 1, len(decision))
+
         # Set the inliers to be where the 1-max(smoothed scores)
         limit = 1-np.max(self._mollifier(dat_range, np.sort(decision)))
 
         self.thresh_ = limit
 
         return cut(decision, limit)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/mtt.py` & `pythresh-0.3.3/pythresh/thresholds/mtt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 # https://github.com/vvaezian/modified_thompson_tau_test/blob/main/src/Modified_Thompson_Tau_Test/modified_thompson_tau_test.py
 
 
 class MTT(BaseThresholder):
     r"""MTT class for Modified Thompson Tau test thresholder.
 
@@ -15,22 +14,28 @@
        to threshold scores generated by the decision_scores where outliers
        are set to any value beyond the smallest outlier detected by the test.
        See :cite:`rengasamy2020mtt` for details.
 
        Parameters
        ----------
 
-       self.alpha : float, optional (default=0.99)
+       alpha : float, optional (default=0.99)
             Confidence level corresponding to the t-Student distribution map to sample
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The Modified Thompson Tau test is a modified univariate t-test that eliminates outliers
        that are more than a number of standard deviations away from the mean. This method is
        done iteratively with the Tau critical value being recalculated after each outlier removal
        until the dataset no longer has data points that fall outside of the criterion. The Tau
@@ -40,39 +45,43 @@
 
            \tau = \frac{t \cdot (n-1)}{\sqrt{n}\sqrt{n-2+t^2}}  \mathrm{,}
 
        where :math:`n` is the number of data points and :math:`t` is the student t-value
 
     """
 
-    def __init__(self, alpha=0.99):
+    def __init__(self, alpha=0.99, random_state=1234):
 
         self.alpha = alpha
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         arr = np.sort(decision.copy())
 
         limit = 1.1
 
         while True:
 
             # Calculate the rejection threshold
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/ocsvm.py` & `pythresh-0.3.3/pythresh/thresholds/ocsvm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import scipy.stats as stats
 from sklearn.kernel_approximation import AdditiveChi2Sampler
 from sklearn.linear_model import RidgeCV, SGDOneClassSVM
 from sklearn.metrics import mean_squared_error
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.svm import OneClassSVM
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import gen_kde, normalize
+from .thresh_utility import check_scores, gen_kde, normalize
 
 
 class OCSVM(BaseThresholder):
     """OCSVM class for One-Class Support Vector Machine thresholder.
 
        Use a one-class svm to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -59,16 +58,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -101,28 +100,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
+
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Get auto nu calculation
         if self.nu == 'auto':
 
             np.seterr(divide='ignore')
             gmean = stats.gmean(decision)
             mean = np.mean(decision)
             med = np.median(decision)
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/qmcd.py` & `pythresh-0.3.3/pythresh/thresholds/qmcd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class QMCD(BaseThresholder):
     """QMCD class for Quasi-Monte Carlo Discrepancy thresholder.
 
        Use the quasi-Monte Carlo discrepancy to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -29,19 +28,25 @@
 
        lim : {'Q', 'P'}, optional (default='P')
             Filtering method to threshold scores using 1 - discrepancy
 
             - 'Q': Use quantile limiting
             - 'P': Use percentile limiting
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        For the QMCD method it is assumed that the decision scores are pseudo-random
        values within a distribution :math:`M`. "Quasi-random" sequences, which are
        numbers that are better equidistributed for :math:`M` than pseudo-random numbers
        are used to calculate the decision scores discrepancy value.
@@ -55,41 +60,45 @@
        The QMCD method utilizes the discrepancy value by assuming that when it is at its lowest
        value (0) the "quasi-random" generated sequences and the decision scores are equally
        equidistributed across :math:`M`. Outliers are assumed to solely raise the discrepancy
        value. And therefore, the contamination of the dataset can be set as one minus the
        discrepancy.
     """
 
-    def __init__(self, method='WD', lim='P'):
+    def __init__(self, method='WD', lim='P', random_state=1234):
 
         super().__init__()
         self.method = method
         self.lim = lim
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Get the quasi Monte-Carlo discrepancy of the labels
         disc = stats.qmc.discrepancy(
             decision.reshape(-1, 1), method=self.method)
 
         # Set the limit to either the quantile or percentile of 1-discrepancy
         if self.lim == 'Q':
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/regr.py` & `pythresh-0.3.3/pythresh/thresholds/regr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class REGR(BaseThresholder):
     """REGR class for Regression based thresholder.
 
        Use the regression to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -29,16 +28,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -66,29 +65,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Create a normal distribution and normalize
         norm = np.random.default_rng(self.random_state).normal(
             loc=0.0, scale=1.0, size=decision.shape)
         norm = normalize(norm)
 
         # Set limit to the y-intercept
         try:
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/thresh_utility.py` & `pythresh-0.3.3/pythresh/thresholds/thresh_utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import numpy as np
 import scipy.stats as stats
 from scipy.special import ndtr
+from sklearn.decomposition import TruncatedSVD
+from sklearn.utils import check_array
 
 
 def normalize(data):
 
-    return ((data - data.min()) / (data.max() - data.min()))
+    return ((data - data.min(axis=0)) /
+            (data.max(axis=0) - data.min(axis=0)))
 
 
 def cut(decision, limit):
 
     labels = np.zeros(len(decision), dtype=int)
 
     labels[decision >= limit] = 1
@@ -31,7 +34,32 @@
     # Create a KDE & CDF of the data
     kde = stats.gaussian_kde(data)
     dat_range = np.linspace(lower, upper, size)
     cdf = np.array(tuple(ndtr(np.ravel(item - kde.dataset) / kde.factor).mean()
                          for item in dat_range))
 
     return cdf, dat_range
+
+
+def check_scores(decision, random_state=None):
+
+    # Check decision scores dimensionality and pre-process
+    if (np.asarray(decision).ndim == 2) & (np.atleast_2d(decision).shape[1] > 1):
+
+        decision = check_array(decision, ensure_2d=True)
+        decision = decompose(decision).squeeze()
+
+    else:
+
+        decision = check_array(decision, ensure_2d=False).squeeze()
+
+    return decision
+
+
+def decompose(data, random_state=None):
+
+    # Decompose decision scores to 1D array for thresholding
+    decomp = TruncatedSVD(n_components=1, random_state=random_state)
+
+    data = decomp.fit_transform(normalize(data))
+
+    return data
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/vae.py` & `pythresh-0.3.3/pythresh/thresholds/vae.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 import scipy.stats as stats
 import torch
 import torch.optim as opt
-from sklearn.utils import check_array
 from torch import nn
 from torch.distributions import Normal, kl_divergence
 from torch.nn.functional import softplus
 from tqdm import tqdm
 
 from .base import BaseThresholder
-from .thresh_utility import cut, normalize
+from .thresh_utility import check_scores, cut, normalize
 
 
 class VAE(BaseThresholder):
     r"""VAE class for Variational AutoEncoder thresholder.
 
        Use a VAE to evaluate a non-parametric means
        to threshold scores generated by the decision_scores where outliers
@@ -53,16 +52,16 @@
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -98,28 +97,32 @@
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
+
         scores = normalize(decision.copy())
 
+        self.dscores_ = scores
+
         if self.latent_dims == 'auto':
             self.latent_dims = self._autodim(scores)
 
         decision = normalize(decision).astype(np.float32).reshape(-1, 1)
 
         self.model = VAE_model(1, self.latent_dims,
                                self.random_state, self.dist,
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/wind.py` & `pythresh-0.3.3/pythresh/thresholds/wind.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from scipy import integrate, stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_kde, normalize
 
 
 class WIND(BaseThresholder):
     r"""WIND class for topological Winding number thresholder.
 
        Use the topological winding number (with respect to the origin) to
        evaluate a non-parametric means to threshold scores generated by
@@ -22,14 +21,16 @@
             Random seed for the normal distribution. Can also be set to None.
 
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The topological winding number or the degree of a continuous mapping. It is an
        integer sum of the number of completed/closed counterclockwise rotations in a plane
        around a point. And is given by,
 
@@ -47,16 +48,16 @@
        distribution of the dataset or shift from inliers to outliers relating to these intersections.
        With this, it is assumed that if an intersection exists, then adjacent/incident regions
        must have different region labels. Since multiple intersection regions may exist. The
        threshold between inliers and outliers is taken as the mean intersection point.
 
        Examples
        --------
-       The effects of randomness can affect the thresholder's output perfomance
-       signicantly. Therefore, to alleviate the effects of randomness on the
+       The effects of randomness can affect the thresholder's output performance
+       significantly. Therefore, to alleviate the effects of randomness on the
        thresholder a combined model can be used with different random_state values.
        E.g.
 
        .. code:: python
 
             # train the KNN detector
             from pyod.models.knn import KNN
@@ -82,27 +83,33 @@
         self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
+        decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
+                   which are the decision scores from a
+                   outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Create a normal distribution and normalize
         size = min(len(decision), 1500)
         norm = stats.norm.rvs(size=size, loc=0.0, scale=1.0,
                               random_state=self.random_state)
         norm = normalize(norm)
 
         # Create a KDE of the labels and the normal distribution
```

### Comparing `pythresh-0.3.2/pythresh/thresholds/yj.py` & `pythresh-0.3.3/pythresh/thresholds/yj.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import numpy as np
 import scipy.stats as stats
-from sklearn.utils import check_array
 
 from .base import BaseThresholder
-from .thresh_utility import cut, gen_kde, normalize
+from .thresh_utility import check_scores, cut, gen_kde, normalize
 
 
 class YJ(BaseThresholder):
     r"""YJ class for Yeo-Johnson transformation thresholder.
 
        Use the Yeo-Johnson transformation to evaluate
        a non-parametric means to threshold scores generated by the
        decision_scores where outliers are set to any value beyond the
        max value in the YJ transformed data.
        See :cite:`raymaekers2021yj` for details.
 
        Parameters
        ----------
 
+       random_state : int, optional (default=1234)
+            Random seed for the random number generators of the thresholders. Can also
+            be set to None.
+
        Attributes
        ----------
 
        thresh_ : threshold value that separates inliers from outliers
 
+       dscores_ : 1D array of decomposed decision scores
+
        Notes
        -----
 
        The Yeo-Johnson transformation is a power transform which is a
        set of power functions that apply a monotonic transformation to
        the dataset. For the decision scores this make their distribution
        more normal-like. The transformation is given by:
@@ -46,39 +51,42 @@
        scores that are beyond maximum value after this transformation are
        considered outliers. However, the closer a set of decision scores are
        to a normal distribution originally the smaller the probability this
        threshold will be able to identify outliers.
 
     """
 
-    def __init__(self):
+    def __init__(self, random_state=1234):
 
-        super().__init__()
+        self.random_state = random_state
 
     def eval(self, decision):
         """Outlier/inlier evaluation process for decision scores.
 
         Parameters
         ----------
         decision : np.array or list of shape (n_samples)
+                   or np.array of shape (n_samples, n_detectors)
                    which are the decision scores from a
                    outlier detection.
 
         Returns
         -------
         outlier_labels : numpy array of shape (n_samples,)
             For each observation, tells whether or not
             it should be considered as an outlier according to the
             fitted model. 0 stands for inliers and 1 for outliers.
         """
 
-        decision = check_array(decision, ensure_2d=False)
+        decision = check_scores(decision, random_state=self.random_state)
 
         decision = normalize(decision)
 
+        self.dscores_ = decision
+
         # Generate KDE
         val, _ = gen_kde(decision, 0, 1, len(decision)*3)
 
         # Use Yeo-Johnson transformation to reshape distribution
         # iterate to get average transformation
         mean_s = np.zeros(len(val))
         for _ in range(50):
```

### Comparing `pythresh-0.3.2/pythresh.egg-info/PKG-INFO` & `pythresh-0.3.3/pythresh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythresh
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python Toolbox for Outlier Detection Thresholding
 Home-page: https://github.com/KulikDM/pythresh
 Download-URL: https://github.com/KulikDM/pythresh/archive/master.zip
 Author: D Kulik
 Project-URL: Documentation, https://pythresh.readthedocs.io/en/latest/
 Keywords: outlier detection,anomaly detection,thresholding,cutoff,contamintion level,data science,machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,27 +71,28 @@
 .. image:: https://zenodo.org/badge/497683169.svg
    :target: https://zenodo.org/badge/latestdoi/497683169
    :alt: Zenodo DOI
 
 ----
 
 PyThresh is a comprehensive and scalable **Python toolkit** for
-**thresholding outlier detection scores** in univariate/multivariate
-data. It has been writen to work in tandem with PyOD and has similar
-syntax and data structures. However, it is not limited to this single
-library. PyThresh is meant to threshold scores generated by an outlier
-detection. It thresholds scores without the need to set a contamination
-level or have the user guess the amount of outliers that may exist in
-the dataset beforehand. These non-parametric methods were written to
-reduce the user's input/guess work and rather rely on statistics instead
-to threshold outlier scores. For thresholding to be applied correctly,
-the outlier detection scores must follow this rule: the higher the
-score, the higher the probability that it is an outlier in the dataset.
-All threshold functions return a binary array where inliers and outliers
-are represented by a 0 and 1 respectively.
+**thresholding outlier detection likelihood scores** in
+univariate/multivariate data. It has been written to work in tandem with
+PyOD and has similar syntax and data structures. However, it is not
+limited to this single library. PyThresh is meant to threshold
+likelihood scores generated by an outlier detector. It thresholds these
+likelihood scores and replaces the need to set a contamination level or
+have the user guess the amount of outliers that may exist in the dataset
+beforehand. These non-parametric methods were written to reduce the
+user's input/guess work and rather rely on statistics instead to
+threshold outlier likelihood scores. For thresholding to be applied
+correctly, the outlier detection likelihood scores must follow this
+rule: the higher the score, the higher the probability that it is an
+outlier in the dataset. All threshold functions return a binary array
+where inliers and outliers are represented by a 0 and 1 respectively.
 
 PyThresh includes more than 30 thresholding algorithms. These algorithms
 range from using simple statistical analysis like the Z-score to more
 complex mathematical methods that involve graph theory and topology.
 
 ************************
  Documentation & Citing
@@ -121,14 +122,35 @@
    # get outlier scores
    decision_scores = clf.decision_scores_  # raw outlier scores on the train data
 
    # get outlier labels
    thres = FILTER()
    labels = thres.eval(decision_scores)
 
+or using multiple outlier detection score sets
+
+.. code:: python
+
+   # train multiple detectors
+   from pyod.models.knn import KNN
+   from pyod.models.pca import PCA
+   from pyod.models.iforest import IForest
+   from pythresh.thresholds.filter import FILTER
+
+   clfs = [KNN(), IForest(), PCA()]
+
+   # get outlier scores for each detector
+   scores = [clf.fit(X_train).decision_scores_ for clf in clfs]
+
+   scores = np.vstack(scores).T
+
+   # get outlier labels
+   thres = FILTER()
+   labels = thres.eval(scores)
+
 **************
  Installation
 **************
 
 It is recommended to use **pip** or **conda** for installation:
 
 .. code:: bash
@@ -174,41 +196,45 @@
 -  torch (used in the VAE thresholder)
 -  tqdm (used in the VAE thresholder)
 
 ****************
  API Cheatsheet
 ****************
 
--  **eval(score)**: evaluate outlier score.
+-  **eval(score)**: evaluate a single outlier or multiple outlier
+   detection likelihood score sets.
 
 Key Attributes of threshold:
 
 -  **thresh_**: Return the threshold value that separates inliers from
    outliers. Outliers are considered all values above this threshold
-   value. Note the threshold value has been derived from normalized
-   scores.
+   value. Note the threshold value has been derived from likelihood
+   scores normalized between 0 and 1.
 
 -  **confidence_interval_**: Return the lower and upper confidence
    interval of the contamination level. Only applies to the COMB
    thresholder
 
+-  **dscores_**: 1D array of the TruncatedSVD decomposed decision scores
+   if multiple outlier detector score sets are passed
+
 ************************
  External Feature Cases
 ************************
 
 **Towards Data Science**: `Thresholding Outlier Detection Scores with
 PyThresh
 <https://towardsdatascience.com/thresholding-outlier-detection-scores-with-pythresh-f26299d14fa>`_
 
 **Towards Data Science**: `When Outliers are Significant: Weighted
 Linear Regression
 <https://towardsdatascience.com/when-outliers-are-significant-weighted-linear-regression-bcdc8389ab10>`_
 
 **ArXiv**: `Estimating the Contamination Factor's Distribution in
-Unsupervised Anomaly Detection <https://arxiv.org/abs/2210.10487>`_
+Unsupervised Anomaly Detection. <https://arxiv.org/abs/2210.10487>`_
 
 ***********************************
  Available Thresholding Algorithms
 ***********************************
 
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | Abbr      | Description                               | References         | Documentation                                                                                                                                          |
@@ -233,14 +259,16 @@
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FGD       | Fixed Gradient Descent                    | [#fgd1]_           | `pythresh.thresholds.fgd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fgd>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FILTER    | Filtering Based                           | [#filter1]_        | `pythresh.thresholds.filter module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.filter>`_            |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | FWFM      | Full Width at Full Minimum                | [#fwfm1]_          | `pythresh.thresholds.fwfm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.fwfm>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
+| GAMGMM    | Bayesian Gamma GMM                        | [#gamgmm1]_        | `pythresh.thresholds.gamgmm module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gamgmm>`_            |
++-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | GESD      | Generalized Extreme Studentized Deviate   | [#gesd1]_          | `pythresh.thresholds.gesd module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.gesd>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | HIST      | Histogram Based                           | [#hist1]_          | `pythresh.thresholds.hist module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.hist>`_                |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | IQR       | Inter-Quartile Region                     | [#iqr1]_           | `pythresh.thresholds.iqr module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.iqr>`_                  |
 +-----------+-------------------------------------------+--------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------+
 | KARCH     | Karcher mean (Riemannian Center of Mass)  | [#karch1]_         | `pythresh.thresholds.karch module <https://pythresh.readthedocs.io/en/latest/pythresh.thresholds.html#module-pythresh.thresholds.karch>`_              |
@@ -401,14 +429,19 @@
    <https://ieeexplore.ieee.org/document/9029258/>`_
 
 .. [#fwfm1]
 
    `Sparse Auto-Regressive: Robust Estimation of AR Parameters
    <https://arxiv.org/abs/1306.3317>`_
 
+.. [#gamgmm1]
+
+   `Estimating the Contamination Factor's Distribution in Unsupervised
+   Anomaly Detection <https://proceedings.mlr.press/v202/perini23a.html>`_
+
 .. [#gesd1]
 
    `An adjusted Grubbs' and generalized extreme studentized deviation
    <https://www.degruyter.com/document/doi/10.1515/dema-2021-0041/html?lang=en>`_
 
 .. [#hist1]
```

### Comparing `pythresh-0.3.2/pythresh.egg-info/SOURCES.txt` & `pythresh-0.3.3/pythresh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 pythresh/thresholds/cpd.py
 pythresh/thresholds/decomp.py
 pythresh/thresholds/dsn.py
 pythresh/thresholds/eb.py
 pythresh/thresholds/fgd.py
 pythresh/thresholds/filter.py
 pythresh/thresholds/fwfm.py
+pythresh/thresholds/gamgmm.py
 pythresh/thresholds/gesd.py
 pythresh/thresholds/hist.py
 pythresh/thresholds/iqr.py
 pythresh/thresholds/karch.py
 pythresh/thresholds/mad.py
 pythresh/thresholds/mcst.py
 pythresh/thresholds/meta.py
```

### Comparing `pythresh-0.3.2/setup.py` & `pythresh-0.3.3/setup.py`

 * *Files identical despite different names*

