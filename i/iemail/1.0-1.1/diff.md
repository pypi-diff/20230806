# Comparing `tmp/iemail-1.0.tar.gz` & `tmp/iemail-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iemail-1.0.tar", last modified: Wed Aug  2 06:00:30 2023, max compression
+gzip compressed data, was "iemail-1.1.tar", last modified: Sun Aug  6 15:14:19 2023, max compression
```

## Comparing `iemail-1.0.tar` & `iemail-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 06:00:30.360004 iemail-1.0/
--rw-rw-rw-   0        0        0     1064 2023-08-02 05:30:09.000000 iemail-1.0/LICENSE
--rw-rw-rw-   0        0        0     2035 2023-08-02 06:00:30.360004 iemail-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1119 2023-08-02 05:50:20.000000 iemail-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 06:00:30.344082 iemail-1.0/iemail/
--rw-rw-rw-   0        0        0       28 2022-10-22 03:07:58.000000 iemail-1.0/iemail/__init__.py
--rw-rw-rw-   0        0        0      156 2023-08-02 05:29:37.000000 iemail-1.0/iemail/exceptions.py
--rw-rw-rw-   0        0        0     1373 2023-08-02 05:32:11.000000 iemail-1.0/iemail/models.py
--rw-rw-rw-   0        0        0      171 2022-10-22 03:07:58.000000 iemail-1.0/iemail/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:00:30.359007 iemail-1.0/iemail.egg-info/
--rw-rw-rw-   0        0        0     2035 2023-08-02 06:00:30.000000 iemail-1.0/iemail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-08-02 06:00:30.000000 iemail-1.0/iemail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:00:30.000000 iemail-1.0/iemail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 06:00:30.000000 iemail-1.0/iemail.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 06:00:30.000000 iemail-1.0/iemail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 06:00:30.361999 iemail-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-08-02 06:00:02.000000 iemail-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:14:19.904660 iemail-1.1/
+-rw-rw-rw-   0        0        0     1064 2023-08-02 05:30:09.000000 iemail-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2032 2023-08-06 15:14:19.906664 iemail-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1119 2023-08-02 05:50:20.000000 iemail-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 15:14:19.827342 iemail-1.1/iemail/
+-rw-rw-rw-   0        0        0       28 2022-10-22 03:07:58.000000 iemail-1.1/iemail/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-08-02 05:29:37.000000 iemail-1.1/iemail/exceptions.py
+-rw-rw-rw-   0        0        0     1373 2023-08-02 05:32:11.000000 iemail-1.1/iemail/models.py
+-rw-rw-rw-   0        0        0      171 2022-10-22 03:07:58.000000 iemail-1.1/iemail/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:14:19.899669 iemail-1.1/iemail.egg-info/
+-rw-rw-rw-   0        0        0     2032 2023-08-06 15:14:19.000000 iemail-1.1/iemail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-08-06 15:14:19.000000 iemail-1.1/iemail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:14:19.000000 iemail-1.1/iemail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 15:14:19.000000 iemail-1.1/iemail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-06 15:14:19.000000 iemail-1.1/iemail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-06 15:14:19.914631 iemail-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2023-08-06 15:13:29.000000 iemail-1.1/setup.py
```

### Comparing `iemail-1.0/LICENSE` & `iemail-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iemail-1.0/PKG-INFO` & `iemail-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iemail
-Version: 1.0
+Version: 1.1
 Summary: Temporary Email Python SDK of https://api.iemail.eu.org/
-Home-page: https://github.com/Danny-Yxzl/mail_gw
+Home-page: https://pypi.org/project/iemail/
 Author: IEmail
 Author-email: i@iemail.eu.org
 Project-URL: HomePage, https://iemail.eu.org/
-Project-URL: API Docs, https://docs.iemail.eu.org/
+Project-URL: API Gateway, https://api.iemail.eu.org/
 Keywords: Tempmail mail iemail email API
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `iemail-1.0/README.md` & `iemail-1.1/README.md`

 * *Files identical despite different names*

### Comparing `iemail-1.0/iemail/models.py` & `iemail-1.1/iemail/models.py`

 * *Files identical despite different names*

### Comparing `iemail-1.0/iemail.egg-info/PKG-INFO` & `iemail-1.1/iemail.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iemail
-Version: 1.0
+Version: 1.1
 Summary: Temporary Email Python SDK of https://api.iemail.eu.org/
-Home-page: https://github.com/Danny-Yxzl/mail_gw
+Home-page: https://pypi.org/project/iemail/
 Author: IEmail
 Author-email: i@iemail.eu.org
 Project-URL: HomePage, https://iemail.eu.org/
-Project-URL: API Docs, https://docs.iemail.eu.org/
+Project-URL: API Gateway, https://api.iemail.eu.org/
 Keywords: Tempmail mail iemail email API
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `iemail-1.0/setup.py` & `iemail-1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='iemail',
-    version='1.0',
+    version='1.1',
     description='Temporary Email Python SDK of https://api.iemail.eu.org/',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/Danny-Yxzl/mail_gw",
+    url="https://pypi.org/project/iemail/",
     author="IEmail",
     author_email="i@iemail.eu.org",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
@@ -24,10 +24,10 @@
         "Programming Language :: Python :: 3.11"
     ],
     keywords="Tempmail mail iemail email API",
     install_requires=["requests"],
     packages=["iemail"],
     project_urls={
         "HomePage": "https://iemail.eu.org/",
-        "API Docs": "https://docs.iemail.eu.org/",
+        "API Gateway": "https://api.iemail.eu.org/",
     },
 )
```

