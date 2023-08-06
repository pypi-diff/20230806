# Comparing `tmp/i2cssh-0.1.6.tar.gz` & `tmp/i2cssh-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.1.6.tar", last modified: Fri Aug  4 08:36:31 2023, max compression
+gzip compressed data, was "i2cssh-0.1.7.tar", last modified: Sun Aug  6 14:38:32 2023, max compression
```

## Comparing `i2cssh-0.1.6.tar` & `i2cssh-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.495392 i2cssh-0.1.6/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.6/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.6/MANIFEST.in
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-04 08:36:31.494830 i2cssh-0.1.6/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.6/README.md
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-04 08:36:31.495543 i2cssh-0.1.6/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1074 2023-08-04 08:34:51.000000 i2cssh-0.1.6/setup.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.475824 i2cssh-0.1.6/src/
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.485187 i2cssh-0.1.6/src/i2cssh/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.6/src/i2cssh/__init__.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24432 2023-08-03 23:27:54.000000 i2cssh-0.1.6/src/i2cssh/lib.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.6/src/i2cssh/main.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.493249 i2cssh-0.1.6/src/i2cssh/tests/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.6/src/i2cssh/tests/__init__.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    36373 2023-08-04 00:04:47.000000 i2cssh-0.1.6/src/i2cssh/tests/test_i2cssh.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-04 08:35:38.000000 i2cssh-0.1.6/src/i2cssh/version.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-04 08:36:31.491399 i2cssh-0.1.6/src/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       44 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/entry_points.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-04 08:36:31.000000 i2cssh-0.1.6/src/i2cssh.egg-info/top_level.txt
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-06 14:38:32.807563 i2cssh-0.1.7/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.7/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.7/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-06 14:38:32.806807 i2cssh-0.1.7/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.7/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-06 14:38:32.807785 i2cssh-0.1.7/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1074 2023-08-04 08:34:51.000000 i2cssh-0.1.7/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-06 14:38:32.785238 i2cssh-0.1.7/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-06 14:38:32.797994 i2cssh-0.1.7/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.7/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24467 2023-08-06 14:35:56.000000 i2cssh-0.1.7/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.7/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-06 14:38:32.805219 i2cssh-0.1.7/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.7/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    36373 2023-08-04 00:04:47.000000 i2cssh-0.1.7/src/i2cssh/tests/test_i2cssh.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-06 14:36:54.000000 i2cssh-0.1.7/src/i2cssh/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-06 14:38:32.803666 i2cssh-0.1.7/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       44 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/entry_points.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-06 14:38:32.000000 i2cssh-0.1.7/src/i2cssh.egg-info/top_level.txt
```

### Comparing `i2cssh-0.1.6/LICENSE.txt` & `i2cssh-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.6/PKG-INFO` & `i2cssh-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.6
+Version: 0.1.7
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.1.6/README.md` & `i2cssh-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.6/setup.py` & `i2cssh-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.6/src/i2cssh/lib.py` & `i2cssh-0.1.7/src/i2cssh/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,16 @@
     valid_options = list(cmdline_opts.keys())
 
     # Load config file and get valid options. Since command line options take precedence, we
     # override the config file options with the command line options.
     config = read_config()
     if config:
         global_opts = filter_valid_options(config, valid_options)
+    else:
+        global_opts = {}
 
     # Because we can split tabs based on cluster/hosts/arguments we first
     # create different groups inside the hosts list. If it turns out we
     # don't need to split tabs, we'll just have one group by flattening
     # the list. Hosts are dictionaries with all the options necessary to spawn the SSH session
     groups = []
```

### Comparing `i2cssh-0.1.6/src/i2cssh/tests/test_i2cssh.py` & `i2cssh-0.1.7/src/i2cssh/tests/test_i2cssh.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.6/src/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.7/src/i2cssh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.6
+Version: 0.1.7
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

