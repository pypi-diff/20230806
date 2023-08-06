# Comparing `tmp/dotscanner-1.4.1.tar.gz` & `tmp/dotscanner-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.4.1.tar", last modified: Sun Aug  6 01:38:20 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.4.2.tar", last modified: Sun Aug  6 03:42:04 2023, max compression
```

## Comparing `dotscanner-1.4.1.tar` & `dotscanner-1.4.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.189692 dotscanner-1.4.1/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-08-01 23:51:41.000000 dotscanner-1.4.1/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 01:38:20.189545 dotscanner-1.4.1/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    13631 2023-08-06 01:37:51.000000 dotscanner-1.4.1/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.184547 dotscanner-1.4.1/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      945 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       49 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       19 2023-08-06 01:38:20.000000 dotscanner-1.4.1/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.184922 dotscanner-1.4.1/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6219 2023-08-06 01:15:43.000000 dotscanner-1.4.1/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)     5028 2023-08-06 01:15:44.000000 dotscanner-1.4.1/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:38:20.189747 dotscanner-1.4.1/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1423 2023-08-06 01:38:19.000000 dotscanner-1.4.1/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.186026 dotscanner-1.4.1/src/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3241 2023-08-06 01:15:41.000000 dotscanner-1.4.1/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    11266 2023-08-06 00:02:21.000000 dotscanner-1.4.1/src/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)    13319 2023-08-06 01:37:52.000000 dotscanner-1.4.1/src/density.py
--rw-r--r--   0 holly      (501) staff       (20)     7759 2023-08-06 01:15:42.000000 dotscanner-1.4.1/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)    12954 2023-08-06 01:15:42.000000 dotscanner-1.4.1/src/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)    13910 2023-08-06 00:37:35.000000 dotscanner-1.4.1/src/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.187299 dotscanner-1.4.1/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5904 2023-08-06 01:15:47.000000 dotscanner-1.4.1/src/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     2397 2023-08-06 00:07:44.000000 dotscanner-1.4.1/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3964 2023-08-06 01:15:46.000000 dotscanner-1.4.1/src/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     6565 2023-08-06 01:15:46.000000 dotscanner-1.4.1/src/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    18607 2023-08-06 01:15:45.000000 dotscanner-1.4.1/src/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    19247 2023-08-06 01:15:45.000000 dotscanner-1.4.1/src/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3537 2023-08-06 01:15:44.000000 dotscanner-1.4.1/src/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.188460 dotscanner-1.4.1/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/__init__.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.188607 dotscanner-1.4.1/tests/data/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/data/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    12091 2023-08-06 01:15:39.000000 dotscanner-1.4.1/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     6950 2023-08-06 01:15:38.000000 dotscanner-1.4.1/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    14804 2023-08-06 01:15:38.000000 dotscanner-1.4.1/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     8907 2023-08-06 01:21:49.000000 dotscanner-1.4.1/tests/test_fullAnalysis.py
--rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:15:37.000000 dotscanner-1.4.1/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6029 2023-08-06 01:15:36.000000 dotscanner-1.4.1/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:38:20.189317 dotscanner-1.4.1/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      523 2023-08-05 23:38:08.000000 dotscanner-1.4.1/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     1111 2023-08-05 23:37:50.000000 dotscanner-1.4.1/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.1/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4439 2023-08-06 01:15:40.000000 dotscanner-1.4.1/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     9117 2023-08-06 01:15:39.000000 dotscanner-1.4.1/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.832469 dotscanner-1.4.2/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-08-01 23:51:41.000000 dotscanner-1.4.2/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 03:42:04.832300 dotscanner-1.4.2/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    13631 2023-08-06 03:41:05.000000 dotscanner-1.4.2/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.827252 dotscanner-1.4.2/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    14253 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      964 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       49 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       19 2023-08-06 03:42:04.000000 dotscanner-1.4.2/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.827709 dotscanner-1.4.2/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-08-06 01:15:43.000000 dotscanner-1.4.2/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)     5031 2023-08-06 03:36:32.000000 dotscanner-1.4.2/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 03:42:04.832534 dotscanner-1.4.2/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1423 2023-08-06 03:42:04.000000 dotscanner-1.4.2/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.828926 dotscanner-1.4.2/src/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3247 2023-08-06 03:40:09.000000 dotscanner-1.4.2/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    11266 2023-08-06 00:02:21.000000 dotscanner-1.4.2/src/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    13328 2023-08-06 03:38:42.000000 dotscanner-1.4.2/src/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     7776 2023-08-06 03:37:38.000000 dotscanner-1.4.2/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    12895 2023-08-06 03:35:29.000000 dotscanner-1.4.2/src/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)       69 2023-08-06 03:39:19.000000 dotscanner-1.4.2/src/programtype.py
+-rw-r--r--   0 holly      (501) staff       (20)    14232 2023-08-06 03:39:16.000000 dotscanner-1.4.2/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.830124 dotscanner-1.4.2/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5904 2023-08-06 01:15:47.000000 dotscanner-1.4.2/src/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     2397 2023-08-06 00:07:44.000000 dotscanner-1.4.2/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3980 2023-08-06 03:35:45.000000 dotscanner-1.4.2/src/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     6572 2023-08-06 03:34:06.000000 dotscanner-1.4.2/src/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    18631 2023-08-06 03:35:10.000000 dotscanner-1.4.2/src/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    19286 2023-08-06 03:35:53.000000 dotscanner-1.4.2/src/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3543 2023-08-06 03:34:44.000000 dotscanner-1.4.2/src/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.831186 dotscanner-1.4.2/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/tests/__init__.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.831370 dotscanner-1.4.2/tests/data/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/tests/data/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    12091 2023-08-06 01:15:39.000000 dotscanner-1.4.2/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     6950 2023-08-06 01:15:38.000000 dotscanner-1.4.2/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    14813 2023-08-06 03:39:18.000000 dotscanner-1.4.2/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     8907 2023-08-06 01:21:49.000000 dotscanner-1.4.2/tests/test_fullAnalysis.py
+-rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:15:37.000000 dotscanner-1.4.2/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6023 2023-08-06 03:39:17.000000 dotscanner-1.4.2/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 03:42:04.832052 dotscanner-1.4.2/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      523 2023-08-05 23:38:08.000000 dotscanner-1.4.2/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     1111 2023-08-05 23:37:50.000000 dotscanner-1.4.2/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.2/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4439 2023-08-06 01:15:40.000000 dotscanner-1.4.2/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     9117 2023-08-06 01:15:39.000000 dotscanner-1.4.2/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.4.1/LICENSE` & `dotscanner-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/PKG-INFO` & `dotscanner-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.4.1
+Version: 1.4.2
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -96,15 +96,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
-#### Use previous analysis
+#### Use previous settings
 
 This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
 
 1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
 2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
