# Comparing `tmp/ckmutil-0.3.2.tar.gz` & `tmp/ckmutil-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ckmutil-0.3.2.tar", last modified: Fri Apr  6 19:17:13 2018, max compression
+gzip compressed data, was "ckmutil-1.0.1.tar", last modified: Sun Aug  6 19:23:07 2023, max compression
```

## Comparing `ckmutil-0.3.2.tar` & `ckmutil-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 straub    (1000) straub    (1000)        0 2018-04-06 19:17:13.000000 ckmutil-0.3.2/
-drwxrwxr-x   0 straub    (1000) straub    (1000)        0 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil/
--rw-rw-r--   0 straub    (1000) straub    (1000)     3693 2017-11-15 12:22:28.000000 ckmutil-0.3.2/ckmutil/test_phases.py
--rw-rw-r--   0 straub    (1000) straub    (1000)     2774 2018-04-06 10:06:35.000000 ckmutil-0.3.2/ckmutil/phases.py
--rw-rw-r--   0 straub    (1000) straub    (1000)     4267 2017-11-13 16:32:17.000000 ckmutil-0.3.2/ckmutil/ckm.py
--rw-rw-r--   0 straub    (1000) straub    (1000)      202 2017-11-08 17:00:18.000000 ckmutil-0.3.2/ckmutil/__init__.py
--rw-rw-r--   0 straub    (1000) straub    (1000)     1061 2017-11-15 12:20:08.000000 ckmutil-0.3.2/ckmutil/test_diag.py
--rw-rw-r--   0 straub    (1000) straub    (1000)      759 2017-11-15 14:06:20.000000 ckmutil-0.3.2/ckmutil/diag.py
--rw-rw-r--   0 straub    (1000) straub    (1000)     1578 2017-11-08 16:50:55.000000 ckmutil-0.3.2/ckmutil/test_ckm.py
-drwxrwxr-x   0 straub    (1000) straub    (1000)        0 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/
--rw-rw-r--   0 straub    (1000) straub    (1000)      329 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/SOURCES.txt
--rw-rw-r--   0 straub    (1000) straub    (1000)        8 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/top_level.txt
--rw-rw-r--   0 straub    (1000) straub    (1000)       22 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/requires.txt
--rw-rw-r--   0 straub    (1000) straub    (1000)        1 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/dependency_links.txt
--rw-rw-r--   0 straub    (1000) straub    (1000)      535 2018-04-06 19:17:13.000000 ckmutil-0.3.2/ckmutil.egg-info/PKG-INFO
--rw-rw-r--   0 straub    (1000) straub    (1000)      483 2017-11-08 14:20:18.000000 ckmutil-0.3.2/README.md
--rw-rw-r--   0 straub    (1000) straub    (1000)       38 2017-06-28 14:54:28.000000 ckmutil-0.3.2/MANIFEST.in
--rw-rw-r--   0 straub    (1000) straub    (1000)      679 2018-04-06 19:16:39.000000 ckmutil-0.3.2/setup.py
--rw-rw-r--   0 straub    (1000) straub    (1000)       38 2018-04-06 19:17:13.000000 ckmutil-0.3.2/setup.cfg
--rw-rw-r--   0 straub    (1000) straub    (1000)     1086 2017-11-08 13:37:09.000000 ckmutil-0.3.2/LICENSE.txt
--rw-rw-r--   0 straub    (1000) straub    (1000)      535 2018-04-06 19:17:13.000000 ckmutil-0.3.2/PKG-INFO
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-06 19:23:07.244375 ckmutil-1.0.1/
+-rw-rw-r--   0 david     (1000) david     (1000)     1086 2023-08-06 18:50:50.000000 ckmutil-1.0.1/LICENSE.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-08-06 18:50:50.000000 ckmutil-1.0.1/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)      809 2023-08-06 19:23:07.244375 ckmutil-1.0.1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      483 2023-08-06 18:50:50.000000 ckmutil-1.0.1/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-06 19:23:07.244375 ckmutil-1.0.1/ckmutil/
+-rw-rw-r--   0 david     (1000) david     (1000)      202 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4267 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/ckm.py
+-rw-rw-r--   0 david     (1000) david     (1000)      944 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/diag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2774 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/phases.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1578 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/test_ckm.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1626 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/test_diag.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3693 2023-08-06 18:50:50.000000 ckmutil-1.0.1/ckmutil/test_phases.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-08-06 19:23:07.244375 ckmutil-1.0.1/ckmutil.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      809 2023-08-06 19:23:07.000000 ckmutil-1.0.1/ckmutil.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      344 2023-08-06 19:23:07.000000 ckmutil-1.0.1/ckmutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-08-06 19:23:07.000000 ckmutil-1.0.1/ckmutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       18 2023-08-06 19:23:07.000000 ckmutil-1.0.1/ckmutil.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-08-06 19:23:07.000000 ckmutil-1.0.1/ckmutil.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      549 2023-08-06 19:22:44.000000 ckmutil-1.0.1/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-08-06 19:23:07.244375 ckmutil-1.0.1/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)       66 2023-08-06 18:55:50.000000 ckmutil-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ckmutil-0.3.2/ckmutil/test_phases.py` & `ckmutil-1.0.1/ckmutil/test_phases.py`

 * *Files identical despite different names*

### Comparing `ckmutil-0.3.2/ckmutil/phases.py` & `ckmutil-1.0.1/ckmutil/phases.py`

 * *Files identical despite different names*

### Comparing `ckmutil-0.3.2/ckmutil/ckm.py` & `ckmutil-1.0.1/ckmutil/ckm.py`

 * *Files identical despite different names*

### Comparing `ckmutil-0.3.2/ckmutil/test_diag.py` & `ckmutil-1.0.1/ckmutil/test_diag.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,20 +7,32 @@
 Mc = np.array([[ 0.82469+0.62495j,  0.37768+0.28744j,  0.40011+0.93478j],
        [ 0.85475+0.60855j,  0.64045+0.93049j,  0.39019+0.6188j ],
        [ 0.68798+0.40478j,  0.38995+0.86032j,  0.20555+0.601j  ]])
 # complex symmetric
 Mcs = np.array([[ 0.82794+0.4311j ,  0.33124+0.73104j,  0.77668+0.14696j],
        [ 0.33124+0.73104j,  0.18407+0.67383j,  0.46557+0.14199j],
        [ 0.77668+0.14696j,  0.46557+0.14199j,  0.94771+0.73933j]])
