# Comparing `tmp/sqlx-batis-1.1.1.tar.gz` & `tmp/sqlx-batis-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-1.1.1.tar", last modified: Fri Aug  4 01:52:22 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-1.1.2.tar", last modified: Sun Aug  6 06:28:16 2023, max compression
```

## Comparing `sqlx-batis-1.1.1.tar` & `sqlx-batis-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/
--rw-rw-rw-   0        0        0     5701 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-1.1.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-08-04 01:51:46.000000 sqlx-batis-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlbatis/
--rw-rw-rw-   0        0        0      927 2023-08-01 15:24:17.000000 sqlx-batis-1.1.1/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     6719 2023-08-01 15:51:50.000000 sqlx-batis-1.1.1/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-1.1.1/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6732 2023-08-03 03:29:50.000000 sqlx-batis-1.1.1/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-1.1.1/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    35069 2023-08-02 00:35:05.000000 sqlx-batis-1.1.1/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     4089 2023-08-02 00:22:16.000000 sqlx-batis-1.1.1/sqlbatis/orm_support.py
--rw-rw-rw-   0        0        0     2672 2023-08-04 01:49:10.000000 sqlx-batis-1.1.1/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 sqlx-batis-1.1.1/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-1.1.1/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1216 2023-08-01 15:23:13.000000 sqlx-batis-1.1.1/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-1.1.1/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-1.1.1/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      489 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/
+-rw-rw-rw-   0        0        0     5701 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-1.1.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-08-06 06:28:03.000000 sqlx-batis-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlbatis/
+-rw-rw-rw-   0        0        0      927 2023-08-01 15:24:17.000000 sqlx-batis-1.1.2/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     6719 2023-08-01 15:51:50.000000 sqlx-batis-1.1.2/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-1.1.2/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6732 2023-08-03 03:29:50.000000 sqlx-batis-1.1.2/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-1.1.2/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    35069 2023-08-02 00:35:05.000000 sqlx-batis-1.1.2/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     3983 2023-08-06 06:26:06.000000 sqlx-batis-1.1.2/sqlbatis/orm_support.py
+-rw-rw-rw-   0        0        0     2672 2023-08-04 01:49:10.000000 sqlx-batis-1.1.2/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 sqlx-batis-1.1.2/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-1.1.2/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1216 2023-08-01 15:23:13.000000 sqlx-batis-1.1.2/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-1.1.2/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-1.1.2/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-08-06 06:28:15.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      489 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 06:28:16.000000 sqlx-batis-1.1.2/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-1.1.1/PKG-INFO` & `sqlx-batis-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 1.1.1
+Version: 1.1.2
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-1.1.1/README.rst` & `sqlx-batis-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/setup.py` & `sqlx-batis-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'sqlx-exec>=1.4.6',
     ],
-    version='1.1.1',
+    version='1.1.2',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-1.1.1/sqlbatis/constant.py` & `sqlx-batis-1.1.2/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/db.py` & `sqlx-batis-1.1.2/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/dbx.py` & `sqlx-batis-1.1.2/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/engine.py` & `sqlx-batis-1.1.2/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/log_support.py` & `sqlx-batis-1.1.2/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/orm.py` & `sqlx-batis-1.1.2/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/orm_support.py` & `sqlx-batis-1.1.2/sqlbatis/orm_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,15 @@
                     args.append(arg)
         where = 'WHERE {}'.format(' and '.join(conditions))
 
     return where, args, limit
 
 
 def split_ids(ids: Sequence[int], batch_size):
-    ids_size = len(ids)
-    n = ids_size // batch_size
-    n += 0 if ids_size % batch_size == 0 else 1
-    return [ids[i:i + batch_size] for i in range(0, ids_size, batch_size)]
+    return [ids[i:i + batch_size] for i in range(0, len(ids), batch_size)]
 
 
 def get_table_name(class_name):
     for i in range(1, len(class_name) - 1)[::-1]:
         if class_name[i].isupper():
             class_name = class_name[:i] + '_' + class_name[i:]
     return class_name.lower()
```

### Comparing `sqlx-batis-1.1.1/sqlbatis/snowflake.py` & `sqlx-batis-1.1.2/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/sql_holder.py` & `sqlx-batis-1.1.2/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/sql_mapper.py` & `sqlx-batis-1.1.2/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/sql_support.py` & `sqlx-batis-1.1.2/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlbatis/__init__.py` & `sqlx-batis-1.1.2/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.1/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-1.1.2/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 1.1.1
+Version: 1.1.2
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

