# Comparing `tmp/eniris-0.7.5.tar.gz` & `tmp/eniris-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eniris-0.7.5.tar", last modified: Sun Aug  6 18:15:16 2023, max compression
+gzip compressed data, was "eniris-0.7.6.tar", last modified: Sun Aug  6 20:49:20 2023, max compression
```

## Comparing `eniris-0.7.5.tar` & `eniris-0.7.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.655688 eniris-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 18:15:04.000000 eniris-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 18:15:16.655688 eniris-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 18:15:04.000000 eniris-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.647688 eniris-0.7.5/eniris/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.651688 eniris-0.7.5/eniris/point/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.651688 eniris-0.7.5/eniris/point/writer/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/writer/buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/writer/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/writer/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/point/writer/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.655688 eniris-0.7.5/eniris/telemessage/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/telemessage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.655688 eniris-0.7.5/eniris/telemessage/writer/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/writer/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/writer/pooled.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-06 18:15:04.000000 eniris-0.7.5/eniris/telemessage/writer/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 18:15:16.651688 eniris-0.7.5/eniris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 18:15:16.000000 eniris-0.7.5/eniris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 18:15:16.000000 eniris-0.7.5/eniris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 18:15:16.000000 eniris-0.7.5/eniris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 18:15:16.000000 eniris-0.7.5/eniris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 18:15:16.000000 eniris-0.7.5/eniris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 18:15:16.655688 eniris-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-06 18:15:04.000000 eniris-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-06 20:49:11.000000 eniris-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:49:20.852753 eniris-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-06 20:49:11.000000 eniris-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.848753 eniris-0.7.6/eniris/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/point/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/point/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/point/writer/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/telemessage/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/telemessage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.852753 eniris-0.7.6/eniris/telemessage/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/pooled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-06 20:49:11.000000 eniris-0.7.6/eniris/telemessage/writer/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:49:20.848753 eniris-0.7.6/eniris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 20:49:20.000000 eniris-0.7.6/eniris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 20:49:20.852753 eniris-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-06 20:49:11.000000 eniris-0.7.6/setup.py
```

### Comparing `eniris-0.7.5/LICENSE` & `eniris-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/PKG-INFO` & `eniris-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.5
+Version: 0.7.6
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.5.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.5/README.md` & `eniris-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/driver.py` & `eniris-0.7.6/eniris/driver.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/namespace.py` & `eniris-0.7.6/eniris/point/namespace.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/point.py` & `eniris-0.7.6/eniris/point/point.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/writer/buffered.py` & `eniris-0.7.6/eniris/point/writer/buffered.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/writer/direct.py` & `eniris-0.7.6/eniris/point/writer/direct.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/writer/filter.py` & `eniris-0.7.6/eniris/point/writer/filter.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/point/writer/writer.py` & `eniris-0.7.6/eniris/point/writer/writer.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/telemessage/telemessage.py` & `eniris-0.7.6/eniris/telemessage/telemessage.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/telemessage/writer/direct.py` & `eniris-0.7.6/eniris/telemessage/writer/direct.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris/telemessage/writer/pooled.py` & `eniris-0.7.6/eniris/telemessage/writer/pooled.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     while True:
       tmw = self.queue.onWaitingToActive()
       if tmw is None:
         logging.debug("Stopped PooledTelemessageWriterDaemon")
         return
       try:
         headers: dict[str, str] = {"Authorization": self.authorizationHeaderFunction()} if self.authorizationHeaderFunction is not None else {}
-        resp = self.session.post(self.url, headers=headers, params=self.params|tmw.telemessage.parameters, timeout=self.timeoutS)
+        resp = self.session.post(self.url, params=self.params|tmw.telemessage.parameters, data=b'/n'.join(tmw.telemessage.lines), headers=headers, timeout=self.timeoutS)
         if resp.status_code == 204:
           tmw.finish(self.queue)
         elif resp.status_code in self.retryStatusCodes:
           tmw.reschedule(f"response with status code {resp.status_code} ({HTTPStatus(resp.status_code).phrase}): {resp.text}", self.queue)
         else:
           logging.error(f"Dropping telemessage due to response with status code {resp.status_code} ({HTTPStatus(resp.status_code).phrase}): {resp.text}")
       except requests.Timeout:
```

### Comparing `eniris-0.7.5/eniris/telemessage/writer/writer.py` & `eniris-0.7.6/eniris/telemessage/writer/writer.py`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/eniris.egg-info/PKG-INFO` & `eniris-0.7.6/eniris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: eniris
-Version: 0.7.5
+Version: 0.7.6
 Summary: Eniris API driver for Python
 Home-page: https://github.com/eniris-international/eniris-api-python-driver
-Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.5.tar.gz
+Download-URL: https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz
 Author: Enris BV
 Author-email: info@eniris.be
 License: MIT
 Keywords: eniris,api,rest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `eniris-0.7.5/eniris.egg-info/SOURCES.txt` & `eniris-0.7.6/eniris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eniris-0.7.5/setup.py` & `eniris-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
   packages = [
     'eniris',
     'eniris.point',
     'eniris.point.writer',
     'eniris.telemessage',
     'eniris.telemessage.writer'
   ],
-  version = '0.7.5',
+  version = '0.7.6',
   description = 'Eniris API driver for Python',
   license='MIT',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Enris BV',
   author_email = 'info@eniris.be',
   url = 'https://github.com/eniris-international/eniris-api-python-driver',
-  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.5.tar.gz',
+  download_url = 'https://github.com/eniris-international/eniris-api-python-driver/archive/refs/tags/v0.7.6.tar.gz',
   keywords = ['eniris', 'api', 'rest'],   # Keywords that define your package best
   install_requires=[
     'requests'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
```

