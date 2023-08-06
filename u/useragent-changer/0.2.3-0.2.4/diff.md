# Comparing `tmp/useragent_changer-0.2.3.tar.gz` & `tmp/useragent_changer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useragent_changer-0.2.3.tar", last modified: Sun Aug  6 19:11:46 2023, max compression
+gzip compressed data, was "useragent_changer-0.2.4.tar", last modified: Sun Aug  6 19:44:11 2023, max compression
```

## Comparing `useragent_changer-0.2.3.tar` & `useragent_changer-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:11:46.508185 useragent_changer-0.2.3/
--rw-r--r--   0 ym         (501) staff       (20)     1054 2023-07-25 08:17:12.000000 useragent_changer-0.2.3/LICENSE.txt
--rw-r--r--   0 ym         (501) staff       (20)     4285 2023-08-06 19:11:46.508057 useragent_changer-0.2.3/PKG-INFO
--rw-r--r--   0 ym         (501) staff       (20)     3223 2023-08-06 19:09:39.000000 useragent_changer-0.2.3/README.md
--rw-r--r--   0 ym         (501) staff       (20)       38 2023-08-06 19:11:46.508232 useragent_changer-0.2.3/setup.cfg
--rw-r--r--   0 ym         (501) staff       (20)     1552 2023-07-25 09:12:22.000000 useragent_changer-0.2.3/setup.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:11:46.497170 useragent_changer-0.2.3/useragent_changer/
--rw-r--r--   0 ym         (501) staff       (20)      542 2023-08-06 19:09:39.000000 useragent_changer-0.2.3/useragent_changer/__init__.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:11:46.506143 useragent_changer-0.2.3/useragent_changer/platform_list/
--rw-r--r--   0 ym         (501) staff       (20)   263131 2022-11-18 14:47:24.000000 useragent_changer-0.2.3/useragent_changer/platform_list/android.csv
--rw-r--r--   0 ym         (501) staff       (20)   753226 2022-11-18 17:06:16.000000 useragent_changer-0.2.3/useragent_changer/platform_list/chrome.csv
--rw-r--r--   0 ym         (501) staff       (20)    12715 2023-07-25 15:08:16.000000 useragent_changer-0.2.3/useragent_changer/platform_list/edge.csv
--rw-r--r--   0 ym         (501) staff       (20)   171945 2022-11-18 17:07:14.000000 useragent_changer-0.2.3/useragent_changer/platform_list/firefox.csv
--rw-r--r--   0 ym         (501) staff       (20)     6140 2022-11-19 19:47:27.000000 useragent_changer-0.2.3/useragent_changer/platform_list/ipad.csv
--rw-r--r--   0 ym         (501) staff       (20)   111220 2022-11-18 13:47:03.000000 useragent_changer-0.2.3/useragent_changer/platform_list/iphone.csv
--rw-r--r--   0 ym         (501) staff       (20)   210591 2022-11-18 15:02:13.000000 useragent_changer-0.2.3/useragent_changer/platform_list/mac.csv
--rw-r--r--   0 ym         (501) staff       (20)   745382 2022-11-18 17:08:10.000000 useragent_changer-0.2.3/useragent_changer/platform_list/safari.csv
--rw-r--r--   0 ym         (501) staff       (20)   298055 2022-11-18 17:04:00.000000 useragent_changer-0.2.3/useragent_changer/platform_list/windows.csv
--rw-r--r--   0 ym         (501) staff       (20)     2476 2023-08-01 17:57:00.000000 useragent_changer-0.2.3/useragent_changer/useragent_changer.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:11:46.498037 useragent_changer-0.2.3/useragent_changer.egg-info/
--rw-r--r--   0 ym         (501) staff       (20)     4285 2023-08-06 19:11:46.000000 useragent_changer-0.2.3/useragent_changer.egg-info/PKG-INFO
--rw-r--r--   0 ym         (501) staff       (20)      646 2023-08-06 19:11:46.000000 useragent_changer-0.2.3/useragent_changer.egg-info/SOURCES.txt
--rw-r--r--   0 ym         (501) staff       (20)        1 2023-08-06 19:11:46.000000 useragent_changer-0.2.3/useragent_changer.egg-info/dependency_links.txt
--rw-r--r--   0 ym         (501) staff       (20)       18 2023-08-06 19:11:46.000000 useragent_changer-0.2.3/useragent_changer.egg-info/top_level.txt
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:44:11.911071 useragent_changer-0.2.4/
+-rw-r--r--   0 ym         (501) staff       (20)     1054 2023-07-25 08:17:12.000000 useragent_changer-0.2.4/LICENSE.txt
+-rw-r--r--   0 ym         (501) staff       (20)     4222 2023-08-06 19:44:11.910954 useragent_changer-0.2.4/PKG-INFO
+-rw-r--r--   0 ym         (501) staff       (20)     3160 2023-08-06 19:42:55.000000 useragent_changer-0.2.4/README.md
+-rw-r--r--   0 ym         (501) staff       (20)       38 2023-08-06 19:44:11.911107 useragent_changer-0.2.4/setup.cfg
+-rw-r--r--   0 ym         (501) staff       (20)     1552 2023-07-25 09:12:22.000000 useragent_changer-0.2.4/setup.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:44:11.907840 useragent_changer-0.2.4/useragent_changer/
+-rw-r--r--   0 ym         (501) staff       (20)      542 2023-08-06 19:42:55.000000 useragent_changer-0.2.4/useragent_changer/__init__.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:44:11.910595 useragent_changer-0.2.4/useragent_changer/platform_list/
+-rw-r--r--   0 ym         (501) staff       (20)   263131 2022-11-18 14:47:24.000000 useragent_changer-0.2.4/useragent_changer/platform_list/android.csv
+-rw-r--r--   0 ym         (501) staff       (20)   753226 2022-11-18 17:06:16.000000 useragent_changer-0.2.4/useragent_changer/platform_list/chrome.csv
+-rw-r--r--   0 ym         (501) staff       (20)    12715 2023-07-25 15:08:16.000000 useragent_changer-0.2.4/useragent_changer/platform_list/edge.csv
+-rw-r--r--   0 ym         (501) staff       (20)   171945 2022-11-18 17:07:14.000000 useragent_changer-0.2.4/useragent_changer/platform_list/firefox.csv
+-rw-r--r--   0 ym         (501) staff       (20)     6140 2022-11-19 19:47:27.000000 useragent_changer-0.2.4/useragent_changer/platform_list/ipad.csv
+-rw-r--r--   0 ym         (501) staff       (20)   111220 2022-11-18 13:47:03.000000 useragent_changer-0.2.4/useragent_changer/platform_list/iphone.csv
+-rw-r--r--   0 ym         (501) staff       (20)   210591 2022-11-18 15:02:13.000000 useragent_changer-0.2.4/useragent_changer/platform_list/mac.csv
+-rw-r--r--   0 ym         (501) staff       (20)   745382 2022-11-18 17:08:10.000000 useragent_changer-0.2.4/useragent_changer/platform_list/safari.csv
+-rw-r--r--   0 ym         (501) staff       (20)   298055 2022-11-18 17:04:00.000000 useragent_changer-0.2.4/useragent_changer/platform_list/windows.csv
+-rw-r--r--   0 ym         (501) staff       (20)     2476 2023-08-01 17:57:00.000000 useragent_changer-0.2.4/useragent_changer/useragent_changer.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-06 19:44:11.908309 useragent_changer-0.2.4/useragent_changer.egg-info/
+-rw-r--r--   0 ym         (501) staff       (20)     4222 2023-08-06 19:44:11.000000 useragent_changer-0.2.4/useragent_changer.egg-info/PKG-INFO
+-rw-r--r--   0 ym         (501) staff       (20)      646 2023-08-06 19:44:11.000000 useragent_changer-0.2.4/useragent_changer.egg-info/SOURCES.txt
+-rw-r--r--   0 ym         (501) staff       (20)        1 2023-08-06 19:44:11.000000 useragent_changer-0.2.4/useragent_changer.egg-info/dependency_links.txt
+-rw-r--r--   0 ym         (501) staff       (20)       18 2023-08-06 19:44:11.000000 useragent_changer-0.2.4/useragent_changer.egg-info/top_level.txt
```

### Comparing `useragent_changer-0.2.3/LICENSE.txt` & `useragent_changer-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/PKG-INFO` & `useragent_changer-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useragent_changer
-Version: 0.2.3
+Version: 0.2.4
 Summary: User-Agent changing library for Python.
 Home-page: https://github.com/gitmori/useragent-changer
 Download-URL: https://github.com/gitmori/useragent-changer
 Author: Yuki Moriya
 Author-email: ym19820219@gmail.com
 Maintainer: Yuki Moriya
 Maintainer-email: ym19820219@gmail.com
