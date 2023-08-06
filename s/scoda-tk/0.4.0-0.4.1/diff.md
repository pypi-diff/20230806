# Comparing `tmp/scoda-tk-0.4.0.tar.gz` & `tmp/scoda-tk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.4.0.tar", last modified: Fri Aug  4 16:39:58 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.1.tar", last modified: Sun Aug  6 14:29:04 2023, max compression
```

## Comparing `scoda-tk-0.4.0.tar` & `scoda-tk-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 17:43:12.000000 scoda-tk-0.4.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 17:43:13.000000 scoda-tk-0.4.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 17:43:21.000000 scoda-tk-0.4.0/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-04 16:38:31.000000 scoda-tk-0.4.0/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 17:43:12.000000 scoda-tk-0.4.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.407112 scoda-tk-0.4.0/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.447111 scoda-tk-0.4.0/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.735104 scoda-tk-0.4.0/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 17:43:17.000000 scoda-tk-0.4.0/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 17:43:17.000000 scoda-tk-0.4.0/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37683 2023-08-04 16:36:57.000000 scoda-tk-0.4.0/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    24791 2023-08-04 16:38:16.000000 scoda-tk-0.4.0/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    64946 2023-08-03 10:06:50.000000 scoda-tk-0.4.0/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:29:04.492895 scoda-tk-0.4.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:29:04.492895 scoda-tk-0.4.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.1/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:28:36.000000 scoda-tk-0.4.1/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:29:04.492895 scoda-tk-0.4.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:29:04.376897 scoda-tk-0.4.1/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:29:04.396897 scoda-tk-0.4.1/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.1/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31673 2023-08-06 13:09:30.000000 scoda-tk-0.4.1/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:29:04.480895 scoda-tk-0.4.1/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.1/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.1/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.1/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.1/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.1/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.1/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    25443 2023-08-06 14:22:59.000000 scoda-tk-0.4.1/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.1/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:29:04.492895 scoda-tk-0.4.1/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:29:04.000000 scoda-tk-0.4.1/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.4.0/LICENSE` & `scoda-tk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/PKG-INFO` & `scoda-tk-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.0/pyproject.toml` & `scoda-tk-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.4.0"
+version = "0.4.1"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.4.0/src/scoda/cpdb.py` & `scoda-tk-0.4.1/src/scoda/cpdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 import copy, os, time, warnings, math
 import numpy as np
 import pandas as pd
-import scanpy as sc
 from matplotlib.pyplot import figure
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 import matplotlib
 from subprocess import Popen, PIPE
 import shlex, anndata
 
+CELLPHONEDB = True
+try:
+    from cellphonedb.src.core.methods import cpdb_degs_analysis_method
+    from cellphonedb.src.core.methods import cpdb_statistical_analysis_method
+except ImportError:
+    print('WARNING: CellPhoneDB seems not be installed. ')
+    CELLPHONEDB = False
+
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
+
+    
 def run_command(cmd, verbose = True):
     cnt = 0
     with Popen(shlex.split(cmd), stdout=PIPE, bufsize=1, \
                universal_newlines=True ) as p:
         for line in p.stdout:
             if (line[:14] == 'Tool returned:'):                    
                 cnt += 1
