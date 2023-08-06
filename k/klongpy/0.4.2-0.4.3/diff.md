# Comparing `tmp/klongpy-0.4.2.tar.gz` & `tmp/klongpy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.4.2.tar", last modified: Wed Jul 26 22:46:24 2023, max compression
+gzip compressed data, was "klongpy-0.4.3.tar", last modified: Sun Aug  6 01:46:01 2023, max compression
```

## Comparing `klongpy-0.4.2.tar` & `klongpy-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.2/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    23130 2023-07-26 22:46:24.901210 klongpy-0.4.2/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    22576 2023-07-26 22:46:02.000000 klongpy-0.4.2/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.2/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    26246 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20565 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.2/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16745 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/sys_fn_ipc.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3089 2023-07-26 22:46:02.000000 klongpy-0.4.2/klongpy/sys_fn_timer.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.2/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy/web/
--rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.2/klongpy/web/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4947 2023-07-24 23:20:23.000000 klongpy-0.4.2/klongpy/web/sys_fn_web.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    23130 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      711 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-26 22:46:24.000000 klongpy-0.4.2/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.2/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-26 22:46:24.901210 klongpy-0.4.2/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-26 22:46:02.000000 klongpy-0.4.2/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-26 22:46:24.901210 klongpy-0.4.2/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.2/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.2/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3196 2023-07-26 22:46:02.000000 klongpy-0.4.2/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.2/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.2/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.2/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.2/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.3/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26611 2023-08-06 01:46:01.993903 klongpy-0.4.3/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26038 2023-08-06 01:44:41.000000 klongpy-0.4.3/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.3/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.3/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.3/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26290 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/core.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/klongpy/db/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      276 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3325 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/df_cache.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     9294 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/file_cache.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1299 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/helpers.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     8711 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/sys_fn_db.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3775 2023-08-06 01:44:41.000000 klongpy-0.4.3/klongpy/db/sys_fn_kvs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.3/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20565 2023-07-26 22:46:02.000000 klongpy-0.4.3/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.3/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.3/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16745 2023-07-26 22:46:02.000000 klongpy-0.4.3/klongpy/sys_fn_ipc.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3089 2023-07-26 22:46:02.000000 klongpy-0.4.3/klongpy/sys_fn_timer.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.3/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.3/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/klongpy/web/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.3/klongpy/web/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4947 2023-07-24 23:20:23.000000 klongpy-0.4.3/klongpy/web/sys_fn_web.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26611 2023-08-06 01:46:01.000000 klongpy-0.4.3/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      853 2023-08-06 01:46:01.000000 klongpy-0.4.3/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-08-06 01:46:01.000000 klongpy-0.4.3/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      251 2023-08-06 01:46:01.000000 klongpy-0.4.3/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-08-06 01:46:01.000000 klongpy-0.4.3/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7573 2023-08-06 01:44:41.000000 klongpy-0.4.3/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-08-06 01:46:01.993903 klongpy-0.4.3/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1186 2023-08-06 01:44:41.000000 klongpy-0.4.3/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-08-06 01:46:01.993903 klongpy-0.4.3/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.3/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      783 2023-08-06 01:44:41.000000 klongpy-0.4.3/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    24477 2023-08-06 01:44:41.000000 klongpy-0.4.3/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1823 2023-08-06 01:44:41.000000 klongpy-0.4.3/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3196 2023-07-26 22:46:02.000000 klongpy-0.4.3/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3682 2023-08-06 01:44:41.000000 klongpy-0.4.3/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.3/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.3/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4371 2023-08-06 01:44:41.000000 klongpy-0.4.3/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.3/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.3/tests/test_util.py
```

### Comparing `klongpy-0.4.2/LICENSE` & `klongpy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/PKG-INFO` & `klongpy-0.4.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Provides-Extra: cuda111
 Provides-Extra: cuda110
 Provides-Extra: cuda102
 Provides-Extra: rocm-5-0
 Provides-Extra: rocm-4-3
 Provides-Extra: repl
 Provides-Extra: web
+Provides-Extra: db
 License-File: LICENSE
 
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
 
@@ -34,20 +35,22 @@
 The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
 # Overview
 
 KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
 * __Simplicity__: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
-* __Speed__: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
-* __Inter-Process Communication (IPC)__: KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
 * __Array Programming__: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
