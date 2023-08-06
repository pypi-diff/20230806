# Comparing `tmp/simple_ts-0.6.tar.gz` & `tmp/simple_ts-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.6.tar", last modified: Fri Jul 14 04:08:42 2023, max compression
+gzip compressed data, was "simple_ts-0.7.tar", last modified: Sun Aug  6 05:47:01 2023, max compression
```

## Comparing `simple_ts-0.6.tar` & `simple_ts-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.894399 simple_ts-0.6/
--rw-rw-rw-   0        0        0      125 2023-07-14 04:08:42.894399 simple_ts-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.6/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 04:08:42.894399 simple_ts-0.6/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-14 04:08:34.000000 simple_ts-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.886914 simple_ts-0.6/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.894399 simple_ts-0.6/simplets/
--rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.6/simplets/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-07-14 04:08:24.000000 simple_ts-0.6/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:47:01.421470 simple_ts-0.7/
+-rw-rw-rw-   0        0        0      125 2023-08-06 05:47:01.419942 simple_ts-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-08-06 05:36:14.000000 simple_ts-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 05:47:01.422656 simple_ts-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-08-06 05:40:19.000000 simple_ts-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 05:47:01.413941 simple_ts-0.7/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-08-06 05:47:01.000000 simple_ts-0.7/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-08-06 05:47:01.000000 simple_ts-0.7/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 05:47:01.000000 simple_ts-0.7/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-06 05:47:01.000000 simple_ts-0.7/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 05:47:01.000000 simple_ts-0.7/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 05:47:01.416944 simple_ts-0.7/simplets/
+-rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.7/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-07-14 17:01:17.000000 simple_ts-0.7/simplets/simplets.py
```

### Comparing `simple_ts-0.6/simplets/simplets.py` & `simple_ts-0.7/simplets/simplets.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
         result = seasonal_decompose(ts, model='additive')
 
 # Obter as componentes da decomposição
         trend = result.trend
         seasonal = result.seasonal
         residuals = result.resid
 
+
+
 # Plotar as componentes da decomposição
         plt.figure(figsize=(10, 8))
         plt.subplot(411)
         plt.plot(ts, label='Original')
         plt.legend(loc='upper left')
 
         plt.subplot(412)
```