@@ -177,21 +192,14 @@
         dfv.rename(index = rend, inplace = True)
     '''        
     return df_pval_info, df_pval_pairs, df_mean_pairs, dfv
 
 ###################################
 ### CellPhoneDB 4.1.0 #############
 
-try:
-    from cellphonedb.src.core.methods import cpdb_degs_analysis_method
-    from cellphonedb.src.core.methods import cpdb_statistical_analysis_method
-except ImportError:
-    print('WARNING: CellPhoneDB seems not be installed. ')
-
-
 def cpdb4_run( adata, cell_types, db, out_dir,
                gene_id_type = 'gene_name', n_cores = 4,
                n_iter = None, pval_th = None, threshold = None):
     
     if isinstance(adata, pd.DataFrame):
         X = adata.astype(int).copy(deep = True)
         cols = list(X.columns.values)
@@ -651,8 +659,297 @@
         ax.spines['right'].set_visible(False)
         ax.spines['bottom'].set_visible(False)
         ax.spines['left'].set_visible(False) 
         
     if title is not None: ax.set_title(title, fontsize = title_fs )
         
     if show: plt.show()
-    return
+    return
+
+
+def plot_cci_circ( df_in, figsize = (10, 10), title = None, title_fs = 16, 
+               text_fs = 14, num_fs = 12, margin = 0.08, alpha = 0.5, 
+               N = 500, R = 4, Rs = 0.1, lw_max = 10, lw_scale = 0.1, 
+               log_lw = False, node_size = 10, rot = True, 
+               cmap = 'Spectral', ax = None, show = True):
+              
+    df = df_in.copy(deep = True)
+    mxv = df_in.max().max()
+    
+    if ax is None: 
+        plt.figure(figsize = figsize)
+        ax = plt.gca()
+        
+    # color_lst = ['orange', 'navy', 'green', 'gold', # 'lime', 'magenta', \
+    #         'turquoise', 'red', 'royalblue', 'firebrick', 'gray']
+    # color_map = cm.get_cmap(cmap)
+    color_map = colormaps[cmap]
+    color_lst = [color_map(i/(df.shape[0]-1)) for i in range(df.shape[0])]
+
+    clst = list(df.index.values) 
+
+    M = df.shape[0]
+    pp = np.arange(M)*(2*math.pi/M)
+    px = np.sin(pp)
+    py = np.cos(pp)
+    pnts = np.array([px, py])
+    
+    for j in range(pnts.shape[1]):
+        p1 = pnts[:,j]
+        for k in range(pnts.shape[1]):
+            p2 = pnts[:,k]
+            
+            val = df.loc[clst[j], clst[k]]
+            if lw_scale > 0:
+                lw = val*lw_scale
+            elif lw_max > 0:
+                lw = val*lw_max/mxv
+            else:
+                lw = val
+            if log_lw: lw = np.log2(lw)                    
+                    
+            if (df.loc[clst[j], clst[k]] != 0): # & (j!= k):
+
+                if j == k:
+                    x, y, c = get_circ( p1, 0.1, N )
+                    K = int(len(x)*0.5)
+                    d = vrot(p1, 1)
+                    d = d*0.05/norm(d)
+                elif (j != k) :
+                    x, y, c = get_arc( p1, p2, R, N )
+
+                    K = int(len(x)*0.5)
+                    d = (p2 - p1)
+                    d = d*0.05/norm(d)
+
+                q2 = np.array([x[K], y[K]])
+                q1 = np.array([x[K] - d[0], y[K] - d[1]])
+
+                s = norm(q1 - q2)
+                
+                ha = 'center'
+                if c[0] < -1:
+                    ha = 'left'
+                elif c[0] > 1:
+                    ha = 'right'
+                    
+                va = 'center'
+                if c[1] < -1:
+                    va = 'bottom'
+                elif c[1] > 1:
+                    va = 'top'
+                    
+                if norm(q2) <= 0.7: # mnR*2:
+                    ha = 'center'
+                    va = 'center'
+                    
+                if ax is None: 
+                    plt.plot(x, y, c = color_lst[j], linewidth = lw, alpha = alpha)
+                    if j != k:
+                        plt.arrow(q1[0], q1[1], q2[0]-q1[0], q2[1]-q1[1], linewidth = lw,
+                              head_width=s/2, head_length=s, 
+                              fc=color_lst[j], ec=color_lst[j])
+                    plt.text( q2[0], q2[1], ' %i ' % val, fontsize = num_fs, 
+                              va = va, ha = ha)
+                else:
+                    ax.plot(x, y, c = color_lst[j], linewidth = lw, alpha = alpha)
+                    if j != k:
+                        ax.arrow(q1[0], q1[1], q2[0]-q1[0], q2[1]-q1[1], linewidth = lw,
+                              head_width=0.05*lw/lw_max, head_length=s, alpha = alpha, 
+                              fc=color_lst[j], ec=color_lst[j])
+                    ax.text( q2[0], q2[1], '%i' % val, fontsize = num_fs, 
+                             va = va, ha = ha)
+
+            elif (df.loc[clst[j], clst[k]] != 0) & (j== k):
+                x, y, c = get_circ( p1, Rs, N )
+                K = int(len(x)*0.5)
+                d = vrot(p1, 1)
+                d = d*0.05/norm(d)
+
+                q2 = np.array([x[K], y[K]])
+                q1 = np.array([x[K] - d[0], y[K] - d[1]])
+
+                s = norm(q1 - q2)
+                
+                ha = 'center'
+                if c[0] < -1:
+                    ha = 'left'
+                elif c[0] > 1:
+                    ha = 'right'
+                    
+                va = 'center'
+                if c[1] < -1:
+                    va = 'bottom'
+                elif c[1] > 1:
+                    va = 'top'
+                    
+                if norm(q2) <= 0.7: # mnR*2:
+                    ha = 'center'
+                    va = 'center'
+                    
+                if ax is None: 
+                    plt.plot(x, y, c = color_lst[j], linewidth = lw, alpha = alpha)
+                    plt.arrow(q1[0], q1[1], q2[0]-q1[0], q2[1]-q1[1], linewidth = lw,
+                              head_width=s/2, head_length=s, 
+                              fc=color_lst[j], ec=color_lst[j])
+                    plt.text( q2[0], q2[1], ' %i ' % val, fontsize = num_fs, 
+                              va = va, ha = ha)
+                else:
+                    ax.plot(x, y, c = color_lst[j], linewidth = lw, alpha = alpha)
+                    ax.arrow(q1[0], q1[1], q2[0]-q1[0], q2[1]-q1[1], linewidth = lw,
+                              head_width=0.05*lw/lw_max, head_length=s, alpha = alpha, 
+                              fc=color_lst[j], ec=color_lst[j])
+                    ax.text( q2[0], q2[1], '%i' % val, fontsize = num_fs, 
+                             va = va, ha = ha)
+    if rot:
+        rotation = 90 - 180*np.abs(pp)/math.pi
+        b = rotation < -90
+        rotation[b] = 180+rotation[b]
+    else:
+        rotation = np.zeros(M)
+        
+    for j in range(pnts.shape[1]):
+        (x, y) = (pnts[0,j], pnts[1,j])
+        
+        ha = 'center'
+        if x < 0:
+            ha = 'right'
+        else: 
+            ha = 'left'
+        va = 'center'
+        if y == 0:
+            pass
+        elif y < 0:
+            va = 'top'
+        else: 
+            va = 'bottom'
+            
+        a = (df.loc[clst[j], clst[j]] != 0)*(Rs*2)
+        if ax is None: 
+            plt.plot( x, y, 'o', ms = node_size, c = color_lst[j])
+            plt.text( x, y, ' %s ' % clst[j], fontsize = text_fs, 
+                      ha = ha, va = va, rotation = rotation[j])
+        else:
+            ax.plot( x, y, 'o', ms = node_size, c = color_lst[j])
+            ax.text( x*(1+a), y*(1+a), '  %s  ' % clst[j], fontsize = text_fs, 
+                     ha = ha, va = va, rotation = rotation[j])
+
+    if ax is None: 
+        plt.xticks([])
+        plt.yticks([])
+        plt.margins(x=margin, y=margin)
+    else:
+        ax.set_xticks([])
+        ax.set_yticks([])
+        ax.margins(x=margin, y=margin)
+        
+        ax.spines['top'].set_visible(False)
+        ax.spines['right'].set_visible(False)
+        ax.spines['bottom'].set_visible(False)
+        ax.spines['left'].set_visible(False) 
+        
+    if title is not None: ax.set_title(title, fontsize = title_fs )
+        
+    if show: plt.show()
+    return
+
+
+def plot_cci_circ_m( df_lst, ncol = 3, figsize = (8,7), title = None, title_y = 1, title_fs = 18, 
+                   text_fs = 16, num_fs = 12, margin = 0.08, alpha = 0.5, 
+                   N = 500, R = 3, Rs = 0.1, lw_max = 20, lw_scale = 0.2, log_lw = False, 
+                   node_size = 10, rot = False, cmap = 'Spectral', ws_hs = (0.2, 0.1) ):
+    
+    cond_lst = list(df_lst.keys())
+    nc = ncol
+    nr = int(np.ceil(len(cond_lst)/nc))
+    # nr, nc = 1, int(len(cond_lst))
+    fig, axes = plt.subplots(figsize = (figsize[0]*nc,figsize[1]*nr), nrows=nr, ncols=nc, # constrained_layout=True, 
+                             gridspec_kw={'width_ratios': [1]*nc})
+    fig.tight_layout() 
+    plt.subplots_adjust(left=0.025, bottom=0.025, right=0.975, top=0.975, wspace=ws_hs[0], hspace=ws_hs[1])
+    if title is not None: plt.suptitle(title, fontsize = title_fs, y = title_y)
+
+    for j, k in enumerate(cond_lst):
+
+        df = df_lst[k]*(df_lst[k] > 0).copy(deep = True)
+
+        plt.subplot(nr,nc,j+1)
+
+        if nr == 1: ax = axes[int(j)]
+        else: ax = axes[int(j/nc)][j%nc]
+
+        plot_cci_circ( df, title = k, title_fs = text_fs + 2, 
+                   text_fs = text_fs, num_fs = num_fs, margin = margin, alpha = alpha, 
+                   N = N, R = R, Rs = Rs, lw_max = lw_max, lw_scale = lw_scale, log_lw = log_lw, 
+                   node_size = node_size, rot = rot, cmap = cmap, 
+                   ax = ax, show = False)
+
+        if len(cond_lst) < (nr*nc):
+            for k in range(int(nr*nc - len(cond_lst))):
+                j = k + len(cond_lst)
+                ax = plt.subplot(nr,nc,j+1)
+                ax.axis('off')
+
+    plt.show()
+    return
+
+
+### Remove common CCI
+def cci_remove_common( df_dct ):
+    
+    idx_dct = {}
+    idxo_dct = {}
+    celltype_lst = []
+
+    for j, g in enumerate(df_dct.keys()):
+        idx_dct[g] = list(df_dct[g].index.values)
+        if j == 0:
+            idx_c = idx_dct[g]
+        else:
+            idx_c = list(set(idx_c).intersection(idx_dct[g]))
+
+        ctA = list(df_dct[g]['cell_A'].unique())
+        ctB = list(df_dct[g]['cell_B'].unique())
+        celltype_lst = list(set(celltype_lst).union(ctA + ctB))
+
+    for g in df_dct.keys():
+        idxo_dct[g] = list(set(idx_dct[g]) - set(idx_c))
+
+    dfs_dct = {}
+    for g in df_dct.keys():
+        dfs_dct[g] = df_dct[g].loc[idxo_dct[g],:]
+
+    celltype_lst.sort()
+    # len(idx_c), celltype_lst
+    
+    if remove_common:
+    
+    return dfs_dct
+
+
+## Get matrices summarizing the num CCIs for each condition
+def cci_get_ni_mat( dfs_dct, remove_common = True ):
+    
+    celltype_lst = []
+    for j, g in enumerate(dfs_dct.keys()):
+        ctA = list(dfs_dct[g]['cell_A'].unique())
+        ctB = list(dfs_dct[g]['cell_B'].unique())
+        celltype_lst = list(set(celltype_lst).union(ctA + ctB))
+
+    celltype_lst.sort()
+    
+    df_lst = {} 
+    for g in dfs_dct.keys():
+        b = dfs_dct[g]['cell_A'].isin(celltype_lst) & (dfs_dct[g]['cell_B'].isin(celltype_lst))
+        dfs = dfs_dct[g].loc[b,:]
+        df = pd.DataFrame(index = celltype_lst, columns = celltype_lst)
+        df.loc[:] = 0
+        for a, b in zip(dfs['cell_A'], dfs['cell_B']):
+            df.loc[a,b] += 1
+
+        df_lst[g] = df
+        
+    if remove_common: 
+        df_lst = cci_remove_common( df_lst )
+        
+    return df_lst
+
```

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.1/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.1/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.1/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.1/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.1/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.1/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.1/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.1/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/deg.py` & `scoda-tk-0.4.1/src/scoda/deg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 import time, os, copy, datetime, math, random, warnings
 import numpy as np
 import pandas as pd
 from scipy import stats
-import seaborn as sns
-from statannot import add_stat_annotation
 import matplotlib.pyplot as plt
 from matplotlib import cm
 
+STATANNOT = True
+try:
+    from statannot import add_stat_annotation
+except ImportError:
+    print('WARNING: statannot not installed or not available. ')
+    STATANNOT = False
+
+SEABORN = True
+try:
+    import seaborn as sns
+except ImportError:
+    print('WARNING: seaborn not installed or not available. ')
+    SEABORN = False
+
 
 ### Example 
 # df_cnt, df_pct= get_population( adata_s.obs['sid'], 
 #                                 adata_s.obs['minor'], sort_by = [] )
 # plot_population(df_pct, figsize=(6, 4), dpi = 80, return_fig = False)
 # df_cnt
     
@@ -198,67 +210,14 @@
         for k in range(nr*nc - len(items)):
             axes[nr-1][len(items)%nc + k].axis("off")
         
     plt.show()
     return 
 
 
-def plot_pct_box_old(df_pct, sg_map, nr_nc, figsize = None, dpi = 100,
-                 title = None, title_y = 1.05, title_fs = 14, 
-                 title_fs2 = 12, label_fs = 11, tick_fs = 10, tick_rot = 0, 
-                 annot_fs = 10, ws_hs = (0.3, 0.3)):
-    
-    df = df_pct.copy(deep = True)
-    nr, nc = nr_nc
-    ws, hs = ws_hs
-    fig, axes = plt.subplots(figsize=figsize, dpi=dpi, nrows=nr, ncols=nc, constrained_layout=True)
-    fig.tight_layout() # Or equivalently,  "plt.tight_layout()"
-    if title is not None:
-        fig.suptitle('%s' % title, x = 0.5, y = title_y, fontsize = title_fs, ha = 'center')
-    plt.subplots_adjust(left=None, bottom=None, right=None, top=None, wspace=ws, hspace=hs)
-
-    items = list(df.columns.values)
-
-    df['Group'] = list(df.index.values)
-    df['Group'].replace(sg_map, inplace = True)
-
-    lst = df['Group'].unique()
-    lst_pair = []
-    for k, l1 in enumerate(lst):
-        for j, l2 in enumerate(lst):
-            if j >  k:
-                lst_pair.append((l1, l2))
-
-    for k, item in enumerate(items):
-        plt.subplot(nr,nc,k+1)
-        ax = sns.boxplot(data = df, x = 'Group', y = item) #, order=['HC', 'CC', 'AC'])
-        if k%nc == 0: plt.ylabel('Percentage', fontsize = label_fs)
-        else: plt.ylabel(None)
-        if k >= nc*(nr-1): plt.xlabel('Condition', fontsize = label_fs)
-        else: plt.xlabel(None)
-        plt.title(item, fontsize = title_fs2)
-        if k < (nr*nc - nc):
-            plt.xticks([])
-            plt.yticks(fontsize = tick_fs)
-        else:
-            plt.xticks(rotation = 0, ha = 'center', fontsize = tick_fs)
-            plt.yticks(fontsize = tick_fs)
-
-        add_stat_annotation(ax, data=df, x = 'Group', y = item, # order=['HC', 'CC', 'AC'],
-                        box_pairs=lst_pair, loc='inside', fontsize = annot_fs,
-                        test='t-test_ind', text_format='simple', verbose=0)
-        #'''
-    if (len(items) < (nr*nc)) & (nr > 1):
-        for k in range(nr*nc - len(items)):
-            axes[nr-1][len(items)%nc + k].axis("off")
-        
-    plt.show()
-    return
-
-
 def select_samples( adata_s, sample_col, N_min = 100, R_max = 2.5, verbose = False ):
 
     pcnt = adata_s.obs[sample_col].value_counts()
     b = pcnt >= N_min
     plst = list(pcnt.index.values[b])
 
     N_min = int(max(pcnt.min(), N_min))