-* __Compatibility__: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
-* __Web server__: Includes a web server, making it easy to build sites backed by KlongPy capabilities.
-* __Timers__: Includes periodic timer facility to periodically perform tasks.
+* [__Speed__](#performance): KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* [__Fast Columnar Database__](#fast-columnar-database): Includes integration with DuckDb, a super fast in-process columnar store that can operate directly on NumPy arrays w/ zero-copy.
+* [__Table and Key-Value Store__](#table-and-key-value-stores): Includes a simple file-backed key value store that can be used to store database tables or raw key/value pairs.
+* [__Inter-Process Communication (IPC)__](#inter-process-communication-ipc-capabilities): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* [__Compatibility__](#python-integration): KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* [__Web server__](#web-server): Includes a web server, making it easy to build sites backed by KlongPy capabilities.
+* [__Timers__](#timer): Includes periodic timer facility to periodically perform tasks.
 
 At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
 Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
 Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
 
@@ -305,34 +308,176 @@
 
 ?> .py("tests/plugins/greetings")
 1
 ?> hello()
 world!
 ```
 
+# Fast Columnar Database 
 
-# Pandas DataFrame integration
+KlongPy provides a module "klongpy.db" that includes DuckDb integration.  DuckDb can operate directly on NumPy arrays, which allows for zero-copy SQL execution over pre-existing NumPy data.
 
-This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
+## Tables
 
-For now, the following works where we convert a DataFrame into a dictionary of columns:
+```
+?> .py("klongpy.db")
+?> t::.table([["a" [1 2 3]] ["b" [2 3 4]]])
+a b
+1 2
+2 3
+3 4
+?> t,"c",,[3 4 5]
+a b c
+1 2 3
+2 3 4
+3 4 5
+```
+
+Indexes (one or more columns) can be created on a table.  The current indexes can be seen in the table discription prefix.
+
+```
+?> .index(t; ["a"])
+['a']
+```
+
+When a column is indexed, it appears with an asterisk in the pretty-print format:
+
+```
+?> t
+a* b
+ 1 2
+ 2 3
+ 3 5
+```
+
+Inserting a row with a pre-existing value at an index results in an update:
+
+```
+?> .insert(t, [3 5 6])
+a* b c
+ 1 2 3
+ 2 3 4
+ 3 5 6
+```
+
+Indexes may be reset via .rindex().  True is returned if the index was reset.
+
+```
+?> .rindex(t)
+1
+```
+
+## Database
+
+Databases are created from a map of table names to table instances.  A database instance is a function which accepts SQL and runs it over the underlying tables.  SQL results are NumPy arrays and can be directly used in normal KlongPy operations.
+
+```
+?> T::.table(,"a",,[1 2 3])
+a
+1
+2
+3
+?> db::.db(:{},"T",,T)
+:db
+?> db("select * from T")
+[1 2 3]
+```
+
+Since KlongPy uses DuckDb under the hood, you can perform sophisticated SQL over the underlying NumPy arrays.  
+
+For example, it's easy to use JOIN with this setup:
+
+```
+d::[]
+d::d,,"a",,[1 2 3]
+d::d,,"b",,[2 3 4]
+T::.table(d)
+
+e::,"c",,[3 4 5]
+G::.table(e)
+
+q:::{}
+q,"T",,T
+q,"G",,G
+db::.db(q)
+```
+
+We can now issue a JOIN SQL:
+
+```
+?> db("select * from T join G on G.c = T.b")
+[[2 3 3]
+ [3 4 4]]
+```
+
+## Pandas DataFrame integration
+
+Tables are backed by Pandas DataFrames, so it's easy to integrate Pandas directly into KlongPy via DuckDb.
 
 ```Python
 from klongpy import KlongInterpreter
 import pandas as pd
-import numpy as np
 
 data = {'Name': ['Alice', 'Bob', 'Charlie', 'David'],
         'Age': [25, 30, 35, 40]}
 df = pd.DataFrame(data)
 
 klong = KlongInterpreter()
-klong['df'] = {col: np.array(df[col]) for col in df.columns}
-klong('df?"Name"') # ==> ['Alice', 'Bob', 'Charlie', 'David']
-klong('df?"Age"')  # ==> [25, 30, 35, 40]
+klong['df'] = df
+r = klong("""
+.py("klongpy.db")
+t::.table(df)
+db::.db(:{},"people",t)
+db("select Age from people")
+""")
+```
+
+# Table and Key-Value Stores
+
+To support the KlongPy database cababilities, the klongpy.db module includes a key-value store capability that allows for saving and retreiving tables from disk.  There is a more generic key-value store as well as a TableStore.  The TableStore merges tables when writing to disk, while the generic key-value store writes raw serialized data and doesn't consider the contents.
+
+Key-value stores operate as dictionaries, so setting a value updates the contents on disk and reading a value retrieves it.  Similar to Klong dictionaries, if the value does not exist, then the undefined value is returned.
+
+### TableStore
+
+Since KlongPy Tables are backed by Pandas DataFrames, it's convenient to be able to save/load them from disk.  For this we use the .tables() command.  If table is already present on disk, then the set results in the merge of the two DataFrames.
+
+Let's consider that we have a table called 'prices' and we want to store it on disk.
+
+```
+?> tbs::.tables("/tmp/tables")
+/tmp/tables:tables
+?> tbs,"prices",prices
+/tmp/tables:tables
+```
+
+Similarly, reading values is the same as getting a value from a dict:
+
+```
+?> prices::tbs?"prices"
+```
+
+### Generic key-value store
+
+A simple key-value store backed by disk is available via the .kvs() command.
+
+```
+?> kvs::.kvs("/tmp/kvs")
+/tmp/kvs:kvs
+?> kvs,"hello",,"world"
+/tmp/kvs:kvs
+```
+
+Now a file /tmp/kvs/hello exists with a pickled instance of "hello".
+
+Retrieving a value is the same as reading from a dictionary:
+
+```
+?> kvs?"hello"
+world
 ```
 
 # Inter-Process Communication (IPC) Capabilities
 
 KlongPy has powerful Inter-Process Communication (IPC) features that enable it to connect and interact with remote KlongPy instances. This includes executing commands, retrieving or storing data, and even defining functions remotely. These new capabilities are available via two new functions: .cli() and .clid().
 
 ## The .cli() Function
```

### Comparing `klongpy-0.4.2/README.md` & `klongpy-0.4.3/klongpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: klongpy
+Version: 0.4.3
+Summary: Python implementation of Klong language.
+Author: Brian Guarraci
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: cupy
+Provides-Extra: cuda12x
+Provides-Extra: cuda11x
+Provides-Extra: cuda111
+Provides-Extra: cuda110
+Provides-Extra: cuda102
+Provides-Extra: rocm-5-0
+Provides-Extra: rocm-4-3
+Provides-Extra: repl
+Provides-Extra: web
+Provides-Extra: db
+License-File: LICENSE
+
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
 
 If you're intrigued by the world of [array languages](https://en.wikipedia.org/wiki/Array_programming) and love Python's versatility, meet KlongPy. This project marries the two, bringing Klong's elegant, terse syntax and the computational power of array programming to Python.
 
@@ -12,20 +35,22 @@
 The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
 # Overview
 
 KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
 * __Simplicity__: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
-* __Speed__: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
-* __Inter-Process Communication (IPC)__: KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
 * __Array Programming__: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
-* __Compatibility__: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
-* __Web server__: Includes a web server, making it easy to build sites backed by KlongPy capabilities.
-* __Timers__: Includes periodic timer facility to periodically perform tasks.
+* [__Speed__](#performance): KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* [__Fast Columnar Database__](#fast-columnar-database): Includes integration with DuckDb, a super fast in-process columnar store that can operate directly on NumPy arrays w/ zero-copy.
+* [__Table and Key-Value Store__](#table-and-key-value-stores): Includes a simple file-backed key value store that can be used to store database tables or raw key/value pairs.
+* [__Inter-Process Communication (IPC)__](#inter-process-communication-ipc-capabilities): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* [__Compatibility__](#python-integration): KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* [__Web server__](#web-server): Includes a web server, making it easy to build sites backed by KlongPy capabilities.
+* [__Timers__](#timer): Includes periodic timer facility to periodically perform tasks.
 
 At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
 Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
 Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
 
@@ -283,34 +308,176 @@
 
 ?> .py("tests/plugins/greetings")
 1
 ?> hello()
 world!
 ```
 
+# Fast Columnar Database 
+
+KlongPy provides a module "klongpy.db" that includes DuckDb integration.  DuckDb can operate directly on NumPy arrays, which allows for zero-copy SQL execution over pre-existing NumPy data.
+
+## Tables
+
+```
+?> .py("klongpy.db")
+?> t::.table([["a" [1 2 3]] ["b" [2 3 4]]])
+a b
+1 2
+2 3
+3 4
+?> t,"c",,[3 4 5]
+a b c
+1 2 3
+2 3 4
+3 4 5
+```
+
+Indexes (one or more columns) can be created on a table.  The current indexes can be seen in the table discription prefix.
+
+```
+?> .index(t; ["a"])
+['a']
+```
+
+When a column is indexed, it appears with an asterisk in the pretty-print format:
+
+```
+?> t
+a* b
+ 1 2
+ 2 3
+ 3 5
+```
+
+Inserting a row with a pre-existing value at an index results in an update:
+
+```
+?> .insert(t, [3 5 6])
+a* b c
+ 1 2 3
+ 2 3 4
+ 3 5 6
+```
+
+Indexes may be reset via .rindex().  True is returned if the index was reset.
+
+```
+?> .rindex(t)
+1
+```
+
+## Database
 
-# Pandas DataFrame integration
+Databases are created from a map of table names to table instances.  A database instance is a function which accepts SQL and runs it over the underlying tables.  SQL results are NumPy arrays and can be directly used in normal KlongPy operations.
 
-This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
+```
+?> T::.table(,"a",,[1 2 3])
+a
+1
+2
+3
+?> db::.db(:{},"T",,T)
+:db
+?> db("select * from T")
+[1 2 3]
+```
+
+Since KlongPy uses DuckDb under the hood, you can perform sophisticated SQL over the underlying NumPy arrays.  
 
-For now, the following works where we convert a DataFrame into a dictionary of columns:
+For example, it's easy to use JOIN with this setup:
+
+```
+d::[]
+d::d,,"a",,[1 2 3]
+d::d,,"b",,[2 3 4]
+T::.table(d)
+
+e::,"c",,[3 4 5]
+G::.table(e)
+
+q:::{}
+q,"T",,T
+q,"G",,G
+db::.db(q)
+```
+
+We can now issue a JOIN SQL:
+
+```
+?> db("select * from T join G on G.c = T.b")
+[[2 3 3]
+ [3 4 4]]
+```
+
+## Pandas DataFrame integration
+
+Tables are backed by Pandas DataFrames, so it's easy to integrate Pandas directly into KlongPy via DuckDb.
 
 ```Python
 from klongpy import KlongInterpreter
 import pandas as pd
-import numpy as np
 
 data = {'Name': ['Alice', 'Bob', 'Charlie', 'David'],
         'Age': [25, 30, 35, 40]}
 df = pd.DataFrame(data)
 
 klong = KlongInterpreter()
-klong['df'] = {col: np.array(df[col]) for col in df.columns}
-klong('df?"Name"') # ==> ['Alice', 'Bob', 'Charlie', 'David']
-klong('df?"Age"')  # ==> [25, 30, 35, 40]
+klong['df'] = df
+r = klong("""
+.py("klongpy.db")
+t::.table(df)
+db::.db(:{},"people",t)
+db("select Age from people")
+""")
+```
+
+# Table and Key-Value Stores
+
+To support the KlongPy database cababilities, the klongpy.db module includes a key-value store capability that allows for saving and retreiving tables from disk.  There is a more generic key-value store as well as a TableStore.  The TableStore merges tables when writing to disk, while the generic key-value store writes raw serialized data and doesn't consider the contents.
+
+Key-value stores operate as dictionaries, so setting a value updates the contents on disk and reading a value retrieves it.  Similar to Klong dictionaries, if the value does not exist, then the undefined value is returned.
+
+### TableStore
+
+Since KlongPy Tables are backed by Pandas DataFrames, it's convenient to be able to save/load them from disk.  For this we use the .tables() command.  If table is already present on disk, then the set results in the merge of the two DataFrames.
+
+Let's consider that we have a table called 'prices' and we want to store it on disk.
+
+```
+?> tbs::.tables("/tmp/tables")
+/tmp/tables:tables
+?> tbs,"prices",prices
+/tmp/tables:tables
+```
+
+Similarly, reading values is the same as getting a value from a dict:
+
+```
+?> prices::tbs?"prices"
+```
+
+### Generic key-value store
+
+A simple key-value store backed by disk is available via the .kvs() command.
+
+```
+?> kvs::.kvs("/tmp/kvs")
+/tmp/kvs:kvs
+?> kvs,"hello",,"world"
+/tmp/kvs:kvs
+```
+
+Now a file /tmp/kvs/hello exists with a pickled instance of "hello".
+
+Retrieving a value is the same as reading from a dictionary:
+
+```
+?> kvs?"hello"
+world
 ```
 
 # Inter-Process Communication (IPC) Capabilities
 
 KlongPy has powerful Inter-Process Communication (IPC) features that enable it to connect and interact with remote KlongPy instances. This includes executing commands, retrieving or storing data, and even defining functions remotely. These new capabilities are available via two new functions: .cli() and .clid().
 
 ## The .cli() Function
```

### Comparing `klongpy-0.4.2/klongpy/adverbs.py` & `klongpy-0.4.3/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/backend.py` & `klongpy-0.4.3/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/core.py` & `klongpy-0.4.3/klongpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from .backend import np
 
 # python3.11 support
 if not hasattr(inspect, 'getargspec'):
     inspect.getargspec = inspect.getfullargspec
 
 
+class KlongException(Exception):
+    pass
+
+
 class KGSym(str):
     def __repr__(self):
         return f":{super().__str__()}"
     def __eq__(self, o):
         return isinstance(o,KGSym) and self.__str__() == o.__str__()
     def __hash__(self):
         return super().__hash__()
```

### Comparing `klongpy-0.4.2/klongpy/dyads.py` & `klongpy-0.4.3/klongpy/dyads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/interpreter.py` & `klongpy-0.4.3/klongpy/interpreter.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/monads.py` & `klongpy-0.4.3/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/sys_fn.py` & `klongpy-0.4.3/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/sys_fn_ipc.py` & `klongpy-0.4.3/klongpy/sys_fn_ipc.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/sys_fn_timer.py` & `klongpy-0.4.3/klongpy/sys_fn_timer.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/sys_var.py` & `klongpy-0.4.3/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/utils.py` & `klongpy-0.4.3/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy/web/sys_fn_web.py` & `klongpy-0.4.3/klongpy/web/sys_fn_web.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/klongpy.egg-info/PKG-INFO` & `klongpy-0.4.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: klongpy
-Version: 0.4.2
-Summary: Python implementation of Klong language.
-Author: Brian Guarraci
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cupy
-Provides-Extra: cuda12x
-Provides-Extra: cuda11x
-Provides-Extra: cuda111
-Provides-Extra: cuda110
-Provides-Extra: cuda102
-Provides-Extra: rocm-5-0
-Provides-Extra: rocm-4-3
-Provides-Extra: repl
-Provides-Extra: web
-License-File: LICENSE
-
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
 
 If you're intrigued by the world of [array languages](https://en.wikipedia.org/wiki/Array_programming) and love Python's versatility, meet KlongPy. This project marries the two, bringing Klong's elegant, terse syntax and the computational power of array programming to Python.
 
@@ -34,20 +12,22 @@
 The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
 # Overview
 
 KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
 * __Simplicity__: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
-* __Speed__: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
-* __Inter-Process Communication (IPC)__: KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
 * __Array Programming__: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
-* __Compatibility__: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
-* __Web server__: Includes a web server, making it easy to build sites backed by KlongPy capabilities.
-* __Timers__: Includes periodic timer facility to periodically perform tasks.
+* [__Speed__](#performance): KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* [__Fast Columnar Database__](#fast-columnar-database): Includes integration with DuckDb, a super fast in-process columnar store that can operate directly on NumPy arrays w/ zero-copy.
+* [__Table and Key-Value Store__](#table-and-key-value-stores): Includes a simple file-backed key value store that can be used to store database tables or raw key/value pairs.
+* [__Inter-Process Communication (IPC)__](#inter-process-communication-ipc-capabilities): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* [__Compatibility__](#python-integration): KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* [__Web server__](#web-server): Includes a web server, making it easy to build sites backed by KlongPy capabilities.
+* [__Timers__](#timer): Includes periodic timer facility to periodically perform tasks.
 
 At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
 Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
 Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
 
@@ -305,34 +285,176 @@
 
 ?> .py("tests/plugins/greetings")
 1
 ?> hello()
 world!
 ```
 
+# Fast Columnar Database 
+
+KlongPy provides a module "klongpy.db" that includes DuckDb integration.  DuckDb can operate directly on NumPy arrays, which allows for zero-copy SQL execution over pre-existing NumPy data.
+
+## Tables
+
+```
+?> .py("klongpy.db")
+?> t::.table([["a" [1 2 3]] ["b" [2 3 4]]])
+a b
+1 2
+2 3
+3 4
+?> t,"c",,[3 4 5]
+a b c
+1 2 3
+2 3 4
+3 4 5
+```
+
+Indexes (one or more columns) can be created on a table.  The current indexes can be seen in the table discription prefix.
+
+```
+?> .index(t; ["a"])
+['a']
+```
+
+When a column is indexed, it appears with an asterisk in the pretty-print format:
+
+```
+?> t
+a* b
+ 1 2
+ 2 3
+ 3 5
+```
+
+Inserting a row with a pre-existing value at an index results in an update:
+
+```
+?> .insert(t, [3 5 6])
+a* b c
+ 1 2 3
+ 2 3 4
+ 3 5 6
+```
+
+Indexes may be reset via .rindex().  True is returned if the index was reset.
+
+```
+?> .rindex(t)
+1
+```
+
+## Database
 
-# Pandas DataFrame integration
+Databases are created from a map of table names to table instances.  A database instance is a function which accepts SQL and runs it over the underlying tables.  SQL results are NumPy arrays and can be directly used in normal KlongPy operations.
 
-This a work in progress, but it's very interesting to think about what DataFrames look like in Klong since they are basically a dictionary of columns.
+```
+?> T::.table(,"a",,[1 2 3])
+a
+1
+2
+3
+?> db::.db(:{},"T",,T)
+:db
+?> db("select * from T")
+[1 2 3]
+```
+
+Since KlongPy uses DuckDb under the hood, you can perform sophisticated SQL over the underlying NumPy arrays.  
 
-For now, the following works where we convert a DataFrame into a dictionary of columns:
+For example, it's easy to use JOIN with this setup:
+
+```
+d::[]
+d::d,,"a",,[1 2 3]
+d::d,,"b",,[2 3 4]
+T::.table(d)
+
+e::,"c",,[3 4 5]
+G::.table(e)
+
+q:::{}
+q,"T",,T
+q,"G",,G
+db::.db(q)
+```
+
+We can now issue a JOIN SQL:
+
+```
+?> db("select * from T join G on G.c = T.b")
+[[2 3 3]
+ [3 4 4]]
+```
+
+## Pandas DataFrame integration
+
+Tables are backed by Pandas DataFrames, so it's easy to integrate Pandas directly into KlongPy via DuckDb.
 
 ```Python
 from klongpy import KlongInterpreter
 import pandas as pd
-import numpy as np
 
 data = {'Name': ['Alice', 'Bob', 'Charlie', 'David'],
         'Age': [25, 30, 35, 40]}
 df = pd.DataFrame(data)
 
 klong = KlongInterpreter()
-klong['df'] = {col: np.array(df[col]) for col in df.columns}
-klong('df?"Name"') # ==> ['Alice', 'Bob', 'Charlie', 'David']
-klong('df?"Age"')  # ==> [25, 30, 35, 40]
+klong['df'] = df
+r = klong("""
+.py("klongpy.db")
+t::.table(df)
+db::.db(:{},"people",t)
+db("select Age from people")
+""")
+```
+
+# Table and Key-Value Stores
+
+To support the KlongPy database cababilities, the klongpy.db module includes a key-value store capability that allows for saving and retreiving tables from disk.  There is a more generic key-value store as well as a TableStore.  The TableStore merges tables when writing to disk, while the generic key-value store writes raw serialized data and doesn't consider the contents.
+
+Key-value stores operate as dictionaries, so setting a value updates the contents on disk and reading a value retrieves it.  Similar to Klong dictionaries, if the value does not exist, then the undefined value is returned.
+
+### TableStore
+
+Since KlongPy Tables are backed by Pandas DataFrames, it's convenient to be able to save/load them from disk.  For this we use the .tables() command.  If table is already present on disk, then the set results in the merge of the two DataFrames.
+
+Let's consider that we have a table called 'prices' and we want to store it on disk.
+
+```
+?> tbs::.tables("/tmp/tables")
+/tmp/tables:tables
+?> tbs,"prices",prices
+/tmp/tables:tables
+```
+
+Similarly, reading values is the same as getting a value from a dict:
+
+```
+?> prices::tbs?"prices"
+```
+
+### Generic key-value store
+
+A simple key-value store backed by disk is available via the .kvs() command.
+
+```
+?> kvs::.kvs("/tmp/kvs")
+/tmp/kvs:kvs
+?> kvs,"hello",,"world"
+/tmp/kvs:kvs
+```
+
+Now a file /tmp/kvs/hello exists with a pickled instance of "hello".
+
+Retrieving a value is the same as reading from a dictionary:
+
+```
+?> kvs?"hello"
+world
 ```
 
 # Inter-Process Communication (IPC) Capabilities
 
 KlongPy has powerful Inter-Process Communication (IPC) features that enable it to connect and interact with remote KlongPy instances. This includes executing commands, retrieving or storing data, and even defining functions remotely. These new capabilities are available via two new functions: .cli() and .clid().
 
 ## The .cli() Function
```

### Comparing `klongpy-0.4.2/klongpy.egg-info/SOURCES.txt` & `klongpy-0.4.3/klongpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 klongpy/sys_var.py
 klongpy/utils.py
 klongpy.egg-info/PKG-INFO
 klongpy.egg-info/SOURCES.txt
 klongpy.egg-info/dependency_links.txt
 klongpy.egg-info/requires.txt
 klongpy.egg-info/top_level.txt
+klongpy/db/__init__.py
+klongpy/db/df_cache.py
+klongpy/db/file_cache.py
+klongpy/db/helpers.py
+klongpy/db/sys_fn_db.py
+klongpy/db/sys_fn_kvs.py
 klongpy/web/__init__.py
 klongpy/web/sys_fn_web.py
 scripts/kgpy
 tests/test_accel.py
 tests/test_examples.py
 tests/test_extra_suite.py
 tests/test_fn.py
```

### Comparing `klongpy-0.4.2/scripts/kgpy` & `klongpy-0.4.3/scripts/kgpy`

 * *Files 5% similar despite different names*

```diff
@@ -261,16 +261,20 @@
                 klong(x)
     
     if args.filename:
         run_file(args.filename)
     else:
         run_repl = True
 
+    tasks = asyncio.all_tasks(loop=loop)
+
     if run_repl:
         if args.load:
             print(f"Loading: {args.load}")
             with open(args.load, "r") as f:
                 klong(f.read())
         colorama.init(autoreset=True)
         show_repl_header(args.server)
         loop.create_task(ConsoleInputHandler.input_producer(loop, klong, args.verbose))
+
+    if asyncio.all_tasks(loop=loop):
         loop.run_forever()
```

### Comparing `klongpy-0.4.2/setup.py` & `klongpy-0.4.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
-    packages=['klongpy', 'klongpy.web'],
-    version='0.4.2',
+    packages=['klongpy', 'klongpy.web', 'klongpy.db'],
+    version='0.4.3',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -27,13 +27,14 @@
         'cuda11x': ["cupy-cuda11x"],
         'cuda111': ["cupy-cuda111"],
         'cuda110': ["cupy-cuda110"],
         'cuda102': ["cupy-cuda102"],
         'rocm-5-0': ["cupy-rocm-5-0"],
         'rocm-4-3': ["cupy-rocm-4-3"],
         'repl': ["colorama"],
-        'web': ["aiohttp"]
+        'web': ["aiohttp"],
+        'db': ["pandas","duckdb"],
     },
     include_package_data=True,
     test_suite='tests',
     scripts=['scripts/kgpy']
 )
```

### Comparing `klongpy-0.4.2/tests/test_accel.py` & `klongpy-0.4.3/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/tests/test_extra_suite.py` & `klongpy-0.4.3/tests/test_extra_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
     @unittest.skip
+    def test_fail_non_terminated_string(self):
+        klong = KlongInterpreter()
+        with self.assertRaises(Exception):
+            klong('a::"T')
+
+    @unittest.skip
+    def test_define_nilad_with_subcall(self):
+        klong = KlongInterpreter()
+        klong("nt::{x}")
+        klong('newt::{nt([["1" 2] ["3" 4] ["5" 6]])}')
+
+    @unittest.skip
     def test_join_two_dict(self):
         klong = KlongInterpreter()
         klong("b:::{[1 2]}")
         klong("c:::{[3 4]}")
         r = klong("b,c")
         self.assertEqual(r, {1: 2, 3: 4})
```

### Comparing `klongpy-0.4.2/tests/test_fn.py` & `klongpy-0.4.3/tests/test_fn.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,22 +52,12 @@
 
     def test_nested_x_scope_dyad_projection(self):
         klong = KlongInterpreter()
         klong('UM::{x;y};G::UM("A";);F::{G(4_x)}')
         r = klong('F("hello")')
         self.assertEqual(r, "o")
 
-    def test_fn_gen(self):
-        """
-        Test the entire suite file.
-        """
-        klong = KlongInterpreter()
-        with open("tests/klong_fn.kg", "r") as f:
-            klong(f.read())
-            r = klong('err')
-            self.assertEqual(r, 0)
-
 if __name__ == "__main__":
     import timeit
     print(timeit.timeit('run_suite_file("klong_fn.kg")', number=10, globals=locals()) / 10)
```

### Comparing `klongpy-0.4.2/tests/test_interop.py` & `klongpy-0.4.3/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/tests/test_join_over.py` & `klongpy-0.4.3/tests/test_join_over.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.assertTrue(kg_equal(r, np.array(['a', 1], dtype=object)))
 
     def test_file_by_lines(self):
         """
         Test the suite file line by line using our own t()
         """
         klong = create_test_klong()
-        with open("tests/klong_join_over.kg", "r") as f:
+        with open("tests/kgtests/klong_join_over.kg", "r") as f:
             skip_header = True
             i = 0
             for r in f.readlines():
                 if skip_header:
                     if r.startswith("t::"):
                         skip_header = False
                     continue
@@ -90,19 +90,12 @@
                 if len(r) == 0:
                     continue
                 i += 1
                 klong.exec(r)
             print(f"executed {i} lines")
 
 
-    def test_gen_file(self):
-        """
-        Test the entire suite file.
-        """
-        self.assertEqual(run_suite_file('klong_join_over.kg'), 0)
-
-
 if __name__ == "__main__":
     import timeit
     number = 20
     print(timeit.timeit('run_suite_file("klong_join_over.kg")', number=number, globals=locals()) / number)
```

### Comparing `klongpy-0.4.2/tests/test_prog.py` & `klongpy-0.4.3/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/tests/test_suite.py` & `klongpy-0.4.3/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/tests/test_suite_file.py` & `klongpy-0.4.3/tests/test_suite_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         klong(t)
 
     def test_file_by_lines(self):
         """
         Test the suite file line by line using our own t()
         """
         klong = create_test_klong()
-        with open("tests/klong_suite.kg", "r") as f:
+        with open("tests/kgtests/klong_suite.kg", "r") as f:
             skip_header = True
             i = 0
             for r in f.readlines():
                 if skip_header:
                     if r.startswith("rnd::"):
                         skip_header = False
                     else:
@@ -138,28 +138,28 @@
             print(f"executed {i} lines")
 
     def test_file_custom_test(self):
         """
         Test the suite file in one go using our own t()
         """
         klong = create_test_klong()
-        with open("tests/klong_suite.kg", "r") as f:
+        with open("tests/kgtests/klong_suite.kg", "r") as f:
             r = f.read()
             i = r.index('rnd::')
             r = r[i:]
             klong(r)
 
-    def test_file(self):
-        """
-        Test the entire suite file.
-        """
-        klong = KlongInterpreter()
-        with open("tests/klong_suite.kg", "r") as f:
-            klong(f.read())
-            r = klong('err')
-            self.assertEqual(r, 0)
-            r = klong['err']
-            self.assertEqual(r, 0)
+    # def test_file(self):
+    #     """
+    #     Test the entire suite file.
+    #     """
+    #     klong = KlongInterpreter()
+    #     with open("tests/kgtests/klong_suite.kg", "r") as f:
+    #         klong(f.read())
+    #         r = klong('err')
+    #         self.assertEqual(r, 0)
+    #         r = klong['err']
+    #         self.assertEqual(r, 0)
 
 
 if __name__ == '__main__':
   unittest.main(failfast=True, exit=False)
```

### Comparing `klongpy-0.4.2/tests/test_sys_fn.py` & `klongpy-0.4.3/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.2/tests/test_util.py` & `klongpy-0.4.3/tests/test_util.py`

 * *Files identical despite different names*

