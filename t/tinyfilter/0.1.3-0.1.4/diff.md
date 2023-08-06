# Comparing `tmp/tinyfilter-0.1.3.tar.gz` & `tmp/tinyfilter-0.1.4.tar.gz`

## Comparing `tinyfilter-0.1.3.tar` & `tinyfilter-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/.DS_Store
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/THANKS.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/.DS_Store
--rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/apple.png
--rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/art.png
--rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/balloon.png
--rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/chanel.png
--rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/einstein.png
--rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/flowers.png
--rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/github.png
--rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/king.png
--rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/lisa.png
--rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/mcdonalds.png
--rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/paint.png
--rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/pink.jpeg
--rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/target.png
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/test.png
--rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/tiny.png
--rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/images/youtube.png
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/Activate.ps1
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/activate
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/activate.csh
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/activate.fish
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/f2py
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/f2py3
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/f2py3.10
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/helloworld
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/python3.10 -> python3
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/new/bin/tinyimggen
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/.DS_Store
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/README.md
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/__main__.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/backup.py
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/example_image.png
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/main.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/main_debug.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/nike.png
--rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/nike2.png
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/output_image.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/old/test.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/src/tinyfilter/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/src/tinyfilter/example.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/LICENSE
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 tinyfilter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/.DS_Store
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/THANKS.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/.DS_Store
+-rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/apple.png
+-rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/art.png
+-rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/balloon.png
+-rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/chanel.png
+-rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/einstein.png
+-rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/flowers.png
+-rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/github.png
+-rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/king.png
+-rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/lisa.png
+-rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/mcdonalds.png
+-rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/paint.png
+-rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/pink.jpeg
+-rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/target.png
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/test.png
+-rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/tiny.png
+-rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/images/youtube.png
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/Activate.ps1
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/activate
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/activate.csh
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/activate.fish
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/f2py
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/f2py3
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/f2py3.10
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/helloworld
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/pip3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/python3.10 -> python3
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/new/bin/tinyimggen
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/.DS_Store
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/README.md
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/__main__.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/backup.py
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/example_image.png
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/main.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/main_debug.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/nike.png
+-rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/nike2.png
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/output_image.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/old/test.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/src/tinyfilter/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/src/tinyfilter/example.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 tinyfilter-0.1.4/PKG-INFO
```

### Comparing `tinyfilter-0.1.3/.DS_Store` & `tinyfilter-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/THANKS.txt` & `tinyfilter-0.1.4/THANKS.txt`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/.DS_Store` & `tinyfilter-0.1.4/images/.DS_Store`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/apple.png` & `tinyfilter-0.1.4/images/apple.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/art.png` & `tinyfilter-0.1.4/images/art.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/balloon.png` & `tinyfilter-0.1.4/images/balloon.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/chanel.png` & `tinyfilter-0.1.4/images/chanel.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/einstein.png` & `tinyfilter-0.1.4/images/einstein.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/flowers.png` & `tinyfilter-0.1.4/images/flowers.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/github.png` & `tinyfilter-0.1.4/images/github.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/king.png` & `tinyfilter-0.1.4/images/king.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/lisa.png` & `tinyfilter-0.1.4/images/lisa.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/mcdonalds.png` & `tinyfilter-0.1.4/images/mcdonalds.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/paint.png` & `tinyfilter-0.1.4/images/paint.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/pink.jpeg` & `tinyfilter-0.1.4/images/pink.jpeg`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/target.png` & `tinyfilter-0.1.4/images/target.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/test.png` & `tinyfilter-0.1.4/images/test.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/tiny.png` & `tinyfilter-0.1.4/images/tiny.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/images/youtube.png` & `tinyfilter-0.1.4/images/youtube.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/new/bin/Activate.ps1` & `tinyfilter-0.1.4/new/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/new/bin/activate` & `tinyfilter-0.1.4/new/bin/activate`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/new/bin/activate.csh` & `tinyfilter-0.1.4/new/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/new/bin/activate.fish` & `tinyfilter-0.1.4/new/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/.DS_Store` & `tinyfilter-0.1.4/old/.DS_Store`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/__main__.py` & `tinyfilter-0.1.4/old/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/backup.py` & `tinyfilter-0.1.4/old/backup.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/example_image.png` & `tinyfilter-0.1.4/old/example_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/main.py` & `tinyfilter-0.1.4/old/main.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/main_debug.py` & `tinyfilter-0.1.4/old/main_debug.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/nike.png` & `tinyfilter-0.1.4/old/nike.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/nike2.png` & `tinyfilter-0.1.4/old/nike2.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/old/output_image.png` & `tinyfilter-0.1.4/old/output_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/src/tinyfilter/__init__.py` & `tinyfilter-0.1.4/src/tinyfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/.gitignore` & `tinyfilter-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/LICENSE` & `tinyfilter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/README.md` & `tinyfilter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.3/PKG-INFO` & `tinyfilter-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: tinyfilter
-Version: 0.1.3
+Version: 0.1.4
 Summary: tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/zroe1/tinyfilter/tree/main
 Author-email: Zephaniah Roe <zroe@uchicago.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: numpy~=1.25.0
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.3 Summary: tinyfilter is
+Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.4 Summary: tinyfilter is
 the computer vision equivalent to micrograd. It convert images into ASCII art
 using the principles of CNNs (convolutional neural networks). Project-URL:
-Homepage, https://github.com/pypa/sampleproject Project-URL: Bug Tracker,
-https://github.com/pypa/sampleproject/issues Author-email: Zephaniah Roe
+Homepage, https://github.com/zroe1/tinyfilter/tree/main Author-email: Zephaniah
+Roe
 uchicago.edu> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy~=1.25.0
 Requires-Dist: pillow Description-Content-Type: text/markdown # tinyfilter
 [Screenshot 2023-08-05 at 4 52 21 PM]  tinyfilter [^1] is the computer vision
 equivalent to Andrej Karpathy's micrograd. It convert images into ASCII art
 using the principles of CNNs (convolutional neural networks).  Unlike other
```

