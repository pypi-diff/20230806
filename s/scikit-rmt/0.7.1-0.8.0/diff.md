# Comparing `tmp/scikit-rmt-0.7.1.tar.gz` & `tmp/scikit-rmt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.7.1.tar", last modified: Fri Jul 14 20:29:18 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.8.0.tar", last modified: Sat Aug  5 11:33:34 2023, max compression
```

## Comparing `scikit-rmt-0.7.1.tar` & `scikit-rmt-0.8.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.418631 scikit-rmt-0.7.1/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.7.1/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      278 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.7.1/CITATION.cff
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.7.1/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.7.1/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2023-07-08 22:52:37.000000 scikit-rmt-0.7.1/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-14 20:29:18.419343 scikit-rmt-0.7.1/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.7.1/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.246593 scikit-rmt-0.7.1/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.7.1/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.7.1/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.255340 scikit-rmt-0.7.1/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.7.1/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.7.1/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.7.1/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.7.1/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.7.1/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.7.1/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.7.1/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.7.1/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.7.1/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       65 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.274690 scikit-rmt-0.7.1/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       66 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-14 20:29:18.000000 scikit-rmt-0.7.1/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-14 20:29:18.420190 scikit-rmt-0.7.1/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.281512 scikit-rmt-0.7.1/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.7.1/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-14 20:17:58.000000 scikit-rmt-0.7.1/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.284218 scikit-rmt-0.7.1/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.7.1/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.7.1/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.7.1/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.287503 scikit-rmt-0.7.1/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.7.1/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.374422 scikit-rmt-0.7.1/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10728 2023-07-13 20:47:52.000000 scikit-rmt-0.7.1/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13872 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    15829 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    14125 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    56473 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/spectral_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.413581 scikit-rmt-0.7.1/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     1936 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_base_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    11990 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_spectral_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14730 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.7.1/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    17231 2023-07-14 20:16:53.000000 scikit-rmt-0.7.1/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-14 20:29:18.417897 scikit-rmt-0.7.1/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.7.1/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2689 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/tutorial/plot_0_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.7.1/tutorial/plot_1_spectral_laws.py
--rw-r--r--   0 santorum   (501) staff       (20)     9183 2023-07-13 18:06:51.000000 scikit-rmt-0.7.1/tutorial/plot_2_plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.222445 scikit-rmt-0.8.0/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.8.0/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-07-13 18:06:51.000000 scikit-rmt-0.8.0/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.8.0/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.8.0/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.8.0/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2023-07-08 22:52:37.000000 scikit-rmt-0.8.0/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    24322 2023-08-05 11:33:34.222780 scikit-rmt-0.8.0/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    19766 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.8.0/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.165810 scikit-rmt-0.8.0/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.8.0/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.8.0/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.8.0/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1276 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.8.0/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.174852 scikit-rmt-0.8.0/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.8.0/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2279 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.8.0/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1343 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.8.0/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.8.0/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.8.0/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.8.0/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.8.0/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       65 2023-07-13 18:06:51.000000 scikit-rmt-0.8.0/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.177840 scikit-rmt-0.8.0/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    24322 2023-08-05 11:33:34.000000 scikit-rmt-0.8.0/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1799 2023-08-05 11:33:34.000000 scikit-rmt-0.8.0/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-08-05 11:33:34.000000 scikit-rmt-0.8.0/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       66 2023-08-05 11:33:34.000000 scikit-rmt-0.8.0/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-08-05 11:33:34.000000 scikit-rmt-0.8.0/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-08-05 11:33:34.223255 scikit-rmt-0.8.0/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.8.0/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.179386 scikit-rmt-0.8.0/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.8.0/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.181963 scikit-rmt-0.8.0/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.8.0/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.8.0/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.8.0/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.184639 scikit-rmt-0.8.0/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.8.0/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.8.0/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.8.0/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.196427 scikit-rmt-0.8.0/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.8.0/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    11143 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    15098 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    16988 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    15256 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     4740 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/misc.py
+-rw-r--r--   0 santorum   (501) staff       (20)    53688 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/spectral_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.205818 scikit-rmt-0.8.0/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1894 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_base_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5762 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    12038 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5106 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    43414 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_spectral_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2235 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14778 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.8.0/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6038 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5136 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    18391 2023-08-05 11:22:48.000000 scikit-rmt-0.8.0/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-08-05 11:33:34.219755 scikit-rmt-0.8.0/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.8.0/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2689 2023-07-13 18:06:51.000000 scikit-rmt-0.8.0/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10284 2023-08-05 11:24:24.000000 scikit-rmt-0.8.0/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9299 2023-08-05 11:24:46.000000 scikit-rmt-0.8.0/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.7.1/LICENSE` & `scikit-rmt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/Makefile` & `scikit-rmt-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/PKG-INFO` & `scikit-rmt-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.7.1
+Version: 0.8.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.1.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.8.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
@@ -112,15 +112,15 @@
         ## A brief tutorial
         
         First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
         **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
         a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
         
         ```python
-        from skrmt.ensemble import GaussianEnsemble
+        from skrmt.ensemble.gaussian_ensemble import GaussianEnsemble
         # sampling a GOE (beta=1) matrix of size 3x3
         goe = GaussianEnsemble(beta=1, n=3)
         print(goe.matrix)
         ```
         ```bash
         [[ 0.34574696 -0.10802385  0.38245343]
          [-0.10802385 -0.60113963  0.28624612]
@@ -139,17 +139,19 @@
         -->
         
         If we sample a **non-symmetric/non-hermitian** random matrix, its eigenvalues do not need to be real,
         so a **2D complex histogram** has been implemented in order to study spectral density of these type
         of random matrices. It would be the case, for example, of **Circular Symplectic Ensemble (CSE)**.
         
         ```python
+        from skrmt.ensemble.circular_ensemble import CircularEnsemble
+        
         # sampling a CSE (beta=4) matrix of size 2000x2000
         cse = CircularEnsemble(beta=4, n=1000)
-        cse.plot_eigval_hist(bins=80, interval=(-2.2,2.2))
+        cse.plot_eigval_hist(bins=80)
         ```
         ![CSE density plot](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/hist_cse_smooth.png)
         <!---
         <img src="imgs/hist_cse_smooth.png" width=650 height=320 alt="CSE density plot">
         -->
         
         We can **boost histogram representation** using the results described by A. Edelman and I. Dumitriu
@@ -167,90 +169,96 @@
         ![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
         <!---
         <img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
         -->
         
         In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
         Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
-        by using the `limit_pdf` argument.
+        by using the `plot_law_pdf=True` argument.
         
-        Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
+        Plot of **Wigner's Semicircle Law**, sampling 100000 *independent* eigenvalues of a GOE matrix:
         ```python
-        from skrmt.ensemble import wigner_semicircular_law
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
-        wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True)
+        wsd = WignerSemicircleDistribution(beta=1)
+        wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
         ```
         ![Wigner Semicircle Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe.png)
         <!---
         <img src="imgs/scl_goe.png" width=450 height=320 alt="Wigner Semicircle Law">
         -->
         
         ```python
-        from skrmt.ensemble import wigner_semicircular_law
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
-        wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True, limit_pdf=True)
+        wsd = WignerSemicircleDistribution(beta=1)
+        wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Wigner Semicircle Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe_pdf.png)
         <!---
         <img src="imgs/scl_goe_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF">
         -->
         
-        Plot of **Marchenko-Pastur Law**, sampling a WRE matrix 5000x5000:
+        Plot of **Marchenko-Pastur Law**, sampling 100000 *independent* eigenvalues of a WRE matrix:
         ```python
-        from skrmt.ensemble import marchenko_pastur_law
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
-        marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True)
+        mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+        mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
         ```
         ![Marchenko-Pastur Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre.png)
         <!---
         <img src="imgs/mpl_wre.png" width=450 height=320 alt="Marchenko-Pastur Law">
         -->
         
         ```python
-        from skrmt.ensemble import marchenko_pastur_law
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
-        marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True, limit_pdf=True)
+        mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+        mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Marchenko-Pastur Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre_pdf.png)
         <!---
         <img src="imgs/mpl_wre_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF">
         -->
         
-        Plot of **Tracy-Widom Law**, sampling 20000 GOE matrices of size 100x100:
+        Plot of **Tracy-Widom Law**, sampling 30000 maximum eigenvalues of GOE matrices:
         ```python
-        from skrmt.ensemble import tracy_widom_law
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
-        tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True)
+        twd = TracyWidomDistribution(beta=1)
+        twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True)
         ```
         ![Tracy-Widom Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe.png)
         <!---
         <img src="imgs/twl_goe.png" width=450 height=320 alt="Tracy-Widom Law">
         -->
         
         ```python
-        from skrmt.ensemble import tracy_widom_law
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
-        tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
+        twd = TracyWidomDistribution(beta=1)
+        twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
         <!---
         <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
         -->
         
-        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
-        - `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
-        - `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
-        - `TracyWidomDistribution` in `skrmt.ensemble.law`.
-        - `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.spectral_law` module:
+        - `WignerSemicircleDistribution` in `skrmt.ensemble.spectral_law`.
+        - `MarchenkoPasturDistribution` in `skrmt.ensemble.spectral_law`.
+        - `TracyWidomDistribution` in `skrmt.ensemble.spectral_law`.
+        - `ManovaSpectrumDistribution` in `skrmt.ensemble.spectral_law`.
         
         For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import WignerSemicircleDistribution
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
         x1 = np.linspace(-5, 5, num=1000)
         x2 = np.linspace(-10, 10, num=2000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for sigma in [0.5, 1.0, 2.0, 4.0]:
@@ -280,15 +288,15 @@
         <img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
         -->
         
         Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import MarchenkoPasturDistribution
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
         x1 = np.linspace(0, 4, num=1000)
         x2 = np.linspace(0, 5, num=2000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
@@ -319,15 +327,15 @@
         <img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
         -->
         
         In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import TracyWidomDistribution
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
         x = np.linspace(-5, 2, num=1000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for beta in [1,2,4]:
             twd = TracyWidomDistribution(beta=beta)
```

### Comparing `scikit-rmt-0.7.1/README.md` & `scikit-rmt-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 ## A brief tutorial
 
 First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
 **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
 a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
 
 ```python
-from skrmt.ensemble import GaussianEnsemble
+from skrmt.ensemble.gaussian_ensemble import GaussianEnsemble
 # sampling a GOE (beta=1) matrix of size 3x3
 goe = GaussianEnsemble(beta=1, n=3)
 print(goe.matrix)
 ```
 ```bash
 [[ 0.34574696 -0.10802385  0.38245343]
  [-0.10802385 -0.60113963  0.28624612]
@@ -130,17 +130,19 @@
 -->
 
 If we sample a **non-symmetric/non-hermitian** random matrix, its eigenvalues do not need to be real,
 so a **2D complex histogram** has been implemented in order to study spectral density of these type
 of random matrices. It would be the case, for example, of **Circular Symplectic Ensemble (CSE)**.
 
 ```python
+from skrmt.ensemble.circular_ensemble import CircularEnsemble
+
 # sampling a CSE (beta=4) matrix of size 2000x2000
 cse = CircularEnsemble(beta=4, n=1000)
-cse.plot_eigval_hist(bins=80, interval=(-2.2,2.2))
+cse.plot_eigval_hist(bins=80)
 ```
 ![CSE density plot](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/hist_cse_smooth.png)
 <!---
 <img src="imgs/hist_cse_smooth.png" width=650 height=320 alt="CSE density plot">
 -->
 
 We can **boost histogram representation** using the results described by A. Edelman and I. Dumitriu
@@ -158,90 +160,96 @@
 ![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
 <!---
 <img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
 -->
 
 In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
 Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
-by using the `limit_pdf` argument.
+by using the `plot_law_pdf=True` argument.
 
-Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
+Plot of **Wigner's Semicircle Law**, sampling 100000 *independent* eigenvalues of a GOE matrix:
 ```python
-from skrmt.ensemble import wigner_semicircular_law
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
-wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True)
+wsd = WignerSemicircleDistribution(beta=1)
+wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
 ```
 ![Wigner Semicircle Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe.png)
 <!---
 <img src="imgs/scl_goe.png" width=450 height=320 alt="Wigner Semicircle Law">
 -->
 
 ```python
-from skrmt.ensemble import wigner_semicircular_law
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
-wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True, limit_pdf=True)
+wsd = WignerSemicircleDistribution(beta=1)
+wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
 ```
 ![Wigner Semicircle Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe_pdf.png)
 <!---
 <img src="imgs/scl_goe_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF">
 -->
 
-Plot of **Marchenko-Pastur Law**, sampling a WRE matrix 5000x5000:
+Plot of **Marchenko-Pastur Law**, sampling 100000 *independent* eigenvalues of a WRE matrix:
 ```python
-from skrmt.ensemble import marchenko_pastur_law
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True)
+mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
 ```
 ![Marchenko-Pastur Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre.png)
 <!---
 <img src="imgs/mpl_wre.png" width=450 height=320 alt="Marchenko-Pastur Law">
 -->
 
 ```python
-from skrmt.ensemble import marchenko_pastur_law
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True, limit_pdf=True)
+mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
 ```
 ![Marchenko-Pastur Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre_pdf.png)
 <!---
 <img src="imgs/mpl_wre_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF">
 -->
 
-Plot of **Tracy-Widom Law**, sampling 20000 GOE matrices of size 100x100:
+Plot of **Tracy-Widom Law**, sampling 30000 maximum eigenvalues of GOE matrices:
 ```python
-from skrmt.ensemble import tracy_widom_law
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
-tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True)
+twd = TracyWidomDistribution(beta=1)
+twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True)
 ```
 ![Tracy-Widom Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe.png)
 <!---
 <img src="imgs/twl_goe.png" width=450 height=320 alt="Tracy-Widom Law">
 -->
 
 ```python
-from skrmt.ensemble import tracy_widom_law
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
-tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
+twd = TracyWidomDistribution(beta=1)
+twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True, plot_law_pdf=True)
 ```
 ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
 <!---
 <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
 -->
 
-The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
-- `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
-- `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
-- `TracyWidomDistribution` in `skrmt.ensemble.law`.
-- `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.spectral_law` module:
+- `WignerSemicircleDistribution` in `skrmt.ensemble.spectral_law`.
+- `MarchenkoPasturDistribution` in `skrmt.ensemble.spectral_law`.
+- `TracyWidomDistribution` in `skrmt.ensemble.spectral_law`.
+- `ManovaSpectrumDistribution` in `skrmt.ensemble.spectral_law`.
 
 For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import WignerSemicircleDistribution
+from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
 x1 = np.linspace(-5, 5, num=1000)
 x2 = np.linspace(-10, 10, num=2000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
 for sigma in [0.5, 1.0, 2.0, 4.0]:
@@ -271,15 +279,15 @@
 <img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
 -->
 
 Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import MarchenkoPasturDistribution
+from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
 x1 = np.linspace(0, 4, num=1000)
 x2 = np.linspace(0, 5, num=2000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
 for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
@@ -310,15 +318,15 @@
 <img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
 -->
 
 In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
-from skrmt.ensemble.law import TracyWidomDistribution
+from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
 x = np.linspace(-5, 2, num=1000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
 for beta in [1,2,4]:
     twd = TracyWidomDistribution(beta=beta)
```

### Comparing `scikit-rmt-0.7.1/conf.py` & `scikit-rmt-0.8.0/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/docs/skrmt.covariance.rst` & `scikit-rmt-0.8.0/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/docs/skrmt.ensemble.rst` & `scikit-rmt-0.8.0/docs/skrmt.ensemble.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 ----------------------------------------
 
 .. automodule:: skrmt.ensemble.circular_ensemble
    :members:
    :undoc-members:
    :show-inheritance:
 
+skrmt.ensemble.utils module
+----------------------------------------
+
+.. automodule:: skrmt.ensemble.utils
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 skrmt.ensemble.tridiagonal\_utils module
 ----------------------------------------
 
 .. automodule:: skrmt.ensemble.tridiagonal_utils
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit-rmt-0.7.1/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.8.0/examples/plot_boosting_density_representation.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,54 +15,54 @@
 ##############################################################################
 # We can sample a random matrix of the Gaussian Ensemble with a relatively
 # large size and plot its spectral density.
 
 goe = GaussianEnsemble(beta=1, n=5000)
 
 t1 = time.time()
-goe.plot_eigval_hist(bins=60, interval=(-2,2))
+goe.plot_eigval_hist(bins=60, density=False, normalize=False)
 t2 = time.time()
 
 ##############################################################################
 # The time needed to compute the previous histogram is:
 print(t2-t1, 'seconds')
 
 ##############################################################################
 # We can speed up this procedure using the tridiagonal form of Gaussian
-# Ensemble random matrices.
+# Ensemble random matrices: ``use_tridiagonal=True``.
 
 goe_tridiag = GaussianEnsemble(beta=1, n=5000, use_tridiagonal=True)
 
 t1 = time.time()
-goe_tridiag.plot_eigval_hist(bins=60, interval=(-2,2))
+goe_tridiag.plot_eigval_hist(bins=60, density=False, normalize=False)
 t2 = time.time()
 
 ##############################################################################
 # The time needed to compute the previous histogram is:
 print(t2-t1, 'seconds')
 
 ##############################################################################
 # This boosting trick can be used with Wishart Ensemble too
 
 wre = WishartEnsemble(beta=1, p=5000, n=10000)
 
 t1 = time.time()
-wre.plot_eigval_hist(bins=60, interval=(0,3))
+wre.plot_eigval_hist(bins=60, density=False, normalize=False)
 t2 = time.time()
 
 ##############################################################################
 # The time needed to compute the previous histogram is:
 print(t2-t1, 'seconds')
 
 ##############################################################################
-# Using tridiagonal form of the Wishart Ensemble:
+# Using tridiagonal form of the Wishart Ensemble by setting ``use_tridiagonal=True``.
 
 wre_tridiag = WishartEnsemble(beta=1, p=5000, n=10000, use_tridiagonal=True)
 
 t1 = time.time()
-wre_tridiag.plot_eigval_hist(bins=60, interval=(0,3))
+wre_tridiag.plot_eigval_hist(bins=60, density=False, normalize=False)
 t2 = time.time()
 
 ##############################################################################
 # The time needed to compute the previous histogram is:
 print(t2-t1, 'seconds')
