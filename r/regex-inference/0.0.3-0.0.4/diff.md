# Comparing `tmp/regex-inference-0.0.3.tar.gz` & `tmp/regex-inference-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-inference-0.0.3.tar", last modified: Sun Aug  6 01:15:02 2023, max compression
+gzip compressed data, was "regex-inference-0.0.4.tar", last modified: Sun Aug  6 02:51:27 2023, max compression
```

## Comparing `regex-inference-0.0.3.tar` & `regex-inference-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 01:14:43.000000 regex-inference-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:15:02.462707 regex-inference-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 01:14:43.000000 regex-inference-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/cmd/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13729 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/jsonl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/inference/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/inference/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference/schema/objs/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/schema/objs/records.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 01:14:44.000000 regex-inference-0.0.3/regex_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 01:15:02.462707 regex-inference-0.0.3/regex_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 01:15:02.000000 regex-inference-0.0.3/regex_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 01:15:02.462707 regex-inference-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-06 01:14:44.000000 regex-inference-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 02:51:09.000000 regex-inference-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 02:51:27.851202 regex-inference-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 02:51:09.000000 regex-inference-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/inference/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-06 02:51:09.000000 regex-inference-0.0.4/regex_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 02:51:27.851202 regex-inference-0.0.4/regex_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 02:51:27.000000 regex-inference-0.0.4/regex_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 02:51:27.851202 regex-inference-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 02:51:09.000000 regex-inference-0.0.4/setup.py
```

### Comparing `regex-inference-0.0.3/LICENSE` & `regex-inference-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-inference-0.0.3/setup.py` & `regex-inference-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,17 +49,13 @@
 
         "Operating System :: OS Independent",
 
     ],
     python_requires='>=3.7',
     tests_require=['pytest'],
     install_requires=[
-        'openai',
-        'langchain'
-    ],
-    entry_points={
-        'console_scripts': [
-            'regex-inference = \
-        regex_inference.cmd.inference:run',
-        ]
-    }
+        'openapi-schema-pydantic==1.2.4',
+        'pydantic==1.10.12',
+        'openai==0.27.8',
+        'langchain==0.0.253'
+    ]
 )
```

