# Comparing `tmp/zfl_data-0.0.2.tar.gz` & `tmp/zfl_data-0.0.3.tar.gz`

## Comparing `zfl_data-0.0.2.tar` & `zfl_data-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/admin.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/apps.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/models.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/tests.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/urls.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/views.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/management/commands/analytics_api.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/management/commands/updates.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0001_initial.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0002_webdata.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0003_remove_webdata_user_date.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0004_godate.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0005_auto_20200727_1146.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0006_auto_20200808_1206.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0007_googleaccess.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0008_auto_20210327_0952.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/static/data/css/data-style.css
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/templates/data/index.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 zfl_data-0.0.2/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.2/README.md
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 zfl_data-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/admin.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/apps.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/models.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/tests.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/urls.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/views.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/management/commands/analytics_api.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/management/commands/updates.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0001_initial.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0002_webdata.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0003_remove_webdata_user_date.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0004_godate.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0005_auto_20200727_1146.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0006_auto_20200808_1206.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0007_googleaccess.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/0008_auto_20210327_0952.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/static/data/css/data-style.css
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.3/data/templates/data/index.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 zfl_data-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.3/README.md
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 zfl_data-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.3/PKG-INFO
```

### Comparing `zfl_data-0.0.2/data/models.py` & `zfl_data-0.0.3/data/models.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/tests.py` & `zfl_data-0.0.3/data/tests.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/views.py` & `zfl_data-0.0.3/data/views.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/management/commands/analytics_api.py` & `zfl_data-0.0.3/data/management/commands/analytics_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 
 
 SCOPES = ['https://www.googleapis.com/auth/analytics.readonly']
 KEY_FILE_LOCATION = os.path.join(settings.ZEROFROMLIGHT_DIR, 'client_secrets.json')
 VIEW_ID = settings.ZEROFROMLIGHT_KEYS['VIEW_ID']
 
 # 12ヵ月前の年・月・日を取得
-months_age_12 = (datetime.datetime.today() - relativedelta(months=12)).strftime("%Y-%m-%d")
+months_age_13 = (datetime.datetime.today() - relativedelta(months=13)).strftime("%Y-%m-%d")
 
 
 def initialize_analyticsreporting():
     credentials = ServiceAccountCredentials.from_json_keyfile_name(
                             KEY_FILE_LOCATION, SCOPES)
     analytics = build('analyticsreporting', 'v4', credentials=credentials)
     return analytics
 
 
-def get_report(analytics):
-    """
-    ブログ閲覧数取得
-
-    """
-    return analytics.reports().batchGet(
-            body={
-            'reportRequests': [{
-                'viewId': VIEW_ID,
-                'pageSize': 10,
-                'dateRanges': [{"startDate": "3daysAgo", "endDate": "today"}],
-                'dimensions': [{'name': 'ga:pagePath'}, {'name': 'ga:pageTitle'}],
-                'dimensionFilterClauses': [{'filters': [{'dimensionName': 'ga:pagePath',
-                                                       'expressions': ['/blogs/detail/']}]
-                                           }],
-                'metrics': [{'expression': 'ga:pageviews'}],
-                'orderBys': [{'fieldName': 'ga:pageviews', 'sortOrder': 'DESCENDING'}],
-             }]
-            }
-            ).execute()
+# def get_report(analytics):
+#     """
+#     ブログ閲覧数取得
+# 
+#     """
+#     return analytics.reports().batchGet(
+#             body={
+#             'reportRequests': [{
+#                 'viewId': VIEW_ID,
+#                 'pageSize': 10,
+#                 'dateRanges': [{"startDate": "3daysAgo", "endDate": "today"}],
+#                 'dimensions': [{'name': 'ga:pagePath'}, {'name': 'ga:pageTitle'}],
+#                 'dimensionFilterClauses': [{'filters': [{'dimensionName': 'ga:pagePath',
+#                                                        'expressions': ['/blogs/detail/']}]
+#                                            }],
+#                 'metrics': [{'expression': 'ga:pageviews'}],
+#                 'orderBys': [{'fieldName': 'ga:pageviews', 'sortOrder': 'DESCENDING'}],
+#              }]
+#             }
+#             ).execute()
 
 
 def get_report_web(analytics):
     """
     本日のアクセス数取得
 
     """
     return analytics.reports().batchGet(
             body={
             'reportRequests': [{
                 'viewId': VIEW_ID,
-                'dateRanges': [{"startDate": months_age_12, "endDate": "today"}],
+                'dateRanges': [{"startDate": months_age_13, "endDate": "today"}],
                 # 'dateRanges': [{"startDate": "5daysAgo", "endDate": "today"}],
                 'dimensions': [{'name': 'ga:date'}],
                 'metrics': [{'expression': 'ga:users'}],
   
              }]
             }
             ).execute()
```

### Comparing `zfl_data-0.0.2/data/migrations/0001_initial.py` & `zfl_data-0.0.3/data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/migrations/0002_webdata.py` & `zfl_data-0.0.3/data/migrations/0002_webdata.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/migrations/0005_auto_20200727_1146.py` & `zfl_data-0.0.3/data/migrations/0005_auto_20200727_1146.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/migrations/0007_googleaccess.py` & `zfl_data-0.0.3/data/migrations/0007_googleaccess.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/migrations/0008_auto_20210327_0952.py` & `zfl_data-0.0.3/data/migrations/0008_auto_20210327_0952.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/data/templates/data/index.html` & `zfl_data-0.0.3/data/templates/data/index.html`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/LICENSE.txt` & `zfl_data-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/README.md` & `zfl_data-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/pyproject.toml` & `zfl_data-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.2/PKG-INFO` & `zfl_data-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfl-data
-Version: 0.0.2
+Version: 0.0.3
 Summary: 'data on zfl'
 Project-URL: Documentation, https://github.com/unknown/Appのパッケージ名#readme
 Project-URL: Issues, https://github.com/unknown/Appのパッケージ名/issues
 Project-URL: Source, https://github.com/unknown/Appのパッケージ名
 Author-email: You are name <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

