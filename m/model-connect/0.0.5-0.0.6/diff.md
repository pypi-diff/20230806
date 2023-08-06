# Comparing `tmp/model-connect-0.0.5.tar.gz` & `tmp/model-connect-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-connect-0.0.5.tar", last modified: Mon Jul 31 04:57:53 2023, max compression
+gzip compressed data, was "model-connect-0.0.6.tar", last modified: Sun Aug  6 20:46:29 2023, max compression
```

## Comparing `model-connect-0.0.5.tar` & `model-connect-0.0.6.tar`

### file list

```diff
@@ -1,63 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.551802 model-connect-0.0.5/
--rw-rw-rw-   0        0        0    10921 2023-07-31 04:57:53.551802 model-connect-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10818 2023-07-31 00:53:30.000000 model-connect-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.488674 model-connect-0.0.5/model_connect/
--rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.5/model_connect/__init__.py
--rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.5/model_connect/connect.py
--rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.5/model_connect/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.513450 model-connect-0.0.5/model_connect/integrations/
--rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.5/model_connect/integrations/__init__.py
--rw-rw-rw-   0        0        0      651 2023-07-31 00:56:43.000000 model-connect-0.0.5/model_connect/integrations/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.515445 model-connect-0.0.5/model_connect/integrations/fastapi/
--rw-rw-rw-   0        0        0      401 2023-07-31 01:00:27.000000 model-connect-0.0.5/model_connect/integrations/fastapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.519606 model-connect-0.0.5/model_connect/integrations/fastapi/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/__init__.py
--rw-rw-rw-   0        0        0      961 2023-07-31 00:49:20.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/model.py
--rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/model_field.py
--rw-rw-rw-   0        0        0      504 2023-07-31 00:52:20.000000 model-connect-0.0.5/model_connect/integrations/fastapi/router.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.521604 model-connect-0.0.5/model_connect/integrations/json/
--rw-rw-rw-   0        0        0        0 2023-07-31 03:58:32.000000 model-connect-0.0.5/model_connect/integrations/json/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-31 03:58:41.000000 model-connect-0.0.5/model_connect/integrations/json/decoder.py
--rw-rw-rw-   0        0        0        0 2023-07-31 03:58:45.000000 model-connect-0.0.5/model_connect/integrations/json/encoder.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.522605 model-connect-0.0.5/model_connect/integrations/json/options/
--rw-rw-rw-   0        0        0        0 2023-07-31 03:58:36.000000 model-connect-0.0.5/model_connect/integrations/json/options/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.528786 model-connect-0.0.5/model_connect/integrations/psycopg2/
--rw-rw-rw-   0        0        0      846 2023-07-31 02:56:09.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.531785 model-connect-0.0.5/model_connect/integrations/psycopg2/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 01:29:50.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/__init__.py
--rw-rw-rw-   0        0        0     4034 2023-07-31 03:53:55.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/processing.py
--rw-rw-rw-   0        0        0     1393 2023-07-31 04:42:27.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/streaming.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/delete.py
--rw-rw-rw-   0        0        0     2960 2023-07-31 04:50:50.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/insert.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.534784 model-connect-0.0.5/model_connect/integrations/psycopg2/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/__init__.py
--rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/model.py
--rw-rw-rw-   0        0        0     1157 2023-07-31 03:44:39.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/model_field.py
--rw-rw-rw-   0        0        0     4135 2023-07-31 04:55:13.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/select.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/update.py
--rw-rw-rw-   0        0        0      840 2023-07-31 01:16:35.000000 model-connect-0.0.5/model_connect/integrations/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.537297 model-connect-0.0.5/model_connect/options/
--rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.5/model_connect/options/__init__.py
--rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.5/model_connect/options/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.540296 model-connect-0.0.5/model_connect/options/global/
--rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.5/model_connect/options/global/__init__.py
--rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.5/model_connect/options/global/global.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.544293 model-connect-0.0.5/model_connect/options/model/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.5/model_connect/options/model/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-07-31 02:56:34.000000 model-connect-0.0.5/model_connect/options/model/model.py
--rw-rw-rw-   0        0        0     1508 2023-07-31 02:03:06.000000 model-connect-0.0.5/model_connect/options/model/query_params.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.546796 model-connect-0.0.5/model_connect/options/model_field/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.5/model_connect/options/model_field/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.549803 model-connect-0.0.5/model_connect/options/model_field/dtos/
--rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/request.py
--rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/response.py
--rw-rw-rw-   0        0        0     3533 2023-07-31 03:43:04.000000 model-connect-0.0.5/model_connect/options/model_field/model_field.py
--rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.5/model_connect/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.509456 model-connect-0.0.5/model_connect.egg-info/
--rw-rw-rw-   0        0        0    10921 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 04:57:53.552802 model-connect-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-31 04:57:46.000000 model-connect-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.754945 model-connect-0.0.6/
+-rw-rw-rw-   0        0        0    10953 2023-08-06 20:46:29.753945 model-connect-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10850 2023-08-06 20:45:51.000000 model-connect-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.690551 model-connect-0.0.6/model_connect/
+-rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.6/model_connect/__init__.py
+-rw-rw-rw-   0        0        0      953 2023-08-04 01:07:58.000000 model-connect-0.0.6/model_connect/connect.py
+-rw-rw-rw-   0        0        0      579 2023-08-03 03:43:00.000000 model-connect-0.0.6/model_connect/constants.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.713018 model-connect-0.0.6/model_connect/globals/
+-rw-rw-rw-   0        0        0        0 2023-08-04 00:33:48.000000 model-connect-0.0.6/model_connect/globals/__init__.py
+-rw-rw-rw-   0        0        0      230 2023-08-04 00:47:00.000000 model-connect-0.0.6/model_connect/globals/connect.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.716018 model-connect-0.0.6/model_connect/globals/options/
+-rw-rw-rw-   0        0        0        0 2023-08-04 00:33:57.000000 model-connect-0.0.6/model_connect/globals/options/__init__.py
+-rw-rw-rw-   0        0        0      896 2023-08-04 00:41:31.000000 model-connect-0.0.6/model_connect/globals/options/connect.py
+-rw-rw-rw-   0        0        0      470 2023-08-04 11:52:20.000000 model-connect-0.0.6/model_connect/globals/options/fastapi.py
+-rw-rw-rw-   0        0        0      119 2023-08-04 00:38:40.000000 model-connect-0.0.6/model_connect/globals/options/psycopg2.py
+-rw-rw-rw-   0        0        0      974 2023-08-04 00:46:31.000000 model-connect-0.0.6/model_connect/globals/registry.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.721534 model-connect-0.0.6/model_connect/integrations/
+-rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.6/model_connect/integrations/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-08-01 02:48:47.000000 model-connect-0.0.6/model_connect/integrations/base.py
+-rw-rw-rw-   0        0        0      355 2023-08-04 01:02:26.000000 model-connect-0.0.6/model_connect/integrations/connect.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.722535 model-connect-0.0.6/model_connect/integrations/fastapi/
+-rw-rw-rw-   0        0        0      161 2023-08-04 01:03:57.000000 model-connect-0.0.6/model_connect/integrations/fastapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.725533 model-connect-0.0.6/model_connect/integrations/fastapi/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.6/model_connect/integrations/fastapi/options/__init__.py
+-rw-rw-rw-   0        0        0     1078 2023-08-04 01:16:18.000000 model-connect-0.0.6/model_connect/integrations/fastapi/options/model.py
+-rw-rw-rw-   0        0        0      382 2023-08-03 01:33:41.000000 model-connect-0.0.6/model_connect/integrations/fastapi/options/model_field.py
+-rw-rw-rw-   0        0        0     1201 2023-08-04 11:53:00.000000 model-connect-0.0.6/model_connect/integrations/fastapi/router.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.728534 model-connect-0.0.6/model_connect/integrations/json/
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:32.000000 model-connect-0.0.6/model_connect/integrations/json/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:41.000000 model-connect-0.0.6/model_connect/integrations/json/decoder.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:45.000000 model-connect-0.0.6/model_connect/integrations/json/encoder.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.730534 model-connect-0.0.6/model_connect/integrations/json/options/
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:36.000000 model-connect-0.0.6/model_connect/integrations/json/options/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.735057 model-connect-0.0.6/model_connect/integrations/psycopg2/
+-rw-rw-rw-   0        0        0      396 2023-08-04 01:02:26.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.738059 model-connect-0.0.6/model_connect/integrations/psycopg2/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:29:50.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/common/__init__.py
+-rw-rw-rw-   0        0        0     6847 2023-08-03 05:16:22.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/common/processing.py
+-rw-rw-rw-   0        0        0     2792 2023-08-03 05:39:33.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/common/streaming.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/delete.py
+-rw-rw-rw-   0        0        0     3549 2023-08-02 04:54:46.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/insert.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.741573 model-connect-0.0.6/model_connect/integrations/psycopg2/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/options/__init__.py
+-rw-rw-rw-   0        0        0      895 2023-08-03 02:06:31.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/options/model.py
+-rw-rw-rw-   0        0        0     3543 2023-08-03 05:05:14.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/options/model_field.py
+-rw-rw-rw-   0        0        0     5729 2023-08-02 02:16:53.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/select.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.6/model_connect/integrations/psycopg2/update.py
+-rw-rw-rw-   0        0        0      670 2023-08-04 01:01:36.000000 model-connect-0.0.6/model_connect/integrations/type_registry.py
+-rw-rw-rw-   0        0        0      282 2023-08-04 01:01:08.000000 model-connect-0.0.6/model_connect/integrations/types.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.743573 model-connect-0.0.6/model_connect/options/
+-rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.6/model_connect/options/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.6/model_connect/options/connect.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.744573 model-connect-0.0.6/model_connect/options/global/
+-rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.6/model_connect/options/global/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.747573 model-connect-0.0.6/model_connect/options/model/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.6/model_connect/options/model/__init__.py
+-rw-rw-rw-   0        0        0     3277 2023-08-04 01:03:57.000000 model-connect-0.0.6/model_connect/options/model/model.py
+-rw-rw-rw-   0        0        0     1508 2023-07-31 02:03:06.000000 model-connect-0.0.6/model_connect/options/model/query_params.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.749573 model-connect-0.0.6/model_connect/options/model_field/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.6/model_connect/options/model_field/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.752946 model-connect-0.0.6/model_connect/options/model_field/dtos/
+-rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.6/model_connect/options/model_field/dtos/__init__.py
+-rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.6/model_connect/options/model_field/dtos/request.py
+-rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.6/model_connect/options/model_field/dtos/response.py
+-rw-rw-rw-   0        0        0     4707 2023-08-04 01:04:12.000000 model-connect-0.0.6/model_connect/options/model_field/model_field.py
+-rw-rw-rw-   0        0        0     3572 2023-08-03 23:44:27.000000 model-connect-0.0.6/model_connect/registry.py
+drwxrwxrwx   0        0        0        0 2023-08-06 20:46:29.709533 model-connect-0.0.6/model_connect.egg-info/
+-rw-rw-rw-   0        0        0    10953 2023-08-06 20:46:29.000000 model-connect-0.0.6/model_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2212 2023-08-06 20:46:29.000000 model-connect-0.0.6/model_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 20:46:29.000000 model-connect-0.0.6/model_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-06 20:46:29.000000 model-connect-0.0.6/model_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 20:46:29.754945 model-connect-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-08-06 20:46:26.000000 model-connect-0.0.6/setup.py
```

### Comparing `model-connect-0.0.5/PKG-INFO` & `model-connect-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
@@ -399,14 +399,15 @@
 python setup.py sdist
 ```
 
 To upload to PyPi:
 
 ```bash
 twine upload dist/*
+# twine upload dist/<filename>
 ```
 
 To do both:
     
 ```bash
 python setup.py sdist
 twine upload dist/*
```

### Comparing `model-connect-0.0.5/README.md` & `model-connect-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,15 @@
 python setup.py sdist
 ```
 
 To upload to PyPi:
 
 ```bash
 twine upload dist/*
+# twine upload dist/<filename>
 ```
 
 To do both:
     
 ```bash
 python setup.py sdist
 twine upload dist/*
```

### Comparing `model-connect-0.0.5/model_connect/integrations/base.py` & `model-connect-0.0.6/model_connect/integrations/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,25 +6,37 @@
     from model_connect.options import ConnectOptions, ModelField
 
 _T = TypeVar('_T')
 
 
 @dataclass
 class BaseIntegrationModel(ABC):
+    @classmethod
+    @property
+    @abstractmethod
+    def integration_name(cls) -> str:
+        ...
+
     @abstractmethod
     def resolve(self, options: 'ConnectOptions'):
         ...
 
 
 @dataclass
 class BaseIntegrationModelField(ABC):
+    @classmethod
+    @property
+    @abstractmethod
+    def integration_name(self) -> str:
+        ...
+
     @abstractmethod
     def resolve(self, options: 'ConnectOptions', model_field: 'ModelField'):
         ...
 
 
-class ModelIntegrations(dict[type[_T], _T]):
+class ModelIntegrations(dict[str, _T]):
     pass
 
 
-class ModelFieldIntegrations(dict[type[_T], _T]):
+class ModelFieldIntegrations(dict[str, _T]):
     pass
```

### Comparing `model-connect-0.0.5/model_connect/integrations/fastapi/options/model.py` & `model-connect-0.0.6/model_connect/integrations/fastapi/options/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,29 @@
     resource_version: int = UNDEFINED
     tag_name: str = UNDEFINED
 
     _connect_options: ConnectOptions = field(
         init=False
     )
 
+    @classmethod
+    @property
+    def integration_name(cls) -> str:
+        return 'fastapi'
+
     def resolve(self, connect_options: ConnectOptions):
         self._connect_options = connect_options
 
         self.resource_path = coalesce(
             self.resource_path,
-            self._connect_options.dataclass_type.__name__.lower()
+            '/' + self._connect_options.model.name_plural_kebab_case,
         )
 
         self.resource_version = coalesce(
             self.resource_version,
-            1
+            None
         )
 
         self.tag_name = coalesce(
             self.tag_name,
-            self._connect_options.dataclass_type.__name__
+            ' '.join(self._connect_options.model.name_plural_parts)
         )
```

### Comparing `model-connect-0.0.5/model_connect/integrations/psycopg2/options/model.py` & `model-connect-0.0.6/model_connect/integrations/psycopg2/options/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 class Psycopg2Model(BaseIntegrationModel):
     tablename: str = UNDEFINED
 
     _connect_options: 'ConnectOptions' = field(
         init=False
     )
 
+    @classmethod
+    @property
+    def integration_name(cls) -> str:
+        return 'psycopg2'
+
     def resolve(self, connect_options: 'ConnectOptions'):
         self._connect_options = connect_options
 
         self.tablename = coalesce(
             self.tablename,
-            self._connect_options.model.name_plural,
-            self._connect_options.model.name_single
+            self._connect_options.model.name_plural_snake_case,
+            self._connect_options.model.name_single_snake_case
         )
-
-        self.tablename = self.tablename.lower()
```

### Comparing `model-connect-0.0.5/model_connect/integrations/psycopg2/options/model_field.py` & `model-connect-0.0.6/model_connect/options/model_field/dtos/response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,62 @@
-from dataclasses import dataclass
+from dataclasses import Field, dataclass, field
+from typing import Any, Callable, TYPE_CHECKING
 
-from model_connect.constants import UNDEFINED, coalesce
-from model_connect.integrations.base import BaseIntegrationModelField
-from model_connect.options import ConnectOptions, ModelField
+from model_connect.constants import UNDEFINED, iter_http_methods, coalesce
 
+if TYPE_CHECKING:
+    from model_connect.options import ConnectOptions
 
-@dataclass
-class Psycopg2ModelField(BaseIntegrationModelField):
-    can_filter: bool = UNDEFINED
-    can_sort: bool = UNDEFINED
-    column_name: str = UNDEFINED
-    include_in_insert: bool = UNDEFINED
-    include_in_select: bool = UNDEFINED
-
-    def resolve(self, options: 'ConnectOptions', model_field: 'ModelField'):
-        self.can_filter = coalesce(
-            self.can_filter,
-            True
-        )
 
-        self.can_sort = coalesce(
-            self.can_sort,
-            True
-        )
+class ResponseDtos(dict[str, 'ResponseDto']):
+    def resolve(
+            self,
+            connect_options: 'ConnectOptions',
+            dataclass_field: Field
+    ):
+        for method in iter_http_methods():
+            method = method.lower()
+            if method not in self:
+                self[method] = ResponseDto()
+
+        for name, dto in self.items():
+            self[name] = coalesce(
+                dto,
+                ResponseDto()
+            )
+
+            self[name].resolve(
+                connect_options,
+                dataclass_field
+            )
 
-        self.column_name = coalesce(
-            self.column_name,
-            model_field.name
-        )
 
-        self.include_in_insert = coalesce(
-            self.include_in_insert,
-            not model_field.is_identifier
-        )
+@dataclass
+class ResponseDto:
+    include: bool = UNDEFINED
+    preprocessor: Callable[[Any], Any] = UNDEFINED
+
+    _connect_options: 'ConnectOptions' = field(
+        init=False
+    )
+
+    _dataclass_field: Field = field(
+        init=False
+    )
+
+    def resolve(
+            self,
+            connect_options: 'ConnectOptions',
+            dataclass_field: Field
+    ):
+        self._connect_options = connect_options
+        self._dataclass_field = dataclass_field
 
-        self.include_in_select = coalesce(
-            self.include_in_select,
-            model_field.dataclass_field.init,
+        self.include = coalesce(
+            self.include,
             True
         )
+
+        self.preprocessor = coalesce(
+            self.preprocessor,
+            None
+        )
```

### Comparing `model-connect-0.0.5/model_connect/options/connect.py` & `model-connect-0.0.6/model_connect/options/connect.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.5/model_connect/options/model/query_params.py` & `model-connect-0.0.6/model_connect/options/model/query_params.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.5/model_connect/options/model_field/dtos/request.py` & `model-connect-0.0.6/model_connect/options/model_field/dtos/request.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.5/model_connect/options/model_field/model_field.py` & `model-connect-0.0.6/model_connect/options/model_field/model_field.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 from dataclasses import Field, fields, dataclass, field
+from types import NoneType
 from typing import TYPE_CHECKING
 
 from model_connect.constants import UNDEFINED, coalesce
 from model_connect.integrations.base import BaseIntegrationModelField, ModelFieldIntegrations
-from model_connect.integrations import registry as integrations_registry
-from model_connect.options.model.query_params import QueryParams
+from model_connect.integrations import type_registry
 from model_connect.options.model_field.dtos.request import RequestDtos
 from model_connect.options.model_field.dtos.response import ResponseDtos
 
 if TYPE_CHECKING:
     from model_connect.options import ConnectOptions
 
 
+def has_default_value(dataclass_field: Field):
+    return dataclass_field.default is not dataclass_field.default_factory
+
+
 class ModelFields(dict[str, 'ModelField']):
     def resolve(
             self,
             options: 'ConnectOptions'
     ):
         # noinspection PyDataclass
         for dataclass_field in fields(options.dataclass_type):
             name = dataclass_field.name
 
             if name not in self:
                 self[name] = ModelField()
 
-            self[name].resolve(options, dataclass_field)
+            self[name].resolve(
+                options,
+                dataclass_field
+            )
 
 
 @dataclass
 class ModelField:
     can_sort: bool = UNDEFINED
     can_filter: bool = UNDEFINED
+    can_group: bool = UNDEFINED
+    is_db_column: bool = UNDEFINED
     is_identifier: bool = UNDEFINED
+    is_required_on_init: bool = UNDEFINED
     request_dtos: RequestDtos = UNDEFINED
     response_dtos: ResponseDtos = UNDEFINED
     query_params: tuple[str, ...] = UNDEFINED
     override_integrations: tuple['BaseIntegrationModelField', ...] = UNDEFINED
 
     _connect_options: 'ConnectOptions' = field(
         init=False
     )
 
     _dataclass_field: Field = field(
         init=False
     )
 
-    _type: type = field(
+    _inferred_type: str = field(
         init=False
     )
 
     _name: str = field(
         init=False
     )
 
@@ -59,51 +69,80 @@
     )
 
     @property
     def dataclass_field(self):
         return self._dataclass_field
 
     @property
-    def type(self):
-        return self._type
+    def inferred_type(self):
+        return self._inferred_type
 
     @property
     def name(self):
         return self._name
 
     @property
     def integrations(self):
         return self._integrations
 
     def resolve(
             self,
-            options: 'ConnectOptions',
+            connect_options: 'ConnectOptions',
             dataclass_field: Field
     ):
-        self._type = dataclass_field.type
+        self._inferred_type = dataclass_field.type
         self._name = dataclass_field.name
 
-        self._connect_options = options
+        if hasattr(self._inferred_type, '__args__'):
+            type_args = self._inferred_type.__args__
+
+            if len(type_args) == 2 and NoneType in type_args:
+                self._inferred_type = coalesce(*type_args)
+
+        self._connect_options = connect_options
         self._dataclass_field = dataclass_field
 
         self.can_sort = coalesce(
             self.can_sort,
             True
         )
 
         self.can_filter = coalesce(
             self.can_filter,
             True
         )
 
+        self.can_group = coalesce(
+            self.can_group,
+            True
+        )
+
+        self.is_db_column = coalesce(
+            self.is_db_column,
+            True
+        )
+
         self.is_identifier = coalesce(
             self.is_identifier,
             False
         )
 
+        is_required_on_init = True
+
+        if dataclass_field.init is False:
+            is_required_on_init = False
+
+        if has_default_value(dataclass_field):
+            is_required_on_init = False
+
+        self.is_required_on_init = coalesce(
+            self.is_required_on_init,
+            is_required_on_init
+        )
+
         self.request_dtos = coalesce(
             self.request_dtos,
             RequestDtos()
         )
 
         self.response_dtos = coalesce(
             self.response_dtos,
@@ -111,18 +150,24 @@
         )
 
         self.override_integrations = coalesce(
             self.override_integrations,
             ()
         )
 
-        self.request_dtos.resolve(options, dataclass_field)
-        self.response_dtos.resolve(options, dataclass_field)
+        self.request_dtos.resolve(connect_options, dataclass_field)
+        self.response_dtos.resolve(connect_options, dataclass_field)
 
         for integration in self.override_integrations:
-            self._integrations[integration.__class__] = integration
+            name = integration.integration_name
+
+            self._integrations[name] = integration
+            self._integrations[name].resolve(connect_options, self)
+
+        for name, _, model_field_class in type_registry.iterate():
+            if name in self._integrations:
+                continue
 
-        for name, (model_class, model_field_class) in integrations_registry.iterate():
-            if model_field_class not in self._integrations:
-                self._integrations[model_field_class] = model_field_class()
+            model_field = model_field_class()
+            model_field.resolve(connect_options, self)
 
-            self._integrations[model_field_class].resolve(options, self)
+            self._integrations[name] = model_field
```

### Comparing `model-connect-0.0.5/model_connect.egg-info/PKG-INFO` & `model-connect-0.0.6/model_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
@@ -399,14 +399,15 @@
 python setup.py sdist
 ```
 
 To upload to PyPi:
 
 ```bash
 twine upload dist/*
+# twine upload dist/<filename>
 ```
 
 To do both:
     
 ```bash
 python setup.py sdist
 twine upload dist/*
```

### Comparing `model-connect-0.0.5/model_connect.egg-info/SOURCES.txt` & `model-connect-0.0.6/model_connect.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,26 @@
 model_connect/connect.py
 model_connect/constants.py
 model_connect/registry.py
 model_connect.egg-info/PKG-INFO
 model_connect.egg-info/SOURCES.txt
 model_connect.egg-info/dependency_links.txt
 model_connect.egg-info/top_level.txt
+model_connect/globals/__init__.py
+model_connect/globals/connect.py
+model_connect/globals/registry.py
+model_connect/globals/options/__init__.py
+model_connect/globals/options/connect.py
+model_connect/globals/options/fastapi.py
+model_connect/globals/options/psycopg2.py
 model_connect/integrations/__init__.py
 model_connect/integrations/base.py
-model_connect/integrations/registry.py
+model_connect/integrations/connect.py
+model_connect/integrations/type_registry.py
+model_connect/integrations/types.py
 model_connect/integrations/fastapi/__init__.py
 model_connect/integrations/fastapi/router.py
 model_connect/integrations/fastapi/options/__init__.py
 model_connect/integrations/fastapi/options/model.py
 model_connect/integrations/fastapi/options/model_field.py
 model_connect/integrations/json/__init__.py
 model_connect/integrations/json/decoder.py
@@ -30,15 +39,14 @@
 model_connect/integrations/psycopg2/common/streaming.py
 model_connect/integrations/psycopg2/options/__init__.py
 model_connect/integrations/psycopg2/options/model.py
 model_connect/integrations/psycopg2/options/model_field.py
 model_connect/options/__init__.py
 model_connect/options/connect.py
 model_connect/options/global/__init__.py
-model_connect/options/global/global.py
 model_connect/options/model/__init__.py
 model_connect/options/model/model.py
 model_connect/options/model/query_params.py
 model_connect/options/model_field/__init__.py
 model_connect/options/model_field/model_field.py
 model_connect/options/model_field/dtos/__init__.py
 model_connect/options/model_field/dtos/request.py
```

### Comparing `model-connect-0.0.5/setup.py` & `model-connect-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 long_description = Path(__name__).parent / 'README.md'
 long_description = long_description.read_text()
 
 setup(
     name='model-connect',
-    version='0.0.5',
+    version='0.0.6',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(
         include=[
             'model_connect',
             'model_connect.*'
         ],
```

