# Comparing `tmp/django-eskiz-sms-0.1.3.tar.gz` & `tmp/django-eskiz-sms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-eskiz-sms-0.1.3.tar", last modified: Sat Jul 15 09:33:25 2023, max compression
+gzip compressed data, was "django-eskiz-sms-0.1.4.tar", last modified: Sun Aug  6 15:03:10 2023, max compression
```

## Comparing `django-eskiz-sms-0.1.3.tar` & `django-eskiz-sms-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.974462 django-eskiz-sms-0.1.3/
--rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2313 2023-07-15 09:33:25.975478 django-eskiz-sms-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-07-15 09:33:10.000000 django-eskiz-sms-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.929465 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/
--rw-rw-rw-   0        0        0     2313 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.957464 django-eskiz-sms-0.1.3/eskiz_sms/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.3/eskiz_sms/__init__.py
--rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.3/eskiz_sms/admin.py
--rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.3/eskiz_sms/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.965457 django-eskiz-sms-0.1.3/eskiz_sms/migrations/
--rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.3/eskiz_sms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.3/eskiz_sms/migrations/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.3/eskiz_sms/models.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.969464 django-eskiz-sms-0.1.3/eskiz_sms/templates/
--rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.3/eskiz_sms/templates/send_sms.html
--rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.3/eskiz_sms/urls.py
--rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.3/eskiz_sms/views.py
--rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      252 2023-07-15 09:33:25.981458 django-eskiz-sms-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1773 2023-07-15 09:21:22.000000 django-eskiz-sms-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:03:10.646691 django-eskiz-sms-0.1.4/
+-rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2291 2023-08-06 15:03:10.647686 django-eskiz-sms-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-07-15 09:33:10.000000 django-eskiz-sms-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-06 15:03:10.571051 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/
+-rw-rw-rw-   0        0        0     2291 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 15:03:10.000000 django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:03:10.592053 django-eskiz-sms-0.1.4/eskiz_sms/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.4/eskiz_sms/__init__.py
+-rw-rw-rw-   0        0        0      799 2023-08-06 15:02:08.000000 django-eskiz-sms-0.1.4/eskiz_sms/admin.py
+-rw-rw-rw-   0        0        0      187 2023-08-06 14:48:21.000000 django-eskiz-sms-0.1.4/eskiz_sms/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:03:10.595057 django-eskiz-sms-0.1.4/eskiz_sms/migrations/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.4/eskiz_sms/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-08-06 14:49:27.000000 django-eskiz-sms-0.1.4/eskiz_sms/models.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:03:10.644689 django-eskiz-sms-0.1.4/eskiz_sms/templates/
+-rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.4/eskiz_sms/templates/send_sms.html
+-rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.4/eskiz_sms/urls.py
+-rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.4/eskiz_sms/views.py
+-rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      252 2023-08-06 15:03:10.651686 django-eskiz-sms-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1751 2023-08-06 14:36:22.000000 django-eskiz-sms-0.1.4/setup.py
```

### Comparing `django-eskiz-sms-0.1.3/PKG-INFO` & `django-eskiz-sms-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1.3
+Version: 0.1.4
 Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
-Home-page: https://github.com/Otajonov/django-eskiz-sms/tree/main
+Home-page: https://docs.tijorat.org/django/
 Author: Ro'zmat Otajonov
 Author-email: hello@tijorat.org
 Maintainer: Ro'zmat Otajonov
 Maintainer-email: hello@tijorat.org
 License: MIT
 Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
 Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1.3/README.rst` & `django-eskiz-sms-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/PKG-INFO` & `django-eskiz-sms-0.1.4/django_eskiz_sms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1.3
+Version: 0.1.4
 Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
-Home-page: https://github.com/Otajonov/django-eskiz-sms/tree/main
+Home-page: https://docs.tijorat.org/django/
 Author: Ro'zmat Otajonov
 Author-email: hello@tijorat.org
 Maintainer: Ro'zmat Otajonov
 Maintainer-email: hello@tijorat.org
 License: MIT
 Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
 Project-URL: GitHub Soure Code, https://github.com/Otajonov/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1.3/eskiz_sms/admin.py` & `django-eskiz-sms-0.1.4/eskiz_sms/admin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from django.contrib import admin
 from .models import EskizSMS, SMSLog
 
 
 @admin.register(EskizSMS)
 class EskizSMSAdmin(admin.ModelAdmin):
-    list_display = ('email', 'password', 'from_name', 'callback_url', 'last_updated', 'eskiz_token')
+    list_display = ('email', 'from_name', 'callback_url', 'last_updated', 'eskiz_token')
+    
+    def get_readonly_fields(self, request, obj=None):
+        return ['last_updated', 'eskiz_token']
 
 
 @admin.register(SMSLog)
 class SMSLogAdmin(admin.ModelAdmin):
-    list_display = ('phone_number', 'message', 'from_name', 'status', 'status_date', 'error_message', 'from_app')
+    list_display = ('phone_number', 'message', 'from_name', 'status', 'status_date',  'from_app', 'error_message')
     list_filter = ['status', 'from_app', 'from_name', 'status_date' ]
     search_fields = ['phone_number', 'message' ]
+    
+    def has_add_permission(self, request):
+        return False
+
+    def has_change_permission(self, request, obj=None):
+        return False
```

### Comparing `django-eskiz-sms-0.1.3/eskiz_sms/templates/send_sms.html` & `django-eskiz-sms-0.1.4/eskiz_sms/templates/send_sms.html`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.3/eskiz_sms/views.py` & `django-eskiz-sms-0.1.4/eskiz_sms/views.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.3/setup.py` & `django-eskiz-sms-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 f = open("README.rst")
 readme = f.read()
 f.close()
 
 
 setup(
@@ -15,15 +15,15 @@
         "Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket"
     ),
     long_description=readme,
     author="Ro'zmat Otajonov",
     author_email="hello@tijorat.org",
     maintainer="Ro'zmat Otajonov",
     maintainer_email="hello@tijorat.org",
-    url="https://github.com/Otajonov/django-eskiz-sms/tree/main",
+    url="https://docs.tijorat.org/django/",
     packages=find_packages(exclude=["tests*"]),
     
     project_urls={
         "Batafsil qo'llanma": "https://docs.tijorat.org/django-eskiz-sms",
         "GitHub Soure Code": "https://github.com/Otajonov/django-eskiz-sms",
     },
```

