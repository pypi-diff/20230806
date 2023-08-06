# Comparing `tmp/betabageldb-0.2.2.tar.gz` & `tmp/betabageldb-0.2.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.2.2.tar", last modified: Sun Aug  6 16:42:16 2023, max compression
+gzip compressed data, was "betabageldb-0.2.31.tar", last modified: Sun Aug  6 18:50:55 2023, max compression
```

## Comparing `betabageldb-0.2.2.tar` & `betabageldb-0.2.31.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 16:42:16.296072 betabageldb-0.2.2/
--rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-08-06 16:42:16.295875 betabageldb-0.2.2/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     2643 2023-07-26 14:55:22.000000 betabageldb-0.2.2/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 16:42:16.287760 betabageldb-0.2.2/bagel/
--rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.2.2/bagel/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 16:42:16.290536 betabageldb-0.2.2/bagel/api/
--rw-r--r--   0 bidhan     (501) staff       (20)    13827 2023-07-24 20:40:18.000000 betabageldb-0.2.2/bagel/api/Cluster.py
--rw-r--r--   0 bidhan     (501) staff       (20)    10713 2023-08-01 18:29:23.000000 betabageldb-0.2.2/bagel/api/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    12194 2023-08-01 18:29:23.000000 betabageldb-0.2.2/bagel/api/fastapi.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.2.2/bagel/api/types.py
--rw-r--r--   0 bidhan     (501) staff       (20)     5926 2023-08-01 18:29:40.000000 betabageldb-0.2.2/bagel/config.py
--rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.2.2/bagel/errors.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 16:42:16.291182 betabageldb-0.2.2/bagel/utils/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.2.2/bagel/utils/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 16:42:16.295442 betabageldb-0.2.2/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-08-06 16:42:16.000000 betabageldb-0.2.2/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      349 2023-08-06 16:42:16.000000 betabageldb-0.2.2/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-08-06 16:42:16.000000 betabageldb-0.2.2/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      472 2023-08-06 16:42:16.000000 betabageldb-0.2.2/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-08-06 16:42:16.000000 betabageldb-0.2.2/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-08-06 16:42:16.296109 betabageldb-0.2.2/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1524 2023-08-06 16:41:50.000000 betabageldb-0.2.2/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 18:50:55.073460 betabageldb-0.2.31/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3198 2023-08-06 18:50:55.073253 betabageldb-0.2.31/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     2643 2023-07-26 14:55:22.000000 betabageldb-0.2.31/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 18:50:55.060321 betabageldb-0.2.31/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.2.31/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 18:50:55.067269 betabageldb-0.2.31/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    13827 2023-07-24 20:40:18.000000 betabageldb-0.2.31/bagel/api/Cluster.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    10713 2023-08-01 18:29:23.000000 betabageldb-0.2.31/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    12194 2023-08-01 18:29:23.000000 betabageldb-0.2.31/bagel/api/fastapi.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.2.31/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     5926 2023-08-01 18:29:40.000000 betabageldb-0.2.31/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.2.31/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 18:50:55.068549 betabageldb-0.2.31/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.2.31/bagel/utils/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-08-06 18:50:55.072910 betabageldb-0.2.31/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3198 2023-08-06 18:50:55.000000 betabageldb-0.2.31/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      349 2023-08-06 18:50:55.000000 betabageldb-0.2.31/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-08-06 18:50:55.000000 betabageldb-0.2.31/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      264 2023-08-06 18:50:55.000000 betabageldb-0.2.31/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-08-06 18:50:55.000000 betabageldb-0.2.31/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-08-06 18:50:55.073501 betabageldb-0.2.31/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1185 2023-08-06 18:46:14.000000 betabageldb-0.2.31/setup.py
```

### Comparing `betabageldb-0.2.2/PKG-INFO` & `betabageldb-0.2.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.2.2
+Version: 0.2.31
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.2.2/README.md` & `betabageldb-0.2.31/README.md`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/__init__.py` & `betabageldb-0.2.31/bagel/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/api/Cluster.py` & `betabageldb-0.2.31/bagel/api/Cluster.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/api/__init__.py` & `betabageldb-0.2.31/bagel/api/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/api/fastapi.py` & `betabageldb-0.2.31/bagel/api/fastapi.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/api/types.py` & `betabageldb-0.2.31/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/config.py` & `betabageldb-0.2.31/bagel/config.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/bagel/errors.py` & `betabageldb-0.2.31/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.2.2/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.2.31/betabageldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.2.2
+Version: 0.2.31
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betabageldb-0.2.2/setup.py` & `betabageldb-0.2.31/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.2.2",
+    version="0.2.31",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     packages=find_packages(),
     install_requires=[
-        "annotated-types==0.5.0",
-        "backoff==2.2.1",
         "certifi==2023.5.7",
         "charset-normalizer==3.2.0",
-        "flatbuffers==23.5.26",
         "graphlib-backport==1.0.3",
-        "humanfriendly==10.0",
         "idna==3.4",
-        "monotonic==1.6",
-        "mpmath==1.3.0",
-        "numpy==1.25.2",
+        "numpy==1.21.6",
         "overrides==7.3.1",
-        "packaging==23.1",
-        "pandas==2.0.3",
+        "pandas==2.0.1",
         "pydantic==1.10.10",
-        "pydantic_core==2.1.2",
-        "pyreadline3==3.4.1",
         "python-dateutil==2.8.2",
         "pytz==2023.3",
         "requests==2.28.2",
         "six==1.16.0",
-        "sympy==1.12",
-        "tokenizers==0.13.3",
-        "tqdm==4.65.0",
-        "typing_extensions==4.6.3",
-        "tzdata==2023.3",
-        "urllib3==1.26.16"
+        "typing-extensions==4.6.3",
+        "urllib3==1.26.16",
+        "tzdata>=2022.1"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

