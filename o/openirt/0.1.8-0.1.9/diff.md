# Comparing `tmp/openirt-0.1.8.tar.gz` & `tmp/openirt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.8.tar", last modified: Mon Jul 17 10:18:02 2023, max compression
+gzip compressed data, was "openirt-0.1.9.tar", last modified: Sun Aug  6 08:25:46 2023, max compression
```

## Comparing `openirt-0.1.8.tar` & `openirt-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.822258 openirt-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-17 10:17:41.000000 openirt-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-07-17 10:18:02.822258 openirt-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-17 10:17:41.000000 openirt-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.819258 openirt-0.1.8/openirt/
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/bayes3PL.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3933 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/irt_instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.821258 openirt-0.1.8/openirt/item_models/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6462 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/norm.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl1.py
--rw-rw-rw-   0 root         (0) root         (0)     4592 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl2.py
--rw-rw-rw-   0 root         (0) root         (0)     4379 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/item_models/pl3.py
--rw-rw-rw-   0 root         (0) root         (0)    10759 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mixed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.821258 openirt-0.1.8/openirt/mmle/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mmle/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5523 2023-07-17 10:17:41.000000 openirt-0.1.8/openirt/mmle/generic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.820258 openirt-0.1.8/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-17 10:18:02.000000 openirt-0.1.8/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 10:18:02.822258 openirt-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-17 10:17:41.000000 openirt-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 10:18:02.822258 openirt-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2445 2023-07-17 10:17:41.000000 openirt-0.1.8/tests/test_p1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.337499 openirt-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 08:25:13.000000 openirt-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      236 2023-08-06 08:25:46.337499 openirt-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-06 08:25:13.000000 openirt-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.331507 openirt-0.1.9/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3933 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/irt_instance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.333505 openirt-0.1.9/openirt/item_models/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3679 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/pl2_si.py
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/item_models/pl3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.335502 openirt-0.1.9/openirt/jmle/
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3344 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/pl2_si.py
+-rw-rw-rw-   0 root         (0) root         (0)     4821 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/jmle/pl3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.335502 openirt-0.1.9/openirt/mmle/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/mmle/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5523 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/mmle/dichotomous.py
+-rw-rw-rw-   0 root         (0) root         (0)    11002 2023-08-06 08:25:13.000000 openirt-0.1.9/openirt/mmle/mixed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.332506 openirt-0.1.9/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-08-06 08:25:46.000000 openirt-0.1.9/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-06 08:25:46.000000 openirt-0.1.9/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 08:25:46.000000 openirt-0.1.9/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-06 08:25:46.000000 openirt-0.1.9/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 08:25:46.337499 openirt-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-08-06 08:25:13.000000 openirt-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 08:25:46.337499 openirt-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-08-06 08:25:13.000000 openirt-0.1.9/tests/test_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-08-06 08:25:13.000000 openirt-0.1.9/tests/test_p1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-08-06 08:25:13.000000 openirt-0.1.9/tests/test_pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-08-06 08:25:13.000000 openirt-0.1.9/tests/test_pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2023-08-06 08:25:13.000000 openirt-0.1.9/tests/test_pl3.py
```

### Comparing `openirt-0.1.8/openirt/bayes3PL.py` & `openirt-0.1.9/openirt/bayes3PL.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.8/openirt/cli.py` & `openirt-0.1.9/openirt/cli.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.8/openirt/irt_instance.py` & `openirt-0.1.9/openirt/irt_instance.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.8/openirt/item_models/norm.py` & `openirt-0.1.9/openirt/jmle/pl2_si.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,108 @@
-from model import Model
 import numpy as np
-from scipy.stats import norm
-from typing import Union
+from item_models import PL2
 