```

### Comparing `scikit-rmt-0.7.1/examples/plot_circular_ensemble.py` & `scikit-rmt-0.8.0/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/examples/plot_complex_histograms.py` & `scikit-rmt-0.8.0/examples/plot_complex_histograms.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 # scikit-rmt takes into account this possibility and uses histograms in 2D in
 # order to represent spectrum distribution of given ensembles.
 
 ##############################################################################
 # In this example, eigenvalue spectrum of CUE random matrix is shown.
 
 cue = CircularEnsemble(beta=2, n=1000)
-cue.plot_eigval_hist(bins=80, interval=(-2.2,2.2))
+cue.plot_eigval_hist(bins=80)
 
 ##############################################################################
 # And the eigenvalue spectrum of CSE.
 
 cse = CircularEnsemble(beta=4, n=1000)
-cse.plot_eigval_hist(bins=80, interval=(-2.2,2.2))
+cse.plot_eigval_hist(bins=80)
 
 ##############################################################################
 # The provided heatmap gives an illustration of the eigenvalue accumulation.
```

### Comparing `scikit-rmt-0.7.1/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.8.0/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/examples/plot_manova_ensemble.py` & `scikit-rmt-0.8.0/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.8.0/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/index.rst` & `scikit-rmt-0.8.0/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.8.0/scikit_rmt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.7.1
+Version: 0.8.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.1.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.8.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
@@ -112,15 +112,15 @@
         ## A brief tutorial
         
         First of all, several random matrix ensembles can be sampled: **Gaussian Ensembles**, **Wishart Ensembles**,
         **Manova Ensembles** and **Circular Ensembles**. As an example, the following code shows how to sample
         a **Gaussian Orthogonal Ensemble (GOE)** random matrix.
         
         ```python
-        from skrmt.ensemble import GaussianEnsemble
+        from skrmt.ensemble.gaussian_ensemble import GaussianEnsemble
         # sampling a GOE (beta=1) matrix of size 3x3
         goe = GaussianEnsemble(beta=1, n=3)
         print(goe.matrix)
         ```
         ```bash
         [[ 0.34574696 -0.10802385  0.38245343]
          [-0.10802385 -0.60113963  0.28624612]
@@ -139,17 +139,19 @@
         -->
         
         If we sample a **non-symmetric/non-hermitian** random matrix, its eigenvalues do not need to be real,
         so a **2D complex histogram** has been implemented in order to study spectral density of these type
         of random matrices. It would be the case, for example, of **Circular Symplectic Ensemble (CSE)**.
         
         ```python
+        from skrmt.ensemble.circular_ensemble import CircularEnsemble
+        
         # sampling a CSE (beta=4) matrix of size 2000x2000
         cse = CircularEnsemble(beta=4, n=1000)
-        cse.plot_eigval_hist(bins=80, interval=(-2.2,2.2))
+        cse.plot_eigval_hist(bins=80)
         ```
         ![CSE density plot](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/hist_cse_smooth.png)
         <!---
         <img src="imgs/hist_cse_smooth.png" width=650 height=320 alt="CSE density plot">
         -->
         
         We can **boost histogram representation** using the results described by A. Edelman and I. Dumitriu
@@ -167,90 +169,96 @@
         ![Joint Eigenvalue PDF for GOE](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/goe_joint_eigval_pdf.png)
         <!---
         <img src="imgs/goe_joint_eigval_pdf.png" width=820 height=370 alt="Joint Eigenvalue PDF for GOE">
         -->
         
         In addition, several spectral laws can be analyzed using this library, such as Wigner's Semicircle Law,
         Marchenko-Pastur Law and Tracy-Widom Law. The analytical probability density function can also be plotted
-        by using the `limit_pdf` argument.
+        by using the `plot_law_pdf=True` argument.
         
-        Plot of **Wigner's Semicircle Law**, sampling a GOE matrix 5000x5000:
+        Plot of **Wigner's Semicircle Law**, sampling 100000 *independent* eigenvalues of a GOE matrix:
         ```python
-        from skrmt.ensemble import wigner_semicircular_law
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
-        wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True)
+        wsd = WignerSemicircleDistribution(beta=1)
+        wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
         ```
         ![Wigner Semicircle Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe.png)
         <!---
         <img src="imgs/scl_goe.png" width=450 height=320 alt="Wigner Semicircle Law">
         -->
         
         ```python
-        from skrmt.ensemble import wigner_semicircular_law
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
-        wigner_semicircular_law(ensemble='goe', n_size=5000, bins=80, density=True, limit_pdf=True)
+        wsd = WignerSemicircleDistribution(beta=1)
+        wsd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Wigner Semicircle Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scl_goe_pdf.png)
         <!---
         <img src="imgs/scl_goe_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF">
         -->
         
-        Plot of **Marchenko-Pastur Law**, sampling a WRE matrix 5000x5000:
+        Plot of **Marchenko-Pastur Law**, sampling 100000 *independent* eigenvalues of a WRE matrix:
         ```python
-        from skrmt.ensemble import marchenko_pastur_law
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
-        marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True)
+        mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+        mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True)
         ```
         ![Marchenko-Pastur Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre.png)
         <!---
         <img src="imgs/mpl_wre.png" width=450 height=320 alt="Marchenko-Pastur Law">
         -->
         
         ```python
-        from skrmt.ensemble import marchenko_pastur_law
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
-        marchenko_pastur_law(ensemble='wre', p_size=5000, n_size=15000, bins=80, density=True, limit_pdf=True)
+        mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+        mpd.plot_empirical_pdf(sample_size=100000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Marchenko-Pastur Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/mpl_wre_pdf.png)
         <!---
         <img src="imgs/mpl_wre_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF">
         -->
         
-        Plot of **Tracy-Widom Law**, sampling 20000 GOE matrices of size 100x100:
+        Plot of **Tracy-Widom Law**, sampling 30000 maximum eigenvalues of GOE matrices:
         ```python
-        from skrmt.ensemble import tracy_widom_law
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
-        tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True)
+        twd = TracyWidomDistribution(beta=1)
+        twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True)
         ```
         ![Tracy-Widom Law](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe.png)
         <!---
         <img src="imgs/twl_goe.png" width=450 height=320 alt="Tracy-Widom Law">
         -->
         
         ```python
-        from skrmt.ensemble import tracy_widom_law
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
-        tracy_widom_law(ensemble='goe', n_size=500, times=20000, bins=80, density=True, limit_pdf=True)
+        twd = TracyWidomDistribution(beta=1)
+        twd.plot_empirical_pdf(sample_size=30000, bins=80, density=True, plot_law_pdf=True)
         ```
         ![Tracy-Widom Law PDF](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/twl_goe_pdf.png)
         <!---
         <img src="imgs/twl_goe_pdf.png" width=450 height=320 alt="Tracy-Widom Law PDF">
         -->
         
-        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.law` module:
-        - `WignerSemicircleDistribution` in `skrmt.ensemble.law`.
-        - `MarchenkoPasturDistribution` in `skrmt.ensemble.law`.
-        - `TracyWidomDistribution` in `skrmt.ensemble.law`.
-        - `ManovaSpectrumDistribution` in `skrmt.ensemble.law`.
+        The proposed package **scikit-rmt** also provides support for **computing and analyzing** the **probability density function (PDF)** and **cumulative distribution function (CDF)** of the main random matrix ensembles. In particular, the following classes are implemented in the `ensemble.spectral_law` module:
+        - `WignerSemicircleDistribution` in `skrmt.ensemble.spectral_law`.
+        - `MarchenkoPasturDistribution` in `skrmt.ensemble.spectral_law`.
+        - `TracyWidomDistribution` in `skrmt.ensemble.spectral_law`.
+        - `ManovaSpectrumDistribution` in `skrmt.ensemble.spectral_law`.
         
         For example, `WignerSemicircleDistribution` can be used to plot the **Wigner's Semicircle Law PDF**:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import WignerSemicircleDistribution
