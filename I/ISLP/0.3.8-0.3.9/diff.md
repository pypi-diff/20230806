# Comparing `tmp/ISLP-0.3.8.tar.gz` & `tmp/ISLP-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISLP-0.3.8.tar", last modified: Mon Aug 29 23:20:29 2022, max compression
+gzip compressed data, was "ISLP-0.3.9.tar", last modified: Wed Aug 31 06:26:00 2022, max compression
```

## Comparing `ISLP-0.3.8.tar` & `ISLP-0.3.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.356370 ISLP-0.3.8/
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.357253 ISLP-0.3.8/ISLP/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     4709 2022-08-25 06:11:51.000000 ISLP-0.3.8/ISLP/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      498 2022-08-29 23:20:29.357324 ISLP-0.3.8/ISLP/_version.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.323387 ISLP-0.3.8/ISLP/bart/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      695 2022-07-27 20:41:11.000000 ISLP-0.3.8/ISLP/bart/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    17277 2022-08-12 01:12:19.000000 ISLP-0.3.8/ISLP/bart/bart.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     5032 2022-08-04 23:06:14.000000 ISLP-0.3.8/ISLP/bart/likelihood.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     8721 2022-08-12 01:12:19.000000 ISLP-0.3.8/ISLP/bart/particle_tree.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     3455 2022-08-02 20:37:55.000000 ISLP-0.3.8/ISLP/bart/test_particle_pyx.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.323697 ISLP-0.3.8/ISLP/bart/tests/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      393 2022-08-12 01:12:19.000000 ISLP-0.3.8/ISLP/bart/tests/test_bart.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    17283 2022-08-02 06:44:36.000000 ISLP-0.3.8/ISLP/bart/tmpbart.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     7233 2022-08-04 23:06:14.000000 ISLP-0.3.8/ISLP/bart/tree.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      839 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/cluster.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.350558 ISLP-0.3.8/ISLP/data/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    19004 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Auto.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    30287 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Auto.data
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   567588 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Bikeshare.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    31378 2022-07-28 04:58:18.000000 ISLP-0.3.8/ISLP/data/Boston.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     5216 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/BrainCancer.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)  1013001 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Caravan.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    16628 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Carseats.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    57053 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/College.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    23417 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Credit.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   404710 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Default.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)  1781887 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Fund.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    21003 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Hitters.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   100128 2022-08-25 04:21:11.000000 ISLP-0.3.8/ISLP/data/IMDB_Y_test.npy
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   100128 2022-08-25 04:21:11.000000 ISLP-0.3.8/ISLP/data/IMDB_Y_train.npy
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   619501 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Khan_xtest.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)  1512553 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Khan_xtrain.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)       44 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Khan_ytest.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      130 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Khan_ytrain.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)  3497088 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/NCI60data.npy
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      601 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/NCI60labs.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   371105 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/NYSE.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    82975 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/OJ.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     3782 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Portfolio.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    10746 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Publication.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    94850 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Smarket.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)   396242 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Wage.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    84560 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/data/Weekly.csv
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     2797 2022-08-12 01:12:19.000000 ISLP-0.3.8/ISLP/info.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     1021 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/lasso.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.353026 ISLP-0.3.8/ISLP/models/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     1735 2022-05-26 02:34:21.000000 ISLP-0.3.8/ISLP/models/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     9058 2022-05-26 05:25:02.000000 ISLP-0.3.8/ISLP/models/columns.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    17618 2022-08-02 00:12:09.000000 ISLP-0.3.8/ISLP/models/generic_selector.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    26111 2022-08-29 20:16:20.000000 ISLP-0.3.8/ISLP/models/model_spec.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     8156 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/sklearn_wrap.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    24359 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/strategy.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.354344 ISLP-0.3.8/ISLP/models/tests/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)        0 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/tests/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      688 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/tests/test_columns.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     9890 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/tests/test_model_matrix.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     5549 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/models/tests/test_selection.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      716 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/poly.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     6935 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/pygam.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      745 2022-08-29 22:40:25.000000 ISLP-0.3.8/ISLP/survival.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     1342 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/svm.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.355480 ISLP-0.3.8/ISLP/torch/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)       80 2022-08-25 03:44:42.000000 ISLP-0.3.8/ISLP/torch/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    12919 2022-08-25 04:20:51.000000 ISLP-0.3.8/ISLP/torch/_make_imdb.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     5329 2022-08-29 17:38:33.000000 ISLP-0.3.8/ISLP/torch/imdb.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     8440 2022-08-26 05:20:01.000000 ISLP-0.3.8/ISLP/torch/lightning.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    19296 2022-07-27 23:30:52.000000 ISLP-0.3.8/ISLP/transforms.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.356121 ISLP-0.3.8/ISLP/wrappers/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)       41 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/wrappers/__init__.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     6486 2022-03-30 04:40:27.000000 ISLP-0.3.8/ISLP/wrappers/regsubsets.py
-drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-29 23:20:29.320930 ISLP-0.3.8/ISLP.egg-info/
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      927 2022-08-29 23:20:29.000000 ISLP-0.3.8/ISLP.egg-info/PKG-INFO
--rw-r--r--   0 jonathantaylor   (504) staff       (20)     1615 2022-08-29 23:20:29.000000 ISLP-0.3.8/ISLP.egg-info/SOURCES.txt
--rw-r--r--   0 jonathantaylor   (504) staff       (20)        1 2022-08-29 23:20:29.000000 ISLP-0.3.8/ISLP.egg-info/dependency_links.txt
--rw-r--r--   0 jonathantaylor   (504) staff       (20)        1 2022-05-26 07:22:10.000000 ISLP-0.3.8/ISLP.egg-info/not-zip-safe
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      255 2022-08-29 23:20:29.000000 ISLP-0.3.8/ISLP.egg-info/requires.txt
--rw-r--r--   0 jonathantaylor   (504) staff       (20)        5 2022-08-29 23:20:29.000000 ISLP-0.3.8/ISLP.egg-info/top_level.txt
--rw-r--r--   0 jonathantaylor   (504) staff       (20)       71 2022-08-25 06:53:33.000000 ISLP-0.3.8/MANIFEST.in
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      927 2022-08-29 23:20:29.356496 ISLP-0.3.8/PKG-INFO
--rw-r--r--   0 jonathantaylor   (504) staff       (20)       79 2022-03-30 04:40:27.000000 ISLP-0.3.8/README.md
--rw-r--r--   0 jonathantaylor   (504) staff       (20)      154 2022-08-29 23:20:29.356956 ISLP-0.3.8/setup.cfg
--rwxr-xr-x   0 jonathantaylor   (504) staff       (20)     8745 2022-08-18 17:50:45.000000 ISLP-0.3.8/setup.py
--rw-r--r--   0 jonathantaylor   (504) staff       (20)    80044 2022-03-30 04:40:27.000000 ISLP-0.3.8/versioneer.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.864087 ISLP-0.3.9/
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.865566 ISLP-0.3.9/ISLP/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     4709 2022-08-25 06:11:51.000000 ISLP-0.3.9/ISLP/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      498 2022-08-31 06:26:00.865682 ISLP-0.3.9/ISLP/_version.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.767011 ISLP-0.3.9/ISLP/bart/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      695 2022-07-27 20:41:11.000000 ISLP-0.3.9/ISLP/bart/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    17277 2022-08-12 01:12:19.000000 ISLP-0.3.9/ISLP/bart/bart.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     5032 2022-08-04 23:06:14.000000 ISLP-0.3.9/ISLP/bart/likelihood.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     8721 2022-08-12 01:12:19.000000 ISLP-0.3.9/ISLP/bart/particle_tree.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     3455 2022-08-02 20:37:55.000000 ISLP-0.3.9/ISLP/bart/test_particle_pyx.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.768235 ISLP-0.3.9/ISLP/bart/tests/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      410 2022-08-29 23:28:57.000000 ISLP-0.3.9/ISLP/bart/tests/test_bart.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    17283 2022-08-02 06:44:36.000000 ISLP-0.3.9/ISLP/bart/tmpbart.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     7233 2022-08-04 23:06:14.000000 ISLP-0.3.9/ISLP/bart/tree.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      839 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/cluster.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.846219 ISLP-0.3.9/ISLP/data/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    19004 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Auto.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    30287 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Auto.data
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   567588 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Bikeshare.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    31378 2022-07-28 04:58:18.000000 ISLP-0.3.9/ISLP/data/Boston.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     5216 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/BrainCancer.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)  1013001 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Caravan.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    16628 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Carseats.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    57053 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/College.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    23417 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Credit.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   404710 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Default.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)  1781887 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Fund.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    21003 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Hitters.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   100128 2022-08-25 04:21:11.000000 ISLP-0.3.9/ISLP/data/IMDB_Y_test.npy
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   100128 2022-08-25 04:21:11.000000 ISLP-0.3.9/ISLP/data/IMDB_Y_train.npy
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   619501 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Khan_xtest.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)  1512553 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Khan_xtrain.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)       44 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Khan_ytest.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      130 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Khan_ytrain.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)  3497088 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/NCI60data.npy
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      601 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/NCI60labs.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   371105 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/NYSE.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    82975 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/OJ.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     3782 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Portfolio.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    10746 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Publication.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    94850 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Smarket.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)   396242 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Wage.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    84560 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/data/Weekly.csv
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     2797 2022-08-12 01:12:19.000000 ISLP-0.3.9/ISLP/info.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     1021 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/lasso.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.854441 ISLP-0.3.9/ISLP/models/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     1735 2022-05-26 02:34:21.000000 ISLP-0.3.9/ISLP/models/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     9058 2022-05-26 05:25:02.000000 ISLP-0.3.9/ISLP/models/columns.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    17618 2022-08-02 00:12:09.000000 ISLP-0.3.9/ISLP/models/generic_selector.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    26111 2022-08-29 20:16:20.000000 ISLP-0.3.9/ISLP/models/model_spec.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     8156 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/models/sklearn_wrap.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    24359 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/models/strategy.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.857978 ISLP-0.3.9/ISLP/models/tests/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)        0 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/models/tests/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      705 2022-08-29 23:22:49.000000 ISLP-0.3.9/ISLP/models/tests/test_columns.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    10323 2022-08-29 23:25:47.000000 ISLP-0.3.9/ISLP/models/tests/test_model_matrix.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     5600 2022-08-29 23:26:21.000000 ISLP-0.3.9/ISLP/models/tests/test_selection.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      716 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/poly.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     6935 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/pygam.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      745 2022-08-29 22:40:25.000000 ISLP-0.3.9/ISLP/survival.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     1342 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/svm.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.862029 ISLP-0.3.9/ISLP/torch/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      843 2022-08-30 06:47:51.000000 ISLP-0.3.9/ISLP/torch/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    12900 2022-08-29 23:27:40.000000 ISLP-0.3.9/ISLP/torch/_make_imdb.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     5336 2022-08-29 23:27:16.000000 ISLP-0.3.9/ISLP/torch/imdb.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     8440 2022-08-26 05:20:01.000000 ISLP-0.3.9/ISLP/torch/lightning.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    19296 2022-07-27 23:30:52.000000 ISLP-0.3.9/ISLP/transforms.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.863505 ISLP-0.3.9/ISLP/wrappers/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)       41 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/wrappers/__init__.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     6486 2022-03-30 04:40:27.000000 ISLP-0.3.9/ISLP/wrappers/regsubsets.py
+drwxr-xr-x   0 jonathantaylor   (504) staff       (20)        0 2022-08-31 06:26:00.759845 ISLP-0.3.9/ISLP.egg-info/
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      927 2022-08-31 06:26:00.000000 ISLP-0.3.9/ISLP.egg-info/PKG-INFO
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)     1615 2022-08-31 06:26:00.000000 ISLP-0.3.9/ISLP.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)        1 2022-08-31 06:26:00.000000 ISLP-0.3.9/ISLP.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)        1 2022-05-26 07:22:10.000000 ISLP-0.3.9/ISLP.egg-info/not-zip-safe
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      255 2022-08-31 06:26:00.000000 ISLP-0.3.9/ISLP.egg-info/requires.txt
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)        5 2022-08-31 06:26:00.000000 ISLP-0.3.9/ISLP.egg-info/top_level.txt
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)       71 2022-08-25 06:53:33.000000 ISLP-0.3.9/MANIFEST.in
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      927 2022-08-31 06:26:00.864292 ISLP-0.3.9/PKG-INFO
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)       79 2022-03-30 04:40:27.000000 ISLP-0.3.9/README.md
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)      154 2022-08-31 06:26:00.865154 ISLP-0.3.9/setup.cfg
+-rwxr-xr-x   0 jonathantaylor   (504) staff       (20)     8745 2022-08-18 17:50:45.000000 ISLP-0.3.9/setup.py
+-rw-r--r--   0 jonathantaylor   (504) staff       (20)    80044 2022-03-30 04:40:27.000000 ISLP-0.3.9/versioneer.py
```

### Comparing `ISLP-0.3.8/ISLP/__init__.py` & `ISLP-0.3.9/ISLP/__init__.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/__init__.py` & `ISLP-0.3.9/ISLP/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/bart.py` & `ISLP-0.3.9/ISLP/bart/bart.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/likelihood.py` & `ISLP-0.3.9/ISLP/bart/likelihood.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/particle_tree.py` & `ISLP-0.3.9/ISLP/bart/particle_tree.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/test_particle_pyx.py` & `ISLP-0.3.9/ISLP/bart/test_particle_pyx.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/tmpbart.py` & `ISLP-0.3.9/ISLP/bart/tmpbart.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/bart/tree.py` & `ISLP-0.3.9/ISLP/bart/tree.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/cluster.py` & `ISLP-0.3.9/ISLP/cluster.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Auto.csv` & `ISLP-0.3.9/ISLP/data/Auto.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Auto.data` & `ISLP-0.3.9/ISLP/data/Auto.data`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Bikeshare.csv` & `ISLP-0.3.9/ISLP/data/Bikeshare.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Boston.csv` & `ISLP-0.3.9/ISLP/data/Boston.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/BrainCancer.csv` & `ISLP-0.3.9/ISLP/data/BrainCancer.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Caravan.csv` & `ISLP-0.3.9/ISLP/data/Caravan.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Carseats.csv` & `ISLP-0.3.9/ISLP/data/Carseats.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/College.csv` & `ISLP-0.3.9/ISLP/data/College.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Credit.csv` & `ISLP-0.3.9/ISLP/data/Credit.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Default.csv` & `ISLP-0.3.9/ISLP/data/Default.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Fund.csv` & `ISLP-0.3.9/ISLP/data/Fund.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Hitters.csv` & `ISLP-0.3.9/ISLP/data/Hitters.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/IMDB_Y_test.npy` & `ISLP-0.3.9/ISLP/data/IMDB_Y_test.npy`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/IMDB_Y_train.npy` & `ISLP-0.3.9/ISLP/data/IMDB_Y_train.npy`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Khan_xtest.csv` & `ISLP-0.3.9/ISLP/data/Khan_xtest.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Khan_xtrain.csv` & `ISLP-0.3.9/ISLP/data/Khan_xtrain.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/NCI60data.npy` & `ISLP-0.3.9/ISLP/data/NCI60data.npy`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/NCI60labs.csv` & `ISLP-0.3.9/ISLP/data/NCI60labs.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/NYSE.csv` & `ISLP-0.3.9/ISLP/data/NYSE.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/OJ.csv` & `ISLP-0.3.9/ISLP/data/OJ.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Portfolio.csv` & `ISLP-0.3.9/ISLP/data/Portfolio.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Publication.csv` & `ISLP-0.3.9/ISLP/data/Publication.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Smarket.csv` & `ISLP-0.3.9/ISLP/data/Smarket.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Wage.csv` & `ISLP-0.3.9/ISLP/data/Wage.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/data/Weekly.csv` & `ISLP-0.3.9/ISLP/data/Weekly.csv`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/info.py` & `ISLP-0.3.9/ISLP/info.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/lasso.py` & `ISLP-0.3.9/ISLP/lasso.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/__init__.py` & `ISLP-0.3.9/ISLP/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/columns.py` & `ISLP-0.3.9/ISLP/models/columns.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/generic_selector.py` & `ISLP-0.3.9/ISLP/models/generic_selector.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/model_spec.py` & `ISLP-0.3.9/ISLP/models/model_spec.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/sklearn_wrap.py` & `ISLP-0.3.9/ISLP/models/sklearn_wrap.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/strategy.py` & `ISLP-0.3.9/ISLP/models/strategy.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/models/tests/test_columns.py` & `ISLP-0.3.9/ISLP/models/tests/test_columns.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from sklearn.base import clone
 
 from pandas.api.types import CategoricalDtype
 from ..columns import _get_column_info
 
 def test_column_info():
 
+    rng = np.random.default_rng(0)
     cat_type = CategoricalDtype(categories=list("abcd"), ordered=True)
-    df = pd.DataFrame(np.random.standard_normal((50, 5)), columns=['Aa', 'B', 'Ccc', 'D', 'E'])
-    df['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
-    df['D'] = pd.Categorical(np.random.choice(['a','b','c','d'], 50, replace=True))
+    df = pd.DataFrame(rng.standard_normal((50, 5)), columns=['Aa', 'B', 'Ccc', 'D', 'E'])
+    df['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
+    df['D'] = pd.Categorical(rng.choice(['a','b','c','d'], 50, replace=True))
     df['D'].astype(cat_type)
     print(_get_column_info(df,
                            df.columns,
                            [False]*4+[True],
                            [False]*5))
```

