# Comparing `tmp/alns-5.3.1.tar.gz` & `tmp/alns-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alns-5.3.1.tar", max compression
+gzip compressed data, was "alns-5.3.2.tar", max compression
```

## Comparing `alns-5.3.1.tar` & `alns-5.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1095 2023-08-03 21:30:16.787223 alns-5.3.1/LICENSE.md
--rw-r--r--   0        0        0     5673 2023-08-03 21:30:16.787223 alns-5.3.1/README.md
--rw-r--r--   0        0        0    11416 2023-08-03 21:30:16.787223 alns-5.3.1/alns/ALNS.py
--rw-r--r--   0        0        0      495 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Outcome.py
--rw-r--r--   0        0        0     5366 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Result.py
--rw-r--r--   0        0        0      637 2023-08-03 21:30:16.787223 alns-5.3.1/alns/State.py
--rw-r--r--   0        0        0     3975 2023-08-03 21:30:16.787223 alns-5.3.1/alns/Statistics.py
--rw-r--r--   0        0        0       89 2023-08-03 21:30:16.787223 alns-5.3.1/alns/__init__.py
--rw-r--r--   0        0        0      885 2023-08-03 21:30:16.787223 alns-5.3.1/alns/accept/AcceptanceCriterion.py
--rw-r--r--   0        0        0     2274 2023-08-03 21:30:16.787223 alns-5.3.1/alns/accept/AdaptiveThreshold.py
--rw-r--r--   0        0        0     1855 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/GreatDeluge.py
--rw-r--r--   0        0        0      276 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/HillClimbing.py
--rw-r--r--   0        0        0     2481 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/LateAcceptanceHillClimbing.py
--rw-r--r--   0        0        0     3543 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/NonLinearGreatDeluge.py
--rw-r--r--   0        0        0      179 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/RandomWalk.py
--rw-r--r--   0        0        0     6080 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/RecordToRecordTravel.py
--rw-r--r--   0        0        0     6398 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/SimulatedAnnealing.py
--rw-r--r--   0        0        0     2214 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/WorseAccept.py
--rw-r--r--   0        0        0      478 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/__init__.py
--rw-r--r--   0        0        0     4170 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_adaptive_threshold.py
--rw-r--r--   0        0        0     2311 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_great_deluge.py
--rw-r--r--   0        0        0      820 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_hill_climbing.py
--rw-r--r--   0        0        0     6012 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_late_acceptance_hill_climbing.py
--rw-r--r--   0        0        0     3452 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_non_linear_great_deluge.py
--rw-r--r--   0        0        0      790 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_random_walk.py
--rw-r--r--   0        0        0     5022 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_record_to_record_travel.py
--rw-r--r--   0        0        0     7119 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_simulated_annealing.py
--rw-r--r--   0        0        0     1947 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_threshold_accept.py
--rw-r--r--   0        0        0     1161 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_update.py
--rw-r--r--   0        0        0     4361 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/tests/test_worse_accept.py
--rw-r--r--   0        0        0      906 2023-08-03 21:30:16.791223 alns-5.3.1/alns/accept/update.py
--rw-r--r--   0        0        0     5247 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/AlphaUCB.py
--rw-r--r--   0        0        0     6462 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/MABSelector.py
--rw-r--r--   0        0        0     3516 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/OperatorSelectionScheme.py
--rw-r--r--   0        0        0      635 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/RandomSelect.py
--rw-r--r--   0        0        0     5090 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/RouletteWheel.py
--rw-r--r--   0        0        0     3598 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/SegmentedRouletteWheel.py
--rw-r--r--   0        0        0      268 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/__init__.py
--rw-r--r--   0        0        0     2358 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_alpha_ucb.py
--rw-r--r--   0        0        0     4379 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_mab_selector.py
--rw-r--r--   0        0        0     2180 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_random_select.py
--rw-r--r--   0        0        0     3871 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_roulette_wheel.py
--rw-r--r--   0        0        0     2754 2023-08-03 21:30:16.791223 alns-5.3.1/alns/select/tests/test_segmented_roulette_wheel.py
--rw-r--r--   0        0        0      842 2023-08-03 21:30:16.791223 alns-5.3.1/alns/show_versions.py
--rw-r--r--   0        0        0      663 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/MaxIterations.py
--rw-r--r--   0        0        0      769 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/MaxRuntime.py
--rw-r--r--   0        0        0     1013 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/NoImprovement.py
--rw-r--r--   0        0        0      669 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      166 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/__init__.py
--rw-r--r--   0        0        0     1290 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_max_iterations.py
--rw-r--r--   0        0        0     1811 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_max_runtime.py
--rw-r--r--   0        0        0     2431 2023-08-03 21:30:16.791223 alns-5.3.1/alns/stop/tests/test_no_improvement.py
--rw-r--r--   0        0        0        0 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/__init__.py
--rw-r--r--   0        0        0      385 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/conftest.py
--rw-r--r--   0        0        0      834 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/states.py
--rw-r--r--   0        0        0    10367 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_alns.py
--rw-r--r--   0        0        0     6962 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_result.py
--rw-r--r--   0        0        0     2796 2023-08-03 21:30:16.791223 alns-5.3.1/alns/tests/test_statistics.py
--rw-r--r--   0        0        0     3032 2023-08-03 21:30:16.815223 alns-5.3.1/pyproject.toml
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 alns-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-08-06 10:25:04.187848 alns-5.3.2/LICENSE.md
+-rw-r--r--   0        0        0     5673 2023-08-06 10:25:04.187848 alns-5.3.2/README.md
+-rw-r--r--   0        0        0    11416 2023-08-06 10:25:04.187848 alns-5.3.2/alns/ALNS.py
+-rw-r--r--   0        0        0      495 2023-08-06 10:25:04.187848 alns-5.3.2/alns/Outcome.py
+-rw-r--r--   0        0        0     5366 2023-08-06 10:25:04.187848 alns-5.3.2/alns/Result.py
+-rw-r--r--   0        0        0      637 2023-08-06 10:25:04.187848 alns-5.3.2/alns/State.py
+-rw-r--r--   0        0        0     3975 2023-08-06 10:25:04.187848 alns-5.3.2/alns/Statistics.py
+-rw-r--r--   0        0        0      116 2023-08-06 10:25:04.187848 alns-5.3.2/alns/__init__.py
+-rw-r--r--   0        0        0      885 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/AcceptanceCriterion.py
+-rw-r--r--   0        0        0     2274 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/AdaptiveThreshold.py
+-rw-r--r--   0        0        0     1855 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/GreatDeluge.py
+-rw-r--r--   0        0        0      276 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/HillClimbing.py
+-rw-r--r--   0        0        0     2481 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/LateAcceptanceHillClimbing.py
+-rw-r--r--   0        0        0     3543 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/NonLinearGreatDeluge.py
+-rw-r--r--   0        0        0      179 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/RandomWalk.py
+-rw-r--r--   0        0        0     6080 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/RecordToRecordTravel.py
+-rw-r--r--   0        0        0     6398 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/SimulatedAnnealing.py
+-rw-r--r--   0        0        0     2214 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/WorseAccept.py
+-rw-r--r--   0        0        0      478 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/__init__.py
+-rw-r--r--   0        0        0     4170 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_adaptive_threshold.py
+-rw-r--r--   0        0        0     2311 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_great_deluge.py
+-rw-r--r--   0        0        0      820 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_hill_climbing.py
+-rw-r--r--   0        0        0     6012 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_late_acceptance_hill_climbing.py
+-rw-r--r--   0        0        0     3452 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_non_linear_great_deluge.py
+-rw-r--r--   0        0        0      790 2023-08-06 10:25:04.187848 alns-5.3.2/alns/accept/tests/test_random_walk.py
+-rw-r--r--   0        0        0     5022 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/tests/test_record_to_record_travel.py
+-rw-r--r--   0        0        0     7119 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/tests/test_simulated_annealing.py
+-rw-r--r--   0        0        0     1947 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/tests/test_threshold_accept.py
+-rw-r--r--   0        0        0     1161 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/tests/test_update.py
+-rw-r--r--   0        0        0     4361 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/tests/test_worse_accept.py
+-rw-r--r--   0        0        0      906 2023-08-06 10:25:04.191848 alns-5.3.2/alns/accept/update.py
+-rw-r--r--   0        0        0     5247 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/AlphaUCB.py
+-rw-r--r--   0        0        0     6462 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/MABSelector.py
+-rw-r--r--   0        0        0     3516 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/OperatorSelectionScheme.py
+-rw-r--r--   0        0        0      635 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/RandomSelect.py
+-rw-r--r--   0        0        0     5090 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/RouletteWheel.py
+-rw-r--r--   0        0        0     3598 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/SegmentedRouletteWheel.py
+-rw-r--r--   0        0        0      268 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/__init__.py
+-rw-r--r--   0        0        0     2358 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/test_alpha_ucb.py
+-rw-r--r--   0        0        0     4379 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/test_mab_selector.py
+-rw-r--r--   0        0        0     2180 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/test_random_select.py
+-rw-r--r--   0        0        0     3871 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/test_roulette_wheel.py
+-rw-r--r--   0        0        0     2754 2023-08-06 10:25:04.191848 alns-5.3.2/alns/select/tests/test_segmented_roulette_wheel.py
+-rw-r--r--   0        0        0      842 2023-08-06 10:25:04.191848 alns-5.3.2/alns/show_versions.py
+-rw-r--r--   0        0        0      663 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/MaxIterations.py
+-rw-r--r--   0        0        0      769 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/MaxRuntime.py
+-rw-r--r--   0        0        0     1013 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/NoImprovement.py
+-rw-r--r--   0        0        0      669 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      166 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/tests/test_max_iterations.py
+-rw-r--r--   0        0        0     1811 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/tests/test_max_runtime.py
+-rw-r--r--   0        0        0     2431 2023-08-06 10:25:04.191848 alns-5.3.2/alns/stop/tests/test_no_improvement.py
+-rw-r--r--   0        0        0        0 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/conftest.py
+-rw-r--r--   0        0        0      834 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/states.py
+-rw-r--r--   0        0        0    10367 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/test_alns.py
+-rw-r--r--   0        0        0     6962 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/test_result.py
+-rw-r--r--   0        0        0     2796 2023-08-06 10:25:04.191848 alns-5.3.2/alns/tests/test_statistics.py
+-rw-r--r--   0        0        0     3032 2023-08-06 10:25:04.207848 alns-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 alns-5.3.2/PKG-INFO
```

### Comparing `alns-5.3.1/LICENSE.md` & `alns-5.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/README.md` & `alns-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/ALNS.py` & `alns-5.3.2/alns/ALNS.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/Result.py` & `alns-5.3.2/alns/Result.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/State.py` & `alns-5.3.2/alns/State.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/Statistics.py` & `alns-5.3.2/alns/Statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/AcceptanceCriterion.py` & `alns-5.3.2/alns/accept/AcceptanceCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/AdaptiveThreshold.py` & `alns-5.3.2/alns/accept/AdaptiveThreshold.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/GreatDeluge.py` & `alns-5.3.2/alns/accept/GreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/LateAcceptanceHillClimbing.py` & `alns-5.3.2/alns/accept/LateAcceptanceHillClimbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/NonLinearGreatDeluge.py` & `alns-5.3.2/alns/accept/NonLinearGreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/RecordToRecordTravel.py` & `alns-5.3.2/alns/accept/RecordToRecordTravel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/SimulatedAnnealing.py` & `alns-5.3.2/alns/accept/SimulatedAnnealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/WorseAccept.py` & `alns-5.3.2/alns/accept/WorseAccept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_adaptive_threshold.py` & `alns-5.3.2/alns/accept/tests/test_adaptive_threshold.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_great_deluge.py` & `alns-5.3.2/alns/accept/tests/test_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_hill_climbing.py` & `alns-5.3.2/alns/accept/tests/test_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_late_acceptance_hill_climbing.py` & `alns-5.3.2/alns/accept/tests/test_late_acceptance_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_non_linear_great_deluge.py` & `alns-5.3.2/alns/accept/tests/test_non_linear_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_random_walk.py` & `alns-5.3.2/alns/accept/tests/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_record_to_record_travel.py` & `alns-5.3.2/alns/accept/tests/test_record_to_record_travel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_simulated_annealing.py` & `alns-5.3.2/alns/accept/tests/test_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_threshold_accept.py` & `alns-5.3.2/alns/accept/tests/test_threshold_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_update.py` & `alns-5.3.2/alns/accept/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/tests/test_worse_accept.py` & `alns-5.3.2/alns/accept/tests/test_worse_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/accept/update.py` & `alns-5.3.2/alns/accept/update.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/AlphaUCB.py` & `alns-5.3.2/alns/select/AlphaUCB.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/MABSelector.py` & `alns-5.3.2/alns/select/MABSelector.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/OperatorSelectionScheme.py` & `alns-5.3.2/alns/select/OperatorSelectionScheme.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/RandomSelect.py` & `alns-5.3.2/alns/select/RandomSelect.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/RouletteWheel.py` & `alns-5.3.2/alns/select/RouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/SegmentedRouletteWheel.py` & `alns-5.3.2/alns/select/SegmentedRouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/tests/test_alpha_ucb.py` & `alns-5.3.2/alns/select/tests/test_alpha_ucb.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/tests/test_mab_selector.py` & `alns-5.3.2/alns/select/tests/test_mab_selector.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/tests/test_random_select.py` & `alns-5.3.2/alns/select/tests/test_random_select.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/tests/test_roulette_wheel.py` & `alns-5.3.2/alns/select/tests/test_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/select/tests/test_segmented_roulette_wheel.py` & `alns-5.3.2/alns/select/tests/test_segmented_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/show_versions.py` & `alns-5.3.2/alns/show_versions.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/MaxIterations.py` & `alns-5.3.2/alns/stop/MaxIterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/MaxRuntime.py` & `alns-5.3.2/alns/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/NoImprovement.py` & `alns-5.3.2/alns/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/StoppingCriterion.py` & `alns-5.3.2/alns/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/tests/test_max_iterations.py` & `alns-5.3.2/alns/stop/tests/test_max_iterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/tests/test_max_runtime.py` & `alns-5.3.2/alns/stop/tests/test_max_runtime.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/stop/tests/test_no_improvement.py` & `alns-5.3.2/alns/stop/tests/test_no_improvement.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/tests/states.py` & `alns-5.3.2/alns/tests/states.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/tests/test_alns.py` & `alns-5.3.2/alns/tests/test_alns.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/tests/test_result.py` & `alns-5.3.2/alns/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/alns/tests/test_statistics.py` & `alns-5.3.2/alns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.3.1/pyproject.toml` & `alns-5.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alns"
-version = "5.3.1"
+version = "5.3.2"
 description = "A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/ALNS"
 include = [
     "LICENSE.md",
```

### Comparing `alns-5.3.1/PKG-INFO` & `alns-5.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alns
-Version: 5.3.1
+Version: 5.3.2
 Summary: A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.
 Home-page: https://github.com/N-Wouda/ALNS
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

