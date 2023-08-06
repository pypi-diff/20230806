# Comparing `tmp/Autotest_api-1.0.2.tar.gz` & `tmp/Autotest_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Autotest_api-1.0.2.tar", last modified: Wed Jul 26 06:25:27 2023, max compression
+gzip compressed data, was "Autotest_api-1.0.3.tar", last modified: Sun Aug  6 10:45:56 2023, max compression
```

## Comparing `Autotest_api-1.0.2.tar` & `Autotest_api-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-07-26 06:25:27.368305 Autotest_api-1.0.2/
--rw-r--r--   0 joson      (501) staff       (20)      988 2023-07-26 06:25:27.368124 Autotest_api-1.0.2/PKG-INFO
--rw-rw-r--   0 joson      (501) staff       (20)      540 2023-05-08 16:20:09.000000 Autotest_api-1.0.2/README.rst
--rw-r--r--   0 joson      (501) staff       (20)       38 2023-07-26 06:25:27.368353 Autotest_api-1.0.2/setup.cfg
--rw-rw-r--   0 joson      (501) staff       (20)     1219 2023-07-26 06:24:53.000000 Autotest_api-1.0.2/setup.py
-drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-07-26 06:25:27.362165 Autotest_api-1.0.2/src/
-drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-07-26 06:25:27.366719 Autotest_api-1.0.2/src/Autotest_api/
--rw-r--r--   0 joson      (501) staff       (20)       20 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/__init__.py
--rw-r--r--   0 joson      (501) staff       (20)     2874 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/create_funtion.py
--rw-r--r--   0 joson      (501) staff       (20)     2719 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/db.py
--rw-r--r--   0 joson      (501) staff       (20)      238 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/exceptions.py
--rw-r--r--   0 joson      (501) staff       (20)     6083 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/extract.py
--rw-r--r--   0 joson      (501) staff       (20)     2059 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/http_session.py
--rw-r--r--   0 joson      (501) staff       (20)     2456 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/log.py
--rw-r--r--   0 joson      (501) staff       (20)     8148 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/mitm_http.py
--rw-r--r--   0 joson      (501) staff       (20)     3055 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/my_builtins.py
--rw-r--r--   0 joson      (501) staff       (20)        0 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/parser.py
--rw-r--r--   0 joson      (501) staff       (20)    15526 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/plugin.py
--rw-r--r--   0 joson      (501) staff       (20)     4719 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/render_template_obj.py
--rw-r--r--   0 joson      (501) staff       (20)     4467 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/report_notify.py
--rw-r--r--   0 joson      (501) staff       (20)     1447 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/request_session.py
--rw-r--r--   0 joson      (501) staff       (20)    36176 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/runner.py
--rw-r--r--   0 joson      (501) staff       (20)     3526 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/start_project.py
--rw-r--r--   0 joson      (501) staff       (20)     7722 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/swagger_parser.py
--rw-r--r--   0 joson      (501) staff       (20)     3803 2023-07-26 05:54:58.000000 Autotest_api-1.0.2/src/Autotest_api/validate.py
-drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-07-26 06:25:27.367891 Autotest_api-1.0.2/src/Autotest_api.egg-info/
--rw-r--r--   0 joson      (501) staff       (20)      988 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/PKG-INFO
--rw-r--r--   0 joson      (501) staff       (20)      815 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/SOURCES.txt
--rw-r--r--   0 joson      (501) staff       (20)        1 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/dependency_links.txt
--rw-r--r--   0 joson      (501) staff       (20)       46 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/entry_points.txt
--rw-r--r--   0 joson      (501) staff       (20)      188 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/requires.txt
--rw-r--r--   0 joson      (501) staff       (20)       13 2023-07-26 06:25:27.000000 Autotest_api-1.0.2/src/Autotest_api.egg-info/top_level.txt
+drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-08-06 10:45:56.986270 Autotest_api-1.0.3/
+-rw-r--r--   0 joson      (501) staff       (20)      988 2023-08-06 10:45:56.986117 Autotest_api-1.0.3/PKG-INFO
+-rw-rw-r--   0 joson      (501) staff       (20)      540 2023-05-08 16:20:09.000000 Autotest_api-1.0.3/README.rst
+-rw-r--r--   0 joson      (501) staff       (20)       38 2023-08-06 10:45:56.986445 Autotest_api-1.0.3/setup.cfg
+-rw-rw-r--   0 joson      (501) staff       (20)     1311 2023-08-06 10:43:54.000000 Autotest_api-1.0.3/setup.py
+drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-08-06 10:45:56.979450 Autotest_api-1.0.3/src/
+drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-08-06 10:45:56.984943 Autotest_api-1.0.3/src/Autotest_api/
+-rw-r--r--   0 joson      (501) staff       (20)       20 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/__init__.py
+-rw-r--r--   0 joson      (501) staff       (20)     2874 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/create_funtion.py
+-rw-r--r--   0 joson      (501) staff       (20)     2719 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/db.py
+-rw-r--r--   0 joson      (501) staff       (20)      238 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/exceptions.py
+-rw-r--r--   0 joson      (501) staff       (20)     6083 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/extract.py
+-rw-r--r--   0 joson      (501) staff       (20)     2059 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/http_session.py
+-rw-r--r--   0 joson      (501) staff       (20)     2456 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/log.py
+-rw-r--r--   0 joson      (501) staff       (20)     8148 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/mitm_http.py
+-rw-r--r--   0 joson      (501) staff       (20)     3055 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/my_builtins.py
+-rw-r--r--   0 joson      (501) staff       (20)        0 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/parser.py
+-rw-r--r--   0 joson      (501) staff       (20)    15526 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/plugin.py
+-rw-r--r--   0 joson      (501) staff       (20)     4719 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/render_template_obj.py
+-rw-r--r--   0 joson      (501) staff       (20)     4467 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/report_notify.py
+-rw-r--r--   0 joson      (501) staff       (20)     1447 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/request_session.py
+-rw-r--r--   0 joson      (501) staff       (20)    36176 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/runner.py
+-rw-r--r--   0 joson      (501) staff       (20)     3526 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/start_project.py
+-rw-r--r--   0 joson      (501) staff       (20)     7722 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/swagger_parser.py
+-rw-r--r--   0 joson      (501) staff       (20)     3803 2023-07-26 05:54:58.000000 Autotest_api-1.0.3/src/Autotest_api/validate.py
+drwxr-xr-x   0 joson      (501) staff       (20)        0 2023-08-06 10:45:56.985890 Autotest_api-1.0.3/src/Autotest_api.egg-info/
+-rw-r--r--   0 joson      (501) staff       (20)      988 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/PKG-INFO
+-rw-r--r--   0 joson      (501) staff       (20)      815 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 joson      (501) staff       (20)        1 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 joson      (501) staff       (20)       46 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/entry_points.txt
+-rw-r--r--   0 joson      (501) staff       (20)      244 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/requires.txt
+-rw-r--r--   0 joson      (501) staff       (20)       13 2023-08-06 10:45:56.000000 Autotest_api-1.0.3/src/Autotest_api.egg-info/top_level.txt
```

### Comparing `Autotest_api-1.0.2/PKG-INFO` & `Autotest_api-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Autotest_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: http/https API run by yaml
 Home-page: https://github.com/leo/Autotest_api
 Author: QA-leo
 Author-email: 994991952@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,Autotest_api
 Classifier: Framework :: Pytest
