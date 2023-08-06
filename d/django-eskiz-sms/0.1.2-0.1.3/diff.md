# Comparing `tmp/django-eskiz-sms-0.1.2.tar.gz` & `tmp/django-eskiz-sms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-eskiz-sms-0.1.2.tar", last modified: Sat Jul 15 08:58:44 2023, max compression
+gzip compressed data, was "django-eskiz-sms-0.1.3.tar", last modified: Sat Jul 15 09:33:25 2023, max compression
```

## Comparing `django-eskiz-sms-0.1.2.tar` & `django-eskiz-sms-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/
--rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2285 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-07-15 08:58:18.000000 django-eskiz-sms-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.019740 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/
--rw-rw-rw-   0        0        0     2285 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.057302 django-eskiz-sms-0.1.2/eskiz_sms/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.2/eskiz_sms/__init__.py
--rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.2/eskiz_sms/admin.py
--rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.2/eskiz_sms/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.067866 django-eskiz-sms-0.1.2/eskiz_sms/migrations/
--rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.2/eskiz_sms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.2/eskiz_sms/migrations/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.2/eskiz_sms/models.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/eskiz_sms/templates/
--rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.2/eskiz_sms/templates/send_sms.html
--rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.2/eskiz_sms/urls.py
--rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.2/eskiz_sms/views.py
--rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      252 2023-07-15 08:58:44.084863 django-eskiz-sms-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1750 2023-07-15 08:56:03.000000 django-eskiz-sms-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.974462 django-eskiz-sms-0.1.3/
+-rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2313 2023-07-15 09:33:25.975478 django-eskiz-sms-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-07-15 09:33:10.000000 django-eskiz-sms-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.929465 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/
+-rw-rw-rw-   0        0        0     2313 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 09:33:25.000000 django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.957464 django-eskiz-sms-0.1.3/eskiz_sms/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.3/eskiz_sms/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.3/eskiz_sms/admin.py
+-rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.3/eskiz_sms/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.965457 django-eskiz-sms-0.1.3/eskiz_sms/migrations/
+-rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.3/eskiz_sms/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.3/eskiz_sms/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.3/eskiz_sms/models.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:33:25.969464 django-eskiz-sms-0.1.3/eskiz_sms/templates/
+-rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.3/eskiz_sms/templates/send_sms.html
+-rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.3/eskiz_sms/urls.py
+-rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.3/eskiz_sms/views.py
+-rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      252 2023-07-15 09:33:25.981458 django-eskiz-sms-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-07-15 09:21:22.000000 django-eskiz-sms-0.1.3/setup.py
```

### Comparing `django-eskiz-sms-0.1.2/PKG-INFO` & `django-eskiz-sms-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1.2
-Summary: Django Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
+Version: 0.1.3
+Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
 Home-page: https://github.com/Otajonov/django-eskiz-sms/tree/main
 Author: Ro'zmat Otajonov
 Author-email: hello@tijorat.org
 Maintainer: Ro'zmat Otajonov
 Maintainer-email: hello@tijorat.org
 License: MIT
 Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
@@ -31,18 +31,20 @@
 
 Djangodan EskizUz yordamida SMS yuborish uchun eng mukammal paket
 
 Paketni pip install django-eskiz-sms deb o'rnatib,
 asosiy appni settings.py ida INSTALLED_APPS ga eskiz_sms deb qo'shing.
 
 Makemigration va migratedan keyin django adminga o'ting.
-Makemigrationda xato bersa requests paketini ham pip install requests qilib o'rnatib oling!
 U yerda EskizSMS degan modelga EskizUZ emailingiz va kabinetdan olgan parolingizni kiriting.
 
 So'ngra asosiy urls.py ga eskiz_sms.urls ni include qiling, bu sms browserda forma orqali sms
 yuborib sinab ko'rish uchun. Xavfsizlik yuzasidan keyin uni uzib qo'ying.
+Bu faqat test uchun. Paketni asli quyidagi yo'l bilan ishlatasiz:
 
 Odatiy ishlatish uchun istalgan joyda from eskiz_sms.views import send_sms yoki boshqa
 yo'l bilan send_sms() degan metodni chaqirib ishlating. Qolgan ishlarni o'zi bajaradi.
 Shuningdek admin panelda SMSLog orqali jo'natilgan SMSlar statistikasini ko'rib tursangiz bo'ladi.
 
+
+Yordam kerak bo'lsa Telegram: https://t.me/a1ie9
 Ishlatish uchun batafsil qo'llanma: https://docs.tijorat.org/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1.2/README.rst` & `django-eskiz-sms-0.1.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Djangodan EskizUz yordamida SMS yuborish uchun eng mukammal paket
 
 Paketni pip install django-eskiz-sms deb o'rnatib,
 asosiy appni settings.py ida INSTALLED_APPS ga eskiz_sms deb qo'shing.
 
 Makemigration va migratedan keyin django adminga o'ting.
