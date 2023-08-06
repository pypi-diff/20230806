# Comparing `tmp/dotscanner-1.4.0.tar.gz` & `tmp/dotscanner-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.4.0.tar", last modified: Sun Aug  6 01:28:14 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.4.1.tar", last modified: Sun Aug  6 01:38:20 2023, max compression
```

## Comparing `dotscanner-1.4.0.tar` & `dotscanner-1.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.558785 dotscanner-1.4.0/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-08-01 23:51:41.000000 dotscanner-1.4.0/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:28:14.558629 dotscanner-1.4.0/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    13607 2023-08-06 00:19:42.000000 dotscanner-1.4.0/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.554039 dotscanner-1.4.0/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      945 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       49 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       19 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.554507 dotscanner-1.4.0/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6219 2023-08-06 01:15:43.000000 dotscanner-1.4.0/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)     5028 2023-08-06 01:15:44.000000 dotscanner-1.4.0/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:28:14.558845 dotscanner-1.4.0/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1423 2023-08-06 01:28:14.000000 dotscanner-1.4.0/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.555535 dotscanner-1.4.0/src/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3241 2023-08-06 01:15:41.000000 dotscanner-1.4.0/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    11266 2023-08-06 00:02:21.000000 dotscanner-1.4.0/src/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)    13292 2023-08-06 01:15:43.000000 dotscanner-1.4.0/src/density.py
--rw-r--r--   0 holly      (501) staff       (20)     7759 2023-08-06 01:15:42.000000 dotscanner-1.4.0/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)    12954 2023-08-06 01:15:42.000000 dotscanner-1.4.0/src/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)    13910 2023-08-06 00:37:35.000000 dotscanner-1.4.0/src/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.556699 dotscanner-1.4.0/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5904 2023-08-06 01:15:47.000000 dotscanner-1.4.0/src/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     2397 2023-08-06 00:07:44.000000 dotscanner-1.4.0/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3964 2023-08-06 01:15:46.000000 dotscanner-1.4.0/src/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     6565 2023-08-06 01:15:46.000000 dotscanner-1.4.0/src/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    18607 2023-08-06 01:15:45.000000 dotscanner-1.4.0/src/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    19247 2023-08-06 01:15:45.000000 dotscanner-1.4.0/src/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3537 2023-08-06 01:15:44.000000 dotscanner-1.4.0/src/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.557622 dotscanner-1.4.0/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/__init__.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.557764 dotscanner-1.4.0/tests/data/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/data/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    12091 2023-08-06 01:15:39.000000 dotscanner-1.4.0/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     6950 2023-08-06 01:15:38.000000 dotscanner-1.4.0/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    14804 2023-08-06 01:15:38.000000 dotscanner-1.4.0/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     8907 2023-08-06 01:21:49.000000 dotscanner-1.4.0/tests/test_fullAnalysis.py
--rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:15:37.000000 dotscanner-1.4.0/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6029 2023-08-06 01:15:36.000000 dotscanner-1.4.0/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.558400 dotscanner-1.4.0/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      523 2023-08-05 23:38:08.000000 dotscanner-1.4.0/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     1111 2023-08-05 23:37:50.000000 dotscanner-1.4.0/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4439 2023-08-06 01:15:40.000000 dotscanner-1.4.0/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     9117 2023-08-06 01:15:39.000000 dotscanner-1.4.0/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.189692 dotscanner-1.4.1/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-08-01 23:51:41.000000 dotscanner-1.4.1/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 01:38:20.189545 dotscanner-1.4.1/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    13631 2023-08-06 01:37:51.000000 dotscanner-1.4.1/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.184547 dotscanner-1.4.1/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      945 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       49 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       19 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.184922 dotscanner-1.4.1/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-08-06 01:15:43.000000 dotscanner-1.4.1/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)     5028 2023-08-06 01:15:44.000000 dotscanner-1.4.1/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:38:20.189747 dotscanner-1.4.1/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1423 2023-08-06 01:38:19.000000 dotscanner-1.4.1/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.186026 dotscanner-1.4.1/src/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3241 2023-08-06 01:15:41.000000 dotscanner-1.4.1/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    11266 2023-08-06 00:02:21.000000 dotscanner-1.4.1/src/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    13319 2023-08-06 01:37:52.000000 dotscanner-1.4.1/src/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     7759 2023-08-06 01:15:42.000000 dotscanner-1.4.1/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    12954 2023-08-06 01:15:42.000000 dotscanner-1.4.1/src/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)    13910 2023-08-06 00:37:35.000000 dotscanner-1.4.1/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.187299 dotscanner-1.4.1/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5904 2023-08-06 01:15:47.000000 dotscanner-1.4.1/src/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     2397 2023-08-06 00:07:44.000000 dotscanner-1.4.1/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3964 2023-08-06 01:15:46.000000 dotscanner-1.4.1/src/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     6565 2023-08-06 01:15:46.000000 dotscanner-1.4.1/src/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    18607 2023-08-06 01:15:45.000000 dotscanner-1.4.1/src/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    19247 2023-08-06 01:15:45.000000 dotscanner-1.4.1/src/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3537 2023-08-06 01:15:44.000000 dotscanner-1.4.1/src/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.188460 dotscanner-1.4.1/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/__init__.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.188607 dotscanner-1.4.1/tests/data/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/data/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    12091 2023-08-06 01:15:39.000000 dotscanner-1.4.1/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     6950 2023-08-06 01:15:38.000000 dotscanner-1.4.1/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    14804 2023-08-06 01:15:38.000000 dotscanner-1.4.1/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     8907 2023-08-06 01:21:49.000000 dotscanner-1.4.1/tests/test_fullAnalysis.py
+-rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:15:37.000000 dotscanner-1.4.1/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6029 2023-08-06 01:15:36.000000 dotscanner-1.4.1/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.189317 dotscanner-1.4.1/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      523 2023-08-05 23:38:08.000000 dotscanner-1.4.1/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     1111 2023-08-05 23:37:50.000000 dotscanner-1.4.1/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4439 2023-08-06 01:15:40.000000 dotscanner-1.4.1/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     9117 2023-08-06 01:15:39.000000 dotscanner-1.4.1/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.4.0/LICENSE` & `dotscanner-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/PKG-INFO` & `dotscanner-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.4.0
+Version: 1.4.1
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -179,14 +179,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+- 1.4.1
+  - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
 - 1.2.0
