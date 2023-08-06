# Comparing `tmp/prda-1.1.0.tar.gz` & `tmp/prda-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prda-1.1.0.tar", last modified: Fri Jul  7 06:45:47 2023, max compression
+gzip compressed data, was "prda-1.1.2.tar", last modified: Sun Aug  6 08:41:09 2023, max compression
```

## Comparing `prda-1.1.0.tar` & `prda-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.235671 prda-1.1.0/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.1.0/LICENSE
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-07-07 06:45:47.235510 prda-1.1.0/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)     2713 2023-06-30 05:36:38.000000 prda-1.1.0/README.md
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.234207 prda-1.1.0/prda/
--rw-r--r--   0 minshaojie   (501) staff       (20)      107 2023-07-07 03:33:54.000000 prda-1.1.0/prda/__init__.py
--rw-r--r--   0 minshaojie   (501) staff       (20)    12932 2023-05-16 06:36:16.000000 prda-1.1.0/prda/graphic.py
--rw-r--r--   0 minshaojie   (501) staff       (20)      856 2023-05-05 07:16:05.000000 prda-1.1.0/prda/iostream.py
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.235299 prda-1.1.0/prda/ml/
--rw-r--r--   0 minshaojie   (501) staff       (20)       61 2023-07-07 03:02:46.000000 prda-1.1.0/prda/ml/__init__.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     3460 2023-07-07 03:02:12.000000 prda-1.1.0/prda/ml/clusters.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     5470 2023-07-07 03:09:34.000000 prda-1.1.0/prda/ml/evaluations.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     5506 2023-07-07 04:11:25.000000 prda-1.1.0/prda/ml/neighbors.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     8809 2023-07-07 03:12:15.000000 prda-1.1.0/prda/prep.py
--rw-r--r--   0 minshaojie   (501) staff       (20)     3389 2022-12-03 12:39:17.000000 prda-1.1.0/prda/utility.py
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-07-07 06:45:47.234796 prda-1.1.0/prda.egg-info/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)      328 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/SOURCES.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/dependency_links.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/requires.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        5 2023-07-07 06:45:47.000000 prda-1.1.0/prda.egg-info/top_level.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-07-07 06:45:47.235719 prda-1.1.0/setup.cfg
--rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-07-07 06:45:43.000000 prda-1.1.0/setup.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-08-06 08:41:09.242045 prda-1.1.2/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.1.2/LICENSE
+-rw-r--r--   0 minshaojie   (501) staff       (20)     4752 2023-08-06 08:41:09.241872 prda-1.1.2/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)     2901 2023-08-06 08:22:47.000000 prda-1.1.2/README.md
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-08-06 08:41:09.239500 prda-1.1.2/prda/
+-rw-r--r--   0 minshaojie   (501) staff       (20)      105 2023-08-06 08:11:40.000000 prda-1.1.2/prda/__init__.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)    12932 2023-08-06 08:12:30.000000 prda-1.1.2/prda/graphic.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)      856 2023-05-05 07:16:05.000000 prda-1.1.2/prda/iostream.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-08-06 08:41:09.241496 prda-1.1.2/prda/ml/
+-rw-r--r--   0 minshaojie   (501) staff       (20)       61 2023-07-07 03:02:46.000000 prda-1.1.2/prda/ml/__init__.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     3460 2023-07-07 03:02:12.000000 prda-1.1.2/prda/ml/clusters.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     5470 2023-07-07 06:50:17.000000 prda-1.1.2/prda/ml/evaluations.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     5506 2023-07-07 04:11:25.000000 prda-1.1.2/prda/ml/neighbors.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     8811 2023-07-07 07:58:41.000000 prda-1.1.2/prda/prep.py
+-rw-r--r--   0 minshaojie   (501) staff       (20)     4193 2023-08-06 08:11:29.000000 prda-1.1.2/prda/stats.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-08-06 08:41:09.240371 prda-1.1.2/prda.egg-info/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     4752 2023-08-06 08:41:09.000000 prda-1.1.2/prda.egg-info/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)      326 2023-08-06 08:41:09.000000 prda-1.1.2/prda.egg-info/SOURCES.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-08-06 08:41:09.000000 prda-1.1.2/prda.egg-info/dependency_links.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-08-06 08:41:09.000000 prda-1.1.2/prda.egg-info/requires.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        5 2023-08-06 08:41:09.000000 prda-1.1.2/prda.egg-info/top_level.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-08-06 08:41:09.242098 prda-1.1.2/setup.cfg
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1199 2023-08-06 08:40:12.000000 prda-1.1.2/setup.py
```

### Comparing `prda-1.1.0/LICENSE` & `prda-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/README.md` & `prda-1.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,17 +30,23 @@
 import numpy as np
 df = pd.DataFrame(data=np.array([np.arange(100) for i in range(5)]).T,columns=['a', 'b', 'c', 'd', 'e'])
 prda.graphic.scatter_3d_html(df, x='a', y='b', z='c', color_hue='d', size_hue='e', title='demo_3d_scatter', filepath='demo_3d_scatter.html')
 ```
 
 the above code will provide an interactive html figure that look like this:
 
-![Image.png](/demo/demo_3d_scatter_screenshot.png)
 
-[demo_3d_scatter.html](/demo/demo_3d_scatter.html)
+
+<iframe src="demo/demo_lineplot.html" width="500" height="300"></iframe>
+
+
+
+<!-- ![Image.png](/demo/demo_3d_scatter_screenshot.png) -->
+
+<!-- [demo_3d_scatter.html](/demo/demo_3d_scatter.html) -->
 
 ----
 
 ```python
 import prda
 import pandas as pd
 import numpy as np