+        from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
         
         x1 = np.linspace(-5, 5, num=1000)
         x2 = np.linspace(-10, 10, num=2000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for sigma in [0.5, 1.0, 2.0, 4.0]:
@@ -280,15 +288,15 @@
         <img src="imgs/wigner_scl_pdf.png" width=450 height=320 alt="Wigner Semicircle Law PDF (Analytical)">
         -->
         
         Similarly, `MarchenkoPasturDistribution` can be used to plot the **Marchenko-Pastur Law PDF**:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import MarchenkoPasturDistribution
+        from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
         
         x1 = np.linspace(0, 4, num=1000)
         x2 = np.linspace(0, 5, num=2000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for ratio in [0.2, 0.4, 0.6, 1.0, 1.4]:
@@ -319,15 +327,15 @@
         <img src="imgs/mpl_pdf.png" width=450 height=320 alt="Marchenko-Pastur Law PDF (Analytical)">
         -->
         
         In the following example, we show how we can plot the **PDF and CDF of the Tracy-Widom distribution** using the class `TracyWidomDistribution`:
         ```python
         import numpy as np
         import matplotlib.pyplot as plt
-        from skrmt.ensemble.law import TracyWidomDistribution
+        from skrmt.ensemble.spectral_law import TracyWidomDistribution
         
         x = np.linspace(-5, 2, num=1000)
         
         fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
         
         for beta in [1,2,4]:
             twd = TracyWidomDistribution(beta=beta)
```

### Comparing `scikit-rmt-0.7.1/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.8.0/scikit_rmt.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -33,28 +33,31 @@
 skrmt/covariance/__init__.py
 skrmt/covariance/estimator.py
 skrmt/covariance/metrics.py
 skrmt/covariance/tests/__init__.py
 skrmt/covariance/tests/test_estimator.py
 skrmt/covariance/tests/test_metrics.py
 skrmt/ensemble/__init__.py
-skrmt/ensemble/_base_ensemble.py
+skrmt/ensemble/base_ensemble.py
 skrmt/ensemble/circular_ensemble.py
 skrmt/ensemble/gaussian_ensemble.py
 skrmt/ensemble/manova_ensemble.py
+skrmt/ensemble/misc.py
 skrmt/ensemble/spectral_law.py
 skrmt/ensemble/tracy_widom_approximator.py
 skrmt/ensemble/tridiagonal_utils.py
+skrmt/ensemble/utils.py
 skrmt/ensemble/wishart_ensemble.py
 skrmt/ensemble/tests/__init__.py
 skrmt/ensemble/tests/test_base_ens.py
 skrmt/ensemble/tests/test_circular_ens.py
 skrmt/ensemble/tests/test_gaussian_ens.py
 skrmt/ensemble/tests/test_manova_ens.py
 skrmt/ensemble/tests/test_spectral_law.py
 skrmt/ensemble/tests/test_tracy_widom_approx.py
 skrmt/ensemble/tests/test_tridiagonalization.py
+skrmt/ensemble/tests/test_utils.py
 skrmt/ensemble/tests/test_wishart_ens.py
 tutorial/README.txt
 tutorial/plot_0_introduction.py
 tutorial/plot_1_spectral_laws.py
 tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.7.1/setup.py` & `scikit-rmt-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/covariance/__init__.py` & `scikit-rmt-0.8.0/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/covariance/estimator.py` & `scikit-rmt-0.8.0/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/covariance/metrics.py` & `scikit-rmt-0.8.0/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.8.0/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.8.0/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/__init__.py` & `scikit-rmt-0.8.0/skrmt/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.8.0/skrmt/ensemble/base_ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,25 @@
     def __init__(self):
         self.matrix = None
         self._eigvals = None
         # default eigenvalue normalization constant
         self.eigval_norm_const = 1.0
 
     @abstractmethod
-    def sample(self):
+    def sample(self, random_state: int = None):
         """Samples new random matrix.
 
         The sampling algorithm depends on the inherited classes, so it should be
         specified by them.
 
+        Args:
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
+
         Returns:
             numpy array containing new matrix sampled.
         """
         # pylint: disable=unnecessary-pass
         pass
 
     @abstractmethod
@@ -93,15 +98,15 @@
         pass
 
     def eigval_hist(
         self,
         bins,
         interval=None,
         density=False,
-        normalize=True,
+        normalize=False,
         avoid_img=False
     ):
         """Calculates the histogram of the matrix eigenvalues.
 
         Calculates the histogram of the current sampled matrix eigenvalues. Some ensembles
         like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble might have
         improved routines to avoid calculating the eigenvalues, so instead the histogram
@@ -117,31 +122,31 @@
             interval (tuple): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False,
+                i.e., the eigenvalues are normalized. Normalization makes the eigenvalues
+                to be in the same support independently of the sample size.
             avoid_img (bool, default=False): If True, eigenvalue imaginary part is ignored.
                 This should be used when the eigenvalue compatation is expected to generate
                 complex eigenvalues with really small imaginary part because of computing
                 rounding errors. E.g.: MANOVA Ensemble eigenvalues.
 
         Returns:
             (tuple) tuple containing:
                 observed (array): List of eigenvalues frequencies per bin. If density is
                 True these values are the relative frequencies in order to get an area under
                 the histogram equal to 1. Otherwise, this list contains the absolute
                 frequencies of the eigenvalues.
-                bins (array): The edges of the bins. Length nbins + 1 (nbins left edges and
-                right edge of last bin)
+                bin_edges (array): The edges of the bins. Length nbins + 1 (nbins left edges
+                and right edge of last bin)
 
         Raises:
             ValueError if interval is not a tuple.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
@@ -157,26 +162,26 @@
 
         # calculating eigenvalues using standard algorithm
         eigvals = self.eigvals(normalize=normalize)
         # ignoring imaginary part because of computing rounding errors
         if avoid_img:
             eigvals = eigvals.real
 
-        # using numpy to obtain histogram in the given interval and no. of bins
-        observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
-        return observed, bins
+        # using numpy to obtain histogram in the given interval and bins
+        observed, bin_edges = np.histogram(eigvals, bins=bins, range=interval, density=density)
+        return observed, bin_edges
 
 
     def plot_eigval_hist(
         self,
         bins,
         interval=None,
         density=False,
-        normalize=True,
-        fig_path=None,
+        normalize=False,
+        savefig_path=None,
         avoid_img=False
     ):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Some ensembles like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble
         have improved routines to avoid calculating the eigenvalues, so the histogram
@@ -193,45 +198,46 @@
             interval (tuple): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False,
+                i.e., the eigenvalues are normalized. Normalization makes the eigenvalues
+                to be in the same support independently of the sample size.
             avoid_img (bool, default=False): If True, eigenvalue imaginary part is ignored.
                 This should be used when the eigenvalue compatation is expected to generate
                 complex eigenvalues with really small imaginary part because of computing
                 rounding errors. E.g.: MANOVA Ensemble eigenvalues.
-            fig_path (string, default=None): path to save the created figure. If it is not
+            savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
-        if not isinstance(interval, tuple):
-            raise ValueError("interval argument must be a tuple")
+        if interval is not None:
+            if not isinstance(interval, tuple):
+                raise ValueError("interval argument must be a tuple")
 
-        observed, bins = self.eigval_hist(bins=bins, interval=interval, density=density,
-                                          normalize=normalize, avoid_img=avoid_img)
-        width = bins[1]-bins[0]
-        plt.bar(bins[:-1], observed, width=width, align='edge')
+        observed, bin_edges = self.eigval_hist(bins=bins, interval=interval, density=density,
+                                               normalize=normalize, avoid_img=avoid_img)
+        width = bin_edges[1]-bin_edges[0]
+        plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
         plt.title("Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("density")
 
         # Saving plot or showing it
-        if fig_path:
-            plt.savefig(fig_path, dpi=1200)
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=1200)
         else:
             plt.show()
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.8.0/skrmt/ensemble/circular_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy import special
 
-from ._base_ensemble import _Ensemble
+from .base_ensemble import _Ensemble
 
 
 
 def _sample_haar_mtx(size):
     """Samples Haar-distributed matrices.
 
     Samples Haar-distributed matrices that are useful to generate
@@ -71,71 +71,86 @@
             Classical Ensembles of Random Unitary Matrices.
             Communications in Mathematical Physics. 349 (2017): 991-1027.
         - "Circular ensemble". Wikipedia.
             en.wikipedia.org/wiki/Circular_ensemble
 
     """
 
-    def __init__(self, beta, n):
+    def __init__(self, beta, n, random_state=None):
         """Constructor for CircularEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int): descriptive integer of the Circular ensemble type.
                 For COE beta=1, for CUE beta=2, for CSE beta=4.
             n (int): random matrix size. Circular ensemble matrices are
                 squared matrices. COE and CUE are of size n times n,
                 and CSE are of size 2n times 2n.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy before sampling the random matrix instance. This 
+                has to be any integer between 0 and 2**32 - 1 (inclusive), or None (default).
+                If None, the seed is obtained from the clock.
 
         """
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
         self._eigvals = None
-        self.matrix = self.sample()
+        self.matrix = self.sample(random_state=random_state)
 
-    def set_size(self, n, resample_mtx=False):
+    def set_size(self, n, resample_mtx=False, random_state: int = None):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             n (int): random matrix size. Circular ensemble matrices are
                 squared matrices. COE and CUE are of size n times n,
                 and CSE are of size 2n times 2n.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         """
         self.n = n
         if resample_mtx:
-            self.matrix = self.sample()
+            self.matrix = self.sample(random_state=random_state)
 
     # pylint: disable=inconsistent-return-statements
-    def sample(self):
+    def sample(self, random_state: int = None):
         """Samples new Circular Ensemble random matrix.
 
         The sampling algorithm depends on the specification of
         beta parameter. If beta=1, COE matrix is sampled; if
         beta=2 CUE matrix is sampled and if beta=4
         CSE matrix is sampled.
 
+        Args:
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
+
         Returns:
             numpy array containing new matrix sampled.
 
         References:
             - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
             - "Circular ensemble". Wikipedia.
                 en.wikipedia.org/wiki/Circular_ensemble
 
         """
+        if random_state is not None:
+            np.random.seed(random_state)
+
         if self.beta == 1:
             return self._sample_coe()
         if self.beta == 2:
             return self._sample_cue()
         if self.beta == 4:
             return self._sample_cse()
 
@@ -219,15 +234,15 @@
             self._eigvals = np.linalg.eigvalsh(self.matrix)
         else:
             # using eigvals since some eigenvalues could be imaginary
             self._eigvals = np.linalg.eigvals(self.matrix)
 
         return norm_const * self._eigvals
 
-    def plot_eigval_hist(self, bins, interval=None, density=False, normalize=True, fig_path=None):
+    def plot_eigval_hist(self, bins, interval=None, density=False, normalize=False, savefig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         It is important to underline that this function works with real and complex
         eigenvalues: if the matrix eigenvalues are complex, they are plotted in the
         complex plane next to a heap map to study eigenvalue density.
 
@@ -239,58 +254,60 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
-            fig_path (string, default=None): path to save the created figure. If it is not
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False,
+                i.e., the eigenvalues are normalized. Normalization makes the eigenvalues
+                to be in the same support independently of the sample size.
+            savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
 
         """
         # pylint: disable=too-many-arguments
         # pylint: disable=too-many-locals
         if self.beta == 1:
             return super().plot_eigval_hist(
-                bins=bins, interval=interval, density=density, normalize=normalize, fig_path=fig_path
+                bins=bins, interval=interval, density=density, normalize=normalize, savefig_path=savefig_path
             )
 
         if (interval is not None) and not isinstance(interval, tuple):
             raise ValueError("interval argument must be a tuple (or None)")
 
         eigvals = self.eigvals()
         xvals = eigvals.real
         yvals = eigvals.imag
 
         if interval is None:
             rang_val = self.beta/2
+            rang_val += 0.1*rang_val
             rang = ((-rang_val, rang_val), (-rang_val, rang_val))
             extent = [-rang_val, rang_val, -rang_val, rang_val]
         else:
             rang = (interval, interval)
             extent = [interval[0], interval[1], interval[0], interval[1]]
 
         fig, axes = plt.subplots(nrows=1, ncols=2)
         fig.set_figheight(5)
         fig.set_figwidth(13)
         fig.subplots_adjust(hspace=.5)
 
         axes[0].set_xlim(rang[0][0], rang[0][1])
         axes[0].set_ylim(rang[1][0], rang[1][1])
         axes[0].plot(xvals, yvals, 'o')
+        axes[0].set_aspect('equal', adjustable='box')
         axes[0].set_title('Complex plane')
         axes[0].set_xlabel('real')
         axes[0].set_ylabel('imaginary')
 
         h2d,_,_,img = axes[1].hist2d(xvals, yvals, range=rang,
                                    cmap=plt.cm.get_cmap('nipy_spectral'))
         fig.colorbar(img, ax=axes[1])
@@ -299,16 +316,16 @@
         axes[1].set_title('Eigenvalue heatmap')
         axes[1].set_xlabel('real')
         axes[1].set_ylabel('imaginary')
 
         plt.suptitle("Complex eigenvalues histogram", fontweight="bold")
 
         # Saving plot or showing it
-        if fig_path:
-            plt.savefig(fig_path, dpi=600)
+        if savefig_path:
+            plt.savefig(savefig_path, dpi=600)
         else:
             plt.show()
 
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.8.0/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 
 import numpy as np
 from scipy import sparse, special
 import matplotlib.pyplot as plt
 
-from ._base_ensemble import _Ensemble
+from .base_ensemble import _Ensemble
 from .tridiagonal_utils import tridiag_eigval_hist
 
 #########################################################################
 ### Gaussian Ensemble = Hermite Ensemble
 
 class GaussianEnsemble(_Ensemble):
     """General Gaussian Ensemble class.
@@ -55,15 +55,15 @@
             "Sturm sequences and random eigenvalue distributions".
             Foundations of Computational Mathematics. 9.4 (2008): 461-483.
         - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
 
-    def __init__(self, beta, n, use_tridiagonal=False, sigma=1.0):
+    def __init__(self, beta, n, use_tridiagonal=False, sigma=1.0, random_state=None):
         """Constructor for GaussianEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int, default=1): descriptive integer of the gaussian ensemble type.
                 For GOE beta=1, for GUE beta=2, for GSE beta=4.
@@ -72,75 +72,89 @@
                 and GSE are of size 2n times 2n.
             use_tridiagonal (bool, default=False): if set to True, Gaussian Ensemble
                 matrices are sampled in its tridiagonal form, which has the same
                 eigenvalues than its standard form. Otherwise, it is sampled using
                 its standard form.
             sigma (float, 1.0): scale (standard deviation) of the random entries of the
                 sampled matrix.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy before sampling the random matrix instance. This 
+                has to be any integer between 0 and 2**32 - 1 (inclusive), or None (default).
+                If None, the seed is obtained from the clock.
 
         """
         if beta not in [1,2,4]:
             raise ValueError(f"Invalid beta: {beta}. Beta value has to be 1, 2 or 4.")
 
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
         self.radius = 2 * np.sqrt(self.beta) * self.sigma
         self._eigvals = None
-        self.matrix = self.sample()
+        self.matrix = self.sample(random_state=random_state)
 
         # default eigenvalue normalization constant
         self.eigval_norm_const = 1/np.sqrt(2*self.n) if self.beta==4 else 1/np.sqrt(self.n)
 
         # non-normalized semicircle interval (keys are betas)
         self._non_normalized_interval = {
             1: (-2*np.sqrt(self.n), 2*np.sqrt(self.n)),
             2: (-2*np.sqrt(2*self.n), 2*np.sqrt(2*self.n)),
             4: (-4*np.sqrt(2*self.n), 4*np.sqrt(2*self.n)),
         }
 
-
-    def set_size(self, n, resample_mtx=True):
+    def set_size(self, n, resample_mtx=True, random_state: int = None):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             n (int): new random matrix size. Gaussian ensemble matrices are
                 squared matrices. GOE and GUE are of size n times n, and
                 GSE are of size 2n times 2n.
             resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         """
         self.n = n
         if resample_mtx:
-            self.matrix = self.sample()
+            self.matrix = self.sample(random_state=random_state)
 
     # pylint: disable=inconsistent-return-statements
-    def sample(self):
+    def sample(self, random_state: int = None):
         """Samples new Gaussian Ensemble random matrix.
 
         The sampling algorithm depends on the specification of
         use_tridiagonal parameter. If use_tridiagonal is set to True,
         a Gaussian Ensemble random matrix in its tridiagonal form
         is sampled. Otherwise, it is sampled using the standard
         form.
 
+        Args:
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
+
         Returns:
             numpy array containing new matrix sampled.
 
         References:
             - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
         """
+        if random_state is not None:
+            np.random.seed(random_state)
+
         if self.use_tridiagonal:
             return self.sample_tridiagonal()
 
         if self.beta == 1:
             return self._sample_goe()
         if self.beta == 2:
             return self._sample_gue()
@@ -240,29 +254,29 @@
         if self._eigvals is not None:
             return norm_const * self._eigvals
 
         # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvalsh(self.matrix)
         return norm_const * self._eigvals
 
-    def eigval_hist(self, bins, interval=None, density=False, normalize=True, avoid_img=False):
+    def eigval_hist(self, bins, interval=None, density=False, normalize=False, avoid_img=False):
         if self.use_tridiagonal:
             if normalize:
                 return tridiag_eigval_hist(
                     self.eigval_norm_const * self.matrix,
                     bins=bins,
                     interval=interval,
                     density=density,
                 )
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
         return super().eigval_hist(bins, interval=interval, density=density,
                                    normalize=normalize, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=True, fig_path=None):
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=False, savefig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
@@ -274,19 +288,19 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
-            fig_path (string, default=None): path to save the created figure. If it is not
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False, i.e.,
+                the eigenvalues are not normalized. Normalization makes the eigenvalues to be
+                in the same support independently of the sample size.
+            savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
@@ -298,37 +312,37 @@
             if normalize:
                 interval = (-self.radius, self.radius)
             else:
                 interval = self._non_normalized_interval[self.beta]
 
         if self.use_tridiagonal:
             # pylint: disable=too-many-arguments
-            observed, bins = self.eigval_hist(
+            observed, bin_edges = self.eigval_hist(
                 bins=bins, interval=interval, density=density, normalize=normalize
             )
+            width = bin_edges[1]-bin_edges[0]
+            plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
-            width = bins[1]-bins[0]
-            plt.bar(bins[:-1], observed, width=width, align='edge')
             plt.title("Eigenvalue histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
-            if fig_path:
-                plt.savefig(fig_path, dpi=1000)
+            if savefig_path:
+                plt.savefig(savefig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
             # pylint: disable=too-many-arguments
             super().plot_eigval_hist(
                 bins=bins,
                 interval=interval,
                 density=density,
                 normalize=normalize,
-                fig_path=fig_path,
+                savefig_path=savefig_path,
             )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
         eigenvalues. If the array of eigenvalues is not provided, the current random
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.8.0/skrmt/ensemble/manova_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 and Manova Quaternion Ensemble.
 
 """
 
 import numpy as np
 from scipy import special
 
-from ._base_ensemble import _Ensemble
+from .base_ensemble import _Ensemble
 
 
 #########################################################################
 ### Manova Ensemble = Jacobi Ensemble
 
 class ManovaEnsemble(_Ensemble):
     """General Manova Ensemble class.
@@ -63,79 +63,94 @@
             "Local Eigenvalue Density for General MANOVA Matrices".
             Journal of Statistical Physics. 152.6 (2013): 1003-1032.
         - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
     """
 
-    def __init__(self, beta, m, n1, n2):
+    def __init__(self, beta, m, n1, n2, random_state=None):
         """Constructor for ManovaEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int): descriptive integer of the Manova ensemble type.
                 For Real beta=1, for Complex beta=2, for Quaternion beta=4.
             m (int): number of rows of the random guassian matrices that
                 generates the matrix of the corresponding ensemble.
             n1 (int): number of columns of the first random guassian matrix
                 that generates the matrix of the corresponding ensemble.
             n2 (int): number of columns of the second random guassian matrix
                 that generates the matrix of the corresponding ensemble.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy before sampling the random matrix instance. This 
+                has to be any integer between 0 and 2**32 - 1 (inclusive), or None (default).
+                If None, the seed is obtained from the clock.
 
         """
         super().__init__()
         # pylint: disable=invalid-name
         self.m = m
         self.n1 = n1
         self.n2 = n2
         self.beta = beta
         self._eigvals = None
-        self.matrix = self.sample()
+        self.matrix = self.sample(random_state=random_state)
 
-    def set_size(self, m, n1, n2, resample_mtx=True):
+    def set_size(self, m, n1, n2, resample_mtx=True, random_state: int = None):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             m (int): number of rows of the random guassian matrices that
                 generates the matrix of the corresponding ensemble.
             n1 (int): number of columns of the first random guassian matrix
                 that generates the matrix of the corresponding ensemble.
             n2 (int): number of columns of the second random guassian matrix
                 that generates the matrix of the corresponding ensemble.
             resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         """
         self.m = m
         self.n1 = n1
         self.n2 = n2
         if resample_mtx:
-            self.matrix = self.sample()
+            self.matrix = self.sample(random_state=random_state)
 
     # pylint: disable=inconsistent-return-statements
-    def sample(self):
+    def sample(self, random_state: int = None):
         """Samples new Manova Ensemble random matrix.
 
         The sampling algorithm depends on the specification of
         beta parameter. If beta=1, Manova Real is sampled; if
         beta=2 Manova Complex is sampled and if beta=4
         Manova Quaternion is sampled.
 
+        Args:
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
+
         Returns:
             numpy array containing new matrix sampled.
 
         References:
             - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
+        if random_state is not None:
+            np.random.seed(random_state)
+
         if self.beta == 1:
             return self._sample_mre()
         if self.beta == 2:
             return self._sample_mce()
         if self.beta == 4:
             return self._sample_mqe()
 
@@ -222,15 +237,15 @@
         if self._eigvals is not None:
             return norm_const * self._eigvals
 
         # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvals(self.matrix)
         return norm_const * self._eigvals
 
-    def plot_eigval_hist(self, bins, interval=(0,1), density=False, normalize=True, fig_path=None):
+    def plot_eigval_hist(self, bins, interval=(0,1), density=False, normalize=False, savefig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
 
         Args:
             bins (int or sequence): If bins is an integer, it defines the number of
                 equal-width bins in the range. If bins is a sequence, it defines the
@@ -239,19 +254,19 @@
             interval (tuple, default=(0,1)): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
-            fig_path (string, default=None): path to save the created figure. If it is not
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False, i.e.,
+                the eigenvalues are not normalized. Normalization makes the eigenvalues to be
+                in the same support independently of the sample size.
+            savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Erdos, L. and Farrell, B.
                 "Local Eigenvalue Density for General MANOVA Matrices".
                 Journal of Statistical Physics. 152.6 (2013): 1003-1032.
             - Dumitriu, I. and Edelman, A.
@@ -261,15 +276,15 @@
         """
         # pylint: disable=too-many-arguments
         return super().plot_eigval_hist(
             bins=bins,
             interval=interval,
             density=density,
             normalize=normalize,
-            fig_path=fig_path,
+            savefig_path=savefig_path,
             avoid_img=True,
         )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/spectral_law.py` & `scikit-rmt-0.8.0/skrmt/ensemble/spectral_law.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,27 @@
-"""Law module
+"""Spectral Law module
 
 This module contains classes that implement the main spectral distributions.
 When the limiting behaviour of the spectrum of a random matrix ensemble is
 well-known, it is often described with a mathematical proven law.
 Probability density functions and cumulative distribution functions are provided
 for the Wigner Semicircle Law, Marchenko-Pastur Law, Tracy-Widom Law and for the
 spectrum of the Manova Ensemble.
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.integrate import quad
+from scipy.stats import rv_continuous
+from scipy import interpolate
 import collections.abc
 
-from .gaussian_ensemble import GaussianEnsemble
-from .wishart_ensemble import WishartEnsemble
-from .manova_ensemble import ManovaEnsemble
 from .tracy_widom_approximator import TW_Approximator
-
-
-def _relu(x):
-    """Element-wise maximum between the value and zero.
-
-    Args:
-        x (ndarray): list of numbers to compute its element-wise maximum.
-    
-    Returns:
-        array_like consisting in the element-wise maximum vector of the given values.
-    """
-    return np.maximum(x, np.zeros_like(x))
-
-
-def _indicator(x, start=None, stop=None, inclusive="both"):
-    r"""Element-wise indicator function within a real interval.
-    The interval can be left-closed, right-closed, closed or open.
-    Visit https://en.wikipedia.org/wiki/Indicator_function for more information.
-
-    Args:
-        x (ndarray): list of numbers to compute its element-wise indicator image.
-        start (double, default=None): left value of the interval. If not provided,
-            the left value is equivalent to :math:`- \infty`.
-        stop (double, default=None): right value of the interval. If not provided,
-            the right value is equivalent to :math:`+ \infty`.
-        inclusive (string, default="both"): type of interval. For left-closed interval
-            use "left", for right-closed interval use "right", for closed interval use
-            "both" and for open interval use "neither".
-
-    Returns:
-        array_like consisting in the element-wise indicator function image of the given values.
-    """
-    if start is None and stop is None:
-        raise ValueError("Error: provide start and/or stop for indicator function.")
-
-    INCLUSIVE_OPTIONS = ["both", "left", "right", "neither"]
-    if inclusive not in INCLUSIVE_OPTIONS:
-        raise ValueError(f"Error: invalid interval inclusive parameter: {inclusive}\n"
-                         "\t inclusive has to be one of the following: {INCLUSIVE_OPTIONS}.")
-
-    if start is not None:
-        if inclusive == "both" or inclusive == "left":
-            condition = (start <= x)
-        elif inclusive == "neither" or inclusive == "right":
-            condition = (start < x)
-    
-    if (start is not None) and (stop is not None):
-        if inclusive == "both" or inclusive == "right":
-            condition = np.logical_and(condition, (x <= stop))
-        elif inclusive == "neither" or inclusive == "left":
-            condition = np.logical_and(condition, (x < stop))
-    elif stop:
-        if inclusive == "both" or inclusive == "right":
-            condition = (x <= stop)
-        elif inclusive == "neither" or inclusive == "left":
-            condition = (x < stop)
-
-    return np.where(condition, 1.0, 0.0)
-
-
-def _plot_func(interval, func, bins=1000, plot_title=None, plot_ylabel=None, savefig_path=None):
-    """Plots a given function (callable) within the provided interval.
-
-    Args:
-        interval (tuple): Delimiters (xmin, xmax) of the histogram.
-        func (callable): Function to be evaluated. The image of the function builds
-            the y-axis values that are plotted.
-        bins (int, default=100): It defines the number of equal-width bins within the
-            provided interval or range.
-        plot_title (string, default=None): Title of the plot.
-        plot_ylabel (string, default=None): Label of the y-axis.
-        savefig_path (string, default=None): path to save the created figure. If it is not
-            provided, the plot is shown at the end of the routine.
-    
-    """
-    if not isinstance(interval, tuple):
-        raise ValueError("interval argument must be a tuple")
-    
-    (xmin, xmax) = interval
-
-    xx = np.linspace(xmin, xmax, num=bins)
-    yy = func(xx)
-
-    plt.plot(xx, yy)
-    plt.xlabel("x")
-    if plot_ylabel:
-        plt.ylabel(plot_ylabel)
-    
-    if plot_title:
-        plt.title(plot_title)
-
-    if savefig_path:
-        plt.savefig(savefig_path, dpi=800)
-    else:
-        plt.show()
-
-
-def _get_bins_centers_and_contour(bins):
-    """Calculates the centers and contour of the given bins.
-
-    Computes the centers of the given bins. Also, the smallest and the largest bin
-    delimitiers are included to define the countour of the representation interval.
-
-    Args:
-        bins (list): list of numbers (floats) that specify each bin delimiter.
-
-    Returns:
-        list of numbers (floats) consisting in the list of bin centers and contour.
-    
-    """
-    centers = [bins[0]] # Adding initial contour
-    l = len(bins)
-    for i in range(l-1):
-        centers.append((bins[i]+bins[i+1])/2) # Adding centers
-    centers.append(bins[-1]) # Adding final contour
-    return centers
+from .misc import relu, indicator, plot_func, get_bins_centers_and_contour
 
 
 class WignerSemicircleDistribution:
     """Wigner Semicircle Distribution class.
 
     The Wigner Semicircle Law describes the spectrum of the Wigner random matrices.
     In particular, random matrices of the Gaussian Ensemble are Wigner matrices,
@@ -184,27 +68,34 @@
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
 
         self.beta = beta
         self.center = center
         self.sigma = sigma
         self.radius = 2.0 * np.sqrt(self.beta) * self.sigma
-    
-    def rvs(self, size):
+        self.default_interval = (self.center - self.radius, self.center + self.radius)
+
+    def rvs(self, size, random_state: int = None):
         """Samples ranfom variates following this distribution.
         This uses the relationship between Wigner Semicircle law and Beta distribution.
 
         Args:
             size (int): sample size.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
         
         Returns:
             numpy array with the generated samples.
         """
         if size <= 0:
             raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
+        
+        if random_state is not None:
+            np.random.seed(random_state)
 
         # Use relationship with beta distribution
         beta_samples = np.random.beta(1.5, 1.5, size=size)
         return self.center + 2*self.radius*beta_samples - self.radius
 
     def pdf(self, x):
         """Computes PDF of the Wigner Semicircle Law.
@@ -212,15 +103,15 @@
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
         Returns:
             float or numpy array with the computed PDF in the given value(s).
         
         """
-        return 2.0 * np.sqrt(_relu(self.radius**2 - (x-self.center)**2)) / (np.pi * self.radius**2)
+        return 2.0 * np.sqrt(relu(self.radius**2 - (x-self.center)**2)) / (np.pi * self.radius**2)
     
     def cdf(self, x):
         """Computes CDF of the Wigner Semicircle Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the CDF.
         
@@ -232,109 +123,123 @@
             return np.select(
                 condlist=[x >= (self.center + self.radius), x <= (self.center - self.radius)],
                 choicelist=[1.0, 0.0],
                 default=(0.5 + ((x-self.center) * np.sqrt(self.radius**2 - (x-self.center)**2))/(np.pi * self.radius**2) \
                          + (np.arcsin((x-self.center)/self.radius)) / np.pi)
             )
     
-    def plot_pdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_pdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the PDF of the Wigner Semicircle Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, center, radius and scale.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.center - self.radius - 0.1, self.center + self.radius + 0.1)
         
-        _plot_func(
-            interval, func=self.pdf, bins=bins, plot_title="Wigner Semicircle law PDF", 
+        plot_func(
+            interval, func=self.pdf, num_x_vals=num_x_vals, plot_title="Wigner Semicircle law PDF", 
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
-    def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_cdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the CDF of the Wigner Semicircle Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, center, radius and scale.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.center - self.radius - 0.1, self.center + self.radius + 0.1)
         
-        _plot_func(
-            interval, func=self.cdf, bins=bins, plot_title="Wigner Semicircle law CDF",
+        plot_func(
+            interval, func=self.cdf, num_x_vals=num_x_vals, plot_title="Wigner Semicircle law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
-    
 
-    def plot_empirical_pdf(self, n_size=10000, bins=100, interval=None, density=False,
-                           plot_law_pdf=False, savefig_path=None):
+    def plot_empirical_pdf(self, sample_size=10000, bins=100, interval=None, density=False,
+                           plot_law_pdf=False, savefig_path=None, random_state=None):
         """Computes and plots Wigner's semicircle empirical law.
 
         Calculates and plots Wigner's semicircle empirical law using random samples generated
         using the relationship between the Wigner Semicircle law and the Beta distribution:
         the Wigner's Semicircle distribution it is a scaled Beta distribution with parameters
         :math:`\alpha = \beta = 3/2`.
 
         Args:
-            n_size (int, default=1000): number of random samples that can be interpreted as
+            sample_size (int, default=1000): number of random samples that can be interpreted as
                 random eigenvalues of a Wigner matrix. This is the sample size.
             bins (int or sequence, default=100): If bins is an integer, it defines the number
                 of equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
+                If one of the bounds of the specified interval is outside of the minimum default
+                interval, this will be adjusted to show the distribution bulk properly.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             plot_law_pdf (bool, default=False): If True, the theoretical law is plotted.
                 If set to False, just the empirical histogram is shown. This parameter is only
                 considered when the argument 'density' is set also to True.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown are the end of the routine.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
-        if n_size<1:
-            raise ValueError("matrix size must be positive")
+        if sample_size<1:
+            raise ValueError("Negative eigenvalue sample size (given = {sample_size})."
+                             " Please, provide a sample size greater or equal than 1.")
         
         if interval is None:
-            interval = (self.center - self.radius, self.center + self.radius)
+            range_interval = self.default_interval
+        else:
+            xmin = min(interval[0], self.default_interval[0])
+            xmax = max(interval[1], self.default_interval[1])
+            if interval[0] > self.default_interval[0]:
+                print(f"Lower bound of interval too large. Setting lower bound to {xmin}.")
+            if interval[1] < self.default_interval[1]:
+                print(f"Upper bound of interval too large. Setting upper bound to {xmax}.")
+            range_interval = (xmin, xmax)
+            print(f"Setting plot interval to {range_interval}.")
 
-        random_samples = self.rvs(size=n_size)
-        observed, bins = np.histogram(random_samples, bins=bins, range=interval, density=density)
+        random_samples = self.rvs(size=sample_size, random_state=random_state)
+        observed, bin_edges = np.histogram(random_samples, bins=bins, range=range_interval, density=density)
 
-        width = bins[1]-bins[0]
-        plt.bar(bins[:-1], observed, width=width, align='edge')
+        width = bin_edges[1]-bin_edges[0]
+        plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
         # Plotting Wigner Semicircle Law pdf
         if plot_law_pdf and density:
-            centers = np.asarray(_get_bins_centers_and_contour(bins))
+            centers = np.asarray(get_bins_centers_and_contour(bin_edges))
             pdf = self.pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
         elif plot_law_pdf and not density:
             print("Warning: Wigner's Semicircle Law PDF is only plotted when density is True.")
 
         plt.title("Wigner Semicircle Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
@@ -344,15 +249,15 @@
         if savefig_path:
             plt.savefig(savefig_path, dpi=1200)
         else:
             plt.show()
 
 
 
-class MarchenkoPasturDistribution:
+class MarchenkoPasturDistribution(rv_continuous):
     """Marchenko-Pastur Distribution class.
 
     The Marchenko-Pastur Law describes the spectrum of the Wishart random matrices.
     Therefore the spectrum of the random matrices of this ensemble converge
     to the Marchenko-Pastur Law when the matrix size goes to infinity. This
     class provides methods to sample eigenvalues following Marchenko-Pastur
     distribution, computing the PDF, computing the CDF and simple methods to
@@ -391,88 +296,92 @@
                 The value of ratio is computed as :math:`\lambda = p/n`.
             beta (int, default=1): descriptive integer of the Wishart ensemble type (:math:`\beta`).
                 For WRE beta=1, for WCE beta=2, for WQE beta=4.
             sigma (float, default=1.0): scale of the distribution (:math:`\sigma`). This value also
                 corresponds to the standard deviation of the random entries of the sampled matrix.
         
         """
+        super().__init__()
+
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
         if ratio <= 0:
             raise ValueError(f"Error: invalid ratio. It has to be positive. Provided ratio = {ratio}.")
 
         self.ratio = ratio
         self.beta = beta
         self.sigma = sigma
         self.lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(self.ratio))**2
         self.lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(self.ratio))**2
         self._var = self.beta * self.sigma**2
-        self._wishart_ens = None
+        self._set_default_interval()
+        # when the support is finite (lambda_minus, lambda_plus) it is better
+        # to explicity approximate the inverse of the CDF to implement rvs
+        self._approximate_inv_cdf()
     
-    def rvs(self, size):
-        """Samples ranfom variates following this distribution.
-
-        Args:
-            size (int): sample size :math:`n`.
-        
-        Returns:
-            numpy array with the generated samples.
-        """
-        if size <= 0:
-            raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
-        
-        _n = int(np.round(size / self.ratio))
-
-        if not self._wishart_ens:
-            self._wishart_ens = WishartEnsemble(beta=self.beta, p=size, n=_n, use_tridiagonal=False, sigma=self.sigma)
+    def _set_default_interval(self):
+        # computing interval according to the matrix size ratio and support
+        if self.ratio <= 1:
+            self.default_interval = (self.lambda_minus, self.lambda_plus)
         else:
-            self._wishart_ens.set_size(p=size, n=_n, resample_mtx=True)
+            self.default_interval = (min(-0.05, self.lambda_minus), self.lambda_plus)
+    
+    def _approximate_inv_cdf(self):
+        # https://gist.github.com/amarvutha/c2a3ea9d42d238551c694480019a6ce1
+        x_vals = np.linspace(self.lambda_minus, self.lambda_plus, 1000)
+        _pdf = self._pdf(x_vals)
+        _cdf = np.cumsum(_pdf)      # approximating CDF
+        cdf_y = _cdf/_cdf.max()     # normalizing approximated CDF to 1.0
+        self._inv_cdf = interpolate.interp1d(cdf_y, x_vals)
+
+    def _rvs(self, size, random_state, _random_state=None):
+        if _random_state is not None:
+            np.random.seed(_random_state)
 
-        if self.beta == 4:
-            return self._wishart_ens.eigvals(normalize=True)[::2]
-        return self._wishart_ens.eigvals(normalize=True)
+        uniform_samples = np.random.random(size=size)
+        return self._inv_cdf(uniform_samples)
 
-    def pdf(self, x):
+    def _pdf(self, x):
         """Computes PDF of the Marchenko-Pastur Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
         Returns:
             float or numpy array with the computed PDF in the given value(s).
         
         """
         with np.errstate(divide='ignore', invalid='ignore'):
-            return np.sqrt(_relu(self.lambda_plus - x) * _relu(x - self.lambda_minus)) \
+            return np.sqrt(relu(self.lambda_plus - x) * relu(x - self.lambda_minus)) \
                 / (2.0 * np.pi * self.ratio * self._var * x)
 
-    def cdf(self, x):
+    def _cdf(self, x):
         """Computes CDF of the Marchenko-Pastur Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the CDF.
         
         Returns:
             float or numpy array with the computed CDF in the given value(s).
         
         """
         with np.errstate(divide='ignore', invalid='ignore'):
-            acum = _indicator(x, start=self.lambda_plus, inclusive="left")
-            acum += np.where(_indicator(x, start=self.lambda_minus, stop=self.lambda_plus, inclusive="left"),
+            acum = indicator(x, start=self.lambda_plus, inclusive="left")
+            acum += np.where(indicator(x, start=self.lambda_minus, stop=self.lambda_plus, inclusive="left"),
                             self._cdf_aux_f(x), 0.0)
 
             if self.ratio <= 1:
                 return acum
             
-            acum += np.where(_indicator(x, start=self.lambda_minus, stop=self.lambda_plus, inclusive="left"),
+            acum += np.where(indicator(x, start=self.lambda_minus, stop=self.lambda_plus, inclusive="left"),
                             (self.ratio-1)/(2*self.ratio), 0.0)
 
             ### This would need to be added if the extra density point at zero is measured
             # https://en.wikipedia.org/wiki/Marchenko%E2%80%93Pastur_distribution
-            # acum += np.where(_indicator(x, start=0, stop=self.lambda_minus, inclusive="left"),
+            # acum += np.where(indicator(x, start=0, stop=self.lambda_minus, inclusive="left"),
             #                 (self.ratio-1)/self.ratio, 0.0)
             return acum
 
     def _cdf_aux_f(self, x):
         first_arctan_term = np.where(x == self.lambda_minus,
                                     MarchenkoPasturDistribution.ARCTAN_OF_INFTY,
                                     np.arctan((self._cdf_aux_r(x)**2 - 1)/(2 * self._cdf_aux_r(x)))
@@ -480,62 +389,62 @@
 
         second_arctan_term = np.where(x == self.lambda_minus,
                                       MarchenkoPasturDistribution.ARCTAN_OF_INFTY,
                                       np.arctan((self.lambda_minus*self._cdf_aux_r(x)**2 - self.lambda_plus) \
                                                 / (2*self._var*(1-self.ratio)*self._cdf_aux_r(x)))
                                 )
         return 1/(2*np.pi*self.ratio) * (np.pi*self.ratio \
-                                         + (1/self._var)*np.sqrt(_relu(self.lambda_plus-x)*_relu(x-self.lambda_minus)) \
+                                         + (1/self._var)*np.sqrt(relu(self.lambda_plus-x)*relu(x-self.lambda_minus)) \
                                          - (1+self.ratio)*first_arctan_term + (1-self.ratio)*second_arctan_term)
 
     def _cdf_aux_r(self, x):
         return np.sqrt((self.lambda_plus-x)/(x - self.lambda_minus))
 
-    def plot_pdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_pdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the PDF of the Marchenko-Pastur Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, ratio, and scale.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
-        _plot_func(
-            interval, func=self.pdf, bins=bins, plot_title="Marchenko-Pastur law PDF",
+        plot_func(
+            interval, func=self._pdf, num_x_vals=num_x_vals, plot_title="Marchenko-Pastur law PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
-    def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_cdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the CDF of the Marchenko-Pastur Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, ratio, and scale.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
-        _plot_func(
-            interval, func=self.cdf, bins=bins, plot_title="Marchenko-Pastur law CDF",
+        plot_func(
+            interval, func=self._cdf, num_x_vals=num_x_vals, plot_title="Marchenko-Pastur law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
-    def plot_empirical_pdf(self, n_size=3000, p_size=None, bins=100, interval=None,
-                           density=False, plot_law_pdf=False, savefig_path=None):
+    def plot_empirical_pdf(self, sample_size=1000, bins=100, interval=None, density=False,
+                           plot_law_pdf=False, savefig_path=None, random_state=None):
         """Computes and plots Marchenko-Pastur empirical law using Wishart Ensemble random matrices.
 
         Calculates and plots Marchenko-Pastur empirical law using Wishart Ensemble random matrices.
         The size of the sampled matrix will depend on the `n_size` (:math:`n`) parameter and on the
         ratio :math:`\lambda` given when instantiating this class, unless the parameter `p_size` (:math:`p`)
         is also given. In this last case, the ratio :math:`\lambda` for the empirical pdf plotting is
         computed as :math:`\lambda = p/n`. If only the sample size :math:`n` is provided, the number
@@ -556,91 +465,73 @@
                 (but not replaced) and the new ratio=p_size/n_size is used instead.
             bins (int or sequence, default=100): If bins is an integer, it defines the number
                 of equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
+                If one of the bounds of the specified interval is outside of the minimum default
+                interval, this will be adjusted to show the distribution bulk properly.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
                 If set to False, just the empirical histogram is shown. This parameter is only
                 considered when the argument 'density' is set also to True.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown are the end of the routine.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
-        if n_size<1 or (p_size is not None and p_size<1):
-            raise ValueError("matrix size must be positive")
-        
-        if interval and interval[0] == 0:
-            print("Warning: setting the beginning of the interval to zero may generate numerical errors.")
-            print(f"Setting interval to (-0.01, {interval[1]})")
-            interval = (-0.01, interval[1])
-
-        # calculating constants depending on matrix sizes
-        if p_size is None:
-            p_size = round(self.ratio * n_size)
-
-        # computing an approximated ratio since p_size is rounded to the closest integer        
-        approx_ratio = p_size/n_size
-        lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(approx_ratio))**2
-        lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(approx_ratio))**2
-        use_tridiag_ratio = (approx_ratio <= 1)
-        if not use_tridiag_ratio:
-            print("Warning: Cannot use tridiagonal histogramming if 'p' (degrees of freedom) is "
-                " greater than 'n' (sample size).\n"
-                f"\t Provided n={n_size} and p={p_size}. Tridiagonal histogramming is therefore deactivated.\n"
-                "\t It is adviced to increase sample size (`n`) to optimize and boost histogramming.")
+        if sample_size<1:
+            raise ValueError("Negative eigenvalue sample size (given = {sample_size})."
+                             " Please, provide a sample size greater or equal than 1.")
 
-        # computing interval according to the matrix size ratio and support
         if interval is None:
-            if approx_ratio <= 1:
-                interval = (lambda_minus, lambda_plus)
-            else:
-                interval = (min(-0.05, lambda_minus), lambda_plus)
+            range_interval = self.default_interval
+        else:
+            xmin = min(interval[0], self.default_interval[0])
+            xmax = max(interval[1], self.default_interval[1])
+            if interval[0] > self.default_interval[0]:
+                print(f"Lower bound of interval too large. Setting lower bound to {xmin}.")
+            if interval[1] < self.default_interval[1]:
+                print(f"Upper bound of interval too large. Setting upper bound to {xmax}.")
+            range_interval = (xmin, xmax)
+            print(f"Setting plot interval to {range_interval}.")
         
-        use_tridiag_sigma = (self.sigma == 1.0)
-        if not use_tridiag_sigma:
-            print(f"Warning: The given scale is not the standard (sigma = {self.sigma}).\n"
-                "\t Tridiagonal histogramming is deactivated.\n"
-                "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
-
-        ens = WishartEnsemble(beta=self.beta, p=p_size, n=n_size, sigma=self.sigma,
-                            use_tridiagonal=(use_tridiag_ratio and use_tridiag_sigma))
-
-        observed, bins = ens.eigval_hist(bins=bins, interval=interval, density=density, normalize=True)
+        random_samples = self._rvs(size=sample_size, random_state=random_state, _random_state=random_state)
+        observed, bin_edges = np.histogram(random_samples, bins=bins, range=range_interval, density=density)
 
-        width = bins[1]-bins[0]
-        plt.bar(bins[:-1], observed, width=width, align='edge')
+        width = bin_edges[1]-bin_edges[0]
+        plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
-            centers = np.array(_get_bins_centers_and_contour(bins))
+            centers = np.asarray(get_bins_centers_and_contour(bin_edges))
             # creating new instance with the approximated ratio depending on the given matrix sizes
-            mpd = MarchenkoPasturDistribution(beta=self.beta, ratio=approx_ratio, sigma=self.sigma)
-            pdf = mpd.pdf(centers)
+            pdf = self._pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
         plt.title("Marchenko-Pastur Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
-        if approx_ratio > 1:
+        if self.ratio > 1:
             if plot_law_pdf and density:
                 ylim_vals = pdf
             else:
                 ylim_vals = observed
             try:
                 plt.ylim(0, np.max(ylim_vals)+0.25*np.max(ylim_vals))
             except ValueError:
@@ -651,15 +542,15 @@
         if savefig_path:
             plt.savefig(savefig_path, dpi=1200)
         else:
             plt.show()
 
 
 
-class TracyWidomDistribution:
+class TracyWidomDistribution(rv_continuous):
     """Tracy-Widom Distribution class.
 
     The Tracy-Widom Law describes the behaviour of the largest eigenvalue of the
     Wigner random matrices. In particular, random matrices of the Gaussian Ensemble
     are Wigner matrices, and therefore the largest eigenvalues of the spectrum of
     the random matrices of this ensemble converge to the Tracy-Widom Law when the
     matrix size and the sample size (number of times a Wigner matrix is generated to
@@ -696,211 +587,172 @@
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int, default=1): descriptive integer of the Gaussian ensemble type.
                 For GOE beta=1, for GUE beta=2, for GSE beta=4.
         
         """
+        super().__init__()
+
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
 
         self.beta = beta
         self.tw_approx = TW_Approximator(beta=self.beta)
+        self.default_interval = (-5, 4-self.beta)
 
-    def rvs(self, size, mtx_size=100):
-        """Samples ranfom variates following this distribution.
-
-        Args:
-            size (int): sample size.
-            mtx_size (int, default=100): matrix size. Remember the Tracy-Widom Law describes the
-                limiting behaviour of the largest eigenvalue of a Wigner matrix. Therefore,
-                a matrix has to be generated to get each sample. This argument specifies the size
-                of the matrix.
-        
-        Returns:
-            numpy array with the generated samples.
-        """
-        if size <= 0:
-            raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
-        if mtx_size <= 0:
-            raise ValueError(f"Error: invalid matrix size. It has to be positive. Provided matrix size = {mtx_size}.")
-
-        self._gaussian_ens = GaussianEnsemble(beta=self.beta, n=mtx_size, use_tridiagonal=False)
-
-        max_eigvals = []
-        for _ in range(size):
-            max_eigvals.append(self._gaussian_ens.eigvals(normalize=False).max())
-            self._gaussian_ens.sample()
-        max_eigvals = np.asarray(max_eigvals)
-
-        # Tracy-Widom eigenvalue distr. normalization constants
-        eigval_scale = 1.0
-        size_scale = 1.0
-        if self.beta == 2:
-            eigval_scale = 1/np.sqrt(2)
-        if self.beta == 4:
-            eigval_scale = size_scale = 1/np.sqrt(2)
-            mtx_size *= 2
-
-        max_eigvals = size_scale*(mtx_size**(1/6))*(eigval_scale*max_eigvals - (2.0*np.sqrt(mtx_size)))
-        return max_eigvals
-
-    def pdf(self, x):
+    def _pdf(self, x):
         """Computes PDF of the Tracy-Widom Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
         Returns:
             float or numpy array with the computed PDF in the given value(s).
         
         """
         return self.tw_approx.pdf(x)
 
-    def cdf(self, x):
+    def _cdf(self, x):
         """Computes CDF of the Tracy-Widom Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the CDF.
         
         Returns:
             float or numpy array with the computed CDF in the given value(s).
         
         """
         return self.tw_approx.cdf(x)
 
-    def plot_pdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_pdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the PDF of the Tracy-Widom Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
-            interval = (-5, 4-self.beta)
+            interval = self.default_interval
         
-        _plot_func(
-            interval, func=self.pdf, bins=bins, plot_title="Tracy-Widom law PDF",
+        plot_func(
+            interval, func=self._pdf, num_x_vals=num_x_vals, plot_title="Tracy-Widom law PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
-    def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_cdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the PDF of the Tracy-Widom Law.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
-            interval = (-5, 4-self.beta)
+            interval = self.default_interval
         
-        _plot_func(
-            interval, func=self.cdf, bins=bins, plot_title="Tracy-Widom law CDF",
+        plot_func(
+            interval, func=self._cdf, num_x_vals=num_x_vals, plot_title="Tracy-Widom law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
-    def plot_empirical_pdf(self, n_size=100, times=1000, bins=100, interval=None,
-                           density=False, plot_law_pdf=False, savefig_path=None):
+    def plot_empirical_pdf(self, sample_size=1000, bins=100, interval=None, density=False,
+                           plot_law_pdf=False, savefig_path=None, random_state=None):
         """Computes and plots Tracy-Widom empirical law using Gaussian Ensemble.
 
         Calculates and plots Tracy-Widom empirical law using Gaussian Ensemble random matrices.
         Because we need to obtain the largest eigenvalue of each sampled random matrix,
         we need to sample a certain amount them. For each random matrix sammpled, its
         largest eigenvalue is calcualted in order to simulate its density.
 
         Args:
             n_size (int, default=100): random matrix size n times n. This is the sample size.
             times (int, default=1000): number of times to sample a random matrix.
             bins (int or sequence, default=100): If bins is an integer, it defines the number
                 of equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
-            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
-                The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
+            interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
+                The lower and upper range of the bins. Lower and upper outliers are ignored.
+                If one of the bounds of the specified interval is outside of the minimum default
+                interval, this will be adjusted to show the distribution bulk properly.
             plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
                 If set to False, just the empirical histogram is shown. This parameter is only
                 considered when the argument 'density' is set also to True.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown are the end of the routine.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
-        if n_size<1 or times<1:
-            raise ValueError("matrix size or number of repetitions must be positive")
+        if sample_size<1:
+            raise ValueError("Negative eigenvalue sample size (given = {sample_size})."
+                             " Please, provide a sample size greater or equal than 1.")
 
-        ens = GaussianEnsemble(beta=self.beta, n=n_size, use_tridiagonal=False)
+        if interval is None:
+            range_interval = self.default_interval
+        else:
+            xmin = min(interval[0], self.default_interval[0])
+            xmax = max(interval[1], self.default_interval[1])
+            if interval[0] > self.default_interval[0]:
+                print(f"Lower bound of interval too large. Setting lower bound to {xmin}.")
+            if interval[1] < self.default_interval[1]:
+                print(f"Upper bound of interval too large. Setting upper bound to {xmax}.")
+            range_interval = (xmin, xmax)
+            print(f"Setting plot interval to {range_interval}.")
 
-        eigvals = []
-        for _ in range(times):
-            eigvals.append(ens.eigvals(normalize=False).max())
-            ens.sample()
-        eigvals = np.asarray(eigvals)
-
-        # Tracy-Widom eigenvalue distr. normalization constants
-        eigval_scale = 1.0
-        size_scale = 1.0
-        if self.beta == 2:
-            eigval_scale = 1/np.sqrt(2)
-        elif self.beta == 4:
-            eigval_scale = size_scale = 1/np.sqrt(2)
-            n_size *= 2
-        eigvals = size_scale*(n_size**(1/6))*(eigval_scale*eigvals - (2.0*np.sqrt(n_size)))
+        random_samples = self.rvs(size=sample_size, random_state=random_state)
+        observed, bin_edges = np.histogram(random_samples, bins=bins, range=range_interval, density=density)
 
-        if interval is None:
-            xmin=eigvals.min()
-            xmax=eigvals.max()
-            interval=(xmin, xmax)
-
-        # using numpy to obtain histogram in the given interval and no. of bins
-        observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
-        width = bins[1]-bins[0]
-        plt.bar(bins[:-1], observed, width=width, align='edge')
+        width = bin_edges[1]-bin_edges[0]
+        plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
-            centers = _get_bins_centers_and_contour(bins)
-            pdf = self.pdf(centers)
+            centers = get_bins_centers_and_contour(bin_edges)
+            pdf = self._pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
         plt.title("Tracy-Widom Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
 
         # Saving plot or showing it
         if savefig_path:
             plt.savefig(savefig_path, dpi=1200)
         else:
             plt.show()
 
 
 
-class ManovaSpectrumDistribution:
+class ManovaSpectrumDistribution(rv_continuous):
     """Manova Spectrum Distribution class.
 
     The spectrum of the random matrices of the Manova Ensemble converge to a
     well-defined function implemented in this class. The class provides methods
     to sample eigenvalues of the Manova Ensemble, computing the PDF, computing
     the CDF and simple methods to plot the former two.
 
@@ -925,162 +777,180 @@
     References:
         - Erdos, L. and Farrell, B.
             "Local Eigenvalue Density for General MANOVA Matrices".
             Journal of Statistical Physics. 152.6 (2013): 1003-1032.
     
     """
 
-    def __init__(self, a, b, beta=1):
+    def __init__(self, ratio_a, ratio_b, beta=1):
         """Constructor for ManovaSpectrumDistribution class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
-            a (float): first random matrix size ratio. This is the ratio between the
+            ratio_a (float): first random matrix size ratio. This is the ratio between the
                 number of degrees of freedom 'p' and the first sample size 'n1'. The value
                 of a = p/n1. Remember a Manova randon matrix is considered a double-Wishart
                 matrix, that's why there are two sample sizes 'n1' and 'n2' (see below).
-            b (float): second random matrix size ratio. This is the ratio between the
+            ratio_b (float): second random matrix size ratio. This is the ratio between the
                 number of degrees of freedom 'p' and the second sample size 'n2'. The value
                 of b = p/n2. Remember a Manova randon matrix is considered a double-Wishart
                 matrix, that's why there are two sample sizes 'n1' and 'n2'.
             beta (int, default=1): descriptive integer of the Manova ensemble type.
                 For MRE beta=1, for WME beta=2, for MQE beta=4.
         
         """
+        super().__init__()
+
         if beta not in [1,2,4]:
             raise ValueError(f"Error: invalid beta. It has to be 1,2 or 4. Provided beta = {beta}.")
-        if a <= 0 or b <= 0:
+        if ratio_a <= 0 or ratio_b <= 0:
             raise ValueError("Error: invalid matrix parameters. They have to be both positive.\n"
-                             f"\tProvided a = {a} and b = {b}.")
+                             f"\tProvided a = {ratio_a} and b = {ratio_b}.")
 
-        if a < 1 or b < 1:
-            print(f"Warning: Setting a < 1 (a = {a}) or b < 1 (b = {b}) may cause numerical instability.")
+        if ratio_a < 1 or ratio_b < 1:
+            print(f"Warning: Setting a < 1 (a = {ratio_a}) or b < 1 (b = {ratio_b}) may cause numerical instability.")
 
-        self.a = a
-        self.b = b
+        self.ratio_a = ratio_a
+        self.ratio_b = ratio_b
         self.beta = beta
-        self.lambda_term1 = np.sqrt((a/(a+b)) * (1 - (1/(a+b))))
-        self.lambda_term2 = np.sqrt((1/(a+b)) * (1 - (a/(a+b))))
+        self.lambda_term1 = np.sqrt((ratio_a/(ratio_a + ratio_b)) * (1 - (1/(ratio_a + ratio_b))))
+        self.lambda_term2 = np.sqrt((1/(ratio_a + ratio_b)) * (1 - (ratio_a/(ratio_a + ratio_b))))
         self.lambda_minus = (self.lambda_term1 - self.lambda_term2)**2
         self.lambda_plus = (self.lambda_term1 + self.lambda_term2)**2
-        self._manova_ens = None
+        self._set_default_interval()
+        # when the support is finite (lambda_minus, lambda_plus) it is better
+        # to explicity approximate the inverse of the CDF to implement rvs
+        self._approximate_inv_cdf()
+    
+    def _set_default_interval(self):
+        interval = [self.lambda_minus, self.lambda_plus]
+        if self.ratio_a <= 1:
+            interval[0] = min(-0.05, self.lambda_minus)
+        if self.ratio_b <= 1:
+            interval[1] = max(self.lambda_plus, 1.05)
+        self.default_interval = tuple(interval)
+
+    def _approximate_inv_cdf(self):
+        # https://gist.github.com/amarvutha/c2a3ea9d42d238551c694480019a6ce1
+        x_vals = np.linspace(self.lambda_minus, self.lambda_plus, 1000)
+        _pdf = self._pdf(x_vals)
+        _cdf = np.cumsum(_pdf)      # approximating CDF
+        cdf_y = _cdf/_cdf.max()     # normalizing approximated CDF to 1.0
+        self._inv_cdf = interpolate.interp1d(cdf_y, x_vals)
+
+    def _rvs(self, size, random_state, _random_state=None):
+        if _random_state is not None:
+            np.random.seed(_random_state)
+
+        uniform_samples = np.random.random(size=size)
+        return self._inv_cdf(uniform_samples)
     
-    def rvs(self, size):
-        """Samples random variates following this distribution.
+    def __pdf_float(self, x):
+        if x <= self.lambda_minus:
+            return 0.0
 
-        Args:
-            size (int): sample size.
-        
-        Returns:
-            numpy array with the generated samples.
-        """
-        if size <= 0:
-            raise ValueError(f"Error: invalid sample size. It has to be positive. Provided size = {size}.")
-        
-        _n1 = int(np.round(size * self.a))
-        _n2 = int(np.round(size * self.b))
+        if x >= self.lambda_plus:
+            return 0.0
 
-        if not self._manova_ens:
-            self._manova_ens = ManovaEnsemble(beta=self.beta, m=size, n1=_n1, n2=_n2)
-        else:
-            self._manova_ens.set_size(m=size, n1=_n1, n2=_n2, resample_mtx=True)
+        return (self.ratio_a + self.ratio_b) * np.sqrt((self.lambda_plus - x) * (x - self.lambda_minus)) \
+                                / (2.0 * np.pi * x * (1-x))
 
-        # normalization here is not crucial since the default normalization const. of Manova is 1.0
-        if self.beta == 4:
-            return self._manova_ens.eigvals(normalize=True)[::2].real
-        return self._manova_ens.eigvals(normalize=True).real
-    
-    def pdf(self, x):
+    def _pdf(self, x):
         """Computes PDF of the Manova Spectrum distribution.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
         Returns:
             float or numpy array with the computed PDF in the given value(s).
         
         """
-        with np.errstate(divide='ignore', invalid='ignore'): 
-            return np.where(np.logical_and(x > self.lambda_minus, x < self.lambda_plus),
-                            (self.a + self.b) * np.sqrt((self.lambda_plus - x) * (x - self.lambda_minus)) \
-                                / (2.0 * np.pi * x * (1-x)),
-                            0.0)
+        # if x is array-like
+        if isinstance(x, (collections.abc.Sequence, np.ndarray)):
+            # TODO: Vectorize this loop in case x is array-like
+            y_ret = []
+            for val in x:
+                y_ret.append(self.__pdf_float(val))
+            return np.asarray(y_ret)
+        # if x is a number (int or float)
+        return self.__pdf_float(x)
     
-    def __cdf(self, x):
+    def __cdf_float(self, x):
         if x <= self.lambda_minus:
             return 0.0
 
         if x >= self.lambda_plus:
             return 1.0
 
         return quad(self.pdf, self.lambda_minus, x)[0]
 
-    def cdf(self, x):
+    def _cdf(self, x):
         """Computes CDF of the Manova Spectrum distribution.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the CDF.
         
         Returns:
             float or numpy array with the computed CDF in the given value(s).
         
         """
         # if x is array-like
         if isinstance(x, (collections.abc.Sequence, np.ndarray)):
+            # TODO: Vectorize this loop in case x is array-like
             y_ret = []
             for val in x:
-                y_ret.append(self.__cdf(val))
+                y_ret.append(self.__cdf_float(val))
             return np.asarray(y_ret)
         
         # if x is a number (int or float)
-        return self.__cdf(x)
+        return self.__cdf_float(x)
 
-    def plot_pdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_pdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the PDF of the Manova Spectrum distribution.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, a, and b.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
-        _plot_func(
-            interval, func=self.pdf, bins=bins, plot_title="Manova spectrum PDF",
+        plot_func(
+            interval, func=self._pdf, num_x_vals=num_x_vals, plot_title="Manova spectrum PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
 
-    def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
+    def plot_cdf(self, interval=None, num_x_vals=1000, savefig_path=None):
         """Plots the CDF of the Manova Spectrum distribution.
 
         Args:
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram. If not
                 provided, the used interval is calculated depending on beta, a, and b.
-            bins (int, default=100): It defines the number of equal-width bins within the
-                provided interval or range.
+            num_x_vals (int, default=100): It defines the number of evenly spaced x values
+                within the given interval or range in which the function (callable) is evaluated.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
 
-        _plot_func(
-            interval, func=self.cdf, bins=bins, plot_title="Manova spectrum CDF",
+        plot_func(
+            interval, func=self._cdf, num_x_vals=num_x_vals, plot_title="Manova spectrum CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
-    def plot_empirical_pdf(self, m_size=1000, n1_size=None, n2_size=None, bins=100, interval=None,
-                           density=False, plot_law_pdf=False, savefig_path=None):
+    def plot_empirical_pdf(self, sample_size=1000, bins=100, interval=None, density=False,
+                           plot_law_pdf=False, savefig_path=None, random_state=None):
         """Computes and plots Manova spectrum empirical pdf and analytical distribution.
 
         Calculates and plots Manova spectrum empirical pdf using Manova Ensemble random matrices.
         The size of the sampeld matrices will depend on the `m_size` (:math:`m`) parameter (no. of
         degrees of freedom) and on the ratios :math:`a` and :math:`b` given when instantiating this
         class, unless the parameters `n1_size` (:math:`n_1`) and/or `n2_size` (:math:`n_2`) are also
         given. In this last case, the new ratio :math:`a` for the empirical pdf plotting is computed
@@ -1104,91 +974,76 @@
                 is used instead to plot the empirical pdf.
             bins (int or sequence, default=100): If bins is an integer, it defines the number
                 of equal-width bins in the range. If bins is a sequence, it defines the
                 bin edges, including the left edge of the first bin and the right
                 edge of the last bin; in this case, bins may be unequally spaced.
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
+                If one of the bounds of the specified interval is outside of the minimum default
+                interval, this will be adjusted to show the distribution bulk properly.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
             plot_law_pdf (bool, default=False): If True, the limiting theoretical law is plotted.
                 If set to False, just the empirical histogram is shown. This parameter is only
                 considered when the argument 'density' is set also to True.
             savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown are the end of the routine.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         References:
             - Laszlo, L. and Farrel, B.
                 "Local Eigenvalue Density for General MANOVA Matrices".
                 Journal of Statistical Physics. 152.6 (2013): 1003-1032.
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
-        if m_size<1 or (n1_size is not None and n1_size<1) or (n2_size is not None and n2_size<1):
-            raise ValueError("matrix size must be positive")
-
-        if n1_size is None:
-            n1_size = round(self.a * m_size)
-        
-        if n2_size is None:
-            n2_size = round(self.b * m_size)
-
-        ens = ManovaEnsemble(beta=self.beta, m=m_size, n1=n1_size, n2=n2_size)
-
-        # computing approximated ratios since the n1_size and n2_size parameters
-        # could have been rounded previously
-        approx_a = n1_size/m_size
-        approx_b = n2_size/m_size
-        if approx_a <= 1 or approx_b <= 1:
-            print("Warning: sample size ('n1_size' or 'n2_size') too small compared "
-                  "to degrees of freedom ('m_size'). It may cause numerical instability.")
-        lambda_term1 = np.sqrt((approx_a/(approx_a+approx_b)) * (1 - (1/(approx_a+approx_b))))
-        lambda_term2 = np.sqrt((1/(approx_a+approx_b)) * (1 - (approx_a/(approx_a+approx_b))))
-        lambda_minus = (lambda_term1 - lambda_term2)**2
-        lambda_plus = (lambda_term1 + lambda_term2)**2
+        # pylint: disable=too-many-arguments
+        if sample_size<1:
+            raise ValueError("Negative eigenvalue sample size (given = {sample_size})."
+                             " Please, provide a sample size greater or equal than 1.")
 
         if interval is None:
-            interval = [lambda_minus, lambda_plus]
-            if approx_a <= 1:
-                interval[0] = min(-0.05, lambda_minus)
-            if approx_b <= 1:
-                interval[1] = max(lambda_plus, 1.05)
-            interval = tuple(interval)
-
-        observed, bins = ens.eigval_hist(
-            bins=bins,
-            interval=interval,
-            density=density,
-            normalize=True,
-            avoid_img=True
-        )
+            range_interval = self.default_interval
+        else:
+            xmin = min(interval[0], self.default_interval[0])
+            xmax = max(interval[1], self.default_interval[1])
+            if interval[0] > self.default_interval[0]:
+                print(f"Lower bound of interval too large. Setting lower bound to {xmin}.")
+            if interval[1] < self.default_interval[1]:
+                print(f"Upper bound of interval too large. Setting upper bound to {xmax}.")
+            range_interval = (xmin, xmax)
+            print(f"Setting plot interval to {range_interval}.")
+
+        random_samples = self._rvs(size=sample_size, random_state=random_state, _random_state=random_state)
+        observed, bin_edges = np.histogram(random_samples, bins=bins, range=range_interval, density=density)
 
-        width = bins[1]-bins[0]
-        plt.bar(bins[:-1], observed, width=width, align='edge')
+        width = bin_edges[1]-bin_edges[0]
+        plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
-            centers = np.array(_get_bins_centers_and_contour(bins))
+            centers = np.asarray(get_bins_centers_and_contour(bin_edges))
             # creating new instance with the approximated ratios depending on the given matrix sizes
-            msd = ManovaSpectrumDistribution(beta=self.beta, a=approx_a, b=approx_b)
-            pdf = msd.pdf(centers)
+            pdf = self._pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
         plt.title("Manova Spectrum - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
-        if approx_a <= 1 or approx_b <= 1:
+        if self.ratio_a <= 1 or self.ratio_b <= 1:
             if plot_law_pdf and density:
                 ylim_vals = pdf
             else:
                 ylim_vals = observed
             try:
                 plt.ylim(0, np.max(ylim_vals) + 0.25*np.max(ylim_vals))
             except ValueError:
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_base_ens.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_base_ens.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Testing _Ensemble abstract class
 '''
 
 import os
 import pytest
 import shutil
 
-from skrmt.ensemble._base_ensemble import _Ensemble
+from skrmt.ensemble.base_ensemble import _Ensemble
 from skrmt.ensemble.gaussian_ensemble import GaussianEnsemble
 
 
 TMP_DIR_PATH = os.path.join(os.getcwd(), "skrmt/ensemble/tests/tmp")
 
 
 @pytest.fixture(scope="module", autouse=True)
@@ -58,13 +58,13 @@
 
     goe.set_eigval_norm_const(0.1)
     assert goe.eigval_norm_const == 0.1
 
 
 
 def test_base_ens_plot():
-        '''Testing WignerSemicircleDistribution plot pdf
-        '''
-        fig_name = "test_base_ens_plot_eigval_hist.png"
-        goe = GaussianEnsemble(beta=1, n=100, use_tridiagonal=False)
-        goe.plot_eigval_hist(fig_path=TMP_DIR_PATH+"/"+fig_name)
-        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
+    """Testing plot eigval hist
+    """
+    fig_name = "test_base_ens_plot_eigval_hist.png"
+    goe = GaussianEnsemble(beta=1, n=100, use_tridiagonal=False)
+    goe.plot_eigval_hist(savefig_path=TMP_DIR_PATH+"/"+fig_name)
+    assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     assert coe.n == n1_size
     assert coe.matrix.shape == (n1_size,n1_size)
 
     coe.set_size(n2_size, resample_mtx=False)
     assert coe.n == n2_size
     assert coe.matrix.shape == (n1_size,n1_size)
 
-    coe.set_size(n2_size, resample_mtx=True)
+    coe.set_size(n2_size, resample_mtx=True, random_state=1)
     assert coe.n == n2_size
     assert coe.matrix.shape == (n2_size,n2_size)
 
 
 def test_coe_eigvals():
     '''Testing all eigenvalues of a COE matrix are real
     '''
@@ -118,15 +118,15 @@
     assert cue.n == n1_size
     assert cue.matrix.shape == (n1_size,n1_size)
 
     cue.set_size(n2_size, resample_mtx=False)
     assert cue.n == n2_size
     assert cue.matrix.shape == (n1_size,n1_size)
 
-    cue.set_size(n2_size, resample_mtx=True)
+    cue.set_size(n2_size, resample_mtx=True, random_state=1)
     assert cue.n == n2_size
     assert cue.matrix.shape == (n2_size,n2_size)
 
 
 def test_cue_eigvals():
     '''Testing all eigenvalues of a CUE matrix have module 1
     '''
@@ -189,15 +189,15 @@
     assert cse.n == n1_size
     assert cse.matrix.shape == (2*n1_size,2*n1_size)
 
     cse.set_size(n2_size, resample_mtx=False)
     assert cse.n == n2_size
     assert cse.matrix.shape == (2*n1_size,2*n1_size)
 
-    cse.set_size(n2_size, resample_mtx=True)
+    cse.set_size(n2_size, resample_mtx=True, random_state=1)
     assert cse.n == n2_size
     assert cse.matrix.shape == (2*n2_size,2*n2_size)
 
 
 def test_beta4_joint_eigval_pdf():
     '''Testing joint eigenvalue pdf
     '''
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     assert goe.n == n1_size
     assert goe.matrix.shape == (n1_size,n1_size)
 
     goe.set_size(n2_size, resample_mtx=False)
     assert goe.n == n2_size
     assert goe.matrix.shape == (n1_size,n1_size)
 
-    goe.set_size(n2_size, resample_mtx=True)
+    goe.set_size(n2_size, resample_mtx=True, random_state=1)
     assert goe.n == n2_size
     assert goe.matrix.shape == (n2_size,n2_size)
 
 
 def test_goe_build_tridiagonal():
     '''Testing tridiagonal form of GSE
     '''
@@ -198,15 +198,15 @@
     assert gue.n == n1_size
     assert gue.matrix.shape == (n1_size,n1_size)
 
     gue.set_size(n2_size, resample_mtx=False)
     assert gue.n == n2_size
     assert gue.matrix.shape == (n1_size,n1_size)
 
-    gue.set_size(n2_size, resample_mtx=True)
+    gue.set_size(n2_size, resample_mtx=True, random_state=1)
     assert gue.n == n2_size
     assert gue.matrix.shape == (n2_size,n2_size)
 
 
 def test_gue_build_tridiagonal():
     '''Testing tridiagonal form of GUE
     '''
@@ -303,15 +303,15 @@
     assert gse.n == n1_size
     assert gse.matrix.shape == (2*n1_size,2*n1_size)
 
     gse.set_size(n2_size, resample_mtx=False)
     assert gse.n == n2_size
     assert gse.matrix.shape == (2*n1_size,2*n1_size)
 
-    gse.set_size(n2_size, resample_mtx=True)
+    gse.set_size(n2_size, resample_mtx=True, random_state=1)
     assert gse.n == n2_size
     assert gse.matrix.shape == (2*n2_size,2*n2_size)
 
 
 def test_gse_build_tridiagonal():
     '''Testing tridiagonal form of GSE
     '''
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     mre.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=False)
     assert mre.m == m2_size
     assert mre.n1 == n21_size
     assert mre.n2 == n22_size
     assert mre.matrix.shape == (m1_size,m1_size)
 
-    mre.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True)
+    mre.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True, random_state=1)
     assert mre.m == m2_size
     assert mre.n1 == n21_size
     assert mre.n2 == n22_size
     assert mre.matrix.shape == (m2_size,m2_size)
 
 
 def test_beta1_joint_eigval_pdf():
@@ -104,15 +104,15 @@
 
     mce.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=False)
     assert mce.m == m2_size
     assert mce.n1 == n21_size
     assert mce.n2 == n22_size
     assert mce.matrix.shape == (m1_size,m1_size)
 
-    mce.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True)
+    mce.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True, random_state=1)
     assert mce.m == m2_size
     assert mce.n1 == n21_size
     assert mce.n2 == n22_size
     assert mce.matrix.shape == (m2_size,m2_size)
 
 
 ##########################################
@@ -156,12 +156,12 @@
 
     mqe.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=False)
     assert mqe.m == m2_size
     assert mqe.n1 == n21_size
     assert mqe.n2 == n22_size
     assert mqe.matrix.shape == (2*m1_size,2*m1_size)
 
-    mqe.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True)
+    mqe.set_size(m=m2_size, n1=n21_size, n2=n22_size, resample_mtx=True, random_state=1)
     assert mqe.m == m2_size
     assert mqe.n1 == n21_size
     assert mqe.n2 == n22_size
     assert mqe.matrix.shape == (2*m2_size,2*m2_size)
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_spectral_law.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_spectral_law.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import shutil
 import numpy as np
 
 from skrmt.ensemble import WignerSemicircleDistribution
 from skrmt.ensemble import MarchenkoPasturDistribution
 from skrmt.ensemble import TracyWidomDistribution
 from skrmt.ensemble import ManovaSpectrumDistribution
-from skrmt.ensemble.spectral_law import _indicator
+from skrmt.ensemble.misc import indicator
 
 
 TMP_DIR_PATH = os.path.join(os.getcwd(), "skrmt/ensemble/tests/tmp")
 
 
 @pytest.fixture(scope="module", autouse=True)
 def _setup_tmp_dir(request):
@@ -77,24 +77,24 @@
         beta = 4
         size = 5
         wsd4 = WignerSemicircleDistribution(beta=beta)
         samples = wsd4.rvs(size=size)
         assert len(samples == size)
 
         size = 10
-        samples = wsd4.rvs(size=size)
+        samples = wsd4.rvs(size=size, random_state=1)
         assert len(samples == size)
     
     def test_wsd_rvs_raise(self):
         '''Testing WignerSemicircleDistribution random variates (sampling)
         raising an exception because of invalid argument
         '''
         with pytest.raises(ValueError):
             wsd = WignerSemicircleDistribution(beta=1)
-            wsd.rvs(-5)
+            wsd.rvs(size=-5)
     
     def test_wsd_pdf(self):
         '''Testing WignerSemicircleDistribution pdf
         '''
         beta = 4
         sigma = 2
         center = 0
@@ -163,122 +163,135 @@
             wsd = WignerSemicircleDistribution(beta=1)
             wsd.plot_pdf(interval=1)
 
     def test_wsd_plot_goe_abs_freq(self):
         fig_name = "test_wsl_goe_absfreq.png"
         wsd = WignerSemicircleDistribution(beta=1)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gue_abs_freq(self):
         fig_name = "test_wsl_gue_absfreq.png"
         wsd = WignerSemicircleDistribution(beta=2)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gse_abs_freq(self):
         fig_name = "test_wsl_gse_absfreq.png"
         wsd = WignerSemicircleDistribution(beta=4)
         wsd.plot_empirical_pdf(
-            n_size=50,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_goe_normalized(self):
         fig_name = "test_wsl_goe_norm.png"
         wsd = WignerSemicircleDistribution(beta=1)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gue_normalized(self):
         fig_name = "test_wsl_gue_norm.png"
         wsd = WignerSemicircleDistribution(beta=2)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gse_normalized(self):
         fig_name = "test_wsl_gse_norm.png"
         wsd = WignerSemicircleDistribution(beta=4)
         wsd.plot_empirical_pdf(
-            n_size=50,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_goe_theoretical(self):
         fig_name = "test_wsl_goe_theory.png"
         wsd = WignerSemicircleDistribution(beta=1)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gue_theoretical(self):
         fig_name = "test_wsl_gue_theory.png"
         wsd = WignerSemicircleDistribution(beta=2)
         wsd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_wsd_plot_gse_theoretical(self):
         fig_name = "test_wsl_gse_theory.png"
         wsd = WignerSemicircleDistribution(beta=4)
         wsd.plot_empirical_pdf(
-            n_size=50,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
+    def test_wsd_plot_tiny_interval_adjusted(self):
+        fig_name = "test_wsl_tiny_interval_adjusted.png"
+        wsd = WignerSemicircleDistribution(beta=1)
+        wsd.plot_empirical_pdf(
+            sample_size=10,
+            bins=10,
+            interval=(-0.1, 0.1),
+            density=True,
+            plot_law_pdf=False,
+            savefig_path=TMP_DIR_PATH+"/"+fig_name
+        )
+        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
+    
     def test_wsd_plot_size_exception(self):
         with pytest.raises(ValueError):
             wsd = WignerSemicircleDistribution(beta=1)
-            wsd.plot_empirical_pdf(n_size=0)
+            wsd.plot_empirical_pdf(sample_size=0)
     
     def test_wsd_plot_ensemble_exception(self):
         with pytest.raises(ValueError):
             wsd = WignerSemicircleDistribution(beta=0)
             wsd.plot_empirical_pdf()
     
 
@@ -296,15 +309,14 @@
 
         assert mpd.beta == beta
         assert mpd.ratio == ratio
         assert mpd.sigma == sigma
         assert mpd.lambda_minus == beta * sigma**2 * (1 - np.sqrt(ratio))**2
         assert mpd.lambda_plus == beta * sigma**2 * (1 + np.sqrt(ratio))**2
         assert mpd._var == beta * sigma**2
-        assert mpd._wishart_ens is None
     
     def test_mpd_init_raise(self):
         '''Testing MarchenkoPasturDistribution init raising exception
         '''
         with pytest.raises(ValueError):
             _ = MarchenkoPasturDistribution(ratio=1, beta=3)
         
@@ -325,24 +337,24 @@
         ratio = 1/3
         size = 5
         mpd4 = MarchenkoPasturDistribution(beta=beta, ratio=ratio)
         samples = mpd4.rvs(size=size)
         assert len(samples == size)
 
         size = 10
-        samples = mpd4.rvs(size=size)
+        samples = mpd4.rvs(size=size, random_state=1)
         assert len(samples == size)
     
     def test_mpd_rvs_raise(self):
         '''Testing MarchenkoPasturDistribution random variates (sampling) raising
         an exception because of an invalid argument
         '''
         with pytest.raises(ValueError):
             mpd = MarchenkoPasturDistribution(beta=1, ratio=1)
-            mpd.rvs(-5)
+            mpd.rvs(size=-5)
     
     def test_mpd_pdf(self):
         '''Testing MarchenkoPasturDistribution pdf
         '''
         beta = 4
         ratio = 1/3
         sigma = 1
@@ -409,222 +421,237 @@
         mpd.plot_cdf(interval=(-1,10), savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mpd_plot_wre_abs_freq(self):
         fig_name = "test_mpl_wre_absfreq.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mpd_plot_wce_abs_freq(self):
         fig_name = "test_mpl_wce_absfreq.png"
         mpd = MarchenkoPasturDistribution(beta=2, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wqe_abs_freq(self):
         fig_name = "test_mpl_wqe_absfreq.png"
         mpd = MarchenkoPasturDistribution(beta=4, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_normalized(self):
         fig_name = "test_mpl_wre_norm.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mpd_plot_wce_normalized(self):
         fig_name = "test_mpl_wce_norm.png"
         mpd = MarchenkoPasturDistribution(beta=2, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wqe_normalized(self):
         fig_name = "test_mpl_wqe_norm.png"
         mpd = MarchenkoPasturDistribution(beta=4, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_theoretical(self):
         fig_name = "test_mpl_wre_theory.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_mpd_plot_wce_theoretical(self):
         fig_name = "test_mpl_wce_theory.png"
         mpd = MarchenkoPasturDistribution(beta=2, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wqe_theoretical(self):
         fig_name = "test_mpl_wqe_theory.png"
         mpd = MarchenkoPasturDistribution(beta=4, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_ratio_ge1(self):
         fig_name = "test_mpl_wre_ratio_ge1.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_theoretical_ratio_ge1(self):
         fig_name = "test_mpl_wre_theory_ratio_ge1.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_interval(self):
         fig_name = "test_mpl_wre_interval.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            n_size=100,
-            bins=100,
-            interval=(0,10),
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
-    def test_mpd_plot_wre_emppdf_p_size(self):
-        fig_name = "test_mpd_wre_emppdf_p_size.png"
+    def test_mpd_plot_wre_emppdf_sample_size(self):
+        fig_name = "test_mpd_wre_emppdf_sample_size.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
         mpd.plot_empirical_pdf(
-            p_size=50,
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
-    def test_mpd_plot_wce_emppdf_p_size(self):
-        fig_name = "test_mpd_wce_emppdf_p_size.png"
+    def test_mpd_plot_wce_emppdf_sample_size(self):
+        fig_name = "test_mpd_wce_emppdf_sample_size.png"
         mpd = MarchenkoPasturDistribution(beta=2, ratio=1/3)
         mpd.plot_empirical_pdf(
-            p_size=50,
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
-    def test_mpd_plot_wqe_emppdf_p_size(self):
-        fig_name = "test_mpd_wqe_emppdf_p_size.png"
+    def test_mpd_plot_wqe_emppdf_sample_size(self):
+        fig_name = "test_mpd_wqe_emppdf_sample_size.png"
         mpd = MarchenkoPasturDistribution(beta=4, ratio=1/3)
         mpd.plot_empirical_pdf(
-            p_size=50,
-            n_size=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_emppdf_ratio_g_1(self):
         fig_name = "test_mpd_plot_wre_emppdf_ratio_g_1.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=2)
         mpd.plot_empirical_pdf(
-            n_size=50,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_mpd_plot_wre_emppdf_ratio_g_1_density(self):
         fig_name = "test_mpd_plot_wre_emppdf_ratio_g_1_density.png"
         mpd = MarchenkoPasturDistribution(beta=1, ratio=2)
         mpd.plot_empirical_pdf(
-            n_size=50,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
+    def test_mpd_plot_tiny_interval_adjusted(self):
+        fig_name = "test_mpd_plot_tiny_interval_adjusted.png"
+        mpd = MarchenkoPasturDistribution(beta=1, ratio=1/2)
+        mpd.plot_empirical_pdf(
+            sample_size=10,
+            bins=10,
+            interval=(mpd.lambda_minus+0.1, mpd.lambda_minus-0.1),
+            density=True,
+            plot_law_pdf=False,
+            savefig_path=TMP_DIR_PATH+"/"+fig_name
+        )
+        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
+    
     def test_mpd_plot_mpl_size_exception(self):
         with pytest.raises(ValueError):
             mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
-            mpd.plot_empirical_pdf(n_size=0)
+            mpd.plot_empirical_pdf(sample_size=0)
     
     def test_mpd_plot_mpl_ensemble_exception(self):
         with pytest.raises(ValueError):
             mpd = MarchenkoPasturDistribution(beta=0, ratio=1/3)
             mpd.plot_empirical_pdf()
 
 
@@ -659,28 +686,24 @@
         beta = 4
         size = 5
         twd4 = TracyWidomDistribution(beta=beta)
         samples = twd4.rvs(size=size)
         assert len(samples == size)
 
         size = 10
-        samples = twd4.rvs(size=size)
+        samples = twd4.rvs(size=size, random_state=1)
         assert len(samples == size)
     
     def test_twd_rvs_raise(self):
         '''Testing TracyWidomDistribution random variates (sampling) raising
         an exception because of an invalid argument
         '''
         with pytest.raises(ValueError):
             twd = TracyWidomDistribution(beta=1)
-            twd.rvs(-5)
-
-        with pytest.raises(ValueError):
-            twd = TracyWidomDistribution(beta=1)
-            twd.rvs(size=5, mtx_size=0)
+            twd.rvs(size=-5)
     
     def test_twd_pdf(self):
         '''Testing TracyWidomDistribution pdf
         '''
         beta = 4
         twd = TracyWidomDistribution(beta=beta)
         assert twd.pdf(-1) > 0.0
@@ -722,493 +745,471 @@
         twd.plot_cdf(interval=(-5,5), savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_goe_abs_freq(self):
         fig_name = "test_twl_goe_abs_freq.png"
         twd = TracyWidomDistribution(beta=1)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gue_abs_freq(self):
         fig_name = "test_twl_gue_abs_freq.png"
         twd = TracyWidomDistribution(beta=2)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gse_abs_freq(self):
         fig_name = "test_twl_gse_abs_freq.png"
         twd = TracyWidomDistribution(beta=4)
         twd.plot_empirical_pdf(
-            n_size=25,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_goe_normalized(self):
         fig_name = "test_twl_goe_normalized.png"
         twd = TracyWidomDistribution(beta=1)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gue_normalized(self):
         fig_name = "test_twl_gue_normalized.png"
         twd = TracyWidomDistribution(beta=2)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gse_normalized(self):
         fig_name = "test_twl_gse_normalized.png"
         twd = TracyWidomDistribution(beta=4)
         twd.plot_empirical_pdf(
-            n_size=25,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_goe_theoretical(self):
         fig_name = "test_twl_goe_theory.png"
         twd = TracyWidomDistribution(beta=1)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gue_theoretical(self):
         fig_name = "test_twl_gue_theory.png"
         twd = TracyWidomDistribution(beta=2)
         twd.plot_empirical_pdf(
-            n_size=50,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_twd_plot_gse_theoretical(self):
         fig_name = "test_twl_gse_theory.png"
         twd = TracyWidomDistribution(beta=4)
         twd.plot_empirical_pdf(
-            n_size=25,
-            times=100,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
+    def test_twd_plot_tiny_interval_adjusted(self):
+        fig_name = "test_twd_plot_tiny_interval_adjusted.png"
+        mpd = TracyWidomDistribution(beta=1)
+        mpd.plot_empirical_pdf(
+            sample_size=10,
+            bins=10,
+            interval=(-0.2, -0.1),
+            density=True,
+            plot_law_pdf=False,
+            savefig_path=TMP_DIR_PATH+"/"+fig_name
+        )
+        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
+    
     def test_twd_plot_size_exception(self):
         with pytest.raises(ValueError):
             twd = TracyWidomDistribution(beta=1)
-            twd.plot_empirical_pdf(n_size=0)
+            twd.plot_empirical_pdf(sample_size=0)
     
     def test_twd_plot_ensemble_exception(self):
         with pytest.raises(ValueError):
             twd = TracyWidomDistribution(beta=0)
-            twd.plot_empirical_pdf(n_size=10)
+            twd.plot_empirical_pdf(sample_size=10)
 
 
 
 class TestManovaSpectrumDistribution:
 
     def test_msd_init_success(self):
         '''Testing ManovaSpectrumDistribution init
         '''
         beta = 4
         a = 3
         b = 3
 
-        msd = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        msd = ManovaSpectrumDistribution(beta=beta, ratio_a=a, ratio_b=b)
 
         assert msd.beta == beta
-        assert msd.a == a
-        assert msd.b == b
+        assert msd.ratio_a == a
+        assert msd.ratio_b == b
 
         assert msd.lambda_term1 == np.sqrt((a/(a+b)) * (1 - (1/(a+b))))
         assert msd.lambda_term2 == np.sqrt((1/(a+b)) * (1 - (a/(a+b))))
         assert msd.lambda_minus == (msd.lambda_term1 - msd.lambda_term2)**2
         assert msd.lambda_plus == (msd.lambda_term1 + msd.lambda_term2)**2
-        assert msd._manova_ens is None
     
     def test_msd_init_raise(self):
         '''Testing ManovaSpectrumDistribution init raising exception
         '''
         with pytest.raises(ValueError):
-            _ = ManovaSpectrumDistribution(a=1, b=1, beta=3)
+            _ = ManovaSpectrumDistribution(ratio_a=1, ratio_b=1, beta=3)
         
         with pytest.raises(ValueError):
-            _ = ManovaSpectrumDistribution(a=0, b=0, beta=1)
+            _ = ManovaSpectrumDistribution(ratio_a=0, ratio_b=0, beta=1)
 
     def test_msd_rvs_success(self):
         '''Testing ManovaSpectrumDistribution random variates (sampling)
         '''
         beta = 1
         a = b = 3
         size = 5
-        msd1 = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        msd1 = ManovaSpectrumDistribution(beta=beta, ratio_a=a, ratio_b=b)
         samples = msd1.rvs(size=size)
         assert len(samples == size)
 
         beta = 4
         a = b = 3
         size = 5
-        msd4 = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        msd4 = ManovaSpectrumDistribution(beta=beta, ratio_a=a, ratio_b=b)
         samples = msd4.rvs(size=size)
         assert len(samples == size)
 
         size = 10
-        samples = msd4.rvs(size=size)
+        samples = msd4.rvs(size=size, random_state=1)
         assert len(samples == size)
     
     def test_msd_rvs_raise(self):
         '''Testing ManovaSpectrumDistribution random variates (sampling) raising an
         exception because of an invalid argument
         '''
         with pytest.raises(ValueError):
-            msd = ManovaSpectrumDistribution(beta=1, a=1, b=1)
-            msd.rvs(-5)
+            msd = ManovaSpectrumDistribution(beta=1, ratio_a=1, ratio_b=1)
+            msd.rvs(size=-5)
     
     def test_msd_pdf(self):
         '''Testing ManovaSpectrumDistribution pdf
         '''
         beta = 4
         a = b = 2
-        msd = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        msd = ManovaSpectrumDistribution(beta=beta, ratio_a=a, ratio_b=b)
 
         middle = np.mean([msd.lambda_minus, msd.lambda_plus])
         assert msd.pdf(middle) > 0.0
         assert msd.pdf(msd.lambda_plus + 0.1) == 0.0
         assert msd.pdf(msd.lambda_minus - 0.01) == 0.0
     
     def test_msd_cdf(self):
         '''Testing ManovaSpectrumDistribution cdf
         '''
         beta = 4
         a = b = 2
-        msd = ManovaSpectrumDistribution(beta=beta, a=a, b=b)
+        msd = ManovaSpectrumDistribution(beta=beta, ratio_a=a, ratio_b=b)
 
         middle = np.mean([msd.lambda_minus, msd.lambda_plus])
         assert msd.cdf(middle) > 0.0
         assert msd.cdf(msd.lambda_plus + 0.1) == 1.0
         assert msd.cdf(msd.lambda_minus - 0.01) == 0.0
     
     def test_msd_plot_pdf(self):
         '''Testing ManovaSpectrumDistribution plot pdf
         '''
         fig_name = "test_msd_pdf_wo_interval.png"
-        msd = ManovaSpectrumDistribution(a=3, b=3)
+        msd = ManovaSpectrumDistribution(ratio_a=3, ratio_b=3)
         msd.plot_pdf(savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
         fig_name = "test_msd_pdf_w_interval.png"
-        msd = ManovaSpectrumDistribution(a=3, b=3)
+        msd = ManovaSpectrumDistribution(ratio_a=3, ratio_b=3)
         msd.plot_pdf(interval=(-1,2), savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_cdf(self):
         '''Testing ManovaSpectrumDistribution plot cdf
         '''
         fig_name = "test_msd_cdf_wo_interval.png"
-        msd = ManovaSpectrumDistribution(a=3, b=3)
+        msd = ManovaSpectrumDistribution(ratio_a=3, ratio_b=3)
         msd.plot_cdf(savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
         fig_name = "test_msd_cdf_w_interval.png"
-        msd = ManovaSpectrumDistribution(a=3, b=3)
+        msd = ManovaSpectrumDistribution(ratio_a=3, ratio_b=3)
         msd.plot_cdf(interval=(-1,2), savefig_path=TMP_DIR_PATH+"/"+fig_name)
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_abs_freq(self):
         fig_name = "test_msd_mre_absfreq.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_msd_plot_mce_abs_freq(self):
         fig_name = "test_msd_mce_absfreq.png"
-        msd = ManovaSpectrumDistribution(beta=2, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=2, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mqe_abs_freq(self):
         fig_name = "test_msd_mqe_absfreq.png"
-        msd = ManovaSpectrumDistribution(beta=4, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=4, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_normalized(self):
         fig_name = "test_msd_mre_norm.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1,ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_msd_plot_mce_normalized(self):
         fig_name = "test_msd_mce_norm.png"
-        msd = ManovaSpectrumDistribution(beta=2, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=2, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mqe_normalized(self):
         fig_name = "test_msd_mqe_norm.png"
-        msd = ManovaSpectrumDistribution(beta=4, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=4, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
+            savefig_path=TMP_DIR_PATH+"/"+fig_name,
+            random_state=1,
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_theoretical(self):
         fig_name = "test_msd_mre_theory.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
     def test_msd_plot_mce_theoretical(self):
         fig_name = "test_msd_mce_theory.png"
-        msd = ManovaSpectrumDistribution(beta=2, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=2, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mqe_theoretical(self):
         fig_name = "test_msd_mqe_theory.png"
-        msd = ManovaSpectrumDistribution(beta=4, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=4, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=40,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_ratio_ge1(self):
         fig_name = "test_msd_mre_ratio_ge1.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=200,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_msd_mre_theoretical_ratio_ge1(self):
         fig_name = "test_msd_wre_theory_ratio_ge1.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=1000,
-            bins=100,
+            sample_size=10,
+            bins=10,
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_interval(self):
         fig_name = "test_msd_mre_interval.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
         msd.plot_empirical_pdf(
-            m_size=200,
-            bins=100,
+            sample_size=10,
+            bins=10,
             interval=(0,10),
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_a_le_1_b_le_1(self):
         fig_name = "test_msd_plot_mre_a_le_1_b_le_1.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=0.9, b=0.9)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=0.9, ratio_b=0.9)
         msd.plot_empirical_pdf(
-            m_size=200,
-            bins=100,
+            sample_size=10,
+            bins=10,
             interval=(0,10),
             density=False,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
     
     def test_msd_plot_mre_a_le_1_b_le_1_density(self):
         fig_name = "test_msd_plot_mre_a_le_1_b_le_1_density.png"
-        msd = ManovaSpectrumDistribution(beta=1, a=0.9, b=0.9)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=0.9, ratio_b=0.9)
         msd.plot_empirical_pdf(
-            m_size=200,
-            bins=100,
+            sample_size=10,
+            bins=10,
             interval=(0,10),
             density=True,
             plot_law_pdf=True,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
 
-    
-    def test_msd_plot_mre_emppdf_n1_size(self):
-        fig_name = "test_msd_mre_emppdf_n1_size.png"
-        mpd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
-        mpd.plot_empirical_pdf(
-            m_size=200,
-            n1_size=500,
-            bins=100,
-            interval=(0,10),
-            density=False,
-            plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
-        )
-        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
-    
-    def test_msd_plot_mre_emppdf_n2_size(self):
-        fig_name = "test_msd_mre_emppdf_n2_size.png"
-        mpd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
-        mpd.plot_empirical_pdf(
-            m_size=200,
-            n2_size=500,
-            bins=100,
-            interval=(0,10),
-            density=False,
-            plot_law_pdf=False,
-            savefig_path=TMP_DIR_PATH+"/"+fig_name
-        )
-        assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
-    
-    def test_msd_plot_mre_emppdf_n1n2_size(self):
-        fig_name = "test_msd_mre_emppdf_n1n2_size.png"
-        mpd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
+    def test_msd_plot_tiny_interval_adjusted(self):
+        fig_name = "test_msd_plot_tiny_interval_adjusted.png"
+        mpd = ManovaSpectrumDistribution(beta=1, ratio_a=2, ratio_b=2)
         mpd.plot_empirical_pdf(
-            m_size=200,
-            n1_size=500,
-            n2_size=600,
-            bins=100,
-            interval=(0,10),
-            density=False,
+            sample_size=10,
+            bins=10,
+            interval=(mpd.lambda_minus+0.1, mpd.lambda_minus-0.1),
+            density=True,
             plot_law_pdf=False,
             savefig_path=TMP_DIR_PATH+"/"+fig_name
         )
         assert os.path.isfile(os.path.join(TMP_DIR_PATH, fig_name)) == True
-    
+
     def test_msd_plot_size_exception(self):
         with pytest.raises(ValueError):
-            msd = ManovaSpectrumDistribution(beta=1, a=3, b=3)
-            msd.plot_empirical_pdf(m_size=0)
+            msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
+            msd.plot_empirical_pdf(sample_size=0)
     
     def test_msd_plot_ensemble_exception(self):
         with pytest.raises(ValueError):
-            msd = ManovaSpectrumDistribution(beta=0, a=3, b=3)
-            msd.plot_empirical_pdf(m_size=10)
+            msd = ManovaSpectrumDistribution(beta=0, ratio_a=3, ratio_b=3)
+            msd.plot_empirical_pdf(sample_size=10)
 
 
 
 def test_indicator_func():
     '''Testing indicator function
     '''
-    assert _indicator(1.0, start=1.0, stop=2.0, inclusive="both") == 1.0
-    assert _indicator(1.0, start=1.0, stop=2.0, inclusive="left") == 1.0
-    assert _indicator(1.0, start=1.0, stop=2.0, inclusive="right") == 0.0
-    assert _indicator(1.0, start=1.0, stop=2.0, inclusive="neither") == 0.0
-    assert _indicator(2.0, start=1.0, stop=2.0, inclusive="both") == 1.0
-    assert _indicator(2.0, start=1.0, stop=2.0, inclusive="left") == 0.0
-    assert _indicator(2.0, start=1.0, stop=2.0, inclusive="right") == 1.0
-    assert _indicator(2.0, start=1.0, stop=2.0, inclusive="neither") == 0.0
-    assert _indicator(2.0, stop=2.0, inclusive="both") == 1.0
-    assert _indicator(2.0, stop=2.0, inclusive="left") == 0.0
-    assert _indicator(2.0, stop=2.0, inclusive="right") == 1.0
-    assert _indicator(2.0, stop=2.0, inclusive="neither") == 0.0
+    assert indicator(1.0, start=1.0, stop=2.0, inclusive="both") == 1.0
+    assert indicator(1.0, start=1.0, stop=2.0, inclusive="left") == 1.0
+    assert indicator(1.0, start=1.0, stop=2.0, inclusive="right") == 0.0
+    assert indicator(1.0, start=1.0, stop=2.0, inclusive="neither") == 0.0
+    assert indicator(2.0, start=1.0, stop=2.0, inclusive="both") == 1.0
+    assert indicator(2.0, start=1.0, stop=2.0, inclusive="left") == 0.0
+    assert indicator(2.0, start=1.0, stop=2.0, inclusive="right") == 1.0
+    assert indicator(2.0, start=1.0, stop=2.0, inclusive="neither") == 0.0
+    assert indicator(2.0, stop=2.0, inclusive="both") == 1.0
+    assert indicator(2.0, stop=2.0, inclusive="left") == 0.0
+    assert indicator(2.0, stop=2.0, inclusive="right") == 1.0
+    assert indicator(2.0, stop=2.0, inclusive="neither") == 0.0
 
 def test_indicator_func_except():
     '''Testing indicator function raising exception
     '''
     with pytest.raises(ValueError):
-        _ = _indicator(2.0)
+        _ = indicator(2.0)
     
     with pytest.raises(ValueError):
-        _ = _indicator(2.0, start=2.0, inclusive="foo")
+        _ = indicator(2.0, start=2.0, inclusive="foo")
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     assert ens.matrix.shape == (p1_size,p1_size)
 
     ens.set_size(p=p2_size, n=n2_size, resample_mtx=False)
     assert ens.p == p2_size
     assert ens.n == n2_size
     assert ens.matrix.shape == (p1_size,p1_size)
 
-    ens.set_size(p=p2_size, n=n2_size, resample_mtx=True)
+    ens.set_size(p=p2_size, n=n2_size, resample_mtx=True, random_state=1)
     assert ens.p == p2_size
     assert ens.n == n2_size
     assert ens.matrix.shape == (p2_size,p2_size)
 
 
 def test_wre_build_tridiagonal():
     '''Testing tridiagonal form of WRE
@@ -223,15 +223,15 @@
     assert ens.matrix.shape == (p1_size,p1_size)
 
     ens.set_size(p=p2_size, n=n2_size, resample_mtx=False)
     assert ens.p == p2_size
     assert ens.n == n2_size
     assert ens.matrix.shape == (p1_size,p1_size)
 
-    ens.set_size(p=p2_size, n=n2_size, resample_mtx=True)
+    ens.set_size(p=p2_size, n=n2_size, resample_mtx=True, random_state=1)
     assert ens.p == p2_size
     assert ens.n == n2_size
     assert ens.matrix.shape == (p2_size,p2_size)
 
 
 def test_wce_build_tridiagonal():
     '''Testing tridiagonal form of WCE
@@ -351,15 +351,15 @@
     assert ens.matrix.shape == (2*p_size1,2*p_size1)
 
     ens.set_size(p=p_size2, n=n_size2, resample_mtx=False)
     assert ens.p == p_size2
     assert ens.n == n_size2
     assert ens.matrix.shape == (2*p_size1,2*p_size1)
 
-    ens.set_size(p=p_size2, n=n_size2, resample_mtx=True)
+    ens.set_size(p=p_size2, n=n_size2, resample_mtx=True, random_state=1)
     assert ens.p == p_size2
     assert ens.n == n_size2
     assert ens.matrix.shape == (2*p_size2,2*p_size2)
 
 
 def test_wqe_build_tridiagonal():
     '''Testing tridiagonal form of WQE
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.8.0/skrmt/ensemble/tridiagonal_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
     Returns:
         (tuple) tuple containing:
             observed (array): List of eigenvalues frequencies per bin. If density is
             True these values are the relative frequencies in order to get an area under
             the histogram equal to 1. Otherwise, this list contains the absolute
             frequencies of the eigenvalues.
-            bins (array): The edges of the bins. Length nbins + 1 (nbins left edges and
-            right edge of last bin)
+            bin_delimiters (array): The edges of the bins. Length nbins + 1 (nbins left edges
+            and right edge of last bin)
     """
     if not isinstance(interval, tuple):
         raise ValueError("interval argument must be a tuple")
 
     if isinstance(bins, int):
         # calculating bin delimiters
         bin_delimiters = np.linspace(interval[0], interval[1], num=bins+1) # O(m)
```

### Comparing `scikit-rmt-0.7.1/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.8.0/skrmt/ensemble/wishart_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy import sparse, special
 
-from ._base_ensemble import _Ensemble
+from .base_ensemble import _Ensemble
 from .tridiagonal_utils import tridiag_eigval_hist
 
 
 #########################################################################
 ### Wishart Ensemble = Laguerre Ensemble
 
 class WishartEnsemble(_Ensemble):
@@ -63,15 +63,15 @@
             Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
         - Bar, Z.D. and Silverstain, J.W.
             Spectral Analysis of Large Dimensional Random Matrices.
             2nd edition. Springer. (2010).
 
     """
 
-    def __init__(self, beta, p, n, use_tridiagonal=False, sigma=1.0):
+    def __init__(self, beta, p, n, use_tridiagonal=False, sigma=1.0, random_state=None):
         """Constructor for WishartEnsemble class.
 
         Initializes an instance of this class with the given parameters.
 
         Args:
             beta (int): descriptive integer of the Wishart ensemble type.
                 For Real beta=1, for Complex beta=2, for Quaternion beta=4
@@ -80,76 +80,91 @@
             n (int): number of columns of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             use_tridiagonal (bool, default=False): if set to True, Wishart Ensemble
                 matrices are sampled in its tridiagonal form, which has the same
                 eigenvalues than its standard form.
             sigma (float, 1.0): scale (standard deviation) of the random entries of the
                 sampled matrix.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy before sampling the random matrix instance. This 
+                has to be any integer between 0 and 2**32 - 1 (inclusive), or None (default).
+                If None, the seed is obtained from the clock.
 
         """
         if beta not in [1,2,4]:
             raise ValueError(f"Invalid beta: {beta}. Beta value has to be 1, 2 or 4.")
 
         super().__init__()
         # pylint: disable=invalid-name
         self.p = p
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
         self._eigvals = None
-        self.matrix = self.sample()
+        self.matrix = self.sample(random_state=random_state)
         # default eigenvalue normalization constant
         self.eigval_norm_const = 1/self.n
         self._compute_parameters()
 
     def _compute_parameters(self):
         # calculating constants depending on matrix sizes
         self.ratio = self.p/self.n
         self.lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(self.ratio))**2
         self.lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(self.ratio))**2
 
-    def set_size(self, p, n, resample_mtx=True):
+    def set_size(self, p, n, resample_mtx=True, random_state: int = None):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
         Args:
             p (int): number of rows of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             n (int): number of columns of the guassian matrix that generates
                 the matrix of the corresponding ensemble.
             resample_mtx (bool, default=True): If set to True, the ensemble matrix is
                 resampled with the new dimensions.
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
 
         """
         self.p = p
         self.n = n
         self._compute_parameters()
         if resample_mtx:
-            self.matrix = self.sample()
+            self.matrix = self.sample(random_state=random_state)
 
     # pylint: disable=inconsistent-return-statements
-    def sample(self):
+    def sample(self, random_state: int = None):
         """Samples new Wishart Ensemble random matrix.
 
         The sampling algorithm depends on the specification of
         use_tridiagonal parameter. If use_tridiagonal is set to True,
         a Wishart Ensemble random matrix in its tridiagonal form
         is sampled. Otherwise, it is sampled using the standard
         form.
 
+        Args:
+            random_state (int, default=None): random seed to initialize the pseudo-random
+                number generator of numpy. This has to be any integer between 0 and 2**32 - 1
+                (inclusive), or None (default). If None, the seed is obtained from the clock.
+
         Returns:
             numpy array containing new matrix sampled.
 
         References:
             - Dumitriu, I. and Edelman, A. "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
         """
+        if random_state is not None:
+            np.random.seed(random_state)
+
         if self.use_tridiagonal:
             if self.p > self.n:  # check reference ("Matrix Models for Beta Ensembles"): page 5, table 1.
                 raise ValueError("Error: cannot use tridiagonal form if 'p' (degrees of freedom)"
                                  " is greater than 'n' (sample size).\n"
                                  f"\t Provided n={self.n} and p={self.p}."
                                  " Set `use_tridiagonal=False` or increase sample size (`n`).")
             
@@ -260,29 +275,29 @@
         if self._eigvals is not None:
             return norm_const * self._eigvals
 
         # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvalsh(self.matrix)
         return norm_const * self._eigvals
 
-    def eigval_hist(self, bins, interval=None, density=False, normalize=True, avoid_img=False):
+    def eigval_hist(self, bins, interval=None, density=False, normalize=False, avoid_img=False):
         if self.use_tridiagonal:
             if normalize:
                 return tridiag_eigval_hist(
                     self.eigval_norm_const * self.matrix,
                     bins=bins,
                     interval=interval,
                     density=density,
                 )
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
         return super().eigval_hist(bins, interval=interval, density=density,
                                    normalize=normalize, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=True, fig_path=None):
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=False, savefig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
@@ -294,19 +309,19 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            normalize (bool, default=True): Whether to normalize the computed eigenvalues
-                by the default normalization constant (see references). Defaults to True, i.e.,
-                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
-                same support independently of the sample size.
-            fig_path (string, default=None): path to save the created figure. If it is not
+            normalize (bool, default=False): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to False, i.e.,
+                the eigenvalues are not normalized. Normalization makes the eigenvalues to be
+                in the same support independently of the sample size.
+            savefig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
@@ -318,36 +333,36 @@
         if interval is None:
             if normalize:
                 interval = (self.lambda_minus, self.lambda_plus)
             else:
                 interval = (self.n*self.lambda_minus, self.n*self.lambda_plus)
 
         if self.use_tridiagonal:
-            observed, bins = self.eigval_hist(
+            observed, bin_edges = self.eigval_hist(
                 bins=bins, interval=interval, density=density, normalize=normalize
             )
+            width = bin_edges[1]-bin_edges[0]
+            plt.bar(bin_edges[:-1], observed, width=width, align='edge')
 
-            width = bins[1]-bins[0]
-            plt.bar(bins[:-1], observed, width=width, align='edge')
             plt.title("Eigenvalue histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
-            if fig_path:
-                plt.savefig(fig_path, dpi=1000)
+            if savefig_path:
+                plt.savefig(savefig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
             super().plot_eigval_hist(
                 bins=bins,
                 interval=interval,
                 density=density,
                 normalize=normalize,
-                fig_path=fig_path,
+                savefig_path=savefig_path,
             )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
         eigenvalues. If the array of eigenvalues is not provided, the current random
```

### Comparing `scikit-rmt-0.7.1/tutorial/plot_0_introduction.py` & `scikit-rmt-0.8.0/tutorial/plot_0_introduction.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.7.1/tutorial/plot_1_spectral_laws.py` & `scikit-rmt-0.8.0/tutorial/plot_1_spectral_laws.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 x1 = np.linspace(0, 1, num=1000)
 x2 = np.linspace(0, 1, num=1000)
 
 fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(12,4))
 
 for a in [1.0, 1.2, 1.4, 1.6]:
     for b in [2.0]:
-        msd = ManovaSpectrumDistribution(beta=1, a=a, b=b)
+        msd = ManovaSpectrumDistribution(beta=1, ratio_a=a, ratio_b=b)
 
         y1 = msd.pdf(x1)
         y2 = msd.pdf(x2)
 
         ax1.plot(x1, y1, label=f"$a$ = {a}, $b$ = {b}")
         ax2.plot(x2, y2, label=f"$a$ = {a}, $b$ = {b}")
```

### Comparing `scikit-rmt-0.7.1/tutorial/plot_2_plot_spectral_laws.py` & `scikit-rmt-0.8.0/tutorial/plot_2_plot_spectral_laws.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,52 +48,49 @@
 # In the former example, GOE matrices of size :math:`n \times n` should be
 # normalized by :math:`1/\sqrt{n}`, which is done by default or by setting
 # `normalize=True`. 
 
 import numpy as np
 from skrmt.ensemble import GaussianEnsemble
 
-n=1000
-goe = GaussianEnsemble(beta=1, n=n)
+goe = GaussianEnsemble(beta=1, n=1000)
 goe.plot_eigval_hist(bins=80, interval=(-10, 10), normalize=True)
 
 ##############################################################################
 # Additionally, we can control the plotting interval to get a better picture
 # of the spectral density. In the GOE case, the spectral distribution is
-# concentrated in the (-2,2) interval.
+# concentrated in the (-2,2) interval. Note that the user does *not* need to
+# worry about the interval, **scikit-rmt** uses an adequate interval by default.
 
 import numpy as np
 from skrmt.ensemble import GaussianEnsemble
 
-n=1000
-goe = GaussianEnsemble(beta=1, n=n)
+goe = GaussianEnsemble(beta=1, n=1000)
 goe.plot_eigval_hist(bins=80, interval=(-2, 2), normalize=True)
 
 ##############################################################################
 # This example would be equivalent for Gaussian Unitary Ensemble (GUE) and
 # Gaussian Symplectic Ensemble (GSE).
 
 ##############################################################################
 # Another example would be using the Wishart Ensemble. In the following
 # snippet of code Wishart Real Ensemble (WRE) is sampled.
 
 from skrmt.ensemble import WishartEnsemble
 
-p, n = 1000, 3000
-wre = WishartEnsemble(beta=1, p=p, n=n)
+wre = WishartEnsemble(beta=1, p=1000, n=3000)
 wre.plot_eigval_hist(bins=80, interval=(-5,5))
 
 ##############################################################################
-# By default, scikit-rmt takes charge of using the most suitable plotting
+# By default, **scikit-rmt** takes charge of using the most suitable plotting
 # interval and eigenvalue normalization constant.
 
 from skrmt.ensemble import WishartEnsemble
 
-p, n = 1000, 3000
-wre = WishartEnsemble(beta=1, p=p, n=n)
+wre = WishartEnsemble(beta=1, p=1000, n=3000)
 wre.plot_eigval_hist(bins=80)
 
 ##############################################################################
 # This example would be equivalent for Wishart Complex Ensemble (WCE) and
 # Wishart Quaternion Ensemble (WQE), with the detail of controlling its
 # representation interval.
 
@@ -131,31 +128,31 @@
 
 ##############################################################################
 # We can easily analyze **Wigner's Semicircle Law** as follows.
 
 from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
 wsd = WignerSemicircleDistribution(beta=1)
-wsd.plot_empirical_pdf(n_size=2000, bins=80)
+wsd.plot_empirical_pdf(sample_size=2000, bins=80)
 
 ##############################################################################
 # We can also study **Marchenko-Pastur Law** as by:
 
 from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-mpd = MarchenkoPasturDistribution(ratio=1/3, beta=1)
-mpd.plot_empirical_pdf(n_size=6000, bins=80)
+mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+mpd.plot_empirical_pdf(sample_size=2000, bins=80)
 
 ##############################################################################
 # Finally, **Tracy-Widom Law** can be represented using:
 
 from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
 twd = TracyWidomDistribution(beta=1)
-twd.plot_empirical_pdf(n_size=100, times=10000, bins=80)
+twd.plot_empirical_pdf(sample_size=2000, bins=80)
 
 ##############################################################################
 # Spectral laws analytical expression
 # -----------------------------------
 # 
 # The spectral laws described so far have been proven to converge to certain
 # analytical functions that defines the limiting behaviour of the eigenvalue
@@ -167,46 +164,46 @@
 # The analytical probability function for the Gaussian Ensemble, known as
 # Wigner Semicircle Law, supported on :math:`[-R, R]` and centered at :math:`(0,0)`
 # is :math:`f(x) = \frac{2}{\pi R^2} \sqrt{R^2 - x^2}`.
 
 from skrmt.ensemble.spectral_law import WignerSemicircleDistribution
 
 wsd = WignerSemicircleDistribution(beta=1)
-wsd.plot_empirical_pdf(n_size=2000, bins=80, density=True, plot_law_pdf=True)
+wsd.plot_empirical_pdf(sample_size=2000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # The analytical probability function for the Wishart Ensemble known as
 # Marchenko-Pastur Law with parameter :math:`\lambda = p/n \in (0,1]` is
 # :math:`f_{\lambda}(x) = \frac{1}{2\pi \sigma^2}\frac{\sqrt{(\lambda_+ - x)(x - \lambda_-)}}{\lambda x}`,
 # where :math:`\lambda_{\pm} = \sigma^2 (1 \pm \sqrt{\lambda})^2`. 
 # If :math:`\lambda > 1` then the limiting distribution has an additional
 # mass probability point in the origin of size :math:`1 - \frac{1}{\lambda}`.
 
 from skrmt.ensemble.spectral_law import MarchenkoPasturDistribution
 
-mpd = MarchenkoPasturDistribution(ratio=1/3, beta=1)
-mpd.plot_empirical_pdf(n_size=6000, bins=80, density=True, plot_law_pdf=True)
+mpd = MarchenkoPasturDistribution(beta=1, ratio=1/3)
+mpd.plot_empirical_pdf(sample_size=2000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # In the other hand, the Tracy-Widom Law has a complex analytical expression,
 # that is the solution of a particular non-linear differential equation, described
 # in detail in:
 # S. Bauman. "The Tracy-Widom Distribution and its Application to Statistical Physics".
 # MIT Department of Physics. 2017.
 # The package scikit-rmt represents a precise
 # approximation of the theoretical Tracy-Widom pdf.
 
 from skrmt.ensemble.spectral_law import TracyWidomDistribution
 
 twd = TracyWidomDistribution(beta=1)
-twd.plot_empirical_pdf(n_size=10, times=5000, bins=80, density=True, plot_law_pdf=True)
+twd.plot_empirical_pdf(sample_size=2000, bins=80, density=True, plot_law_pdf=True)
 
 ##############################################################################
 # Finally, the limiting distribution of the Manova Ensemble is not described
 # by any famous Law, but its expression has been determined. This library
 # provides functionality to show it on top of the empirical histogram of the
 # eigenvalue spectrum.
 
 from skrmt.ensemble.spectral_law import ManovaSpectrumDistribution
 
-msd = ManovaSpectrumDistribution(a=3, b=3, beta=1)
-msd.plot_empirical_pdf(m_size=1000, bins=80, density=True, plot_law_pdf=True)
+msd = ManovaSpectrumDistribution(beta=1, ratio_a=3, ratio_b=3)
+msd.plot_empirical_pdf(sample_size=2000, bins=80, density=True, plot_law_pdf=True)
```

