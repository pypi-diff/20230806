# Comparing `tmp/django_vite_plugin-1.3.0.tar.gz` & `tmp/django_vite_plugin-1.3.1.tar.gz`

## Comparing `django_vite_plugin-1.3.0.tar` & `django_vite_plugin-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/__init__.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/config_helper.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/urls.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/management/commands/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/management/commands/django_vite_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/templatetags/__init__.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/src/django_vite_plugin/templatetags/vite.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/LICENSE
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/__init__.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/config_helper.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/urls.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/management/commands/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/management/commands/django_vite_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/templatetags/__init__.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/src/django_vite_plugin/templatetags/vite.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 django_vite_plugin-1.3.1/PKG-INFO
```

### Comparing `django_vite_plugin-1.3.0/src/django_vite_plugin/config_helper.py` & `django_vite_plugin-1.3.1/src/django_vite_plugin/config_helper.py`

 * *Files identical despite different names*

### Comparing `django_vite_plugin-1.3.0/src/django_vite_plugin/utils.py` & `django_vite_plugin-1.3.1/src/django_vite_plugin/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 if CONFIG['BUILD_URL_PREFIX'][-1] != "/":
     CONFIG['BUILD_URL_PREFIX'] += "/"
 
 if CONFIG['DEV_MODE'] is False and 'JS_ATTRS_BUILD' in CONFIG:
     CONFIG['JS_ATTRS'] = CONFIG['JS_ATTRS_BUILD']
 
 VITE_MANIFEST  = {}
-manifest_path = getattr(settings, 'BASE_DIR') / CONFIG['BUILD_DIR'].lstrip('/\\') / 'manifest.json'
+
+if isinstance(CONFIG['BUILD_DIR'], str):
+    manifest_path = getattr(settings, 'BASE_DIR') / CONFIG['BUILD_DIR'].lstrip('/\\')
+else:
+    manifest_path = CONFIG['BUILD_DIR']
+manifest_path = manifest_path / 'manifest.json'
+
 if not CONFIG['DEV_MODE'] and path.isfile(manifest_path):
     try:
         manifest_file = open(manifest_path, "r")
         manifest_content = manifest_file.read()
         manifest_file.close()
         VITE_MANIFEST = json.loads(manifest_content)
     except Exception as error:
```

### Comparing `django_vite_plugin-1.3.0/src/django_vite_plugin/management/commands/django_vite_plugin.py` & `django_vite_plugin-1.3.1/src/django_vite_plugin/management/commands/django_vite_plugin.py`

 * *Files identical despite different names*

### Comparing `django_vite_plugin-1.3.0/src/django_vite_plugin/templatetags/vite.py` & `django_vite_plugin-1.3.1/src/django_vite_plugin/templatetags/vite.py`

 * *Files identical despite different names*

### Comparing `django_vite_plugin-1.3.0/LICENSE` & `django_vite_plugin-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_vite_plugin-1.3.0/README.md` & `django_vite_plugin-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_vite_plugin-1.3.0/pyproject.toml` & `django_vite_plugin-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django_vite_plugin"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Sakibur Rahman Khan", email="sakib.saad.khan@gmail.com" },
 ]
 description = "Vite build tools integration for django"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_vite_plugin-1.3.0/PKG-INFO` & `django_vite_plugin-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_vite_plugin
-Version: 1.3.0
+Version: 1.3.1
 Summary: Vite build tools integration for django
 Project-URL: Homepage, https://github.com/protibimbok/django-vite-plugin
 Project-URL: Bug Tracker, https://github.com/protibimbok/django-vite-plugin/issues
 Author-email: Sakibur Rahman Khan <sakib.saad.khan@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_vite_plugin Version: 1.3.0 Summary: Vite
+Metadata-Version: 2.1 Name: django_vite_plugin Version: 1.3.1 Summary: Vite
 build tools integration for django Project-URL: Homepage, https://github.com/
 protibimbok/django-vite-plugin Project-URL: Bug Tracker, https://github.com/
 protibimbok/django-vite-plugin/issues Author-email: Sakibur Rahman Khan
 saad.khan@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-
 Type: text/markdown # Django Vite Plugin [![PyPI version](https://
```

