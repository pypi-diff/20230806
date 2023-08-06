# Comparing `tmp/sqlconstructor-1.0.17.tar.gz` & `tmp/sqlconstructor-1.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlconstructor-1.0.17.tar", last modified: Fri Aug  4 03:11:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sqlconstructor-1.0.17.tar` & `sqlconstructor-1.0.18.tar`

### file list

```diff
@@ -1,20 +1,34 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:11:11.166810 sqlconstructor-1.0.17/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sqlconstructor-1.0.17/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8934 2023-08-04 03:11:11.166810 sqlconstructor-1.0.17/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8133 2023-08-04 03:10:31.000000 sqlconstructor-1.0.17/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      867 2023-08-04 03:05:49.000000 sqlconstructor-1.0.17/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-08-04 03:11:11.166810 sqlconstructor-1.0.17/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:11:11.164810 sqlconstructor-1.0.17/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:11:11.165810 sqlconstructor-1.0.17/src/sqlconstructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-08-04 01:04:49.000000 sqlconstructor-1.0.17/src/sqlconstructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-08-04 01:04:49.000000 sqlconstructor-1.0.17/src/sqlconstructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-08-04 01:04:50.000000 sqlconstructor-1.0.17/src/sqlconstructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5130 2023-08-04 02:53:00.000000 sqlconstructor-1.0.17/src/sqlconstructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1651 2023-08-04 01:40:25.000000 sqlconstructor-1.0.17/src/sqlconstructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5559 2023-08-04 01:16:46.000000 sqlconstructor-1.0.17/src/sqlconstructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-08-04 01:04:51.000000 sqlconstructor-1.0.17/src/sqlconstructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:11:11.166810 sqlconstructor-1.0.17/src/sqlconstructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8934 2023-08-04 03:11:11.000000 sqlconstructor-1.0.17/src/sqlconstructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      425 2023-08-04 03:11:11.000000 sqlconstructor-1.0.17/src/sqlconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-08-04 03:11:11.000000 sqlconstructor-1.0.17/src/sqlconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       15 2023-08-04 03:11:11.000000 sqlconstructor-1.0.17/src/sqlconstructor.egg-info/top_level.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/pytest.ini
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/__init__.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/constants.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/helpers.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_container.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_query.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/src/sqlconstructor/sql_section.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/simple_query_dict.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/select_section_of_simple_query.sql
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/fixtures/expected_examples/simple_query.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_container_filled_by_section_call.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_del_vars.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_init.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_reset_vars.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_set_vars.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_container/test_wrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_add.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_building_process.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_query/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_call_section.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_init.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/tests/test_sql_section/test_upper_sql_keywords.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/LICENSE
+-rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/pyproject.toml
+-rw-r--r--   0        0        0     9594 2020-02-02 00:00:00.000000 sqlconstructor-1.0.18/PKG-INFO
```

