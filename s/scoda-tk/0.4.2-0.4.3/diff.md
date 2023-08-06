# Comparing `tmp/scoda-tk-0.4.2.tar.gz` & `tmp/scoda-tk-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.4.2.tar", last modified: Sun Aug  6 14:32:37 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.3.tar", last modified: Sun Aug  6 14:40:23 2023, max compression
```

## Comparing `scoda-tk-0.4.2.tar` & `scoda-tk-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:32:37.707992 scoda-tk-0.4.2/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.2/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.2/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:32:37.707992 scoda-tk-0.4.2/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.2/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:32:21.000000 scoda-tk-0.4.2/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:32:37.707992 scoda-tk-0.4.2/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.2/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:32:37.691993 scoda-tk-0.4.2/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:32:37.691993 scoda-tk-0.4.2/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.2/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.2/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:32:37.707992 scoda-tk-0.4.2/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.2/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.2/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.2/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.2/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.2/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.2/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    25443 2023-08-06 14:22:59.000000 scoda-tk-0.4.2/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.2/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:32:37.707992 scoda-tk-0.4.2/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:32:37.000000 scoda-tk-0.4.2/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.037516 scoda-tk-0.4.3/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:40:02.000000 scoda-tk-0.4.3/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:40:23.037516 scoda-tk-0.4.3/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.001517 scoda-tk-0.4.3/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.001517 scoda-tk-0.4.3/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.3/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.3/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.3/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.3/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.3/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.3/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    25444 2023-08-06 14:39:49.000000 scoda-tk-0.4.3/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.3/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.4.2/LICENSE` & `scoda-tk-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/PKG-INFO` & `scoda-tk-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.2
+Version: 0.4.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.2/pyproject.toml` & `scoda-tk-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.4.2"
+version = "0.4.3"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.4.2/src/scoda/cpdb.py` & `scoda-tk-0.4.3/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.3/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.3/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.3/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.3/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.3/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.3/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/deg.py` & `scoda-tk-0.4.3/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/gsea.py` & `scoda-tk-0.4.3/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/hicat.py` & `scoda-tk-0.4.3/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/icnv.py` & `scoda-tk-0.4.3/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/misc.py` & `scoda-tk-0.4.3/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda/pipeline.py` & `scoda-tk-0.4.3/src/scoda/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     ref_ind = None
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
-    '''
+    #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
                      resolution = 1, N_pca = 15, n_neighbors = 15,
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
```

### Comparing `scoda-tk-0.4.2/src/scoda/viz.py` & `scoda-tk-0.4.3/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.2/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.3/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.2
+Version: 0.4.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.2/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.3/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

