# Comparing `tmp/ondewo-client-utils-1.0.0.tar.gz` & `tmp/ondewo-client-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-client-utils-1.0.0.tar", last modified: Fri Mar 31 12:38:37 2023, max compression
+gzip compressed data, was "ondewo-client-utils-1.0.1.tar", last modified: Sun Aug  6 17:16:11 2023, max compression
```

## Comparing `ondewo-client-utils-1.0.0.tar` & `ondewo-client-utils-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:38:37.774577 ondewo-client-utils-1.0.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-03-31 12:36:02.000000 ondewo-client-utils-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1529 2023-03-31 12:38:37.774577 ondewo-client-utils-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      699 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:38:37.773577 ondewo-client-utils-1.0.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:38:37.774577 ondewo-client-utils-1.0.0/ondewo/utils/
--rw-rw-r--   0 root         (0) root         (0)      580 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.0/ondewo/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2009 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.0/ondewo/utils/base_client.py
--rw-rw-r--   0 root         (0) root         (0)     1564 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.0/ondewo/utils/base_client_config.py
--rw-rw-r--   0 root         (0) root         (0)      736 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.0/ondewo/utils/base_service_container.py
--rw-rw-r--   0 root         (0) root         (0)     2614 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.0/ondewo/utils/base_services_interface.py
--rw-rw-r--   0 root         (0) root         (0)     1730 2023-03-31 12:13:44.000000 ondewo-client-utils-1.0.0/ondewo/utils/helpers.py
--rw-rw-r--   0 root         (0) root         (0)      925 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.0/ondewo/utils/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 12:38:37.774577 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-03-31 12:38:37.000000 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-31 12:38:37.000000 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 12:38:37.000000 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-03-31 12:38:37.000000 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-31 12:38:37.000000 ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-03-31 12:38:37.774577 ondewo-client-utils-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1750 2023-03-31 12:29:34.000000 ondewo-client-utils-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:16:11.341735 ondewo-client-utils-1.0.1/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-03-31 12:36:02.000000 ondewo-client-utils-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-08-06 17:16:11.342735 ondewo-client-utils-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      699 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:16:11.341735 ondewo-client-utils-1.0.1/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.1/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:16:11.341735 ondewo-client-utils-1.0.1/ondewo/utils/
+-rw-rw-r--   0 root         (0) root         (0)      580 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.1/ondewo/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2009 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.1/ondewo/utils/base_client.py
+-rw-rw-r--   0 root         (0) root         (0)     1564 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.1/ondewo/utils/base_client_config.py
+-rw-rw-r--   0 root         (0) root         (0)      736 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.1/ondewo/utils/base_service_container.py
+-rw-rw-r--   0 root         (0) root         (0)     2614 2023-03-31 12:11:34.000000 ondewo-client-utils-1.0.1/ondewo/utils/base_services_interface.py
+-rw-rw-r--   0 root         (0) root         (0)     1730 2023-03-31 12:13:44.000000 ondewo-client-utils-1.0.1/ondewo/utils/helpers.py
+-rw-rw-r--   0 root         (0) root         (0)      925 2023-03-31 11:34:47.000000 ondewo-client-utils-1.0.1/ondewo/utils/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:16:11.341735 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-08-06 17:16:11.000000 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-06 17:16:11.000000 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 17:16:11.000000 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-08-06 17:16:11.000000 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-06 17:16:11.000000 ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-08-06 17:16:11.342735 ondewo-client-utils-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1750 2023-08-06 17:15:19.000000 ondewo-client-utils-1.0.1/setup.py
```

### Comparing `ondewo-client-utils-1.0.0/LICENSE` & `ondewo-client-utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/PKG-INFO` & `ondewo-client-utils-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ondewo-client-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library contains utilities and base classes for gRPC clients.
 Home-page: https://github.com/ondewo/ondewo-client-utils-python
-Author: Ondewo GbmH
+Author: Ondewo GmbH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: ondewo-client-utils Version: 1.0.0 Summary: This
+Metadata-Version: 2.1 Name: ondewo-client-utils Version: 1.0.1 Summary: This
 library contains utilities and base classes for gRPC clients. Home-page: https:
-//github.com/ondewo/ondewo-client-utils-python Author: Ondewo GbmH Author-
+//github.com/ondewo/ondewo-client-utils-python Author: Ondewo GmbH Author-
 email: info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Requires-Python:
```

### Comparing `ondewo-client-utils-1.0.0/README.md` & `ondewo-client-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/__init__.py` & `ondewo-client-utils-1.0.1/ondewo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/base_client.py` & `ondewo-client-utils-1.0.1/ondewo/utils/base_client.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/base_client_config.py` & `ondewo-client-utils-1.0.1/ondewo/utils/base_client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/base_service_container.py` & `ondewo-client-utils-1.0.1/ondewo/utils/base_service_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/base_services_interface.py` & `ondewo-client-utils-1.0.1/ondewo/utils/base_services_interface.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/helpers.py` & `ondewo-client-utils-1.0.1/ondewo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo/utils/text.py` & `ondewo-client-utils-1.0.1/ondewo/utils/text.py`

 * *Files identical despite different names*

### Comparing `ondewo-client-utils-1.0.0/ondewo_client_utils.egg-info/PKG-INFO` & `ondewo-client-utils-1.0.1/ondewo_client_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ondewo-client-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library contains utilities and base classes for gRPC clients.
 Home-page: https://github.com/ondewo/ondewo-client-utils-python
-Author: Ondewo GbmH
+Author: Ondewo GmbH
 Author-email: info@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: ondewo-client-utils Version: 1.0.0 Summary: This
+Metadata-Version: 2.1 Name: ondewo-client-utils Version: 1.0.1 Summary: This
 library contains utilities and base classes for gRPC clients. Home-page: https:
-//github.com/ondewo/ondewo-client-utils-python Author: Ondewo GbmH Author-
+//github.com/ondewo/ondewo-client-utils-python Author: Ondewo GmbH Author-
 email: info@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Operating System :: OS Independent Requires-Python:
```

### Comparing `ondewo-client-utils-1.0.0/setup.py` & `ondewo-client-utils-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 
 long_description: str = read_file('README.md')
 requires: List[str] = read_requirements('requirements.txt')
 
 setuptools.setup(
     name='ondewo-client-utils',
-    version='1.0.0',
-    author='Ondewo GbmH',
+    version='1.0.1',
+    author='Ondewo GmbH',
     author_email='info@ondewo.com',
     description='This library contains utilities and base classes for gRPC clients.',
     long_description=long_description,
     include_package_data=True,
     long_description_content_type='text/markdown',
     url='https://github.com/ondewo/ondewo-client-utils-python',
     packages=setuptools.find_packages(include=['ondewo*', ]),
```