@@ -24,18 +24,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # useragent-changer
 A library for changing user agents in order to verify the operation of web systems.
 
 ## Features
-- This package contains a total of 19381 User-Agents for Android, iPhone, iPad, Windows, Mac, Chrome, Edge, Safari and Firefox.
+- This package contains a total of 19,381 User-Agent data for Android (2,144), Chrome (4,996), Edge (91), Firefox (2,132), iPad (45), iPhone (750), Mac (1,739), Safari (4,952), Windows (2,532).
 - User-Agent corresponding to each platform is described in 9 csv files in the data folder in this package.
-- Number of User-Agent data: Android (2144), Chrome (4996), Edge (91), Firefox (2132), iPad (45), iPhone (750), Mac (1739), Safari (4952), Windows (2532)
-- There are a total of 19381 User-Agents.
 - Supports Python 3.x
 
 ### Installation
 Enter one of the following two commands:
 ```
 pip install useragent-changer
 ```
@@ -116,14 +114,16 @@
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.2 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.3 August 06, 2023
     - Fixed README file and version number
+- 0.2.4 August 06, 2023
+    - Fixed README file and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.3/README.md` & `useragent_changer-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # useragent-changer
 A library for changing user agents in order to verify the operation of web systems.
 
 ## Features
-- This package contains a total of 19381 User-Agents for Android, iPhone, iPad, Windows, Mac, Chrome, Edge, Safari and Firefox.
+- This package contains a total of 19,381 User-Agent data for Android (2,144), Chrome (4,996), Edge (91), Firefox (2,132), iPad (45), iPhone (750), Mac (1,739), Safari (4,952), Windows (2,532).
 - User-Agent corresponding to each platform is described in 9 csv files in the data folder in this package.
