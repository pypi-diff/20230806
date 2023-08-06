# Comparing `tmp/naruno_scan-0.1.0.tar.gz` & `tmp/naruno_scan-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_scan-0.1.0.tar", last modified: Thu Jul 27 13:42:06 2023, max compression
+gzip compressed data, was "naruno_scan-0.1.1.tar", last modified: Sun Aug  6 12:25:08 2023, max compression
```

## Comparing `naruno_scan-0.1.0.tar` & `naruno_scan-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.824976 naruno_scan-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/src/naruno_scan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 13:42:06.000000 naruno_scan-0.1.0/src/naruno_scan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/src/scan/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/src/scan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/src/scan/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/src/scan/assets/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:42:06.828976 naruno_scan-0.1.0/src/scan/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/src/scan/assets/icons/loading-animation.png
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/src/scan/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-27 13:41:56.000000 naruno_scan-0.1.0/src/scan/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.015454 naruno_scan-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/src/naruno_scan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 12:25:07.000000 naruno_scan-0.1.1/src/naruno_scan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/src/scan/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/src/scan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/src/scan/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/src/scan/assets/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:25:08.019454 naruno_scan-0.1.1/src/scan/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/src/scan/assets/icons/loading-animation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/src/scan/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-06 12:24:58.000000 naruno_scan-0.1.1/src/scan/scan.py
```

### Comparing `naruno_scan-0.1.0/LICENSE` & `naruno_scan-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naruno_scan-0.1.0/PKG-INFO` & `naruno_scan-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno_scan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Scan website for Naruno
 Home-page: https://github.com/Naruno/scan
 Author: Onur Atakan ULUSOY
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: # Naruno Scan
         This is a simple website that build withj `flet` and `KOT` modules. It's show the situation of Naruno's network.
```

### Comparing `naruno_scan-0.1.0/setup.py` & `naruno_scan-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='naruno_scan',
-version='0.1.0',
+version='0.1.1',
 description="""Scan website for Naruno""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/Naruno/scan',
 author='Onur Atakan ULUSOY',
 author_email='onur.atakan.ulusoy@naruno.org',
 license='MPL-2.0',
```

### Comparing `naruno_scan-0.1.0/src/naruno_scan.egg-info/PKG-INFO` & `naruno_scan-0.1.1/src/naruno_scan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno-scan
-Version: 0.1.0
+Version: 0.1.1
 Summary: Scan website for Naruno
 Home-page: https://github.com/Naruno/scan
 Author: Onur Atakan ULUSOY
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: # Naruno Scan
         This is a simple website that build withj `flet` and `KOT` modules. It's show the situation of Naruno's network.
```

### Comparing `naruno_scan-0.1.0/src/scan/assets/favicon.png` & `naruno_scan-0.1.1/src/scan/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `naruno_scan-0.1.0/src/scan/assets/icons/loading-animation.png` & `naruno_scan-0.1.1/src/scan/assets/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `naruno_scan-0.1.0/src/scan/gui.py` & `naruno_scan-0.1.1/src/scan/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from threading import Thread
 import time
+import traceback
 import flet as ft
 
 from .scan import SCAN, the_statatus_db, the_block_db
 import os
 
 
 network = None
@@ -28,14 +29,15 @@
     global interval_1
     global interval_2
     global thread_generated
     global block_record
     global status_record
     page.scroll = "AUTO"
     page.theme = ft.Theme(font_family="Poppins")
+    page.title = "Scan"
 
     page.appbar = ft.AppBar(
         bgcolor="#212529",
         leading=ft.Image(
                 src=f"https://docs.naruno.org/assets/images/logo.png",
                 width=40,
                 height=40,
@@ -224,16 +226,18 @@
                                             ft.DataCell(ft.Text(i["signature"]), on_tap=lambda e, i=i: show_bs(i)),
                                             ft.DataCell(ft.Text(i["transaction_fee"])),
 
                                         ],
                                     ) for i in validating_list]
             
 
-
-            page.update()        
+            try:
+                page.update()        
+            except:
+                traceback.print_exc()
 
     def block_situation_tracker():
         global block_record
         block_record = None
         try:
             raw_record = the_block_db.get_all()
 
@@ -289,19 +293,23 @@
                                             ft.DataCell(ft.Text(i[1])),
 
                                         ],
                                     ) for i in nodes]
 
 
 
-            page.update()
+            try:
+                page.update()        
+            except:
+                traceback.print_exc()
     def status_situation_tracker():
         global status_record
         status_record = the_statatus_db.get("status")
-        page.pubsub.send_all_on_topic("status", "status")
+        if status_record != None:
+            page.pubsub.send_all_on_topic("status", "status")
 
 
 
     
     def threaderstatus_situation_tracker():
         while True:
             status_situation_tracker()
```

### Comparing `naruno_scan-0.1.0/src/scan/scan.py` & `naruno_scan-0.1.1/src/scan/scan.py`

 * *Files identical despite different names*

