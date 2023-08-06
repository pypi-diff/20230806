# Comparing `tmp/remotion_lambda-4.0.17.tar.gz` & `tmp/remotion_lambda-4.1.0a12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.17.tar", last modified: Fri Aug  4 15:48:56 2023, max compression
+gzip compressed data, was "remotion_lambda-4.1.0a12.tar", last modified: Sun Aug  6 15:58:27 2023, max compression
```

## Comparing `remotion_lambda-4.0.17.tar` & `remotion_lambda-4.1.0a12.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.161940 remotion_lambda-4.0.17/
--rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/LICENSE
--rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-08-04 15:48:56.161777 remotion_lambda-4.0.17/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/README.md
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.160144 remotion_lambda-4.0.17/remotion_lambda/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/models.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/remotionclient.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-04 15:40:30.000000 remotion_lambda-4.0.17/remotion_lambda/version.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.160929 remotion_lambda-4.0.17/remotion_lambda.egg-info/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-04 15:48:56.161977 remotion_lambda-4.0.17/setup.cfg
--rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/setup.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.161541 remotion_lambda-4.0.17/tests/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/test_get_render_progress_client.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/test_render_client.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870838 remotion_lambda-4.1.0a12/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2023-08-06 15:58:27.870663 remotion_lambda-4.1.0a12/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.869636 remotion_lambda-4.1.0a12/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       91 2023-08-06 15:40:13.000000 remotion_lambda-4.1.0a12/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870149 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      429 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-06 15:58:27.000000 remotion_lambda-4.1.0a12/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-06 15:58:27.870887 remotion_lambda-4.1.0a12/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-06 15:58:27.870482 remotion_lambda-4.1.0a12/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-08-06 15:29:11.000000 remotion_lambda-4.1.0a12/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.17/LICENSE` & `remotion_lambda-4.1.0a12/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.17/remotion_lambda/models.py` & `remotion_lambda-4.1.0a12/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.17/remotion_lambda/remotionclient.py` & `remotion_lambda-4.1.0a12/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.17/setup.py` & `remotion_lambda-4.1.0a12/setup.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.17/tests/test_render_client.py` & `remotion_lambda-4.1.0a12/tests/test_render_client.py`

 * *Files identical despite different names*

