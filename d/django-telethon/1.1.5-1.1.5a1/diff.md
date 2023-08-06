# Comparing `tmp/django-telethon-1.1.5.tar.gz` & `tmp/django-telethon-1.1.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-telethon-1.1.5.tar", last modified: Thu Nov  3 20:09:26 2022, max compression
+gzip compressed data, was "dist/django-telethon-1.1.5a1.tar", last modified: Thu Nov  3 20:08:29 2022, max compression
```

## Comparing `django-telethon-1.1.5.tar` & `django-telethon-1.1.5a1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-11-03 19:52:50.000000 django-telethon-1.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-11-03 19:52:50.000000 django-telethon-1.1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10937 2022-11-03 20:09:26.000000 django-telethon-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9711 2022-11-03 19:52:50.000000 django-telethon-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon/
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/management/commands/runtelegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7810 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon/models/
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2055 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1438 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/sentfiles.py
--rw-rw-rw-   0 root         (0) root         (0)     1830 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      720 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/models/states.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/receivers.py
--rw-rw-rw-   0 root         (0) root         (0)     9016 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/signals.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4164 2022-11-03 19:52:50.000000 django-telethon-1.1.5/django_telethon/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2022-11-03 20:08:23.000000 django-telethon-1.1.5/django_telethon/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10937 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      949 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-03 20:09:26.000000 django-telethon-1.1.5/django_telethon.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      266 2022-11-03 19:52:50.000000 django-telethon-1.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-11-03 20:09:26.000000 django-telethon-1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1856 2022-11-03 20:09:21.000000 django-telethon-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       98 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10939 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9711 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/management/commands/runtelegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7810 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon/models/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/sentfiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      720 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/models/states.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/receivers.py
+-rw-rw-rw-   0 root         (0) root         (0)     9016 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      135 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/django_telethon/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2022-11-03 20:08:23.000000 django-telethon-1.1.5a1/django_telethon/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10939 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      949 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/django_telethon.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      266 2022-11-03 19:52:50.000000 django-telethon-1.1.5a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      229 2022-11-03 20:08:29.000000 django-telethon-1.1.5a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2022-11-03 20:08:24.000000 django-telethon-1.1.5a1/setup.py
```

### Comparing `django-telethon-1.1.5/LICENSE` & `django-telethon-1.1.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/PKG-INFO` & `django-telethon-1.1.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.1.5
+Version: 1.1.5a1
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-telethon-1.1.5/README.md` & `django-telethon-1.1.5a1/README.md`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/admin.py` & `django-telethon-1.1.5a1/django_telethon/admin.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/management/commands/runtelegram.py` & `django-telethon-1.1.5a1/django_telethon/management/commands/runtelegram.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/migrations/0001_initial.py` & `django-telethon-1.1.5a1/django_telethon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/models/entities.py` & `django-telethon-1.1.5a1/django_telethon/models/entities.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/models/login.py` & `django-telethon-1.1.5a1/django_telethon/models/login.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/models/sentfiles.py` & `django-telethon-1.1.5a1/django_telethon/models/sentfiles.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/models/sessions.py` & `django-telethon-1.1.5a1/django_telethon/models/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/models/states.py` & `django-telethon-1.1.5a1/django_telethon/models/states.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/receivers.py` & `django-telethon-1.1.5a1/django_telethon/receivers.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/sessions.py` & `django-telethon-1.1.5a1/django_telethon/sessions.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/utils.py` & `django-telethon-1.1.5a1/django_telethon/utils.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon/views.py` & `django-telethon-1.1.5a1/django_telethon/views.py`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/django_telethon.egg-info/PKG-INFO` & `django-telethon-1.1.5a1/django_telethon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-telethon
-Version: 1.1.5
+Version: 1.1.5a1
 Summary: Telethon for django
 Home-page: https://github.com/ali-zahedi/django-telethon
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-telethon-1.1.5/django_telethon.egg-info/SOURCES.txt` & `django-telethon-1.1.5a1/django_telethon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-telethon-1.1.5/setup.py` & `django-telethon-1.1.5a1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-telethon',
-    version='1.1.5',
+    version='1.1.5-alpha.1',
     packages=find_packages(),
     include_package_data=True,
     license='BSD License',
     description='Telethon for django',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/ali-zahedi/django-telethon',
```