@@ -65,17 +71,19 @@
 |  2  |  2.0  | 0.04 | 4.0 |
 | ... |  ...  |  ... |  ... |
 | 498 | 498.0 | 9.96 | 6.0 |
 | 499 | 499.0 | 9.98 | 5.0 |
 
 And code with the above DataFrame will draw anther plot look like this:
 
-![lineplot_screenshot.png](demo/demo_lineplot_screenshot.png)
+<iframe src="demo/demo_lineplot.html" width="500" height="300"></iframe>
+
+<!-- ![lineplot_screenshot.png](demo/demo_lineplot_screenshot.png) -->
 
-[demo_lineplot.html](/demo/demo_lineplot.html)
+<!-- [demo_lineplot.html](/demo/demo_lineplot.html) -->
 
 Although the current *prda* is far from completion, let along perfection. It is under improvement regularly.
 
 ----
 ## Updates
 ### 2023.5.3 Major Updates
 Add several easy-to-use functions, including `prep::`pca, select_continuous_variables, handle_missing_data, apply_linear_func(row-wisely), and `ml::`match_clusters, evaluate_param_combinations(optimal parameters searching, with base class::sklearn.base.BaseEstimator), etc.
```

### Comparing `prda-1.1.0/prda/graphic.py` & `prda-1.1.2/prda/graphic.py`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/prda/iostream.py` & `prda-1.1.2/prda/iostream.py`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/prda/ml/clusters.py` & `prda-1.1.2/prda/ml/clusters.py`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/prda/ml/evaluations.py` & `prda-1.1.2/prda/ml/evaluations.py`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/prda/ml/neighbors.py` & `prda-1.1.2/prda/ml/neighbors.py`

 * *Files identical despite different names*

### Comparing `prda-1.1.0/prda/prep.py` & `prda-1.1.2/prda/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from sklearn import preprocessing
 import pandas as pd
 import numpy as np
 
 __all__ = ['normalization', 'convert_df', 'drop_first_n', 'pca', 'handle_missing_data', 'select_continuous_variables', 'apply_linear_func']
         
-def normalization(data: np.ndarray, min_: float = 0, max_: float = 1.0, bias: float = 0.1)-> np.ndarray:
+def normalization(data: np.ndarray, min_: float = 0, max_: float = 1.0, bias: float = 0)-> np.ndarray:
     """
     Scaling data to lie between a given minimum and maximum value (MinMaxScaler).
 
     [Note] that this is a `feature-wise` scaler, rather than sample-wise which is the case in Sci-kit Learn
 
     Considering all datas `as one dataset`.
 
@@ -19,15 +19,15 @@
 
         X_std = (X - X.min) / (X.max - X.min)
         X_scaled = X_std * (max_ - min_) + min_
 
     Parameters
     ----------
     data : numpy.ndarray
-    ndarray as original shape
+        ndarray as original shape
     """
     data = np.asarray(data)
     datalen = 1
     for i in data.shape:
         if i != 0:
             datalen = datalen * i
     scaler = preprocessing.MinMaxScaler(feature_range=(min_, max_))
```

### Comparing `prda-1.1.0/prda/utility.py` & `prda-1.1.2/prda/stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-""" The :mod:`prda.utility` contains ``what you might use`` when handling your data.
+""" The :mod:`prda.stats` contains ``what you might use`` when handling your data.
 """
 
 import random
 import numpy as np
 import pandas as pd
 from scipy.stats import anderson, kstest
+from sklearn.neighbors import KernelDensity
 
 __all__ = ['nlargest_dict', 'get_distribution', 'classify_indices', 'gussian_test', 'choice_weighted', 'classify_indices']
 
 def nlargest_dict(dict_: dict, n: int)-> list:
     """This function returns `n` largest elements from `dict_`
 
     Parameters
@@ -113,7 +114,39 @@
                     distribution[keys[i-1]] += 1
                     break
     else:
         raise KeyError('Sorry, data type: ', popul_type, 'not supported right now.')
     return distribution
 
 
+def compute_probabilities(X, h=0.5):
+    """_summary_
+
+    Parameters
+    ----------
+    X : _type_
+        _description_
+    h : float, optional
+        bandwidth of Gaussian kernel, by default 0.5
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+    if X.ndim == 1:
+        X = X.reshape(-1, 1)
+    
+    # Create a Kernel Density Estimator
+    kde = KernelDensity(kernel='gaussian', bandwidth=h)
+
+    # Fit the KDE model to the data
+    kde.fit(X)
+
+    # Evaluate the KDE model on the data points
+    log_probabilities = kde.score_samples(X)
+
+    # Convert log probabilities to probabilities
+    probabilities = np.exp(log_probabilities)
+    normalized_probabilities = probabilities / np.sum(probabilities)
+
+    return normalized_probabilities
```