### Comparing `sqlconstructor-1.0.17/LICENSE` & `sqlconstructor-1.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.17/PKG-INFO` & `sqlconstructor-1.0.18/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlconstructor
-Version: 1.0.17
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
-Author-email: Andrey Smirnov <abc-sm@yandex.ru>
-Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
-Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
-Project-URL: Telegram, https://t.me/sqlconstructor
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -38,101 +23,124 @@
 q = sc.SqlQuery()
 # register as many SqlSection instances as you'd like
 q['select'](
     'id',
     'name',
 )
 q['from'](
-    'catalog'
+    'product'
 )
 q['where'](
-    "name = 'Smart'"
+    "quality = 'Best'",
+    'and brand_id = 1',
 )
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
+### Output
+SqlSection automatically transform all sql keywords in uppercase.
+It does not upper in following cases:
+1) if sql keyword is located in inline/multiline comment.
+2) if sql keyword is located inside single/double quotes.
+Output of sql_text is
+```sql
+SELECT
+  id,
+  name
+FROM
+  product
+WHERE
+  quality = 'Best'
+  AND brand_id = 1
+```
 ### Another portion of theory
 1) Because of sql headers ('select', 'from' and etc.) cannot be unique that's why it is only possible to append sql sections (but not get it back by index).
 2) We register (i.e. append) SqlSection by \_\_getitem\_\_ method of SqlQuery. It is possible to add sections with duplicate header. Header can be any string! SqlSection instances will be written in query in order you set them.
 3) When we call \_\_call\_\_ method of SqlSection we build SqlContainer of SqlSection (combining sql header with values passed by arguments).
 
 
 ### Build query with placeholders to be replaced by variables later
 You could add placeholder in query by adding **$variable_name** syntax.
 #### Set variable instantly
 ```python
 import sqlconstructor as sc
 
 
-def get_product_query(prod_name: str) -> sc.SqlContainer:
+def get_product_query(
+    product_quality: str, 
+    brand_identifier: int,
+) -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
     )
     q['from'](
-        'catalog'
+        'product'
     )
     q['where'](
-        'name = $product_name'
-    )(product_name=prod_name)
+        'quality = $quality',
+        'and brand_id = $brand_id'
+    )(qulaity=product_quality, brand_id=brand_identifier)
     q['order by']('name DESC')
     container: sc.SqlContainer = q()
     return container
 ```
 
 #### or later in SqlContainer
 ```python
 import sqlconstructor as sc
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variable to existing container
-    container(product_name='Smart')
+    # set variables to existing container
+    container(quality='Best', brand_id=1)
     # or
-    container.vars['product_name'] = 'Smart'
+    container.vars['quality'] = 'Best'
+    container.vars['brand_id'] = 1
 
     # if you would like to rewrite all vars
-    new_vars = {'product_name': 'Smart'}
+    new_vars = {'quality': 'Medium', 'brand_id': 2}
     container.vars = new_vars
 
     # if you would like to remove all vars
     container.vars.clear()
 
 
 def get_product_query() -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
     )
     q['from'](
-        'catalog'
+        'product'
     )
     q['where'](
-        'name = $product_name'
+        'quality = $quality',
+        'and brand_id = $brand_id'
     )
     container: sc.SqlContainer = q()
     return container
 ```
 
 ### You could cache SqlContainer and set/change variables later
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variable to existing container
-    container(product_name='Smart')
+    # set variables to existing container
+    container(quality='Best', brand_id=1)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
 
@@ -140,15 +148,15 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    container.vars['product_name'] = 'Smart'
+    container.vars.update({'quality': 'Best', 'brand_id': 1})
     # to replace placeholders by variables call 'dumps' method
     sql_text: str = container.dumps()
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
@@ -157,15 +165,15 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    container.vars['product_name'] = 'Smart'
+    container.vars.update({'quality': 'Best', 'brand_id': 1})
     # get sql without replacing placeholders by variables
     sql_text: str = str(container)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
@@ -177,31 +185,34 @@
 import sqlconstructor as sc
 from typing import List
 
 
 def main():
     q = sc.SqlQuery()
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
     q['from'](
-        'catalog as c',
+        'product as p',
     )
     q['left join lateral'](
         get_left_join_lateral(),
     )
