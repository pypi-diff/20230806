# Comparing `tmp/MetaHeuristicsFS-0.0.7.tar.gz` & `tmp/MetaHeuristicsFS-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MetaHeuristicsFS-0.0.7.tar", last modified: Sun Mar 19 03:44:17 2023, max compression
+gzip compressed data, was "dist/MetaHeuristicsFS-0.0.8.tar", last modified: Sun Aug  6 13:53:04 2023, max compression
```

## Comparing `MetaHeuristicsFS-0.0.7.tar` & `MetaHeuristicsFS-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/
--rw-rw-r--   0 azim      (1000) azim      (1000)     7939 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/setup.cfg
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/
--rw-rw-r--   0 azim      (1000) azim      (1000)    72532 2023-03-19 03:36:01.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.py
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/
--rw-rw-r--   0 azim      (1000) azim      (1000)     7939 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/PKG-INFO
--rw-rw-r--   0 azim      (1000) azim      (1000)       26 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/requires.txt
--rw-rw-r--   0 azim      (1000) azim      (1000)      280 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/SOURCES.txt
--rw-rw-r--   0 azim      (1000) azim      (1000)       17 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/top_level.txt
--rw-rw-r--   0 azim      (1000) azim      (1000)        1 2023-03-19 03:44:17.000000 MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/dependency_links.txt
--rw-r--r--   0 azim      (1000) azim      (1000)     7413 2023-03-19 02:08:49.000000 MetaHeuristicsFS-0.0.7/README.rst
--rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 MetaHeuristicsFS-0.0.7/LICENSE
--rw-r--r--   0 azim      (1000) azim      (1000)      925 2023-03-19 03:32:43.000000 MetaHeuristicsFS-0.0.7/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:53:04.199348 MetaHeuristicsFS-0.0.8/
+-rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 MetaHeuristicsFS-0.0.8/LICENSE
+-rw-rw-r--   0 azim      (1000) azim      (1000)     8949 2023-08-06 13:53:04.203348 MetaHeuristicsFS-0.0.8/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)     7433 2023-08-06 13:52:46.000000 MetaHeuristicsFS-0.0.8/README.rst
+-rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-08-06 13:53:04.203348 MetaHeuristicsFS-0.0.8/setup.cfg
+-rw-r--r--   0 azim      (1000) azim      (1000)      926 2023-08-06 13:51:24.000000 MetaHeuristicsFS-0.0.8/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:53:04.183348 MetaHeuristicsFS-0.0.8/src/
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:53:04.199348 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/
+-rw-rw-r--   0 azim      (1000) azim      (1000)     8949 2023-08-06 13:53:04.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/PKG-INFO
+-rw-rw-r--   0 azim      (1000) azim      (1000)      280 2023-08-06 13:53:04.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/SOURCES.txt
+-rw-rw-r--   0 azim      (1000) azim      (1000)        1 2023-08-06 13:53:04.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/dependency_links.txt
+-rw-rw-r--   0 azim      (1000) azim      (1000)       26 2023-08-06 13:53:04.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/requires.txt
+-rw-rw-r--   0 azim      (1000) azim      (1000)       17 2023-08-06 13:53:04.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/top_level.txt
+-rw-rw-r--   0 azim      (1000) azim      (1000)    72532 2023-03-19 03:36:01.000000 MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MetaHeuristicsFS-0.0.7/PKG-INFO` & `MetaHeuristicsFS-0.0.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: MetaHeuristicsFS
-Version: 0.0.7
-Summary: Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists`
-Home-page: https://github.com/StatguyUser/MetaHeuristicsFS
-Author: StatguyUser
-License: UNKNOWN
-Download-URL: https://github.com/MetaHeuristicsFS/MetaHeuristicsFS.git
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 What is it?
 ===========
 
-Companion library of machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
+Companion library of machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
 
 MetaHeuristicsFS module helps in identifying combination of features that gives best result. Process of searching best combination is called 'feature selection'. This library uses metaheuristic based algorithms such as genetic algorithm, simulated annealing, ant colony optimization, and particle swarm optimization, for performing feature selection.
 
 
 Input parameters
 ================
 
@@ -118,22 +106,20 @@
 ================
 
  - [Example 1 - Regression](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/main/Chapter%208%20-%20Predicting%20Room%20Bookings%20-%20More%20Genetic%20Algorithm%20Iterations.ipynb)
  - [Example 2 - Classification](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/37ba0d2921fbabbb83df44c6eb7a1242b19a637f/Chapter%208%20-%20Hotel%20Cancelation%20.ipynb)
 
 How to cite
 ================
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
+Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
 
 Where to get it?
 ================
 
 `pip install MetaHeuristicsFS`
 
 Dependencies
 ============
 
  - [numpy](https://numpy.org/)
  - [scikit-learn](https://scikit-learn.org/)
 
-
-
```