### Comparing `ISLP-0.3.8/ISLP/models/tests/test_model_matrix.py` & `ISLP-0.3.9/ISLP/models/tests/test_model_matrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,78 +7,84 @@
 from sklearn.preprocessing import (OneHotEncoder,
                                    OrdinalEncoder)
 from sklearn.decomposition import PCA
 
 default_encoders = {'categorical': Contrast(method=None),
                     'ordinal': OrdinalEncoder()}
 
+
 def test_interaction():
 
+    rng = np.random.default_rng(0)
     I = Interaction(['V', 'U'],
                     {'V':[0,2],
                      'U':[1,3,5]},
                     {'V':[0,1],'U':[0,1,2]})
-    X = np.random.standard_normal((50,10))
+    X = rng.standard_normal((50,10))
     W = I.fit_transform(X)
 
     W2 = np.array([X[:,0]*X[:,1],
                    X[:,0]*X[:,3],
                    X[:,0]*X[:,5],
                    X[:,2]*X[:,1],
                    X[:,2]*X[:,3],
                    X[:,2]*X[:,5]]).T
     print(np.linalg.norm(W-W2))
     print(W.columns)
 
 def test_ndarray():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(1)
+    X = rng.standard_normal((50,5))
 
     M = ModelSpec(terms=[1, (3,2)],
                   default_encoders=default_encoders)
     M.fit(X)
     MX = M.transform(X)
 
     np.testing.assert_allclose(X[:,1], MX[:,1])
     np.testing.assert_allclose(X[:,2] * X[:,3], MX[:,2])
     
 def test_dataframe1():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(2)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     
     M = ModelSpec(terms=['A','D',('D','E')],
                   default_encoders=default_encoders)
     clone(M)
     MX = np.asarray(M.fit_transform(D))
 
     np.testing.assert_allclose(X[:,0], MX[:,1])
     np.testing.assert_allclose(X[:,3], MX[:,2])
     np.testing.assert_allclose(X[:,3]*X[:,4], MX[:,3])    
 
 def test_dataframe2():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(3)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['V','B','A','D','E'])
     
     M = ModelSpec(terms=['A', 'D', 'B', ('D','E'), 'V'],
                   default_encoders=default_encoders)
     clone(M)
 
     MX = M.fit_transform(D)
 
     X2 = D.copy()
     MX2 = M.transform(D)
     np.testing.assert_allclose(MX, MX2)
     
 def test_dataframe3():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(8)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     M = ModelSpec(terms=['A', 'E', ('D','E')],
                   default_encoders=default_encoders)
     MX = np.asarray(M.fit_transform(D))
     M2 = clone(M)
 
     DE = pd.get_dummies(D['E'])