```

### Comparing `scoda-tk-0.4.0/src/scoda/gsea.py` & `scoda-tk-0.4.1/src/scoda/gsea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 import numpy as np
 import pandas as pd
-import scanpy as sc
-import gseapy as gp
-import seaborn as sns
 import matplotlib.pyplot as plt
 import os, warnings, random
 import matplotlib as mpl
 
+'''
+import scanpy as sc
+import gseapy as gp
+import seaborn as sns
+'''
+
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
+
+SEABORN = True
+try:
+    import seaborn as sns
+except ImportError:
+    print('WARNING: seaborn not installed or not available. ')
+    SEABORN = False
+
+GSEAPY = True
+try:
+    import gseapy as gp
+except ImportError:
+    print('WARNING: gseapy not installed or not available. ')
+    GSEAPY = False
+
+
 ### Example
 # data = 'BRL_mouse'
 # adata_t = sc.read_h5ad('mmColon_85K_%s_ann.h5ad' % data)
 
 # ## Normalize and log-transform
 # sc.pp.normalize_total(adata_t, target_sum=1e4)
 # sc.pp.log1p(adata_t)
```

### Comparing `scoda-tk-0.4.0/src/scoda/hicat.py` & `scoda-tk-0.4.1/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.0/src/scoda/icnv.py` & `scoda-tk-0.4.1/src/scoda/icnv.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,37 @@
 import matplotlib.pyplot as plt
 from sklearn import cluster, mixture
 from sklearn.neighbors import kneighbors_graph
 from sknetwork.clustering import Louvain
 from sklearn.decomposition import PCA, IncrementalPCA, TruncatedSVD
 from scipy import stats
 
-import scanpy as sc
-import infercnvpy as cnv
+CLUSTERING_AGO = 'lv'
+SKNETWORK = True
+try:
+    from sknetwork.clustering import Louvain
+except ImportError:
+    print('WARNING: sknetwork not installed. GMM will be used for clustering.')
+    CLUSTERING_AGO = 'gm'
+    SKNETWORK = False
+
+INFERCNVPY = True
+try:
+    import infercnvpy as cnv
+except ImportError:
+    print('ERROR: infercnvpy not installed. Tumor cell identification will not be performed.')
+    INFERCNVPY = False
+
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
 
-cell_cycle_genes_s = ['ATAD2', 'BLM', 'BRIP1', 'CASP8AP2', 'CCNE2',
-         'CDC45', 'CDC6', 'CDCA7', 'CHAF1B', 'CLSPN', 'DSCC1',
-         'DTL', 'E2F8', 'EXO1', 'FEN1', 'GINS2', 'GMNN', 'HELLS',
-         'MCM2', 'MCM4', 'MCM5', 'MCM6', 'MLF1IP', 'MSH2', 'NASP',
-         'PCNA', 'POLA1', 'POLD3', 'PRIM1', 'RAD51', 'RAD51AP1',
-         'RFC2', 'RPA2', 'RRM1', 'RRM2', 'SLBP', 'TIPIN', 'TYMS',
-         'UBR7', 'UHRF1', 'UNG', 'USP1', 'WDR76']
-
-cell_cycle_genes_g2m = ['ANLN', 'ANP32E', 'AURKA', 'AURKB', 'BIRC5',
-         'BUB1', 'CBX5', 'CCNB2', 'CDC20', 'CDC25C', 'CDCA2',
-         'CDCA3', 'CDCA8', 'CDK1', 'CENPA', 'CENPE', 'CENPF',
-         'CKAP2', 'CKAP2L', 'CKAP5', 'CKS1B', 'CKS2', 'CTCF',
-         'DLGAP5', 'ECT2', 'FAM64A', 'G2E3', 'GAS2L3', 'GTSE1',
-         'HJURP', 'HMGB2', 'HMMR', 'HN1', 'KIF11', 'KIF20B', 'KIF23',
-         'KIF2C', 'LBR', 'MKI67', 'NCAPD2', 'NDC80', 'NEK2', 'NUF2',
-         'NUSAP1', 'PSRC1', 'RANGAP1', 'SMC4', 'TACC3', 'TMPO', 'TOP2A',
-         'TPX2', 'TTK', 'TUBB4B', 'UBE2C']
 
 MIN_ABS_VALUE = 1e-8
 
 def bimodal_fit( x ):
     
     df_param = pd.DataFrame( columns = ['value'], \
                           index = ['w0', 'm0', 'v0', 'w1', 'm1', 'v1'] )