### Comparing `MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.py` & `MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.py`

 * *Files identical despite different names*

### Comparing `MetaHeuristicsFS-0.0.7/src/MetaHeuristicsFS.egg-info/PKG-INFO` & `MetaHeuristicsFS-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,139 +1,136 @@
 Metadata-Version: 2.1
 Name: MetaHeuristicsFS
-Version: 0.0.7
-Summary: Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists`
+Version: 0.0.8
+Summary: Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists`
 Home-page: https://github.com/StatguyUser/MetaHeuristicsFS
 Author: StatguyUser
 License: UNKNOWN
 Download-URL: https://github.com/MetaHeuristicsFS/MetaHeuristicsFS.git
+Description: What is it?
+        ===========
+        
+        Companion library of machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
+        
+        MetaHeuristicsFS module helps in identifying combination of features that gives best result. Process of searching best combination is called 'feature selection'. This library uses metaheuristic based algorithms such as genetic algorithm, simulated annealing, ant colony optimization, and particle swarm optimization, for performing feature selection.
+        
+        
+        Input parameters
+        ================
+        
+          - **Machine Learning Parameters: These are common for all algorithms**
+            
+            `columns_list` : Column names present in x_train_dataframe and x_test which will be used as input list for searching best list of features.
+        
+            `data_dict` : X and Y training and test data provided in dictionary format. Below is example of 5 fold cross validation data with keys.
+                {0:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                1:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                2:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                3:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                4:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array}}
+                
+            If you only have train and test data and do not wish to do cross validation, use above dictionary format, with only one key.
+        
+            `use_validation_data` : Whether you want to use validation data as a boolean True or False. Default value is True. If false, user need not provide x_validation_dataframe and y_validation_dataframe
+            
+            `x_validation_dataframe` : dataframe containing features of validatoin dataset. Default is blank pandas dataframe.
+            
+            `y_validation_dataframe` : dataframe containing dependent variable of validation dataset. Default is blank pandas dataframe.
+            
+            `model` : Model object. It should have .fit and .predict attribute
+                
+            `cost_function_improvement` : Objective is to whether increase or decrease the cost during subsequent iterations.
+                For regression it should be 'decrease' and for classification it should be 'increase'
+        
+            `cost_function` : Cost function for finding cost between actual and predicted values, depending on regression or classification problem.
+                cost function should accept 'actual' and 'predicted' as arrays and return cost for the both.
+            
+            `average` : Averaging to be used. This is useful for clasification metrics such as 'f1_score', 'jaccard_score', 'fbeta_score', 'precision_score',
+                'recall_score' and 'roc_auc_score' when dependent variable is multi-class
+            
+          - **Genetic Algorithm Feature Selection (GeneticAlgorithmFS) Parameters**
+            
+            `generations` : Number of generations to run genetic algorithm. 100 as deafult
+            
+            `population` : Number of individual chromosomes. 50 as default. It should be kept as low number if number of possible permutation and combination of feature sets are small.
+            
+            `prob_crossover` : Probability of crossover. 0.9 as default
+            
+            `prob_mutation` : Probability of mutation. 0.1 as default
+                
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+          - **Simulated Annealing Feature Selection (SimulatedAnnealingFS) Parameters**
+            
+            `temperature` : Initial temperature for annealing. Default is 1500
+            
+            `iterations` : Number of times simulated annealing will search for solutions. Default is 100.
+            
+            `n_perturb` : Number of times feature set will be perturbed in an iteration. Default is 1.
+            
+            `n_features_percent_perturb` : Percentage of features that will be perturbed during each perturbation. Value are between 1 and 100.
+            
+            `alpha` : Temperature reduction factor. Defaults is 0.9.
+                
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+          - **Ant Colony Optimization Feature Selection (AntColonyOptimizationFS) Parameters**
+            
+            `iterations` : Number of times ant colony optimization will search for solutions. Default is 100
+            
+            `N_ants` : Number of ants in each iteration. Default is 100.
+        
+            `run_time` : Number of minutes to run the algorithm. This is checked in between each iteration.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from iterations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+            `evaporation_rate` : Evaporation rate. Values are between 0 and 1. If it is too large, chances are higher to find global optima, but computationally expensive. If it is low, chances of finding global optima are less. Default is kept as 0.9
+            
+            `Q` : Pheromene update coefficient. Value between 0 and 1. It affects the convergence speed. If it is large, ACO will get stuck at local optima. Default is kept as 0.2
+        
+          - **Particle Swarm Optimization Feature Selection (ParticleSwarmOptimizationFS) Parameters**
+            
+            `iterations` : Number of times particle swarm optimization will search for solutions. Default is 100.
+            
+            `swarmSize` : Size of the swarm in each iteration. Default is 100.
+            
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+        Output
+        ================
+        
+          - **best_columns** : List object with list of column names which gives best performance for the model. These features can be used for training and saving models separately by the user.
+        
+        Examples
+        ================
+        
+         - [Example 1 - Regression](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/main/Chapter%208%20-%20Predicting%20Room%20Bookings%20-%20More%20Genetic%20Algorithm%20Iterations.ipynb)
+         - [Example 2 - Classification](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/37ba0d2921fbabbb83df44c6eb7a1242b19a637f/Chapter%208%20-%20Hotel%20Cancelation%20.ipynb)
+        
+        How to cite
+        ================
+        Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
+        
+        Where to get it?
+        ================
+        
+        `pip install MetaHeuristicsFS`
+        
+        Dependencies
+        ============
+        
+         - [numpy](https://numpy.org/)
+         - [scikit-learn](https://scikit-learn.org/)
+        
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-What is it?
-===========
-
-Companion library of machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
-
-MetaHeuristicsFS module helps in identifying combination of features that gives best result. Process of searching best combination is called 'feature selection'. This library uses metaheuristic based algorithms such as genetic algorithm, simulated annealing, ant colony optimization, and particle swarm optimization, for performing feature selection.
-
-
-Input parameters
-================
-
-  - **Machine Learning Parameters: These are common for all algorithms**
-    
-    `columns_list` : Column names present in x_train_dataframe and x_test which will be used as input list for searching best list of features.
-
-    `data_dict` : X and Y training and test data provided in dictionary format. Below is example of 5 fold cross validation data with keys.
-        {0:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        1:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        2:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        3:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        4:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array}}
-        
-    If you only have train and test data and do not wish to do cross validation, use above dictionary format, with only one key.
-
-    `use_validation_data` : Whether you want to use validation data as a boolean True or False. Default value is True. If false, user need not provide x_validation_dataframe and y_validation_dataframe
-    
-    `x_validation_dataframe` : dataframe containing features of validatoin dataset. Default is blank pandas dataframe.
-    
-    `y_validation_dataframe` : dataframe containing dependent variable of validation dataset. Default is blank pandas dataframe.
-    
-    `model` : Model object. It should have .fit and .predict attribute
-        
-    `cost_function_improvement` : Objective is to whether increase or decrease the cost during subsequent iterations.
-        For regression it should be 'decrease' and for classification it should be 'increase'
-
-    `cost_function` : Cost function for finding cost between actual and predicted values, depending on regression or classification problem.
-        cost function should accept 'actual' and 'predicted' as arrays and return cost for the both.
-    
-    `average` : Averaging to be used. This is useful for clasification metrics such as 'f1_score', 'jaccard_score', 'fbeta_score', 'precision_score',
-        'recall_score' and 'roc_auc_score' when dependent variable is multi-class
-    
-  - **Genetic Algorithm Feature Selection (GeneticAlgorithmFS) Parameters**
-    
-    `generations` : Number of generations to run genetic algorithm. 100 as deafult
-    
-    `population` : Number of individual chromosomes. 50 as default. It should be kept as low number if number of possible permutation and combination of feature sets are small.
-    
-    `prob_crossover` : Probability of crossover. 0.9 as default
-    
-    `prob_mutation` : Probability of mutation. 0.1 as default
-        
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-  - **Simulated Annealing Feature Selection (SimulatedAnnealingFS) Parameters**
-    
-    `temperature` : Initial temperature for annealing. Default is 1500
-    
-    `iterations` : Number of times simulated annealing will search for solutions. Default is 100.
-    
-    `n_perturb` : Number of times feature set will be perturbed in an iteration. Default is 1.
-    
-    `n_features_percent_perturb` : Percentage of features that will be perturbed during each perturbation. Value are between 1 and 100.
-    
-    `alpha` : Temperature reduction factor. Defaults is 0.9.
-        
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-  - **Ant Colony Optimization Feature Selection (AntColonyOptimizationFS) Parameters**
-    
-    `iterations` : Number of times ant colony optimization will search for solutions. Default is 100
-    
-    `N_ants` : Number of ants in each iteration. Default is 100.
-
-    `run_time` : Number of minutes to run the algorithm. This is checked in between each iteration.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from iterations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-    `evaporation_rate` : Evaporation rate. Values are between 0 and 1. If it is too large, chances are higher to find global optima, but computationally expensive. If it is low, chances of finding global optima are less. Default is kept as 0.9
-    
-    `Q` : Pheromene update coefficient. Value between 0 and 1. It affects the convergence speed. If it is large, ACO will get stuck at local optima. Default is kept as 0.2
-
-  - **Particle Swarm Optimization Feature Selection (ParticleSwarmOptimizationFS) Parameters**
-    
-    `iterations` : Number of times particle swarm optimization will search for solutions. Default is 100.
-    
-    `swarmSize` : Size of the swarm in each iteration. Default is 100.
-    
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-Output
-================
-
-  - **best_columns** : List object with list of column names which gives best performance for the model. These features can be used for training and saving models separately by the user.
-
-Examples
-================
-
- - [Example 1 - Regression](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/main/Chapter%208%20-%20Predicting%20Room%20Bookings%20-%20More%20Genetic%20Algorithm%20Iterations.ipynb)
- - [Example 2 - Classification](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/37ba0d2921fbabbb83df44c6eb7a1242b19a637f/Chapter%208%20-%20Hotel%20Cancelation%20.ipynb)
-
-How to cite
-================
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
-
-Where to get it?
-================
-
-`pip install MetaHeuristicsFS`
-
-Dependencies
-============
-
- - [numpy](https://numpy.org/)
- - [scikit-learn](https://scikit-learn.org/)
-
-
-
```

### Comparing `MetaHeuristicsFS-0.0.7/README.rst` & `MetaHeuristicsFS-0.0.8/src/MetaHeuristicsFS.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,125 +1,136 @@
-What is it?
-===========
-
-Companion library of machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
-
-MetaHeuristicsFS module helps in identifying combination of features that gives best result. Process of searching best combination is called 'feature selection'. This library uses metaheuristic based algorithms such as genetic algorithm, simulated annealing, ant colony optimization, and particle swarm optimization, for performing feature selection.
-
-
-Input parameters
-================
-
-  - **Machine Learning Parameters: These are common for all algorithms**
-    
-    `columns_list` : Column names present in x_train_dataframe and x_test which will be used as input list for searching best list of features.
-
-    `data_dict` : X and Y training and test data provided in dictionary format. Below is example of 5 fold cross validation data with keys.
-        {0:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        1:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        2:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        3:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
-        4:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array}}
-        
-    If you only have train and test data and do not wish to do cross validation, use above dictionary format, with only one key.
-
-    `use_validation_data` : Whether you want to use validation data as a boolean True or False. Default value is True. If false, user need not provide x_validation_dataframe and y_validation_dataframe
-    
-    `x_validation_dataframe` : dataframe containing features of validatoin dataset. Default is blank pandas dataframe.
-    
-    `y_validation_dataframe` : dataframe containing dependent variable of validation dataset. Default is blank pandas dataframe.
-    
-    `model` : Model object. It should have .fit and .predict attribute
-        
-    `cost_function_improvement` : Objective is to whether increase or decrease the cost during subsequent iterations.
-        For regression it should be 'decrease' and for classification it should be 'increase'
-
-    `cost_function` : Cost function for finding cost between actual and predicted values, depending on regression or classification problem.
-        cost function should accept 'actual' and 'predicted' as arrays and return cost for the both.
-    
-    `average` : Averaging to be used. This is useful for clasification metrics such as 'f1_score', 'jaccard_score', 'fbeta_score', 'precision_score',
-        'recall_score' and 'roc_auc_score' when dependent variable is multi-class
-    
-  - **Genetic Algorithm Feature Selection (GeneticAlgorithmFS) Parameters**
-    
-    `generations` : Number of generations to run genetic algorithm. 100 as deafult
-    
-    `population` : Number of individual chromosomes. 50 as default. It should be kept as low number if number of possible permutation and combination of feature sets are small.
-    
-    `prob_crossover` : Probability of crossover. 0.9 as default
-    
-    `prob_mutation` : Probability of mutation. 0.1 as default
-        
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-  - **Simulated Annealing Feature Selection (SimulatedAnnealingFS) Parameters**
-    
-    `temperature` : Initial temperature for annealing. Default is 1500
-    
-    `iterations` : Number of times simulated annealing will search for solutions. Default is 100.
-    
-    `n_perturb` : Number of times feature set will be perturbed in an iteration. Default is 1.
-    
-    `n_features_percent_perturb` : Percentage of features that will be perturbed during each perturbation. Value are between 1 and 100.
-    
-    `alpha` : Temperature reduction factor. Defaults is 0.9.
-        
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-  - **Ant Colony Optimization Feature Selection (AntColonyOptimizationFS) Parameters**
-    
-    `iterations` : Number of times ant colony optimization will search for solutions. Default is 100
-    
-    `N_ants` : Number of ants in each iteration. Default is 100.
-
-    `run_time` : Number of minutes to run the algorithm. This is checked in between each iteration.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from iterations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-    `evaporation_rate` : Evaporation rate. Values are between 0 and 1. If it is too large, chances are higher to find global optima, but computationally expensive. If it is low, chances of finding global optima are less. Default is kept as 0.9
-    
-    `Q` : Pheromene update coefficient. Value between 0 and 1. It affects the convergence speed. If it is large, ACO will get stuck at local optima. Default is kept as 0.2
-
-  - **Particle Swarm Optimization Feature Selection (ParticleSwarmOptimizationFS) Parameters**
-    
-    `iterations` : Number of times particle swarm optimization will search for solutions. Default is 100.
-    
-    `swarmSize` : Size of the swarm in each iteration. Default is 100.
-    
-    `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
-        At start of each generation it is checked if runtime has exceeded than alloted time.
-        If case run time did exceeds provided limit, best result from generations executed so far is given as output.
-        Default is 2 hours. i.e. 120 minutes.
-
-Output
-================
-
-  - **best_columns** : List object with list of column names which gives best performance for the model. These features can be used for training and saving models separately by the user.
-
-Examples
-================
-
- - [Example 1 - Regression](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/main/Chapter%208%20-%20Predicting%20Room%20Bookings%20-%20More%20Genetic%20Algorithm%20Iterations.ipynb)
- - [Example 2 - Classification](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/37ba0d2921fbabbb83df44c6eb7a1242b19a637f/Chapter%208%20-%20Hotel%20Cancelation%20.ipynb)
-
-How to cite
-================
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
-
-Where to get it?
-================
-
-`pip install MetaHeuristicsFS`
-
-Dependencies
-============
-
- - [numpy](https://numpy.org/)
- - [scikit-learn](https://scikit-learn.org/)
-
+Metadata-Version: 2.1
+Name: MetaHeuristicsFS
+Version: 0.0.8
+Summary: Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists`
+Home-page: https://github.com/StatguyUser/MetaHeuristicsFS
+Author: StatguyUser
+License: UNKNOWN
+Download-URL: https://github.com/MetaHeuristicsFS/MetaHeuristicsFS.git
+Description: What is it?
+        ===========
+        
+        Companion library of machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
+        
+        MetaHeuristicsFS module helps in identifying combination of features that gives best result. Process of searching best combination is called 'feature selection'. This library uses metaheuristic based algorithms such as genetic algorithm, simulated annealing, ant colony optimization, and particle swarm optimization, for performing feature selection.
+        
+        
+        Input parameters
+        ================
+        
+          - **Machine Learning Parameters: These are common for all algorithms**
+            
+            `columns_list` : Column names present in x_train_dataframe and x_test which will be used as input list for searching best list of features.
+        
+            `data_dict` : X and Y training and test data provided in dictionary format. Below is example of 5 fold cross validation data with keys.
+                {0:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                1:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                2:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                3:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array},
+                4:{'x_train':x_train_dataframe,'y_train':y_train_array,'x_test':x_test_dataframe,'y_test':y_test_array}}
+                
+            If you only have train and test data and do not wish to do cross validation, use above dictionary format, with only one key.
+        
+            `use_validation_data` : Whether you want to use validation data as a boolean True or False. Default value is True. If false, user need not provide x_validation_dataframe and y_validation_dataframe
+            
+            `x_validation_dataframe` : dataframe containing features of validatoin dataset. Default is blank pandas dataframe.
+            
+            `y_validation_dataframe` : dataframe containing dependent variable of validation dataset. Default is blank pandas dataframe.
+            
+            `model` : Model object. It should have .fit and .predict attribute
+                
+            `cost_function_improvement` : Objective is to whether increase or decrease the cost during subsequent iterations.
+                For regression it should be 'decrease' and for classification it should be 'increase'
+        
+            `cost_function` : Cost function for finding cost between actual and predicted values, depending on regression or classification problem.
+                cost function should accept 'actual' and 'predicted' as arrays and return cost for the both.
+            
+            `average` : Averaging to be used. This is useful for clasification metrics such as 'f1_score', 'jaccard_score', 'fbeta_score', 'precision_score',
+                'recall_score' and 'roc_auc_score' when dependent variable is multi-class
+            
+          - **Genetic Algorithm Feature Selection (GeneticAlgorithmFS) Parameters**
+            
+            `generations` : Number of generations to run genetic algorithm. 100 as deafult
+            
+            `population` : Number of individual chromosomes. 50 as default. It should be kept as low number if number of possible permutation and combination of feature sets are small.
+            
+            `prob_crossover` : Probability of crossover. 0.9 as default
+            
+            `prob_mutation` : Probability of mutation. 0.1 as default
+                
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+          - **Simulated Annealing Feature Selection (SimulatedAnnealingFS) Parameters**
+            
+            `temperature` : Initial temperature for annealing. Default is 1500
+            
+            `iterations` : Number of times simulated annealing will search for solutions. Default is 100.
+            
+            `n_perturb` : Number of times feature set will be perturbed in an iteration. Default is 1.
+            
+            `n_features_percent_perturb` : Percentage of features that will be perturbed during each perturbation. Value are between 1 and 100.
+            
+            `alpha` : Temperature reduction factor. Defaults is 0.9.
+                
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+          - **Ant Colony Optimization Feature Selection (AntColonyOptimizationFS) Parameters**
+            
+            `iterations` : Number of times ant colony optimization will search for solutions. Default is 100
+            
+            `N_ants` : Number of ants in each iteration. Default is 100.
+        
+            `run_time` : Number of minutes to run the algorithm. This is checked in between each iteration.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from iterations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+            `evaporation_rate` : Evaporation rate. Values are between 0 and 1. If it is too large, chances are higher to find global optima, but computationally expensive. If it is low, chances of finding global optima are less. Default is kept as 0.9
+            
+            `Q` : Pheromene update coefficient. Value between 0 and 1. It affects the convergence speed. If it is large, ACO will get stuck at local optima. Default is kept as 0.2
+        
+          - **Particle Swarm Optimization Feature Selection (ParticleSwarmOptimizationFS) Parameters**
+            
+            `iterations` : Number of times particle swarm optimization will search for solutions. Default is 100.
+            
+            `swarmSize` : Size of the swarm in each iteration. Default is 100.
+            
+            `run_time` : Number of minutes to run the algorithm. This is checked in between generations.
+                At start of each generation it is checked if runtime has exceeded than alloted time.
+                If case run time did exceeds provided limit, best result from generations executed so far is given as output.
+                Default is 2 hours. i.e. 120 minutes.
+        
+        Output
+        ================
+        
+          - **best_columns** : List object with list of column names which gives best performance for the model. These features can be used for training and saving models separately by the user.
+        
+        Examples
+        ================
+        
+         - [Example 1 - Regression](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/main/Chapter%208%20-%20Predicting%20Room%20Bookings%20-%20More%20Genetic%20Algorithm%20Iterations.ipynb)
+         - [Example 2 - Classification](https://github.com/StatguyUser/feature_engineering_and_selection_for_explanable_models/blob/37ba0d2921fbabbb83df44c6eb7a1242b19a637f/Chapter%208%20-%20Hotel%20Cancelation%20.ipynb)
+        
+        How to cite
+        ================
+        Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
+        
+        Where to get it?
+        ================
+        
+        `pip install MetaHeuristicsFS`
+        
+        Dependencies
+        ============
+        
+         - [numpy](https://numpy.org/)
+         - [scikit-learn](https://scikit-learn.org/)
+        
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `MetaHeuristicsFS-0.0.7/LICENSE` & `MetaHeuristicsFS-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MetaHeuristicsFS-0.0.7/setup.py` & `MetaHeuristicsFS-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 else:
     with open('README.rst', encoding='utf-8') as f:
         long_description = f.read()
 
 
 setup(
     name='MetaHeuristicsFS',
-    version='0.0.7',
-    description='Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists`',
+    version='0.0.8',
+    description='Implementation of metaheuristic algorithms for machine learning feature selection. Companion library for the book `Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists`',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='StatguyUser',
     url='https://github.com/StatguyUser/MetaHeuristicsFS',
     install_requires=['numpy','scikit-learn','pandas'],
     download_url='https://github.com/MetaHeuristicsFS/MetaHeuristicsFS.git',
     py_modules=["MetaHeuristicsFS"],
```

