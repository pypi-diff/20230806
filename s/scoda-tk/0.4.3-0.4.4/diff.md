# Comparing `tmp/scoda-tk-0.4.3.tar.gz` & `tmp/scoda-tk-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.4.3.tar", last modified: Sun Aug  6 14:40:23 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.4.tar", last modified: Sun Aug  6 14:47:13 2023, max compression
```

## Comparing `scoda-tk-0.4.3.tar` & `scoda-tk-0.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.037516 scoda-tk-0.4.3/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:40:02.000000 scoda-tk-0.4.3/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:40:23.037516 scoda-tk-0.4.3/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.3/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.001517 scoda-tk-0.4.3/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.001517 scoda-tk-0.4.3/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.3/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.3/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.3/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.3/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.3/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.3/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.3/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    25444 2023-08-06 14:39:49.000000 scoda-tk-0.4.3/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.3/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:40:23.033516 scoda-tk-0.4.3/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:40:22.000000 scoda-tk-0.4.3/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:47:13.868394 scoda-tk-0.4.4/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-04 16:51:18.000000 scoda-tk-0.4.4/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-04 16:51:18.000000 scoda-tk-0.4.4/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:47:13.868394 scoda-tk-0.4.4/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-04 16:51:24.000000 scoda-tk-0.4.4/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-06 14:46:59.000000 scoda-tk-0.4.4/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-06 14:47:13.868394 scoda-tk-0.4.4/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-04 16:51:18.000000 scoda-tk-0.4.4/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:47:13.848395 scoda-tk-0.4.4/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:47:13.852395 scoda-tk-0.4.4/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-04 16:51:24.000000 scoda-tk-0.4.4/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31646 2023-08-06 14:32:11.000000 scoda-tk-0.4.4/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:47:13.868394 scoda-tk-0.4.4/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-04 16:51:21.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-04 16:51:23.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-04 16:51:23.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-04 16:51:22.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-04 16:51:23.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-04 16:51:21.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-04 16:51:20.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-04 16:51:24.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-04 16:51:22.000000 scoda-tk-0.4.4/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17013 2023-08-06 13:08:04.000000 scoda-tk-0.4.4/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14381 2023-08-06 13:11:44.000000 scoda-tk-0.4.4/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-04 16:51:20.000000 scoda-tk-0.4.4/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37991 2023-08-06 14:18:36.000000 scoda-tk-0.4.4/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31437 2023-08-06 13:15:03.000000 scoda-tk-0.4.4/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    25447 2023-08-06 14:46:47.000000 scoda-tk-0.4.4/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    65443 2023-08-06 14:21:33.000000 scoda-tk-0.4.4/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-06 14:47:13.868394 scoda-tk-0.4.4/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-06 14:47:13.000000 scoda-tk-0.4.4/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.4.3/LICENSE` & `scoda-tk-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/PKG-INFO` & `scoda-tk-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.3
+Version: 0.4.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.3/pyproject.toml` & `scoda-tk-0.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.4.3"
+version = "0.4.4"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.4.3/src/scoda/cpdb.py` & `scoda-tk-0.4.4/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.4/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.4/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.4/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.4/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.4/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.4/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.4/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.4/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/deg.py` & `scoda-tk-0.4.4/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/gsea.py` & `scoda-tk-0.4.4/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/hicat.py` & `scoda-tk-0.4.4/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/icnv.py` & `scoda-tk-0.4.4/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/misc.py` & `scoda-tk-0.4.4/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda/pipeline.py` & `scoda-tk-0.4.4/src/scoda/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,15 +578,15 @@
 
             ref_types = tumor_id_ref_celltypes
 
             df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
                                    ref_key = "celltype_major", use_ref_only = False, 
                                    clustering_algo = cnv_clustering_algo, 
                                    clustering_resolution = cnv_clustering_resolution, 
-                                   connectivity_thresh = cnv_connectivity_thresh, 
+                                   connectivity_threshold = cnv_connectivity_thresh, 
                                    n_cores = n_cores_to_use, verbose = False, 
                                    tumor_dec_th_max = 0.1, tumor_dec_margin = 0.05, 
                                    net_search_mode = 'max', cmd_cutoff = 0.03, gcm = 0.05 )
             
             if verbose: print('%sTumor cells identification done. ' % print_prefix)
             # adata_t.write(file_h5ad)
```

### Comparing `scoda-tk-0.4.3/src/scoda/viz.py` & `scoda-tk-0.4.4/src/scoda/viz.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.4.3/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.4/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.4.3
+Version: 0.4.4
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.4.3/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.4/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

