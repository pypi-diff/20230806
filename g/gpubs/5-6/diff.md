# Comparing `tmp/gpubs-5.tar.gz` & `tmp/gpubs-6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpubs-5.tar", last modified: Fri Aug  4 01:43:34 2023, max compression
+gzip compressed data, was "gpubs-6.tar", last modified: Sun Aug  6 14:39:34 2023, max compression
```

## Comparing `gpubs-5.tar` & `gpubs-6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-5/MANIFEST.in
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-04 01:43:34.223223 gpubs-5/PKG-INFO
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/gpubs/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-5/gpubs/__init__.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-08-04 01:43:34.000000 gpubs-5/gpubs/_version.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)    19754 2023-06-24 04:34:36.000000 gpubs-5/gpubs/api.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     2111 2023-06-24 02:02:55.000000 gpubs-5/gpubs/fetch.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      209 2023-06-24 01:55:43.000000 gpubs-5/gpubs/log.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     7035 2023-06-24 02:40:36.000000 gpubs-5/gpubs/models.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     5065 2023-08-04 01:20:02.000000 gpubs-5/gpubs/parse.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1301 2023-06-24 01:55:43.000000 gpubs-5/gpubs/reference.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1899 2023-06-24 03:41:23.000000 gpubs-5/gpubs/search_words.py
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/gpubs.egg-info/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/PKG-INFO
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/SOURCES.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/dependency_links.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/requires.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-08-04 01:43:34.000000 gpubs-5/gpubs.egg-info/top_level.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-08-04 01:43:12.000000 gpubs-5/release-info.json
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-04 01:43:34.223223 gpubs-5/scripts/
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-5/scripts/create_search_terms_file.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-5/scripts/download_pubs.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-5/scripts/search.awk
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-08-04 01:43:34.223223 gpubs-5/setup.cfg
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1141 2023-06-24 02:06:26.000000 gpubs-5/setup.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-06 14:39:34.412789 gpubs-6/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-6/MANIFEST.in
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-06 14:39:34.412789 gpubs-6/PKG-INFO
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-06 14:39:34.412789 gpubs-6/gpubs/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-6/gpubs/__init__.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-08-06 14:39:34.000000 gpubs-6/gpubs/_version.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)    19754 2023-06-24 04:34:36.000000 gpubs-6/gpubs/api.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     2111 2023-06-24 02:02:55.000000 gpubs-6/gpubs/fetch.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      209 2023-06-24 01:55:43.000000 gpubs-6/gpubs/log.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     7035 2023-06-24 02:40:36.000000 gpubs-6/gpubs/models.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     6244 2023-08-06 14:32:28.000000 gpubs-6/gpubs/parse.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1301 2023-06-24 01:55:43.000000 gpubs-6/gpubs/reference.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1899 2023-06-24 03:41:23.000000 gpubs-6/gpubs/search_words.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-06 14:39:34.412789 gpubs-6/gpubs.egg-info/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-08-06 14:39:34.000000 gpubs-6/gpubs.egg-info/PKG-INFO
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-08-06 14:39:34.000000 gpubs-6/gpubs.egg-info/SOURCES.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-08-06 14:39:34.000000 gpubs-6/gpubs.egg-info/dependency_links.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       88 2023-08-06 14:39:34.000000 gpubs-6/gpubs.egg-info/requires.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-08-06 14:39:34.000000 gpubs-6/gpubs.egg-info/top_level.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-08-06 13:43:18.000000 gpubs-6/release-info.json
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-08-06 14:39:34.412789 gpubs-6/scripts/
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-6/scripts/create_search_terms_file.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-6/scripts/download_pubs.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-6/scripts/search.awk
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-08-06 14:39:34.412789 gpubs-6/setup.cfg
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1172 2023-08-06 14:30:26.000000 gpubs-6/setup.py
```

### Comparing `gpubs-5/gpubs/api.py` & `gpubs-6/gpubs/api.py`

 * *Files identical despite different names*

### Comparing `gpubs-5/gpubs/fetch.py` & `gpubs-6/gpubs/fetch.py`

 * *Files identical despite different names*

### Comparing `gpubs-5/gpubs/models.py` & `gpubs-6/gpubs/models.py`

 * *Files identical despite different names*

### Comparing `gpubs-5/gpubs/reference.py` & `gpubs-6/gpubs/reference.py`

 * *Files identical despite different names*

### Comparing `gpubs-5/gpubs/search_words.py` & `gpubs-6/gpubs/search_words.py`

 * *Files identical despite different names*

### Comparing `gpubs-5/scripts/create_search_terms_file.sh` & `gpubs-6/scripts/create_search_terms_file.sh`

 * *Files identical despite different names*

### Comparing `gpubs-5/scripts/download_pubs.sh` & `gpubs-6/scripts/download_pubs.sh`

 * *Files identical despite different names*

### Comparing `gpubs-5/scripts/search.awk` & `gpubs-6/scripts/search.awk`

 * *Files identical despite different names*

### Comparing `gpubs-5/setup.py` & `gpubs-6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,18 +18,19 @@
             url=f'http://github.org/{j["REPONAME"]}',
             author=j["AUTHOR"],
             author_email=j["EMAIL"],
             keywords=j["KEYWORDS"],
             include_package_data=True,
             install_requires=[
                 "ipykernel==6.19.2",
-                "pydantic==1.10.8",
-                "requests==2.29.0",
+                "lxml==4.9.2",
                 "nltk==3.7",
                 "pandas==1.5.3",
+                "pydantic==1.10.8",
+                "requests==2.29.0",
             ],
             scripts=[
                 "scripts/create_search_terms_file.sh",
                 "scripts/search.awk",
                 "scripts/download_pubs.sh",
             ],
         )
```

