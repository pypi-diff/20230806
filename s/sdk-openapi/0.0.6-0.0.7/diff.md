# Comparing `tmp/sdk-openapi-0.0.6.tar.gz` & `tmp/sdk-openapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk-openapi-0.0.6.tar", last modified: Wed Aug  2 15:08:52 2023, max compression
+gzip compressed data, was "sdk-openapi-0.0.7.tar", last modified: Sat Aug  5 09:22:00 2023, max compression
```

## Comparing `sdk-openapi-0.0.6.tar` & `sdk-openapi-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 15:08:52.653540 sdk-openapi-0.0.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-02 15:08:52.653540 sdk-openapi-0.0.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      657 2023-08-02 14:42:12.000000 sdk-openapi-0.0.6/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 15:08:52.645540 sdk-openapi-0.0.6/openapi/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      180 2023-07-24 07:04:11.000000 sdk-openapi-0.0.6/openapi/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2023-08-02 14:40:26.000000 sdk-openapi-0.0.6/openapi/constants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2107 2023-08-02 15:07:26.000000 sdk-openapi-0.0.6/openapi/core.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 15:08:52.653540 sdk-openapi-0.0.6/sdk_openapi.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-02 15:08:52.000000 sdk-openapi-0.0.6/sdk_openapi.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-08-02 15:08:52.000000 sdk-openapi-0.0.6/sdk_openapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 15:08:52.000000 sdk-openapi-0.0.6/sdk_openapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 15:08:52.000000 sdk-openapi-0.0.6/sdk_openapi.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-08-02 15:08:52.000000 sdk-openapi-0.0.6/sdk_openapi.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-02 15:08:52.653540 sdk-openapi-0.0.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      997 2023-08-02 15:08:48.000000 sdk-openapi-0.0.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-05 09:22:00.437984 sdk-openapi-0.0.7/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-05 09:22:00.437984 sdk-openapi-0.0.7/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      657 2023-08-02 14:42:12.000000 sdk-openapi-0.0.7/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-05 09:22:00.437984 sdk-openapi-0.0.7/openapi/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      232 2023-08-05 08:30:37.000000 sdk-openapi-0.0.7/openapi/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2023-08-05 08:05:43.000000 sdk-openapi-0.0.7/openapi/constants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2121 2023-08-05 08:28:03.000000 sdk-openapi-0.0.7/openapi/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2494 2023-08-05 08:33:07.000000 sdk-openapi-0.0.7/openapi/core_async.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-05 09:22:00.437984 sdk-openapi-0.0.7/sdk_openapi.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1208 2023-08-05 09:22:00.000000 sdk-openapi-0.0.7/sdk_openapi.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      271 2023-08-05 09:22:00.000000 sdk-openapi-0.0.7/sdk_openapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-05 09:22:00.000000 sdk-openapi-0.0.7/sdk_openapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-05 09:22:00.000000 sdk-openapi-0.0.7/sdk_openapi.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-08-05 09:22:00.000000 sdk-openapi-0.0.7/sdk_openapi.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-08-05 09:22:00.437984 sdk-openapi-0.0.7/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      997 2023-08-05 09:21:44.000000 sdk-openapi-0.0.7/setup.py
```

### Comparing `sdk-openapi-0.0.6/PKG-INFO` & `sdk-openapi-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk-openapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: The python package for api.qewertyy.me
 Home-page: https://github.com/Qewertyy/Open-API
 Author: Qewertyy
 Author-email: Qewertyy.irl@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot,Image Generations,Latent Diffusion,State of Art
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sdk-openapi-0.0.6/README.md` & `sdk-openapi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sdk-openapi-0.0.6/sdk_openapi.egg-info/PKG-INFO` & `sdk-openapi-0.0.7/sdk_openapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk-openapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: The python package for api.qewertyy.me
 Home-page: https://github.com/Qewertyy/Open-API
 Author: Qewertyy
 Author-email: Qewertyy.irl@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot,Image Generations,Latent Diffusion,State of Art
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sdk-openapi-0.0.6/setup.py` & `sdk-openapi-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 setup(
     name="sdk-openapi",
-    version="0.0.6",
+    version="0.0.7",
     author="Qewertyy",
     author_email="Qewertyy.irl@gmail.com",
     description="The python package for api.qewertyy.me",
     url="https://github.com/Qewertyy/Open-API",
     python_requires=">=3.8",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
```

