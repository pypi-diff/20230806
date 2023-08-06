# Comparing `tmp/marginaleffects-0.0.3.tar.gz` & `tmp/marginaleffects-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marginaleffects-0.0.3.tar", max compression
+gzip compressed data, was "marginaleffects-0.0.4.tar", max compression
```

## Comparing `marginaleffects-0.0.3.tar` & `marginaleffects-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-06-23 12:22:21.334170 marginaleffects-0.0.3/LICENSE
--rw-r--r--   0        0        0    23288 2023-07-24 22:11:24.850825 marginaleffects-0.0.3/README.md
--rw-r--r--   0        0        0      213 2023-07-03 23:36:04.163006 marginaleffects-0.0.3/marginaleffects/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-01 14:37:00.809371 marginaleffects-0.0.3/marginaleffects/by.py
--rw-r--r--   0        0        0     1958 2023-07-24 01:30:03.435871 marginaleffects-0.0.3/marginaleffects/classes.py
--rw-r--r--   0        0        0    12629 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/comparisons.py
--rw-r--r--   0        0        0     1293 2023-07-03 23:29:26.413040 marginaleffects-0.0.3/marginaleffects/datagrid.py
--rw-r--r--   0        0        0     1573 2023-07-22 00:54:29.376618 marginaleffects-0.0.3/marginaleffects/equivalence.py
--rw-r--r--   0        0        0     3159 2023-07-01 12:13:24.451354 marginaleffects-0.0.3/marginaleffects/estimands.py
--rw-r--r--   0        0        0      803 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/hypotheses.py
--rw-r--r--   0        0        0     6910 2023-07-03 23:29:26.413040 marginaleffects-0.0.3/marginaleffects/hypothesis.py
--rw-r--r--   0        0        0     4870 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/predictions.py
--rw-r--r--   0        0        0    13777 2023-07-23 15:35:08.210252 marginaleffects-0.0.3/marginaleffects/sanity.py
--rw-r--r--   0        0        0     1361 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/slopes.py
--rw-r--r--   0        0        0      399 2023-07-03 23:29:26.423040 marginaleffects-0.0.3/marginaleffects/transform.py
--rw-r--r--   0        0        0     2287 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/uncertainty.py
--rw-r--r--   0        0        0     2926 2023-07-22 00:54:29.376618 marginaleffects-0.0.3/marginaleffects/utils.py
--rw-r--r--   0        0        0      771 2023-07-24 22:11:12.810825 marginaleffects-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    23943 1970-01-01 00:00:00.000000 marginaleffects-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 12:35:22.380022 marginaleffects-0.0.4/LICENSE
+-rw-r--r--   0        0        0    23288 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/README.md
+-rw-r--r--   0        0        0      225 2023-07-25 21:40:13.691981 marginaleffects-0.0.4/marginaleffects/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-02 17:04:59.766245 marginaleffects-0.0.4/marginaleffects/by.py
+-rw-r--r--   0        0        0     1958 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/marginaleffects/classes.py
+-rw-r--r--   0        0        0    12629 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/marginaleffects/comparisons.py
+-rw-r--r--   0        0        0     5097 2023-07-25 21:42:37.931948 marginaleffects-0.0.4/marginaleffects/datagrid.py
+-rw-r--r--   0        0        0     1573 2023-07-17 21:14:19.192874 marginaleffects-0.0.4/marginaleffects/equivalence.py
+-rw-r--r--   0        0        0     3159 2023-07-02 17:04:59.766245 marginaleffects-0.0.4/marginaleffects/estimands.py
+-rw-r--r--   0        0        0      912 2023-08-02 13:56:14.866878 marginaleffects-0.0.4/marginaleffects/hypotheses.py
+-rw-r--r--   0        0        0     6904 2023-08-02 13:56:14.866878 marginaleffects-0.0.4/marginaleffects/hypothesis.py
+-rw-r--r--   0        0        0     5562 2023-08-06 18:45:51.594091 marginaleffects-0.0.4/marginaleffects/predictions.py
+-rw-r--r--   0        0        0    13777 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/marginaleffects/sanity.py
+-rw-r--r--   0        0        0     1361 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/marginaleffects/slopes.py
+-rw-r--r--   0        0        0      399 2023-07-03 19:04:37.399801 marginaleffects-0.0.4/marginaleffects/transform.py
+-rw-r--r--   0        0        0     2287 2023-07-25 21:40:11.021982 marginaleffects-0.0.4/marginaleffects/uncertainty.py
+-rw-r--r--   0        0        0     3039 2023-08-06 18:31:12.034273 marginaleffects-0.0.4/marginaleffects/utils.py
+-rw-r--r--   0        0        0      789 2023-08-06 18:47:48.134071 marginaleffects-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    23943 1970-01-01 00:00:00.000000 marginaleffects-0.0.4/PKG-INFO
```

### Comparing `marginaleffects-0.0.3/LICENSE` & `marginaleffects-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/README.md` & `marginaleffects-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/by.py` & `marginaleffects-0.0.4/marginaleffects/by.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/classes.py` & `marginaleffects-0.0.4/marginaleffects/classes.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/comparisons.py` & `marginaleffects-0.0.4/marginaleffects/comparisons.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/equivalence.py` & `marginaleffects-0.0.4/marginaleffects/equivalence.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/estimands.py` & `marginaleffects-0.0.4/marginaleffects/estimands.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/hypothesis.py` & `marginaleffects-0.0.4/marginaleffects/hypothesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         for i in range(x.shape[0]):
             tmp = f"marginaleffects__{i + 1}"
             hypothesis = re.sub(f"b{i + 1}", tmp, hypothesis)
 
         rowlabels = [f"marginaleffects__{i + 1}" for i in range(x.shape[0])]
     else:
