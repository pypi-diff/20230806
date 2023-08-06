# Comparing `tmp/indexpaper-0.0.1.tar.gz` & `tmp/indexpaper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexpaper-0.0.1.tar", last modified: Wed Aug  2 09:27:39 2023, max compression
+gzip compressed data, was "indexpaper-0.0.3.tar", last modified: Sun Aug  6 15:52:50 2023, max compression
```

## Comparing `indexpaper-0.0.1.tar` & `indexpaper-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-02 09:27:39.172589 indexpaper-0.0.1/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2023-07-29 22:10:33.000000 indexpaper-0.0.1/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3299 2023-08-02 09:27:39.172589 indexpaper-0.0.1/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2639 2023-07-29 23:14:58.000000 indexpaper-0.0.1/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-02 09:27:39.172589 indexpaper-0.0.1/indexpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     3299 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      232 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       47 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      146 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-02 09:27:39.000000 indexpaper-0.0.1/indexpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-08-02 09:27:39.172589 indexpaper-0.0.1/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1503 2023-08-02 08:12:46.000000 indexpaper-0.0.1/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-06 15:52:50.535092 indexpaper-0.0.3/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)    11357 2023-07-29 22:10:33.000000 indexpaper-0.0.3/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5838 2023-08-06 15:52:50.535092 indexpaper-0.0.3/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5178 2023-08-06 15:21:25.000000 indexpaper-0.0.3/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-08-06 15:52:50.535092 indexpaper-0.0.3/indexpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     5838 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      232 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       47 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      172 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-08-06 15:52:50.000000 indexpaper-0.0.3/indexpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-08-06 15:52:50.535092 indexpaper-0.0.3/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1538 2023-08-06 14:56:02.000000 indexpaper-0.0.3/setup.py
```

### Comparing `indexpaper-0.0.1/LICENSE` & `indexpaper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indexpaper-0.0.1/setup.py` & `indexpaper-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.3'
 DESCRIPTION = 'indexpaper - library to index papers with vector databases'
 LONG_DESCRIPTION = 'indexpaper - library to index papers with vector databases'
 
 # Setting up
 setup(
     name="indexpaper",
     version=VERSION,
     author="antonkulaga (Anton Kulaga)",
     author_email="<antonkulaga@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['pyfunctional', 'more-itertools', 'click', 'python-dotenv', 'tiktoken',
+    install_requires=['pyfunctional', 'pycomfort', 'more-itertools', 'click', 'python-dotenv', 'tiktoken',
                       'langchain', 'openai', 'Deprecated', 'loguru',
-                      'qdrant-client', 'chromadb', 'sentence_transformers', 'datasets'],
+                      'qdrant-client', 'chromadb', 'sentence_transformers', 'datasets', 'polars', 'beartype'],
     keywords=['python', 'utils', 'files', 'papers', 'download', 'index', 'vector databases'],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
```

