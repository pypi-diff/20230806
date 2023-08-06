# Comparing `tmp/tcia_utils-1.6.2.tar.gz` & `tmp/tcia_utils-1.6.3.tar.gz`

## Comparing `tcia_utils-1.6.2.tar` & `tcia_utils-1.6.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    72518 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/src/tcia_utils/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/LICENSE
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 tcia_utils-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    72518 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/LICENSE
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/PKG-INFO
```

### Comparing `tcia_utils-1.6.2/src/tcia_utils/datacite.py` & `tcia_utils-1.6.3/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/src/tcia_utils/nbia.py` & `tcia_utils-1.6.3/src/tcia_utils/nbia.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/src/tcia_utils/pathdb.py` & `tcia_utils-1.6.3/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/src/tcia_utils/utils.py` & `tcia_utils-1.6.3/src/tcia_utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 
-def searchDf(search_term, column_name=None, dataframe_var='df'):
-    # If the custom dataframe variable name is provided, use that to get the dataframe
-    if dataframe_var in globals():
-        df = globals()[dataframe_var]
+def searchDf(search_term, column_name=None, dataframe=None,):
+    if dataframe is None:
+        # If dataframe is not provided, assume the dataframe is named 'df'
+        if 'df' in globals():
+            df = globals()['df']
+        else:
+            raise ValueError("Dataframe variable 'df' not found in the global namespace.")
     else:
-        raise ValueError(f"Dataframe variable '{dataframe_var}' not found in the global namespace.")
+        df = dataframe
 
     if column_name:
         result = df[df[column_name].astype(str).str.contains(search_term, case=False)]
     else:
         result = df[df.apply(lambda row: any(row.astype(str).str.contains(search_term, case=False)), axis=1)]
     return result
```

### Comparing `tcia_utils-1.6.2/.gitignore` & `tcia_utils-1.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/LICENSE` & `tcia_utils-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/README.md` & `tcia_utils-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.2/pyproject.toml` & `tcia_utils-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.6.2"
+version = "1.6.3"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.6.2/PKG-INFO` & `tcia_utils-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.6.2
+Version: 1.6.3
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

