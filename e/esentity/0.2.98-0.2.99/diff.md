# Comparing `tmp/esentity-0.2.98.tar.gz` & `tmp/esentity-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esentity-0.2.98.tar", max compression
+gzip compressed data, was "esentity-0.2.99.tar", max compression
```

## Comparing `esentity-0.2.98.tar` & `esentity-0.2.99.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       23 2022-11-02 18:41:41.090413 esentity-0.2.98/esentity/__init__.py
--rw-r--r--   0        0        0   146246 2022-11-02 18:41:26.552044 esentity-0.2.98/esentity/api.py
--rw-r--r--   0        0        0     2304 2022-02-27 16:26:43.296489 esentity-0.2.98/esentity/encoder.py
--rw-r--r--   0        0        0    57941 2022-10-20 22:22:15.674127 esentity-0.2.98/esentity/ext.py
--rw-r--r--   0        0        0    58994 2022-10-20 22:22:04.553263 esentity-0.2.98/esentity/models.py
--rw-r--r--   0        0        0    12265 2022-02-27 16:25:40.743010 esentity-0.2.98/esentity/routes.py
--rw-r--r--   0        0        0    10560 2022-04-27 09:43:55.424029 esentity-0.2.98/esentity/tasks.py
--rw-r--r--   0        0        0     9258 2022-02-27 16:25:59.323595 esentity-0.2.98/esentity/telegram.py
--rw-r--r--   0        0        0      358 2022-11-02 18:41:47.544354 esentity-0.2.98/pyproject.toml
--rw-r--r--   0        0        0      538 2022-11-02 18:43:00.626819 esentity-0.2.98/setup.py
--rw-r--r--   0        0        0      399 2022-11-02 18:43:00.626956 esentity-0.2.98/PKG-INFO
+-rw-r--r--   0        0        0       23 2022-11-03 09:11:38.915830 esentity-0.2.99/esentity/__init__.py
+-rw-r--r--   0        0        0   146246 2022-11-03 09:11:23.929444 esentity-0.2.99/esentity/api.py
+-rw-r--r--   0        0        0     2304 2022-02-27 16:26:43.296489 esentity-0.2.99/esentity/encoder.py
+-rw-r--r--   0        0        0    57981 2022-11-03 09:11:11.804254 esentity-0.2.99/esentity/ext.py
+-rw-r--r--   0        0        0    58994 2022-10-20 22:22:04.553263 esentity-0.2.99/esentity/models.py
+-rw-r--r--   0        0        0    12265 2022-02-27 16:25:40.743010 esentity-0.2.99/esentity/routes.py
+-rw-r--r--   0        0        0    10560 2022-04-27 09:43:55.424029 esentity-0.2.99/esentity/tasks.py
+-rw-r--r--   0        0        0     9258 2022-02-27 16:25:59.323595 esentity-0.2.99/esentity/telegram.py
+-rw-r--r--   0        0        0      358 2022-11-03 09:11:44.887242 esentity-0.2.99/pyproject.toml
+-rw-r--r--   0        0        0      538 2022-11-03 09:11:53.093092 esentity-0.2.99/setup.py
+-rw-r--r--   0        0        0      399 2022-11-03 09:11:53.093219 esentity-0.2.99/PKG-INFO
```

### Comparing `esentity-0.2.98/esentity/api.py` & `esentity-0.2.99/esentity/api.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/esentity/encoder.py` & `esentity-0.2.99/esentity/encoder.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/esentity/ext.py` & `esentity-0.2.99/esentity/ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1800,33 +1800,35 @@
                     "size": aggs_count,
                     "order": {"_key": "asc"}
                 }
             } for item in aggs_fields
         }
 
         # args: service
-        pages, found, aggs, _ = Page.provider_by_context(
+        items, total, aggs, _ = Page.provider_by_context(
             is_searchable=True,
             is_redirect=False,
             country=current_user.country_full,
             services=service,
             provider_tags=tags,
             _locale=g.language,
             _source=True,
             _count=count,
             _aggs=_aggs,
         )
 
         t = current_app.jinja_env.get_template('_ext-rating_casinos.html')
         s = t.render(
-            pages=pages, 
-            found=f'{found} matching casinos', 
-            service=service, 
+            items=items, 
+            total=total, 
             count=count,
+            percent=20,
+            service=service, 
             tags=tags,
+            cnt_casinos_total='1000',
             aggs=process_aggs(aggs, 'provider_tags', tags_enabled),
         )
         return s
 
     def parse(self, parser):
         lineno = next(parser.stream).lineno
```

### Comparing `esentity-0.2.98/esentity/models.py` & `esentity-0.2.99/esentity/models.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/esentity/routes.py` & `esentity-0.2.99/esentity/routes.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/esentity/tasks.py` & `esentity-0.2.99/esentity/tasks.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/esentity/telegram.py` & `esentity-0.2.99/esentity/telegram.py`

 * *Files identical despite different names*

### Comparing `esentity-0.2.98/setup.py` & `esentity-0.2.99/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['esentity']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'esentity',
-    'version': '0.2.98',
+    'version': '0.2.99',
     'description': 'Elasticsearch Entity Tools',
     'long_description': None,
     'author': 'Slotmarks',
     'author_email': 'info@slotmarks.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://slotmarks.com',
```