-Makemigrationda xato bersa requests paketini ham pip install requests qilib o'rnatib oling!
 U yerda EskizSMS degan modelga EskizUZ emailingiz va kabinetdan olgan parolingizni kiriting.
 
 So'ngra asosiy urls.py ga eskiz_sms.urls ni include qiling, bu sms browserda forma orqali sms
 yuborib sinab ko'rish uchun. Xavfsizlik yuzasidan keyin uni uzib qo'ying.
+Bu faqat test uchun. Paketni asli quyidagi yo'l bilan ishlatasiz:
 
 Odatiy ishlatish uchun istalgan joyda from eskiz_sms.views import send_sms yoki boshqa
 yo'l bilan send_sms() degan metodni chaqirib ishlating. Qolgan ishlarni o'zi bajaradi.
 Shuningdek admin panelda SMSLog orqali jo'natilgan SMSlar statistikasini ko'rib tursangiz bo'ladi.
 
+
+Yordam kerak bo'lsa Telegram: https://t.me/a1ie9
 Ishlatish uchun batafsil qo'llanma: https://docs.tijorat.org/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/PKG-INFO` & `django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-eskiz-sms
-Version: 0.1.2
-Summary: Django Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
+Version: 0.1.3
+Summary: Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket
 Home-page: https://github.com/Otajonov/django-eskiz-sms/tree/main
 Author: Ro'zmat Otajonov
 Author-email: hello@tijorat.org
 Maintainer: Ro'zmat Otajonov
 Maintainer-email: hello@tijorat.org
 License: MIT
 Project-URL: Batafsil qo'llanma, https://docs.tijorat.org/django-eskiz-sms
@@ -31,18 +31,20 @@
 
 Djangodan EskizUz yordamida SMS yuborish uchun eng mukammal paket
 
 Paketni pip install django-eskiz-sms deb o'rnatib,
 asosiy appni settings.py ida INSTALLED_APPS ga eskiz_sms deb qo'shing.
 
 Makemigration va migratedan keyin django adminga o'ting.
-Makemigrationda xato bersa requests paketini ham pip install requests qilib o'rnatib oling!
 U yerda EskizSMS degan modelga EskizUZ emailingiz va kabinetdan olgan parolingizni kiriting.
 
 So'ngra asosiy urls.py ga eskiz_sms.urls ni include qiling, bu sms browserda forma orqali sms
 yuborib sinab ko'rish uchun. Xavfsizlik yuzasidan keyin uni uzib qo'ying.
+Bu faqat test uchun. Paketni asli quyidagi yo'l bilan ishlatasiz:
 
 Odatiy ishlatish uchun istalgan joyda from eskiz_sms.views import send_sms yoki boshqa
 yo'l bilan send_sms() degan metodni chaqirib ishlating. Qolgan ishlarni o'zi bajaradi.
 Shuningdek admin panelda SMSLog orqali jo'natilgan SMSlar statistikasini ko'rib tursangiz bo'ladi.
 
+
+Yordam kerak bo'lsa Telegram: https://t.me/a1ie9
 Ishlatish uchun batafsil qo'llanma: https://docs.tijorat.org/django-eskiz-sms
```

### Comparing `django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/SOURCES.txt` & `django-eskiz-sms-0.1.3/django_eskiz_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/eskiz_sms/admin.py` & `django-eskiz-sms-0.1.3/eskiz_sms/admin.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/eskiz_sms/migrations/0001_initial.py` & `django-eskiz-sms-0.1.3/eskiz_sms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/eskiz_sms/models.py` & `django-eskiz-sms-0.1.3/eskiz_sms/models.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/eskiz_sms/templates/send_sms.html` & `django-eskiz-sms-0.1.3/eskiz_sms/templates/send_sms.html`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/eskiz_sms/views.py` & `django-eskiz-sms-0.1.3/eskiz_sms/views.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.2/setup.py` & `django-eskiz-sms-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 f = open("README.rst")
 readme = f.read()
 f.close()
 
 
 setup(
     name="django-eskiz-sms",
     version=__version__,
     description=(
-        "Django Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket"
+        "Djangoda Eskiz.Uz API orqali SMS yuborish uchun eng mukammal paket"
     ),
     long_description=readme,
     author="Ro'zmat Otajonov",
     author_email="hello@tijorat.org",
     maintainer="Ro'zmat Otajonov",
     maintainer_email="hello@tijorat.org",
     url="https://github.com/Otajonov/django-eskiz-sms/tree/main",
@@ -48,9 +48,10 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     zip_safe=False,
     python_requires=">=3.7",
     install_requires=[
         "Django>=3.2",
+        "requests",
     ],
 )
```