@@ -179,15 +179,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-- 1.4.1
+- 1.4.2
   - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
```

### Comparing `dotscanner-1.4.1/README.md` & `dotscanner-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
-#### Use previous analysis
+#### Use previous settings
 
 This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
 
 1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
 2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
@@ -159,15 +159,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-- 1.4.1
+- 1.4.2
   - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
```

### Comparing `dotscanner-1.4.1/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.4.2/dotscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.4.1
+Version: 1.4.2
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -96,15 +96,15 @@
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
 
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
-#### Use previous analysis
+#### Use previous settings
 
 This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
 
 1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
 2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
@@ -179,15 +179,15 @@
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-- 1.4.1
+- 1.4.2
   - Bug fixes
 - 1.4.0
   - Added option to re-analyze data on different images using previous analysis settings
 - 1.3.0
   - Added option to re-analyze data on the same image without redrawing regions
   - Added particle displacement tracking during lifetime measurement
   - Added histogram output for lifetimes measurements
```

### Comparing `dotscanner-1.4.1/dotscanner.egg-info/SOURCES.txt` & `dotscanner-1.4.2/dotscanner.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 settings/configmanagement.py
 src/__init__.py
 src/__main__.py
 src/dataprocessing.py
 src/density.py
 src/files.py
 src/lifetime.py
+src/programtype.py
 src/strings.py
 src/ui/DefaultUserSettingsEditor.py
 src/ui/DialogWindow.py
 src/ui/MicroscopeImage.py
 src/ui/RegionSelector.py
 src/ui/ThresholdAdjuster.py
 src/ui/UserSettings.py
```

### Comparing `dotscanner-1.4.1/settings/config.py` & `dotscanner-1.4.2/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/settings/configmanagement.py` & `dotscanner-1.4.2/settings/configmanagement.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,10 +149,10 @@
     quit()
 
 
 def resetConfigFile():
     configFilePath = getConfigFilePath()
 
     with open(configFilePath, "w") as file:
-        file.write(strings.defaultConfigFileContents)
+        file.write(strings.DEFAULT_CONFIG_FILE_CONTENTS)
 
     quit()
```

### Comparing `dotscanner-1.4.1/setup.py` & `dotscanner-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.4.1', # Required 
+    version='1.4.2', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
```

### Comparing `dotscanner-1.4.1/src/__main__.py` & `dotscanner-1.4.2/src/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import settings.config as cfg
 import settings.configmanagement as cm
+import src.density as density
+import src.files as files
+import src.lifetime as lifetime
+from src.programtype import ProgramType
+import src.strings as strings
 from src.ui.UserSettings import UserSettings
 from src.ui.ThresholdAdjuster import ThresholdAdjuster
 from src.ui.RegionSelector import RegionSelector
 from src.ui.MicroscopeImage import MicroscopeImage
-from src.strings import ProgramType
-import src.strings as strings
-import src.lifetime as lifetime
-import src.files as files
-import src.density as density
 
 cm.runChecks()
 
 
 def main():
     while True:
         userSettings = UserSettings()
         directory, filenames = files.getDirectoryAndFilenames(userSettings)
         if userSettings.program == ProgramType.DENSITY:
             getDensityData(directory, filenames, userSettings)
         elif userSettings.program == ProgramType.LIFETIME:
             getLifetimeData(directory, filenames, userSettings)
         else:
-            raise Exception(strings.programNameException)
+            raise Exception(strings.PROGRAM_NAME_EXCEPTION)
 
 
 def getDensityData(directory, filenames, userSettings):
     if userSettings.reanalysis:
         if len(filenames) == 1:
             density.reanalyzeSingleDensityFile(
                 directory, filenames[0], userSettings
```

### Comparing `dotscanner-1.4.1/src/dataprocessing.py` & `dotscanner-1.4.2/src/dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/src/density.py` & `dotscanner-1.4.2/src/density.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 def getMicroscopeImageFromReanalysisFile(directory, filename, userSettings, singleFile):
     microscopeImage = None
     try:
         microscopeImage = MicroscopeImage(directory, filename, userSettings)
     except:
         displayFilename = filename if len(
             filename) < 25 else f"{filename[:12]}...{filename[-12:]}"
-        message = strings.reanalysisNotInFile if singleFile else strings.reanalysisNotInFolder
+        message = strings.REANALYSIS_NOT_IN_FILE if singleFile else strings.REANALYSIS_NOT_IN_FOLDER
         DialogWindow("File not found", message.format(filename=displayFilename),
                      "Ok", "Cancel", positiveButtonAction=quit, positiveButtonColor="blue")
         quit()
     return microscopeImage
 
 
 def getReanalysisAdjustments(densityData, newUserSettings, microscopeImage):
@@ -250,15 +250,15 @@
                                       microscopeImage.lowerBlobThreshScale)
 
 
 def saveDensityDataFiles(directory, filename, targetPath, dotTotal, surveyedArea, density, error,
                          microscopeImage, userSettings, skipped=False):
     if not os.path.exists(targetPath):
         with open(targetPath, "a") as file:
