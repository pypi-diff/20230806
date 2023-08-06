# Comparing `tmp/useragent_changer-0.2.1.tar.gz` & `tmp/useragent_changer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useragent_changer-0.2.1.tar", last modified: Sat Aug  5 18:29:05 2023, max compression
+gzip compressed data, was "useragent_changer-0.2.2.tar", last modified: Sat Aug  5 19:28:44 2023, max compression
```

## Comparing `useragent_changer-0.2.1.tar` & `useragent_changer-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 18:29:05.081946 useragent_changer-0.2.1/
--rw-r--r--   0 ym         (501) staff       (20)     1054 2023-07-25 08:17:12.000000 useragent_changer-0.2.1/LICENSE.txt
--rw-r--r--   0 ym         (501) staff       (20)     3992 2023-08-05 18:29:05.081822 useragent_changer-0.2.1/PKG-INFO
--rw-r--r--   0 ym         (501) staff       (20)     2965 2023-08-05 18:13:11.000000 useragent_changer-0.2.1/README.md
--rw-r--r--   0 ym         (501) staff       (20)       38 2023-08-05 18:29:05.081983 useragent_changer-0.2.1/setup.cfg
--rw-r--r--   0 ym         (501) staff       (20)     1552 2023-07-25 09:12:22.000000 useragent_changer-0.2.1/setup.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 18:29:05.070716 useragent_changer-0.2.1/useragent_changer/
--rw-r--r--   0 ym         (501) staff       (20)      507 2023-08-05 18:13:11.000000 useragent_changer-0.2.1/useragent_changer/__init__.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 18:29:05.080121 useragent_changer-0.2.1/useragent_changer/platform_list/
--rw-r--r--   0 ym         (501) staff       (20)   263131 2022-11-18 14:47:24.000000 useragent_changer-0.2.1/useragent_changer/platform_list/android.csv
--rw-r--r--   0 ym         (501) staff       (20)   753226 2022-11-18 17:06:16.000000 useragent_changer-0.2.1/useragent_changer/platform_list/chrome.csv
--rw-r--r--   0 ym         (501) staff       (20)    12715 2023-07-25 15:08:16.000000 useragent_changer-0.2.1/useragent_changer/platform_list/edge.csv
--rw-r--r--   0 ym         (501) staff       (20)   171945 2022-11-18 17:07:14.000000 useragent_changer-0.2.1/useragent_changer/platform_list/firefox.csv
--rw-r--r--   0 ym         (501) staff       (20)     6140 2022-11-19 19:47:27.000000 useragent_changer-0.2.1/useragent_changer/platform_list/ipad.csv
--rw-r--r--   0 ym         (501) staff       (20)   111220 2022-11-18 13:47:03.000000 useragent_changer-0.2.1/useragent_changer/platform_list/iphone.csv
--rw-r--r--   0 ym         (501) staff       (20)   210591 2022-11-18 15:02:13.000000 useragent_changer-0.2.1/useragent_changer/platform_list/mac.csv
--rw-r--r--   0 ym         (501) staff       (20)   745382 2022-11-18 17:08:10.000000 useragent_changer-0.2.1/useragent_changer/platform_list/safari.csv
--rw-r--r--   0 ym         (501) staff       (20)   298055 2022-11-18 17:04:00.000000 useragent_changer-0.2.1/useragent_changer/platform_list/windows.csv
--rw-r--r--   0 ym         (501) staff       (20)     2476 2023-08-01 17:57:00.000000 useragent_changer-0.2.1/useragent_changer/useragent_changer.py
-drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 18:29:05.071376 useragent_changer-0.2.1/useragent_changer.egg-info/
--rw-r--r--   0 ym         (501) staff       (20)     3992 2023-08-05 18:29:05.000000 useragent_changer-0.2.1/useragent_changer.egg-info/PKG-INFO
--rw-r--r--   0 ym         (501) staff       (20)      646 2023-08-05 18:29:05.000000 useragent_changer-0.2.1/useragent_changer.egg-info/SOURCES.txt
--rw-r--r--   0 ym         (501) staff       (20)        1 2023-08-05 18:29:05.000000 useragent_changer-0.2.1/useragent_changer.egg-info/dependency_links.txt
--rw-r--r--   0 ym         (501) staff       (20)       18 2023-08-05 18:29:05.000000 useragent_changer-0.2.1/useragent_changer.egg-info/top_level.txt
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 19:28:44.132104 useragent_changer-0.2.2/
+-rw-r--r--   0 ym         (501) staff       (20)     1054 2023-07-25 08:17:12.000000 useragent_changer-0.2.2/LICENSE.txt
+-rw-r--r--   0 ym         (501) staff       (20)     4106 2023-08-05 19:28:44.131949 useragent_changer-0.2.2/PKG-INFO
+-rw-r--r--   0 ym         (501) staff       (20)     3044 2023-08-05 19:07:43.000000 useragent_changer-0.2.2/README.md
+-rw-r--r--   0 ym         (501) staff       (20)       38 2023-08-05 19:28:44.132157 useragent_changer-0.2.2/setup.cfg
+-rw-r--r--   0 ym         (501) staff       (20)     1552 2023-07-25 09:12:22.000000 useragent_changer-0.2.2/setup.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 19:28:44.119397 useragent_changer-0.2.2/useragent_changer/
+-rw-r--r--   0 ym         (501) staff       (20)      542 2023-08-05 19:10:38.000000 useragent_changer-0.2.2/useragent_changer/__init__.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 19:28:44.130135 useragent_changer-0.2.2/useragent_changer/platform_list/
+-rw-r--r--   0 ym         (501) staff       (20)   263131 2022-11-18 14:47:24.000000 useragent_changer-0.2.2/useragent_changer/platform_list/android.csv
+-rw-r--r--   0 ym         (501) staff       (20)   753226 2022-11-18 17:06:16.000000 useragent_changer-0.2.2/useragent_changer/platform_list/chrome.csv
+-rw-r--r--   0 ym         (501) staff       (20)    12715 2023-07-25 15:08:16.000000 useragent_changer-0.2.2/useragent_changer/platform_list/edge.csv
+-rw-r--r--   0 ym         (501) staff       (20)   171945 2022-11-18 17:07:14.000000 useragent_changer-0.2.2/useragent_changer/platform_list/firefox.csv
+-rw-r--r--   0 ym         (501) staff       (20)     6140 2022-11-19 19:47:27.000000 useragent_changer-0.2.2/useragent_changer/platform_list/ipad.csv
+-rw-r--r--   0 ym         (501) staff       (20)   111220 2022-11-18 13:47:03.000000 useragent_changer-0.2.2/useragent_changer/platform_list/iphone.csv
+-rw-r--r--   0 ym         (501) staff       (20)   210591 2022-11-18 15:02:13.000000 useragent_changer-0.2.2/useragent_changer/platform_list/mac.csv
+-rw-r--r--   0 ym         (501) staff       (20)   745382 2022-11-18 17:08:10.000000 useragent_changer-0.2.2/useragent_changer/platform_list/safari.csv
+-rw-r--r--   0 ym         (501) staff       (20)   298055 2022-11-18 17:04:00.000000 useragent_changer-0.2.2/useragent_changer/platform_list/windows.csv
+-rw-r--r--   0 ym         (501) staff       (20)     2476 2023-08-01 17:57:00.000000 useragent_changer-0.2.2/useragent_changer/useragent_changer.py
+drwxr-xr-x   0 ym         (501) staff       (20)        0 2023-08-05 19:28:44.120046 useragent_changer-0.2.2/useragent_changer.egg-info/
+-rw-r--r--   0 ym         (501) staff       (20)     4106 2023-08-05 19:28:44.000000 useragent_changer-0.2.2/useragent_changer.egg-info/PKG-INFO
+-rw-r--r--   0 ym         (501) staff       (20)      646 2023-08-05 19:28:44.000000 useragent_changer-0.2.2/useragent_changer.egg-info/SOURCES.txt
+-rw-r--r--   0 ym         (501) staff       (20)        1 2023-08-05 19:28:44.000000 useragent_changer-0.2.2/useragent_changer.egg-info/dependency_links.txt
+-rw-r--r--   0 ym         (501) staff       (20)       18 2023-08-05 19:28:44.000000 useragent_changer-0.2.2/useragent_changer.egg-info/top_level.txt
```

### Comparing `useragent_changer-0.2.1/LICENSE.txt` & `useragent_changer-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/PKG-INFO` & `useragent_changer-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: useragent_changer
-Version: 0.2.1
+Version: 0.2.2
 Summary: User-Agent changing library for Python.
