# Comparing `tmp/logfunc-1.5.1.tar.gz` & `tmp/logfunc-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-1.5.1.tar", last modified: Fri Aug  4 19:23:18 2023, max compression
+gzip compressed data, was "logfunc-1.5.2.tar", last modified: Sun Aug  6 03:43:22 2023, max compression
```

## Comparing `logfunc-1.5.1.tar` & `logfunc-1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 19:23:18.682097 logfunc-1.5.1/
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     1068 2023-06-24 05:08:03.000000 logfunc-1.5.1/LICENSE
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-04 19:23:18.682097 logfunc-1.5.1/PKG-INFO
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     3417 2023-08-04 00:55:39.000000 logfunc-1.5.1/README.md
-drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 19:23:18.682097 logfunc-1.5.1/logfunc/
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     6073 2023-08-04 19:22:07.000000 logfunc-1.5.1/logfunc/__init__.py
-drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-04 19:23:18.682097 logfunc-1.5.1/logfunc.egg-info/
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-04 19:23:18.000000 logfunc-1.5.1/logfunc.egg-info/PKG-INFO
--rw-rw-r--   0 udesk     (1000) udesk     (1000)      170 2023-08-04 19:23:18.000000 logfunc-1.5.1/logfunc.egg-info/SOURCES.txt
--rw-rw-r--   0 udesk     (1000) udesk     (1000)        1 2023-08-04 19:23:18.000000 logfunc-1.5.1/logfunc.egg-info/dependency_links.txt
--rw-rw-r--   0 udesk     (1000) udesk     (1000)        8 2023-08-04 19:23:18.000000 logfunc-1.5.1/logfunc.egg-info/top_level.txt
--rw-rw-r--   0 udesk     (1000) udesk     (1000)       38 2023-08-04 19:23:18.682097 logfunc-1.5.1/setup.cfg
--rw-rw-r--   0 udesk     (1000) udesk     (1000)     1121 2023-08-04 19:22:15.000000 logfunc-1.5.1/setup.py
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-06 03:43:22.252254 logfunc-1.5.2/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     1068 2023-06-24 05:08:03.000000 logfunc-1.5.2/LICENSE
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-06 03:43:22.252254 logfunc-1.5.2/PKG-INFO
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     3417 2023-08-04 00:55:39.000000 logfunc-1.5.2/README.md
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-06 03:43:22.252254 logfunc-1.5.2/logfunc/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     6034 2023-08-06 03:42:23.000000 logfunc-1.5.2/logfunc/__init__.py
+drwxrwxr-x   0 udesk     (1000) udesk     (1000)        0 2023-08-06 03:43:22.252254 logfunc-1.5.2/logfunc.egg-info/
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     4281 2023-08-06 03:43:22.000000 logfunc-1.5.2/logfunc.egg-info/PKG-INFO
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)      170 2023-08-06 03:43:22.000000 logfunc-1.5.2/logfunc.egg-info/SOURCES.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)        1 2023-08-06 03:43:22.000000 logfunc-1.5.2/logfunc.egg-info/dependency_links.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)        8 2023-08-06 03:43:22.000000 logfunc-1.5.2/logfunc.egg-info/top_level.txt
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)       38 2023-08-06 03:43:22.252254 logfunc-1.5.2/setup.cfg
+-rw-rw-r--   0 udesk     (1000) udesk     (1000)     1121 2023-08-06 03:42:25.000000 logfunc-1.5.2/setup.py
```

### Comparing `logfunc-1.5.1/LICENSE` & `logfunc-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-1.5.1/PKG-INFO` & `logfunc-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.5.1
+Version: 1.5.2
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `logfunc-1.5.1/README.md` & `logfunc-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `logfunc-1.5.1/logfunc/__init__.py` & `logfunc-1.5.2/logfunc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                 curval = None
     elif evar in ['LOGF_SINGLE_MSG', 'LOGF_USE_PRINT']:
         val = str(val).upper()
         if val == 'TRUE':
             curval = True
         elif val == 'FALSE':
             curval = False
-    print('@@evar', evar, val, curval)
     return curval
 
 
 def trunc_str(string: str, max_length: Optional[int] = TRUNC_STR_LEN) -> str:
     """
     Truncates a string if its length exceeds the specified maximum length.
     If the string is truncated, it appends '...' to indicate the truncation. If
```

### Comparing `logfunc-1.5.1/logfunc.egg-info/PKG-INFO` & `logfunc-1.5.2/logfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 1.5.1
+Version: 1.5.2
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/tree/main
 Author: Cary Carter
 Author-email: ccarterdev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `logfunc-1.5.1/setup.py` & `logfunc-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='logfunc',
-    version='1.5.1',
+    version='1.5.2',
     packages=find_packages(),
     install_requires=[],
     author='Cary Carter',
     author_email='ccarterdev@gmail.com',
     description='An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

