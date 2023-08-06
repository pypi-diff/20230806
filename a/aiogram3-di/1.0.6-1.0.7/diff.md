# Comparing `tmp/aiogram3_di-1.0.6.tar.gz` & `tmp/aiogram3_di-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.6.tar", last modified: Wed Aug  2 12:30:33 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.7.tar", last modified: Sun Aug  6 12:58:41 2023, max compression
```

## Comparing `aiogram3_di-1.0.6.tar` & `aiogram3_di-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:30:33.252182 aiogram3_di-1.0.6/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.6/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-02 12:30:33.252182 aiogram3_di-1.0.6/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1407 2023-08-02 12:12:17.000000 aiogram3_di-1.0.6/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:30:33.252182 aiogram3_di-1.0.6/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.6/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-02 12:30:28.000000 aiogram3_di-1.0.6/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      276 2023-07-31 08:28:38.000000 aiogram3_di-1.0.6/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1067 2023-08-02 12:10:09.000000 aiogram3_di-1.0.6/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5569 2023-08-02 12:28:07.000000 aiogram3_di-1.0.6/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-02 12:30:33.252182 aiogram3_di-1.0.6/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-02 12:30:33.000000 aiogram3_di-1.0.6/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-08-02 12:30:33.000000 aiogram3_di-1.0.6/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-08-02 12:30:33.000000 aiogram3_di-1.0.6/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-08-02 12:30:33.000000 aiogram3_di-1.0.6/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-08-02 12:30:33.000000 aiogram3_di-1.0.6/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-08-02 12:30:33.252182 aiogram3_di-1.0.6/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.6/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-06 12:58:41.015772 aiogram3_di-1.0.7/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.7/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-06 12:58:41.015772 aiogram3_di-1.0.7/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1407 2023-08-02 12:12:17.000000 aiogram3_di-1.0.7/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-06 12:58:41.015772 aiogram3_di-1.0.7/aiogram3_di/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      168 2023-08-06 12:56:40.000000 aiogram3_di-1.0.7/aiogram3_di/__init__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       22 2023-08-06 12:55:17.000000 aiogram3_di-1.0.7/aiogram3_di/_version.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      240 2023-08-06 12:50:50.000000 aiogram3_di-1.0.7/aiogram3_di/depends.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1067 2023-08-02 12:10:09.000000 aiogram3_di-1.0.7/aiogram3_di/middleware.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     5569 2023-08-02 12:28:07.000000 aiogram3_di-1.0.7/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-06 12:58:41.015772 aiogram3_di-1.0.7/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2037 2023-08-06 12:58:40.000000 aiogram3_di-1.0.7/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-08-06 12:58:40.000000 aiogram3_di-1.0.7/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-08-06 12:58:40.000000 aiogram3_di-1.0.7/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-08-06 12:58:40.000000 aiogram3_di-1.0.7/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-08-06 12:58:40.000000 aiogram3_di-1.0.7/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-08-06 12:58:41.015772 aiogram3_di-1.0.7/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.7/setup.py
```

### Comparing `aiogram3_di-1.0.6/LICENSE` & `aiogram3_di-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.6/PKG-INFO` & `aiogram3_di-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3_di
-Version: 1.0.6
+Version: 1.0.7
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
```

### Comparing `aiogram3_di-1.0.6/README.md` & `aiogram3_di-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.6/aiogram3_di/middleware.py` & `aiogram3_di-1.0.7/aiogram3_di/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.6/aiogram3_di/utils.py` & `aiogram3_di-1.0.7/aiogram3_di/utils.py`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.6/aiogram3_di.egg-info/PKG-INFO` & `aiogram3_di-1.0.7/aiogram3_di.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-di
-Version: 1.0.6
+Version: 1.0.7
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
```

### Comparing `aiogram3_di-1.0.6/setup.py` & `aiogram3_di-1.0.7/setup.py`

 * *Files identical despite different names*