@@ -185,15 +188,15 @@
                     label_fs = 12, tick_fs = 11, legend_fs = 11, 
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
     return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix]], params
 
 
-def get_cnv_threshold_useref( obs, ref_ind, score_key = 'tumor_score', 
+def get_cnv_threshold_useref( obs, ref_ind, ref_ind_org, score_key = 'tumor_score', 
                               cluster_key = 'cnv_leiden', th_max = 0, refp_min = 0.9, 
                               p_exc = 0.1, ucr = 0.1, plot_stat = True, 
                               suffix = '', Data = None ):
     
     th_min = -th_max
     
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
@@ -223,14 +226,17 @@
         df.loc[idx, 'ref_frac'] = ref_percent
         if (ref_percent >= refp_min):
             b_inc.append(True)
         else:
             b_inc.append(False)
 
     df['b_inc'] = b_inc
+    b = df['b_inc']
+    normal_max = df.loc[b, 'cmean'].max()
+    
     b = np.array(b_inc)
     # print(df)
 
     ns = np.sum(b)
     # if ns == 0: refp_min *= 0.95
     if ns == 0:
         print('ERROR: no reference type clusters found.')
@@ -343,84 +349,80 @@
     
     dec = pd.Series(['Normal']*len(s), index = obs.index)
     '''
     b = s >= th
     dec[b] = 'Tumor'
     dec[~b] = 'Normal'
     '''
-    br = np.array(ref_ind)
     bs = (s > th)
     
     #'''
     lt = th - (th - m0)*ucr # p_exc 
     ut = th + (m1 - th)*ucr #p_exc
-#     b = (s > lt) & (s < ut) & (~br)
-#     print(lt, ut, np.sum(~br), np.sum(b))
-#     dec[b] = 'unclear'
     #'''
     
     df['dec'] = 'Normal'
-    for idx in idx_lst:
-        b1 = obs[cluster_key] == idx
-        if df.loc[idx, 'cmean'] > ut:            
-            dec[b1&(~br)] = 'Tumor'
-            df.loc[idx, 'dec'] = 'Tumor'
-        elif df.loc[idx, 'cmean'] < lt:
-            pass
-        else:
-            dec[b1&(~br)] = 'unclear'
-            df.loc[idx, 'dec'] = 'unclear'
-            
-        # obs.loc[b1&(~br), score_key] = df.loc[idx, 'cmean']
-            
-#             if np.sum(b1&br) == 0:
-#                 dec[b1] = 'Tumor'
-#             elif (np.sum(b1&br)/np.sum(b1)) >= refp_min:
-#                 pass
-#             else:
-#                 dec[b1&bs&(~br)] = 'Tumor'
-
-#                 # if np.sum(b1&(~br)&bs)/np.sum(b1) < 0.4:
-#                 if np.sum(b1&bs&(~br)/np.sum(b1) < 0.3:
-#                     pass
-#                 else:
-#                     # dec[b1&(~br)&bs] = 'Tumor'
-#                     dec[b1&bs&(~br)] = 'Tumor'
-    '''
-    lt = th - (th - m0)*p_exc 
-    ut = th + (m1 - th)*p_exc
-    b = (s > lt) & (s < ut) & (~br)
-    print(lt, ut, np.sum(~br), np.sum(b))
-    dec[b] = 'unclear'
+    if ref_ind_org is not None:
+        br = np.array(ref_ind)
+        for idx in idx_lst:
+            b1 = obs[cluster_key] == idx
+            if df.loc[idx, 'cmean'] > ut:            
+                dec[b1&(~br)] = 'Tumor'
+                df.loc[idx, 'dec'] = 'Tumor'
+            elif df.loc[idx, 'cmean'] < lt:
+                pass
+            else:
+                dec[b1&(~br)] = 'unclear'
+                df.loc[idx, 'dec'] = 'unclear'
+    else:
+        for idx in idx_lst:
+            b1 = obs[cluster_key] == idx
+            if df.loc[idx, 'cmean'] > ut:            
+                dec[b1] = 'Tumor'
+                df.loc[idx, 'dec'] = 'Tumor'
+            elif df.loc[idx, 'cmean'] < lt:
+                pass
+            else:
+                dec[b1] = 'unclear'
+                df.loc[idx, 'dec'] = 'unclear'
+                    
     #'''
+    b = (df['b_inc'] == False) & (df['cmean'] > normal_max) & (df['dec'] == 'Normal')
+    if np.sum(b) > 0:
+        name_set = 'Tumor'
+        df.loc[b, 'dec'] = name_set 
+        for c in list(df.index.values[b]):
+            b = obs[cluster_key] == c
+            dec[b] = name_set
+    
     if ss_div_dm > 1:
         b = dec == 'Tumor'
         print('INFO: %i among %i were identified as tumor cells.' \
               % (np.sum(b), len(b)))
     
-    # b = (obs[ref_key].isin(ref_types)) | (s <= th)
-    # dec[b] = 'Normal'    
     obs['tumor_dec'+ suffix] = dec
 
     tclust = dec.copy(deep = True)
-    tclust[:] = None
+    tclust[:] = 'Normal'
     cnt = 1
     for c in idx_lst:
         b = obs[cluster_key] == c
         b1 = dec == 'Tumor'
         if np.sum(b&b1) > 0:
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
-    # obs['tumor_cluster'+ suffix] = tclust
+    obs['tumor_cluster'+ suffix] = tclust
     
     etime = round(time.time() - start_time) 
     # print('CNVth(%i) ' % etime, end = '', flush = True)
     
     params = {}
     params['th'] = th
+    params['th_lower'] = lt
+    params['th_upper'] = ut
     params['m0'] = m0
     params['v0'] = v0
     params['w0'] = w0
     params['m1'] = m1
     params['v1'] = v1
     params['w1'] = w1
     params['df'] = df
@@ -431,72 +433,14 @@
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
     return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix]], params
     # return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]], params
 
 
-def initially_detect_major_clusters( X_pca, y_clust, cobj, pmaj = 0.7, 
-                             cutoff = 0.01, verbose = False ):
-    
-    adj_agg = cobj.aggregate_
-    adj_agg_mat = adj_agg.todense().astype(int) 
-    labels_unique, counts = np.unique(y_clust, return_counts=True)
-
-    ## Get neighbor clusters
-    # cutoff = 0.01
-    aj = {}
-    for j in range(len(labels_unique)):
-        a = []
-        b = []
-        for k in range(len(labels_unique)):
-            if (adj_agg_mat[j,k] >= adj_agg_mat[j,j]*cutoff) & (adj_agg_mat[j,k] >= adj_agg_mat[k,k]*cutoff):
-                a.append(k)
-                b.append(adj_agg_mat[j,k])
-        if len(a) > 0:
-            odr = (-np.array(b)).argsort()
-            a1 = []
-            b1 = []
-            bn = []
-            for o in odr:
-                a1.append(a[o])
-                b1.append(b[o])
-                nv = int(10*np.log10(b[o]/adj_agg_mat[j,j] + 1e-10))
-                bn.append(nv)
-            d = dict(zip(a1,bn))
-            bn.sort(reverse = True)
-            aj[j] = d
-
-    ## Get community list
-    communities = []
-    for key in aj.keys():
-        d = aj[key]
-        nodes = list(d.keys())
-        if len(nodes) > 1:
-            common = nodes
-            for n in nodes:
-                common = list(set(common).intersection(list(aj[n].keys())))
-            if len(common) > 1:
-                communities.append(common)
-                # print(key, ': ', common)
-
-    to_del = []
-    for k, c in enumerate(communities):
-        b = False
-        for k2, c2 in enumerate(communities):
-            if (k2 != k) & (k not in to_del) & (k2 not in to_del):
-                if (len(list(set(c) - set(c2))) == 0):
-                    to_del.append(k)
-
-    for k in reversed(to_del):
-        del communities[k]
-    
-    return merge_communities(communities)
-
-
 def merge_communities( communities ):
     
     cm = copy.deepcopy(communities)
     to_del = []
     for j in reversed(range(len(cm))):
         if j > 0:
             for k in range(j):
