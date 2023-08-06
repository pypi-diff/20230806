# Comparing `tmp/scoda-tk-0.4.5.tar.gz` & `tmp/scoda-tk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.4.5.tar", last modified: Sun Aug  6 14:54:15 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.6.tar", last modified: Sun Aug  6 15:14:31 2023, max compression
```

## Comparing `scoda-tk-0.4.5.tar` & `scoda-tk-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:54:15.151094 scoda-tk-0.4.5/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.5/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.5/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:54:15.151094 scoda-tk-0.4.5/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.5/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:53:59.000000 scoda-tk-0.4.5/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:54:15.151094 scoda-tk-0.4.5/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.5/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:54:15.123094 scoda-tk-0.4.5/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:54:15.127094 scoda-tk-0.4.5/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.5/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.5/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:54:15.147094 scoda-tk-0.4.5/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.5/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.5/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.5/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.5/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.5/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.5/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    25684 2023-08-06 14:53:49.000000 scoda-tk-0.4.5/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.5/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:54:15.151094 scoda-tk-0.4.5/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:54:15.000000 scoda-tk-0.4.5/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 15:14:31.477949 scoda-tk-0.4.6/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.6/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.6/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 15:14:31.477949 scoda-tk-0.4.6/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.6/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 15:13:02.000000 scoda-tk-0.4.6/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 15:14:31.477949 scoda-tk-0.4.6/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.6/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 15:14:31.457949 scoda-tk-0.4.6/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 15:14:31.457949 scoda-tk-0.4.6/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.6/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.6/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 15:14:31.477949 scoda-tk-0.4.6/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.6/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.6/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.6/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.6/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37583 2023-08-06 15:14:11.000000 scoda-tk-0.4.6/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.6/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    25671 2023-08-06 15:12:43.000000 scoda-tk-0.4.6/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.6/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 15:14:31.477949 scoda-tk-0.4.6/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 15:14:31.000000 scoda-tk-0.4.6/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.4.5/LICENSE` & `scoda-tk-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/PKG-INFO` & `scoda-tk-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.5/pyproject.toml` & `scoda-tk-0.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.4.5"
+version = "0.4.6"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.4.5/src/scoda/cpdb.py` & `scoda-tk-0.4.6/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.6/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.6/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.6/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.6/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.6/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.6/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.6/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.6/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/deg.py` & `scoda-tk-0.4.6/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/gsea.py` & `scoda-tk-0.4.6/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/hicat.py` & `scoda-tk-0.4.6/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/icnv.py` & `scoda-tk-0.4.6/src/scoda/icnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import warnings, math, time, copy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn import cluster, mixture
 from sklearn.neighbors import kneighbors_graph
-from sknetwork.clustering import Louvain
 from sklearn.decomposition import PCA, IncrementalPCA, TruncatedSVD
 from scipy import stats
+from sklearn.neighbors import KNeighborsRegressor
+from sklearn.neighbors import NearestNeighbors
 
 CLUSTERING_AGO = 'lv'
 SKNETWORK = True
 try:
     from sknetwork.clustering import Louvain
 except ImportError:
     print('WARNING: sknetwork not installed. GMM will be used for clustering.')
@@ -650,31 +651,14 @@
             cnv.tl.cnv_score(adata, groupby = cluster_key, key_added = 'cnv_score')
             
         print('done.')
 
     return adata
 
 
-
-from sklearn.decomposition import PCA
-from sklearn import cluster, mixture
-from sklearn.neighbors import KNeighborsRegressor
-from sklearn.neighbors import kneighbors_graph
-from sklearn.neighbors import NearestNeighbors
-
-CLUSTERING_AGO = 'lv'
-SKNETWORK = True
-try:
-    from sknetwork.clustering import Louvain
-except ImportError:
-    print('WARNING: sknetwork not installed. GMM will be used for clustering.')
-    CLUSTERING_AGO = 'km'
-    SKNETWORK = False
-
-    
 def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10, 
                    mode='connectivity', n_cores = 4):
                    # mode='distance', n_cores = 4):
     
     adj = None
     if clust_algo[:2] == 'gm':
         gmm = mixture.GaussianMixture(n_components = int(N_clusters), random_state = 0)
```

### Comparing `scoda-tk-0.4.5/src/scoda/misc.py` & `scoda-tk-0.4.6/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda/pipeline.py` & `scoda-tk-0.4.6/src/scoda/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,21 +22,22 @@
     dct = {}
     with open(file, 'r') as f:
         for line in f:
             items = line.split('\t')
             dct[items[0]] = items[2:]
     return dct
 
+
 from scoda.icnv import run_icnv, identify_tumor_cells
 from scoda.cpdb import cpdb4_run, cpdb4_get_results, cpdb_plot, cpdb_get_gp_n_cp #, plot_circ
 from scoda.gsea import select_samples, run_enrich, run_enrichr, run_prerank
 from scoda.deg import deg_multi, get_population, plot_population
 from scoda.misc import plot_sankey_e, get_opt_files_path
 
-from scoda.hicat import HiCAT, show_summary, get_markers_major_type
+from scoda.hicat import HiCAT, get_markers_major_type
 from scoda.hicat import get_markers_cell_type, get_markers_minor_type2, load_markers_all
 
 
 def scoda_hicat(adata, mkr_db, verbose = False):
     
     X1 = adata.to_df()
```

### Comparing `scoda-tk-0.4.5/src/scoda/viz.py` & `scoda-tk-0.4.6/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.5/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.6/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.5/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.6/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

