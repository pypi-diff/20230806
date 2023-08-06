# Comparing `tmp/update-linux-3.0.0.tar.gz` & `tmp/update-linux-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-3.0.0.tar", last modified: Sun Aug  6 10:11:26 2023, max compression
+gzip compressed data, was "update-linux-3.0.1.tar", last modified: Sun Aug  6 10:26:06 2023, max compression
```

## Comparing `update-linux-3.0.0.tar` & `update-linux-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/
--rw-r--r--   0 barry     (1000) barry     (1000)    11357 2023-07-31 10:07:15.000000 update-linux-3.0.0/LICENSE
--rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:11:26.339997 update-linux-3.0.0/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     5894 2023-08-06 10:10:09.000000 update-linux-3.0.0/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)      992 2023-07-31 11:05:10.000000 update-linux-3.0.0/pyproject.toml
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-08-06 10:11:26.339997 update-linux-3.0.0/setup.cfg
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    26926 2023-08-06 10:04:41.000000 update-linux-3.0.0/src/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-3.0.0/src/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:11:26.339997 update-linux-3.0.0/src/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      332 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-08-06 10:11:26.000000 update-linux-3.0.0/src/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:26:06.727298 update-linux-3.0.1/
+-rw-r--r--   0 barry     (1000) barry     (1000)    11357 2023-07-31 10:07:15.000000 update-linux-3.0.1/LICENSE
+-rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:26:06.727298 update-linux-3.0.1/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     5894 2023-08-06 10:10:09.000000 update-linux-3.0.1/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)      992 2023-07-31 11:05:10.000000 update-linux-3.0.1/pyproject.toml
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-08-06 10:26:06.727298 update-linux-3.0.1/setup.cfg
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:26:06.726298 update-linux-3.0.1/src/
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:26:06.727298 update-linux-3.0.1/src/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    27081 2023-08-06 10:22:46.000000 update-linux-3.0.1/src/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-3.0.1/src/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-08-06 10:26:06.727298 update-linux-3.0.1/src/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     6534 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      332 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       33 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-08-06 10:26:06.000000 update-linux-3.0.1/src/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-3.0.0/LICENSE` & `update-linux-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `update-linux-3.0.0/PKG-INFO` & `update-linux-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 3.0.0
+Version: 3.0.1
 Summary: Command to automate the routine updating of packages and system upgrading for Unix systems.
 Author-email: Barry Scott <barry@barrys-emacs.org>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/barry-scott/CLI-tools
 Project-URL: Bug Tracker, https://github.com/barry-scott/CLI-tools/issues
 Keywords: development
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `update-linux-3.0.0/README.md` & `update-linux-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `update-linux-3.0.0/pyproject.toml` & `update-linux-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `update-linux-3.0.0/src/update_linux/__init__.py` & `update-linux-3.0.1/src/update_linux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath  # type: ignore
 
-VERSION = '3.0.0'
+VERSION = '3.0.1'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -374,29 +374,37 @@
             rc = ssh_wait( host, wait=False, log_fn=None )
             if rc != 0:
                 self.warn( host, 'Is not reachable' )
                 return None, None, None
 
         os_release = {}
 
-        try:
-            with open( '/etc/os-release' ) as f:
-                for line in f:
-                    line = line.strip()
-                    if line == '' or '=' not in line:
-                        continue
-
-                    key, value = line.split( '=', 1 )
-                    if value.startswith('"') and value.endswith('"'):
-                        value = value[1:-1]
-                    os_release[key] = value
-
-        except IOError as e:
-            self.error( host, str(e) )
-            return None, None, None
+        if host is None:
+            try:
+                with open( '/etc/os-release' ) as f:
+                    stdout = f.readlines()
+
+            except IOError as e:
+                self.error( host, str(e) )
+                return None, None, None
+
+        else:
+            cmd = ['cat', '/etc/os-release']
+            rc, stdout = self.runAndLog( host, cmd, log=False )
+
+        for line in stdout:
+            line = line.strip()
+            if line == '' or '=' not in line:
+                continue
+
+            key, value = line.split( '=', 1 )
+            if value.startswith('"') and value.endswith('"'):
+                value = value[1:-1]
+            os_release[key] = value
+
 
         os_main_id = os_release.get('ID', None)
         os_id_set = set([os_main_id])
         os_version_id = os_release.get('VERSION_ID', 'Unknown')
         if 'ID_LIKE' in os_release:
             for ID in os_release['ID_LIKE'].split():
                 os_id_set.add( ID )
```

### Comparing `update-linux-3.0.0/src/update_linux.egg-info/PKG-INFO` & `update-linux-3.0.1/src/update_linux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 3.0.0
+Version: 3.0.1
 Summary: Command to automate the routine updating of packages and system upgrading for Unix systems.
 Author-email: Barry Scott <barry@barrys-emacs.org>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/barry-scott/CLI-tools
 Project-URL: Bug Tracker, https://github.com/barry-scott/CLI-tools/issues
 Keywords: development
 Classifier: Intended Audience :: End Users/Desktop
```