@@ -517,86 +461,25 @@
     
     ss = np.array(ss)
     odr = ss.argsort()
     
     return cm[odr[0]]
 
 
-def extend_major_clusters_old(adj_agg_mat, seed_clusters):
-
-    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
-
-    for a in range(adj_agg_mat.shape[0] - len(seed_clusters)):
-        # def get_pv( s, adj_agg_mat, seed_clusters ):
-        mn = adj_agg_mat[seed_clusters, :].mean(axis = 0)
-        sd = adj_agg_mat[seed_clusters, :].std(axis = 0)
-
-        pvss = []
-        for n in range(adj_agg_mat.shape[0]):
-
-            if n in seed_clusters:
-                pvs = []
-                for s in seed_clusters:
-                    if n != s:
-                        st = np.abs(mn[s] - mn[n])/((sd[s] + sd[n]))
-                        pv = stats.t.sf(st*np.sqrt(2), df = len(seed_clusters))*2
-                        pv = np.round(pv, 3)
-                        pvs.append(pv)
-
-                # print(n, pvs, np.max(pvs))
-                pvss.append(pvs)
-
-        pvss = np.array(pvss)
-        th = pvss.max(axis = 1).min()
-
-        pvss = []
-        nodes = []
-        for n in range(adj_agg_mat.shape[0]):
-
-            if n not in seed_clusters:
-                pvs = []
-                for s in seed_clusters:
-                    st = np.abs(mn[s] - mn[n])/((sd[s] + sd[n]))
-                    pv = stats.t.sf(st*np.sqrt(2), df = len(seed_clusters))*2
-                    pv = np.round(pv, 3)
-                    pvs.append(pv)
-
-                # print(n, pvs, np.max(pvs))
-                nodes.append(n)
-                pvss.append(pvs)
-
-        pvss = np.array(pvss)
-        nodes = np.array(nodes)
-        pvs = pvss.max(axis = 1)
-        odr = pvs.argsort()
-        mx_pv = pvs[odr[-1]]
-        if mx_pv >= th:
-            seed_clusters.append(nodes[odr[-1]])
-            # print(th, mx_pv, seed_clusters)
-        else:
-            break
-            
-    return seed_clusters
-
-
 def extend_major_clusters( adj_agg_mat, seed_clusters, 
                            cluster_size, n_neighbors, alpha = 0.08, 
                            pv_cutoff = None, mode = 'max', 
                            verbose = False ):
 
     selected_clusters = copy.deepcopy(seed_clusters)
     maj_clusters = copy.deepcopy(seed_clusters)
     pair_clusters = list(np.zeros(len(seed_clusters)))
     metrics = list(np.zeros(len(seed_clusters)))
     thresholds = list(np.zeros(len(seed_clusters)))
     
-    adj_agg_mat = np.array(adj_agg_mat)
-    adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
-    adj_agg_mat = adj_agg_mat + adj_agg_mat.transpose()
-
     csz_lst = [cluster_size[n] for n in maj_clusters]
     odr = (-np.array(csz_lst)).argsort()
     maj_clusters = [maj_clusters[o] for o in odr]
     
     core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
 
     for j, n in enumerate(maj_clusters):
@@ -696,29 +579,60 @@
     else:
         core_mxs = core_mat.sum(axis = 1)
     
     return (np.array(selected_clusters), 
            np.array(maj_clusters), np.array(pair_clusters), metrics, thresholds)
 
 
+def initially_detect_major_clusters( adj_agg_mat, cluster_scores,
+                           cluster_size, n_neighbors, alpha = 0.08, 
+                           pv_cutoff = None, mode = 'max', 
+                           verbose = False ):
+
+    cluster_lst = list(np.arange(len(cluster_size)))
+    
+    selected_clusters = []
+    score = 1e4
+    for c in cluster_lst:
+        seed_clusters = [c]
+        selected, maj, pairs, mets, threshs = \
+            extend_major_clusters( adj_agg_mat, seed_clusters, 
+                           cluster_size, n_neighbors, alpha = 0.08, 
+                           pv_cutoff = None, mode = 'max', 
+                           verbose = False )
+        
+        sz = 0
+        ss = 0
+        for s in selected:
+            sz += cluster_size[s]
+            ss += cluster_size[s]*cluster_scores[s]
+        ss = ss/sz
+        
+        # if ss < score:
+        if len(selected) > len(selected_clusters):
+            score = ss
+            selected_clusters = copy.deepcopy(selected)
+            
+    return selected_clusters
+
+
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
              resolution = 2, N_pca = 15, n_neighbors = 10, umap = True, pca = True, n_cores = 4 ):
     
     pca_umap = umap
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
     
         ## Normalize and log-transform
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
 
         sc.pp.highly_variable_genes(adata, n_top_genes = 2000) # , flavor = 'seurat_v3')
-        # sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
 
         cnv.io.genomic_position_from_gtf(gtf_file, adata, gtf_gene_id='gene_name', adata_gene_id=None, inplace=True)
         cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, 
                         window_size=100, n_jobs = n_cores)
 
         if pca:
             print('PCA .. ', end = '')
@@ -749,15 +663,15 @@
 
 CLUSTERING_AGO = 'lv'
 SKNETWORK = True
 try:
     from sknetwork.clustering import Louvain
 except ImportError:
     print('WARNING: sknetwork not installed. GMM will be used for clustering.')
-    CLUSTERING_AGO = 'gm'
+    CLUSTERING_AGO = 'km'
     SKNETWORK = False
 
     
 def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
                    mode='connectivity', n_cores = 4):
                    # mode='distance', n_cores = 4):
     
@@ -820,27 +734,49 @@
 
     df['b_inc'] = b_inc
     b = np.array(b_inc)
     # print(df)
     return df
 
 
+def find_num_clusters( N, Clustering_resolution = 1 ):
+    return int(max(((N*(Clustering_resolution**2))**(1/6))*5, 10))
+
+def merge_small_clusters( adj_agg_mat, cluster_size, alpha, min_cluster_size = 100 ):
+    
+    b = np.array(cluster_size) < min_cluster_size
+    if np.sum(b) == 0:
+        return None
+    else:
+        dct = {}
+        clst = list(np.arange(len(cluster_size))[b])
+        for c in clst:
+            met = adj_agg_mat[:,c]
+            odr = met.argsort()
+            md = met[odr[-1]]
+            csz = md/cluster_size[c]
+            if csz >= (alpha):
+                dct[c] = odr[-1]
+            
+        return dct    
+
+
 def identify_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, clust = None, 
                          Clustering_algo = 'lv', Clustering_resolution = 1, N_clusters = 30,
                          # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                          gmm_N_comp = 20, th_max = 0.1, refp_min = 0.9, p_exc = 0.1, 
                          dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
                          gcm = 0.05, plot_stat = False, use_ref = False, 
                          n_cores = 4, connectivity_thresh = 0.08, net_search_mode = 'sum', 
-                         suffix = '', Data = None, verbose = False):
+                         suffix = '', Data = None, verbose = False, use_umap = False):
+    
+    N_clusters = find_num_clusters( X_cnv.shape[0], Clustering_resolution*0.5 )
     
