# Comparing `tmp/web3_app-0.1.0.tar.gz` & `tmp/web3_app-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3_app-0.1.0.tar", last modified: Sun Aug  6 00:18:54 2023, max compression
+gzip compressed data, was "web3_app-0.1.1.tar", last modified: Sun Aug  6 10:08:52 2023, max compression
```

## Comparing `web3_app-0.1.0.tar` & `web3_app-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.839982 web3_app-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-08-06 00:18:39.000000 web3_app-0.1.0/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 00:18:39.000000 web3_app-0.1.0/LICENSE-src-web3_app-chat__.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 00:18:39.000000 web3_app-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-06 00:18:54.839982 web3_app-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-06 00:18:39.000000 web3_app-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:18:54.839982 web3_app-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-06 00:18:39.000000 web3_app-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/web3_app/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/web3_app/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/web3_app/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/assets/icons/loading-animation.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/web3_app/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/chat/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-06 00:18:39.000000 web3_app-0.1.0/src/web3_app/web3_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:18:54.835982 web3_app-0.1.0/src/web3_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 00:18:54.000000 web3_app-0.1.0/src/web3_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.029008 web3_app-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-08-06 10:08:37.000000 web3_app-0.1.1/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 10:08:37.000000 web3_app-0.1.1/LICENSE-src-web3_app-chat__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 10:08:37.000000 web3_app-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-06 10:08:52.029008 web3_app-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-06 10:08:37.000000 web3_app-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:08:52.029008 web3_app-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-06 10:08:37.000000 web3_app-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.021008 web3_app-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.025008 web3_app-0.1.1/src/web3_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.025008 web3_app-0.1.1/src/web3_app/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.029008 web3_app-0.1.1/src/web3_app/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/assets/icons/loading-animation.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.029008 web3_app-0.1.1/src/web3_app/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/chat/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-08-06 10:08:37.000000 web3_app-0.1.1/src/web3_app/web3_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:08:52.025008 web3_app-0.1.1/src/web3_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 10:08:51.000000 web3_app-0.1.1/src/web3_app.egg-info/top_level.txt
```

### Comparing `web3_app-0.1.0/LICENSE-others__.md` & `web3_app-0.1.1/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/LICENSE-src-web3_app-chat__.md` & `web3_app-0.1.1/LICENSE-src-web3_app-chat__.md`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/PKG-INFO` & `web3_app-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3_app
-Version: 0.1.0
+Version: 0.1.1
 Summary: The source of Web3.
 Home-page: https://github.com/Naruno/Web3_App
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Web3 App for Naruno
         Web3 is an platform for an milestone in Naruno.
```

### Comparing `web3_app-0.1.0/setup.py` & `web3_app-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='web3_app',
-version='0.1.0',
+version='0.1.1',
 description="""The source of Web3.""",
 long_description_content_type="text/markdown",
 include_package_data=True,
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 url='https://github.com/Naruno/Web3_App',
 author="Naruno Developers",
 author_email='onur.atakan.ulusoy@naruno.org',
```

### Comparing `web3_app-0.1.0/src/web3_app/assets/favicon.png` & `web3_app-0.1.1/src/web3_app/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/src/web3_app/assets/icons/loading-animation.png` & `web3_app-0.1.1/src/web3_app/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/src/web3_app/chat/chat.py` & `web3_app-0.1.1/src/web3_app/chat/chat.py`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/src/web3_app/gui.py` & `web3_app-0.1.1/src/web3_app/gui.py`

 * *Files identical despite different names*

### Comparing `web3_app-0.1.0/src/web3_app/web3_app.py` & `web3_app-0.1.1/src/web3_app/web3_app.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,14 +95,17 @@
                     
                     if action not in ["username", "post"]:
                         control = False
 
                     if action == "username":
                         if len(data) > 15:
                             control = False
+                        for _user in database.get_all():
+                            if _user["username"] == data:
+                                control = False
                     elif action == "post":
                         if len(data) > 100:
                             control = False
                         if time.time() - self.get_user(user)["last_post"] < self.post_wait_time:
                             control = False
```

### Comparing `web3_app-0.1.0/src/web3_app.egg-info/PKG-INFO` & `web3_app-0.1.1/src/web3_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3-app
-Version: 0.1.0
+Version: 0.1.1
 Summary: The source of Web3.
 Home-page: https://github.com/Naruno/Web3_App
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Web3 App for Naruno
         Web3 is an platform for an milestone in Naruno.
```