-- Number of User-Agent data: Android (2144), Chrome (4996), Edge (91), Firefox (2132), iPad (45), iPhone (750), Mac (1739), Safari (4952), Windows (2532)
-- There are a total of 19381 User-Agents.
 - Supports Python 3.x
 
 ### Installation
 Enter one of the following two commands:
 ```
 pip install useragent-changer
 ```
@@ -90,14 +88,16 @@
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.2 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.3 August 06, 2023
     - Fixed README file and version number
+- 0.2.4 August 06, 2023
+    - Fixed README file and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.3/setup.py` & `useragent_changer-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/__init__.py` & `useragent_changer-0.2.4/useragent_changer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 # Make the module name 'useragent_changer' optional.
 from .useragent_changer import *
 
 __copyright__    = 'Copyright (C) 2023 Yuki Moriya'
-__version__      = '0.2.3'
+__version__      = '0.2.4'
 __description__  = 'User-Agent changing library for Python.'
 __author__       = 'Yuki Moriya'
 __author_email__ = 'ym19820219@gmail.com'
 __keywords__     = 'useragent user_agent user-agent ua useragent_change useragent_changer useragent-changer useragent-change'
 __url__          = 'https://github.com/gitmori/useragent-changer'
 __license__      = 'MIT'
```

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/android.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/android.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/chrome.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/chrome.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/edge.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/edge.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/firefox.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/firefox.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/ipad.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/ipad.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/iphone.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/iphone.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/mac.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/mac.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/safari.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/safari.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/platform_list/windows.csv` & `useragent_changer-0.2.4/useragent_changer/platform_list/windows.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer/useragent_changer.py` & `useragent_changer-0.2.4/useragent_changer/useragent_changer.py`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.3/useragent_changer.egg-info/PKG-INFO` & `useragent_changer-0.2.4/useragent_changer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useragent-changer
-Version: 0.2.3
+Version: 0.2.4
 Summary: User-Agent changing library for Python.
 Home-page: https://github.com/gitmori/useragent-changer
 Download-URL: https://github.com/gitmori/useragent-changer
 Author: Yuki Moriya
 Author-email: ym19820219@gmail.com
 Maintainer: Yuki Moriya
 Maintainer-email: ym19820219@gmail.com
@@ -24,18 +24,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # useragent-changer
 A library for changing user agents in order to verify the operation of web systems.
 
 ## Features
-- This package contains a total of 19381 User-Agents for Android, iPhone, iPad, Windows, Mac, Chrome, Edge, Safari and Firefox.
+- This package contains a total of 19,381 User-Agent data for Android (2,144), Chrome (4,996), Edge (91), Firefox (2,132), iPad (45), iPhone (750), Mac (1,739), Safari (4,952), Windows (2,532).
 - User-Agent corresponding to each platform is described in 9 csv files in the data folder in this package.
-- Number of User-Agent data: Android (2144), Chrome (4996), Edge (91), Firefox (2132), iPad (45), iPhone (750), Mac (1739), Safari (4952), Windows (2532)
-- There are a total of 19381 User-Agents.
 - Supports Python 3.x
 
 ### Installation
 Enter one of the following two commands:
 ```
 pip install useragent-changer
 ```
@@ -116,14 +114,16 @@
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.2 August 06, 2023
     - Fixed README file, test files and version number
 - 0.2.3 August 06, 2023
     - Fixed README file and version number
+- 0.2.4 August 06, 2023
+    - Fixed README file and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.3/useragent_changer.egg-info/SOURCES.txt` & `useragent_changer-0.2.4/useragent_changer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

