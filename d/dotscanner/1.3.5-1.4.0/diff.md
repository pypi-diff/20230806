# Comparing `tmp/dotscanner-1.3.5.tar.gz` & `tmp/dotscanner-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotscanner-1.3.5.tar", last modified: Thu Jul 20 22:24:37 2023, max compression
+gzip compressed data, was "dist/dotscanner-1.4.0.tar", last modified: Sun Aug  6 01:28:14 2023, max compression
```

## Comparing `dotscanner-1.3.5.tar` & `dotscanner-1.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.410915 dotscanner-1.3.5/
--rw-r--r--   0 holly      (501) staff       (20)     1103 2023-06-05 02:24:39.000000 dotscanner-1.3.5/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)    13629 2023-07-20 22:24:37.410735 dotscanner-1.3.5/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)    12974 2023-07-20 22:19:47.000000 dotscanner-1.3.5/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.405744 dotscanner-1.3.5/dotscanner/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/dotscanner/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2755 2023-06-07 06:04:06.000000 dotscanner-1.3.5/dotscanner/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    10277 2023-06-06 23:47:07.000000 dotscanner-1.3.5/dotscanner/dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)    10147 2023-06-07 06:04:08.000000 dotscanner-1.3.5/dotscanner/density.py
--rw-r--r--   0 holly      (501) staff       (20)     6462 2023-07-20 21:39:52.000000 dotscanner-1.3.5/dotscanner/files.py
--rw-r--r--   0 holly      (501) staff       (20)    10595 2023-06-07 06:04:07.000000 dotscanner-1.3.5/dotscanner/lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6867 2023-07-20 21:46:19.000000 dotscanner-1.3.5/dotscanner/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.408101 dotscanner-1.3.5/dotscanner/ui/
--rw-r--r--   0 holly      (501) staff       (20)     5179 2023-06-06 23:47:11.000000 dotscanner-1.3.5/dotscanner/ui/DefaultUserSettingsEditor.py
--rw-r--r--   0 holly      (501) staff       (20)     1858 2023-06-06 23:47:12.000000 dotscanner-1.3.5/dotscanner/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     3510 2023-06-07 03:30:32.000000 dotscanner-1.3.5/dotscanner/ui/MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     5764 2023-06-07 06:04:13.000000 dotscanner-1.3.5/dotscanner/ui/RegionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)    16392 2023-06-07 06:12:10.000000 dotscanner-1.3.5/dotscanner/ui/ThresholdAdjuster.py
--rw-r--r--   0 holly      (501) staff       (20)    15478 2023-07-20 22:12:44.000000 dotscanner-1.3.5/dotscanner/ui/UserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/dotscanner/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     3097 2023-06-06 23:47:14.000000 dotscanner-1.3.5/dotscanner/ui/window.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.406952 dotscanner-1.3.5/dotscanner.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)    13629 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     1050 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       56 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       17 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/requires.txt
--rw-r--r--   0 holly      (501) staff       (20)       26 2023-07-20 22:24:37.000000 dotscanner-1.3.5/dotscanner.egg-info/top_level.txt
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.408502 dotscanner-1.3.5/settings/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/settings/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     6219 2023-06-06 20:41:22.000000 dotscanner-1.3.5/settings/config.py
--rw-r--r--   0 holly      (501) staff       (20)    11284 2023-06-05 02:24:39.000000 dotscanner-1.3.5/settings/configmanagement.py
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-07-20 22:24:37.410982 dotscanner-1.3.5/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1444 2023-07-20 22:24:37.000000 dotscanner-1.3.5/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.409651 dotscanner-1.3.5/tests/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/__init__.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.409787 dotscanner-1.3.5/tests/data/
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/data/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)    10018 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/test_dataprocessing.py
--rw-r--r--   0 holly      (501) staff       (20)     5619 2023-06-07 06:18:09.000000 dotscanner-1.3.5/tests/test_density.py
--rw-r--r--   0 holly      (501) staff       (20)    14518 2023-07-20 21:50:56.000000 dotscanner-1.3.5/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     7470 2023-06-16 00:50:00.000000 dotscanner-1.3.5/tests/test_fullAnalysis.py
--rw-r--r--   0 holly      (501) staff       (20)    10886 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/test_lifetime.py
--rw-r--r--   0 holly      (501) staff       (20)     6051 2023-07-20 21:53:10.000000 dotscanner-1.3.5/tests/test_strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-07-20 22:24:37.410476 dotscanner-1.3.5/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)      487 2023-06-07 03:30:33.000000 dotscanner-1.3.5/tests/ui/FakeMicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     1086 2023-06-07 06:04:14.000000 dotscanner-1.3.5/tests/ui/FakeUserSettings.py
--rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.3.5/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     4099 2023-06-07 03:02:28.000000 dotscanner-1.3.5/tests/ui/test_MicroscopeImage.py
--rw-r--r--   0 holly      (501) staff       (20)     8287 2023-06-07 06:12:11.000000 dotscanner-1.3.5/tests/ui/test_ThresholdAdjuster.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.558785 dotscanner-1.4.0/
+-rw-r--r--   0 holly      (501) staff       (20)     1103 2023-08-01 23:51:41.000000 dotscanner-1.4.0/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:28:14.558629 dotscanner-1.4.0/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)    13607 2023-08-06 00:19:42.000000 dotscanner-1.4.0/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.554039 dotscanner-1.4.0/dotscanner.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      945 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       49 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       17 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/requires.txt
+-rw-r--r--   0 holly      (501) staff       (20)       19 2023-08-06 01:28:14.000000 dotscanner-1.4.0/dotscanner.egg-info/top_level.txt
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.554507 dotscanner-1.4.0/settings/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/settings/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     6219 2023-08-06 01:15:43.000000 dotscanner-1.4.0/settings/config.py
+-rw-r--r--   0 holly      (501) staff       (20)     5028 2023-08-06 01:15:44.000000 dotscanner-1.4.0/settings/configmanagement.py
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:28:14.558845 dotscanner-1.4.0/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1423 2023-08-06 01:28:14.000000 dotscanner-1.4.0/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.555535 dotscanner-1.4.0/src/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3241 2023-08-06 01:15:41.000000 dotscanner-1.4.0/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)    11266 2023-08-06 00:02:21.000000 dotscanner-1.4.0/src/dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)    13292 2023-08-06 01:15:43.000000 dotscanner-1.4.0/src/density.py
+-rw-r--r--   0 holly      (501) staff       (20)     7759 2023-08-06 01:15:42.000000 dotscanner-1.4.0/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)    12954 2023-08-06 01:15:42.000000 dotscanner-1.4.0/src/lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)    13910 2023-08-06 00:37:35.000000 dotscanner-1.4.0/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.556699 dotscanner-1.4.0/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     5904 2023-08-06 01:15:47.000000 dotscanner-1.4.0/src/ui/DefaultUserSettingsEditor.py
+-rw-r--r--   0 holly      (501) staff       (20)     2397 2023-08-06 00:07:44.000000 dotscanner-1.4.0/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     3964 2023-08-06 01:15:46.000000 dotscanner-1.4.0/src/ui/MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     6565 2023-08-06 01:15:46.000000 dotscanner-1.4.0/src/ui/RegionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)    18607 2023-08-06 01:15:45.000000 dotscanner-1.4.0/src/ui/ThresholdAdjuster.py
+-rw-r--r--   0 holly      (501) staff       (20)    19247 2023-08-06 01:15:45.000000 dotscanner-1.4.0/src/ui/UserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     3537 2023-08-06 01:15:44.000000 dotscanner-1.4.0/src/ui/window.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.557622 dotscanner-1.4.0/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/__init__.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.557764 dotscanner-1.4.0/tests/data/
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/data/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)    12091 2023-08-06 01:15:39.000000 dotscanner-1.4.0/tests/test_dataprocessing.py
+-rw-r--r--   0 holly      (501) staff       (20)     6950 2023-08-06 01:15:38.000000 dotscanner-1.4.0/tests/test_density.py
+-rw-r--r--   0 holly      (501) staff       (20)    14804 2023-08-06 01:15:38.000000 dotscanner-1.4.0/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     8907 2023-08-06 01:21:49.000000 dotscanner-1.4.0/tests/test_fullAnalysis.py
+-rw-r--r--   0 holly      (501) staff       (20)    14231 2023-08-06 01:15:37.000000 dotscanner-1.4.0/tests/test_lifetime.py
+-rw-r--r--   0 holly      (501) staff       (20)     6029 2023-08-06 01:15:36.000000 dotscanner-1.4.0/tests/test_strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:28:14.558400 dotscanner-1.4.0/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)      523 2023-08-05 23:38:08.000000 dotscanner-1.4.0/tests/ui/FakeMicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     1111 2023-08-05 23:37:50.000000 dotscanner-1.4.0/tests/ui/FakeUserSettings.py
+-rw-r--r--   0 holly      (501) staff       (20)        0 2023-06-05 02:24:39.000000 dotscanner-1.4.0/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     4439 2023-08-06 01:15:40.000000 dotscanner-1.4.0/tests/ui/test_MicroscopeImage.py
+-rw-r--r--   0 holly      (501) staff       (20)     9117 2023-08-06 01:15:39.000000 dotscanner-1.4.0/tests/ui/test_ThresholdAdjuster.py
```

### Comparing `dotscanner-1.3.5/LICENSE` & `dotscanner-1.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Holly Allen and Brian Davis
+Copyright (c) 2023 Holly Allen and Brian Davis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dotscanner-1.3.5/PKG-INFO` & `dotscanner-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.5
+Version: 1.4.0
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -15,184 +15,215 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dot Scanner
+
 > Software designed for analysis of microscope imaging data
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
-Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
+Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is _especially_ useful for noisy image data, where manual "by-eye" analysis is unreliable.
 
 ## Getting Started
 
 ### Dependencies
 