```

### Comparing `dotscanner-1.4.0/README.md` & `dotscanner-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+- 1.4.1
+  - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
 - 1.2.0
```

### Comparing `dotscanner-1.4.0/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.4.1/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.4.0
+Version: 1.4.1
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -179,14 +179,16 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
+- 1.4.1
+  - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
 - 1.2.0
```

### Comparing `dotscanner-1.4.0/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.4.1/dotscanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/settings/config.py` & `dotscanner-1.4.1/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/settings/configmanagement.py` & `dotscanner-1.4.1/settings/configmanagement.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/setup.py` & `dotscanner-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.4.0', # Required 
+    version='1.4.1', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.4.0/src/__main__.py` & `dotscanner-1.4.1/src/__main__.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/dataprocessing.py` & `dotscanner-1.4.1/src/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/density.py` & `dotscanner-1.4.1/src/density.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     try:
         microscopeImage = MicroscopeImage(directory, filename, userSettings)
     except:
         displayFilename = filename if len(
             filename) < 25 else f"{filename[:12]}...{filename[-12:]}"
         message = strings.reanalysisNotInFile if singleFile else strings.reanalysisNotInFolder
         DialogWindow("File not found", message.format(filename=displayFilename),
-                     "Ok", "Cancel", positiveButtonColor="blue")
+                     "Ok", "Cancel", positiveButtonAction=quit, positiveButtonColor="blue")
         quit()
     return microscopeImage
 
 
 def getReanalysisAdjustments(densityData, newUserSettings, microscopeImage):
     adjustments = [None for _ in range(8)]
     if densityData[0] != microscopeImage.lowerDotThreshScale:
```

### Comparing `dotscanner-1.4.0/src/files.py` & `dotscanner-1.4.1/src/files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/lifetime.py` & `dotscanner-1.4.1/src/lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/strings.py` & `dotscanner-1.4.1/src/strings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.4.1/src/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/DialogWindow.py` & `dotscanner-1.4.1/src/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/MicroscopeImage.py` & `dotscanner-1.4.1/src/ui/MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/RegionSelector.py` & `dotscanner-1.4.1/src/ui/RegionSelector.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/ThresholdAdjuster.py` & `dotscanner-1.4.1/src/ui/ThresholdAdjuster.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/UserSettings.py` & `dotscanner-1.4.1/src/ui/UserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/src/ui/window.py` & `dotscanner-1.4.1/src/ui/window.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_dataprocessing.py` & `dotscanner-1.4.1/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_density.py` & `dotscanner-1.4.1/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_files.py` & `dotscanner-1.4.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_fullAnalysis.py` & `dotscanner-1.4.1/tests/test_fullAnalysis.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_lifetime.py` & `dotscanner-1.4.1/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/test_strings.py` & `dotscanner-1.4.1/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/ui/FakeMicroscopeImage.py` & `dotscanner-1.4.1/tests/ui/FakeMicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/ui/FakeUserSettings.py` & `dotscanner-1.4.1/tests/ui/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.4.1/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.0/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.4.1/tests/ui/test_ThresholdAdjuster.py`

 * *Files identical despite different names*

