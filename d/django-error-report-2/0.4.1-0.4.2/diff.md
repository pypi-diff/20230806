# Comparing `tmp/django-error-report-2-0.4.1.tar.gz` & `tmp/django-error-report-2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-error-report-2-0.4.1.tar", last modified: Tue Jul  4 22:03:21 2023, max compression
+gzip compressed data, was "django-error-report-2-0.4.2.tar", last modified: Sat Aug  5 23:02:03 2023, max compression
```

## Comparing `django-error-report-2-0.4.1.tar` & `django-error-report-2-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.195551 django-error-report-2-0.4.1/
--rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/LICENSE.txt
--rw-r--r--   0 matmair    (501) staff       (20)       37 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/MANIFEST.in
--rw-r--r--   0 matmair    (501) staff       (20)     2153 2023-07-04 22:03:21.195354 django-error-report-2-0.4.1/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)     1567 2023-07-04 21:07:36.000000 django-error-report-2-0.4.1/README.md
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.192123 django-error-report-2-0.4.1/django_error_report_2.egg-info/
--rw-r--r--   0 matmair    (501) staff       (20)     2153 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/PKG-INFO
--rw-r--r--   0 matmair    (501) staff       (20)      572 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/SOURCES.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/dependency_links.txt
--rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/not-zip-safe
--rw-r--r--   0 matmair    (501) staff       (20)       12 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/requires.txt
--rw-r--r--   0 matmair    (501) staff       (20)       13 2023-07-04 22:03:21.000000 django-error-report-2-0.4.1/django_error_report_2.egg-info/top_level.txt
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.194312 django-error-report-2-0.4.1/error_report/
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)      955 2023-07-04 21:59:36.000000 django-error-report-2-0.4.1/error_report/admin.py
--rw-r--r--   0 matmair    (501) staff       (20)      180 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/apps.py
--rw-r--r--   0 matmair    (501) staff       (20)     1050 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/middleware.py
-drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-07-04 22:03:21.194859 django-error-report-2-0.4.1/error_report/migrations/
--rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/migrations/0001_initial.py
--rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/migrations/__init__.py
--rw-r--r--   0 matmair    (501) staff       (20)     1750 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/models.py
--rw-r--r--   0 matmair    (501) staff       (20)      105 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/settings.py
--rw-r--r--   0 matmair    (501) staff       (20)      306 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/urls.py
--rw-r--r--   0 matmair    (501) staff       (20)      395 2023-07-04 20:58:50.000000 django-error-report-2-0.4.1/error_report/views.py
--rw-r--r--   0 matmair    (501) staff       (20)       38 2023-07-04 22:03:21.195615 django-error-report-2-0.4.1/setup.cfg
--rw-r--r--   0 matmair    (501) staff       (20)     1161 2023-07-04 22:02:34.000000 django-error-report-2-0.4.1/setup.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-08-05 23:02:03.378956 django-error-report-2-0.4.2/
+-rw-r--r--   0 matmair    (501) staff       (20)     1086 2023-07-04 20:58:50.000000 django-error-report-2-0.4.2/LICENSE.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       38 2023-08-05 22:19:12.000000 django-error-report-2-0.4.2/MANIFEST.in
+-rw-r--r--   0 matmair    (501) staff       (20)     2139 2023-08-05 23:02:03.379024 django-error-report-2-0.4.2/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)     1553 2023-08-05 22:19:12.000000 django-error-report-2-0.4.2/README.md
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-08-05 23:02:03.376592 django-error-report-2-0.4.2/django_error_report_2.egg-info/
+-rw-r--r--   0 matmair    (501) staff       (20)     2139 2023-08-05 23:02:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/PKG-INFO
+-rw-r--r--   0 matmair    (501) staff       (20)      582 2023-08-05 23:02:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/SOURCES.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-08-05 23:02:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/dependency_links.txt
+-rw-r--r--   0 matmair    (501) staff       (20)        1 2023-07-04 21:03:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/not-zip-safe
+-rw-r--r--   0 matmair    (501) staff       (20)       12 2023-08-05 23:02:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/requires.txt
+-rw-r--r--   0 matmair    (501) staff       (20)       13 2023-08-05 23:02:03.000000 django-error-report-2-0.4.2/django_error_report_2.egg-info/top_level.txt
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-08-05 23:02:03.378397 django-error-report-2-0.4.2/error_report/
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.2/error_report/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)     2376 2023-08-05 22:58:51.000000 django-error-report-2-0.4.2/error_report/admin.py
+-rw-r--r--   0 matmair    (501) staff       (20)      270 2023-08-05 22:29:11.000000 django-error-report-2-0.4.2/error_report/apps.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1227 2023-08-05 22:32:58.000000 django-error-report-2-0.4.2/error_report/middleware.py
+drwxr-xr-x   0 matmair    (501) staff       (20)        0 2023-08-05 23:02:03.378847 django-error-report-2-0.4.2/error_report/migrations/
+-rw-r--r--   0 matmair    (501) staff       (20)     1131 2023-07-04 20:58:50.000000 django-error-report-2-0.4.2/error_report/migrations/0001_initial.py
+-rw-r--r--   0 matmair    (501) staff       (20)        0 2023-07-04 20:58:50.000000 django-error-report-2-0.4.2/error_report/migrations/__init__.py
+-rw-r--r--   0 matmair    (501) staff       (20)     1739 2023-08-05 22:41:57.000000 django-error-report-2-0.4.2/error_report/models.py
+-rw-r--r--   0 matmair    (501) staff       (20)      155 2023-08-05 22:28:11.000000 django-error-report-2-0.4.2/error_report/settings.py
+-rw-r--r--   0 matmair    (501) staff       (20)      352 2023-08-05 22:28:19.000000 django-error-report-2-0.4.2/error_report/urls.py
+-rw-r--r--   0 matmair    (501) staff       (20)      481 2023-08-05 22:25:08.000000 django-error-report-2-0.4.2/error_report/views.py
+-rw-r--r--   0 matmair    (501) staff       (20)      537 2023-08-05 23:02:03.379499 django-error-report-2-0.4.2/setup.cfg
+-rw-r--r--   0 matmair    (501) staff       (20)     1208 2023-08-05 22:42:44.000000 django-error-report-2-0.4.2/setup.py
```

### Comparing `django-error-report-2-0.4.1/LICENSE.txt` & `django-error-report-2-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.1/PKG-INFO` & `django-error-report-2-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.1
+Version: 0.4.2
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-              
+
 django-error-report-2
 ===================
 Maintained fork of [django-error-report](https://github.com/mhsiddiqui/django-error-report). Original author  [mhsiddiqui](https://github.com/mhsiddiqui/)
 
 View all Django Error detail in Django Admin.
 
 Error-report save Django error traceback and details which would be the
```

### Comparing `django-error-report-2-0.4.1/README.md` & `django-error-report-2-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-              
+
 django-error-report-2
 ===================
 Maintained fork of [django-error-report](https://github.com/mhsiddiqui/django-error-report). Original author  [mhsiddiqui](https://github.com/mhsiddiqui/)
 
 View all Django Error detail in Django Admin.
 
 Error-report save Django error traceback and details which would be the
```

### Comparing `django-error-report-2-0.4.1/django_error_report_2.egg-info/PKG-INFO` & `django-error-report-2-0.4.2/django_error_report_2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-error-report-2
-Version: 0.4.1
+Version: 0.4.2
 Summary: View Django Error Report in Django Admin
 Home-page: https://github.com/matmair/django-error-report-2
 Author: M Hassan Siddiqui
 Author-email: mhassan.eeng@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-              
+
 django-error-report-2
 ===================
 Maintained fork of [django-error-report](https://github.com/mhsiddiqui/django-error-report). Original author  [mhsiddiqui](https://github.com/mhsiddiqui/)
 
 View all Django Error detail in Django Admin.
 
 Error-report save Django error traceback and details which would be the
```

### Comparing `django-error-report-2-0.4.1/django_error_report_2.egg-info/SOURCES.txt` & `django-error-report-2-0.4.2/django_error_report_2.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 django_error_report_2.egg-info/PKG-INFO
 django_error_report_2.egg-info/SOURCES.txt
 django_error_report_2.egg-info/dependency_links.txt
 django_error_report_2.egg-info/not-zip-safe
 django_error_report_2.egg-info/requires.txt
 django_error_report_2.egg-info/top_level.txt
```

### Comparing `django-error-report-2-0.4.1/error_report/middleware.py` & `django-error-report-2-0.4.2/error_report/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+"""Middleware for django-error-report-2 package."""
 from __future__ import absolute_import, unicode_literals
 
-import traceback
 import sys
+import traceback
 
 from django.views.debug import ExceptionReporter
 
 from error_report.models import Error
 from error_report.settings import ERROR_DETAIL_SETTINGS
 
 
 class ExceptionProcessor(object):
-    """
-    Middleware that save details of exception that occurs in any app to the database.
-    """
+    """Middleware that save details of exception that occurs in any app to the database."""
 
     def __init__(self, get_response=None):
+        """Save `get_response` for later reference."""
         self.get_response = get_response
 
     def __call__(self, request):
+        """Return normal response."""
         return self.get_response(request)
 
     def process_exception(self, request, exception):
+        """Save exception to database."""
         kind, info, data = sys.exc_info()
         if not ERROR_DETAIL_SETTINGS.get('ERROR_DETAIL_ENABLE', True):
             return None
         error = Error.objects.create(
             kind=kind.__name__,
             html=ExceptionReporter(request, kind, info, data).get_traceback_html(),
             path=request.build_absolute_uri(),
```

### Comparing `django-error-report-2-0.4.1/error_report/migrations/0001_initial.py` & `django-error-report-2-0.4.2/error_report/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-error-report-2-0.4.1/error_report/models.py` & `django-error-report-2-0.4.2/error_report/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
+"""Models for django-error-report-2 package."""
 from __future__ import absolute_import, unicode_literals
 
 from django.db import models
+from django.utils import version
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 
-from django.utils import version
-
 from error_report.settings import ERROR_DETAIL_SETTINGS
 
 if version.get_complete_version() < (1, 10):
     from django.core.urlresolvers import reverse
 else:
     from django.urls import reverse
 
 
 class Error(models.Model):
-    """
-    Model for storing the individual errors.
-    """
+    """Model for storing the individual errors."""
     kind = models.CharField(_('type'),
                             null=True, blank=True, max_length=128, db_index=True
                             )
     info = models.TextField(
         null=False,
     )
     data = models.TextField(
@@ -35,28 +33,21 @@
     )
     html = models.TextField(
         null=True, blank=True,
     )
     modified = models.DateTimeField(auto_now=True)
 
     class Meta:
-        """
-        Meta information for the model.
-        """
+        """Meta information for the model."""
         verbose_name = _('Error')
         verbose_name_plural = _('Errors')
 
     def __unicode__(self):
-        """
-        String representation of the object.
-        """
+        """String representation of the object."""
         return "%s: %s" % (self.kind, self.info)
 
     def html_iframe(self):
-        """
-        Return an Iframe for Viewing Error detail in django admin
-        :return:
-        """
+        """Return an Iframe for Viewing Error detail in django admin."""
         return \
-            format_html('<iframe style="width: 100%; height: {}px;" src="{}"></iframe>',
-                        ERROR_DETAIL_SETTINGS.get('ERROR_DETAIL_HEIGHT', 1000),
-                        reverse('error-html-link', kwargs={'error': self.id}))
+            format_html('<iframe style="width: 100%; height: {height}px;" src="{link}"></iframe>',
+                        height=ERROR_DETAIL_SETTINGS.get('ERROR_DETAIL_HEIGHT', 1000),
+                        link=reverse('error-html-link', kwargs={'error': self.id}))
```

### Comparing `django-error-report-2-0.4.1/setup.py` & `django-error-report-2-0.4.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from os import path
-from setuptools import setup, find_packages
+"""Setup for django-error-report-2 package."""
 from codecs import open
+from os import path
 
+from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
@@ -33,9 +34,9 @@
     ],
     packages=find_packages(exclude=['build', 'dist', 'django_error_report.egg-info']),
     zip_safe=False,
     license="BSD License",
     install_requires=[
         'Django>=1.7'
     ],
-    version='0.4.1',
+    version='0.4.2',
 )
```