-    N_clusters = int(np.log2(X_cnv.shape[0])*2*np.sqrt(Clustering_resolution))
-    gmm_N_comp = int(N_clusters/2)
     if Clustering_algo != 'lv':
-        print('Clustering using %s with N_clusters = %i, %i. ' % (Clustering_algo.upper(), N_clusters, gmm_N_comp))
+        print('Clustering using %s with N_clusters = %i. ' % (Clustering_algo.upper(), N_clusters))
     
     ## Remove all zero X_cnv
     X_cnv_mean = np.array(X_cnv.sum(axis = 1))
     b = X_cnv_mean == 0
     if np.sum(b) > 0:
         # print(np.sum(b))
         odr = np.array(X_cnv_mean).argsort()
@@ -849,60 +785,166 @@
         idxs = np.arange(X_cnv.shape[0])[list(b)]
         for i in idxs:
             X_cnv[i,:] = x_cnv
             
     ref_addon = None
     score_key = 'tumor_score' + suffix
     cluster_key = 'cnv_cluster' 
-    ## Get X_pca for ref_type cells
-
+    
+    ##########
+    ## PCA ###
     start_time = time.time()
     start_time_a = start_time
     print('Running iCNV addon .. ', end = '', flush = True)
     
     if isinstance(X_cnv, pd.DataFrame):
         df = pd.DataFrame(index = X_cnv.index.values)
     else:
         df = pd.DataFrame()
         X_cnv = pd.DataFrame(X_cnv)
     
     N_components_pca = 15
-    # pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
     pca_obj = TruncatedSVD(n_components = int(N_components_pca), random_state = 0) # , algorithm = 'arpack')
     
     if not pca: 
         X_pca = pca_obj.fit_transform(X_cnv)
+        if use_umap:
+            umap_obj = umap.UMAP(random_state=0)
+            X_vec = umap_obj.fit_transform(X_pca)
+        else: 
+            X_vec = copy.deepcopy(X_pca)
         
         etime = round(time.time() - start_time) 
         print('P(%i) .. ' % etime, end = '', flush = True)
         start_time = time.time()           
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
+        if use_umap:
+            umap_obj = umap.UMAP(random_state=0)
+            X_vec = umap_obj.fit_transform(X_pca)
+        else: 
+            X_vec = copy.deepcopy(X_pca)
+       
+    ################
+    ## Clustering ##
+    if ref_ind is None: 
+        y_clust, cobj, adj = clustering_alg( X_vec, clust_algo = Clustering_algo, N_clusters = N_clusters, 
+                                             resolution = Clustering_resolution, N_neighbors = n_neighbors, 
+                                             mode = 'connectivity', n_cores = n_cores)
+        if adj is None:
+            adj = kneighbors_graph(X_vec, int(n_neighbors), mode = 'connectivity', 
+                                   include_self=True, n_jobs = n_cores)
+        N_clusters = int(np.max(y_clust) + 1)
+    else:            
+        X_vec_sel = X_vec[~ref_ind, :]
+        resolution = Clustering_resolution*(np.sum(~ref_ind)/len(ref_ind))*0.5
+        N_cs = find_num_clusters( np.sum(~ref_ind), resolution*0.5 )
+        # print('Res/Nclust A: ', resolution, N_clusters)
+        y_clust_sel, cobj, adj = clustering_alg( X_vec_sel, clust_algo = Clustering_algo, N_clusters = N_cs, 
+                                             resolution = resolution, N_neighbors = n_neighbors, 
+                                             mode = 'connectivity', n_cores = n_cores)
             
-    y_clust, cobj, adj = clustering_alg( X_pca, clust_algo = Clustering_algo, N_clusters = N_clusters, 
-                                         resolution = Clustering_resolution, N_neighbors = n_neighbors, 
-                                         mode = 'connectivity', n_cores = n_cores)
-
-    if adj is None:
-        adj = kneighbors_graph(X_pca, int(n_neighbors), mode = 'connectivity', 
+        X_vec_ref = X_vec[ref_ind, :]
+        resolution = Clustering_resolution*(np.sum(ref_ind)/len(ref_ind))*0.5
+        N_cr = find_num_clusters( np.sum(ref_ind), resolution*0.5 )
+        # print('Res/Nclust B: ', resolution, N_clusters)
+        y_clust_ref, cobj, adj = clustering_alg( X_vec_ref, clust_algo = Clustering_algo, N_clusters = N_cr, 
+                                             resolution = resolution, N_neighbors = n_neighbors, 
+                                             mode = 'connectivity', n_cores = n_cores)
+
+        y_clust = np.zeros(X_vec.shape[0], dtype = int)
+        y_clust[ref_ind] = y_clust_ref
+        y_clust[~ref_ind] = y_clust_sel + (1 + np.max(y_clust_ref)) 
+        
+        N_clusters = N_cs + N_cr
+        adj = kneighbors_graph(X_vec, int(n_neighbors), mode = 'connectivity', 
                                include_self=True, n_jobs = n_cores)
     
     etime = round(time.time() - start_time) 
-    print('C(%i) .. ' % etime, end = '', flush = True)
+    print('C(%i, Nc:%i) .. ' % (etime, N_clusters), end = '', flush = True)
     start_time = time.time()
     
-    cnv_clust_lst = list(set(y_clust))
-    cnv_clust_lst.sort()
+    ## Compute Cluster size, Aggregated Adj.Mat and Merge Small clusters 
+    for kk in range(2):
+        
+        cnv_clust_lst = list(set(y_clust))
+        cnv_clust_lst.sort()
+
+        cluster_size = [] 
+        for c in cnv_clust_lst:
+            b = y_clust == c
+            cluster_size.append(np.sum(b))
+
+        ## Generate agg_adj_mat
+        if (ref_ind is None) & (Clustering_algo == 'lv'):
+            adj_agg = cobj.aggregate_
+            adj_agg_mat = np.array(adj_agg.todense().astype(int)) 
+        else:
+            rows = adj.tocoo().row
+            cols = adj.tocoo().col
+            vals = adj.data
+
+            adj_agg_mat = np.zeros([len(cnv_clust_lst), len(cnv_clust_lst)], dtype = int)
+            for r, c, v in zip(rows, cols, vals):
+                adj_agg_mat[y_clust[r],y_clust[c]] += 1
+
+            adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
+            adj_agg_mat = adj_agg_mat + adj_agg_mat.transpose()
+                
+        if np.min(cluster_size) >= 100:
+            break
+        else:
+            ## Merge small clusters to a closest one
+            cc_dct = merge_small_clusters( adj_agg_mat, cluster_size, 
+                                           alpha = connectivity_thresh, min_cluster_size = 100 )
+            if cc_dct is not None:
+                for ck in cc_dct.keys():
+                    b = y_clust == ck
+                    y_clust[b] = cc_dct[ck]
+
+                ## Re-numbering
+                cnv_clust_lst = list(set(y_clust))
+                cnv_clust_lst.sort()
+                y_clust_new = np.zeros(X_vec.shape[0], dtype = int)
+                for j, c in enumerate(cnv_clust_lst):
+                    b = y_clust == c
+                    y_clust_new[b] = j
+                y_clust = y_clust_new
+            else:
+                break
+    
+                
     df[cluster_key] = y_clust
+    
+    ## Find cluster sizes
+    abs_X_cnv = np.sqrt(X_cnv**2)
+    '''
+    Nn = int(X_cnv.shape[1]*0.85)
+    abs_X_cnv = np.sort((abs_X_cnv), axis = 1)[:,Nn:]
+    print('abs_X_cnv shape: ', abs_X_cnv.shape)
+    '''
+    y_conf = (abs_X_cnv.mean(axis = 1))*100
         
+    cluster_scores = []
+    for c in cnv_clust_lst:
+        b = y_clust == c
+        cluster_scores.append(y_conf[b].mean())
+       
+    ## Find seed clusters
     cluster_sel = None
     
-    if ref_ind is not None: # use_ref:
+    if ref_ind is None: 
+        # cluster_sel = initially_detect_major_clusters_old(X_vec, y_clust, adj_agg_mat, pmaj = 0.7, 
+        #                  cutoff = cmd_cutoff, verbose = False )        
+        cluster_sel = initially_detect_major_clusters( adj_agg_mat, cluster_scores, 
+                           cluster_size, n_neighbors, alpha = connectivity_thresh, 
+                           pv_cutoff = None, mode = net_search_mode, 
+                           verbose = verbose )
+    else:
         b = ref_ind
-        #'''
         b_inc = []
         for idx in cnv_clust_lst:
             b = y_clust == idx
             bt = b & ref_ind
             cnt = np.sum(bt)
 
             if (cnt >= refp_min*np.sum(b)):
@@ -910,139 +952,101 @@
             else:
                 b_inc.append(False)
 
         if np.sum(b_inc) > 0:
             cluster_sel = list(np.array(cnv_clust_lst)[b_inc]) 
         else:
             print('ERROR: No reference cell types found.')
-            df[score_key] = 0
-            df['tumor_prob'+ suffix] = 0
-            df['tumor_dec'+ suffix] = 'NA'
-            # df['tumor_cluster'+ suffix] = ''
-            return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                      'tumor_prob'+suffix]]
-            # return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
-            #           'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
-        #'''
-    else:
-        cluster_sel = initially_detect_major_clusters(X_pca, y_clust, cobj, pmaj = 0.7, 
-                         cutoff = cmd_cutoff, verbose = False )        
-
-    if CLUSTERING_AGO == 'lv':
-        adj_agg = cobj.aggregate_
-        adj_agg_mat = np.array(adj_agg.todense().astype(int)) 
-    else:
-        rows = adj.tocoo().row
-        cols = adj.tocoo().col
-        vals = adj.data
-
-        adj_agg_mat = np.zeros([len(cnv_clust_lst), len(cnv_clust_lst)], dtype = int)
-        for r, c, v in zip(rows, cols, vals):
-            adj_agg_mat[y_clust[r],y_clust[c]] += 1
+            return 
 
