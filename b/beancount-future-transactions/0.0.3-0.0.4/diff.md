# Comparing `tmp/beancount-future-transactions-0.0.3.tar.gz` & `tmp/beancount-future-transactions-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount-future-transactions-0.0.3.tar", last modified: Wed Feb 22 11:29:52 2023, max compression
+gzip compressed data, was "beancount-future-transactions-0.0.4.tar", last modified: Sun Aug  6 11:53:16 2023, max compression
```

## Comparing `beancount-future-transactions-0.0.3.tar` & `beancount-future-transactions-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-22 11:29:52.532000 beancount-future-transactions-0.0.3/
--rw-rw-r--   0 user      (1000) user      (1000)       55 2021-12-28 14:18:19.000000 beancount-future-transactions-0.0.3/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      161 2022-01-26 18:08:01.000000 beancount-future-transactions-0.0.3/Jenkinsfile
--rw-rw-r--   0 user      (1000) user      (1000)       18 2021-12-28 14:27:17.000000 beancount-future-transactions-0.0.3/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     1307 2023-02-22 11:29:52.532000 beancount-future-transactions-0.0.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      572 2021-12-28 14:14:25.000000 beancount-future-transactions-0.0.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-22 11:29:52.532000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1307 2023-02-22 11:29:52.000000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      504 2023-02-22 11:29:52.000000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-22 11:29:52.000000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-22 11:29:25.000000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       21 2023-02-22 11:29:52.000000 beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       18 2023-02-22 10:34:27.000000 beancount-future-transactions-0.0.3/build.parameters
--rw-rw-r--   0 user      (1000) user      (1000)      130 2023-02-22 11:29:52.533000 beancount-future-transactions-0.0.3/setup.cfg
--rwxrwxr-x   0 user      (1000) user      (1000)     1465 2023-02-22 11:29:40.000000 beancount-future-transactions-0.0.3/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-22 11:29:52.530000 beancount-future-transactions-0.0.3/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-22 11:29:52.532000 beancount-future-transactions-0.0.3/src/beancount_extensions/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-12-28 14:14:56.000000 beancount-future-transactions-0.0.3/src/beancount_extensions/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-02-22 11:29:52.532000 beancount-future-transactions-0.0.3/src/beancount_extensions/future_transactions/
--rw-rw-r--   0 user      (1000) user      (1000)      811 2022-01-26 18:06:04.000000 beancount-future-transactions-0.0.3/src/beancount_extensions/future_transactions/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      488 2022-01-26 18:05:31.000000 beancount-future-transactions-0.0.3/src/beancount_extensions/future_transactions/test_transactions.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-06 11:53:16.206000 beancount-future-transactions-0.0.4/
+-rw-rw-r--   0 user      (1000) user      (1000)       55 2021-12-28 14:18:19.000000 beancount-future-transactions-0.0.4/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2021-12-28 14:27:17.000000 beancount-future-transactions-0.0.4/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     1180 2023-08-06 11:53:16.206000 beancount-future-transactions-0.0.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      572 2021-12-28 14:14:25.000000 beancount-future-transactions-0.0.4/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-06 11:53:16.205000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1180 2023-08-06 11:53:15.000000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      475 2023-08-06 11:53:16.000000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-08-06 11:53:15.000000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-08-06 11:53:15.000000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-08-06 11:53:15.000000 beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      130 2023-08-06 11:53:16.206000 beancount-future-transactions-0.0.4/setup.cfg
+-rwxrwxr-x   0 user      (1000) user      (1000)     1465 2023-02-22 11:29:40.000000 beancount-future-transactions-0.0.4/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-06 11:53:16.204000 beancount-future-transactions-0.0.4/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-06 11:53:16.205000 beancount-future-transactions-0.0.4/src/beancount_extensions/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-12-28 14:14:56.000000 beancount-future-transactions-0.0.4/src/beancount_extensions/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-06 11:53:16.205000 beancount-future-transactions-0.0.4/src/beancount_extensions/future_transactions/
+-rw-rw-r--   0 user      (1000) user      (1000)      811 2023-08-06 11:52:57.000000 beancount-future-transactions-0.0.4/src/beancount_extensions/future_transactions/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      488 2022-01-26 18:05:31.000000 beancount-future-transactions-0.0.4/src/beancount_extensions/future_transactions/test_transactions.py
```

### Comparing `beancount-future-transactions-0.0.3/PKG-INFO` & `beancount-future-transactions-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: beancount-future-transactions
-Version: 0.0.3
+Version: 0.0.4
 Summary: A plugin for Beancount that suppresses future transactions
 Home-page: http://github.com/Rudd-O/beancount-future-transactions
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPL
-Description: # Beancount future transactions
-        
-        This is a very simple plugin for Beancount that filters out transactions with a future date, provided they are tagged with the `#future` tag.
-        
-        To use:
-        
-        * Install using your favorite Python method — probably `pip` or `python setup.py install`, although you may want to install to your user directory (`pip --user`).
-        * Include the stanza `plugin "beancount_extensions.future_transactions"` in your Beancount file.
-        
-        That's it.
-        
-        From this point on, any transaction with a future tagged `#future` will not appear in your reports and queries.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: beancount
+
+# Beancount future transactions
+
+This is a very simple plugin for Beancount that filters out transactions with a future date, provided they are tagged with the `#future` tag.
+
+To use:
+
+* Install using your favorite Python method — probably `pip` or `python setup.py install`, although you may want to install to your user directory (`pip --user`).
+* Include the stanza `plugin "beancount_extensions.future_transactions"` in your Beancount file.
+
+That's it.
+
+From this point on, any transaction with a future tagged `#future` will not appear in your reports and queries.
```

### Comparing `beancount-future-transactions-0.0.3/README.md` & `beancount-future-transactions-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `beancount-future-transactions-0.0.3/beancount_future_transactions.egg-info/PKG-INFO` & `beancount-future-transactions-0.0.4/beancount_future_transactions.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: beancount-future-transactions
-Version: 0.0.3
+Version: 0.0.4
 Summary: A plugin for Beancount that suppresses future transactions
 Home-page: http://github.com/Rudd-O/beancount-future-transactions
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 License: GPL
-Description: # Beancount future transactions
-        
-        This is a very simple plugin for Beancount that filters out transactions with a future date, provided they are tagged with the `#future` tag.
-        
-        To use:
-        
-        * Install using your favorite Python method — probably `pip` or `python setup.py install`, although you may want to install to your user directory (`pip --user`).
-        * Include the stanza `plugin "beancount_extensions.future_transactions"` in your Beancount file.
-        
-        That's it.
-        
-        From this point on, any transaction with a future tagged `#future` will not appear in your reports and queries.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires: beancount
+
+# Beancount future transactions
+
+This is a very simple plugin for Beancount that filters out transactions with a future date, provided they are tagged with the `#future` tag.
+
+To use:
+
+* Install using your favorite Python method — probably `pip` or `python setup.py install`, although you may want to install to your user directory (`pip --user`).
+* Include the stanza `plugin "beancount_extensions.future_transactions"` in your Beancount file.
+
+That's it.
+
+From this point on, any transaction with a future tagged `#future` will not appear in your reports and queries.
```

### Comparing `beancount-future-transactions-0.0.3/setup.py` & `beancount-future-transactions-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `beancount-future-transactions-0.0.3/src/beancount_extensions/future_transactions/__init__.py` & `beancount-future-transactions-0.0.4/src/beancount_extensions/future_transactions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A plugin that suppresses future transactions when enabled.
 """
 
 __author__ = 'Manuel Amador (Rudd-O)'
 __plugins__ = ('future_transactions_plugin',)
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import datetime
 from beancount.core import data
 
 # The name of the metadata field that indicates this is a future transaction
 # that should be filtered out if it is past today's date.
 META = 'future'
```