-    q['where']('c.name = $product_name')(product_name='Smart')
+    q['where'](
+      'p.quality = $quality',
+      'and brand_id = $brand_id'
+    )(quality='Best', brand_id=1)
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
     j = sc.SqlQuery()
     j['select'](
-        'id',
-        'expiration_date',
+        'e.id',
+        'e.expiration_date',
     )
     j['from']('expiration as e')
     j['where'](*get_filters())
     j['limit'](100)
     """
     You could get SqlContainer with wrapped subquery 
     in some different ways:
@@ -212,43 +223,43 @@
     # or more explicit
     return j().wrap('AS exp ON TRUE')
 
 
 def get_filters() -> List[str]:
     """Create filters"""
     where = []
-    where.append('c.id = e.id')
-    where.append('AND expiration_date <= now()')
+    where.append('p.id = e.id')
+    where.append('AND e.expiration_date <= now()')
     return where
 ```
-### Append simple sql statements to query
+### Append simple string (simple sql statement) to query
 
 It is possible to append string or any SqlContainer to query as new SqlSection without header in this way:
 ```python
 import sqlconstructor as sc
 
 
 def main():
     q = sc.SqlQuery()
     q += '-- some comment here'
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
 ```
-### Append ready SqlContainer to query
+### Append SqlContainer to query
 ```python
 import sqlconstructor as sc
 
 
 def main():
     q = sc.SqlQuery()
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
     q += get_from_statement()
     ...
 
 
 def get_from_statement() -> sc.SqlContainer:
     ...
```

### Comparing `sqlconstructor-1.0.17/README.md` & `sqlconstructor-1.0.18/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: sqlconstructor
+Version: 1.0.18
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
+Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
+Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
+Project-URL: Telegram, https://t.me/sqlconstructor
+Author-email: Andrey Smirnov <abc-sm@yandex.ru>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -23,101 +38,124 @@
 q = sc.SqlQuery()
 # register as many SqlSection instances as you'd like
 q['select'](
     'id',
     'name',
 )
 q['from'](
-    'catalog'
+    'product'
 )
 q['where'](
-    "name = 'Smart'"
+    "quality = 'Best'",
+    'and brand_id = 1',
 )
 
 # build query into SqlContainer
 container: sc.SqlContainer = q()
 # get sql as string
 sql_text: str = str(container)
 ```
+### Output
+SqlSection automatically transform all sql keywords in uppercase.
+It does not upper in following cases:
+1) if sql keyword is located in inline/multiline comment.
+2) if sql keyword is located inside single/double quotes.
+Output of sql_text is
+```sql
+SELECT
+  id,
+  name
+FROM
+  product
+WHERE
+  quality = 'Best'
+  AND brand_id = 1
+```
 ### Another portion of theory
 1) Because of sql headers ('select', 'from' and etc.) cannot be unique that's why it is only possible to append sql sections (but not get it back by index).
 2) We register (i.e. append) SqlSection by \_\_getitem\_\_ method of SqlQuery. It is possible to add sections with duplicate header. Header can be any string! SqlSection instances will be written in query in order you set them.
 3) When we call \_\_call\_\_ method of SqlSection we build SqlContainer of SqlSection (combining sql header with values passed by arguments).
 
 
 ### Build query with placeholders to be replaced by variables later
 You could add placeholder in query by adding **$variable_name** syntax.
 #### Set variable instantly
 ```python
 import sqlconstructor as sc
 
 
-def get_product_query(prod_name: str) -> sc.SqlContainer:
+def get_product_query(
+    product_quality: str, 
+    brand_identifier: int,
+) -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
     )
     q['from'](
-        'catalog'
+        'product'
     )
     q['where'](
-        'name = $product_name'
-    )(product_name=prod_name)
+        'quality = $quality',
+        'and brand_id = $brand_id'
+    )(qulaity=product_quality, brand_id=brand_identifier)
     q['order by']('name DESC')
     container: sc.SqlContainer = q()
     return container
 ```
 
 #### or later in SqlContainer
 ```python
 import sqlconstructor as sc
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variable to existing container
-    container(product_name='Smart')
+    # set variables to existing container
+    container(quality='Best', brand_id=1)
     # or
-    container.vars['product_name'] = 'Smart'
+    container.vars['quality'] = 'Best'
+    container.vars['brand_id'] = 1
 
     # if you would like to rewrite all vars
-    new_vars = {'product_name': 'Smart'}
+    new_vars = {'quality': 'Medium', 'brand_id': 2}
     container.vars = new_vars
 
     # if you would like to remove all vars
     container.vars.clear()
 
 
 def get_product_query() -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
     )
     q['from'](
-        'catalog'
+        'product'
     )
     q['where'](
-        'name = $product_name'
+        'quality = $quality',
+        'and brand_id = $brand_id'
     )
     container: sc.SqlContainer = q()
     return container
 ```
 
 ### You could cache SqlContainer and set/change variables later
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variable to existing container
-    container(product_name='Smart')
+    # set variables to existing container
+    container(quality='Best', brand_id=1)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
 
@@ -125,15 +163,15 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    container.vars['product_name'] = 'Smart'
+    container.vars.update({'quality': 'Best', 'brand_id': 1})
     # to replace placeholders by variables call 'dumps' method
     sql_text: str = container.dumps()
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
@@ -142,15 +180,15 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    container.vars['product_name'] = 'Smart'
+    container.vars.update({'quality': 'Best', 'brand_id': 1})
     # get sql without replacing placeholders by variables
     sql_text: str = str(container)
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
@@ -162,31 +200,34 @@
 import sqlconstructor as sc
 from typing import List
 
 
 def main():
     q = sc.SqlQuery()
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
     q['from'](
-        'catalog as c',
+        'product as p',
     )
     q['left join lateral'](
         get_left_join_lateral(),
     )
-    q['where']('c.name = $product_name')(product_name='Smart')
+    q['where'](
+      'p.quality = $quality',
+      'and brand_id = $brand_id'
+    )(quality='Best', brand_id=1)
 
 
 def get_left_join_lateral() -> sc.SqlContainer:
     j = sc.SqlQuery()
     j['select'](
-        'id',
-        'expiration_date',
+        'e.id',
+        'e.expiration_date',
     )
     j['from']('expiration as e')
     j['where'](*get_filters())
     j['limit'](100)
     """
     You could get SqlContainer with wrapped subquery 
     in some different ways:
