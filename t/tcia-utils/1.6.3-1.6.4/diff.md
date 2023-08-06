# Comparing `tmp/tcia_utils-1.6.3.tar.gz` & `tmp/tcia_utils-1.6.4.tar.gz`

## Comparing `tcia_utils-1.6.3.tar` & `tcia_utils-1.6.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    72518 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/src/tcia_utils/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/LICENSE
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 tcia_utils-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    72518 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/LICENSE
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 tcia_utils-1.6.4/PKG-INFO
```

### Comparing `tcia_utils-1.6.3/src/tcia_utils/datacite.py` & `tcia_utils-1.6.4/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/src/tcia_utils/nbia.py` & `tcia_utils-1.6.4/src/tcia_utils/nbia.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/src/tcia_utils/pathdb.py` & `tcia_utils-1.6.4/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/.gitignore` & `tcia_utils-1.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/LICENSE` & `tcia_utils-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/README.md` & `tcia_utils-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.6.3/pyproject.toml` & `tcia_utils-1.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.6.3"
+version = "1.6.4"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.6.3/PKG-INFO` & `tcia_utils-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.6.3
+Version: 1.6.4
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

