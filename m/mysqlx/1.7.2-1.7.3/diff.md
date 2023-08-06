# Comparing `tmp/mysqlx-1.7.2.tar.gz` & `tmp/mysqlx-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.7.2.tar", last modified: Wed Aug  2 02:24:06 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.7.3.tar", last modified: Sun Aug  6 06:31:52 2023, max compression
```

## Comparing `mysqlx-1.7.2.tar` & `mysqlx-1.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:24:06.000000 mysqlx-1.7.2/
-drwxrwxrwx   0        0        0        0 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx/
--rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.7.2/mysqlx/db.py
--rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.7.2/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.7.2/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6049 2023-08-02 02:22:18.000000 mysqlx-1.7.2/mysqlx/orm.py
--rw-rw-rw-   0        0        0     1430 2023-07-30 16:14:15.000000 mysqlx-1.7.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5290 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      279 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 02:24:06.000000 mysqlx-1.7.2/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5290 2023-08-02 02:24:06.000000 mysqlx-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     4633 2023-07-30 08:45:57.000000 mysqlx-1.7.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-02 02:24:06.000000 mysqlx-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1375 2023-08-02 02:24:00.000000 mysqlx-1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:31:52.000000 mysqlx-1.7.3/
+drwxrwxrwx   0        0        0        0 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx/
+-rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.7.3/mysqlx/db.py
+-rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.7.3/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.7.3/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6049 2023-08-02 02:22:18.000000 mysqlx-1.7.3/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     1430 2023-07-30 16:14:15.000000 mysqlx-1.7.3/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5290 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      279 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 06:31:52.000000 mysqlx-1.7.3/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5290 2023-08-06 06:31:52.000000 mysqlx-1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4633 2023-07-30 08:45:57.000000 mysqlx-1.7.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-06 06:31:52.000000 mysqlx-1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1375 2023-08-06 06:29:42.000000 mysqlx-1.7.3/setup.py
```

### Comparing `mysqlx-1.7.2/mysqlx/db.py` & `mysqlx-1.7.3/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/mysqlx/dbx.py` & `mysqlx-1.7.3/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/mysqlx/log_support.py` & `mysqlx-1.7.3/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/mysqlx/orm.py` & `mysqlx-1.7.3/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/mysqlx/__init__.py` & `mysqlx-1.7.3/mysqlx/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.7.3/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.7.2
+Version: 1.7.3
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.7.2/PKG-INFO` & `mysqlx-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.7.2
+Version: 1.7.3
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.7.2/README.rst` & `mysqlx-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.7.2/setup.py` & `mysqlx-1.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.1.9',
+        'sqlx-batis>=1.1.2',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.7.2',
+    version='1.7.3',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

