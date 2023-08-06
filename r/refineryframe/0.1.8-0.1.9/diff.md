# Comparing `tmp/refineryframe-0.1.8.tar.gz` & `tmp/refineryframe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.1.8.tar", last modified: Sat Aug  5 14:04:51 2023, max compression
+gzip compressed data, was "refineryframe-0.1.9.tar", last modified: Sat Aug  5 16:27:24 2023, max compression
```

## Comparing `refineryframe-0.1.8.tar` & `refineryframe-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.067758 refineryframe-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 14:04:38.000000 refineryframe-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 14:04:51.063758 refineryframe-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31172 2023-08-05 14:04:38.000000 refineryframe-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/refineryframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36627 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/detect_unexpected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/refiner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 14:04:38.000000 refineryframe-0.1.8/refineryframe/replace_unexpected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/refineryframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31901 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 14:04:51.000000 refineryframe-0.1.8/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 14:04:50.000000 refineryframe-0.1.8/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:04:51.067758 refineryframe-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 14:04:50.000000 refineryframe-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:51.063758 refineryframe-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-05 14:04:38.000000 refineryframe-0.1.8/tests/test_refiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:27:24.231776 refineryframe-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 16:27:07.000000 refineryframe-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-08-05 16:27:24.231776 refineryframe-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-08-05 16:27:21.000000 refineryframe-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:27:24.231776 refineryframe-0.1.9/refineryframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-05 16:27:21.000000 refineryframe-0.1.9/refineryframe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36687 2023-08-05 16:27:07.000000 refineryframe-0.1.9/refineryframe/detect_unexpected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12527 2023-08-05 16:27:07.000000 refineryframe-0.1.9/refineryframe/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-05 16:27:07.000000 refineryframe-0.1.9/refineryframe/refiner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14051 2023-08-05 16:27:07.000000 refineryframe-0.1.9/refineryframe/replace_unexpected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:27:24.231776 refineryframe-0.1.9/refineryframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-08-05 16:27:24.000000 refineryframe-0.1.9/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 16:27:24.000000 refineryframe-0.1.9/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:27:24.000000 refineryframe-0.1.9/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 16:27:24.000000 refineryframe-0.1.9/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 16:27:24.000000 refineryframe-0.1.9/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:27:24.231776 refineryframe-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-05 16:27:21.000000 refineryframe-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:27:24.231776 refineryframe-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-05 16:27:07.000000 refineryframe-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-08-05 16:27:07.000000 refineryframe-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-08-05 16:27:07.000000 refineryframe-0.1.9/tests/test_refiner.py
```

### Comparing `refineryframe-0.1.8/LICENSE` & `refineryframe-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.8/PKG-INFO` & `refineryframe-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -876,15 +876,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
-     'ids_for_dedup': None,
+     'ids_for_dedup': 'ALL',
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.8/README.md` & `refineryframe-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -856,15 +856,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
-     'ids_for_dedup': None,
+     'ids_for_dedup': 'ALL',
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.8/refineryframe/detect_unexpected.py` & `refineryframe-0.1.9/refineryframe/detect_unexpected.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
         ROW_DUPLICATES = False
         KEY_DUPLICATES = False
 
         duplicates = dataframe.duplicated()
         n_duplicates = duplicates.sum()
 
-        if (subset is not None) and (subset in list(dataframe.columns)):
+        if (subset is not None) and (subset != "ALL") and (subset in list(dataframe.columns)):
             subset_duplicates = dataframe.duplicated(subset=subset)
             n_subset_duplicates = subset_duplicates.sum()
 
             if n_subset_duplicates > 0:
                 logger.warning(f"There are {n_subset_duplicates} duplicate keys : {n_subset_duplicates/dataframe.shape[0]*100:.2f}%")
 
                 n_true_dup = n_subset_duplicates - n_duplicates
@@ -705,17 +705,17 @@
 
         if unexpected_conditions:
             run_check_additional_cons = sum([unexpected_conditions[i]['warning'] for i in unexpected_conditions]) > 0
         else:
             run_check_additional_cons = False
 
 