-Home-page: https://github.com/gitmori/useragent_changer
-Download-URL: https://github.com/gitmori/useragent_changer
+Home-page: https://github.com/gitmori/useragent-changer
+Download-URL: https://github.com/gitmori/useragent-changer
 Author: Yuki Moriya
 Author-email: ym19820219@gmail.com
 Maintainer: Yuki Moriya
 Maintainer-email: ym19820219@gmail.com
 License: MIT
-Keywords: useragent user_agent user-agent ua useragent_change useragent_changer
+Keywords: useragent user_agent user-agent ua useragent_change useragent_changer useragent-changer useragent-change
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -108,14 +108,16 @@
 ```
 
 ## Changelog
 - 0.1.1 August 02, 2023
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
+- 0.2.2 August 06, 2023
+    - Fixed README file, test files and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.1/README.md` & `useragent_changer-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 ```
 
 ## Changelog
 - 0.1.1 August 02, 2023
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
+- 0.2.2 August 06, 2023
+    - Fixed README file, test files and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.1/setup.py` & `useragent_changer-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/android.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/android.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/chrome.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/chrome.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/edge.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/edge.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/firefox.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/firefox.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/ipad.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/ipad.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/iphone.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/iphone.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/mac.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/mac.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/safari.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/safari.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/platform_list/windows.csv` & `useragent_changer-0.2.2/useragent_changer/platform_list/windows.csv`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer/useragent_changer.py` & `useragent_changer-0.2.2/useragent_changer/useragent_changer.py`

 * *Files identical despite different names*

