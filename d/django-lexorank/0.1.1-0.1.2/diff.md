# Comparing `tmp/django_lexorank-0.1.1.tar.gz` & `tmp/django_lexorank-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_lexorank-0.1.1.tar", max compression
+gzip compressed data, was "django_lexorank-0.1.2.tar", max compression
```

## Comparing `django_lexorank-0.1.1.tar` & `django_lexorank-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-08-06 16:03:57.877756 django_lexorank-0.1.1/LICENSE
--rw-r--r--   0        0        0     3456 2023-08-06 21:18:08.061475 django_lexorank-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-08-03 18:23:10.714000 django_lexorank-0.1.1/django_lexorank/__init__.py
--rw-r--r--   0        0        0      489 2023-08-06 10:52:45.401000 django_lexorank-0.1.1/django_lexorank/admin.py
--rw-r--r--   0        0        0      104 2023-08-06 10:54:04.667000 django_lexorank-0.1.1/django_lexorank/apps.py
--rw-r--r--   0        0        0     1817 2023-08-06 15:13:30.915126 django_lexorank-0.1.1/django_lexorank/fields.py
--rw-r--r--   0        0        0     5017 2023-08-06 15:13:34.774411 django_lexorank-0.1.1/django_lexorank/lexorank.py
--rw-r--r--   0        0        0     1739 2023-08-06 19:33:03.324562 django_lexorank-0.1.1/django_lexorank/managers.py
--rw-r--r--   0        0        0        0 2023-08-06 10:56:59.851000 django_lexorank-0.1.1/django_lexorank/migrations/__init__.py
--rw-r--r--   0        0        0     8201 2023-08-06 21:06:49.593696 django_lexorank-0.1.1/django_lexorank/models.py
--rw-r--r--   0        0        0     1403 2023-08-06 21:19:14.635008 django_lexorank-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 django_lexorank-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3368 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/__init__.py
+-rw-r--r--   0        0        0      489 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/admin.py
+-rw-r--r--   0        0        0      104 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/apps.py
+-rw-r--r--   0        0        0     1817 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/fields.py
+-rw-r--r--   0        0        0     5017 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/lexorank.py
+-rw-r--r--   0        0        0     1739 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/managers.py
+-rw-r--r--   0        0        0        0 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/migrations/__init__.py
+-rw-r--r--   0        0        0     8201 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/django_lexorank/models.py
+-rw-r--r--   0        0        0     1678 2023-08-06 21:51:27.577360 django_lexorank-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4480 1970-01-01 00:00:00.000000 django_lexorank-0.1.2/PKG-INFO
```

### Comparing `django_lexorank-0.1.1/LICENSE` & `django_lexorank-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_lexorank-0.1.1/README.md` & `django_lexorank-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 
 
 ```shell
 pip install django-lexorank
 ```
 
 
-## Configuration
-
-
-Add `django_lexorank` to `INSTALLED_APPS` in your Django settings:
-
-
 ## Usage
 
 
 ### Defining models
 
 To add ranking to your model, you need to inherit it from `RankedModel`.
```

### Comparing `django_lexorank-0.1.1/django_lexorank/fields.py` & `django_lexorank-0.1.2/django_lexorank/fields.py`

 * *Files identical despite different names*

### Comparing `django_lexorank-0.1.1/django_lexorank/lexorank.py` & `django_lexorank-0.1.2/django_lexorank/lexorank.py`

 * *Files identical despite different names*

### Comparing `django_lexorank-0.1.1/django_lexorank/managers.py` & `django_lexorank-0.1.2/django_lexorank/managers.py`

 * *Files identical despite different names*

### Comparing `django_lexorank-0.1.1/django_lexorank/models.py` & `django_lexorank-0.1.2/django_lexorank/models.py`

 * *Files identical despite different names*

### Comparing `django_lexorank-0.1.1/PKG-INFO` & `django_lexorank-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: django-lexorank
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package implements an algorithm similar to JIRA's lexorank, but without using buckets for rebalancing that can be used with Django projects.
 License: MIT
 Author: Alex Rozum
 Author-email: rozumalex@gmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2,<4.0)
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: django (>=3.2,<5)
 Project-URL: Bug Tracker, https://github.com/rozumdev/django-lexorank/issues/
 Project-URL: Homepage, https://github.com/rozumdev/django-lexorank/
 Description-Content-Type: text/markdown
 
 # django-lexorank
 
 [![Test workflow](https://github.com/rozumdev/django-lexorank/actions/workflows/tests.yml/badge.svg)](https://github.com/rozumdev/django-lexorank/actions/workflows/test.yml/)
@@ -31,20 +37,14 @@
 
 
 ```shell
 pip install django-lexorank
 ```
 
 
-## Configuration
-
-
-Add `django_lexorank` to `INSTALLED_APPS` in your Django settings:
-
-
 ## Usage
 
 
 ### Defining models
 
 To add ranking to your model, you need to inherit it from `RankedModel`.
```