-        if ids_for_dedup is None:
+        if ((ids_for_dedup is None) or (ids_for_dedup == "ALL")):
 
-            if (len(index_cols) > 0) and (index_cols in list(dataframe.columns)):
+            if (len(index_cols) > 0) and (list(index_cols) in list(dataframe.columns)):
                 ids_for_dedup = list(index_cols)
             else:
                 ids_for_dedup = list(dataframe.columns)
 
 
         # Checks scan
         unexpected_exceptions_scaned = {
```

### Comparing `refineryframe-0.1.8/refineryframe/other.py` & `refineryframe-0.1.9/refineryframe/other.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.8/refineryframe/refiner.py` & `refineryframe-0.1.9/refineryframe/refiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,15 @@
     loggerLvl = attr.ib(default=logging.INFO)
     dotline_length = attr.ib(default=50, type=int)
 
     lower_bound = attr.ib(default=-float("inf"))
     upper_bound = attr.ib(default=float("inf"))
     earliest_date = attr.ib(default="1900-08-25")
     latest_date = attr.ib(default="2100-01-01")
-
-    ids_for_dedup = attr.ib(default=None, type=list)
+    ids_for_dedup = attr.ib(default="ALL", type=list)
 
     unexpected_exceptions_duv = attr.ib(default={"col_names_types": "NONE",
                                               "missing_values": "NONE",
                                               "missing_types": "NONE",
                                               "inf_values": "NONE",
                                               "date_format": "NONE",
                                               "duplicates": "NONE",
```

### Comparing `refineryframe-0.1.8/refineryframe/replace_unexpected.py` & `refineryframe-0.1.9/refineryframe/replace_unexpected.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.1.8/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.1.9/refineryframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -876,15 +876,15 @@
      'logger_name': 'Refiner',
      'loggerLvl': 10,
      'dotline_length': 50,
      'lower_bound': -inf,
      'upper_bound': inf,
      'earliest_date': '1900-08-25',
      'latest_date': '2100-01-01',
-     'ids_for_dedup': None,
+     'ids_for_dedup': 'ALL',
      'unexpected_exceptions_duv': {'col_names_types': 'NONE',
       'missing_values': 'ALL',
       'missing_types': 'ALL',
       'inf_values': 'NONE',
       'date_format': 'NONE',
       'duplicates': 'ALL',
       'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.8/setup.py` & `refineryframe-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "attrs>=22.2.0",
     "datetime",
     "pandas",
     "numpy",
     "unidecode"
 ]
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them according to set of predefined rules'
 
 # Setting up
 setup(
     name="refineryframe",
     #use_scm_version=True,
```

### Comparing `refineryframe-0.1.8/tests/conftest.py` & `refineryframe-0.1.9/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                         'logger_name': 'Refiner',
                         'loggerLvl': 10,
                         'dotline_length': 50,
                         'lower_bound': -np.inf,
                         'upper_bound': np.inf,
                         'earliest_date': '1900-08-25',
                         'latest_date': '2100-01-01',
-                        'ids_for_dedup': None,
+                        'ids_for_dedup': 'ALL',
                         'unexpected_exceptions_duv': {'col_names_types': 'NONE',
                         'missing_values': 'ALL',
                         'missing_types': 'ALL',
                         'inf_values': 'NONE',
                         'date_format': 'NONE',
                         'duplicates': 'ALL',
                         'date_range': 'NONE',
```

### Comparing `refineryframe-0.1.8/tests/test_refiner.py` & `refineryframe-0.1.9/tests/test_refiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from refineryframe.refiner import Refiner, check_duplicates
 
 def test_make_refiner_class(df, replace_dict, unexpected_exceptions):
 
     try:
         tns = Refiner(dataframe = df,
               replace_dict = replace_dict,
+              ids_for_dedup = None,
               loggerLvl = logging.DEBUG,
               unexpected_exceptions_duv = unexpected_exceptions)
     except Exception as e:
         pytest.fail(f"divide function raised an exception: {e}")
 
     # If no exception was raised, the test passes
     assert isinstance(tns, Refiner)
```