+# complex symmetric with two degenerate singular values
+Mcsd = np.array([[ 0.20019824+0.21595061j,  0.0563654 -0.14476247j,
+         0.09818666-0.1975587j ],
+       [ 0.0563654 -0.14476247j,  0.2457214 -0.00074698j,
+        -0.04078761+0.19632891j],
+       [ 0.09818666-0.1975587j , -0.04078761+0.19632891j,
+         0.19381973+0.13898357j]])
 
 class TestDiag(unittest.TestCase):
     def test_svd(self):
         U, S, V = msvd(Mc)
         npt.assert_array_almost_equal(U @ np.diag(S) @ V.conj().T, Mc, decimal=12)
         npt.assert_array_equal(S.imag, np.array([0, 0, 0]))
         self.assertTrue(S[1] >= S[0])
         self.assertTrue(S[2] >= S[1])
 
     def test_takfac(self):
         npt.assert_array_equal(Mcs - Mcs.T, np.zeros((3,3)))
         U, S = mtakfac(Mcs)
         npt.assert_array_almost_equal(U.conj() @ np.diag(S) @ U.conj().T, Mcs, decimal=6)
+
+    def test_takfac_degenerate(self):
+        npt.assert_array_equal(Mcsd - Mcsd.T, np.zeros((3,3)))
+        U, S = mtakfac(Mcsd)
+        npt.assert_array_almost_equal(U.conj() @ np.diag(S) @ U.conj().T, Mcsd, decimal=6)
```

### Comparing `ckmutil-0.3.2/ckmutil/diag.py` & `ckmutil-1.0.1/ckmutil/diag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Functions for the diagonalization of fermion mass matrices."""
 
 import numpy as np
+from scipy.linalg import fractional_matrix_power
 
 def msvd(m):
   """Modified singular value decomposition.
 
   Returns U, S, V where Udagger M V = diag(S) and the singular values
   are sorted in ascending order (small to large).
   """
@@ -20,10 +21,14 @@
 def mtakfac(m):
   """Modified Takagi factorization of a (complex) symmetric matrix.
 
   Returns U, S where U^T M U = diag(S) and the singular values
   are sorted in ascending order (small to large).
   """
   u, s, v = msvd(np.asarray(m, dtype=complex))
-  f = np.sqrt(u.conj().T @ v.conj())
-  w = v @ f
+  z2 = u.conj().T @ v.conj()
+  if np.all(np.abs(z2 - np.diag(np.diag(z2))) < 1e-14): # if z2 is diagonal
+    z = np.sqrt(z2)
+  else:
+    z = fractional_matrix_power(z2,1/2)
+  w = v @ z
   return w, s
```

### Comparing `ckmutil-0.3.2/ckmutil/test_ckm.py` & `ckmutil-1.0.1/ckmutil/test_ckm.py`

 * *Files identical despite different names*

### Comparing `ckmutil-0.3.2/LICENSE.txt` & `ckmutil-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

