# Comparing `tmp/medisearch_client-0.1.4.tar.gz` & `tmp/medisearch_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medisearch_client-0.1.4.tar", last modified: Sun Aug  6 03:08:14 2023, max compression
+gzip compressed data, was "medisearch_client-0.1.5.tar", last modified: Sun Aug  6 03:19:51 2023, max compression
```

## Comparing `medisearch_client-0.1.4.tar` & `medisearch_client-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.367505 medisearch_client-0.1.4/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:08:14.367358 medisearch_client-0.1.4/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)     3233 2023-08-06 03:06:58.000000 medisearch_client-0.1.4/README.md
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.366499 medisearch_client-0.1.4/medisearch_client/
--rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.4/medisearch_client/__init__.py
--rw-r--r--   0 mpmisko    (501) staff       (20)     4779 2023-08-06 02:57:12.000000 medisearch_client-0.1.4/medisearch_client/client.py
-drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:08:14.367176 medisearch_client-0.1.4/medisearch_client.egg-info/
--rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/PKG-INFO
--rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/SOURCES.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/dependency_links.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/requires.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 03:08:14.000000 medisearch_client-0.1.4/medisearch_client.egg-info/top_level.txt
--rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 03:08:14.367543 medisearch_client-0.1.4/setup.cfg
--rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 03:07:54.000000 medisearch_client-0.1.4/setup.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.240139 medisearch_client-0.1.5/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:19:51.240017 medisearch_client-0.1.5/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3233 2023-08-06 03:06:58.000000 medisearch_client-0.1.5/README.md
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.239189 medisearch_client-0.1.5/medisearch_client/
+-rw-r--r--   0 mpmisko    (501) staff       (20)       36 2023-08-05 22:49:03.000000 medisearch_client-0.1.5/medisearch_client/__init__.py
+-rw-r--r--   0 mpmisko    (501) staff       (20)     4780 2023-08-06 03:18:15.000000 medisearch_client-0.1.5/medisearch_client/client.py
+drwxr-xr-x   0 mpmisko    (501) staff       (20)        0 2023-08-06 03:19:51.239858 medisearch_client-0.1.5/medisearch_client.egg-info/
+-rw-r--r--   0 mpmisko    (501) staff       (20)     3507 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/PKG-INFO
+-rw-r--r--   0 mpmisko    (501) staff       (20)      280 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)        1 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       17 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/requires.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       18 2023-08-06 03:19:51.000000 medisearch_client-0.1.5/medisearch_client.egg-info/top_level.txt
+-rw-r--r--   0 mpmisko    (501) staff       (20)       38 2023-08-06 03:19:51.240174 medisearch_client-0.1.5/setup.cfg
+-rw-r--r--   0 mpmisko    (501) staff       (20)      556 2023-08-06 03:18:29.000000 medisearch_client-0.1.5/setup.py
```

### Comparing `medisearch_client-0.1.4/PKG-INFO` & `medisearch_client-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch_client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
```

### Comparing `medisearch_client-0.1.4/README.md` & `medisearch_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `medisearch_client-0.1.4/medisearch_client/client.py` & `medisearch_client-0.1.5/medisearch_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,8 +128,8 @@
       if self.interrupted:
         break
       data = json.loads(self.socket.recv())
       yield data
       if "event" in data and (data["event"] == "articles" or
                               data["event"] == "error"):
         break
-    self.interrupted = True
+    self.interrupted = False
```

### Comparing `medisearch_client-0.1.4/medisearch_client.egg-info/PKG-INFO` & `medisearch_client-0.1.5/medisearch_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medisearch-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple client for the MediSearch API
 Home-page: https://github.com/MediSearch/medisearch_client_python
 Author: Michal Pandy
 Author-email: founders@medisearch.io
 Description-Content-Type: text/markdown
```

### Comparing `medisearch_client-0.1.4/setup.py` & `medisearch_client-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup file for the medisearch_client package."""
 
 from setuptools import setup, find_packages
 
 setup(
     name="medisearch_client",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "websocket-client",
     ],
     author="Michal Pandy",
     author_email="founders@medisearch.io",
     description="A simple client for the MediSearch API",
```