-            file.write(strings.densityOutputFileHeader)
+            file.write(strings.DENSITY_OUTPUT_FILE_HEADER)
 
     if skipped:
         output = f"{filename} skipped - - - - - - - - - - - -\n"
 
     else:
         density = np.round(density, 7)
         error = np.round(error, 7)
```

### Comparing `dotscanner-1.4.1/src/files.py` & `dotscanner-1.4.2/src/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PIL import Image
 import os
 
 import settings.config as cfg
+from src.programtype import ProgramType
 import src.strings as strings
-from src.strings import ProgramType
 
 
 def fixDirectory(string):
     return string if string.endswith("/") else string + "/"
 
 
 def getDirectoryAndFilenames(userSettings, testing=False):
@@ -19,21 +19,21 @@
         filename = os.path.basename(filepath)
         return directory, [filename]
 
     elif os.path.isdir(filepath):
         directory = fixDirectory(filepath)
 
     else:
-        raise Exception(strings.filepathException)
+        raise Exception(strings.FILEPATH_EXCEPTION)
 
     filenames = getSortedFilenames(
         directory, startImage, userSettings.program, testing=testing)
 
     if not len(filenames):
-        raise Exception(strings.noFilesException)
+        raise Exception(strings.NO_FILES_EXCEPTION)
 
     return directory, filenames
 
 
 def getFilenamesWithExtension(directory, fileExtension, testing=False):
     filenames = []
     for filename in os.listdir(directory):
@@ -47,15 +47,15 @@
 
 
 def verifyImageExtension(directory, filename):
     try:
         Image.open(directory + filename)
     except:
         extension = filename.split(".")[-1]
-        print(strings.invalidImageExtension.format(extension=extension))
+        print(strings.INVALID_IMAGE_EXTENSION.format(extension=extension))
         quit()
 
 
 def getLeftEdgeOfTrailingNumber(string, index):
     if index == 0:
         return 0
 
@@ -66,15 +66,15 @@
             return index + 1
     return index + 1
 
 
 def getMostCommonFileExtension(directory):
     filenames = os.listdir(directory)
     if not len(filenames):
-        raise Exception(strings.noFilesException)
+        raise Exception(strings.NO_FILES_EXCEPTION)
 
     extensionFrequencies = {}  # Maps the extension string to the number of times it appears
     for filename in filenames:
         if filename.startswith(".") or filename.endswith(".txt"):
             continue
 
         if len(filename.split(".")) > 1:
@@ -87,15 +87,15 @@
     highestFrequency = 0
     for extension, frequency in extensionFrequencies.items():
         if frequency > highestFrequency:
             highestFrequency = frequency
             mostCommonExtension = extension
 
     if mostCommonExtension is None:
-        raise Exception(strings.noFilesException)
+        raise Exception(strings.NO_FILES_EXCEPTION)
 
     return "." + mostCommonExtension
 
 
 def getRightEdgeOfTrailingNumber(string):
     periodReached = False
     for index, char in enumerate(reversed(string)):
@@ -104,28 +104,28 @@
 
         if not periodReached:
             continue
 
         if char.isdigit():
             return len(string) - index - 1
 
-    raise Exception(strings.fileNumberingException)
+    raise Exception(strings.FILE_NUMBERING_EXCEPTION)
 
 
 def getSortedFilenames(directory, startImage, programSelected, testing=False):
     if hasNoValidFiles(directory):
         return []
 
     fileExtension = getMostCommonFileExtension(directory)
     filenames = getFilenamesWithExtension(
         directory, fileExtension, testing=testing)
 
     allFilesNumbered = allFilesAreNumbered(filenames)
     if programSelected == ProgramType.LIFETIME and not allFilesNumbered:
-        raise Exception(strings.fileNumberingException)
+        raise Exception(strings.FILE_NUMBERING_EXCEPTION)
 
     if allFilesNumbered:
         filenames.sort(key=lambda filename: getTrailingNumber(filename))
     else:
         filenames.sort()
 
     if programSelected == ProgramType.LIFETIME and startImage != "":
```

### Comparing `dotscanner-1.4.1/src/lifetime.py` & `dotscanner-1.4.2/src/lifetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import matplotlib.pyplot as pl
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 import numpy as np
 import os
 
 import settings.config as cfg
 import src.files as files
 import src.dataprocessing as dp
 import src.strings as strings
@@ -17,15 +16,15 @@
             coordsToPlot[frame] = set()
         if (x, y) not in coordsToPlot[frame]:
             coordsToPlot[frame].add((x, y))
 
 
 def checkEnoughFramesForLifetimes(filenames, userSettings):
     if len(filenames) <= 2 * (userSettings.skipsAllowed + 1):
-        raise Exception(strings.tooFewFramesException)
+        raise Exception(strings.TOO_FEW_FRAMES_EXCEPTION)
 
 
 def coordExistsInPrevFrame(y, x, imageNumber, imageNumberToCoordMap, dotSize, skipsAllowed):
     firstFrameNumber = max(0, imageNumber - skipsAllowed - 1)
     frameNumbers = range(firstFrameNumber, imageNumber)
     for frameNumber in reversed(frameNumbers):
         frameCoords = imageNumberToCoordMap[frameNumber]
@@ -136,15 +135,15 @@
             for x in xSet:
                 updateLifetimeResults(imageNumber, y, x, lifetimes, resultCoords, startImages,
                                       displacements, imageNumberToCoordMap, edgeFrameNumbers,
                                       dotSize, skipsAllowed, removeEdgeFrames,
                                       userSettings.saveFigures, coordsToPlot)
 
     if not len(lifetimes):
-        print(strings.noLifetimesFoundError)
+        print(strings.NO_LIFETIMES_FOUND_ERROR)
         quit()
 
     saveLifetimeDataFiles(directory, lifetimes, resultCoords, startImages, displacements,
                           imageNumberToBlobCoordMap, imageNumberToFilenameMap,
                           middleMicroscopeImage, userSettings, coordsToPlot,
                           middleMicroscopeImage.polygon, testing=testing)
```

### Comparing `dotscanner-1.4.1/src/strings.py` & `dotscanner-1.4.2/src/strings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,107 +1,79 @@
 import settings.config as cfg
