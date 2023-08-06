# Comparing `tmp/bayescombat-0.0.5.tar.gz` & `tmp/bayescombat-0.0.6.tar.gz`

## Comparing `bayescombat-0.0.5.tar` & `bayescombat-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.5/src/BayesComBat/__init__.py
--rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 bayescombat-0.0.5/src/BayesComBat/harmonize.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bayescombat-0.0.5/.gitignore
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.5/README.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bayescombat-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bayescombat-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.6/src/BayesComBat/__init__.py
+-rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 bayescombat-0.0.6/src/BayesComBat/harmonize.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bayescombat-0.0.6/.gitignore
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.6/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bayescombat-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 bayescombat-0.0.6/PKG-INFO
```

### Comparing `bayescombat-0.0.5/src/BayesComBat/harmonize.py` & `bayescombat-0.0.6/src/BayesComBat/harmonize.py`

 * *Files identical despite different names*

### Comparing `bayescombat-0.0.5/pyproject.toml` & `bayescombat-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "BayesComBat"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Maxwell Reynolds", email="maxreynolds55@gmail.com" },
 ]
 description = "Fully Bayesian ComBat Harmonization"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,13 +16,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'numpy >= 1.21',
   'pandas > 1.3',
   'jax == 0.2.17',
-  'numpyro == 0.7.2'
+  'numpyro == 0.7.2',
+  'jaxlib==0.1.68'
 
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/batmanlab/BayesComBat"
```

### Comparing `bayescombat-0.0.5/PKG-INFO` & `bayescombat-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: BayesComBat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fully Bayesian ComBat Harmonization
 Project-URL: Homepage, https://github.com/batmanlab/BayesComBat
 Author-email: Maxwell Reynolds <maxreynolds55@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: jax==0.2.17
+Requires-Dist: jaxlib==0.1.68
 Requires-Dist: numpy>=1.21
 Requires-Dist: numpyro==0.7.2
 Requires-Dist: pandas>1.3
 Description-Content-Type: text/markdown
 
 # Repository for Fully Bayesian ComBat
```

