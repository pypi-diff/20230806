# Comparing `tmp/YzDB-0.0.2.tar.gz` & `tmp/YzDB-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YzDB-0.0.2.tar", last modified: Sat Aug  5 07:58:46 2023, max compression
+gzip compressed data, was "YzDB-0.0.3.tar", last modified: Sun Aug  6 05:04:24 2023, max compression
```

## Comparing `YzDB-0.0.2.tar` & `YzDB-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,31 @@
-drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.169814 YzDB-0.0.2/
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     1070 2023-08-05 06:44:36.000000 YzDB-0.0.2/LICENSE
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-05 07:58:46.169692 YzDB-0.0.2/PKG-INFO
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     1913 2023-08-05 06:44:36.000000 YzDB-0.0.2/README.md
-drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.168599 YzDB-0.0.2/YzDB.egg-info/
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/PKG-INFO
--rw-r--r--   0 huangyanzhong   (501) staff       (20)      322 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/SOURCES.txt
--rw-r--r--   0 huangyanzhong   (501) staff       (20)        1 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/dependency_links.txt
--rw-r--r--   0 huangyanzhong   (501) staff       (20)       78 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/requires.txt
--rw-r--r--   0 huangyanzhong   (501) staff       (20)        5 2023-08-05 07:58:46.000000 YzDB-0.0.2/YzDB.egg-info/top_level.txt
--rw-r--r--   0 huangyanzhong   (501) staff       (20)       38 2023-08-05 07:58:46.169854 YzDB-0.0.2/setup.cfg
--rw-r--r--   0 huangyanzhong   (501) staff       (20)      977 2023-08-05 07:58:02.000000 YzDB-0.0.2/setup.py
-drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.168996 YzDB-0.0.2/tests/
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     3760 2023-08-05 07:34:44.000000 YzDB-0.0.2/tests/test_db_base.py
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     2699 2023-08-05 07:34:31.000000 YzDB-0.0.2/tests/test_mysql_operations.py
--rw-r--r--   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:36:29.000000 YzDB-0.0.2/tests/test_sqlite_operations.py
-drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:58:46.169500 YzDB-0.0.2/yzdb/
--rw-r--r--   0 huangyanzhong   (501) staff       (20)      116 2023-08-05 07:57:43.000000 YzDB-0.0.2/yzdb/__init__.py
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     1571 2023-08-05 07:51:42.000000 YzDB-0.0.2/yzdb/conn_mysql.py
--rw-r--r--   0 huangyanzhong   (501) staff       (20)      975 2023-08-05 07:57:30.000000 YzDB-0.0.2/yzdb/conn_sqlite.py
--rw-r--r--   0 huangyanzhong   (501) staff       (20)     2490 2023-08-05 07:30:39.000000 YzDB-0.0.2/yzdb/db_base.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-06 05:04:24.594304 YzDB-0.0.3/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1070 2023-08-05 06:44:36.000000 YzDB-0.0.3/LICENSE
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-06 05:04:24.594177 YzDB-0.0.3/PKG-INFO
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1913 2023-08-05 06:44:36.000000 YzDB-0.0.3/README.md
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-06 05:04:24.592126 YzDB-0.0.3/YzDB.egg-info/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2336 2023-08-06 05:04:24.000000 YzDB-0.0.3/YzDB.egg-info/PKG-INFO
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      598 2023-08-06 05:04:24.000000 YzDB-0.0.3/YzDB.egg-info/SOURCES.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        1 2023-08-06 05:04:24.000000 YzDB-0.0.3/YzDB.egg-info/dependency_links.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)       78 2023-08-06 05:04:24.000000 YzDB-0.0.3/YzDB.egg-info/requires.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        5 2023-08-06 05:04:24.000000 YzDB-0.0.3/YzDB.egg-info/top_level.txt
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)       38 2023-08-06 05:04:24.594348 YzDB-0.0.3/setup.cfg
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      977 2023-08-06 05:03:48.000000 YzDB-0.0.3/setup.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-06 05:04:24.592464 YzDB-0.0.3/tests/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     3760 2023-08-05 07:34:44.000000 YzDB-0.0.3/tests/test_db_base.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2699 2023-08-05 07:34:31.000000 YzDB-0.0.3/tests/test_mysql_operations.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)        0 2023-08-05 07:36:29.000000 YzDB-0.0.3/tests/test_sqlite_operations.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-06 05:04:24.592907 YzDB-0.0.3/yzdb/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      141 2023-08-06 05:03:42.000000 YzDB-0.0.3/yzdb/__init__.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     1571 2023-08-06 04:58:08.000000 YzDB-0.0.3/yzdb/conn_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      975 2023-08-06 04:58:10.000000 YzDB-0.0.3/yzdb/conn_sqlite.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2490 2023-08-05 07:30:39.000000 YzDB-0.0.3/yzdb/db_base.py
+drwxr-xr-x   0 huangyanzhong   (501) staff       (20)        0 2023-08-06 05:04:24.593997 YzDB-0.0.3/yzdb/operations/
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)      215 2023-08-06 05:03:25.000000 YzDB-0.0.3/yzdb/operations/__init__.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2719 2023-08-05 06:44:36.000000 YzDB-0.0.3/yzdb/operations/add_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2755 2023-08-05 07:53:14.000000 YzDB-0.0.3/yzdb/operations/add_sqlite.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2316 2023-08-05 06:44:36.000000 YzDB-0.0.3/yzdb/operations/drop_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     2460 2023-08-05 07:53:28.000000 YzDB-0.0.3/yzdb/operations/drop_sqlite.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     3090 2023-08-05 06:44:36.000000 YzDB-0.0.3/yzdb/operations/modify_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     3282 2023-08-05 07:53:40.000000 YzDB-0.0.3/yzdb/operations/modify_sqlite.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     6263 2023-08-05 06:44:36.000000 YzDB-0.0.3/yzdb/operations/query_mysql.py
+-rw-r--r--   0 huangyanzhong   (501) staff       (20)     6809 2023-08-05 07:53:58.000000 YzDB-0.0.3/yzdb/operations/query_sqlite.py
```

### Comparing `YzDB-0.0.2/LICENSE` & `YzDB-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/PKG-INFO` & `YzDB-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YzDB
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for easy using database
 Home-page: https://github.com/Yanzhong-Hub/yzdb
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `YzDB-0.0.2/README.md` & `YzDB-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/YzDB.egg-info/PKG-INFO` & `YzDB-0.0.3/YzDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YzDB
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for easy using database
 Home-page: https://github.com/Yanzhong-Hub/yzdb
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `YzDB-0.0.2/setup.py` & `YzDB-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # requirements
 with open("requirements.txt", "r") as f:
     requirements = f.read()
     requirements = requirements.split("\n")
 
 setup(
     name="YzDB",  # Need modify
-    version="0.0.2",  # Need modify
+    version="0.0.3",  # Need modify
     author="Yanzhong Huang",
     author_email="yanzhong.huang@outlook.com",
     description="A package for easy using database",  # Need modify
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yanzhong-Hub/yzdb",  # Need modify
     packages=find_packages(),
```

### Comparing `YzDB-0.0.2/tests/test_db_base.py` & `YzDB-0.0.3/tests/test_db_base.py`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/tests/test_mysql_operations.py` & `YzDB-0.0.3/tests/test_mysql_operations.py`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/yzdb/conn_mysql.py` & `YzDB-0.0.3/yzdb/conn_mysql.py`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/yzdb/conn_sqlite.py` & `YzDB-0.0.3/yzdb/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `YzDB-0.0.2/yzdb/db_base.py` & `YzDB-0.0.3/yzdb/db_base.py`

 * *Files identical despite different names*