```

### Comparing `Autotest_api-1.0.2/README.rst` & `Autotest_api-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/setup.py` & `Autotest_api-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 The setup script.
 """
 
 setup(
     name='Autotest_api',
     url='https://github.com/leo/Autotest_api',
-    version='v1.0.2',
+    version='v1.0.3',
     author="QA-leo",
     author_email='994991952@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["Autotest_api"],
     classifiers=[
@@ -33,14 +33,17 @@
         'PyYAML>=6.0',
         'requests==2.18.4',
         'allure-pytest>=2.12.0',
         'pymysql>=1.0.2',
         'DingtalkChatbot>=1.5.7',
         'Faker>=15.3.4',
         'requests_toolbelt>=0.10.1',
+        'redis>=4.6.0',
+        'websocket-client>=1.6.1',
+        'websockets>=11.0.3',
     ],
     entry_points={
         'pytest11': [
             'Autotest_api = Autotest_api.plugin',
         ]
     }
 )
```

### Comparing `Autotest_api-1.0.2/src/Autotest_api/create_funtion.py` & `Autotest_api-1.0.3/src/Autotest_api/create_funtion.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/db.py` & `Autotest_api-1.0.3/src/Autotest_api/db.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/extract.py` & `Autotest_api-1.0.3/src/Autotest_api/extract.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/http_session.py` & `Autotest_api-1.0.3/src/Autotest_api/http_session.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/log.py` & `Autotest_api-1.0.3/src/Autotest_api/log.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/mitm_http.py` & `Autotest_api-1.0.3/src/Autotest_api/mitm_http.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/my_builtins.py` & `Autotest_api-1.0.3/src/Autotest_api/my_builtins.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/plugin.py` & `Autotest_api-1.0.3/src/Autotest_api/plugin.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/render_template_obj.py` & `Autotest_api-1.0.3/src/Autotest_api/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/report_notify.py` & `Autotest_api-1.0.3/src/Autotest_api/report_notify.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/request_session.py` & `Autotest_api-1.0.3/src/Autotest_api/request_session.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/runner.py` & `Autotest_api-1.0.3/src/Autotest_api/runner.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/start_project.py` & `Autotest_api-1.0.3/src/Autotest_api/start_project.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/swagger_parser.py` & `Autotest_api-1.0.3/src/Autotest_api/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api/validate.py` & `Autotest_api-1.0.3/src/Autotest_api/validate.py`

 * *Files identical despite different names*

### Comparing `Autotest_api-1.0.2/src/Autotest_api.egg-info/PKG-INFO` & `Autotest_api-1.0.3/src/Autotest_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Autotest-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: http/https API run by yaml
 Home-page: https://github.com/leo/Autotest_api
 Author: QA-leo
 Author-email: 994991952@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,Autotest_api
 Classifier: Framework :: Pytest
```

### Comparing `Autotest_api-1.0.2/src/Autotest_api.egg-info/SOURCES.txt` & `Autotest_api-1.0.3/src/Autotest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