-        if "term" not in x.columns or x["term"].count() != x["term"].unique().count():
+        if "term" not in x.columns or len(x["term"]) != len(x["term"].unique()):
             msg = 'To use term names in a `hypothesis` string, the same function call without `hypothesis` argument must produce a `term` column with unique row identifiers. You can use `b1`, `b2`, etc. indices instead of term names in the `hypotheses` string Ex: "b1 + b2 = 0" Alternatively, you can use the `newdata`, `variables`, or `by` arguments:'
             raise ValueError(msg)
 
         rowlabels = x["term"].to_list()
 
     def eval_string_function(vec, hypothesis, rowlabels):
         env = {rowlabel: vec[i] for i, rowlabel in enumerate(rowlabels)}
```

### Comparing `marginaleffects-0.0.3/marginaleffects/predictions.py` & `marginaleffects-0.0.4/marginaleffects/predictions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import patsy
 import polars as pl
 
 from .by import get_by
 from .equivalence import get_equivalence
 from .hypothesis import get_hypothesis
-from .sanity import sanitize_newdata, sanitize_vcov
+from .sanity import sanitize_newdata, sanitize_vcov, get_variables_names
 from .transform import get_transform
 from .uncertainty import get_jacobian, get_se, get_z_p_ci
-from .utils import sort_columns
+from .utils import sort_columns, get_modeldata, get_pad, upcast
 from .classes import MarginaleffectsDataFrame
 
 
 def get_predictions(model, params, newdata: pl.DataFrame):
     if isinstance(newdata, np.ndarray):
         exog = newdata
     else:
@@ -90,14 +90,30 @@
     """
     pass
 
     # sanity checks
     V = sanitize_vcov(vcov, model)
     newdata = sanitize_newdata(model, newdata, wts=wts)
 
+    # pad
+    modeldata = get_modeldata(model)
+    pad = []
+    vs = get_variables_names(variables = None, model = model, newdata = modeldata)
+    for v in vs:
+        if not newdata[v].is_numeric():
+            uniqs = modeldata[v].unique()
+            if not all(uniq in newdata[v] for uniq in uniqs):
+                pad.append(get_pad(modeldata, v, uniqs))
+    if len(pad) > 0:
+        pad = pl.concat(pad)
+        tmp = upcast([newdata, pad])
+        newdata = pl.concat(tmp, how = "diagonal")
+    else:
+        pad = pl.DataFrame()
+
     # predictors
     y, exog = patsy.dmatrices(model.model.formula, newdata.to_pandas())
 
     # estimands
     def fun(x):
         out = get_predictions(model, np.array(x), exog)
         out = get_by(model, out, newdata=newdata, by=by, wts=wts)
@@ -110,14 +126,18 @@
         se = get_se(J, V)
         out = out.with_columns(pl.Series(se).alias("std_error"))
         out = get_z_p_ci(out, model, conf_level=conf_level)
     out = get_transform(out, transform=transform)
     out = get_equivalence(out, equivalence=equivalence)
     out = sort_columns(out, by=by)
 
+    # unpad
+    if "rowid" in out.columns and pad.shape[0] > 0:
+        out = out[:-pad.shape[0]:]
+
     out = MarginaleffectsDataFrame(out, by=by, conf_level=conf_level)
     return out
 
 
 def avg_predictions(
     model,
     conf_level=0.95,
```

### Comparing `marginaleffects-0.0.3/marginaleffects/sanity.py` & `marginaleffects-0.0.4/marginaleffects/sanity.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/slopes.py` & `marginaleffects-0.0.4/marginaleffects/slopes.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/uncertainty.py` & `marginaleffects-0.0.4/marginaleffects/uncertainty.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.3/marginaleffects/utils.py` & `marginaleffects-0.0.4/marginaleffects/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import numpy as np
 import polars as pl
 
 
 def get_modeldata(fit):
     df = fit.model.data.frame
     try:
@@ -75,26 +76,30 @@
     ]
 
     tmp = [df for df in dfs if type(df) is pl.DataFrame]
 
     if len(tmp) == 0:
         return dfs
 
-    for col in tmp[0].columns:
-        dtypes = [df[col].dtype for df in tmp]
+    cols = [df.columns for df in tmp]
+    cols = set(list(itertools.chain(*cols)))
+
+    for col in cols:
+        dtypes = [df[col].dtype for df in tmp if col in df.columns]
         match = [
             next((i for i, x in enumerate(numeric_types) if x == dtype), None)
             for dtype in dtypes
         ]
         match = list(set(match))
         if len(match) > 1:
             match = max(match)
             if match is not None:
                 for i, v in enumerate(tmp):
                     tmp[i] = tmp[i].with_columns(pl.col(col).cast(numeric_types[match]))
+
     return tmp
 
 
 
 def get_variable_type(variable, newdata):
     inttypes = [pl.Int32, pl.Int64, pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64]
     if variable not in newdata.columns:
```

### Comparing `marginaleffects-0.0.3/pyproject.toml` & `marginaleffects-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marginaleffects"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Vincent Arel-Bundock <vincent.arel-bundock@umontreal.ca>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pandas = "^2.0.2"
@@ -22,14 +22,15 @@
 mkautodoc = "^0.2.0"
 matplotlib = "^3.7.1"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 typing-extensions = "^4.7.0"
 pytest-xdist = "^3.3.1"
+bandit = "^1.7.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = [
```

### Comparing `marginaleffects-0.0.3/PKG-INFO` & `marginaleffects-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marginaleffects
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Vincent Arel-Bundock
 Author-email: vincent.arel-bundock@umontreal.ca
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

