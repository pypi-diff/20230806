# Comparing `tmp/zfl_data-0.0.3.tar.gz` & `tmp/zfl_data-0.0.4.tar.gz`

## Comparing `zfl_data-0.0.3.tar` & `zfl_data-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,17 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/admin.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/apps.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/models.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/tests.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/urls.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/views.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/management/commands/analytics_api.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/management/commands/updates.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0001_initial.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0002_webdata.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0003_remove_webdata_user_date.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0004_godate.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0005_auto_20200727_1146.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0006_auto_20200808_1206.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0007_googleaccess.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0008_auto_20210327_0952.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/static/data/css/data-style.css
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/templates/data/index.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 zfl_data-0.0.3/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.3/README.md
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 zfl_data-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/admin.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/apps.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/models.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/tests.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/urls.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/views.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/management/commands/analytics_api.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/management/commands/updates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/static/data/css/data-style.css
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.4/data/templates/data/index.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 zfl_data-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.4/README.md
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 zfl_data-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.4/PKG-INFO
```

### Comparing `zfl_data-0.0.3/data/models.py` & `zfl_data-0.0.4/data/models.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/data/tests.py` & `zfl_data-0.0.4/data/tests.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/data/views.py` & `zfl_data-0.0.4/data/views.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/data/management/commands/analytics_api.py` & `zfl_data-0.0.4/data/management/commands/analytics_api.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/data/management/commands/updates.py` & `zfl_data-0.0.4/data/management/commands/updates.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/data/templates/data/index.html` & `zfl_data-0.0.4/data/templates/data/index.html`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/LICENSE.txt` & `zfl_data-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/README.md` & `zfl_data-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.3/pyproject.toml` & `zfl_data-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -127,9 +127,9 @@
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 
 # ビルド実行時に含めるファイルと含めないファイルの設定
 # 以下は配布用Djangoアプリに対しての設定
 [tool.hatch.build]
 include = ["data/*"]
-# exclude = ["data/migrations/*"]
+exclude = ["data/migrations/*"]
```

### Comparing `zfl_data-0.0.3/PKG-INFO` & `zfl_data-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfl-data
-Version: 0.0.3
+Version: 0.0.4
 Summary: 'data on zfl'
 Project-URL: Documentation, https://github.com/unknown/Appのパッケージ名#readme
 Project-URL: Issues, https://github.com/unknown/Appのパッケージ名/issues
 Project-URL: Source, https://github.com/unknown/Appのパッケージ名
 Author-email: You are name <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