-
-
-class ProgramType:
-    DENSITY = "Density"
-    LIFETIME = "Lifetime"
-
-
-configurationsWindowTitle = "Dot Scanner - Configurations"
-
-defaultConfigurationsEditorWindowTitle = "Dot Scanner - Default Configurations"
+from src.programtype import ProgramType
 
 
 def outputFileTopHeader(programType):
     return f"\
 # Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for {programType.lower()} measurement\n#"
 
 
-densityOutputFileHeader = f"{outputFileTopHeader(ProgramType.DENSITY)}\n\
-# If this file is selected for re-analysis, the following settings will be read in and used unless \
-changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
-output file in this same directory.\n\
-#\n\
-# lowerDotThreshScale | upperDotThreshScale | lowerBlobThreshScale | blob size | dot size | \
-upper contrast | polygon vertices\n\
-#\n\
-# Any values changed in the threshold adjustment window during re-analysis will be changed for \
-all files listed in the data output below. Other settings can be adjusted in the config file \
-using the \"Edit defaults\" button in the main configuration window.\n\
-#\n\
-# The data columns are organized as follows:\n\
-# filename | number of dots | number of pixels surveyed | \
-density (per sq {'pix' if cfg.SCALE is None else 'um'}) | error | lowerDotThreshScale | \
-upperDotThreshScale | lowerBlobThreshScale | blobSize | dotSize | lowerContrast | upperContrast | \
-polygon vertices (x, y)\n#\n"
-
-fileNumberingException = "Filenames must contain sequentially-ordered numbers with no gaps and \
-have valid file extensions to calculate lifetimes."
+CONFIGURATIONS_WINDOW_TITLE = "Dot Scanner - Configurations"
+DEFAULT_CONFIGURATIONS_EDITOR_WINDOW_TITLE = "Dot Scanner - Default Configurations"
+REGION_SELECTOR_WINDOW_TITLE = "Dot Scanner - Region Selection (click the plot to add polygon vertices)"
+THRESHOLD_ADJUSTER_WINDOW_TITLE = "Dot Scanner - Threshold Adjustment"
+
+DENSITY_OUTPUT_FILE_HEADER = '''{header}
+# If this file is selected for re-analysis, the following settings will be read in and used unless changed in the threshold adjustment window. The re-analyzed data will then be given in a new output file in this same directory.
+#
+# lowerDotThreshScale | upperDotThreshScale | lowerBlobThreshScale | blob size | dot size | upper contrast | polygon vertices
+#
+# Any values changed in the threshold adjustment window during re-analysis will be changed for all files listed in the data output below. Other settings can be adjusted in the config file using the "Edit defaults" button in the main configuration window.
+#
+# The data columns are organized as follows:
+# filename | number of dots | number of pixels surveyed | density (per sq {unit}) | error | lowerDotThreshScale | upperDotThreshScale | lowerBlobThreshScale | blobSize | dotSize | lowerContrast | upperContrast | polygon vertices (x, y)
+#
+'''.format(header=outputFileTopHeader(ProgramType.DENSITY), unit="pix" if cfg.SCALE is None else "um")
+
+FILE_NUMBERING_EXCEPTION = "Filenames must contain sequentially-ordered numbers with no gaps and have valid file extensions to calculate lifetimes."
 
-fileNumberingWarning = "WARNING: Filenames must contain sequentially-ordered numbers to calculate \
-lifetimes."
+FILE_NUMBERING_WARNING = "WARNING: Filenames must contain sequentially-ordered numbers to calculate lifetimes."
 
-filepathException = "Filepath must point to a file or directory."
+FILEPATH_EXCEPTION = "Filepath must point to a file or directory."
 
-invalidImageExtension = '''
+INVALID_IMAGE_EXTENSION = '''
 "{extension}" is not a valid image extension. 
 Make sure the most common file type in the folder you've selected has a valid extension.'''
 
-invalidPolygonWarning = "\nNo valid, enclosed polygon drawn. No measurements made."
+INVALID_POLYGON_WARNING = "\nNo valid, enclosed polygon drawn. No measurements made."
 
-invalidDotAndBlobSizeEdit = "\nInvalid input. Previous dot and blob size values will be retained."
+INVALID_DOT_AND_BLOB_SIZE_EDIT = "\nInvalid input. Previous dot and blob size values will be retained."
 
-invalidThresholdEdit = "\nInvalid input. Previous threshold values will be retained."
+INVALID_THRESHOLD_EDIT = "\nInvalid input. Previous threshold values will be retained."
 
-lifetimeSingleFileException = "Lifetimes must be calculated using a directory of images, \
-not a single image."
+LIFETIME_SINGLE_FILE_WARNING = "WARNING: Lifetimes must be calculated using a directory of images, not a single image."
 
-lifetimeSingleFileWarning = "WARNING: Lifetimes must be calculated using a directory of images, \
-not a single image."
+LOWER_BLOB_THRESH_SCALE_WARNING = "\nWARNING: Lower blob threshold scale set below 1.0, which means blobs can be dimmer than the brightest dots, which shouldn't happen. Setting to 1.0."
 
-lowerBlobThreshScaleWarning = "\nWARNING: Lower blob threshold scale set below 1.0, which means \
-blobs can be dimmer than the brightest dots, which shouldn't happen. Setting to 1.0."
+MAX_CONTRAST_WARNING = "\nWARNING: Max contrast reached. Previous contrast values will be retained."
 
-maxContrastWarning = "\nWARNING: Max contrast reached. Previous contrast values will be retained."
+NO_FILES_EXCEPTION = "No valid files selected. Does the folder you've selected contain files with valid file extensions (e.g., .tiff)? Subfolders within the selected folder will not be scanned for files. Check the values of 'FILEPATH' and 'START_IMAGE' in the configurations file."
 
