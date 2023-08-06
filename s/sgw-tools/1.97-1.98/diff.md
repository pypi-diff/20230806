# Comparing `tmp/sgw_tools-1.97.tar.gz` & `tmp/sgw_tools-1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.97.tar", last modified: Sun Aug  6 12:30:17 2023, max compression
+gzip compressed data, was "sgw_tools-1.98.tar", last modified: Sun Aug  6 13:54:26 2023, max compression
```

## Comparing `sgw_tools-1.97.tar` & `sgw_tools-1.98.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 12:29:38.000000 sgw_tools-1.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:30:17.395610 sgw_tools-1.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-06 12:29:38.000000 sgw_tools-1.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:30:17.395610 sgw_tools-1.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 12:29:38.000000 sgw_tools-1.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:29:38.000000 sgw_tools-1.97/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-08-06 12:29:38.000000 sgw_tools-1.97/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.811122 sgw_tools-1.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 13:53:47.000000 sgw_tools-1.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 13:54:26.807122 sgw_tools-1.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-06 13:53:47.000000 sgw_tools-1.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:54:26.811122 sgw_tools-1.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 13:53:47.000000 sgw_tools-1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:53:47.000000 sgw_tools-1.98/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-08-06 13:53:47.000000 sgw_tools-1.98/tests/test_biggraph.py
```

### Comparing `sgw_tools-1.97/LICENSE` & `sgw_tools-1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.97/PKG-INFO` & `sgw_tools-1.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.97
+Version: 1.98
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.97/setup.py` & `sgw_tools-1.98/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.97",
+    version="1.98",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.97/sgw_tools/__init__.py` & `sgw_tools-1.98/sgw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.97/sgw_tools/filters.py` & `sgw_tools-1.98/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.97/sgw_tools/graph.py` & `sgw_tools-1.98/sgw_tools/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,18 @@
     def dwq(self):
         if self._dwq is None:
             self._Wq, self._dwq = util.magneticAdjacencyMatrix(self, self.q)
         return self._dwq
 
     @property
     def lmin(self):
+        """
+        Smallest non-zero eigenvalue.
+        np.nan if all the eigenvalues are zero.
+        """
         if self._lmin is None:
             self.logger.warning('The smallest non-zero eigenvalue G.lmin is not '
                                 'available, we need to estimate it. '
                                 'Explicitly call G.estimate_lmin() or '
                                 'G.compute_fourier_basis() '
                                 'once beforehand to suppress this warning.')
             self.estimate_lmin()
```

### Comparing `sgw_tools-1.97/sgw_tools/graphs.py` & `sgw_tools-1.98/sgw_tools/graphs.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.97/sgw_tools/util.py` & `sgw_tools-1.98/sgw_tools/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,45 +65,50 @@
 
 
 def _estimate_lmin(G, maxiter):
     N = G.N
     if N > 100:
         approx_evecs = np.empty((N, 2))
         # 0-eigenvector (exact)
-        approx_evecs[:,:-1] = 1
+        approx_evecs[:,0] = 1
         # 1st non-zero eigenvector (guess)
         idxs = np.arange(N)
         one_idxs = np.random.choice(idxs, N//2, replace=False)
         neg_one_idxs = idxs[np.isin(idxs, one_idxs, assume_unique=True, invert=True)]
-        approx_evecs[one_idxs,-1] = 1
-        approx_evecs[neg_one_idxs,-1] = -1
+        approx_evecs[one_idxs,1] = 1
+        approx_evecs[neg_one_idxs,1] = -1
         if N&1:
-            approx_evecs[neg_one_idxs[-1],-1] = 0
+            approx_evecs[neg_one_idxs[-1],1] = 0
     
         # simple pre-conditioner
         M = sparse.spdiags(1/G.L.diagonal(), 0, N, N)
         evals, _ = sparse.linalg.lobpcg(G.L, approx_evecs, M=M, largest=False, maxiter=maxiter)
-        lmin = evals[-1]
-    else:
+        lmin = evals[1]
+    elif N > 1:
         # if small then do exact calculation
         G.compute_fourier_basis(spectrum_only=True)
         lmin = G.lmin
+    else:
+        # single vertex has eigenvalue zero
+        return np.nan
 
     assert lmin >= 0, "Smallest eigenvalue is negative {}".format(lmin)
     if np.isclose(lmin, 0):
         raise ValueError("Second eigenvalue is (close to) zero: {}".format(lmin))
     return lmin
 
 
 def estimate_lmin(G, maxiter=2000):
     lmins = []
     for subG in G.extract_components():
-        lmin = _estimate_lmin(subG, maxiter)
-        lmins.append(lmin)
-    return sorted(lmins)[0]
+        if subG.N > 1:  # skip trivial components
+            lmin = _estimate_lmin(subG, maxiter)
+            if not np.isnan(lmin):
+                lmins.append(lmin)
+    return sorted(lmins)[0] if lmins else np.nan
 
 
 def estimate_lmax(G, method='lanczos'):
     if method == 'lanczos':
         try:
             lmax = sparse.linalg.eigsh(G.L, k=1, tol=5e-3,
                                        ncv=min(G.N, 10),
```

### Comparing `sgw_tools-1.97/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.98/sgw_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw-tools
-Version: 1.97
+Version: 1.98
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.97/tests/test_biggraph.py` & `sgw_tools-1.98/tests/test_biggraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,27 @@
         G.compute_laplacian(lap_type='combinatorial')
         test_combinatorial(G)
         G.compute_laplacian(lap_type='normalized')
         test_normalized(G)
         G.compute_laplacian(lap_type='adjacency')
         test_adjacency(G)
 
+    def test_estimate_lmin(self):
+        graph = BigGraph([
+            [0, 3, 0, 1],
+            [3, 0, 1, 0],
+            [0, 1, 0, 3],
+            [1, 0, 3, 0],
+        ])
+        graph.estimate_lmin()
+        np.testing.assert_approx_equal(graph.lmin, 2)
+
+        graph = BigGraph.create_from(graphs.Sensor(N=107, seed=27))
+        np.testing.assert_approx_equal(graph.lmin, 0.08818931)
+
     def test_estimate_lmax(self):
         graph = BigGraph.create_from(graphs.Sensor())
         self.assertRaises(ValueError, graph.estimate_lmax, method='unk')
     
         def check_lmax(graph, lmax):
             graph.estimate_lmax(method='bounds')
             np.testing.assert_allclose(graph.lmax, lmax)
```