### Comparing `useragent_changer-0.2.1/useragent_changer.egg-info/PKG-INFO` & `useragent_changer-0.2.2/useragent_changer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: useragent-changer
-Version: 0.2.1
+Version: 0.2.2
 Summary: User-Agent changing library for Python.
-Home-page: https://github.com/gitmori/useragent_changer
-Download-URL: https://github.com/gitmori/useragent_changer
+Home-page: https://github.com/gitmori/useragent-changer
+Download-URL: https://github.com/gitmori/useragent-changer
 Author: Yuki Moriya
 Author-email: ym19820219@gmail.com
 Maintainer: Yuki Moriya
 Maintainer-email: ym19820219@gmail.com
 License: MIT
-Keywords: useragent user_agent user-agent ua useragent_change useragent_changer
+Keywords: useragent user_agent user-agent ua useragent_change useragent_changer useragent-changer useragent-change
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -108,14 +108,16 @@
 ```
 
 ## Changelog
 - 0.1.1 August 02, 2023
     - First push
 - 0.2.1 August 06, 2023
     - Fixed README file, test files and version number
+- 0.2.2 August 06, 2023
+    - Fixed README file, test files and version number
 
 ## Author
 Yuki Moriya ([gitmori](https://github.com/gitmori/))  
 ym19820219@gmail.com
 
 ## Licence
 Copyright (c) 2023 Yuki Moriya
```

### Comparing `useragent_changer-0.2.1/useragent_changer.egg-info/SOURCES.txt` & `useragent_changer-0.2.2/useragent_changer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

