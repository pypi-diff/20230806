# Comparing `tmp/bayescombat-0.0.3.tar.gz` & `tmp/bayescombat-0.0.4.tar.gz`

## Comparing `bayescombat-0.0.3.tar` & `bayescombat-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.3/src/BayesComBat/__init__.py
--rw-r--r--   0        0        0    16590 2020-02-02 00:00:00.000000 bayescombat-0.0.3/src/BayesComBat/harmonize.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bayescombat-0.0.3/.gitignore
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.3/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bayescombat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 bayescombat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.4/src/BayesComBat/__init__.py
+-rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 bayescombat-0.0.4/src/BayesComBat/harmonize.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bayescombat-0.0.4/.gitignore
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.4/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bayescombat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 bayescombat-0.0.4/PKG-INFO
```

### Comparing `bayescombat-0.0.3/src/BayesComBat/harmonize.py` & `bayescombat-0.0.4/src/BayesComBat/harmonize.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     #Numpyro With MCMC
 
     rng_key = random.PRNGKey(0)
     rng_key, rng_key_ = random.split(rng_key)
 
     #10,000 samples but do 1000 x 10
     num_warmup, num_samples, n_iterations, warmup_thinning = 4000, 1000, 10, 10
+    print()
 
     # Run NUTS.
     kernel = NUTS(reparam_model)
     num_chains = 4
     mcmc = MCMC(kernel, num_warmup = num_warmup, num_samples = num_samples, num_chains = num_chains, thinning=warmup_thinning)
     mcmc.warmup(rng_key_, X_df = df[covariates], i = df[batch_var], j = df[subject_var], 
                 unique_i=unique_i,unique_j=unique_j,i_counts=i_counts,v_count=v_count,x_count=x_count,j_count=j_count,i_count=i_count,feature_zeros=feature_zeros,feature_ones=feature_ones,feature_0_5=feature_0_5,
```

### Comparing `bayescombat-0.0.3/pyproject.toml` & `bayescombat-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "BayesComBat"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Maxwell Reynolds", email="maxreynolds55@gmail.com" },
 ]
 description = "Fully Bayesian ComBat Harmonization"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'numpy >= 1.21',
   'pandas > 1.3',
-  'numpyro >= 0.7.2'
+  'numpyro == 0.7.2'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/batmanlab/BayesComBat"
```

### Comparing `bayescombat-0.0.3/PKG-INFO` & `bayescombat-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: BayesComBat
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fully Bayesian ComBat Harmonization
 Project-URL: Homepage, https://github.com/batmanlab/BayesComBat
 Author-email: Maxwell Reynolds <maxreynolds55@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy>=1.21
-Requires-Dist: numpyro>=0.7.2
+Requires-Dist: numpyro==0.7.2
 Requires-Dist: pandas>1.3
 Description-Content-Type: text/markdown
 
 # Repository for Fully Bayesian ComBat
 
 This is the home of Fully Bayesian Combat, an extension of [Longitudinal ComBat](https://github.com/jcbeer/longCombat) which uses fully Bayesian inference rather than empirical Bayes.
```