-    cluster_size = [] 
-    for c in cnv_clust_lst:
-        b = y_clust == c
-        cluster_size.append(np.sum(b))
-    
+    seed_clusters = copy.deepcopy(cluster_sel)
     cluster_sel, cluster_odr, pair_cluster, strength_odr, threshold_odr = \
             extend_major_clusters(adj_agg_mat, cluster_sel, cluster_size, 
                                   n_neighbors = n_neighbors, 
                                   alpha = connectivity_thresh, pv_cutoff = None, 
                                   mode = net_search_mode, verbose = verbose )
     
     b = y_clust == cluster_sel[0]
     if len(cluster_sel) > 1:
         for c in cluster_sel[1:]:
             b = b | (y_clust == c)
     ref_ind2 = b
     
     etime = round(time.time() - start_time) 
-    print('NS(%i) N_ref: %i -> %i .. ' % \
-          (etime, np.sum(ref_ind), np.sum(ref_ind2)), end = '')
+    if ref_ind is None: 
+        print('NS(%i) N_ref: %i .. ' % \
+              (etime, np.sum(ref_ind2)), end = '')
+    else:
+        print('NS(%i) N_ref: %i -> %i .. ' % \
+              (etime, np.sum(ref_ind), np.sum(ref_ind2)), end = '')
     start_time = time.time()
 
-    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
     #'''
-    X_pca_sel = X_pca[ref_ind2,:]
+    X_vec_sel = X_vec[ref_ind2,:]
+    gmm_N_comp = find_num_clusters( np.sum(ref_ind2), Clustering_resolution )
     
     gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
-    gmm.fit(X_pca_sel)
-    y_conf_gmm = -gmm.score_samples(X_pca)
+    gmm.fit(X_vec_sel)
+    y_conf_gmm = -gmm.score_samples(X_vec)
     #'''
 
-    # df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm)))
     MIN_VAL = 1e-10
-    df[score_key] = np.log((y_conf)*(1/(1+np.exp(-y_conf_gmm*gcm))) + MIN_VAL) 
+    df['tumor_score'] = np.log((y_conf)*(1/(1+np.exp(-y_conf_gmm*gcm))) + MIN_VAL) 
+    # df['tumor_score'] = ((y_conf)*(1/(1+np.exp(-y_conf_gmm*gcm))) + MIN_VAL) 
     df['y_conf'] = y_conf
+    df['y_conf_gmm'] = y_conf_gmm
     df['tumor_prob'] = (1/(1+np.exp(-y_conf_gmm*gcm)))
     df['tumor_dec'] = 'Normal'
     b = df[score_key] > 0
     df.loc[b, 'tumor_dec'] = 'Tumor'
-    # df[score_key] = np.log(y_conf + 1e-10)
 
