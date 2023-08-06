# Comparing `tmp/starco_utiles-3.0.tar.gz` & `tmp/starco_utiles-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starco_utiles-3.0.tar", last modified: Sun Aug  6 15:18:10 2023, max compression
+gzip compressed data, was "starco_utiles-4.0.tar", last modified: Sun Aug  6 15:25:26 2023, max compression
```

## Comparing `starco_utiles-3.0.tar` & `starco_utiles-4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:18:10.313219 starco_utiles-3.0/
--rw-r--r--   0 root         (0) root         (0)      161 2023-08-06 15:18:10.313219 starco_utiles-3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:18:10.313219 starco_utiles-3.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      148 2023-08-06 15:17:53.000000 starco_utiles-3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:18:10.313219 starco_utiles-3.0/starco_utiles/
--rw-rw-r--   0 root         (0) root         (0)       97 2023-08-06 15:17:25.000000 starco_utiles-3.0/starco_utiles/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      988 2023-08-06 15:15:43.000000 starco_utiles-3.0/starco_utiles/debug.py
--rw-rw-r--   0 root         (0) root         (0)      254 2023-08-06 15:14:49.000000 starco_utiles-3.0/starco_utiles/directories.py
--rw-rw-r--   0 root         (0) root         (0)      264 2023-08-06 15:10:03.000000 starco_utiles-3.0/starco_utiles/structures.py
--rw-rw-r--   0 root         (0) root         (0)     1668 2023-08-06 15:09:09.000000 starco_utiles-3.0/starco_utiles/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:18:10.313219 starco_utiles-3.0/starco_utiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)      161 2023-08-06 15:18:10.000000 starco_utiles-3.0/starco_utiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2023-08-06 15:18:10.000000 starco_utiles-3.0/starco_utiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:18:10.000000 starco_utiles-3.0/starco_utiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-08-06 15:18:10.000000 starco_utiles-3.0/starco_utiles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:25:26.959772 starco_utiles-4.0/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-08-06 15:25:26.959772 starco_utiles-4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 15:25:26.959772 starco_utiles-4.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      148 2023-08-06 15:22:24.000000 starco_utiles-4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:25:26.959772 starco_utiles-4.0/starco_utiles/
+-rw-rw-r--   0 root         (0) root         (0)       97 2023-08-06 15:17:25.000000 starco_utiles-4.0/starco_utiles/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      987 2023-08-06 15:25:11.000000 starco_utiles-4.0/starco_utiles/debug.py
+-rw-rw-r--   0 root         (0) root         (0)      254 2023-08-06 15:14:49.000000 starco_utiles-4.0/starco_utiles/directories.py
+-rw-rw-r--   0 root         (0) root         (0)      264 2023-08-06 15:10:03.000000 starco_utiles-4.0/starco_utiles/structures.py
+-rw-rw-r--   0 root         (0) root         (0)     1668 2023-08-06 15:09:09.000000 starco_utiles-4.0/starco_utiles/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 15:25:26.959772 starco_utiles-4.0/starco_utiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-08-06 15:25:26.000000 starco_utiles-4.0/starco_utiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2023-08-06 15:25:26.000000 starco_utiles-4.0/starco_utiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 15:25:26.000000 starco_utiles-4.0/starco_utiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-08-06 15:25:26.000000 starco_utiles-4.0/starco_utiles.egg-info/top_level.txt
```

### Comparing `starco_utiles-3.0/starco_utiles/debug.py` & `starco_utiles-4.0/starco_utiles/debug.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,13 +17,13 @@
                 err= traceback.format_exc()
                 errl = err.split('\n')
                 err_msg = '\n\t'.join(errl[1:])
                 pm+='\n'+err_msg
             else:
                 error = str(error)
                 pm+='\t'+error
-            with open(path_maker([],self.realative_path)+'/log','a+') as f:
+            with open(path_maker([],self.relative_path)+'/log','a+') as f:
                 f.write(pm+'\n\n')
                 if self.debug_mode:
                     print(pm)
 
         except:pass
```

### Comparing `starco_utiles-3.0/starco_utiles/time.py` & `starco_utiles-4.0/starco_utiles/time.py`

 * *Files identical despite different names*