-class Norm(Model):
-    def __init__(self):
-        super().__init__(Norm.norm_p, 2, True)
-    
-    @staticmethod
-    def norm_p(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
-        """_summary_
-        takes array of a abilities (n*1) and array of params (2*m) and returns prob (n*m)
-
-        Args:
-            ability (Union[list, np.ndarray, float]): _description_
-            params (Union[list, np.ndarray]): _description_
-
-        Returns:
-            np.ndarray: _description_
-        """
-        ability = np.array(ability)
-        params = np.array(params)
-        z = np.matmul(ability[:, np.newaxis], [params[1]])
-        z += np.tile(params[0], (len(ability), 1))
-        return norm.cdf(z)
-    
-    @staticmethod
-    def __norm_density(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
-        ability = np.array(ability)
-        params = np.array(params)
-        z = np.matmul(ability[:, np.newaxis], [params[1]])
-        z += np.tile(params[0], (len(ability), 1))
-        return norm.pdf(z)
-    
-    @staticmethod
-    def convert_param_form(self, params):
-        return np.array([-params[0] / params[1], 1 / params[1]])
-    
-    def estimate_ability_max_lik(self, params: Union[list, np.ndarray], 
-                         results: Union[list, np.ndarray],
-                         end=0.00000001,
-                         eps=0.01) -> np.ndarray:
-        est = 0.5
-        prev_est = 0
-        while abs(est - prev_est) > end:
-            P = self.prob(est, params)[0]
-            W = (1 - P) * P
-            h = self.norm_density(est, params)[0]
-            prev_est = est
-            denom = np.sum(params[1]**2 * W)
-            if denom < eps or np.any(W < eps):
-                break
-            est = est + (np.sum(params[1] * W  * ((results - P)/ h)) / denom)
-        return est
-    
-    def estimate_item_params_max_lik(self, 
-                            ability: Union[list, np.ndarray], 
-                            result: Union[list, np.ndarray], 
-                            sigm_orig=0,
-                            lamb_orig=1, 
-                            end=0.0000001,  
-                            eps=0.1) -> np.ndarray:
-        ability = np.array(ability)
-        result = np.array(result)
-        est = [sigm_orig, lamb_orig]
-        prev_est = [0, 0]
-        while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
-            P = self.prob(
-                ability, [[est[0]], [est[1]]]).transpose()[0]
-            h = self.norm_density(ability, [[est[0]], [est[1]]]).transpose()[0]
-            W = h**2 / (P * (1 - P))
-            L11 = -np.sum(W)
-            L12 = -np.sum(ability * W)
-            L22 = -np.sum(ability**2 * W)
-            L = np.array([[L11, L12], [L12, L22]])
-
-            if abs(np.linalg.det(L)) < eps:
-                break
-            L_inv = np.linalg.inv(L)
-
-            v = (result - P) / h
-            obs_mat = np.array([np.sum(W * v), np.sum(W * v * ability)])
-            prev_est = est
-            est = est - np.matmul(L_inv, obs_mat)
-        return est
+
+def estimate_ability_max_lik(
+    params: np.ndarray,
+    results: np.ndarray,
+    end=0.00000001,
+    eps=0.01,
+    eps2=0.000001,
+) -> np.ndarray:
+    """
+    Estimate abilities using maximum likelihood estimation.
+
+    Parameters
+    ----------
+        params : np.ndarray
+            Item parameters. Each column is a different item, each row is
+            a different parameter.
+        results : np.ndarray
+            Results. Each row is a different individual, each column is a
+            different item.
+        end : float
+            Convergence threshold.
+        eps : float
+            Threshold for detecting a near-singular matrix.
+        eps2 : float
+            Threshold for detecting small values of P*Q.
+
+    Returns
+    -------
+        np.ndarray
+            Array of abilities.
+    """
+    params = np.array(params)
+    results = np.array(results)
+    est = 0.5
+    prev_est = 0
+    while abs(est - prev_est) > end:
+        P = PL2.pl2_p(est, params)[0]
+        W = (1 - P) * P
+        denom = np.sum(params[1] ** 2 * W)
+        if abs(denom) < eps or np.any(np.abs(W) < eps2):
+            print('break1')
+            break
+        prev_est = est
+        est = est + (np.sum(params[1] * W * ((results - P) / W)) / denom)
+    return est
+
+
+def estimate_item_params_max_lik(
+    ability: np.ndarray,
+    result: np.ndarray,
+    sigm_orig=-1,
+    lamb_orig=1,
+    end=0.00001,
+    eps=0.0001,
+) -> np.ndarray:
+    """
+    Estimate item parameters using maximum likelihood estimation.
+
+    Parameters
+    ----------
+        ability : np.ndarray
+            Array of abilities.
+        result : np.ndarray
+            Results. Each row is a different individual, each column is a
+            different item.
+        sigm_orig : float
+            Initial value for the discrimination parameter.
+        lamb_orig : float
+            Initial value for the difficulty parameter.
+        end : float
+            Convergence threshold.
+        eps : float
+            Threshold for detecting a near-singular matrix.
+
+    Returns
+    -------
+        np.ndarray
+            Array of item parameters.
+    """
+    ability = np.array(ability)
+    result = np.array(result)
+    est = [sigm_orig, lamb_orig]
+    prev_est = [0, 0]
+    i = 0
+    while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
+        P = PL2.pl2_p(ability, [[est[0]], [est[1]]]).transpose()[0]
+        W = P * (1 - P)
+        L11 = -np.sum(W)
+        L12 = -np.sum(ability * W)
+        L22 = -np.sum(ability**2 * W)
+        L = np.array([[L11, L12], [L12, L22]])
+        print(est)
+        if abs(np.linalg.det(L)) < eps:
+            # print(f'break2: {abs(np.linalg.det(L))}')
+            # break
+            L += np.identity(2) * 1e-6
+        L_inv = np.linalg.inv(L)
+
+        obs_mat = np.array([np.sum(result - P), np.sum((result - P) * ability)])
+        prev_est = est
+        est = est - np.matmul(L_inv, obs_mat)
+        i += 1
+        if i > 10000:
+            break
+    return est
```

### Comparing `openirt-0.1.8/openirt/item_models/pl1.py` & `openirt-0.1.9/openirt/jmle/pl1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,72 @@
-from model import Model
 import numpy as np
-from pl2 import PL2
+from item_models import Model, PL1
+from jmle.pl2 import estimate_ability_max_lik as pl2_estimate_ability_max_lik
 
 
-class PL1(Model):
+def estimate_ability_max_lik(
+    params: np.ndarray,
+    results: np.ndarray,
+    end=0.00000001,
+    eps=0.01,
+    eps2=0.000001,
+) -> np.ndarray:
     """
-    1-parameter logistic model (Rasch model).
-    p(\\theta) = 1 / (1 + e^{-(\\zeta + \\theta)}
+    Estimate abilities using the maximum likelihood method.
+    See Model.estimate_ability_max_lik and PL2.estimate_ability_max_lik.
     """
-    def __init__(self):
-        super().__init__(
-            PL1.pl1_p,
-            num_params=1,
-            multi=True,
-            prov_params=[0],
-            loc_param=0,
-            param_bounds=[(-7, 7)],
-            loc_param_asc=False,
-        )
-
-    @staticmethod
-    def pl1_p(
-        ability: np.ndarray, 
-        params: np.ndarray
-    ) -> np.ndarray:
-        """
-        Probability of a correct response given the ability and item 
-        parameters.
-
-        Args:
-            ability : np.ndarray 
-                Array of abilities.
-            params : np.ndarray
-                Item parameters. Item parameters. Each column is a different
-                item, each row is a different parameter.
-
-        Returns:
-            np.ndarray: Array of probabilities. Each row is a different
-            individual, each column is a different item.
-        """
-        return PL2().pl2_p(ability, [params[0], np.ones(len(params[0]))])
-
-    def estimate_ability_max_lik(
-        self,
-        params: Union[list, np.ndarray],
-        results: Union[list, np.ndarray],
-        end=0.00000001,
-        eps=0.01,
-        eps2=0.000001,
-    ) -> np.ndarray:
-        """
-        Estimate the ability of an individual given the item parameters and responses.
-
-        Args:
-            params: A list or numpy array representing the item parameters.
-            results: A list or numpy array representing the item responses.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
-
-        Returns:
-            A numpy array representing the estimated ability.
-        """
-        return PL2().estimate_ability_max_lik(
-            [params[0], np.ones(len(params[0]))], results, end, eps, eps2
-        )
-
-    def estimate_item_params_max_lik(
-        self,
-        ability: Union[list, np.ndarray],
-        result: Union[list, np.ndarray],
-        sigm_orig=0,
-        end=0.0000001,
-        eps=0.0001,
-    ) -> np.ndarray:
-        """
-        Estimate the parameters of the model given the abilities and item responses.
-
-        Args:
-            ability: A list or numpy array containing the abilities of individuals.
-            result: A list or numpy array representing the item responses.
-            sigm_orig: The initial value for the parameter sigm.
-            end: The convergence threshold.
-            eps: The threshold for detecting a near-singular matrix.
-
-        Returns:
-            A numpy array representing the estimated parameters.
-        """
-        ability = np.array(ability)
-        result = np.array(result)
-        est = sigm_orig
-        prev_est = est + 2 * end
-        while abs(est - prev_est) > end:
-            P = self.pl1_p(ability, [[est]]).transpose()[0]
-            L1 = np.sum(result - P)
-            L2 = -np.sum(P * (1 - P))
-
-            if abs(L2) < eps:
-                break
-
-            prev_est = est
-            est = est - L1 / L2
-        return np.array([est])
+    return pl2_estimate_ability_max_lik(
+        [params[0], np.ones(len(params[0]))], results, end, eps, eps2
+    )
+
+
+def estimate_item_params_max_lik(
+    model: Model,
+    ability: np.ndarray,
+    result: np.ndarray,
+    sigm_orig=0,
+    end=1e-10,
+    eps=1e-10,
+) -> np.ndarray:
+    """
+    Estimate item parameters using maximum likelihood estimation.
+
+    Parameters
+    ----------
+        model : Model
+            Instance of PL1 model.
+        ability : np.ndarray
+            Array of abilities.
+        result : np.ndarray
+            Results. Each row is a different individual, each column is a
+            different item.
+        sigm_orig : float
+            Initial value for the discrimination parameter.
+        lamb_orig : float
+            Initial value for the difficulty parameter.
+        end : float
+            Convergence threshold.
+        eps : float
+            Threshold for detecting a near-singular matrix.
+
+    Returns
+    -------
+        np.ndarray
+            Array of item parameters.
+    """
+    ability = np.array(ability)
+    result = np.array(result)
+    est = sigm_orig
+    prev_est = est + 2 * end
+    while abs(est - prev_est) > end:
+        P = PL1.pl1_p(ability, [[est]]).transpose()[0]
+        L1 = np.sum(P - result)
+        L2 = -np.sum(P * (1 - P))
+        if abs(L2) < eps:
+            L += 1e-10
+        prev_est = est
+        est = est - L1 / L2
+        
+        # enforce bounds
+        est = model.param_bounds[0][0] if est < model.param_bounds[0][0] else est
+        est = model.param_bounds[0][1] if est > model.param_bounds[0][1] else est
+    return np.array([est])
```

### Comparing `openirt-0.1.8/openirt/mixed.py` & `openirt-0.1.9/openirt/mmle/mixed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import numpy as np
 from item_models import PL1, PL2, PL3
 from scipy.stats import norm
 import scipy.integrate as integrate
 from scipy.optimize import minimize
 import matplotlib.pyplot as plt
 
+
 # mention: we assume there is some sort of location param.
 # For graded models we must also assume icc is increasing, so we place bounds
-class Mixed():
-    def __init__(self, 
-                 responses, 
-                 categories,
-                 models, 
-                 prov_params=None,
-                 param_bounds=None,
-                 loc_param_idx=None,
-                 loc_param_asc=None) -> None:
+class Mixed:
+    def __init__(
+        self,
+        responses,
+        categories,
+        models,
+        prov_params=None,
+        param_bounds=None,
+        loc_param_idx=None,
+        loc_param_asc=None,
+    ) -> None:
         # loc_param asc is a list of booleans, corresponding to each item. The boolean is 'True' if a higher location
         # corresponds to a more difficult item.
         self.responses = responses
         self.num_subjects, self.num_items = responses.shape
         self.categories = categories
         self.models = models
-        self.grouped_resp, self.group_idxs, self.group_count= self._group_subjects(responses)
+        self.grouped_resp, self.group_idxs, self.group_count = self._group_subjects(
+            responses
+        )
         self.set_loc_params(loc_param_idx)
         self.ability_distr = lambda ability: norm.pdf(ability)
         self.set_param_bounds(param_bounds)
         self.set_loc_param_asc(loc_param_asc)
         self.set_prov_params(prov_params)
 
         # print(self.condit_prob_of_indiv_resp(params=self.prov_params, item=0, resp=1, ability=0.4))
-        
-        
+
     def set_loc_params(self, loc_param):
         # if None, we assume all models either:
         # - are predefined (pl1-pl3, norm)
         # - only have one parameter
         # With this assumption we can construct this object
         # This can be given in the solve step instead of constructor..?
         if loc_param is None:
@@ -43,35 +47,45 @@
             for m in self.models:
                 if m.loc_param is not None:
                     self.loc_params.append(m.loc_param)
                 else:
                     self.loc_params.append(0)
         else:
             self.loc_params = loc_param
-            
+
     def set_prov_params(self, prov_params):
         self.prov_params = []
         if prov_params is None:
             for i, m in enumerate(self.models):
                 if m.prov_params:
-                    self.prov_params.append(np.tile(m.prov_params, (self.categories[i]-1, 1)).T.astype(float))
-                    
+                    self.prov_params.append(
+                        np.tile(m.prov_params, (self.categories[i] - 1, 1)).T.astype(
+                            float
+                        )
+                    )
+
                     # distribute location parameters (assuming bounds exist)
                     lower_bound = self.param_bounds[i][self.loc_params[i]][0]
                     upper_bound = self.param_bounds[i][self.loc_params[i]][1]
                     if self.loc_param_asc[i]:
-                        self.prov_params[i][self.loc_params[i]] = np.linspace(lower_bound, upper_bound, self.categories[i]+1)[1:-1]
+                        self.prov_params[i][self.loc_params[i]] = np.linspace(
+                            lower_bound, upper_bound, self.categories[i] + 1
+                        )[1:-1]
                     else:
-                        self.prov_params[i][self.loc_params[i]] = np.linspace(upper_bound, lower_bound, self.categories[i]+1)[1:-1]
+                        self.prov_params[i][self.loc_params[i]] = np.linspace(
+                            upper_bound, lower_bound, self.categories[i] + 1
+                        )[1:-1]
                 else:
                     raise ValueError('"prov_params" is None')
         else:
             for i, p in enumerate(prov_params):
-                self.prov_params.append(np.tile(p, (self.categories[i]-1, 1)).T.astype(float))
-                
+                self.prov_params.append(
+                    np.tile(p, (self.categories[i] - 1, 1)).T.astype(float)
+                )
+
     def set_param_bounds(self, param_bounds):
         # if none, we assume that all items have attribute, or we dont use bounds
         if param_bounds is None:
             self.param_bounds = []
             for m in self.models:
                 if m.param_bounds is not None:
                     self.param_bounds.append(m.param_bounds)
@@ -82,165 +96,182 @@
 
     def set_loc_param_asc(self, loc_param_asc):
         if loc_param_asc is None:
             self.loc_param_asc = []
             for m in self.models:
                 if m.loc_param_asc is not None:
                     self.loc_param_asc.append(m.loc_param_asc)
-                else: 
+                else:
                     self.loc_param_asc.append(True)
         else:
             self.loc_param_asc = loc_param_asc
-            
 
     def _group_subjects(self, responses):
         return np.unique(responses, axis=0, return_inverse=True, return_counts=True)
 
     # P*_{i,k}(\theta)
     # 1 when k = -1
     # 0 when k = m-1 ?
     def boundary_prob(self, params, item, resp, ability):
         # resp is single resp
         if resp == -1:
             return 1
         if resp == self.categories[item] - 1:
             return 0
-        temp_params = params[item][:,resp].reshape(self.models[item].num_params, 1)
+        temp_params = params[item][:, resp].reshape(self.models[item].num_params, 1)
         return self.models[item].p([ability], temp_params)[0][0]
-    
+
     # P(U_{li}|\theta) = P(U_{li} = k|\theta) = P_{ik}(\theta) = P*_{i,k-1}(\theta) - P*_{ik}(\theta)
     def condit_prob_of_indiv_resp(self, params, resp, item, ability):
         # resp is single resp
-        return max(self.boundary_prob(params, item, resp - 1, ability) - self.boundary_prob(params, item, resp, ability), 1e-3)
-    
+        return max(
+            self.boundary_prob(params, item, resp - 1, ability)
+            - self.boundary_prob(params, item, resp, ability),
+            1e-3,
+        )
+
     # P(U_l|\theta) = \prod_{i=1}^n P(U_{li}|\theta)
     def condit_prob_of_resp_vect(self, params, resp, ability):
-        return np.prod([self.condit_prob_of_indiv_resp(params, u, i, ability) for i, u in enumerate(resp)])
-    
+        return np.prod(
+            [
+                self.condit_prob_of_indiv_resp(params, u, i, ability)
+                for i, u in enumerate(resp)
+            ]
+        )
+
     # P(U_l) = \int P(U_l|\theta) \pi(\theta) d\theta
     def marginal_prob_of_resp(self, params, resp):
-        integrand = lambda ability: self.condit_prob_of_resp_vect(params, resp, ability) * self.ability_distr(ability)
+        integrand = lambda ability: self.condit_prob_of_resp_vect(
+            params, resp, ability
+        ) * self.ability_distr(ability)
         result, _ = integrate.quad(integrand, -7, 7, epsabs=1e-3, epsrel=1e-3)
         return result
-    
+
     # L = \sum_{l=1}^{L} r_l \log{P(U_l)}
     def log_likelihood(self, params):
-        marg_p = np.array([self.marginal_prob_of_resp(params, resp) for resp in self.grouped_resp])
+        marg_p = np.array(
+            [self.marginal_prob_of_resp(params, resp) for resp in self.grouped_resp]
+        )
         if np.any(marg_p <= 0):
             return -np.inf
         return np.sum(self.group_count * np.log(marg_p))
-    
+
     def loc_param_bounds(self, params, item, param_type_idx, boundary_idx):
         tot_lower_bound = self.param_bounds[item][param_type_idx][0]
         tot_upper_bound = self.param_bounds[item][param_type_idx][1]
         if self.loc_param_asc[item]:
             # lower bound
             if boundary_idx == 0:
                 lower = tot_lower_bound
             else:
-                lower = params[item][param_type_idx][boundary_idx-1]
+                lower = params[item][param_type_idx][boundary_idx - 1]
             # upper bound
             if boundary_idx == self.categories[item] - 2:
                 upper = tot_upper_bound
             else:
-                upper = params[item][param_type_idx][boundary_idx+1]
+                upper = params[item][param_type_idx][boundary_idx + 1]
         else:
             # lower bound
             if boundary_idx == self.categories[item] - 2:
                 lower = tot_lower_bound
             else:
-                lower = params[item][param_type_idx][boundary_idx+1]
+                lower = params[item][param_type_idx][boundary_idx + 1]
             # upper bound
             if boundary_idx == 0:
                 upper = tot_upper_bound
             else:
-                upper = params[item][param_type_idx][boundary_idx-1]
+                upper = params[item][param_type_idx][boundary_idx - 1]
         return lower, upper
-        
+
     def maximize_log_lik_loc(self, params, item, param_type_idx, boundary_idx):
         initial_guess = params[item][param_type_idx][boundary_idx]
+
         def obj_func(x):
             params[item][param_type_idx][boundary_idx] = x
             return -self.log_likelihood(params)
-        result = minimize(obj_func,
-                          initial_guess,
-                          bounds=[self.loc_param_bounds(params, item, param_type_idx, boundary_idx)],
-                          tol=1e-3)
+
+        result = minimize(
+            obj_func,
+            initial_guess,
+            bounds=[self.loc_param_bounds(params, item, param_type_idx, boundary_idx)],
+            tol=1e-3,
+        )
         return result.x[0], -result.fun
-            
+
     def maximize_log_lik(self, params, item, param_type_idx):
         initial_guess = params[item][param_type_idx][0]
+
         def obj_func(x):
             params[item][param_type_idx] = x
             return -self.log_likelihood(params)
-        result = minimize(obj_func,
-                          initial_guess,
-                          bounds=[self.param_bounds[item][param_type_idx]],
-                          tol=1e-3)
+
+        result = minimize(
+            obj_func,
+            initial_guess,
+            bounds=[self.param_bounds[item][param_type_idx]],
+            tol=1e-3,
+        )
         return result.x[0], -result.fun
 
-    def em_mmle(self, eps=0.01):
-        params = self.prov_params.copy() 
+    def em_mmle(self, eps=0.1):
+        params = self.prov_params.copy()
         prev_log_L = -np.inf
         log_L = self.log_likelihood(params)
-        while log_L - prev_log_L > eps:
-            print(f'prev log L: {prev_log_L}')
-            print(f'log L: {log_L}')
+        while abs(log_L - prev_log_L) > eps:
+            print(f"prev log L: {prev_log_L}")
+            print(f"log L: {log_L}")
             prev_log_L = log_L
             for i in range(len(params)):
                 # item_params are all parameters for item i
                 for param_type_idx in range(self.models[i].num_params):
                     # param_type are the same type of parameters for i, e.g. all the betas
                     if param_type_idx == self.loc_params[i]:
                         # optimize all location params separately
                         for k in range(self.categories[i] - 1):
-                            print(f'maximizing item {i}, {param_type_idx}th parameter, where k={k}')
-                            new_param, log_L = self.maximize_log_lik_loc(params, i, param_type_idx, k)
+                            print(
+                                f"maximizing item {i}, {param_type_idx}th parameter, where k={k}"
+                            )
+                            new_param, log_L = self.maximize_log_lik_loc(
+                                params, i, param_type_idx, k
+                            )
                     else:
-                        print(f'maximizing item {i}, {param_type_idx}th parameter, (all k)')
-                        new_param, log_L = self.maximize_log_lik(params, i, param_type_idx)
+                        print(
+                            f"maximizing item {i}, {param_type_idx}th parameter, (all k)"
+                        )
+                        new_param, log_L = self.maximize_log_lik(
+                            params, i, param_type_idx
+                        )
         return params
-    
+
     # \bar(\theta_l) = \frac{\int \theta P(U_l|\theta) \pi(\theta) d\theta}{P(U_l)}
     def estimate_ability_post_mean(self, params, group):
-        integrand = lambda ability: self.condit_prob_of_resp_vect(params, self.grouped_resp[group], ability) * self.ability_distr(ability) * ability
+        integrand = (
+            lambda ability: self.condit_prob_of_resp_vect(
+                params, self.grouped_resp[group], ability
+            )
+            * self.ability_distr(ability)
+            * ability
+        )
         numer, _ = integrate.quad(integrand, -7, 7, epsabs=1e-3, epsrel=1e-3)
         denom = self.marginal_prob_of_resp(params, self.grouped_resp[group])
         return numer / denom
-        
+    
+    def estimate_abilities_post_mean(self, params):
+        abilities = np.array([self.estimate_ability_post_mean(params, group) for group in range(len(self.grouped_resp))])
+        abilities = abilities[self.group_idxs]
+        return abilities
+
     def plot_boundaries(self, params, i):
         ability = np.linspace(-5, 5)
         for k, param in enumerate(params[i].T):
-            prob = self.models[i].p(ability, param.reshape(models[i].num_params,1))
-            plt.plot(ability, prob, label=f'P*_{k}')
+            prob = self.models[i].p(ability, param.reshape(self.models[i].num_params, 1))
+            plt.plot(ability, prob, label=f"P*_{k}")
         plt.legend()
         plt.show()
-    
+
     def plot_irccc(self, params, i):
         ability = np.linspace(-5, 5)
-        for k in range(categories[i]):
+        for k in range(self.categories[i]):
             prob = [self.condit_prob_of_indiv_resp(params, k, i, ab) for ab in ability]
-            plt.plot(ability, prob, label=f'P_{k}')
+            plt.plot(ability, prob, label=f"P_{k}")
         plt.legend()
         plt.show()
-
-# important to clean data, eliminate options that arent chosen
-responses = np.array([[0, 0],
-                      [1, 3],
-                      [2, 1],
-                      [1, 2]])
-
-categories = (3, 4)
-models = (PL2(), PL1())
-
-mixed = Mixed(responses, categories, models)
-
-
-par = [np.array([[ 1.2990496 , -1.55895654],
-       [ 1.32044104,  1.32044104]]), np.array([[ 1.17551977, -0.17228615, -1.37332456]])]
-print(mixed.estimate_ability_post_mean(par, 2))
-
-def p_category(i, ablility):
-    # returns array with probability of each category
-    pass
-
-
```

### Comparing `openirt-0.1.8/openirt/mmle/generic.py` & `openirt-0.1.9/openirt/mmle/dichotomous.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.8/setup.py` & `openirt-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     ) as fp:
         return fp.read()
 
 setup(
     name='openirt',
     packages = find_packages(include=['openirt', 
                                       'openirt.item_models', 
-                                      'openirt.mmle']),
+                                      'openirt.mmle',
+                                      'openirt.jmle']),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
-    url='https://gitlab.com/pleased/...',
-    version='0.1.8',
+    url='https://gitlab.com/pleased/item-response-theory-toolkit',
+    version='0.1.9',
     description='Item response theory toolkit',
     author='Johan Hay',
-    license='MIT',
+    license='',
 )
```

