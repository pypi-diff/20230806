# Comparing `tmp/dl2050utils-1.0.98.tar.gz` & `tmp/dl2050utils-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl2050utils-1.0.98.tar", last modified: Mon Dec 13 11:09:05 2021, max compression
+gzip compressed data, was "dl2050utils-1.0.99.tar", last modified: Mon Dec 13 11:09:53 2021, max compression
```

## Comparing `dl2050utils-1.0.98.tar` & `dl2050utils-1.0.99.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jn         (501) staff       (20)        0 2021-12-13 11:09:05.718183 dl2050utils-1.0.98/
--rw-r--r--   0 jn         (501) staff       (20)      561 2021-12-13 11:09:05.718241 dl2050utils-1.0.98/PKG-INFO
--rw-r--r--   0 jn         (501) staff       (20)        8 2020-08-17 13:19:00.000000 dl2050utils-1.0.98/README
-drwxr-xr-x   0 jn         (501) staff       (20)        0 2021-12-13 11:09:05.718150 dl2050utils-1.0.98/dl2050utils/
--rw-r--r--   0 jn         (501) staff       (20)      745 2021-12-13 11:00:50.990183 dl2050utils-1.0.98/dl2050utils/__config__.py
--rw-r--r--   0 jn         (501) staff       (20)        0 2020-08-17 14:03:21.000000 dl2050utils-1.0.98/dl2050utils/__init__.py
--rw-r--r--   0 jn         (501) staff       (20)       18 2021-12-13 11:09:05.697859 dl2050utils-1.0.98/dl2050utils/__version__.py
--rw-r--r--   0 jn         (501) staff       (20)     6778 2021-09-15 16:55:47.000000 dl2050utils-1.0.98/dl2050utils/com.py
--rw-r--r--   0 jn         (501) staff       (20)     2413 2021-01-30 09:56:00.000000 dl2050utils-1.0.98/dl2050utils/core.py
--rw-r--r--   0 jn         (501) staff       (20)     4521 2021-01-18 09:56:16.000000 dl2050utils-1.0.98/dl2050utils/dbdefs.py
--rw-r--r--   0 jn         (501) staff       (20)     9482 2021-12-02 15:20:22.797260 dl2050utils-1.0.98/dl2050utils/dbpg.py
--rw-r--r--   0 jn         (501) staff       (20)     9346 2021-04-07 09:08:09.000000 dl2050utils-1.0.98/dl2050utils/df.py
--rw-r--r--   0 jn         (501) staff       (20)     2514 2021-12-13 10:31:07.968874 dl2050utils-1.0.98/dl2050utils/env.py
--rw-r--r--   0 jn         (501) staff       (20)     3845 2021-02-02 12:54:28.000000 dl2050utils-1.0.98/dl2050utils/etl.py
--rw-r--r--   0 jn         (501) staff       (20)     2368 2021-12-13 11:09:02.664180 dl2050utils-1.0.98/dl2050utils/fs.py
--rw-r--r--   0 jn         (501) staff       (20)     2184 2020-08-17 12:01:23.000000 dl2050utils-1.0.98/dl2050utils/ju.py
--rw-r--r--   0 jn         (501) staff       (20)     2897 2020-11-05 11:34:55.000000 dl2050utils-1.0.98/dl2050utils/log.py
--rw-r--r--   0 jn         (501) staff       (20)     6564 2020-11-21 15:58:50.000000 dl2050utils-1.0.98/dl2050utils/mq.py
--rw-r--r--   0 jn         (501) staff       (20)       39 2020-08-17 13:18:51.000000 dl2050utils-1.0.98/setup.cfg
--rw-r--r--   0 jn         (501) staff       (20)     1512 2021-12-13 11:08:08.103278 dl2050utils-1.0.98/setup.py
+drwxr-xr-x   0 jn         (501) staff       (20)        0 2021-12-13 11:09:53.877668 dl2050utils-1.0.99/
+-rw-r--r--   0 jn         (501) staff       (20)      561 2021-12-13 11:09:53.877718 dl2050utils-1.0.99/PKG-INFO
+-rw-r--r--   0 jn         (501) staff       (20)        8 2020-08-17 13:19:00.000000 dl2050utils-1.0.99/README
+drwxr-xr-x   0 jn         (501) staff       (20)        0 2021-12-13 11:09:53.877641 dl2050utils-1.0.99/dl2050utils/
+-rw-r--r--   0 jn         (501) staff       (20)      745 2021-12-13 11:00:50.990183 dl2050utils-1.0.99/dl2050utils/__config__.py
+-rw-r--r--   0 jn         (501) staff       (20)        0 2020-08-17 14:03:21.000000 dl2050utils-1.0.99/dl2050utils/__init__.py
+-rw-r--r--   0 jn         (501) staff       (20)       18 2021-12-13 11:09:53.857064 dl2050utils-1.0.99/dl2050utils/__version__.py
+-rw-r--r--   0 jn         (501) staff       (20)     6778 2021-09-15 16:55:47.000000 dl2050utils-1.0.99/dl2050utils/com.py
+-rw-r--r--   0 jn         (501) staff       (20)     2413 2021-01-30 09:56:00.000000 dl2050utils-1.0.99/dl2050utils/core.py
+-rw-r--r--   0 jn         (501) staff       (20)     4521 2021-01-18 09:56:16.000000 dl2050utils-1.0.99/dl2050utils/dbdefs.py
+-rw-r--r--   0 jn         (501) staff       (20)     9482 2021-12-02 15:20:22.797260 dl2050utils-1.0.99/dl2050utils/dbpg.py
+-rw-r--r--   0 jn         (501) staff       (20)     9346 2021-04-07 09:08:09.000000 dl2050utils-1.0.99/dl2050utils/df.py
+-rw-r--r--   0 jn         (501) staff       (20)     2514 2021-12-13 10:31:07.968874 dl2050utils-1.0.99/dl2050utils/env.py
+-rw-r--r--   0 jn         (501) staff       (20)     3845 2021-02-02 12:54:28.000000 dl2050utils-1.0.99/dl2050utils/etl.py
+-rw-r--r--   0 jn         (501) staff       (20)     2368 2021-12-13 11:09:02.664180 dl2050utils-1.0.99/dl2050utils/fs.py
+-rw-r--r--   0 jn         (501) staff       (20)     2184 2020-08-17 12:01:23.000000 dl2050utils-1.0.99/dl2050utils/ju.py
+-rw-r--r--   0 jn         (501) staff       (20)     2897 2020-11-05 11:34:55.000000 dl2050utils-1.0.99/dl2050utils/log.py
+-rw-r--r--   0 jn         (501) staff       (20)     6564 2020-11-21 15:58:50.000000 dl2050utils-1.0.99/dl2050utils/mq.py
+-rw-r--r--   0 jn         (501) staff       (20)       39 2020-08-17 13:18:51.000000 dl2050utils-1.0.99/setup.cfg
+-rw-r--r--   0 jn         (501) staff       (20)     1515 2021-12-13 11:09:41.766348 dl2050utils-1.0.99/setup.py
```

### Comparing `dl2050utils-1.0.98/dl2050utils/__config__.py` & `dl2050utils-1.0.99/dl2050utils/__config__.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/com.py` & `dl2050utils-1.0.99/dl2050utils/com.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/core.py` & `dl2050utils-1.0.99/dl2050utils/core.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/dbdefs.py` & `dl2050utils-1.0.99/dl2050utils/dbdefs.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/dbpg.py` & `dl2050utils-1.0.99/dl2050utils/dbpg.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/df.py` & `dl2050utils-1.0.99/dl2050utils/df.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/env.py` & `dl2050utils-1.0.99/dl2050utils/env.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/etl.py` & `dl2050utils-1.0.99/dl2050utils/etl.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/fs.py` & `dl2050utils-1.0.99/dl2050utils/fs.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/ju.py` & `dl2050utils-1.0.99/dl2050utils/ju.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/log.py` & `dl2050utils-1.0.99/dl2050utils/log.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/dl2050utils/mq.py` & `dl2050utils-1.0.99/dl2050utils/mq.py`

 * *Files identical despite different names*

### Comparing `dl2050utils-1.0.98/setup.py` & `dl2050utils-1.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,11 +40,11 @@
 )
 
 cmd = f'gh release create -t "{version_camel}" --notes "Update" dist/{name}-{version}.tar.gz'
 print(cmd)
 res, sout = sh_run(cmd)
 print(sout)
 
-cmd = f'twine upload dist/* --repository {name}'
+cmd = f'twine upload dist/* --repository {package}'
 print(cmd)
 res, sout = sh_run(cmd)
 print(sout)
```

