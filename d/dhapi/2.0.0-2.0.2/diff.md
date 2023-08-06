# Comparing `tmp/dhapi-2.0.0.tar.gz` & `tmp/dhapi-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-2.0.0.tar", last modified: Sat Jul  8 07:18:28 2023, max compression
+gzip compressed data, was "dhapi-2.0.2.tar", last modified: Sun Aug  6 14:50:22 2023, max compression
```

## Comparing `dhapi-2.0.0.tar` & `dhapi-2.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889818 dhapi-2.0.0/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-05-14 08:41:15.000000 dhapi-2.0.0/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-07-08 07:18:28.889706 dhapi-2.0.0/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)     2328 2023-07-08 06:48:18.000000 dhapi-2.0.0/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-05-14 08:41:15.000000 dhapi-2.0.0/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-07-08 07:18:28.889854 dhapi-2.0.0/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-14 08:41:15.000000 dhapi-2.0.0/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.884989 dhapi-2.0.0/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.887284 dhapi-2.0.0/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888159 dhapi-2.0.0/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4980 2023-07-08 07:11:45.000000 dhapi-2.0.0/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888409 dhapi-2.0.0/src/dhapi/configuration/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/configuration/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      862 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/configuration/logger.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888616 dhapi-2.0.0/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3960 2023-07-08 07:12:17.000000 dhapi-2.0.0/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.888821 dhapi-2.0.0/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2231 2023-05-21 06:21:51.000000 dhapi-2.0.0/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889320 dhapi-2.0.0/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4467 2023-07-08 07:13:59.000000 dhapi-2.0.0/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/router.py
--rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/router/version_checker.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.889548 dhapi-2.0.0/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-05-14 08:41:15.000000 dhapi-2.0.0/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-07-08 07:18:28.887938 dhapi-2.0.0/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      775 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)      101 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/requires.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-07-08 07:18:28.000000 dhapi-2.0.0/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.105931 dhapi-2.0.2/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-08-06 13:22:10.000000 dhapi-2.0.2/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-08-06 14:50:22.105805 dhapi-2.0.2/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)     2328 2023-08-06 13:22:10.000000 dhapi-2.0.2/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-08-06 13:22:10.000000 dhapi-2.0.2/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-08-06 14:50:22.105965 dhapi-2.0.2/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-08-06 14:39:27.000000 dhapi-2.0.2/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.102087 dhapi-2.0.2/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.103295 dhapi-2.0.2/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.104261 dhapi-2.0.2/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4980 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.104498 dhapi-2.0.2/src/dhapi/configuration/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/configuration/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      862 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/configuration/logger.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.104789 dhapi-2.0.2/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3960 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.105008 dhapi-2.0.2/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2231 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.105448 dhapi-2.0.2/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4467 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/router/router.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     1067 2023-08-06 14:49:03.000000 dhapi-2.0.2/src/dhapi/router/version_checker.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.105641 dhapi-2.0.2/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-08-06 13:22:10.000000 dhapi-2.0.2/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-08-06 14:50:22.104038 dhapi-2.0.2/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     2983 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      775 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       83 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/requires.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-08-06 14:50:22.000000 dhapi-2.0.2/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-2.0.0/LICENSE.txt` & `dhapi-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/PKG-INFO` & `dhapi-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 2.0.0
+Version: 2.0.2
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
```

### Comparing `dhapi-2.0.0/README.md` & `dhapi-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/setup.py` & `dhapi-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/client/lottery_client.py` & `dhapi-2.0.2/src/dhapi/client/lottery_client.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/configuration/logger.py` & `dhapi-2.0.2/src/dhapi/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-2.0.2/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/purchase/lotto645_controller.py` & `dhapi-2.0.2/src/dhapi/purchase/lotto645_controller.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/router/arg_parser.py` & `dhapi-2.0.2/src/dhapi/router/arg_parser.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/router/router.py` & `dhapi-2.0.2/src/dhapi/router/router.py`

 * *Files identical despite different names*

### Comparing `dhapi-2.0.0/src/dhapi/router/version_checker.py` & `dhapi-2.0.2/src/dhapi/router/version_checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from subprocess import call
 from packaging import version
 
-from johnnydep.lib import JohnnyDist
-from johnnydep import logs
-
-logs.configure_logging(verbosity=0)
+# from johnnydep.lib import JohnnyDist
+# from johnnydep import logs
+#
+# logs.configure_logging(verbosity=0)
 
 PACKAGE_NAME = "dhapi"
 
 
 def _upgrade():
     call("pip install --upgrade " + PACKAGE_NAME, shell=True)
 
 
 def get_versions():
     """
     :return (installed_version, latest_version)
     """
-    dist = JohnnyDist(PACKAGE_NAME)
-    return dist.version_installed, dist.version_latest
+    # dist = JohnnyDist(PACKAGE_NAME)
+    # return dist.version_installed, dist.version_latest
+    return ("0.0.0", "0.0.0")  # TODO(seonghyeok): Implement this function. JoynnyDist is not working.
 
 
 def suggest_upgrade():
     installed_version, latest_version = get_versions()
     if version.parse(installed_version) != version.parse(latest_version):
         print(
             f"""현재 설치된 버전은 최신 버전이 아닙니다. (현재 버전: {installed_version} / 최신 버전: {latest_version})
```

### Comparing `dhapi-2.0.0/src/dhapi.egg-info/PKG-INFO` & `dhapi-2.0.2/src/dhapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhapi
-Version: 2.0.0
+Version: 2.0.2
 Summary: 동행복권 비공식 API
 Home-page: https://github.com/roeniss/dhlottery-api
 Author: Roeniss Moon
 Author-email: roeniss2@gmail.com
 Project-URL: Bug Reports, https://github.com/roeniss/dhlottery-api/issues
 Project-URL: Source, https://github.com/roeniss/dhlottery-api/
 Keywords: donghaeng,lottery,lotto645,api,korean
```

### Comparing `dhapi-2.0.0/src/dhapi.egg-info/SOURCES.txt` & `dhapi-2.0.2/src/dhapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

