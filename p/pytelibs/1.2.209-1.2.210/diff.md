# Comparing `tmp/pytelibs-1.2.209.tar.gz` & `tmp/pytelibs-1.2.210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.209.tar", last modified: Mon Jul 31 14:21:35 2023, max compression
+gzip compressed data, was "pytelibs-1.2.210.tar", last modified: Sun Aug  6 05:40:14 2023, max compression
```

## Comparing `pytelibs-1.2.209.tar` & `pytelibs-1.2.210.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.235431 pytelibs-1.2.209/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.209/LICENSE
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-31 14:21:35.235431 pytelibs-1.2.209/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.209/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.175431 pytelibs-1.2.209/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      584 2023-07-31 14:17:46.000000 pytelibs-1.2.209/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-07-31 14:07:15.000000 pytelibs-1.2.209/pytelibs/_globvals.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-31 14:20:57.000000 pytelibs-1.2.209/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-31 14:17:59.000000 pytelibs-1.2.209/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.225431 pytelibs-1.2.209/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 14:21:35.235431 pytelibs-1.2.209/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.209/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 05:40:14.806025 pytelibs-1.2.210/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.210/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-08-06 05:40:14.796025 pytelibs-1.2.210/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.210/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 05:40:14.736025 pytelibs-1.2.210/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-07-31 14:17:46.000000 pytelibs-1.2.210/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-31 14:07:15.000000 pytelibs-1.2.210/pytelibs/_globvals.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-08-06 05:38:40.000000 pytelibs-1.2.210/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-08-06 05:38:57.000000 pytelibs-1.2.210/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 05:40:14.786025 pytelibs-1.2.210/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-08-06 05:40:14.000000 pytelibs-1.2.210/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-08-06 05:40:14.000000 pytelibs-1.2.210/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 05:40:14.000000 pytelibs-1.2.210/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-08-06 05:40:14.000000 pytelibs-1.2.210/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-06 05:40:14.000000 pytelibs-1.2.210/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-06 05:40:14.806025 pytelibs-1.2.210/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.210/setup.py
```

### Comparing `pytelibs-1.2.209/LICENSE` & `pytelibs-1.2.210/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.209/PKG-INFO` & `pytelibs-1.2.210/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.209
+Version: 1.2.210
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.209/pytelibs/__init__.py` & `pytelibs-1.2.210/pytelibs/__init__.py`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.209/pytelibs/_globvals.py` & `pytelibs-1.2.210/pytelibs/_globvals.py`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.209/pytelibs/_journal.py` & `pytelibs-1.2.210/pytelibs/_journal.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     -1001221450384,  # @pyrogramlounge
     -1001109500936,  # @TelethonChat
     -1001235155926,  # @RoseSupportChat
     -1001421589523,  # @tdspya
     -1001360494801,  # @OFIOpenChat
     -1001275084637,  # @OFIChat
     -1001435671639,  # @xfichat
+    -1001817962988,
 )
 
 GUCAST_BLACKLIST = (
     777000,  # Telegram
     4247000,  # @notoscam
     431415000,  # @BotSupport
     454000,  # @dmcatelegram
```

### Comparing `pytelibs-1.2.209/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.210/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.209
+Version: 1.2.210
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.209/setup.py` & `pytelibs-1.2.210/setup.py`

 * *Files identical despite different names*

