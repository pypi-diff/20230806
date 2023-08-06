# Comparing `tmp/bayescombat-0.0.1.tar.gz` & `tmp/bayescombat-0.0.2.tar.gz`

## Comparing `bayescombat-0.0.1.tar` & `bayescombat-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.1/src/BayesComBat/__init__.py
--rw-r--r--   0        0        0    16670 2020-02-02 00:00:00.000000 bayescombat-0.0.1/src/BayesComBat/harmonize.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 bayescombat-0.0.1/.gitignore
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.1/README.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bayescombat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bayescombat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bayescombat-0.0.2/src/BayesComBat/__init__.py
+-rw-r--r--   0        0        0    16670 2020-02-02 00:00:00.000000 bayescombat-0.0.2/src/BayesComBat/harmonize.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bayescombat-0.0.2/.gitignore
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bayescombat-0.0.2/README.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 bayescombat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bayescombat-0.0.2/PKG-INFO
```

### Comparing `bayescombat-0.0.1/src/BayesComBat/harmonize.py` & `bayescombat-0.0.2/src/BayesComBat/harmonize.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
 
     #Numpyro With MCMC
 
     rng_key = random.PRNGKey(0)
     rng_key, rng_key_ = random.split(rng_key)
 
     #10,000 samples but do 1000 x 10
-    # num_warmup, num_samples, n_iterations, warmup_thinning = 4000, 1000, 10, 10
-    num_warmup, num_samples, n_iterations, warmup_thinning = 400, 100, 10, 10
+    num_warmup, num_samples, n_iterations, warmup_thinning = 4000, 1000, 10, 10
+    # num_warmup, num_samples, n_iterations, warmup_thinning = 400, 100, 10, 10
 
     # Run NUTS.
     kernel = NUTS(reparam_model)
     num_chains = 4
     mcmc = MCMC(kernel, num_warmup = num_warmup, num_samples = num_samples, num_chains = num_chains, thinning=warmup_thinning)
     mcmc.warmup(rng_key_, X_df = df[covariates], i = df[batch_var], j = df[subject_var], 
                 unique_i=unique_i,unique_j=unique_j,i_counts=i_counts,v_count=v_count,x_count=x_count,j_count=j_count,i_count=i_count,feature_zeros=feature_zeros,feature_ones=feature_ones,feature_0_5=feature_0_5,
```

### Comparing `bayescombat-0.0.1/pyproject.toml` & `bayescombat-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "BayesComBat"
-version = "0.0.1"
+version = "0.0.2"
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
+dependencies = [
+  'numpy >= 1.21',
+  'pandas > 1.3',
+  'numpyro >= 0.7.2',
+  'jax >= 0.2.17',
+]
 
 [project.urls]
 "Homepage" = "https://github.com/batmanlab/BayesComBat"
```

