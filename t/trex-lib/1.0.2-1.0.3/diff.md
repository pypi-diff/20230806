# Comparing `tmp/trex-lib-1.0.2.tar.gz` & `tmp/trex-lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-lib-1.0.2.tar", last modified: Tue Aug  1 02:31:42 2023, max compression
+gzip compressed data, was "trex-lib-1.0.3.tar", last modified: Sun Aug  6 14:41:52 2023, max compression
```

## Comparing `trex-lib-1.0.2.tar` & `trex-lib-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.338131 trex-lib-1.0.2/
--rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.2/LICENSE
--rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.2/MANIFEST.in
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-08-01 02:31:42.338294 trex-lib-1.0.2/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.2/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.2/pyproject.toml
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-01 02:31:42.338884 trex-lib-1.0.2/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      911 2023-08-01 02:30:32.000000 trex-lib-1.0.2/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.314446 trex-lib-1.0.2/trex_lib.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-08-01 02:31:42.000000 trex-lib-1.0.2/trex_lib.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1247 2023-08-01 02:31:42.000000 trex-lib-1.0.2/trex_lib.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-01 02:31:42.000000 trex-lib-1.0.2/trex_lib.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)      124 2023-08-01 02:31:42.000000 trex-lib-1.0.2/trex_lib.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-08-01 02:31:42.000000 trex-lib-1.0.2/trex_lib.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.315008 trex-lib-1.0.2/trexlib/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.2/trexlib/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5304 2023-03-08 04:35:45.000000 trex-lib-1.0.2/trexlib/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.315796 trex-lib-1.0.2/trexlib/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.2/trexlib/libs/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.316314 trex-lib-1.0.2/trexlib/libs/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.2/trexlib/libs/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.2/trexlib/libs/controllers/task_base_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.317537 trex-lib-1.0.2/trexlib/libs/firebase/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.2/trexlib/libs/firebase/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.2/trexlib/libs/firebase/firebase_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.318613 trex-lib-1.0.2/trexlib/libs/flask_wtf/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.2/trexlib/libs/flask_wtf/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.2/trexlib/libs/flask_wtf/crsf_ext.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.323411 trex-lib-1.0.2/trexlib/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.2/trexlib/utils/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.334057 trex-lib-1.0.2/trexlib/utils/common/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.2/trexlib/utils/common/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-1.0.2/trexlib/utils/common/cache_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.2/trexlib/utils/common/common_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.2/trexlib/utils/common/conftest.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.2/trexlib/utils/common/crm_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.2/trexlib/utils/common/currency_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2707 2021-09-16 10:19:23.000000 trex-lib-1.0.2/trexlib/utils/common/date_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.2/trexlib/utils/common/float_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.2/trexlib/utils/common/format_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.2/trexlib/utils/common/pagination_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.2/trexlib/utils/common/phone_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.2/trexlib/utils/common/user_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.2/trexlib/utils/crypto_util.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-01 02:31:42.337216 trex-lib-1.0.2/trexlib/utils/google/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.2/trexlib/utils/google/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.2/trexlib/utils/google/bigquery_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4051 2022-09-09 02:31:34.000000 trex-lib-1.0.2/trexlib/utils/google/cloud_tasks_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.2/trexlib/utils/google/gcloud_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.2/trexlib/utils/log_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.2/trexlib/utils/security_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     5590 2023-06-14 07:07:14.000000 trex-lib-1.0.2/trexlib/utils/string_util.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.2/trexlib/utils/url_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.568588 trex-lib-1.0.3/
+-rw-r--r--   0 jacklok    (501) staff       (20)     1052 2020-09-03 05:31:42.000000 trex-lib-1.0.3/LICENSE
+-rw-r--r--   0 jacklok    (501) staff       (20)       58 2020-09-03 00:38:04.000000 trex-lib-1.0.3/MANIFEST.in
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-08-06 14:41:52.568832 trex-lib-1.0.3/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       34 2020-09-03 04:20:20.000000 trex-lib-1.0.3/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)      172 2021-08-13 04:29:57.000000 trex-lib-1.0.3/pyproject.toml
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-08-06 14:41:52.570155 trex-lib-1.0.3/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      911 2023-08-06 14:41:48.000000 trex-lib-1.0.3/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.541209 trex-lib-1.0.3/trex_lib.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      462 2023-08-06 14:41:52.000000 trex-lib-1.0.3/trex_lib.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1247 2023-08-06 14:41:52.000000 trex-lib-1.0.3/trex_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-08-06 14:41:52.000000 trex-lib-1.0.3/trex_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)      124 2023-08-06 14:41:52.000000 trex-lib-1.0.3/trex_lib.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       14 2023-08-06 14:41:52.000000 trex-lib-1.0.3/trex_lib.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.541852 trex-lib-1.0.3/trexlib/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-04 07:13:04.000000 trex-lib-1.0.3/trexlib/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5304 2023-03-08 04:35:45.000000 trex-lib-1.0.3/trexlib/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.542841 trex-lib-1.0.3/trexlib/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:13.000000 trex-lib-1.0.3/trexlib/libs/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.543832 trex-lib-1.0.3/trexlib/libs/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2023-02-13 02:03:08.000000 trex-lib-1.0.3/trexlib/libs/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9782 2023-03-28 03:00:42.000000 trex-lib-1.0.3/trexlib/libs/controllers/task_base_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.545627 trex-lib-1.0.3/trexlib/libs/firebase/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2022-06-09 04:14:24.000000 trex-lib-1.0.3/trexlib/libs/firebase/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      378 2022-06-09 06:38:00.000000 trex-lib-1.0.3/trexlib/libs/firebase/firebase_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.547062 trex-lib-1.0.3/trexlib/libs/flask_wtf/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-22 09:26:46.000000 trex-lib-1.0.3/trexlib/libs/flask_wtf/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      133 2021-01-22 09:30:44.000000 trex-lib-1.0.3/trexlib/libs/flask_wtf/crsf_ext.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.552157 trex-lib-1.0.3/trexlib/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-09-01 09:38:27.000000 trex-lib-1.0.3/trexlib/utils/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.563513 trex-lib-1.0.3/trexlib/utils/common/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2020-08-31 07:47:30.000000 trex-lib-1.0.3/trexlib/utils/common/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      428 2020-09-03 08:42:39.000000 trex-lib-1.0.3/trexlib/utils/common/cache_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4514 2022-09-26 14:54:31.000000 trex-lib-1.0.3/trexlib/utils/common/common_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      488 2020-09-01 10:21:00.000000 trex-lib-1.0.3/trexlib/utils/common/conftest.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1194 2020-09-04 02:28:26.000000 trex-lib-1.0.3/trexlib/utils/common/crm_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1573 2021-04-21 02:37:36.000000 trex-lib-1.0.3/trexlib/utils/common/currency_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2707 2021-09-16 10:19:23.000000 trex-lib-1.0.3/trexlib/utils/common/date_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      290 2020-09-01 10:20:46.000000 trex-lib-1.0.3/trexlib/utils/common/float_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4201 2021-03-04 08:12:18.000000 trex-lib-1.0.3/trexlib/utils/common/format_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1086 2020-09-04 07:48:19.000000 trex-lib-1.0.3/trexlib/utils/common/pagination_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2021-06-24 07:11:43.000000 trex-lib-1.0.3/trexlib/utils/common/phone_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      825 2021-08-13 09:35:21.000000 trex-lib-1.0.3/trexlib/utils/common/user_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      840 2021-07-01 09:54:24.000000 trex-lib-1.0.3/trexlib/utils/crypto_util.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-08-06 14:41:52.567323 trex-lib-1.0.3/trexlib/utils/google/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-01-20 04:05:45.000000 trex-lib-1.0.3/trexlib/utils/google/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12907 2021-08-20 10:49:32.000000 trex-lib-1.0.3/trexlib/utils/google/bigquery_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4051 2022-09-09 02:31:34.000000 trex-lib-1.0.3/trexlib/utils/google/cloud_tasks_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1364 2023-03-08 04:49:28.000000 trex-lib-1.0.3/trexlib/utils/google/gcloud_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      159 2020-09-04 07:30:52.000000 trex-lib-1.0.3/trexlib/utils/log_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3215 2021-08-13 04:41:06.000000 trex-lib-1.0.3/trexlib/utils/security_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     5597 2023-08-06 14:12:27.000000 trex-lib-1.0.3/trexlib/utils/string_util.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1277 2020-09-04 07:38:09.000000 trex-lib-1.0.3/trexlib/utils/url_util.py
```

### Comparing `trex-lib-1.0.2/LICENSE` & `trex-lib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/setup.py` & `trex-lib-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-lib',  
-     version='1.0.2',
+     version='1.0.3',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex Core library package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-lib",
      packages=setuptools.find_packages(),