@@ -88,18 +94,19 @@
 
     X2 = D.copy()
     MX2 = M.transform(D)
     np.testing.assert_allclose(MX, MX2)
 
 def test_dataframe4():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(9)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     M = ModelSpec(terms=['A', 'E', ('D','E'), 'D'],
                   default_encoders=default_encoders)
     MX = np.asarray(M.fit_transform(D))
 
     DE = pd.get_dummies(D['E'])
     np.testing.assert_allclose(X[:,0], MX[:,1])
@@ -112,99 +119,105 @@
     np.testing.assert_allclose(MX, MX2)
 
     print(MX2.columns)
     return M, D
     
 def test_dataframe5():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(10)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     M = ModelSpec(terms=['A', 'E', ('D','E')],
                   default_encoders=default_encoders)
     MX = np.asarray(M.fit_transform(D))
 
     # check they agree on copy of dataframe
 
     X2 = D.copy()
     MX2 = M.transform(D)
     np.testing.assert_allclose(MX, MX2)
     
 def test_dataframe6():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(11)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     W = Variable(('A','E'), 'AE', None)
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     M = ModelSpec(terms=['A',W,(W,'D',)],
                   default_encoders=default_encoders)
     MX = M.fit_transform(D)
 
     MX = np.asarray(MX)
 
 def test_dataframe7():
     