-[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
+[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed.
 
 ### Installation
 
 To install Dot Scanner, open a terminal window and run the following command:
 
 ```
 pip install dotscanner
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ### Running the Software
 
 To launch the main graphical user interface (GUI), run the following command:
 
 ```
 dotscanner
 ```
 
-Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works.
 
 ## The Configurations Window
+
 The first window displayed in the GUI is the Configurations Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
 
 If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
 
 If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
 
-The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
+The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed.
+
+If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. _(Note that trying to run a lifetime program on a single image will not be allowed by the software.)_ This selection is made through the **Program** dropdown menu:
 
-If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
 
 If **Lifetime** is selected, some additional options will appear:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
 
 ### Descriptions of Configuration Options
 
 #### Save figures
+
 Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
 
 #### Blob size
-This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
+
+This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots” (the dimmer particles of interest in the image) are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
 
 #### Dot size
+
 Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
 
 #### Thresholds
+
 There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
+
 1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
+
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
+
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
+
+1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
+2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
-This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
+
+This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images _must be numbered sequentially_).
 
 #### Skips allowed
+
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
-      
+
 #### Remove edge frames
+
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
+
 Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
+
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
 #### Contrast
+
 These buttons adjust the contrast of the image.
 
 #### Dots
+
 These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
 
 #### Blobs
-These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
+
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. _Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well._
 
 #### Edit
+
 This button changes the left button bar view to display some manual threshold and size adjustment options:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
 
-*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+_(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the_ **Done** _button, or pressing the_ **return** _key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)_
 
 #### Reset
+
 This button resets the adjusted thresholds back to the default values.
 
 #### Skip
+
 This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
 
 ## The Region Selector Window
+
 Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
 
-This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
+This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. _(In other words, it is not necessary to re-click the first vertex created to close the polygon.)_
 
 Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data._
 
 ## Authors
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.5
-     * Bug fixes
-* 1.3.0
-     * Added option to re-analyze data without redrawing regions
-     * Added particle displacement tracking during lifetime measurement
-     * Added histogram output for lifetimes measurements
-* 1.2.0
-     * Added options for editing the configuration file
-     * Added startup processes to check the configuration file for errors
-* 1.1.0
-     * Migrated the remaining portions of the app from a terminal interface to a GUI
-* 1.0.0
-     * Initial Release
+- 1.4.0
+  - Added option to re-analyze data on different images using previous analysis settings
+- 1.3.0
+  - Added option to re-analyze data on the same image without redrawing regions
+  - Added particle displacement tracking during lifetime measurement
+  - Added histogram output for lifetimes measurements
+- 1.2.0
+  - Added options for editing the configuration file
+  - Added startup processes to check the configuration file for errors
+- 1.1.0
+  - Migrated the remaining portions of the app from a terminal interface to a GUI
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
 
 ## Development
 
 To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
 
 ```
 python -m dotscanner
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Testing
 
 Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
 
 ## Citations
```

### Comparing `dotscanner-1.3.5/README.md` & `dotscanner-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,178 +1,209 @@
 # Dot Scanner
+
 > Software designed for analysis of microscope imaging data
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
-Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
+Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is _especially_ useful for noisy image data, where manual "by-eye" analysis is unreliable.
 
 ## Getting Started
 
 ### Dependencies
 
-[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
+[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed.
 
 ### Installation
 
 To install Dot Scanner, open a terminal window and run the following command:
 
 ```
 pip install dotscanner
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ### Running the Software
 
 To launch the main graphical user interface (GUI), run the following command:
 
 ```
 dotscanner
 ```
 
-Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works.
 
 ## The Configurations Window
+
 The first window displayed in the GUI is the Configurations Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
 
 If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
 
 If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
 
-The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
+The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed.
+
+If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. _(Note that trying to run a lifetime program on a single image will not be allowed by the software.)_ This selection is made through the **Program** dropdown menu:
 
-If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
 
 If **Lifetime** is selected, some additional options will appear:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
 
 ### Descriptions of Configuration Options
 
 #### Save figures
+
 Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
 
 #### Blob size
-This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
+
+This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots” (the dimmer particles of interest in the image) are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
 
 #### Dot size
+
 Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
 
 #### Thresholds
+
 There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
+
 1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
+
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
+
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
+
+1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
+2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
-This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
+
+This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images _must be numbered sequentially_).
 
 #### Skips allowed
+
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
-      
+
 #### Remove edge frames
+
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
+
 Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
+
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
 #### Contrast
+
 These buttons adjust the contrast of the image.
 
 #### Dots
+
 These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
 
 #### Blobs
-These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
+
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. _Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well._
 
 #### Edit
+
 This button changes the left button bar view to display some manual threshold and size adjustment options:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
 
-*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+_(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the_ **Done** _button, or pressing the_ **return** _key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)_
 
 #### Reset
+
 This button resets the adjusted thresholds back to the default values.
 
 #### Skip
+
 This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
 
 ## The Region Selector Window
+
 Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
 
-This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
+This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. _(In other words, it is not necessary to re-click the first vertex created to close the polygon.)_
 
 Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data._
 
 ## Authors
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.5
-     * Bug fixes
-* 1.3.0
-     * Added option to re-analyze data without redrawing regions
-     * Added particle displacement tracking during lifetime measurement
-     * Added histogram output for lifetimes measurements
-* 1.2.0
-     * Added options for editing the configuration file
-     * Added startup processes to check the configuration file for errors
-* 1.1.0
-     * Migrated the remaining portions of the app from a terminal interface to a GUI
-* 1.0.0
-     * Initial Release
+- 1.4.0
+  - Added option to re-analyze data on different images using previous analysis settings
+- 1.3.0
+  - Added option to re-analyze data on the same image without redrawing regions
+  - Added particle displacement tracking during lifetime measurement
+  - Added histogram output for lifetimes measurements
+- 1.2.0
+  - Added options for editing the configuration file
+  - Added startup processes to check the configuration file for errors
+- 1.1.0
+  - Migrated the remaining portions of the app from a terminal interface to a GUI
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
 
 ## Development
 
 To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
 
 ```
 python -m dotscanner
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Testing
 
 Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
 
 ## Citations
```

### Comparing `dotscanner-1.3.5/dotscanner/__main__.py` & `dotscanner-1.4.0/src/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,86 @@
+import settings.config as cfg
 import settings.configmanagement as cm
+from src.ui.UserSettings import UserSettings
+from src.ui.ThresholdAdjuster import ThresholdAdjuster
+from src.ui.RegionSelector import RegionSelector
+from src.ui.MicroscopeImage import MicroscopeImage
+from src.strings import ProgramType
+import src.strings as strings
+import src.lifetime as lifetime
+import src.files as files
+import src.density as density
 
 cm.runChecks()
 
-import dotscanner.density as density
-import dotscanner.files as files
-import dotscanner.lifetime as lifetime
-import dotscanner.strings as strings
-from dotscanner.strings import ProgramType
-from dotscanner.ui.MicroscopeImage import MicroscopeImage
-from dotscanner.ui.RegionSelector import RegionSelector
-from dotscanner.ui.ThresholdAdjuster import ThresholdAdjuster
-from dotscanner.ui.UserSettings import UserSettings
-import settings.config as cfg
 
 def main():
-	while True:
-		userSettings = UserSettings()
-		directory, filenames = files.getDirectoryAndFilenames(userSettings)
-		if userSettings.program == ProgramType.DENSITY:
-			getDensityData(directory, filenames, userSettings)
-		elif userSettings.program == ProgramType.LIFETIME:
-			getLifetimeData(directory, filenames, userSettings)
-		else:
-			raise Exception(strings.programNameException)
-	
+    while True:
+        userSettings = UserSettings()
+        directory, filenames = files.getDirectoryAndFilenames(userSettings)
+        if userSettings.program == ProgramType.DENSITY:
+            getDensityData(directory, filenames, userSettings)
+        elif userSettings.program == ProgramType.LIFETIME:
+            getLifetimeData(directory, filenames, userSettings)
+        else:
+            raise Exception(strings.programNameException)
+
+
 def getDensityData(directory, filenames, userSettings):
-	if userSettings.reanalysis:
-		density.reanalyzeDensityData(directory, userSettings)
-		return
-	
-	density.checkUnitsConsistent(directory)
-	alreadyMeasured = density.getAlreadyMeasured(directory)
-	targetPath = files.getAnalysisTargetPath(directory, cfg.DENSITY_OUTPUT_FILENAME)
-	for filename in filenames:
-		if filename in alreadyMeasured:
-			print(strings.alreadyMeasuredNotification(filename))
-			continue
-		
-		print(f"\n----------\nDisplaying {filename}\n----------")
-		microscopeImage = MicroscopeImage(directory, filename, userSettings)
-		
-		thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
-		userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
-		if microscopeImage.skipped:
-			density.skipFile(directory, filename, targetPath, userSettings, microscopeImage)
-			continue
-		
-		RegionSelector(microscopeImage, userSettings)
-		if microscopeImage.skipped:
-			density.skipFile(directory, filename, targetPath, userSettings, microscopeImage)
-			continue
-		
-		density.measureDensity(directory, filename, targetPath, microscopeImage, userSettings)
+    if userSettings.reanalysis:
+        if len(filenames) == 1:
+            density.reanalyzeSingleDensityFile(
+                directory, filenames[0], userSettings
+            )
+        else:
+            density.reanalyzeDensityData(directory, userSettings)
+        return
+
+    density.checkUnitsConsistent(directory)
+    alreadyMeasured = density.getAlreadyMeasured(directory)
+    targetPath = files.getAnalysisTargetPath(
+        directory, cfg.DENSITY_OUTPUT_FILENAME)
+    for filename in filenames:
+        if filename in alreadyMeasured:
+            print(strings.alreadyMeasuredNotification(filename))
+            continue
+
+        print(f"\n----------\nDisplaying {filename}\n----------")
+        microscopeImage = MicroscopeImage(directory, filename, userSettings)
+
+        thresholdAdjuster = ThresholdAdjuster(microscopeImage, userSettings)
+        # Updating with the threshold adjustments
+        userSettings = thresholdAdjuster.userSettings
+        if microscopeImage.skipped:
+            density.skipFile(directory, filename, targetPath,
+                             userSettings, microscopeImage)
+            continue
+
+        RegionSelector(microscopeImage, userSettings)
+        if microscopeImage.skipped:
+            density.skipFile(directory, filename, targetPath,
+                             userSettings, microscopeImage)
+            continue
+
+        density.measureDensity(directory, filename,
+                               targetPath, microscopeImage, userSettings)
+
 
 def getLifetimeData(directory, filenames, userSettings):
-	lifetime.checkEnoughFramesForLifetimes(filenames, userSettings)
-	
-	middleIndex = len(filenames) // 2
-	middleMicroscopeImage = MicroscopeImage(directory, filenames[middleIndex], userSettings)
-	
-	thresholdAdjuster = ThresholdAdjuster(middleMicroscopeImage, userSettings, skipButton=False)
-	userSettings = thresholdAdjuster.userSettings # Updating with the threshold adjustments
-	RegionSelector(middleMicroscopeImage, userSettings, skipButton=False)
-	
-	lifetime.measureLifetime(directory, filenames, middleMicroscopeImage, userSettings)
+    lifetime.checkEnoughFramesForLifetimes(filenames, userSettings)
+
+    middleIndex = len(filenames) // 2
+    middleMicroscopeImage = MicroscopeImage(
+        directory, filenames[middleIndex], userSettings)
+
+    thresholdAdjuster = ThresholdAdjuster(
+        middleMicroscopeImage, userSettings, skipButton=False)
+    # Updating with the threshold adjustments
+    userSettings = thresholdAdjuster.userSettings
+    RegionSelector(middleMicroscopeImage, userSettings, skipButton=False)
+
+    lifetime.measureLifetime(directory, filenames,
+                             middleMicroscopeImage, userSettings)
+
 
 if __name__ == '__main__':
-	main()
+    main()
```

### Comparing `dotscanner-1.3.5/dotscanner.egg-info/PKG-INFO` & `dotscanner-1.4.0/dotscanner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotscanner
-Version: 1.3.5
+Version: 1.4.0
 Summary: A program designed for analysis of microscope imaging data
 Home-page: https://github.com/bdavis222/dotscanner
 Author: Holly Allen and Brian Davis
 Author-email: holly.allen@colorado.edu
 Project-URL: Bug Reports, https://github.com/bdavis222/dotscanner/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/dotscanner
@@ -15,184 +15,215 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dot Scanner
+
 > Software designed for analysis of microscope imaging data
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
-Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is *especially* useful for noisy image data, where manual "by-eye" analysis is unreliable.
+Dot Scanner is designed to simplify analysis of microscope imaging data. The program runs entirely within a window-based graphical user interface, so as to not require any programming knowledge from the user in order to complete their image analysis (see the images below for examples). This software is _especially_ useful for noisy image data, where manual "by-eye" analysis is unreliable.
 
 ## Getting Started
 
 ### Dependencies
 
-[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed. 
+[Python 3](https://www.python.org/downloads/) must be installed before Dot Scanner can be installed.
 
 ### Installation
 
 To install Dot Scanner, open a terminal window and run the following command:
 
 ```
 pip install dotscanner
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ### Running the Software
 
 To launch the main graphical user interface (GUI), run the following command:
 
 ```
 dotscanner
 ```
 
-Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works. 
+Some demo images are included in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) of this GitHub project, which can be downloaded and used as explained below to familiarize oneself with how the software works.
 
 ## The Configurations Window
+
 The first window displayed in the GUI is the Configurations Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/3.png)
 
 If the **File** or **Folder** buttons are clicked, another window opens, allowing the user to select a file or folder for analysis (the images in the [demo images folder](https://github.com/bdavis222/dotscanner/blob/main/images/demo/) can be downloaded to try this out for oneself):
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/4.png)
 
 If repeated analysis is being performed at the same target filepath, the user can avoid continuously repeating this step by setting a default filepath. This is done by clicking the "Edit defaults" button. An entire configurations file is editable for other defaults as well. Any of the variables in this configurations file can be modified to change the default behavior of the software.
 
-The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed. 
+The software will run as expected on any folder where the most common file extension within the folder belongs to the images wanting to be analyzed. By default, the entire folder will be scanned, and the most common file type found within the folder will be set as the file type to analyze. If the user is experiencing issues with the wrong file type being selected, it is recommended that they reorganize their data into folders containing only their images to be analyzed.
+
+If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. _(Note that trying to run a lifetime program on a single image will not be allowed by the software.)_ This selection is made through the **Program** dropdown menu:
 
-If a folder containing several images is selected, the user has the option to change the default program from **Density** to **Lifetime**. *(Note that trying to run a lifetime program on a single image will not be allowed by the software.)* This selection is made through the **Program** dropdown menu:
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/5.png)
 
 If **Lifetime** is selected, some additional options will appear:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/6.png)
 
 ### Descriptions of Configuration Options
 
 #### Save figures
+
 Selecting this option will output graphical plots to a `figures` folder that will be created within the folder containing the data being analyzed. These plots serve to allow the user to quickly verify their selections made during analysis.
 
 #### Blob size
-This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots”—the dimmer particles of interest in the image—are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
+
+This option sets the radius (or, more accurately, roughly the half width of a square) of exclusion around "blobs" (in pixels). Blobs are regions of the image that are saturated and overexposed. For example, if the blob size is set to 5, then a square region extending 5 pixels in each direction (left, right, up, and down) will be defined from each overexposed pixel (meaning the square will span 11 pixels on each side, including the central pixel), and all of the pixels within those regions will be ignored during analysis. This ensures that the “dots” (the dimmer particles of interest in the image) are not too close to any of these regions, and thus the outer edges of blobs are not confused as dots.
 
 #### Dot size
+
 Similar to the blob size option, this sets the size of a "dot" in the dataset. Because dots should not overlap, the larger the dot size, the fewer dots will be detected, as dimmer pixels within a brighter dot's region will not be recognized as dots, and will therefore be removed.
 
 #### Thresholds
+
 There are three thresholds that can be set to adjust the detection sensitivity for "dots" and "blobs" in a given image. The three editable text boxes correspond to the following variables (displayed from left to right in the Configurations Window):
+
 1. `LOWER_DOT_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the dots. The default is 1.5, which corresponds to 1.5 standard deviations above the mean of the data. Lower this value to increase the number of faint dots detected, or raise it to reduce the number.
 2. `UPPER_DOT_THRESH_SCALE`: Scaling for the upper threshold defining the brightness of the dots. The default is 5, which corresponds to 5 standard deviations above the mean. Lower this value to reduce the number of bright dots detected, or raise it to increase the number.
 3. `LOWER_BLOB_THRESH_SCALE`: Scaling for the lower threshold defining the brightness of the blobs. The default is 2, which corresponds to 2 times the value of `UPPER_DOT_THRESH_SCALE`. Lower this value to increase the number of blobs detected, or raise it to reduce the number.
 
 #### Edit defaults
+
 This opens a new window that allows the user to edit the default filepath or edit/reset the entire configuration file directly.
 
 #### Use previous analysis
-This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat the analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file.
+
+This opens a new window that allows the user to browse for a previous .txt analysis file to use to repeat analysis. Information on which settings are reused during re-analysis is included in the header of each analysis file. There are two main scenarios for using this feature:
+
+1. **Re-analyzing the same image or set of images.** _This is useful if the user wants to tweak one or two parameters of an analysis without running through the entire folder of images one by one again._
+2. **Analyzing a new image or set of images with the same analysis settings as a previous analysis.** _This is useful if the user has already run analysis on a set of green images and wants to run the exact same analysis on their red counterparts, for example._
 
 Clicking **Next**, or pressing the **return** key on the keyboard, will save the user’s selections and open the Threshold Adjustment Window.
 
 ### Descriptions of Configuration Options for the Lifetime Program
 
 #### Start image
-This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images *must be numbered sequentially*).
+
+This option sets the first image to be considered in a lifetime calculation. The default is the first image in the folder (as the images _must be numbered sequentially_).
 
 #### Skips allowed
+
 This sets the number of consecutive images that are allowed to be skipped in a lifetime calculation. This can be useful for dimmer dots where an image or two in a series are relatively out of focus, resulting in an unwanted non-detection for those frames. By increasing the number of skips allowed, these particles will be retained as long as they are back in focus and bright enough for detection in subsequent frames.
-      
+
 #### Remove edge frames
+
 This dictates whether edge frames should be removed from a lifetime calculation. If a particle is detected in the first frame of an image, for example, it cannot be determined whether the particle existed before the first image was taken, so it might not make sense to include this in a lifetime calculation (and the same may also be true for particles in the last frame). If the number of skips allowed in the lifetime calculation is greater than zero, this will increase how many edge frames are removed from analysis.
 
 ## The Threshold Adjustment Window
+
 Clicking the **Next** button, or pressing the **return** key on the keyboard, from the Configurations Window saves the configuration settings selected by the user and advances to the Threshold Adjustment Window. This window shows the image data with the dots and blobs identified, and features several button groups on the left sidebar:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/7.png)
 
 From top to bottom, these button groups perform the following actions:
 
 #### View
+
 These buttons allow four different viewing options: zooming in on the top left, top right, bottom left, bottom right, or zooming back out to show the full image. The user can also press the **spacebar** on the keyboard to cycle through these different views.
 
 #### Contrast
+
 These buttons adjust the contrast of the image.
 
 #### Dots
+
 These buttons adjust the sensitivity for detecting “dots” in the image (the fainter, smaller dots, as opposed to the much brighter and larger “blobs”). The user can also press the **up** and **down** arrow keys on the keyboard to make these adjustments.
 
 #### Blobs
-These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. *Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well.*
+
+These buttons adjust the sensitivity for detecting “blobs” in the image. The user can also press the **right** and **left** arrow keys on the keyboard to make these adjustments. _Note: since increasing the blob sensitivity changes the threshold between blobs and dots, this results in a different number of dots being detected as well._
 
 #### Edit
+
 This button changes the left button bar view to display some manual threshold and size adjustment options:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/8.png)
 
-*(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the* **Done** *button, or pressing the* **return** *key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)*
+_(Once the thresholds or sizes are changed by entering new numbers into the text boxes, clicking the_ **Done** _button, or pressing the_ **return** _key on the keyboard, saves the settings and returns the left button bar to the original button configuration.)_
 
 #### Reset
+
 This button resets the adjusted thresholds back to the default values.
 
 #### Skip
+
 This button skips the current image (for example, if the user decides the data quality is not sufficient for measurement). The **escape** key on the keyboard can also be pressed to perform a skip.
 
 ## The Region Selector Window
+
 Clicking the **Done** button, or pressing the **return** key on the keyboard, from the main Threshold Adjustment Window saves the threshold settings selected by the user and advances to the Region Selector Window:
+
 ![](https://github.com/bdavis222/dotscanner/blob/main/images/9.png)
 
-This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. *(In other words, it is not necessary to re-click the first vertex created to close the polygon.)*
+This window allows the user to click different locations on the image to set the vertices of a polygon within which the measurements will be made. At any point, the polygon can be reset by clicking the **Reset** button, or by pressing the **backspace** key on the keyboard. It is important to note that after at least three vertices have been placed, the dotted line shows how the program will enclose the polygon once the **Done** button, or the **return** key on the keyboard, is pressed. _(In other words, it is not necessary to re-click the first vertex created to close the polygon.)_
 
 Information about the image processing will be displayed in the terminal, including progress bars to estimate the time to completion of longer processes, like lifetime calculations and the saving of multiple figures.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your data._
 
 ## Authors
 
 Holly Allen (holly.allen@colorado.edu)
 
 Brian Davis
 
 ## Release History
 
-* 1.3.5
-     * Bug fixes
-* 1.3.0
-     * Added option to re-analyze data without redrawing regions
-     * Added particle displacement tracking during lifetime measurement
-     * Added histogram output for lifetimes measurements
-* 1.2.0
-     * Added options for editing the configuration file
-     * Added startup processes to check the configuration file for errors
-* 1.1.0
-     * Migrated the remaining portions of the app from a terminal interface to a GUI
-* 1.0.0
-     * Initial Release
+- 1.4.0
+  - Added option to re-analyze data on different images using previous analysis settings
+- 1.3.0
+  - Added option to re-analyze data on the same image without redrawing regions
+  - Added particle displacement tracking during lifetime measurement
+  - Added histogram output for lifetimes measurements
+- 1.2.0
+  - Added options for editing the configuration file
+  - Added startup processes to check the configuration file for errors
+- 1.1.0
+  - Migrated the remaining portions of the app from a terminal interface to a GUI
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/dotscanner/blob/main/LICENSE) file for details.
 
 ## Development
 
 To contribute, download or clone the project. From the top level of the project's folder structure, one can use the following command to run a local version of the software (e.g., for UI testing):
 
 ```
 python -m dotscanner
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Testing
 
 Unit tests for this software were written for use with [Python's built-in unittest framework](https://docs.python.org/3/library/unittest.html), and are stored in the `tests` folder. To run tests, download the project, navigate to the top level of the project's folder structure and run the following command:
 
 ```
 python -m unittest
 ```
 
-*(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
+_(Note that the_ `python3` _command may be required instead of_ `python` _for some Python installations.)_
 
 ### Bug Reports and Feature Requests
 
 To report a bug, visit the [issues page](https://github.com/bdavis222/dotscanner/issues). New feature requests are also welcome!
 
 ## Citations
```

### Comparing `dotscanner-1.3.5/settings/config.py` & `dotscanner-1.4.0/settings/config.py`

 * *Files identical despite different names*

### Comparing `dotscanner-1.3.5/setup.py` & `dotscanner-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='dotscanner',
-    version='1.3.5', # Required 
+    version='1.4.0', # Required 
     description='A program designed for analysis of microscope imaging data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/dotscanner',
     author='Holly Allen and Brian Davis',
     author_email='holly.allen@colorado.edu',
     classifiers=[
@@ -20,21 +20,21 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: Unix',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows'
     ],
     packages=find_packages(),
-    py_modules=['dotscanner', 'dotscanner.ui', 'settings', 'tests', 'tests.ui'],
+    py_modules=['src', 'src.ui', 'settings', 'tests', 'tests.ui'],
     python_requires='>=3.7, <4',
     install_requires=['matplotlib', 'numpy'],
     project_urls={
         'Bug Reports': 'https://github.com/bdavis222/dotscanner/issues',
         'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
         'Source': 'https://github.com/bdavis222/dotscanner',
     },
     entry_points={
         'console_scripts': [
-            'dotscanner = dotscanner.__main__:main'
+            'dotscanner = src.__main__:main'
         ]
     }
 )
```

### Comparing `dotscanner-1.3.5/tests/test_files.py` & `dotscanner-1.4.0/tests/test_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,308 +1,342 @@
-import dotscanner.files as files
-import dotscanner.strings as strings
-from dotscanner.strings import ProgramType
-from tests.ui.FakeUserSettings import FakeUserSettings
 import mock
 import unittest
 
+import src.files as files
+import src.strings as strings
+from src.strings import ProgramType
+from tests.ui.FakeUserSettings import FakeUserSettings
+
+
 class TestFiles(unittest.TestCase):
     def getTestFilenames(self):
-        return ["file03.png", "file02.png", "file01.png", "file05.PNG", "file04.png", "file11.png", 
-        "readme.md", "test", "directory2/"]
-    
+        return ["file03.png", "file02.png", "file01.png", "file05.PNG", "file04.png", "file11.png",
+                "readme.md", "test", "directory2/"]
+
     def test_fixDirectory(self):
         string = "test"
-        
+
         self.assertEqual(files.fixDirectory(string), "test/")
-        
+
         string2 = "testString/"
-        
+
         self.assertEqual(files.fixDirectory(string2), "testString/")
-    
+
     def test_getRightEdgeOfTrailingNumber(self):
-        self.assertEqual(files.getRightEdgeOfTrailingNumber("test123.fil35e"), 6)
-        self.assertEqual(files.getRightEdgeOfTrailingNumber("test123gjw.file"), 6)
-        self.assertEqual(files.getRightEdgeOfTrailingNumber("test123lj010.file"), 11)
+        self.assertEqual(
+            files.getRightEdgeOfTrailingNumber("test123.fil35e"), 6)
+        self.assertEqual(
+            files.getRightEdgeOfTrailingNumber("test123gjw.file"), 6)
+        self.assertEqual(files.getRightEdgeOfTrailingNumber(
+            "test123lj010.file"), 11)
         self.assertEqual(files.getRightEdgeOfTrailingNumber("6.file"), 0)
         self.assertEqual(files.getRightEdgeOfTrailingNumber("010.file"), 2)
-    
+
     def test_getLeftEdgeOfTrailingNumber(self):
-        self.assertEqual(files.getLeftEdgeOfTrailingNumber("test123.fil35e", 6), 4)
-        self.assertEqual(files.getLeftEdgeOfTrailingNumber("test123gjw.file", 6), 4)
-        self.assertEqual(files.getLeftEdgeOfTrailingNumber("test123lj010.file", 11), 9)
+        self.assertEqual(files.getLeftEdgeOfTrailingNumber(
+            "test123.fil35e", 6), 4)
+        self.assertEqual(files.getLeftEdgeOfTrailingNumber(
+            "test123gjw.file", 6), 4)
+        self.assertEqual(files.getLeftEdgeOfTrailingNumber(
+            "test123lj010.file", 11), 9)
         self.assertEqual(files.getLeftEdgeOfTrailingNumber("6.file", 0), 0)
         self.assertEqual(files.getLeftEdgeOfTrailingNumber("010.file", 2), 0)
-    
+
     def test_getTrailingNumber(self):
         self.assertEqual(files.getTrailingNumber("test123.fil35e"), 123)
         self.assertEqual(files.getTrailingNumber("test123gjw.file"), 123)
         self.assertEqual(files.getTrailingNumber("test123lj010.file"), 10)
         self.assertEqual(files.getTrailingNumber("6.file"), 6)
         self.assertEqual(files.getTrailingNumber("010.file"), 10)
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getMostCommonFileExtension(self, mock_listdir):
         mock_listdir.return_value = self.getTestFilenames()
-        
+
         extension = files.getMostCommonFileExtension("test/directory/")
-        
+
         self.assertEqual(extension, ".png")
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getFilenamesWithExtension(self, mock_listdir):
         mock_listdir.return_value = self.getTestFilenames()
-        
-        unsortedFilenames = files.getFilenamesWithExtension("test/directory/", ".png")
-        
+
+        unsortedFilenames = files.getFilenamesWithExtension(
+            "test/directory/", ".png", testing=True)
+
         self.assertIn("file03.png", unsortedFilenames)
         self.assertIn("file02.png", unsortedFilenames)
         self.assertIn("file01.png", unsortedFilenames)
         self.assertIn("file05.PNG", unsortedFilenames)
         self.assertIn("file04.png", unsortedFilenames)
         self.assertIn("file11.png", unsortedFilenames)
         self.assertNotIn("readme.md", unsortedFilenames)
         self.assertNotIn("test", unsortedFilenames)
         self.assertNotIn("directory2/", unsortedFilenames)
-        
-        unsortedFilenames2 = files.getFilenamesWithExtension("test/directory/", ".md")
-        
+
+        unsortedFilenames2 = files.getFilenamesWithExtension(
+            "test/directory/", ".md", testing=True)
+
         self.assertIn("readme.md", unsortedFilenames2)
         self.assertNotIn("file02.png", unsortedFilenames2)
         self.assertNotIn("file01.png", unsortedFilenames2)
         self.assertNotIn("file05.PNG", unsortedFilenames2)
         self.assertNotIn("file04.png", unsortedFilenames2)
         self.assertNotIn("file11.png", unsortedFilenames2)
         self.assertNotIn("file03.png", unsortedFilenames2)
         self.assertNotIn("test", unsortedFilenames2)
         self.assertNotIn("directory2/", unsortedFilenames2)
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getSortedFilenames_withDensityProgramNumbered(self, mock_listdir):
         mock_listdir.return_value = self.getTestFilenames()
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="file01.png", 
-            programSelected="density")
-        
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="file01.png", programSelected="density", testing=True)
+
         self.assertEqual(
-            sortedFilenames, 
-            ["file01.png", "file02.png", "file03.png", "file04.png", "file05.PNG", "file11.png"]
+            sortedFilenames,
+            ["file01.png", "file02.png", "file03.png",
+                "file04.png", "file05.PNG", "file11.png"]
         )
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="file04.png", 
-            programSelected="density")
-        
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="file04.png", programSelected="density", testing=True)
+
         # The value of startImage should be ignored for a density program
         self.assertEqual(
-            sortedFilenames, 
-            ["file01.png", "file02.png", "file03.png", "file04.png", "file05.PNG", "file11.png"]
+            sortedFilenames,
+            ["file01.png", "file02.png", "file03.png",
+                "file04.png", "file05.PNG", "file11.png"]
         )
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getSortedFilenames_withDensityProgramUnnumbered(self, mock_listdir):
-        mock_listdir.return_value = ["filec.png", "fileb.png", "filea.png", "filef.png", 
-        "filee.PNG", "filed.png"]
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="filec.png", 
-            programSelected="density")
-        
+        mock_listdir.return_value = ["filec.png", "fileb.png", "filea.png", "filef.png",
+                                     "filee.PNG", "filed.png"]
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="filec.png", programSelected="density", testing=True)
+
         # The value of startImage should be ignored for a density program
         self.assertEqual(
-            sortedFilenames, 
-            ["filea.png", "fileb.png", "filec.png", "filed.png", "filee.PNG", "filef.png"]
+            sortedFilenames,
+            ["filea.png", "fileb.png", "filec.png",
+                "filed.png", "filee.PNG", "filef.png"]
         )
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getSortedFilenames_withDensityProgramUnnumberedNoStartImage(self, mock_listdir):
-        mock_listdir.return_value = ["filec.png", "fileb.png", "filea.png", "filef.png", 
-        "filee.PNG", "filed.png"]
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="", 
-            programSelected="density")
-        
+        mock_listdir.return_value = ["filec.png", "fileb.png", "filea.png", "filef.png",
+                                     "filee.PNG", "filed.png"]
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="", programSelected="density", testing=True)
+
         # The value of startImage should be ignored for a density program
         self.assertEqual(
-            sortedFilenames, 
-            ["filea.png", "fileb.png", "filec.png", "filed.png", "filee.PNG", "filef.png"]
+            sortedFilenames,
+            ["filea.png", "fileb.png", "filec.png",
+                "filed.png", "filee.PNG", "filef.png"]
         )
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_getSortedFilenames_withLifetimeProgram(self, mock_listdir):
         mock_listdir.return_value = self.getTestFilenames()
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="file01.png", 
-            programSelected="lifetime")
-        
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="file01.png", programSelected="lifetime", testing=True)
+
         self.assertEqual(
-            sortedFilenames, 
-            ["file01.png", "file02.png", "file03.png", "file04.png", "file05.PNG", "file11.png"]
+            sortedFilenames,
+            ["file01.png", "file02.png", "file03.png",
+                "file04.png", "file05.PNG", "file11.png"]
         )
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="file04.png", 
-            programSelected=ProgramType.LIFETIME)
-        
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="file04.png", programSelected=ProgramType.LIFETIME,
+            testing=True)
+
         self.assertEqual(
-            sortedFilenames, 
+            sortedFilenames,
             ["file04.png", "file05.PNG", "file11.png"]
         )