```

### Comparing `trex-lib-1.0.2/trex_lib.egg-info/SOURCES.txt` & `trex-lib-1.0.3/trex_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/conf.py` & `trex-lib-1.0.3/trexlib/conf.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/libs/controllers/task_base_routes.py` & `trex-lib-1.0.3/trexlib/libs/controllers/task_base_routes.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/common_util.py` & `trex-lib-1.0.3/trexlib/utils/common/common_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/crm_util.py` & `trex-lib-1.0.3/trexlib/utils/common/crm_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/currency_util.py` & `trex-lib-1.0.3/trexlib/utils/common/currency_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/date_util.py` & `trex-lib-1.0.3/trexlib/utils/common/date_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/format_util.py` & `trex-lib-1.0.3/trexlib/utils/common/format_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/pagination_util.py` & `trex-lib-1.0.3/trexlib/utils/common/pagination_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/phone_util.py` & `trex-lib-1.0.3/trexlib/utils/common/phone_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/common/user_util.py` & `trex-lib-1.0.3/trexlib/utils/common/user_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/crypto_util.py` & `trex-lib-1.0.3/trexlib/utils/crypto_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/google/bigquery_util.py` & `trex-lib-1.0.3/trexlib/utils/google/bigquery_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/google/cloud_tasks_util.py` & `trex-lib-1.0.3/trexlib/utils/google/cloud_tasks_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/google/gcloud_util.py` & `trex-lib-1.0.3/trexlib/utils/google/gcloud_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/security_util.py` & `trex-lib-1.0.3/trexlib/utils/security_util.py`

 * *Files identical despite different names*

### Comparing `trex-lib-1.0.2/trexlib/utils/string_util.py` & `trex-lib-1.0.3/trexlib/utils/string_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Created on Jul 3, 2012
 
 @author: sglok
 '''
 import random, re, string, logging
 import hmac
-from datetime import time
+from datetime import datetime
 
 WHITESPACE_PATTERN  = re.compile(r'\s')
 DASH_PATTERN        = re.compile(r'-')
 
 ALPHANUMERIC_CHARS  = string.ascii_lowercase + string.ascii_uppercase + string.digits
 NUMERIC_CHARS       = string.digits
 
@@ -29,15 +29,15 @@
 
     if isinstance(b, str):
         b = b.encode("utf-8")  # type: ignore
 
     return hmac.compare_digest(a, b)
 
 def random_string(number_character, is_human_mistake_safe=False):
-    random.seed(time.time())
+    random.seed(datetime.now())
     if is_human_mistake_safe:
         if number_character and type(number_character) is int and number_character>=0:
             return ''.join(random.sample(HUMAN_SAFE_ALPHANUMERIC_CHARS, number_character))
         else:
             return ''
 
     else:
```

### Comparing `trex-lib-1.0.2/trexlib/utils/url_util.py` & `trex-lib-1.0.3/trexlib/utils/url_util.py`

 * *Files identical despite different names*

