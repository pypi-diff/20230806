# Comparing `tmp/regex-inference-0.0.5.tar.gz` & `tmp/regex-inference-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-inference-0.0.5.tar", last modified: Sun Aug  6 04:13:07 2023, max compression
+gzip compressed data, was "regex-inference-0.0.6.tar", last modified: Sun Aug  6 06:42:40 2023, max compression
```

## Comparing `regex-inference-0.0.5.tar` & `regex-inference-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 04:12:48.000000 regex-inference-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 04:13:07.333952 regex-inference-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 04:12:48.000000 regex-inference-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.329952 regex-inference-0.0.5/regex_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/regex_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/inference/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 04:12:48.000000 regex-inference-0.0.5/regex_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:13:07.333952 regex-inference-0.0.5/regex_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 04:13:07.000000 regex-inference-0.0.5/regex_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 04:13:07.333952 regex-inference-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 04:12:48.000000 regex-inference-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:42:40.264477 regex-inference-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 06:42:22.000000 regex-inference-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 06:42:40.264477 regex-inference-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 06:42:22.000000 regex-inference-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:42:40.260477 regex-inference-0.0.6/regex_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 06:42:22.000000 regex-inference-0.0.6/regex_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:42:40.264477 regex-inference-0.0.6/regex_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 06:42:22.000000 regex-inference-0.0.6/regex_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-08-06 06:42:22.000000 regex-inference-0.0.6/regex_inference/inference/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 06:42:22.000000 regex-inference-0.0.6/regex_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 06:42:40.260477 regex-inference-0.0.6/regex_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 06:42:40.000000 regex-inference-0.0.6/regex_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 06:42:40.000000 regex-inference-0.0.6/regex_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 06:42:40.000000 regex-inference-0.0.6/regex_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 06:42:40.000000 regex-inference-0.0.6/regex_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 06:42:40.000000 regex-inference-0.0.6/regex_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 06:42:40.264477 regex-inference-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 06:42:22.000000 regex-inference-0.0.6/setup.py
```

### Comparing `regex-inference-0.0.5/LICENSE` & `regex-inference-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.5/regex_inference/inference/engine.py` & `regex-inference-0.0.6/regex_inference/inference/engine.py`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.5/setup.py` & `regex-inference-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "Programming Language :: Python :: 3",
 
         "License :: OSI Approved :: MIT License",
 
         "Operating System :: OS Independent",
 
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     tests_require=['pytest'],
     install_requires=[
         'openapi-schema-pydantic==1.2.4',
         'pydantic==1.10.12',
         'openai==0.27.8',
         'langchain==0.0.253'
     ]
```