-        
-        sortedFilenames = files.getSortedFilenames("test/directory/", startImage="", 
-            programSelected="lifetime")
-        
+
+        sortedFilenames = files.getSortedFilenames(
+            "test/directory/", startImage="", programSelected="lifetime", testing=True)
+
         self.assertEqual(
-            sortedFilenames, 
-            ["file01.png", "file02.png", "file03.png", "file04.png", "file05.PNG", "file11.png"]
+            sortedFilenames,
+            ["file01.png", "file02.png", "file03.png",
+                "file04.png", "file05.PNG", "file11.png"]
         )
-    
-    @mock.patch("dotscanner.files.os.path.basename")
-    @mock.patch("dotscanner.files.os.path.dirname")
-    @mock.patch("dotscanner.files.os.path.isfile")
+
+    @mock.patch("src.files.os.path.basename")
+    @mock.patch("src.files.os.path.dirname")
+    @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forFile(self, mock_isfile, mock_dirname, mock_basename):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = True
         mock_dirname.return_value = "test/directory/"
         mock_basename.return_value = "testFile.png"
-        
-        directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+
+        directory, filenames = files.getDirectoryAndFilenames(
+            fakeUserSettings, testing=True)
+
         self.assertEqual(directory, "test/directory/")
         self.assertEqual(filenames, ["testFile.png"])
