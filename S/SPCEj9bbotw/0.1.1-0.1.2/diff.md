# Comparing `tmp/SPCEj9bbotw-0.1.1.tar.gz` & `tmp/SPCEj9bbotw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.1.1.tar", last modified: Wed Aug  2 17:46:22 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.1.2.tar", last modified: Sun Aug  6 05:18:59 2023, max compression
```

## Comparing `SPCEj9bbotw-0.1.1.tar` & `SPCEj9bbotw-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:46:22.855343 SPCEj9bbotw-0.1.1/
--rw-rw-rw-   0        0        0       58 2023-08-02 17:46:22.855343 SPCEj9bbotw-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 17:46:22.835882 SPCEj9bbotw-0.1.1/SPCEj9bbotw/
--rw-rw-rw-   0        0        0       25 2023-08-02 17:46:09.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-08-02 17:07:17.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/_main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:46:22.848884 SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/
--rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/_.py
--rw-rw-rw-   0        0        0        0 2023-08-02 17:03:01.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/__init__.py
--rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/_matrix.py
--rw-rw-rw-   0        0        0     2917 2023-08-02 16:51:39.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/_plot.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:46:22.854341 SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/
--rw-rw-rw-   0        0        0      206 2023-08-02 17:45:08.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9055 2023-08-02 16:34:50.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/kernels.py
--rw-rw-rw-   0        0        0     6764 2023-08-02 10:18:20.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/optimizer.py
--rw-rw-rw-   0        0        0     6989 2023-08-02 17:32:32.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/optimizer_matrix.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:46:22.844884 SPCEj9bbotw-0.1.1/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-02 17:46:22.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-08-02 17:46:22.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:46:22.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 17:46:22.000000 SPCEj9bbotw-0.1.1/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 17:46:22.856343 SPCEj9bbotw-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      169 2023-08-02 17:45:38.000000 SPCEj9bbotw-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:18:59.518644 SPCEj9bbotw-0.1.2/
+-rw-rw-rw-   0        0        0       58 2023-08-06 05:18:59.517643 SPCEj9bbotw-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 05:18:59.494638 SPCEj9bbotw-0.1.2/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0       25 2023-08-06 05:16:55.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:18:59.511642 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/
+-rw-rw-rw-   0        0        0     1999 2023-08-06 05:09:37.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/Jsparse.py
+-rw-rw-rw-   0        0        0     3024 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/_.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/__init__.py
+-rw-rw-rw-   0        0        0     3025 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/_matrix.py
+-rw-rw-rw-   0        0        0     3997 2023-08-06 05:15:58.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/_plot.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:18:59.516643 SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/
+-rw-rw-rw-   0        0        0      206 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9055 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/kernels.py
+-rw-rw-rw-   0        0        0     6764 2023-08-06 05:08:32.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0     7362 2023-08-06 05:11:15.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/optimizer_matrix.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:18:59.506641 SPCEj9bbotw-0.1.2/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-06 05:18:59.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-08-06 05:18:59.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 05:18:59.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-06 05:18:59.000000 SPCEj9bbotw-0.1.2/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 05:18:59.518644 SPCEj9bbotw-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      169 2023-08-06 05:17:03.000000 SPCEj9bbotw-0.1.2/setup.py
```

### Comparing `SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/_.py` & `SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/_.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.1.1/SPCEj9bbotw/functions/_matrix.py` & `SPCEj9bbotw-0.1.2/SPCEj9bbotw/functions/_matrix.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/kernels.py` & `SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/kernels.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/optimizer.py` & `SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.1.1/SPCEj9bbotw/optimizer/optimizer_matrix.py` & `SPCEj9bbotw-0.1.2/SPCEj9bbotw/optimizer/optimizer_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
 from functions._matrix import *
+from functions.Jsparse import Jsparse as Jsp
 
 
 '''
 - sparse matrix type ver 
 - coefficient matrix of primal variable is calculated by cupy inverse function.
 - y_gpu just only for result plot
 '''
@@ -60,15 +61,15 @@
         
         self.z_lb_scl = self.scale['inv/z']*np.array([np.log(self.cond['m_0'] - self.cond['alpha']*self.cond['rho2']*
                                                              self.dt*i) for i in range(self.n+1)])
         self.z_ub_scl = self.scale['inv/z']*np.array([np.log(self.cond['m_0'] - self.cond['alpha']*self.cond['rho1']*
                                                              self.dt*i) for i in range(self.n+1)])
         
         
-    def make_mtrx(self):
+    def make_mtrx(self, n_out):
         self.TM = {}      
         self.TM['y2u-sig'] = transformation.extract((4,11), [0,1,2,9], self.n)
         block = np.zeros((2, 2*11))
         block[0, 20] = 1
         block[1,10] = 1
         self.TM['y2sig-z'] = transformation.band(block, self.n, 11)
         self.TM['y2sig-z'] = self.TM['y2sig-z'][:, 11:]
@@ -118,14 +119,23 @@
         
         ##b3
         self.b3 = sp.csr_matrix((2*self.n, 1))
         self.b3[1] = -self.scale['inv/z']*np.log(self.cond['m_0'])
         
         # ||xn||^2 - Zn
         self.coeff_y = self.rho*self.C.T@self.C
+        
+        st_idx =  11*(self.n - (n_out+1))
+        idx = [0]*3 + [1]*6 + [0]*2
+        shape = [11*self.n, 11*self.n]
+        data = [0, 100, 100, 0, 1, 1]
+        repeat = n_out
+        objective = Jsp.diag_part(st_idx, idx, shape, data, repeat)
+    
+        self.coeff_y[:] = self.coeff_y + objective
         self.coeff_y[-8:-2, -8:-2] = self.coeff_y[-8:-2, -8:-2] + sp.csr_matrix(sp.diags([1000, 100, 100, 10, 1, 1]))
         a = sp.hstack([self.coeff_y, self.talpha])
         b = sp.hstack([self.alpha, sp.csr_matrix((7*self.n,7*self.n))])
         self.coeff_y = sp.vstack([a,b])
         self.tilde_C_gpu = cp.array(self.coeff_y.toarray().astype(np.float32))
         self.tilde_C_gpu = cp.linalg.inv(self.tilde_C_gpu)
```