-noFilesException = "No valid files selected. Does the folder you've selected contain files with \
-valid file extensions (e.g., .tiff)? Subfolders within the selected folder will not be scanned for \
-files. Check the values of 'FILEPATH' and 'START_IMAGE' in the configurations file."
-
-noLifetimesFoundError = """
+NO_LIFETIMES_FOUND_ERROR = """
 No lifetimes measured.
 Check that your images are arranged as a time series."""
 
-programNameException = "Invalid program name selected in configurations file."
+PROGRAM_NAME_EXCEPTION = "Invalid program name selected in configurations file."
 
-reanalysisNotInFile = """Filename not found in reanalysis file:
+REANALYSIS_NOT_IN_FILE = """Filename not found in reanalysis file:
 {filename}
 Reanalysis requires identical naming."""
 
-reanalysisNotInFolder = """Filename not found in images folder:
+REANALYSIS_NOT_IN_FOLDER = """Filename not found in images folder:
 {filename}
 Reanalysis requires identical naming."""
 
-regionSelectorWindowTitle = "Dot Scanner - Region Selection (click the plot to add polygon \
-vertices)"
-
-startImageDirectoryWarning = "WARNING: Start image must be in the same directory as the other \
-lifetime files."
-
-thresholdAdjusterWindowTitle = "Dot Scanner - Threshold Adjustment"
+START_IMAGE_DIRECTORY_WARNING = "WARNING: Start image must be in the same directory as the other lifetime files."
 
-tooFewFramesException = "There are not enough images to get meaningful lifetimes."
+TOO_FEW_FRAMES_EXCEPTION = "There are not enough images to get meaningful lifetimes."
 
-upperDotThreshScaleWarning = "\nWARNING: Upper dot threshold scale set below lower dot threshold \
-scale. Previous threshold values will be retained."
+UPPER_DOT_THRESH_SCALE_WARNING = "\nWARNING: Upper dot threshold scale set below lower dot threshold scale. Previous threshold values will be retained."
 
-windowSizeWarning = "\nWARNING: The current window height is smaller than 550 pixels, potentially \
-resulting in some buttons not being visible. However, the Return key will still allow confirmation \
-in each window, and the Escape key will allow for skipping files, when the option is available."
+WINDOW_SIZE_WARNING = "\nWARNING: The current window height is smaller than 550 pixels, potentially resulting in some buttons not being visible. However, the Return key will still allow confirmation in each window, and the Escape key will allow for skipping files, when the option is available."
 
 
 def alreadyMeasuredNotification(filename):
     return f"\nFile {filename} already measured in {cfg.DENSITY_OUTPUT_FILENAME} file. Skipping."
 
 
 def densityOutput(filename, dotTotal, surveyedArea, density, error, microscopeImage, userSettings):
@@ -134,52 +106,65 @@
 
 
 def invalidFilenameInDensityAnalysisFile(lineArray):
     return f"Filename with valid extension not found in the following line in densities file:\n\
 {' '.join(lineArray)}"
 
 
+LIFETIME_OUTPUT_FILE_HEADER_TEMPLATE = '''{header}
+# If this file is selected for re-analysis, the following settings will be read in and used unless changed in the threshold adjustment window. The re-analyzed data will then be given in a new output file in this same directory.
+#
+# Polygon vertices (x, y): {verticesString}
+# Threshold scales: {thresholdsString}
+# Contrast settings: {lowerContrast}, {upperContrast}
+# Dot size: {dotSize} | Blob size: {blobSize}
+#
+# The following settings were used in this analysis, but will not be read in during re-analysis (these and other settings can be adjusted in the config file using the "Edit defaults" button in the main configuration window):
+#
+# Remove edge frames: {removeEdgeFrames} | Save figures: {saveFigures} | Skips allowed: {skipsAllowed}{startImageHeaderText}
+#
+# The data columns are organized as follows:
+# x | y | lifetime | starting image | displacement squared (sq px)
+#
+'''
+
+
 def lifetimeOutputFileHeader(microscopeImage, userSettings):
     verticesStringList = []
     for vertex in microscopeImage.polygon[:-1]:
         y, x = vertex
         verticesStringList.append(f"({x}, {y})")
     verticesString = ", ".join(verticesStringList)
 
     thresholdsStringList = []
     for threshold in microscopeImage.thresholds:
         thresholdsStringList.append(str(threshold))
     thresholdsString = ", ".join(thresholdsStringList)
 
-    return f"{outputFileTopHeader(ProgramType.LIFETIME)}\n\
-# If this file is selected for re-analysis, the following settings will be read in and used unless \
-changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
-output file in this same directory.\n\
-#\n\
-# Polygon vertices (x, y): {verticesString}\n\
-# Threshold scales: {thresholdsString}\n\
-# Contrast settings: {userSettings.lowerContrast}, {userSettings.upperContrast}\n\
-# Dot size: {userSettings.dotSize} | Blob size: {userSettings.blobSize}\n\
-#\n\
-# The following settings were used in this analysis, but will not be read in during re-analysis \
-(these and other settings can be adjusted in the config file using the \"Edit defaults\" button \
-in the main configuration window):\n\
-#\n\
-# Remove edge frames: \
-{userSettings.removeEdgeFrames} | Save figures: {userSettings.saveFigures} | Skips allowed: \
-{userSettings.skipsAllowed}{getLifetimeStartImageHeaderText(userSettings.startImage)}\n#\n\
-# The data columns are organized as follows:\n\
-# x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
+    return LIFETIME_OUTPUT_FILE_HEADER_TEMPLATE.format(
+        header=outputFileTopHeader(ProgramType.LIFETIME),
+        verticesString=verticesString,
+        thresholdsString=thresholdsString,
+        lowerContrast=userSettings.lowerContrast,
+        upperContrast=userSettings.upperContrast,
+        dotSize=userSettings.dotSize,
+        blobSize=userSettings.blobSize,
+        removeEdgeFrames=userSettings.removeEdgeFrames,
+        saveFigures=userSettings.saveFigures,
+        skipsAllowed=userSettings.skipsAllowed,
+        startImageHeaderText=getLifetimeStartImageHeaderText(
+            userSettings.startImage)
+    )
 
 
 def getLifetimeStartImageHeaderText(startImage):
     return f" | Start image: {startImage.split('/')[-1]}" if startImage != "" else ""
 
 
-defaultConfigFileContents = '''# Default selections run by the software (can be changed by the user):
+DEFAULT_CONFIG_FILE_CONTENTS = '''# Default selections run by the software (can be changed by the user):
 
 FILEPATH = ""
 # Path to the file or directory of files that should be used. The default value is an empty string: ""
 
 PROGRAM = "density"
 # Whether a "density" program or "lifetime" program should be run
```

### Comparing `dotscanner-1.4.1/src/ui/DefaultUserSettingsEditor.py` & `dotscanner-1.4.2/src/ui/DefaultUserSettingsEditor.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/src/ui/DialogWindow.py` & `dotscanner-1.4.2/src/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/src/ui/MicroscopeImage.py` & `dotscanner-1.4.2/src/ui/MicroscopeImage.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.updateThresholds()
         self.dotCoords, self.blobCoords = self.getCoords()
 
     def decreaseUpperDotThreshScale(self):
         value = self.upperDotThreshScale - cfg.THRESHOLD_DELTA
         value = round(value, 1)
         if value < self.lowerDotThreshScale:
-            print(strings.upperDotThreshScaleWarning)
+            print(strings.UPPER_DOT_THRESH_SCALE_WARNING)
             return
         self.upperDotThreshScale = value
         self.updateThresholds()
         self.dotCoords, self.blobCoords = self.getCoords()
 
     def getCoords(self):
         combination = (self.thresholds,
@@ -58,15 +58,15 @@
         else:
             return []
 
     def increaseLowerDotThreshScale(self):
         value = self.lowerDotThreshScale + cfg.THRESHOLD_DELTA
         value = round(value, 1)
         if value > self.upperDotThreshScale:
-            print(strings.upperDotThreshScaleWarning)
+            print(strings.UPPER_DOT_THRESH_SCALE_WARNING)
             return
         self.lowerDotThreshScale = value
         self.updateThresholds()
         self.dotCoords, self.blobCoords = self.getCoords()
 
     def increaseUpperDotThreshScale(self):
         value = self.upperDotThreshScale + cfg.THRESHOLD_DELTA
@@ -77,19 +77,19 @@
 
     def setThresholds(self, newThresholds):
         newLowerDotThreshScale = round(newThresholds[0], 1)
         newUpperDotThreshScale = round(newThresholds[1], 1)
         newLowerBlobThreshScale = round(newThresholds[2], 1)
 
         if newUpperDotThreshScale < newLowerDotThreshScale:
-            print(strings.upperDotThreshScaleWarning)
+            print(strings.UPPER_DOT_THRESH_SCALE_WARNING)
             return
 
         if newLowerBlobThreshScale < 1:
-            print(strings.lowerBlobThreshScaleWarning)
+            print(strings.LOWER_BLOB_THRESH_SCALE_WARNING)
             newLowerBlobThreshScale = 1.0
 
         self.lowerDotThreshScale = newLowerDotThreshScale
         self.upperDotThreshScale = newUpperDotThreshScale
         self.lowerBlobThreshScale = newLowerBlobThreshScale
 
         self.updateThresholds()
```

### Comparing `dotscanner-1.4.1/src/ui/RegionSelector.py` & `dotscanner-1.4.2/src/ui/RegionSelector.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         self.xList, self.yList = [], []
         self.drawingBlocked = False
         if userSettings.reanalysis:
             self.setPolygonData(microscopeImage)
 
         self.image = microscopeImage
-        self.window = ui.createPlotWindow(strings.regionSelectorWindowTitle)
+        self.window = ui.createPlotWindow(strings.REGION_SELECTOR_WINDOW_TITLE)
 
         self.figure, self.axes, _, self.dotScatter, self.blobScatter = ui.createPlots(
             self.image.data, userSettings)
 
         self.clickMarkerBackdrop = self.axes.scatter(
             [None], [None], s=100, marker='x', color="k", linewidth=4)
         self.underLine, = self.axes.plot(
@@ -113,15 +113,15 @@
                 self.xList.append(self.xList[0])
                 self.yList.append(self.yList[0])
                 for y, x in zip(self.yList, self.xList):
                     self.image.polygon.append(
                         [int(round(y, 0)), int(round(x, 0))])
 
             else:  # An invalid polygon was drawn
-                print(strings.invalidPolygonWarning)
+                print(strings.INVALID_POLYGON_WARNING)
 
         self.line.figure.canvas.mpl_disconnect(self.connectId)
         self.window.destroy()
         self.window.after(100, self.window.quit)
 
     def finishWithReturnKey(self, _):
         self.finish()
@@ -147,15 +147,15 @@
         self.clickMarkerBackdrop.set_offsets([None, None])
         self.clickMarker.set_offsets([None, None])
         self.clickMarkerBackdrop.figure.canvas.draw_idle()
         self.clickMarker.figure.canvas.draw_idle()
 
     def setPolygonData(self, microscopeImage):
         if not microscopeImage.polygon:
-            raise Exception(strings.invalidPolygonWarning)
+            raise Exception(strings.INVALID_POLYGON_WARNING)
         for pair in microscopeImage.polygon:
             y, x = pair
             self.xList.append(x)
             self.yList.append(y)
         self.drawingBlocked = True
 
     def skip(self):
```

### Comparing `dotscanner-1.4.1/src/ui/ThresholdAdjuster.py` & `dotscanner-1.4.2/src/ui/ThresholdAdjuster.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
             (len(self.image.data) / 2,    len(self.image.data) - 1),
             (len(self.image.data) / 2,    len(self.image.data) - 1),
             (0,                           len(self.image.data) / 2),
             (0,                           len(self.image.data) / 2),
         ]
 
         ui.setupWindow()
-        self.window = ui.createPlotWindow(strings.thresholdAdjusterWindowTitle)
+        self.window = ui.createPlotWindow(
+            strings.THRESHOLD_ADJUSTER_WINDOW_TITLE)
         self.windowScaling = ui.getWindowScaling()
 
         self.figure, self.axes, self.dataPlot, self.dotScatter, self.blobScatter = ui.createPlots(
             self.image.data, userSettings)
 
         dp.setScatterData(
             self.image.dotCoords, self.image.blobCoords, self.dotScatter, self.blobScatter)
@@ -291,28 +292,28 @@
             numberIn1 = round(float(self.entryThreshold1.get()), 1)
             numberIn2 = round(float(self.entryThreshold2.get()), 1)
             numberIn3 = round(float(self.entryThreshold3.get()), 1)
             newThresholds = (numberIn1, numberIn2, numberIn3)
 
         except:
             self.setThresholdEntries(self.image.thresholds)
-            print(strings.invalidThresholdEdit)
+            print(strings.INVALID_THRESHOLD_EDIT)
             return
 
         try:
             self.dotSize = int(round(float(self.entryDotSize.get()), 0))
             self.blobSize = int(round(float(self.entryBlobSize.get()), 0))
             self.image.dotSize = self.dotSize
             self.image.blobSize = self.blobSize
             self.userSettings.dotSize = self.dotSize
             self.userSettings.blobSize = self.blobSize
 
         except:
             self.setDotAndBlobSizeEntries(self.dotSize, self.blobSize)
-            print(strings.invalidDotAndBlobSizeEdit)
+            print(strings.INVALID_DOT_AND_BLOB_SIZE_EDIT)
             return
 
         self.image.setThresholds(newThresholds)
         self.setThresholdEntries(self.image.thresholds)
 
         self.image.dotCoords, self.image.blobCoords = self.image.getCoords()
         dp.setScatterData(self.image.dotCoords, self.image.blobCoords, self.dotScatter,
```

### Comparing `dotscanner-1.4.1/src/ui/UserSettings.py` & `dotscanner-1.4.2/src/ui/UserSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import tkinter as tk
 from tkinter import filedialog
 
 import settings.config as cfg
 import src.files as files
+from src.programtype import ProgramType
 import src.strings as strings
-from src.strings import ProgramType
 import src.ui.window as ui
 from src.ui.DefaultUserSettingsEditor import DefaultUserSettingsEditor
 
 EMPTY_DIRECTORY_SET = set(["", " ", "/"])
 
 
 class UserSettings:
@@ -190,21 +190,21 @@
         chosenImage = os.path.basename(chosenFilepath)
         if chosenImage != "":
             if os.path.isfile(self.filepath):
                 self.buttonSelectStartingImage.config(
                     text="Browse...", fg="black")
                 self.startImage = ""
                 self.labelWarning.configure(
-                    text=strings.lifetimeSingleFileWarning)
+                    text=strings.LIFETIME_SINGLE_FILE_WARNING)
             elif os.path.dirname(chosenFilepath) != self.filepath:
                 self.buttonSelectStartingImage.config(
                     text="Browse...", fg="black")
                 self.startImage = ""
                 self.labelWarning.configure(
-                    text=strings.startImageDirectoryWarning)
+                    text=strings.START_IMAGE_DIRECTORY_WARNING)
 
             else:
                 try:
                     trailingNumberString = str(
                         files.getTrailingNumber(chosenImage))
                     if len(trailingNumberString) > 10:
                         trailingNumberString = "..." + \
@@ -214,30 +214,31 @@
                     self.startImage = chosenImage
 
                 except:
                     self.buttonSelectStartingImage.config(
                         text="Browse...", fg="black")
                     self.startImage = ""
                     self.labelWarning.configure(
-                        text=strings.fileNumberingWarning)
+                        text=strings.FILE_NUMBERING_WARNING)
 
         self.window.update()
         self.window.focus_force()
 
     def checkForWarning(self):
         if os.path.isfile(self.filepath) and self.program == ProgramType.LIFETIME:
-            self.labelWarning.configure(text=strings.lifetimeSingleFileWarning)
+            self.labelWarning.configure(
+                text=strings.LIFETIME_SINGLE_FILE_WARNING)
         else:
             self.labelWarning.configure(text="")
 
     def decreaseUpperContrast(self):
         value = self.upperContrast - cfg.CONTRAST_DELTA
         value = round(value, 1)
         if value <= self.lowerContrast:
-            print(strings.maxContrastWarning)
+            print(strings.MAX_CONTRAST_WARNING)
             return
         self.upperContrast = value
 
     def done(self):
         if self.filepathNotSet():
             return
         self.dotSize = int(self.entryDotSize.get())
@@ -246,15 +247,15 @@
         self.upperDotThresh = round(float(self.entryThreshold2.get()), 1)
         self.lowerBlobThresh = round(float(self.entryThreshold3.get()), 1)
         self.skipsAllowed = int(self.entrySkipsAllowed.get())
         self.thresholds = (self.lowerDotThresh,
                            self.upperDotThresh, self.lowerBlobThresh)
         if not cfg.DYNAMIC_WINDOW:
             if cfg.WINDOW_HEIGHT < 550:
-                print(strings.windowSizeWarning)
+                print(strings.WINDOW_SIZE_WARNING)
         self.window.destroy()
         self.window.quit()
 
     def doneWithReturnKey(self, _):
         self.done()
 
     def editDefaults(self):
@@ -262,15 +263,15 @@
 
     def getProgramType(self, programString):
         if programString.lower() == "density":
             return ProgramType.DENSITY
         elif programString.lower() == "lifetime":
             return ProgramType.LIFETIME
         else:
-            raise Exception(strings.programNameException)
+            raise Exception(strings.PROGRAM_NAME_EXCEPTION)
 
     def filepathNotSet(self):
         return self.filepath in EMPTY_DIRECTORY_SET
 
     def increaseUpperContrast(self):
         value = self.upperContrast + cfg.CONTRAST_DELTA
         value = round(value, 1)
```

### Comparing `dotscanner-1.4.1/src/ui/window.py` & `dotscanner-1.4.2/src/ui/window.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,25 +22,25 @@
                                facecolors="none", edgecolor=cfg.BLOB_COLOR,
                                linewidths=cfg.BLOB_THICKNESS)
     return figure, axes, dataPlot, dotScatter, blobScatter
 
 
 def createConfigurationsWindow():
     window = tk.Tk()
-    window.title(strings.configurationsWindowTitle)
+    window.title(strings.CONFIGURATIONS_WINDOW_TITLE)
     width, _ = getWindowDimensions()
     if width > 650:
         width = 650
     window.geometry(f"{width}x170+{cfg.WINDOW_X}+{cfg.WINDOW_Y}")
     return window
 
 
 def createDefaultConfigurationsEditorWindow():
     window = tk.Tk()
-    window.title(strings.defaultConfigurationsEditorWindowTitle)
+    window.title(strings.DEFAULT_CONFIGURATIONS_EDITOR_WINDOW_TITLE)
     width, _ = getWindowDimensions()
     if width > 650:
         width = 650
     window.geometry(f"{width}x170+{cfg.WINDOW_X + 20}+{cfg.WINDOW_Y + 20}")
     return window
```

### Comparing `dotscanner-1.4.1/tests/test_dataprocessing.py` & `dotscanner-1.4.2/tests/test_dataprocessing.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/test_density.py` & `dotscanner-1.4.2/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/test_files.py` & `dotscanner-1.4.2/tests/test_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import mock
 import unittest
 
 import src.files as files
+from src.programtype import ProgramType
 import src.strings as strings
-from src.strings import ProgramType
 from tests.ui.FakeUserSettings import FakeUserSettings
 
 
 class TestFiles(unittest.TestCase):
     def getTestFilenames(self):
         return ["file03.png", "file02.png", "file01.png", "file05.PNG", "file04.png", "file11.png",
                 "readme.md", "test", "directory2/"]
@@ -213,15 +213,15 @@
         mock_isdir.return_value = True
         mock_listdir.return_value = []
 
         with self.assertRaises(Exception) as context:
             directory, filenames = files.getDirectoryAndFilenames(
                 fakeUserSettings, testing=True)
 
-        self.assertTrue(strings.noFilesException in str(context.exception))
+        self.assertTrue(strings.NO_FILES_EXCEPTION in str(context.exception))
 
     @mock.patch("src.files.os.listdir")
     @mock.patch("src.files.os.path.isdir")
     @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forNeitherFileNorDirectory(self, mock_isfile, mock_isdir,
                                                                  mock_listdir):
         fakeUserSettings = FakeUserSettings()
@@ -229,15 +229,15 @@
         mock_isdir.return_value = False
         mock_listdir.return_value = []
 
         with self.assertRaises(Exception) as context:
             directory, filenames = files.getDirectoryAndFilenames(
                 fakeUserSettings, testing=True)
 
-        self.assertTrue(strings.filepathException in str(context.exception))
+        self.assertTrue(strings.FILEPATH_EXCEPTION in str(context.exception))
 
     @mock.patch("src.files.os.listdir")
     @mock.patch("src.files.os.path.isdir")
     @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forFilesWithoutExtensions(self, mock_isfile, mock_isdir,
                                                                 mock_listdir):
         fakeUserSettings = FakeUserSettings()
@@ -245,15 +245,15 @@
         mock_isdir.return_value = True
         mock_listdir.return_value = ["file", "file2"]
 
         with self.assertRaises(Exception) as context:
             directory, filenames = files.getDirectoryAndFilenames(
                 fakeUserSettings, testing=True)
 
-        self.assertTrue(strings.noFilesException in str(context.exception))
+        self.assertTrue(strings.NO_FILES_EXCEPTION in str(context.exception))
 
     @mock.patch("src.files.os.listdir")
     @mock.patch("src.files.os.path.isdir")
     @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forFilesWithoutNumbers(self, mock_isfile, mock_isdir,
                                                              mock_listdir):
         fakeUserSettings = FakeUserSettings()
```

### Comparing `dotscanner-1.4.1/tests/test_fullAnalysis.py` & `dotscanner-1.4.2/tests/test_fullAnalysis.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/test_lifetime.py` & `dotscanner-1.4.2/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/test_strings.py` & `dotscanner-1.4.2/tests/test_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import mock
 import unittest
 
+from src.programtype import ProgramType
 import src.strings as strings
-import settings.config as cfg
 from tests.ui.FakeMicroscopeImage import FakeMicroscopeImage
 from tests.ui.FakeUserSettings import FakeUserSettings
 
 
 class TestStrings(unittest.TestCase):
     @mock.patch("settings.config.DENSITY_OUTPUT_FILENAME", "density.txt")
     def test_alreadyMeasuredNotification(self):
@@ -55,20 +55,20 @@
                 ["file", "array", "example"]),
             f"Filename with valid extension not found in the following line in densities file:\n\
 file array example"
         )
 
     def test_outputFileTopHeader(self):
         self.assertEqual(
-            strings.outputFileTopHeader(strings.ProgramType.DENSITY),
+            strings.outputFileTopHeader(ProgramType.DENSITY),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for density measurement\n#"
         )
         self.assertEqual(
-            strings.outputFileTopHeader(strings.ProgramType.LIFETIME),
+            strings.outputFileTopHeader(ProgramType.LIFETIME),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n#"
         )
 
     def test_lifetimeOutputFileHeader(self):
         fakeMicroscopeImage = FakeMicroscopeImage(
             polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5,
```

### Comparing `dotscanner-1.4.1/tests/ui/FakeMicroscopeImage.py` & `dotscanner-1.4.2/tests/ui/FakeMicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/ui/FakeUserSettings.py` & `dotscanner-1.4.2/tests/ui/FakeUserSettings.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/ui/test_MicroscopeImage.py` & `dotscanner-1.4.2/tests/ui/test_MicroscopeImage.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.4.1/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.4.2/tests/ui/test_ThresholdAdjuster.py`

 * *Files identical despite different names*