-    
-    @mock.patch("dotscanner.files.os.listdir")
-    @mock.patch("dotscanner.files.os.path.isdir")
-    @mock.patch("dotscanner.files.os.path.isfile")
+
+    @mock.patch("src.files.os.listdir")
+    @mock.patch("src.files.os.path.isdir")
+    @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forDirectory(self, mock_isfile, mock_isdir, mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = False
         mock_isdir.return_value = True
         mock_listdir.return_value = self.getTestFilenames()
-        
-        directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+
+        directory, filenames = files.getDirectoryAndFilenames(
+            fakeUserSettings, testing=True)
+
         self.assertEqual(directory, fakeUserSettings.filepath)
         self.assertEqual(
-            filenames, 
-            ["file01.png", "file02.png", "file03.png", "file04.png", "file05.PNG", "file11.png"]
+            filenames,
+            ["file01.png", "file02.png", "file03.png",
+                "file04.png", "file05.PNG", "file11.png"]
         )
-    
-    @mock.patch("dotscanner.files.os.listdir")
-    @mock.patch("dotscanner.files.os.path.isdir")
-    @mock.patch("dotscanner.files.os.path.isfile")
+
+    @mock.patch("src.files.os.listdir")
+    @mock.patch("src.files.os.path.isdir")
+    @mock.patch("src.files.os.path.isfile")
     def test_getDirectoryAndFilenames_forEmptyDirectory(self, mock_isfile, mock_isdir, mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = False
         mock_isdir.return_value = True
         mock_listdir.return_value = []
-        
+
         with self.assertRaises(Exception) as context:
-            directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+            directory, filenames = files.getDirectoryAndFilenames(
+                fakeUserSettings, testing=True)
+
         self.assertTrue(strings.noFilesException in str(context.exception))
-    
-    @mock.patch("dotscanner.files.os.listdir")
-    @mock.patch("dotscanner.files.os.path.isdir")
-    @mock.patch("dotscanner.files.os.path.isfile")
-    def test_getDirectoryAndFilenames_forNeitherFileNorDirectory(self, mock_isfile, mock_isdir, 
-        mock_listdir):
+
+    @mock.patch("src.files.os.listdir")
+    @mock.patch("src.files.os.path.isdir")
+    @mock.patch("src.files.os.path.isfile")
+    def test_getDirectoryAndFilenames_forNeitherFileNorDirectory(self, mock_isfile, mock_isdir,
+                                                                 mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = False
         mock_isdir.return_value = False
         mock_listdir.return_value = []
-        
+
         with self.assertRaises(Exception) as context:
-            directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+            directory, filenames = files.getDirectoryAndFilenames(
+                fakeUserSettings, testing=True)
+
         self.assertTrue(strings.filepathException in str(context.exception))
-    
-    @mock.patch("dotscanner.files.os.listdir")
-    @mock.patch("dotscanner.files.os.path.isdir")
-    @mock.patch("dotscanner.files.os.path.isfile")
-    def test_getDirectoryAndFilenames_forFilesWithoutExtensions(self, mock_isfile, mock_isdir, 
-        mock_listdir):
+
+    @mock.patch("src.files.os.listdir")
+    @mock.patch("src.files.os.path.isdir")
+    @mock.patch("src.files.os.path.isfile")
+    def test_getDirectoryAndFilenames_forFilesWithoutExtensions(self, mock_isfile, mock_isdir,
+                                                                mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = False
         mock_isdir.return_value = True
         mock_listdir.return_value = ["file", "file2"]
-        
+
         with self.assertRaises(Exception) as context:
-            directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+            directory, filenames = files.getDirectoryAndFilenames(
+                fakeUserSettings, testing=True)
+
         self.assertTrue(strings.noFilesException in str(context.exception))
-    
-    @mock.patch("dotscanner.files.os.listdir")
-    @mock.patch("dotscanner.files.os.path.isdir")
-    @mock.patch("dotscanner.files.os.path.isfile")
-    def test_getDirectoryAndFilenames_forFilesWithoutNumbers(self, mock_isfile, mock_isdir, 
-        mock_listdir):
+
+    @mock.patch("src.files.os.listdir")
+    @mock.patch("src.files.os.path.isdir")
+    @mock.patch("src.files.os.path.isfile")
+    def test_getDirectoryAndFilenames_forFilesWithoutNumbers(self, mock_isfile, mock_isdir,
+                                                             mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_isfile.return_value = False
         mock_isdir.return_value = True
         mock_listdir.return_value = ["filec.png", "filez.png", "filea.png"]
-        
-        directory, filenames = files.getDirectoryAndFilenames(fakeUserSettings)
-        
+
+        directory, filenames = files.getDirectoryAndFilenames(
+            fakeUserSettings, testing=True)
+
         self.assertEqual(filenames, ["filea.png", "filec.png", "filez.png"])
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_hasNoValidFiles_forEmptyDirectory(self, mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_listdir.return_value = []
-        
+
         self.assertTrue(files.hasNoValidFiles(fakeUserSettings))
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_hasNoValidFiles_forNoFileExtensions(self, mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_listdir.return_value = ["dir1", "other", "file75"]
-        
+
         self.assertTrue(files.hasNoValidFiles(fakeUserSettings))
-    
-    @mock.patch("dotscanner.files.os.listdir")
+
+    @mock.patch("src.files.os.listdir")
     def test_hasNoValidFiles_forSingleFileWithExtension(self, mock_listdir):
         fakeUserSettings = FakeUserSettings()
         mock_listdir.return_value = ["dir1", "other", "file75.png"]
-        
+
         self.assertFalse(files.hasNoValidFiles(fakeUserSettings))
-    
+
     def test_allFilesAreNumbered_withAllNumberedFiles(self):
-        testFiles = ["file03.png", "file02.png", "file05.PNG", "file04.png", "file11.png"]
+        testFiles = ["file03.png", "file02.png",
+                     "file05.PNG", "file04.png", "file11.png"]
         self.assertTrue(files.allFilesAreNumbered(testFiles))
-    
+
     def test_allFilesAreNumbered_withOneUnnumberedFile(self):
-        testFiles = ["file03.png", "file02.png", "file05.PNG", "file.png", "file11.png"]
+        testFiles = ["file03.png", "file02.png",
+                     "file05.PNG", "file.png", "file11.png"]
         self.assertFalse(files.allFilesAreNumbered(testFiles))
-    
+
     def test_filenameIsNumbered(self):
         self.assertFalse(files.filenameIsNumbered("filename.txt"))
         self.assertTrue(files.filenameIsNumbered("filename1.txt"))
-    
+
     def test_getFilenameWithNewTrailingNumber(self):
-        newFilename = files.getFilenameWithNewTrailingNumber("filename1.txt", 65)
-        newFilename2 = files.getFilenameWithNewTrailingNumber("filename87.txt", 3)
-        
+        newFilename = files.getFilenameWithNewTrailingNumber(
+            "filename1.txt", 65)
+        newFilename2 = files.getFilenameWithNewTrailingNumber(
+            "filename87.txt", 3)
+
         self.assertEqual(newFilename, "filename65.txt")
         self.assertEqual(newFilename2, "filename3.txt")
-    
+
     def test_incrementTargetPathName(self):
-        self.assertEqual(files.incrementTargetPathName("path/to/file2.txt"), "path/to/file3.txt")
-        self.assertEqual(files.incrementTargetPathName("path/to/file66.txt"), "path/to/file67.txt")
-    
+        self.assertEqual(files.incrementTargetPathName(
+            "path/to/file2.txt"), "path/to/file3.txt")
+        self.assertEqual(files.incrementTargetPathName(
+            "path/to/file66.txt"), "path/to/file67.txt")
+
     def test_getExtensionIndexFromDensityAnalysisFileLineArray(self):
         line1 = "SD-RFP-2.tif 290 20247 0.0143231 0.0008411 1.5 5.0 2.0 5 2 0.0 5.0 (168, 425), \
 (151, 392), (62, 148), (112, 109), (230, 379)"
         line2 = "SD 525-2.tif 195 11325 0.0172185 0.001233 1.5 5.0 2.0 5 2 0.0 5.0 (88, 198), \
 (128, 187), (154, 165), (224, 353), (184, 411)"
         line3 = "SD 525-2tif 210 13151 0.0159684 0.0011019 1.5 5.0 2.0 5 2 0.0 5.0 (125, 438), \
 (95, 213), (148, 192), (214, 368)"
         lineArray1 = line1.split()
         lineArray2 = line2.split()
         lineArray3 = line3.split()
-        extensionIndex1 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray1)
-        extensionIndex2 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray2)
-        extensionIndex3 = files.getExtensionIndexFromDensityAnalysisFileLineArray(lineArray3)
-        
+        extensionIndex1 = files.getExtensionIndexFromDensityAnalysisFileLineArray(
+            lineArray1)
+        extensionIndex2 = files.getExtensionIndexFromDensityAnalysisFileLineArray(
+            lineArray2)
+        extensionIndex3 = files.getExtensionIndexFromDensityAnalysisFileLineArray(
+            lineArray3)
+
         self.assertEqual(extensionIndex1, 0)
         self.assertEqual(extensionIndex2, 1)
         self.assertEqual(extensionIndex3, -1)
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dotscanner-1.3.5/tests/test_strings.py` & `dotscanner-1.4.0/tests/test_strings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,92 @@
-import dotscanner.strings as strings
+import mock
+import unittest
+
+import src.strings as strings
 import settings.config as cfg
 from tests.ui.FakeMicroscopeImage import FakeMicroscopeImage
 from tests.ui.FakeUserSettings import FakeUserSettings
-import mock
-import unittest
+
 
 class TestStrings(unittest.TestCase):
     @mock.patch("settings.config.DENSITY_OUTPUT_FILENAME", "density.txt")
     def test_alreadyMeasuredNotification(self):
         output = strings.alreadyMeasuredNotification(filename="test.png")
-        
+
         self.assertEqual(
-            output, 
+            output,
             f"\nFile test.png already measured in density.txt file. Skipping."
         )
-    
+
     def test_densityOutput(self):
         fakeUserSettings = FakeUserSettings(dotSize=2, blobSize=5)
         fakeMicroscopeImage = FakeMicroscopeImage(
-            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5,
             upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         output = strings.densityOutput(
-            filename="test.png", 
+            filename="test.png",
             dotTotal=6,
             surveyedArea=600,
             density=0.01,
             error=0.0001,
             microscopeImage=fakeMicroscopeImage,
             userSettings=fakeUserSettings
         )
-        
+
         self.assertEqual(
             output,
             "test.png 6 600 0.01 0.0001 1.5 5.0 2.0 5 2 0.0 5.0 (1, 1), (1, 10), (10, 10), (10, 1)\n"
         )
-    
+
     def test_fileSkippedNotification(self):
         output = strings.fileSkippedNotification("test.png")
-        
+
         self.assertEqual(output, "\nFile test.png skipped")
-    
+
     def test_invalidAnalysisFileWarning(self):
         self.assertEqual(
             strings.invalidAnalysisFileWarning("test_file.png"),
             f'\nInvalid analysis file selected: "test_file.png". A valid file has a .txt extension \
 and contains density or lifetime data.'
         )
-    
+
     def test_invalidFilenameInDensityAnalysisFile(self):
         self.assertEqual(
-            strings.invalidFilenameInDensityAnalysisFile(["file", "array", "example"]),
+            strings.invalidFilenameInDensityAnalysisFile(
+                ["file", "array", "example"]),
             f"Filename with valid extension not found in the following line in densities file:\n\
 file array example"
         )
-    
+
     def test_outputFileTopHeader(self):
         self.assertEqual(
             strings.outputFileTopHeader(strings.ProgramType.DENSITY),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for density measurement\n#"
         )
         self.assertEqual(
             strings.outputFileTopHeader(strings.ProgramType.LIFETIME),
             f"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n#"
         )
-    
+
     def test_lifetimeOutputFileHeader(self):
         fakeMicroscopeImage = FakeMicroscopeImage(
-            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5,
             upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         fakeUserSettings = FakeUserSettings(
-            dotSize=2, blobSize=5, skipsAllowed=1, lowerDotThresh=1.5, upperDotThresh=5.0, 
+            dotSize=2, blobSize=5, skipsAllowed=1, lowerDotThresh=1.5, upperDotThresh=5.0,
             lowerBlobThresh=2.0, removeEdgeFrames=True)
-        
-        output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
-        
+
+        output = strings.lifetimeOutputFileHeader(
+            fakeMicroscopeImage, fakeUserSettings)
+
         self.assertEqual(
             output,
-"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
+            "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
 #\n\
 # If this file is selected for re-analysis, the following settings will be read in and used unless \
 changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
 output file in this same directory.\n\
 #\n\
 # Polygon vertices (x, y): (1, 1), (1, 10), (10, 10), (10, 1)\n\
@@ -95,28 +99,29 @@
 in the main configuration window):\n\
 #\n\
 # Remove edge frames: True | Save figures: False | Skips allowed: 1\n\
 #\n\
 # The data columns are organized as follows:\n\
 # x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
         )
-    
+
     def test_lifetimeOutputFileHeaderWithStartImage(self):
         fakeMicroscopeImage = FakeMicroscopeImage(
-            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5, 
+            polygon=[[1, 1], [10, 1], [10, 10], [1, 10], [1, 1]], lowerDotThreshScale=1.5,
             upperDotThreshScale=5.0, lowerBlobThreshScale=2.0)
         fakeUserSettings = FakeUserSettings(
-            dotSize=2, blobSize=5, startImage="path/to/image.png", skipsAllowed=1, 
+            dotSize=2, blobSize=5, startImage="path/to/image.png", skipsAllowed=1,
             lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0, removeEdgeFrames=True)
-        
-        output = strings.lifetimeOutputFileHeader(fakeMicroscopeImage, fakeUserSettings)
-        
+
+        output = strings.lifetimeOutputFileHeader(
+            fakeMicroscopeImage, fakeUserSettings)
+
         self.assertEqual(
             output,
-"# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
+            "# Dot Scanner (https://github.com/bdavis222/dotscanner)\n\
 # Generated output file for lifetime measurement\n\
 #\n\
 # If this file is selected for re-analysis, the following settings will be read in and used unless \
 changed in the threshold adjustment window. The re-analyzed data will then be given in a new \
 output file in this same directory.\n\
 #\n\
 # Polygon vertices (x, y): (1, 1), (1, 10), (10, 10), (10, 1)\n\
@@ -131,9 +136,10 @@
 # Remove edge frames: True | Save figures: False | \
 Skips allowed: 1 | Start image: image.png\n\
 #\n\
 # The data columns are organized as follows:\n\
 # x | y | lifetime | starting image | displacement squared (sq px)\n#\n"
         )
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `dotscanner-1.3.5/tests/ui/FakeUserSettings.py` & `dotscanner-1.4.0/tests/ui/FakeUserSettings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class FakeUserSettings:
-    def __init__(self, filepath="test/directory/", dotSize=2, blobSize=5, saveFigures=False, 
-        startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0, upperContrast=5.0,
-        lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0, program="density", 
-        polygon=None, densityData={}, reanalysis=False):
+    def __init__(self, filepath="test/directory/", dotSize=2, blobSize=5, saveFigures=False,
+                 startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0,
+                 upperContrast=5.0, lowerDotThresh=1.5, upperDotThresh=5.0, lowerBlobThresh=2.0,
+                 program="density", polygon=None, densityData={}, reanalysis=False):
         self.filepath = filepath
         self.dotSize = dotSize
         self.blobSize = blobSize
         self.saveFigures = saveFigures
         self.startImage = startImage
         self.skipsAllowed = skipsAllowed
         self.removeEdgeFrames = removeEdgeFrames
```

### Comparing `dotscanner-1.3.5/tests/ui/test_ThresholdAdjuster.py` & `dotscanner-1.4.0/tests/ui/test_ThresholdAdjuster.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,189 +1,197 @@
-from dotscanner.ui.MicroscopeImage import MicroscopeImage
-from dotscanner.ui.ThresholdAdjuster import ThresholdAdjuster
-from tests.ui.FakeUserSettings import FakeUserSettings
 import mock
 import numpy as np
 import unittest
 from unittest.mock import MagicMock
 
+from src.ui.MicroscopeImage import MicroscopeImage
+from src.ui.ThresholdAdjuster import ThresholdAdjuster
+from tests.ui.FakeUserSettings import FakeUserSettings
+
+
 class TestThresholdAdjuster(unittest.TestCase):
-	@mock.patch("dotscanner.dataprocessing.getData")
-	def getMicroscopeImageAndUserSettings(self, mock_getData):
-		testData = np.array([
-			[ 2,  0,  0,  0,  0,  0, -2,  0,  0,  0,  0,  0,  0],
- 			[ 2,  2,  0,  0,  0,  1,  0, -1, -1,  0,  0,  0,  0],
- 			[ 0,  0,  0,  0,  0,  0,  0,  0, -2,  0,  2,  0,  0],
- 			[ 0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
- 			[-1,  0,  0,  0,  0,  0,  1,  0,  0,  0,  0,  0,  0],
- 			[ 0,  0,  0,  0,  0,  0,  5,  4,  0,  0,  0,  0,  0],
- 			[ 0,  0,  0,  0,  0,  0,  2,  0, -1,  0,  0,  0,  0],
- 			[ 0,  0,  0,  0,  0,  0,  0, -1, -1,  0,  0,  0,  0],
- 			[ 0,  7,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
- 			[ 0,  5,  9,  0,  0,  0,  0,  1,  0,  0,  0,  8,  0],
- 			[-1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
- 		])
-		mock_getData.return_value = testData
-		fakeUserSettings = FakeUserSettings(
-			filepath="test/directory/", dotSize=2, blobSize=3, saveFigures=False, 
-			startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0, 
-			upperContrast=5.0, lowerDotThresh=1.2, upperDotThresh=1.8, lowerBlobThresh=1.3, 
-			program="density", polygon=None, densityData={})
-		microscopeImage = MicroscopeImage("test/directory/", "filename.png", fakeUserSettings)
-		return microscopeImage, fakeUserSettings
-	
-	def test_upperDotThresholdScaleDown(self):
-		'''getFullDataSquareSum generates the following from the given test data:
- 		[[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
-		 [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
-		 [ 4  4  2  0  1  1  0 -4 -4 -1  2  2  0]
-		 [-1 -1  0  0  0  1  1 -1 -2  0  2  2  0]
-		 [-1 -1  0  0  0  6 10 10  4  0  0  0  0]
-		 [-1 -1  0  0  0  8 12 11  3 -1  0  0  0]
-		 [ 0  0  0  0  0  7 10  8  1 -2  0  0  0]
-		 [ 7  7  7  0  0  2  1 -1 -3 -2  1  1  1]
-		 [12 21 21  9  0  0  0 -1 -1 -1  9  9  9]
-		 [11 20 21  9  0  0  1  1  1  0 10 10 10]
-		 [ 4 13 14  9  0  0  1  1  1  0  9  9  9]]
-		
-		Given the threshold scales of 1.2, 1.8, and 1.3, the thresholds are:
-		6.151707193431039, 9.227560790146558, and 11.995829027190528
-		
-		Decreasing the upper dot thresh scale by 0.1 results in the following:
-		6.151707193431039, 8.714918524027306, and 11.995829027190528
-		
-		This means that getFullDataSquareSum values of 9 will be evaluated as potential blobs now,
-		resulting in the previous dot with testData value 8 detected at (x, y) = (11, 9) no
-		longer being detected as a dot.
-		
-		Also, because of the getFullDataSquareSum values of 9 at (x, y) = (3, 8) and (10, 8), and 
-		the blob size of 3, the testData values of 5, 4, and 2 near the middle of the image are
-		no longer considered, and the testData value of 1 at (x, y) = (6, 4) is the new dot.'''
-		
-		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
-		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
-		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
-		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
-		
-		# Expected offsets = [[6, 5], [11, 9]]
-		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets), 2)
-		self.assertIn([6, 5], dotOffsets)
-		self.assertIn([11, 9], dotOffsets)
-		self.assertEqual(len(dotOffsets), 2)
-		
-		thresholdAdjuster.upperDotThresholdScaleDown()
-		
-		# Expected offsets = [[6, 4]]
-		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
-		self.assertEqual(len(dotOffsets2), 1)
-		self.assertIn([6, 4], dotOffsets2)
-	
-	def test_upperDotThresholdScaleUp(self):
-		# This is the inverse of the previous test, scaling down first, and then back up
-		
-		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
-		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
-		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
-		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
-		
-		thresholdAdjuster.upperDotThresholdScaleDown()
-		
-		# Expected offsets = [[6, 4]]
-		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
-		self.assertEqual(len(dotOffsets), 1)
-		self.assertIn([6, 4], dotOffsets)
-		
-		thresholdAdjuster.upperDotThresholdScaleUp()
-		
-		# Expected offsets = [[6, 5], [11, 9]]
-		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets2), 2)
-		self.assertIn([6, 5], dotOffsets2)
-		self.assertIn([11, 9], dotOffsets2)
-	
-	def test_lowerDotThresholdScaleDown(self):
-		'''getFullDataSquareSum generates the following from the given test data:
- 		[[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
-		 [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
-		 [ 4  4  2  0  1  1  0 -4 -4 -1  2  2  0]
-		 [-1 -1  0  0  0  1  1 -1 -2  0  2  2  0]
-		 [-1 -1  0  0  0  6 10 10  4  0  0  0  0]
-		 [-1 -1  0  0  0  8 12 11  3 -1  0  0  0]
-		 [ 0  0  0  0  0  7 10  8  1 -2  0  0  0]
-		 [ 7  7  7  0  0  2  1 -1 -3 -2  1  1  1]
-		 [12 21 21  9  0  0  0 -1 -1 -1  9  9  9]
-		 [11 20 21  9  0  0  1  1  1  0 10 10 10]
-		 [ 4 13 14  9  0  0  1  1  1  0  9  9  9]]
-		
-		Given the threshold scales of 1.2, 1.8, and 1.3, the thresholds are:
-		6.151707193431039, 9.227560790146558, and 11.995829027190528
-		
-		Decreasing the lower dot thresh scale by 0.1 results in the following:
-		5.639064927311785, 8.714918524027306, and 11.995829027190528
-		
-		This means that getFullDataSquareSum values of 6 will be bright enough to be dots now,
-		resulting in a new dot at (0, 0).'''
-		
-		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
-		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
-		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
-		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
-		
-		# Expected offsets = [[6, 5], [11, 9]]
-		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets), 2)
-		self.assertIn([6, 5], dotOffsets)
-		self.assertIn([11, 9], dotOffsets)
-		
-		thresholdAdjuster.lowerDotThresholdScaleDown()
-		
-		# Expected offsets = [[0, 0], [6, 5], [11, 9]]
-		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets2), 3)
-		self.assertIn([0, 0], dotOffsets2)
-		self.assertIn([6, 5], dotOffsets2)
-		self.assertIn([11, 9], dotOffsets2)
-	
-	def test_lowerDotThresholdScaleUp(self):
-		# This is the inverse of the previous test, scaling down first, and then back up
-		
-		microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
-		thresholdAdjuster = ThresholdAdjuster(microscopeImage, fakeUserSettings, drawUi=False)
-		thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
-		thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
-		
-		thresholdAdjuster.lowerDotThresholdScaleDown()
-		
-		# Expected offsets = [[0, 0], [6, 5], [11, 9]]
-		dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets), 3)
-		self.assertIn([0, 0], dotOffsets)
-		self.assertIn([6, 5], dotOffsets)
-		self.assertIn([11, 9], dotOffsets)
-		
-		thresholdAdjuster.lowerDotThresholdScaleUp()
-		
-		# Expected offsets = [[6, 5], [11, 9]]
-		dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
-		
-		self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
-		self.assertEqual(len(dotOffsets2), 2)
-		self.assertIn([6, 5], dotOffsets2)
-		self.assertIn([11, 9], dotOffsets2)
+    @mock.patch("src.dataprocessing.getData")
+    def getMicroscopeImageAndUserSettings(self, mock_getData):
+        testData = np.array([
+            [2,  0,  0,  0,  0,  0, -2,  0,  0,  0,  0,  0,  0],
+            [2,  2,  0,  0,  0,  1,  0, -1, -1,  0,  0,  0,  0],
+            [0,  0,  0,  0,  0,  0,  0,  0, -2,  0,  2,  0,  0],
+            [0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0],
+            [-1,  0,  0,  0,  0,  0,  1,  0,  0,  0,  0,  0,  0],
+            [0,  0,  0,  0,  0,  0,  5,  4,  0,  0,  0,  0,  0],
+            [0,  0,  0,  0,  0,  0,  2,  0, -1,  0,  0,  0,  0],
+            [0,  0,  0,  0,  0,  0,  0, -1, -1,  0,  0,  0,  0],
+            [0,  7,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
+            [0,  5,  9,  0,  0,  0,  0,  1,  0,  0,  0,  8,  0],
+            [-1,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  1,  0],
+        ])
+        mock_getData.return_value = testData
+        fakeUserSettings = FakeUserSettings(
+            filepath="test/directory/", dotSize=2, blobSize=3, saveFigures=False,
+            startImage="", skipsAllowed=0, removeEdgeFrames=True, lowerContrast=0.0,
+            upperContrast=5.0, lowerDotThresh=1.2, upperDotThresh=1.8, lowerBlobThresh=1.3,
+            program="density", polygon=None, densityData={})
+        microscopeImage = MicroscopeImage(
+            "test/directory/", "filename.png", fakeUserSettings)
+        return microscopeImage, fakeUserSettings
+
+    def test_upperDotThresholdScaleDown(self):
+        '''getFullDataSquareSum generates the following from the given test data:
+        [[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
+         [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
+         [ 4  4  2  0  1  1  0 -4 -4 -1  2  2  0]
+         [-1 -1  0  0  0  1  1 -1 -2  0  2  2  0]
+         [-1 -1  0  0  0  6 10 10  4  0  0  0  0]
+         [-1 -1  0  0  0  8 12 11  3 -1  0  0  0]
+         [ 0  0  0  0  0  7 10  8  1 -2  0  0  0]
+         [ 7  7  7  0  0  2  1 -1 -3 -2  1  1  1]
+         [12 21 21  9  0  0  0 -1 -1 -1  9  9  9]
+         [11 20 21  9  0  0  1  1  1  0 10 10 10]
+         [ 4 13 14  9  0  0  1  1  1  0  9  9  9]]
+
+        Given the threshold scales of 1.2, 1.8, and 1.3, the thresholds are:
+        6.151707193431039, 9.227560790146558, and 11.995829027190528
+
+        Decreasing the upper dot thresh scale by 0.1 results in the following:
+        6.151707193431039, 8.714918524027306, and 11.995829027190528
+
+        This means that getFullDataSquareSum values of 9 will be evaluated as potential blobs now,
+        resulting in the previous dot with testData value 8 detected at (x, y) = (11, 9) no
+        longer being detected as a dot.
+
+        Also, because of the getFullDataSquareSum values of 9 at (x, y) = (3, 8) and (10, 8), and 
+        the blob size of 3, the testData values of 5, 4, and 2 near the middle of the image are
+        no longer considered, and the testData value of 1 at (x, y) = (6, 4) is the new dot.'''
+
+        microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
+        thresholdAdjuster = ThresholdAdjuster(
+            microscopeImage, fakeUserSettings, drawUi=False)
+        thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
+        thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
+
+        # Expected offsets = [[6, 5], [11, 9]]
+        dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets), 2)
+        self.assertIn([6, 5], dotOffsets)
+        self.assertIn([11, 9], dotOffsets)
+        self.assertEqual(len(dotOffsets), 2)
+
+        thresholdAdjuster.upperDotThresholdScaleDown()
+
+        # Expected offsets = [[6, 4]]
+        dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
+        self.assertEqual(len(dotOffsets2), 1)
+        self.assertIn([6, 4], dotOffsets2)
+
+    def test_upperDotThresholdScaleUp(self):
+        # This is the inverse of the previous test, scaling down first, and then back up
+
+        microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
+        thresholdAdjuster = ThresholdAdjuster(
+            microscopeImage, fakeUserSettings, drawUi=False)
+        thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
+        thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
+
+        thresholdAdjuster.upperDotThresholdScaleDown()
+
+        # Expected offsets = [[6, 4]]
+        dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.7, 1.3))
+        self.assertEqual(len(dotOffsets), 1)
+        self.assertIn([6, 4], dotOffsets)
+
+        thresholdAdjuster.upperDotThresholdScaleUp()
+
+        # Expected offsets = [[6, 5], [11, 9]]
+        dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets2), 2)
+        self.assertIn([6, 5], dotOffsets2)
+        self.assertIn([11, 9], dotOffsets2)
+
+    def test_lowerDotThresholdScaleDown(self):
+        '''getFullDataSquareSum generates the following from the given test data:
+        [[ 6  6  2  0  1 -1 -2 -4 -2 -1  0  0  0]
+         [ 6  6  2  0  1 -1 -2 -6 -4 -1  2  2  0]
+         [ 4  4  2  0  1  1  0 -4 -4 -1  2  2  0]
+         [-1 -1  0  0  0  1  1 -1 -2  0  2  2  0]
+         [-1 -1  0  0  0  6 10 10  4  0  0  0  0]
+         [-1 -1  0  0  0  8 12 11  3 -1  0  0  0]
+         [ 0  0  0  0  0  7 10  8  1 -2  0  0  0]
+         [ 7  7  7  0  0  2  1 -1 -3 -2  1  1  1]
+         [12 21 21  9  0  0  0 -1 -1 -1  9  9  9]
+         [11 20 21  9  0  0  1  1  1  0 10 10 10]
+         [ 4 13 14  9  0  0  1  1  1  0  9  9  9]]
+
+        Given the threshold scales of 1.2, 1.8, and 1.3, the thresholds are:
+        6.151707193431039, 9.227560790146558, and 11.995829027190528
+
+        Decreasing the lower dot thresh scale by 0.1 results in the following:
+        5.639064927311785, 8.714918524027306, and 11.995829027190528
+
+        This means that getFullDataSquareSum values of 6 will be bright enough to be dots now,
+        resulting in a new dot at (0, 0).'''
+
+        microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
+        thresholdAdjuster = ThresholdAdjuster(
+            microscopeImage, fakeUserSettings, drawUi=False)
+        thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
+        thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
+
+        # Expected offsets = [[6, 5], [11, 9]]
+        dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets), 2)
+        self.assertIn([6, 5], dotOffsets)
+        self.assertIn([11, 9], dotOffsets)
+
+        thresholdAdjuster.lowerDotThresholdScaleDown()
+
+        # Expected offsets = [[0, 0], [6, 5], [11, 9]]
+        dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets2), 3)
+        self.assertIn([0, 0], dotOffsets2)
+        self.assertIn([6, 5], dotOffsets2)
+        self.assertIn([11, 9], dotOffsets2)
+
+    def test_lowerDotThresholdScaleUp(self):
+        # This is the inverse of the previous test, scaling down first, and then back up
+
+        microscopeImage, fakeUserSettings = self.getMicroscopeImageAndUserSettings()
+        thresholdAdjuster = ThresholdAdjuster(
+            microscopeImage, fakeUserSettings, drawUi=False)
+        thresholdAdjuster.setThresholdEntries = MagicMock(return_value=None)
+        thresholdAdjuster.canvas.draw = MagicMock(return_value=None)
+
+        thresholdAdjuster.lowerDotThresholdScaleDown()
+
+        # Expected offsets = [[0, 0], [6, 5], [11, 9]]
+        dotOffsets = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.1, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets), 3)
+        self.assertIn([0, 0], dotOffsets)
+        self.assertIn([6, 5], dotOffsets)
+        self.assertIn([11, 9], dotOffsets)
+
+        thresholdAdjuster.lowerDotThresholdScaleUp()
+
+        # Expected offsets = [[6, 5], [11, 9]]
+        dotOffsets2 = thresholdAdjuster.dotScatter.get_offsets()
+
+        self.assertEqual(microscopeImage.thresholds, (1.2, 1.8, 1.3))
+        self.assertEqual(len(dotOffsets2), 2)
+        self.assertIn([6, 5], dotOffsets2)
+        self.assertIn([11, 9], dotOffsets2)
+
 
 if __name__ == '__main__':
-	unittest.main()
+    unittest.main()
```