-    X = np.random.standard_normal((50,6))
+    rng = np.random.default_rng(12)
+    X = rng.standard_normal((50,6))
     D = pd.DataFrame(X, columns=['AA','Bbbb','C','Ddd','Y','Eee'])
-    D['Ddd'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['Eee'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['Ddd'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['Eee'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
         
     M = ModelSpec(terms=D.columns.drop(['Y','C']),
                   default_encoders=default_encoders)
     MX = M.fit_transform(D)
     print(MX.columns)
     MX = np.asarray(MX)
 
 def test_dataframe8():
     
-    X = np.random.standard_normal((50,6))
+    rng = np.random.default_rng(13)
+    X = rng.standard_normal((50,6))
     D = pd.DataFrame(X, columns=['A','B','C','D','Y','E'])
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     poly =  Poly(degree=3)
     # raises a ValueError because poly will have been already fit -- need new instance of Poly
     W = Variable(('A',), 'poly(A)', poly)
     M = ModelSpec(terms=list(D.columns.drop(['Y','C'])) + [(W,'E')],
                   default_encoders=default_encoders)
     MX = M.fit_transform(D)
 
     print(MX.columns)
     MX = np.asarray(MX)
 
 def test_dataframe9():
     
-    X = np.random.standard_normal((50,6))
+    rng = np.random.default_rng(14)
+    X = rng.standard_normal((50,6))
     D = pd.DataFrame(X, columns=['A','B','C','D','Y','E'])
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     poly =  Poly(degree=3)
     # raises a ValueError because poly will have been already fit -- need new instance of Poly
     W = Variable(('A',), 'poly(A)', poly)
     U = Variable(('B',), 'poly(B)', clone(poly))
     M = ModelSpec(terms=list(D.columns.drop(['Y','C'])) + [W,U],
                   default_encoders=default_encoders)
     MX = M.fit_transform(D)
 
     print(MX.columns)
     MX = np.asarray(MX)
 
 def test_dataframe10():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(15)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     W = Variable(('A','E'), 'AE', None)
     U = Variable((W, 'C'), 'WC', None)
-    D['D'] = pd.Categorical(np.random.choice(['a','b','c'], 50, replace=True))
-    D['E'] = pd.Categorical(np.random.choice(range(4,8), 50, replace=True))
+    D['D'] = pd.Categorical(rng.choice(['a','b','c'], 50, replace=True))
+    D['E'] = pd.Categorical(rng.choice(range(4,8), 50, replace=True))
     
     M = ModelSpec(terms=['A', 'E', 'C', W, (W, 'D',), U],
                   default_encoders=default_encoders)
     MX = M.fit_transform(D)
     print(MX.columns)
     MX = np.asarray(MX)
 
@@ -212,15 +225,16 @@
     V2 = np.column_stack([MX[:,M.column_map_['A']],
                           MX[:,M.column_map_['E']],
                           MX[:,M.column_map_['C']]])
     print(np.linalg.norm(V-V2))
 
 def test_poly_ns_bs():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(16)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     
     M = ModelSpec(terms=[poly('A', intercept=True, degree=3),
                          ns('E', df=5),
                          bs('D', df=4)])
 
     MX = M.fit_transform(D)
@@ -230,68 +244,73 @@
                           bs('D', df=4)])
     MX2 = M2.fit_transform(D)
     print(MX.columns)
     print(MX2.columns)
 
 def test_submodel():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(17)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     
     M = ModelSpec(terms=[poly('A', intercept=True, degree=3),
                          ns('E', df=5),
                          bs('D', df=4)])
 
     M.fit(D)
     MX = M.transform(D)
     MXsub = M.build_submodel(D, M.terms[:2])
     print(MX.columns)
     print(MXsub.columns)
 
 def test_contrast():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(18)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
-    D['C'] = pd.Categorical(np.random.choice(range(4,9), 50, replace=True))
+    D['C'] = pd.Categorical(rng.choice(range(4,9), 50, replace=True))
     for method in ['sum', 'drop', None, lambda p: np.identity(p)]:
         M = ModelSpec(terms=[poly('A', intercept=True, degree=3),
                              contrast('C', method),
                              bs('D', df=4)])
 
         M.fit(D)
         MX = M.transform(D)
         MXsub = M.build_submodel(D, M.terms[:2])
         print(method, MX.columns)
     print(MXsub.columns)
     
 def test_sequence():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(19)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
     
     M = ModelSpec(terms=[poly('A', intercept=True, degree=3),
                          ns('E', df=5),
                          bs('D', df=4)])
     M.fit(D)
     for df in M.build_sequence(D):
         print(df.columns)
     
 def test_poly_ns_bs2():
     
-    X = np.random.standard_normal((50,5))
+    rng = np.random.default_rng(20)
+    X = rng.standard_normal((50,5))
     D = pd.DataFrame(X, columns=['A','B','C','D','E'])
-    D['C'] = pd.Categorical(np.random.choice(range(4,9), 50, replace=True))
+    D['C'] = pd.Categorical(rng.choice(range(4,9), 50, replace=True))
     M = ModelSpec(terms=[(poly('A', intercept=True, degree=3),'C')])
     MX = M.fit_transform(D)
     print(MX.columns)
 
     
 def test_pca():
     
-    X = np.random.standard_normal((50,8))
+    rng = np.random.default_rng(21)
+    X = rng.standard_normal((50,8))
     D = pd.DataFrame(X, columns=['A','B','C','D','E', 'F', 'G', 'H'])
     
     pca_ = Variable(('A','B','C','D'), 'pca(ABCD)', PCA(n_components=2))
     M = ModelSpec(terms=[poly('F', intercept=True, degree=3),
                          pca_])
 
     MX = M.fit_transform(D)
```

### Comparing `ISLP-0.3.8/ISLP/models/tests/test_selection.py` & `ISLP-0.3.9/ISLP/models/tests/test_selection.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 from ISLP.models import ModelSpec as MS
 from ISLP.models.strategy import min_max, Stepwise, validator_from_constraints
 from ISLP.models.generic_selector import FeatureSelector
 
 def test_min_max():
 
+    rng = np.random.default_rng(0)
     n, p = 100, 7
-    X = np.random.standard_normal((n, p))
-    Y = np.random.standard_normal(n)
+    X = rng.standard_normal((n, p))
+    Y = rng.standard_normal(n)
     D = pd.DataFrame(X, columns=['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'][:p])
-    D['A'] = pd.Categorical(np.random.choice(range(5), (n,), replace=True))
+    D['A'] = pd.Categorical(rng.choice(range(5), (n,), replace=True))
 
     model_spec = MS(list(D.columns))
     model_spec.fit(D)
 
     strategy = min_max(model_spec,
                        min_terms=1,
                        max_terms=len(model_spec.terms),
@@ -36,18 +37,19 @@
     print('selected')
     print(min_max_selector.selected_state_)
     print(min_max_selector.results_[min_max_selector.selected_state_])
 
 def test_step():
 
     n, p = 100, 7
-    X = np.random.standard_normal((n, p))
-    Y = np.random.standard_normal(n)
+    rng = np.random.default_rng(1)
+    X = rng.standard_normal((n, p))
+    Y = rng.standard_normal(n)
     D = pd.DataFrame(X, columns=['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'][:p])
-    D['A'] = pd.Categorical(np.random.choice(range(5), (n,), replace=True))
+    D['A'] = pd.Categorical(rng.choice(range(5), (n,), replace=True))
 
     model_spec = MS(list(D.columns))
     model_spec.fit(D)
 
     for (direction,
          upper_terms,
          lower_terms) in product(['forward',
@@ -110,19 +112,20 @@
 
         print(step_selector.results_)
         print(step_selector.selected_state_)
         print('huh')
         
 def test_constraint():
 
+    rng = np.random.default_rng(3)
     n, p = 100, 7
-    X = np.random.standard_normal((n, p))
-    Y = np.random.standard_normal(n)
+    X = rng.standard_normal((n, p))
+    Y = rng.standard_normal(n)
     D = pd.DataFrame(X, columns=['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'][:p])
-    D['A'] = pd.Categorical(np.random.choice(range(5), (n,), replace=True))
+    D['A'] = pd.Categorical(rng.choice(range(5), (n,), replace=True))
 
     model_spec = MS(list(D.columns))
     model_spec.fit(D)
 
     constraints = np.zeros((len(model_spec.terms),)*2)
     constraints[3,4] = 1
     constraints[4,5] = 1
```

### Comparing `ISLP-0.3.8/ISLP/poly.py` & `ISLP-0.3.9/ISLP/poly.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/pygam.py` & `ISLP-0.3.9/ISLP/pygam.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/survival.py` & `ISLP-0.3.9/ISLP/survival.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/svm.py` & `ISLP-0.3.9/ISLP/svm.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/torch/_make_imdb.py` & `ISLP-0.3.9/ISLP/torch/_make_imdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,14 @@
 """
 import pickle
 
 import numpy as np
 from scipy.sparse import coo_matrix, save_npz
 import torch
 
-np.random.seed(1)
-
 try:
     from keras.datasets import imdb
     from tensorflow.keras.preprocessing.sequence \
         import pad_sequences
 except:
     raise ImportError('requires keras.datasets')
```

### Comparing `ISLP-0.3.8/ISLP/torch/imdb.py` & `ISLP-0.3.9/ISLP/torch/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,18 +82,18 @@
     X_test, X_train = [load_npz(_get_imdb(f'IMDB_{r}', root))
                        for r in ['X_test.npz',
                                  'X_train.npz']]
     Y_test, Y_train = [np.load(_get_imdb(f'IMDB_{r}', root))
                        for r in ['Y_test.npy',
                                  'Y_train.npy']]
     
-    np.random.seed(random_state)
+    rng = np.random.default_rng(random_state)
     mask = np.zeros(X_train.shape[0], bool)
     mask[:-int(validation)] = 1
-    np.random.shuffle(mask)
+    rng.shuffle(mask)
     
     X_train_tmp, Y_train_tmp = X_train, Y_train
     X_train, Y_train = X_train_tmp[mask], Y_train_tmp[mask]
     X_valid, Y_valid = X_train_tmp[~mask], Y_train_tmp[~mask]
 
     return (X_train, Y_train), (X_valid, Y_valid), (X_test, Y_test)
```

### Comparing `ISLP-0.3.8/ISLP/torch/lightning.py` & `ISLP-0.3.9/ISLP/torch/lightning.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/transforms.py` & `ISLP-0.3.9/ISLP/transforms.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP/wrappers/regsubsets.py` & `ISLP-0.3.9/ISLP/wrappers/regsubsets.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/ISLP.egg-info/PKG-INFO` & `ISLP-0.3.9/ISLP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISLP
-Version: 0.3.8
+Version: 0.3.9
 Summary: Testing a fixed value of lambda
 Home-page: http://github.org/jonathan.taylor/ISLP
 Download-URL: 
 Author: ISLP authors
 Author-email: 
 Maintainer: Jonathan Taylor
 Maintainer-email:
```

### Comparing `ISLP-0.3.8/ISLP.egg-info/SOURCES.txt` & `ISLP-0.3.9/ISLP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/PKG-INFO` & `ISLP-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISLP
-Version: 0.3.8
+Version: 0.3.9
 Summary: Testing a fixed value of lambda
 Home-page: http://github.org/jonathan.taylor/ISLP
 Download-URL: 
 Author: ISLP authors
 Author-email: 
 Maintainer: Jonathan Taylor
 Maintainer-email:
```

### Comparing `ISLP-0.3.8/setup.py` & `ISLP-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `ISLP-0.3.8/versioneer.py` & `ISLP-0.3.9/versioneer.py`

 * *Files identical despite different names*