-    '''
-    yc = np.array(df[score_key])
-    odr = yc.argsort()
-    n1 = int(len(yc)*0.01)
-    n2 = int(len(yc)*0.99)
-    ymin = yc[odr[n1]]
-    ymax = yc[odr[n2]]
-    df[score_key].clip(lower=ymin, upper=ymax, inplace = True)
-    b = df[score_key] <= np.log(MIN_VAL*10)
-    mnv = df.loc[~b, score_key].min()
-    df.loc[b, score_key] = mnv
-    #'''
-    
     etime = round(time.time() - start_time) 
     print('G(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
     #'''
-    dft, td_params = get_cnv_threshold_useref( df, ref_ind2, 
+    dft, td_params = get_cnv_threshold_useref( df, ref_ind2, ref_ind,
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_max = th_max, refp_min = refp_min, p_exc = p_exc, 
                                        ucr = dec_margin, plot_stat = plot_stat, 
                                        suffix = suffix, Data = Data )
     #'''
     
     summary = {}
     summary['tumor_dec_params'] = td_params
     summary['adj_mat'] = adj
     summary['agg_adj_mat'] = adj_agg_mat
-    # summary['cluster_sizes'] = cluster_size
-    # summary['normal_clusters'] = cluster_sel
-    # summary['cluster_selection_order'] = cluster_odr
-    # summary['connection_strengths'] = strength_odr
     summary['connectivity_threshold'] = connectivity_thresh
     
-    td_params['df'].rename(columns = {'dec': 'tumor_dec'}, inplace = True)
-    df_res = td_params['df'].copy(deep = True)
     # df_res = get_cluster_stat( df, ref_ind2, cluster_key = 'cnv_cluster', 
     #                            score_key = 'tumor_score', refp_min = 0.9)
-    # df_res['Normal'] = False
-    # for c in cluster_sel: df_res.loc[c, 'Normal'] = True
+    td_params['df'].rename(columns = {'dec': 'tumor_dec'}, inplace = True)
+    df_res = td_params['df'].copy(deep = True)
+    
     df_res['cluster_size'] = cluster_size
-    df_res['selected'] = 0
-    df_res.loc[cluster_sel, 'selected'] = 1
-    df_res['selection_order'] = 0
-    df_res['paired_cluster'] = 0
-    df_res['edge_wgt'] = 0
-    df_res['threshold'] = 0
+    df_res['cluster_score'] = cluster_scores
+    df_res['seed'] = False
+    for c in seed_clusters:
+        df_res.loc[c, 'seed'] = True
+    df_res['selected'] = False
+    df_res.loc[cluster_sel, 'selected'] = True
+    df_res['selection_order'] = -1
+    df_res['paired_cluster'] = -1
+    df_res['edge_wgt'] = -1
+    df_res['threshold'] = -1
     for j, (c, p, v, u) in enumerate(zip(cluster_odr, pair_cluster, strength_odr, threshold_odr)): 
         df_res.loc[c, 'selection_order'] = j
         df_res.loc[c, 'paired_cluster'] = p
         df_res.loc[c, 'edge_wgt'] = v
         df_res.loc[c, 'threshold'] = u
-    # df_res.rename(columns = {'dec': 'tumor_dec'}, inplace = True)
     df_res.drop(columns = 'b_inc', inplace = True)
     summary['cnv_cluster_info'] = df_res    
     
     etime = round(time.time() - start_time_a) 
-    print('done (%i) ' % etime) #, end = '', flush = True)
+    print('done (%i) ' % etime) 
     
     return df, summary, cobj, X_pca
 
 
 def plot_td_stats( params, n_bins = 30, title = None, title_fs = 14,
                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
```

### Comparing `scoda-tk-0.4.0/src/scoda/misc.py` & `scoda-tk-0.4.1/src/scoda/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import time, os, copy, datetime, math, random, warnings
 import numpy as np
 import pandas as pd
-import scanpy as sc
-import seaborn as sns
-from statannot import add_stat_annotation
 import matplotlib.pyplot as plt
 from matplotlib import cm
-from MarkerCount.hicat import get_markers_cell_type, get_markers_minor_type2, get_markers_major_type
-
 from importlib_resources import files
 
+from scoda.hicat import get_markers_cell_type, get_markers_minor_type2, get_markers_major_type
+
+'''
+import scanpy as sc
+'''
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
+
+
+
 dir_gtmap = 'GTmap'
 dir_opt_files = 'default_optional_files'
 
 def load_GTmap( target = 'hg38' ):
     
     if target in ['hg38', 'hg19', 'mm10']:
         path = files('scoda.%s' % dir_gtmap).joinpath('GTmap_%s.csv' % target)
```

### Comparing `scoda-tk-0.4.0/src/scoda/pipeline.py` & `scoda-tk-0.4.1/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import time, os, copy, datetime, math, random, warnings
 import numpy as np
 import pandas as pd
-import scanpy as sc
 import anndata
 
-import gseapy as gp
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
+
+GSEAPY = True
+try:
+    import gseapy as gp
+except ImportError:
+    print('WARNING: gseapy not installed or not available. ')
+    GSEAPY = False
+
 
 def load_gmt_file(file):
     dct = {}
     with open(file, 'r') as f:
         for line in f:
             items = line.split('\t')
             dct[items[0]] = items[2:]
@@ -82,56 +94,64 @@
     
     return # adata
 
 
 def scoda_icnv_addon( adata_t, gtf_file, ref_types = None, 
                       ref_key = "celltype_major", use_ref_only = False, 
                       clustering_algo = 'lv', clustering_resolution = 1, 
-                      connectivity_thresh = 0.08, n_cores = 4, verbose = False,
-                      tumor_dec_margin = 0.05, tumor_dec_th_max = 0.1,  
-                      net_search_mode = 'max', cmd_cutoff = 0.03, gcm = 0.05 ):
+                      connectivity_threshold = 0.1, n_cores = 4, verbose = False,
+                      tumor_dec_margin = 0.05, tumor_dec_th_max = 0.5,  
+                      net_search_mode = 'max', cmd_cutoff = 0.03, gcm = 0.05, 
+                      use_umap = False ):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
-    #'''
+    '''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 1, N_pca = 15, n_neighbors = 15,
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
     pca = False
 
     df_res, summary, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, clust = None, 
                            use_cnv_score = False, Clustering_algo = clustering_algo, 
                            Clustering_resolution = clustering_resolution, N_clusters = 30,
                            gmm_N_comp = 20, th_max = tumor_dec_th_max, refp_min = 0.9, p_exc = 0.1, 
-                           dec_margin = tumor_dec_margin, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
+                           dec_margin = tumor_dec_margin, n_neighbors = 10, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
-                           connectivity_thresh = connectivity_thresh, net_search_mode = net_search_mode,
-                           suffix = '', Data = None, n_cores = n_cores, verbose = verbose)
+                           connectivity_thresh = connectivity_threshold, net_search_mode = net_search_mode,
+                           suffix = '', Data = None, n_cores = n_cores, verbose = verbose, use_umap = use_umap)
 
     if not pca: adata.obsm['X_cnv_pca'] = X_pca
         
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
     adata_t.uns['cnv'] = adata.uns['cnv']
 
     adata_t.obs['cnv_cluster'] = list(df_res['cnv_cluster'].astype(str))
     adata_t.obs['tumor_dec'] = list(df_res['tumor_dec'])
     adata_t.obs['tumor_score'] = list(df_res['tumor_score'])
+    
+    if 'log_tumor_score' in list(df_res.columns.values):
+        adata_t.obs['log_tumor_score'] = list(df_res['log_tumor_score'])
+    if 'y_conf' in list(df_res.columns.values):
+        adata_t.obs['y_conf'] = list(df_res['y_conf'])
+    if 'y_conf_gmm' in list(df_res.columns.values):
+        adata_t.obs['y_conf_gmm'] = list(df_res['y_conf_gmm'])
 
     adata_t.uns['cnv_ref_celltypes'] = ref_types2
     # summary['clustering_obj'] = cobj
     adata_t.uns['cnv_addon_summary'] = summary
 
     lst1 = list(df_res.index.values)
     lst2 = list(adata_t.obs.index.values)
@@ -146,15 +166,14 @@
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
     #'''
     return df_res
 
 
-
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
                cci_base = 'celltype_minor', unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
                data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4,
                print_prefix = ''):
     
     if cci_base in list(adata_t.obs.columns.values):
         celltype_col = cci_base
```

### Comparing `scoda-tk-0.4.0/src/scoda/viz.py` & `scoda-tk-0.4.1/src/scoda/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import time, os, copy, datetime, math, random, warnings
 import anndata
 import numpy as np
 import pandas as pd
 from scipy import stats
-import seaborn as sns
-from statannot import add_stat_annotation
 import matplotlib.pyplot as plt
 from matplotlib import cm, colormaps
-from importlib_resources import files
 import matplotlib as mpl
-
-import scanpy as sc
 from matplotlib.pyplot import figure
 from matplotlib.patches import Rectangle
 
+from importlib_resources import files
+
+SCANVPY = True
+try:
+    import scanpy as sc
+except ImportError:
+    print('WARNING: scanpy not installed.')
+    SCANVPY = False
+
+STATANNOT = True
+try:
+    from statannot import add_stat_annotation
+except ImportError:
+    print('WARNING: statannot not installed or not available. ')
+    STATANNOT = False
+
+SEABORN = True
+try:
+    import seaborn as sns
+except ImportError:
+    print('WARNING: seaborn not installed or not available. ')
+    SEABORN = False
+
 try:
     import plotly.graph_objects as go
 except ImportError:
     print('WARNING: plotly not installed.')
     
 ### Example 
 # lst = [adata_t.obs['cell_type_major_pred'], adata_t.obs['tumor_dec'], adata_t.obs['subtype']] #, 
@@ -753,19 +771,21 @@
     dfs_dct = {}
     for g in df_dct.keys():
         dfs_dct[g] = df_dct[g].loc[idxo_dct[g],:]
 
     celltype_lst.sort()
     # len(idx_c), celltype_lst
     
+    if remove_common:
+    
     return dfs_dct
 
 
 ## Get matrices summarizing the num CCIs for each condition
-def cci_get_ni_mat( dfs_dct ):
+def cci_get_ni_mat( dfs_dct, remove_common = True ):
     
     celltype_lst = []
     for j, g in enumerate(dfs_dct.keys()):
         ctA = list(dfs_dct[g]['cell_A'].unique())
         ctB = list(dfs_dct[g]['cell_B'].unique())
         celltype_lst = list(set(celltype_lst).union(ctA + ctB))
 
@@ -778,14 +798,17 @@
         df = pd.DataFrame(index = celltype_lst, columns = celltype_lst)
         df.loc[:] = 0
         for a, b in zip(dfs['cell_A'], dfs['cell_B']):
             df.loc[a,b] += 1
 
         df_lst[g] = df
         
+    if remove_common: 
+        df_lst = cci_remove_common( df_lst )
+        
     return df_lst
 
 
 def cci_get_df_to_plot( df_dct, pval_cutoff = 0.01, mean_cutoff = 1, target_cells = None ):
 
     idx_lst_all = []
     for k in df_dct.keys():
```

### Comparing `scoda-tk-0.4.0/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.1/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.0/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.1/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

