# Comparing `tmp/bebi103-0.1.8.tar.gz` & `tmp/bebi103-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bebi103-0.1.8.tar", last modified: Wed Mar 17 04:30:46 2021, max compression
+gzip compressed data, was "bebi103-0.1.9.tar", last modified: Wed Nov 17 09:57:34 2021, max compression
```

## Comparing `bebi103-0.1.8.tar` & `bebi103-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.098114 bebi103-0.1.8/
--rw-r--r--   0 bois       (501) staff       (20)       90 2020-09-01 08:17:13.000000 bebi103-0.1.8/.gitignore
--rw-r--r--   0 bois       (501) staff       (20)     1482 2017-09-01 06:50:32.000000 bebi103-0.1.8/LICENSE.md
--rw-r--r--   0 bois       (501) staff       (20)       42 2017-09-01 06:50:32.000000 bebi103-0.1.8/MANIFEST.in
--rw-r--r--   0 bois       (501) staff       (20)      841 2021-03-17 04:30:46.098313 bebi103-0.1.8/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)      249 2020-09-02 09:32:39.000000 bebi103-0.1.8/README.md
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.006929 bebi103-0.1.8/bebi103/
--rw-r--r--   0 bois       (501) staff       (20)       13 2021-01-01 20:40:56.000000 bebi103-0.1.8/bebi103/.gitignore
--rw-r--r--   0 bois       (501) staff       (20)     1262 2021-03-17 04:28:08.000000 bebi103-0.1.8/bebi103/__init__.py
--rw-r--r--   0 bois       (501) staff       (20)    17330 2021-01-01 20:40:56.000000 bebi103-0.1.8/bebi103/bootstrap.py
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.015097 bebi103-0.1.8/bebi103/deprecated/
--rw-r--r--   0 bois       (501) staff       (20)     1621 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/bootstrap_deprecated.py
--rw-r--r--   0 bois       (501) staff       (20)    15082 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/emcee.py
--rw-r--r--   0 bois       (501) staff       (20)    30945 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/hotdists.py
--rw-r--r--   0 bois       (501) staff       (20)     1581 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/make_hot.py
--rw-r--r--   0 bois       (501) staff       (20)    21252 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/pm.py
--rw-r--r--   0 bois       (501) staff       (20)    22381 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/stan_deprecated.py
--rw-r--r--   0 bois       (501) staff       (20)     4049 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/deprecated/tools.py
--rw-r--r--   0 bois       (501) staff       (20)    29874 2021-01-02 18:54:52.000000 bebi103-0.1.8/bebi103/deprecated/viz_deprecated.py
--rw-r--r--   0 bois       (501) staff       (20)    30977 2021-03-15 18:00:39.000000 bebi103-0.1.8/bebi103/gp.py
--rw-r--r--   0 bois       (501) staff       (20)     5812 2021-01-01 20:40:56.000000 bebi103-0.1.8/bebi103/hv.py
--rw-r--r--   0 bois       (501) staff       (20)    43865 2021-03-04 20:04:15.000000 bebi103-0.1.8/bebi103/image.py
--rw-r--r--   0 bois       (501) staff       (20)    64957 2021-03-04 20:04:16.000000 bebi103-0.1.8/bebi103/stan.py
--rw-r--r--   0 bois       (501) staff       (20)      510 2021-01-01 20:40:56.000000 bebi103-0.1.8/bebi103/stan_int_rng.stan
--rw-r--r--   0 bois       (501) staff       (20)      366 2021-01-01 20:40:56.000000 bebi103-0.1.8/bebi103/stan_real_rng.stan
--rw-r--r--   0 bois       (501) staff       (20)     7984 2021-01-01 20:40:57.000000 bebi103-0.1.8/bebi103/utils.py
--rw-r--r--   0 bois       (501) staff       (20)    93030 2021-03-05 00:21:32.000000 bebi103-0.1.8/bebi103/viz.py
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.010081 bebi103-0.1.8/bebi103.egg-info/
--rw-r--r--   0 bois       (501) staff       (20)      841 2021-03-17 04:30:45.000000 bebi103-0.1.8/bebi103.egg-info/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)     1563 2021-03-17 04:30:45.000000 bebi103-0.1.8/bebi103.egg-info/SOURCES.txt
--rw-r--r--   0 bois       (501) staff       (20)        1 2021-03-17 04:30:45.000000 bebi103-0.1.8/bebi103.egg-info/dependency_links.txt
--rw-r--r--   0 bois       (501) staff       (20)      105 2021-03-17 04:30:45.000000 bebi103-0.1.8/bebi103.egg-info/requires.txt
--rw-r--r--   0 bois       (501) staff       (20)        8 2021-03-17 04:30:45.000000 bebi103-0.1.8/bebi103.egg-info/top_level.txt
--rw-r--r--   0 bois       (501) staff       (20)      939 2021-03-17 04:27:48.000000 bebi103-0.1.8/codemeta.json
--rw-r--r--   0 bois       (501) staff       (20)     1092 2017-09-01 06:50:11.000000 bebi103-0.1.8/copyright.txt
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.018865 bebi103-0.1.8/doc/
--rw-r--r--   0 bois       (501) staff       (20)        7 2020-09-01 08:18:06.000000 bebi103-0.1.8/doc/.gitignore
--rw-r--r--   0 bois       (501) staff       (20)      634 2020-08-06 20:14:02.000000 bebi103-0.1.8/doc/Makefile
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.020148 bebi103-0.1.8/doc/_static/
--rw-r--r--   0 bois       (501) staff       (20)      731 2020-08-06 20:14:02.000000 bebi103-0.1.8/doc/_static/custom.css
--rw-r--r--   0 bois       (501) staff       (20)   401764 2020-08-06 20:14:48.000000 bebi103-0.1.8/doc/_static/logo.png
--rw-r--r--   0 bois       (501) staff       (20)     5674 2020-08-07 21:24:09.000000 bebi103-0.1.8/doc/conf.py
--rw-r--r--   0 bois       (501) staff       (20)      825 2020-09-02 09:33:58.000000 bebi103-0.1.8/doc/credits_and_citation.rst
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.023297 bebi103-0.1.8/doc/getting_started/
--rw-r--r--   0 bois       (501) staff       (20)      989 2020-09-02 09:25:54.000000 bebi103-0.1.8/doc/getting_started/installation.rst
--rw-r--r--   0 bois       (501) staff       (20)     1530 2021-03-01 09:25:19.000000 bebi103-0.1.8/doc/getting_started/purpose.rst
--rw-r--r--   0 bois       (501) staff       (20)      692 2020-09-02 09:21:05.000000 bebi103-0.1.8/doc/index.rst
--rw-r--r--   0 bois       (501) staff       (20)      795 2020-08-06 20:14:02.000000 bebi103-0.1.8/doc/make.bat
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.077812 bebi103-0.1.8/doc/user_guide/
--rw-r--r--   0 bois       (501) staff       (20)       84 2020-08-27 06:17:35.000000 bebi103-0.1.8/doc/user_guide/.gitignore
--rw-r--r--   0 bois       (501) staff       (20)     1972 2021-03-17 04:29:05.000000 bebi103-0.1.8/doc/user_guide/api.rst
--rw-r--r--   0 bois       (501) staff       (20)   435859 2020-09-02 09:16:21.000000 bebi103-0.1.8/doc/user_guide/bootstrap.ipynb
--rw-r--r--   0 bois       (501) staff       (20)  6018831 2020-09-02 07:40:50.000000 bebi103-0.1.8/doc/user_guide/hv.ipynb
--rw-r--r--   0 bois       (501) staff       (20)      791 2020-09-02 09:20:36.000000 bebi103-0.1.8/doc/user_guide/image.ipynb
--rw-r--r--   0 bois       (501) staff       (20)     2461 2020-09-01 16:37:34.000000 bebi103-0.1.8/doc/user_guide/sample_data.csv
--rw-r--r--   0 bois       (501) staff       (20)     1006 2020-09-01 16:37:13.000000 bebi103-0.1.8/doc/user_guide/sample_data.py
--rw-r--r--   0 bois       (501) staff       (20)     1570 2020-08-30 06:06:18.000000 bebi103-0.1.8/doc/user_guide/sample_model.stan
--rw-r--r--   0 bois       (501) staff       (20)     1642 2020-09-01 17:18:07.000000 bebi103-0.1.8/doc/user_guide/sample_model_noncentered.stan
--rw-r--r--   0 bois       (501) staff       (20)      914 2020-08-31 07:51:12.000000 bebi103-0.1.8/doc/user_guide/sample_model_prior_predictive.stan
--rw-r--r--   0 bois       (501) staff       (20)  2710020 2021-01-03 04:04:37.000000 bebi103-0.1.8/doc/user_guide/sbc_results.csv
--rw-r--r--   0 bois       (501) staff       (20) 13264972 2021-03-08 19:34:26.000000 bebi103-0.1.8/doc/user_guide/stan.ipynb
--rw-r--r--   0 bois       (501) staff       (20)  3034584 2020-09-02 07:40:52.000000 bebi103-0.1.8/doc/user_guide/using_user_guide.ipynb
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.091162 bebi103-0.1.8/legacy/
--rw-r--r--   0 bois       (501) staff       (20)    61231 2017-09-01 06:50:11.000000 bebi103-0.1.8/legacy/bebi103.py
--rw-r--r--   0 bois       (501) staff       (20)    50639 2017-09-03 19:57:01.000000 bebi103-0.1.8/legacy/bebi103_original.py
--rw-r--r--   0 bois       (501) staff       (20)      104 2021-03-01 09:27:29.000000 bebi103-0.1.8/requirements.txt
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.093423 bebi103-0.1.8/sandbox/
--rw-r--r--   0 bois       (501) staff       (20)     2626 2017-09-01 06:53:20.000000 bebi103-0.1.8/sandbox/bokeh_mcmc.py
--rw-r--r--   0 bois       (501) staff       (20)      108 2021-03-17 04:30:46.098829 bebi103-0.1.8/setup.cfg
--rw-r--r--   0 bois       (501) staff       (20)     2192 2019-06-04 21:50:44.000000 bebi103-0.1.8/setup.py
--rw-r--r--   0 bois       (501) staff       (20)     2644 2017-09-01 06:50:11.000000 bebi103-0.1.8/test_bebi103.py
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-03-17 04:30:46.096457 bebi103-0.1.8/tests/
--rw-r--r--   0 bois       (501) staff       (20)        0 2017-09-01 06:50:32.000000 bebi103-0.1.8/tests/__init__.py
--rw-r--r--   0 bois       (501) staff       (20)     6996 2018-10-09 17:03:13.000000 bebi103-0.1.8/tests/frog_tongue_adhesion.csv
--rw-r--r--   0 bois       (501) staff       (20)     2644 2017-09-01 06:52:16.000000 bebi103-0.1.8/tests/test_bebi103.py
--rw-r--r--   0 bois       (501) staff       (20)      102 2017-09-01 06:50:32.000000 bebi103-0.1.8/tests/test_sample.py
--rw-r--r--   0 bois       (501) staff       (20)   257997 2018-10-11 16:55:30.000000 bebi103-0.1.8/tests/test_viz.ipynb
--rw-r--r--   0 bois       (501) staff       (20)      449 2017-09-01 06:50:32.000000 bebi103-0.1.8/update_docs.sh
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.991396 bebi103-0.1.9/
+-rw-r--r--   0 bois       (501) staff       (20)       90 2020-09-01 08:17:13.000000 bebi103-0.1.9/.gitignore
+-rw-r--r--   0 bois       (501) staff       (20)     1482 2017-09-01 06:50:32.000000 bebi103-0.1.9/LICENSE.md
+-rw-r--r--   0 bois       (501) staff       (20)       42 2017-09-01 06:50:32.000000 bebi103-0.1.9/MANIFEST.in
+-rw-r--r--   0 bois       (501) staff       (20)      807 2021-11-17 09:57:34.991659 bebi103-0.1.9/PKG-INFO
+-rw-r--r--   0 bois       (501) staff       (20)      249 2020-09-02 09:32:39.000000 bebi103-0.1.9/README.md
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.862982 bebi103-0.1.9/bebi103/
+-rw-r--r--   0 bois       (501) staff       (20)       13 2021-01-01 20:40:56.000000 bebi103-0.1.9/bebi103/.gitignore
+-rw-r--r--   0 bois       (501) staff       (20)     1262 2021-11-17 09:55:54.000000 bebi103-0.1.9/bebi103/__init__.py
+-rw-r--r--   0 bois       (501) staff       (20)    17330 2021-01-01 20:40:56.000000 bebi103-0.1.9/bebi103/bootstrap.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.869851 bebi103-0.1.9/bebi103/deprecated/
+-rw-r--r--   0 bois       (501) staff       (20)     1621 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/bootstrap_deprecated.py
+-rw-r--r--   0 bois       (501) staff       (20)    15082 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/emcee.py
+-rw-r--r--   0 bois       (501) staff       (20)    30945 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/hotdists.py
+-rw-r--r--   0 bois       (501) staff       (20)     1581 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/make_hot.py
+-rw-r--r--   0 bois       (501) staff       (20)    21252 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/pm.py
+-rw-r--r--   0 bois       (501) staff       (20)    22381 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/stan_deprecated.py
+-rw-r--r--   0 bois       (501) staff       (20)     4049 2021-01-01 20:40:57.000000 bebi103-0.1.9/bebi103/deprecated/tools.py
+-rw-r--r--   0 bois       (501) staff       (20)    29874 2021-01-02 18:54:52.000000 bebi103-0.1.9/bebi103/deprecated/viz_deprecated.py
+-rw-r--r--   0 bois       (501) staff       (20)    30977 2021-03-15 18:00:39.000000 bebi103-0.1.9/bebi103/gp.py
+-rw-r--r--   0 bois       (501) staff       (20)     5812 2021-01-01 20:40:56.000000 bebi103-0.1.9/bebi103/hv.py
+-rw-r--r--   0 bois       (501) staff       (20)    43865 2021-03-04 20:04:15.000000 bebi103-0.1.9/bebi103/image.py
+-rw-r--r--   0 bois       (501) staff       (20)    64957 2021-03-04 20:04:16.000000 bebi103-0.1.9/bebi103/stan.py
+-rw-r--r--   0 bois       (501) staff       (20)      510 2021-01-01 20:40:56.000000 bebi103-0.1.9/bebi103/stan_int_rng.stan
+-rw-r--r--   0 bois       (501) staff       (20)      366 2021-01-01 20:40:56.000000 bebi103-0.1.9/bebi103/stan_real_rng.stan
+-rw-r--r--   0 bois       (501) staff       (20)     7978 2021-11-17 09:00:13.000000 bebi103-0.1.9/bebi103/utils.py
+-rw-r--r--   0 bois       (501) staff       (20)    93367 2021-11-17 08:36:00.000000 bebi103-0.1.9/bebi103/viz.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.864606 bebi103-0.1.9/bebi103.egg-info/
+-rw-r--r--   0 bois       (501) staff       (20)      807 2021-11-17 09:57:34.000000 bebi103-0.1.9/bebi103.egg-info/PKG-INFO
+-rw-r--r--   0 bois       (501) staff       (20)     1563 2021-11-17 09:57:34.000000 bebi103-0.1.9/bebi103.egg-info/SOURCES.txt
+-rw-r--r--   0 bois       (501) staff       (20)        1 2021-11-17 09:57:34.000000 bebi103-0.1.9/bebi103.egg-info/dependency_links.txt
+-rw-r--r--   0 bois       (501) staff       (20)      105 2021-11-17 09:57:34.000000 bebi103-0.1.9/bebi103.egg-info/requires.txt
+-rw-r--r--   0 bois       (501) staff       (20)        8 2021-11-17 09:57:34.000000 bebi103-0.1.9/bebi103.egg-info/top_level.txt
+-rw-r--r--   0 bois       (501) staff       (20)      939 2021-11-17 09:56:25.000000 bebi103-0.1.9/codemeta.json
+-rw-r--r--   0 bois       (501) staff       (20)     1092 2017-09-01 06:50:11.000000 bebi103-0.1.9/copyright.txt
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.877472 bebi103-0.1.9/doc/
+-rw-r--r--   0 bois       (501) staff       (20)        7 2020-09-01 08:18:06.000000 bebi103-0.1.9/doc/.gitignore
+-rw-r--r--   0 bois       (501) staff       (20)      634 2020-08-06 20:14:02.000000 bebi103-0.1.9/doc/Makefile
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.878720 bebi103-0.1.9/doc/_static/
+-rw-r--r--   0 bois       (501) staff       (20)      731 2020-08-06 20:14:02.000000 bebi103-0.1.9/doc/_static/custom.css
+-rw-r--r--   0 bois       (501) staff       (20)   401764 2020-08-06 20:14:48.000000 bebi103-0.1.9/doc/_static/logo.png
+-rw-r--r--   0 bois       (501) staff       (20)     5674 2020-08-07 21:24:09.000000 bebi103-0.1.9/doc/conf.py
+-rw-r--r--   0 bois       (501) staff       (20)      825 2020-09-02 09:33:58.000000 bebi103-0.1.9/doc/credits_and_citation.rst
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.881768 bebi103-0.1.9/doc/getting_started/
+-rw-r--r--   0 bois       (501) staff       (20)      989 2020-09-02 09:25:54.000000 bebi103-0.1.9/doc/getting_started/installation.rst
+-rw-r--r--   0 bois       (501) staff       (20)     1530 2021-03-01 09:25:19.000000 bebi103-0.1.9/doc/getting_started/purpose.rst
+-rw-r--r--   0 bois       (501) staff       (20)      692 2020-09-02 09:21:05.000000 bebi103-0.1.9/doc/index.rst
+-rw-r--r--   0 bois       (501) staff       (20)      795 2020-08-06 20:14:02.000000 bebi103-0.1.9/doc/make.bat
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.939833 bebi103-0.1.9/doc/user_guide/
+-rw-r--r--   0 bois       (501) staff       (20)       84 2020-08-27 06:17:35.000000 bebi103-0.1.9/doc/user_guide/.gitignore
+-rw-r--r--   0 bois       (501) staff       (20)     1972 2021-03-17 04:29:05.000000 bebi103-0.1.9/doc/user_guide/api.rst
+-rw-r--r--   0 bois       (501) staff       (20)   435859 2020-09-02 09:16:21.000000 bebi103-0.1.9/doc/user_guide/bootstrap.ipynb
+-rw-r--r--   0 bois       (501) staff       (20)  6018831 2020-09-02 07:40:50.000000 bebi103-0.1.9/doc/user_guide/hv.ipynb
+-rw-r--r--   0 bois       (501) staff       (20)      791 2020-09-02 09:20:36.000000 bebi103-0.1.9/doc/user_guide/image.ipynb
+-rw-r--r--   0 bois       (501) staff       (20)     2461 2020-09-01 16:37:34.000000 bebi103-0.1.9/doc/user_guide/sample_data.csv
+-rw-r--r--   0 bois       (501) staff       (20)     1006 2020-09-01 16:37:13.000000 bebi103-0.1.9/doc/user_guide/sample_data.py
+-rw-r--r--   0 bois       (501) staff       (20)     1570 2020-08-30 06:06:18.000000 bebi103-0.1.9/doc/user_guide/sample_model.stan
+-rw-r--r--   0 bois       (501) staff       (20)     1642 2020-09-01 17:18:07.000000 bebi103-0.1.9/doc/user_guide/sample_model_noncentered.stan
+-rw-r--r--   0 bois       (501) staff       (20)      914 2020-08-31 07:51:12.000000 bebi103-0.1.9/doc/user_guide/sample_model_prior_predictive.stan
+-rw-r--r--   0 bois       (501) staff       (20)  2710020 2021-01-03 04:04:37.000000 bebi103-0.1.9/doc/user_guide/sbc_results.csv
+-rw-r--r--   0 bois       (501) staff       (20) 13264972 2021-03-08 19:34:26.000000 bebi103-0.1.9/doc/user_guide/stan.ipynb
+-rw-r--r--   0 bois       (501) staff       (20)  3034584 2020-09-02 07:40:52.000000 bebi103-0.1.9/doc/user_guide/using_user_guide.ipynb
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.985106 bebi103-0.1.9/legacy/
+-rw-r--r--   0 bois       (501) staff       (20)    61231 2017-09-01 06:50:11.000000 bebi103-0.1.9/legacy/bebi103.py
+-rw-r--r--   0 bois       (501) staff       (20)    50639 2017-09-03 19:57:01.000000 bebi103-0.1.9/legacy/bebi103_original.py
+-rw-r--r--   0 bois       (501) staff       (20)      104 2021-03-01 09:27:29.000000 bebi103-0.1.9/requirements.txt
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.985907 bebi103-0.1.9/sandbox/
+-rw-r--r--   0 bois       (501) staff       (20)     2626 2017-09-01 06:53:20.000000 bebi103-0.1.9/sandbox/bokeh_mcmc.py
+-rw-r--r--   0 bois       (501) staff       (20)      108 2021-11-17 09:57:34.992271 bebi103-0.1.9/setup.cfg
+-rw-r--r--   0 bois       (501) staff       (20)     2192 2019-06-04 21:50:44.000000 bebi103-0.1.9/setup.py
+-rw-r--r--   0 bois       (501) staff       (20)     2644 2017-09-01 06:50:11.000000 bebi103-0.1.9/test_bebi103.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2021-11-17 09:57:34.988909 bebi103-0.1.9/tests/
+-rw-r--r--   0 bois       (501) staff       (20)        0 2017-09-01 06:50:32.000000 bebi103-0.1.9/tests/__init__.py
+-rw-r--r--   0 bois       (501) staff       (20)     6996 2018-10-09 17:03:13.000000 bebi103-0.1.9/tests/frog_tongue_adhesion.csv
+-rw-r--r--   0 bois       (501) staff       (20)     2644 2017-09-01 06:52:16.000000 bebi103-0.1.9/tests/test_bebi103.py
+-rw-r--r--   0 bois       (501) staff       (20)      102 2017-09-01 06:50:32.000000 bebi103-0.1.9/tests/test_sample.py
+-rw-r--r--   0 bois       (501) staff       (20)   257997 2018-10-11 16:55:30.000000 bebi103-0.1.9/tests/test_viz.ipynb
+-rw-r--r--   0 bois       (501) staff       (20)      449 2017-09-01 06:50:32.000000 bebi103-0.1.9/update_docs.sh
```

### Comparing `bebi103-0.1.8/LICENSE.md` & `bebi103-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/PKG-INFO` & `bebi103-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bebi103
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python utilities for the Caltech course BE/Bi 103: Data Analysis in the Biological Sciences.
 Home-page: https://github.com/justinbois/bebi103
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/bebi103/tarball/0.1.8
-Description: # bebi103
-        
-        [![DOI](https://data.caltech.edu/badge/44303442.svg)](https://data.caltech.edu/badge/latestdoi/44303442)
-        
-        Utilities Caltech BE/Bi 103 ab: Data Analysis in the Biological Sciences
-        
-        Please see [the documentation](http://bebi103.github.io/).
+Download-URL: https://github.com/justinbois/bebi103/tarball/0.1.9
 Keywords: GitHub,Python,Instruction,Biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.md
+
+# bebi103
+
+[![DOI](https://data.caltech.edu/badge/44303442.svg)](https://data.caltech.edu/badge/latestdoi/44303442)
+
+Utilities Caltech BE/Bi 103 ab: Data Analysis in the Biological Sciences
+
+Please see [the documentation](http://bebi103.github.io/).
+
```

### Comparing `bebi103-0.1.8/bebi103/__init__.py` & `bebi103-0.1.9/bebi103/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,8 +43,8 @@
         "Could not import `stan` submodule. Perhaps ArviZ or PyStan or CmdStanPy is/are"
         " not properly installed."
     )
 
 
 __author__ = """Justin Bois"""
 __email__ = "bois@caltech.edu"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `bebi103-0.1.8/bebi103/bootstrap.py` & `bebi103-0.1.9/bebi103/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/bootstrap_deprecated.py` & `bebi103-0.1.9/bebi103/deprecated/bootstrap_deprecated.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/emcee.py` & `bebi103-0.1.9/bebi103/deprecated/emcee.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/hotdists.py` & `bebi103-0.1.9/bebi103/deprecated/hotdists.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/make_hot.py` & `bebi103-0.1.9/bebi103/deprecated/make_hot.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/pm.py` & `bebi103-0.1.9/bebi103/deprecated/pm.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/stan_deprecated.py` & `bebi103-0.1.9/bebi103/deprecated/stan_deprecated.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/tools.py` & `bebi103-0.1.9/bebi103/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/deprecated/viz_deprecated.py` & `bebi103-0.1.9/bebi103/deprecated/viz_deprecated.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/gp.py` & `bebi103-0.1.9/bebi103/gp.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/hv.py` & `bebi103-0.1.9/bebi103/hv.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/image.py` & `bebi103-0.1.9/bebi103/image.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/stan.py` & `bebi103-0.1.9/bebi103/stan.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/bebi103/utils.py` & `bebi103-0.1.9/bebi103/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     Returns
     -------
     output : ndarray
         `data` as a one-dimensional NumPy array, dtype float.
     """
     # If it's scalar, convert to array
     if np.isscalar(data):
-        data = np.array([data], dtype=np.float)
+        data = np.array([data], dtype=float)
 
     # Convert data to NumPy array
-    data = np.array(data, dtype=np.float)
+    data = np.array(data, dtype=float)
 
     # Make sure it is 1D
     if len(data.shape) != 1:
         raise RuntimeError("Input must be a 1D array or Pandas series.")
 
     # Remove NaNs
     data = data[~np.isnan(data)]
```

### Comparing `bebi103-0.1.8/bebi103/viz.py` & `bebi103-0.1.9/bebi103/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -2018,22 +2018,31 @@
 
     if plot_ecdf:
         plots[0][0].yaxis.axis_label = "ECDF"
 
     # Take off tick labels
     for i in range(len(parameters) - 1):
         for j in range(i + 1):
-            plots[i][j].xaxis.major_label_text_font_size = "0pt"
+            plots[i][j].xaxis.visible = False
+
+            # To keep darkened part of axis visible, instead use:
+            # plots[i][j].xaxis.major_label_text_font_size = "0pt"
 
     if not plot_ecdf:
-        plots[0][0].yaxis.major_label_text_font_size = "0pt"
+        plots[0][0].yaxis.visible = False
+
+        # To keep darkened part of axis visible, instead use:
+        # plots[0][0].yaxis.major_label_text_font_size = "0pt"
 
     for i in range(1, len(parameters)):
         for j in range(1, i + 1):
-            plots[i][j].yaxis.major_label_text_font_size = "0pt"
+            plots[i][j].yaxis.visible = False
+
+            # To keep darkened part of axis visible, instead use:
+            # plots[i][j].yaxis.major_label_text_font_size = "0pt"
 
     grid = bokeh.layouts.gridplot(plots, toolbar_location="left")
 
     return grid
 
 
 def contour(
```

### Comparing `bebi103-0.1.8/bebi103.egg-info/PKG-INFO` & `bebi103-0.1.9/bebi103.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bebi103
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python utilities for the Caltech course BE/Bi 103: Data Analysis in the Biological Sciences.
 Home-page: https://github.com/justinbois/bebi103
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/bebi103/tarball/0.1.8
-Description: # bebi103
-        
-        [![DOI](https://data.caltech.edu/badge/44303442.svg)](https://data.caltech.edu/badge/latestdoi/44303442)
-        
-        Utilities Caltech BE/Bi 103 ab: Data Analysis in the Biological Sciences
-        
-        Please see [the documentation](http://bebi103.github.io/).
+Download-URL: https://github.com/justinbois/bebi103/tarball/0.1.9
 Keywords: GitHub,Python,Instruction,Biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE.md
+
+# bebi103
+
+[![DOI](https://data.caltech.edu/badge/44303442.svg)](https://data.caltech.edu/badge/latestdoi/44303442)
+
+Utilities Caltech BE/Bi 103 ab: Data Analysis in the Biological Sciences
+
+Please see [the documentation](http://bebi103.github.io/).
+
```

### Comparing `bebi103-0.1.8/bebi103.egg-info/SOURCES.txt` & `bebi103-0.1.9/bebi103.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/codemeta.json` & `bebi103-0.1.9/codemeta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -22,9 +22,9 @@
         "Instruction",
         "Biology"
     ],
     "license": "https://spdx.org/licenses/BSD-3-Clause",
     "maintainer": "https://orcid.org/0000-0001-7137-8746",
     "name": "bebi103",
     "programmingLanguage": "Python",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `bebi103-0.1.8/copyright.txt` & `bebi103-0.1.9/copyright.txt`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/Makefile` & `bebi103-0.1.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/_static/custom.css` & `bebi103-0.1.9/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/_static/logo.png` & `bebi103-0.1.9/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/conf.py` & `bebi103-0.1.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/credits_and_citation.rst` & `bebi103-0.1.9/doc/credits_and_citation.rst`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/getting_started/installation.rst` & `bebi103-0.1.9/doc/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/getting_started/purpose.rst` & `bebi103-0.1.9/doc/getting_started/purpose.rst`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/index.rst` & `bebi103-0.1.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/make.bat` & `bebi103-0.1.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/api.rst` & `bebi103-0.1.9/doc/user_guide/api.rst`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/bootstrap.ipynb` & `bebi103-0.1.9/doc/user_guide/bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/hv.ipynb` & `bebi103-0.1.9/doc/user_guide/hv.ipynb`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/image.ipynb` & `bebi103-0.1.9/doc/user_guide/image.ipynb`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sample_data.csv` & `bebi103-0.1.9/doc/user_guide/sample_data.csv`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sample_data.py` & `bebi103-0.1.9/doc/user_guide/sample_data.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sample_model.stan` & `bebi103-0.1.9/doc/user_guide/sample_model.stan`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sample_model_noncentered.stan` & `bebi103-0.1.9/doc/user_guide/sample_model_noncentered.stan`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sample_model_prior_predictive.stan` & `bebi103-0.1.9/doc/user_guide/sample_model_prior_predictive.stan`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/sbc_results.csv` & `bebi103-0.1.9/doc/user_guide/sbc_results.csv`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/stan.ipynb` & `bebi103-0.1.9/doc/user_guide/stan.ipynb`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/doc/user_guide/using_user_guide.ipynb` & `bebi103-0.1.9/doc/user_guide/using_user_guide.ipynb`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/legacy/bebi103.py` & `bebi103-0.1.9/legacy/bebi103.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/legacy/bebi103_original.py` & `bebi103-0.1.9/legacy/bebi103_original.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/sandbox/bokeh_mcmc.py` & `bebi103-0.1.9/sandbox/bokeh_mcmc.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/setup.py` & `bebi103-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/test_bebi103.py` & `bebi103-0.1.9/test_bebi103.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/tests/frog_tongue_adhesion.csv` & `bebi103-0.1.9/tests/frog_tongue_adhesion.csv`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/tests/test_bebi103.py` & `bebi103-0.1.9/tests/test_bebi103.py`

 * *Files identical despite different names*

### Comparing `bebi103-0.1.8/tests/test_viz.ipynb` & `bebi103-0.1.9/tests/test_viz.ipynb`

 * *Files identical despite different names*

