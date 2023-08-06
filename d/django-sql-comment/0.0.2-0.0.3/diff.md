# Comparing `tmp/django-sql-comment-0.0.2.tar.gz` & `tmp/django-sql-comment-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-sql-comment-0.0.2.tar", last modified: Tue May  5 14:58:13 2020, max compression
+gzip compressed data, was "dist/django-sql-comment-0.0.3.tar", last modified: Wed Jun  3 19:00:56 2020, max compression
```

## Comparing `django-sql-comment-0.0.2.tar` & `django-sql-comment-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/
-drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment/
-drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment/management/
--rw-rw-r--   0 phil      (1001) phil      (1001)        0 2020-04-27 13:04:47.000000 django-sql-comment-0.0.2/django_sql_comment/management/__init__.py
-drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment/management/commands/
--rw-rw-r--   0 phil      (1001) phil      (1001)        0 2020-04-27 13:04:51.000000 django-sql-comment-0.0.2/django_sql_comment/management/commands/__init__.py
--rw-rw-r--   0 phil      (1001) phil      (1001)      611 2020-05-05 12:48:46.000000 django-sql-comment-0.0.2/django_sql_comment/management/commands/sqlcomment.py
--rw-rw-r--   0 phil      (1001) phil      (1001)     1793 2020-05-05 14:55:59.000000 django-sql-comment-0.0.2/django_sql_comment/__init__.py
--rw-rw-r--   0 phil      (1001) phil      (1001)     2058 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/PKG-INFO
--rwxrwxr-x   0 phil      (1001) phil      (1001)     1904 2020-05-05 14:56:14.000000 django-sql-comment-0.0.2/setup.py
--rw-rw-r--   0 phil      (1001) phil      (1001)      926 2020-05-05 14:51:51.000000 django-sql-comment-0.0.2/README.rst
--rw-rw-r--   0 phil      (1001) phil      (1001)       38 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/setup.cfg
-drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/
--rw-rw-r--   0 phil      (1001) phil      (1001)        1 2020-05-05 13:41:46.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/not-zip-safe
--rw-rw-r--   0 phil      (1001) phil      (1001)     2058 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1001) phil      (1001)       19 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1001) phil      (1001)      405 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1001) phil      (1001)        1 2020-05-05 14:58:13.000000 django-sql-comment-0.0.2/django_sql_comment.egg-info/dependency_links.txt
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/django_sql_comment/
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/django_sql_comment/management/
+-rw-rw-r--   0 phil      (1001) phil      (1001)        0 2020-04-27 13:04:47.000000 django-sql-comment-0.0.3/django_sql_comment/management/__init__.py
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/django_sql_comment/management/commands/
+-rw-rw-r--   0 phil      (1001) phil      (1001)        0 2020-04-27 13:04:51.000000 django-sql-comment-0.0.3/django_sql_comment/management/commands/__init__.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)      611 2020-05-05 12:48:46.000000 django-sql-comment-0.0.3/django_sql_comment/management/commands/sqlcomment.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)     2163 2020-06-03 18:56:47.000000 django-sql-comment-0.0.3/django_sql_comment/__init__.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)     2058 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/PKG-INFO
+-rwxrwxr-x   0 phil      (1001) phil      (1001)     1904 2020-06-03 18:57:19.000000 django-sql-comment-0.0.3/setup.py
+-rw-rw-r--   0 phil      (1001) phil      (1001)      926 2020-05-05 14:51:51.000000 django-sql-comment-0.0.3/README.rst
+-rw-rw-r--   0 phil      (1001) phil      (1001)       38 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/setup.cfg
+drwxrwxr-x   0 phil      (1001) phil      (1001)        0 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/
+-rw-rw-r--   0 phil      (1001) phil      (1001)        1 2020-05-05 13:41:46.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/not-zip-safe
+-rw-rw-r--   0 phil      (1001) phil      (1001)     2058 2020-06-03 19:00:55.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1001) phil      (1001)       19 2020-06-03 19:00:55.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1001) phil      (1001)      405 2020-06-03 19:00:56.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1001) phil      (1001)        1 2020-06-03 19:00:55.000000 django-sql-comment-0.0.3/django_sql_comment.egg-info/dependency_links.txt
```

### Comparing `django-sql-comment-0.0.2/django_sql_comment/management/commands/sqlcomment.py` & `django-sql-comment-0.0.3/django_sql_comment/management/commands/sqlcomment.py`

 * *Files identical despite different names*

### Comparing `django-sql-comment-0.0.2/django_sql_comment/__init__.py` & `django-sql-comment-0.0.3/django_sql_comment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.apps import apps
+from django.contrib.postgres.fields import ArrayField
 from django.db import DEFAULT_DB_ALIAS, connections, router, transaction
 from django.utils.encoding import force_text
 from django.utils.text import camel_case_to_spaces
 
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def field_name_is_auto(field):
     return field.verbose_name == field.name.replace('_', ' ')
 
 
 def model_name_is_auto(model):
@@ -24,15 +25,21 @@
             table = model._meta.db_table
             comment = (None if model_name_is_auto(model)
                        else model._meta.verbose_name)
             yield out('COMMENT ON TABLE "{}" IS %s'.format(table),
                       comment or None)
             for f in model._meta.fields:
                 strings = (('' if field_name_is_auto(f) else f.verbose_name),
-                           f.help_text)
+                           f.help_text,
+                           (('' if field_name_is_auto(f.base_field)
+                             else f.base_field.verbose_name)
+                            if isinstance(f, ArrayField) else ''),
+                           (f.base_field.help_text if isinstance(f, ArrayField)
+                            else ''),)
+
                 comment = ' | '.join(map(force_text, filter(None, strings)))
                 yield out('COMMENT ON COLUMN "{}"."{}" IS %s'
                           .format(table, f.column),
                           comment or None)
 
 
 def sqlcomment_post_migrate(app_config, using=DEFAULT_DB_ALIAS, apps=apps,
```

### Comparing `django-sql-comment-0.0.2/PKG-INFO` & `django-sql-comment-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-sql-comment
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django management command to generate SQL for applying your models' verbose name and help_text as PostgreSQL COMMENTs
 Home-page: https://github.com/tuffnatty/django-sql-comment
 Author: Phil Krylov
 Author-email: phil.krylov@gmail.com
 License: MIT
 Description: Django SQL COMMENT
         ==================
```

### Comparing `django-sql-comment-0.0.2/setup.py` & `django-sql-comment-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
-version = '0.0.2'
+version = '0.0.3'
 
 
 if sys.argv[-1] == 'publish':
     try:
         import wheel
         print("Wheel version: ", wheel.__version__)
     except ImportError:
```

### Comparing `django-sql-comment-0.0.2/README.rst` & `django-sql-comment-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-sql-comment-0.0.2/django_sql_comment.egg-info/PKG-INFO` & `django-sql-comment-0.0.3/django_sql_comment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-sql-comment
-Version: 0.0.2
+Version: 0.0.3
 Summary: Django management command to generate SQL for applying your models' verbose name and help_text as PostgreSQL COMMENTs
 Home-page: https://github.com/tuffnatty/django-sql-comment
 Author: Phil Krylov
 Author-email: phil.krylov@gmail.com
 License: MIT
 Description: Django SQL COMMENT
         ==================
```