@@ -197,43 +238,43 @@
     # or more explicit
     return j().wrap('AS exp ON TRUE')
 
 
 def get_filters() -> List[str]:
     """Create filters"""
     where = []
-    where.append('c.id = e.id')
-    where.append('AND expiration_date <= now()')
+    where.append('p.id = e.id')
+    where.append('AND e.expiration_date <= now()')
     return where
 ```
-### Append simple sql statements to query
+### Append simple string (simple sql statement) to query
 
 It is possible to append string or any SqlContainer to query as new SqlSection without header in this way:
 ```python
 import sqlconstructor as sc
 
 
 def main():
     q = sc.SqlQuery()
     q += '-- some comment here'
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
 ```
-### Append ready SqlContainer to query
+### Append SqlContainer to query
 ```python
 import sqlconstructor as sc
 
 
 def main():
     q = sc.SqlQuery()
     q['select'](
-        'c.id',
-        'c.name',
+        'p.id',
+        'p.name',
     )
     q += get_from_statement()
     ...
 
 
 def get_from_statement() -> sc.SqlContainer:
     ...
```

### Comparing `sqlconstructor-1.0.17/pyproject.toml` & `sqlconstructor-1.0.18/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.17"
+version = "1.0.18"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.17/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.18/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.17/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.18/src/sqlconstructor/sql_container.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.17/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.18/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.17/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.18/src/sqlconstructor/sql_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             parentheses and optionally add text after parentheses. If wrapper_text is provided
             and is not None then do wrap SQL query with parentheses and add 'wrap' value
             after parentheses (empty string is possible). If you provide an empty string
             in 'wrap' argument then only parentheses will wrap SQL query text.
             - ind : int - you could set additional indentation for each line of query text.
             But it is rarely used because nested subelements automatically add 2 space indentation.
         """
-        params = {'text': self.text(ind=ind)}
+        params = {'text': self.__text(ind=ind)}
         if wrap is not None:
             params['wrapper_text'] = wrap
         container = SqlContainer(**params)
 
         # inherit all vars of included containers
         vars_of_containers = {
             key: value
@@ -121,21 +121,20 @@
         self.add(text)
         return self
 
     def add(self, text: str | SqlContainer):
         """Add text as sql section"""
         self[''](text)
 
-    def text(
+    def __text(
         self,
         ind: int = 0,  # indentation
     ) -> str:
         """
-        Usually called automatically when you use __call__ method.
-        Rarely called directly.
+        Used in __call__ method.
         Description:
             - Build SQL text by SQL sections and return string (not SqlContainer!).
         Params:
             - ind: int - add additional indentation for each line of SQL query.
         """
         sections = [section.container for section in self.sections if section]
         query_text = '\n'.join(str(x) for x in sections) if sections else ''
```

### Comparing `sqlconstructor-1.0.17/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.18/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

