# Comparing `tmp/RapidMangaDL-0.2.4.tar.gz` & `tmp/RapidMangaDL-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RapidMangaDL-0.2.4.tar", last modified: Sun Jul 23 12:48:20 2023, max compression
+gzip compressed data, was "RapidMangaDL-0.2.5.tar", last modified: Sun Aug  6 14:11:56 2023, max compression
```

## Comparing `RapidMangaDL-0.2.4.tar` & `RapidMangaDL-0.2.5.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.596277 RapidMangaDL-0.2.4/
--rw-rw-rw-   0        0        0     1104 2023-07-19 04:26:03.000000 RapidMangaDL-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     7036 2023-07-23 12:48:20.594275 RapidMangaDL-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5609 2023-07-23 12:48:06.000000 RapidMangaDL-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.439710 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/
--rw-rw-rw-   0        0        0     7036 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1112 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      295 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-23 12:48:20.000000 RapidMangaDL-0.2.4/RapidMangaDL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2195 2023-07-19 06:16:58.000000 RapidMangaDL-0.2.4/cx_setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.452731 RapidMangaDL-0.2.4/manga_dl/
--rw-rw-rw-   0        0        0      106 2023-07-19 10:39:30.000000 RapidMangaDL-0.2.4/manga_dl/__init__.py
--rw-rw-rw-   0        0        0     7195 2023-07-23 10:27:14.000000 RapidMangaDL-0.2.4/manga_dl/app.py
--rw-rw-rw-   0        0        0     8308 2023-07-23 10:17:27.000000 RapidMangaDL-0.2.4/manga_dl/main.py
--rw-rw-rw-   0        0        0    30776 2023-07-23 06:22:54.000000 RapidMangaDL-0.2.4/manga_dl/manga.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.468717 RapidMangaDL-0.2.4/manga_dl/manga_sources/
--rw-rw-rw-   0        0        0      615 2023-07-23 11:57:18.000000 RapidMangaDL-0.2.4/manga_dl/manga_sources/__init__.py
--rw-rw-rw-   0        0        0     6955 2023-07-23 06:06:38.000000 RapidMangaDL-0.2.4/manga_dl/manga_sources/base_source.py
--rw-rw-rw-   0        0        0    20194 2023-07-23 10:58:45.000000 RapidMangaDL-0.2.4/manga_dl/manga_sources/source1.py
--rw-rw-rw-   0        0        0     9640 2023-07-23 11:59:54.000000 RapidMangaDL-0.2.4/manga_dl/manga_sources/source2.py
--rw-rw-rw-   0        0        0    14406 2023-07-23 10:28:35.000000 RapidMangaDL-0.2.4/manga_dl/manga_sources/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.515260 RapidMangaDL-0.2.4/manga_dl/public/
--rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.2.4/manga_dl/public/bootstrap530.css
--rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.2.4/manga_dl/public/bootstrap530.js
--rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.2.4/manga_dl/public/error.png
--rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.2.4/manga_dl/public/jquery321.js
--rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.2.4/manga_dl/public/loading-fast.gif
--rw-rw-rw-   0        0        0     8748 2023-07-23 11:52:48.000000 RapidMangaDL-0.2.4/manga_dl/public/manga.js
--rw-rw-rw-   0        0        0     3407 2023-07-19 11:51:16.000000 RapidMangaDL-0.2.4/manga_dl/public/search.js
--rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.2.4/manga_dl/public/style.css
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.542256 RapidMangaDL-0.2.4/manga_dl/templates/
--rw-rw-rw-   0        0        0     4243 2023-07-23 10:14:40.000000 RapidMangaDL-0.2.4/manga_dl/templates/chapter.html
--rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.2.4/manga_dl/templates/layout.html
--rw-rw-rw-   0        0        0    13076 2023-07-23 11:08:07.000000 RapidMangaDL-0.2.4/manga_dl/templates/manga.html
--rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.2.4/manga_dl/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-23 12:48:20.590276 RapidMangaDL-0.2.4/manga_dl/tools/
--rw-rw-rw-   0        0        0      183 2023-07-17 14:00:50.000000 RapidMangaDL-0.2.4/manga_dl/tools/__init__.py
--rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.2.4/manga_dl/tools/create_pdf.py
--rw-rw-rw-   0        0        0     9652 2023-07-17 09:15:36.000000 RapidMangaDL-0.2.4/manga_dl/tools/download.py
--rw-rw-rw-   0        0        0     7272 2023-07-23 09:35:52.000000 RapidMangaDL-0.2.4/manga_dl/tools/downloader2.py
--rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.2.4/manga_dl/tools/downloader3.py
--rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.2.4/manga_dl/tools/exceptions.py
--rw-rw-rw-   0        0        0     7137 2023-07-17 14:19:26.000000 RapidMangaDL-0.2.4/manga_dl/tools/flask_cloudflared.py
--rw-rw-rw-   0        0        0     1308 2023-07-18 07:58:37.000000 RapidMangaDL-0.2.4/manga_dl/tools/models.py
--rw-rw-rw-   0        0        0    10732 2023-07-23 11:03:24.000000 RapidMangaDL-0.2.4/manga_dl/tools/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-23 12:48:20.596277 RapidMangaDL-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2189 2023-07-23 12:47:46.000000 RapidMangaDL-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:56.264660 RapidMangaDL-0.2.5/
+-rw-rw-rw-   0        0        0     1104 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     7042 2023-08-06 14:11:56.263657 RapidMangaDL-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5615 2023-08-06 14:09:54.000000 RapidMangaDL-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:55.255774 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/
+-rw-rw-rw-   0        0        0     7042 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      295 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 14:11:54.000000 RapidMangaDL-0.2.5/RapidMangaDL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:55.274783 RapidMangaDL-0.2.5/manga_dl/
+-rw-rw-rw-   0        0        0      106 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/__init__.py
+-rw-rw-rw-   0        0        0     7195 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/app.py
+-rw-rw-rw-   0        0        0     8308 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/main.py
+-rw-rw-rw-   0        0        0    30776 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:55.288778 RapidMangaDL-0.2.5/manga_dl/manga_sources/
+-rw-rw-rw-   0        0        0      615 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga_sources/__init__.py
+-rw-rw-rw-   0        0        0     6955 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga_sources/base_source.py
+-rw-rw-rw-   0        0        0    20195 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga_sources/source1.py
+-rw-rw-rw-   0        0        0     9640 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga_sources/source2.py
+-rw-rw-rw-   0        0        0    14406 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/manga_sources/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:56.002380 RapidMangaDL-0.2.5/manga_dl/public/
+-rw-rw-rw-   0        0        0   232918 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/bootstrap530.css
+-rw-rw-rw-   0        0        0    80427 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/bootstrap530.js
+-rw-rw-rw-   0        0        0    65212 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/error.png
+-rw-rw-rw-   0        0        0    86663 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/jquery321.js
+-rw-rw-rw-   0        0        0   215111 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/loading-fast.gif
+-rw-rw-rw-   0        0        0     8748 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/manga.js
+-rw-rw-rw-   0        0        0     3407 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/search.js
+-rw-rw-rw-   0        0        0     4075 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/public/style.css
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:56.208924 RapidMangaDL-0.2.5/manga_dl/templates/
+-rw-rw-rw-   0        0        0     4243 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/templates/chapter.html
+-rw-rw-rw-   0        0        0     3200 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/templates/layout.html
+-rw-rw-rw-   0        0        0    13076 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/templates/manga.html
+-rw-rw-rw-   0        0        0     2287 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-08-06 14:11:56.260662 RapidMangaDL-0.2.5/manga_dl/tools/
+-rw-rw-rw-   0        0        0      183 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/__init__.py
+-rw-rw-rw-   0        0        0     8192 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/create_pdf.py
+-rw-rw-rw-   0        0        0     9652 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/download.py
+-rw-rw-rw-   0        0        0     7272 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/downloader2.py
+-rw-rw-rw-   0        0        0     8588 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/downloader3.py
+-rw-rw-rw-   0        0        0      188 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/exceptions.py
+-rw-rw-rw-   0        0        0     7137 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/flask_cloudflared.py
+-rw-rw-rw-   0        0        0     1308 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/models.py
+-rw-rw-rw-   0        0        0    10732 2023-08-06 14:05:41.000000 RapidMangaDL-0.2.5/manga_dl/tools/utils.py
+-rw-rw-rw-   0        0        0       42 2023-08-06 14:11:56.264660 RapidMangaDL-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2189 2023-08-06 14:10:13.000000 RapidMangaDL-0.2.5/setup.py
```

### Comparing `RapidMangaDL-0.2.4/LICENSE` & `RapidMangaDL-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/PKG-INFO` & `RapidMangaDL-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.2.4
+Version: 0.2.5
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
@@ -60,29 +60,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli.gif)
+![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI (Graphical User Interface)
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_gui.gif)
+![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 To create a shareable link, you can use the `--share` flag:
 
 ```bash
 manga-dl gui --share
 ```
```

### Comparing `RapidMangaDL-0.2.4/README.md` & `RapidMangaDL-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli.gif)
+![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI (Graphical User Interface)
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_gui.gif)
+![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 To create a shareable link, you can use the `--share` flag:
 
 ```bash
 manga-dl gui --share
 ```
```

### Comparing `RapidMangaDL-0.2.4/RapidMangaDL.egg-info/PKG-INFO` & `RapidMangaDL-0.2.5/RapidMangaDL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.2.4
+Version: 0.2.5
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
@@ -60,29 +60,29 @@
 
 ```bash
 manga-dl
 ```
 
 Here's a quick demo:
 
-![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli.gif)
+![CLI](https://github.com/shhossain/RapidMangaDL/raw/main/cli_demo.gif)
 
 # Web-based GUI (Graphical User Interface)
 
 The Web-based GUI offers a graphical interface to interact with the application. You can easily search for manga, select chapters, and initiate downloads.
 
 To start the server, run:
 
 ```bash
 manga-dl gui
 ```
 
 Here's a sneak peek:
 
-![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_gui.gif)
+![WEB DEMO](https://github.com/shhossain/RapidMangaDL/raw/main/web_demo.gif)
 
 To create a shareable link, you can use the `--share` flag:
 
 ```bash
 manga-dl gui --share
 ```
```

### Comparing `RapidMangaDL-0.2.4/RapidMangaDL.egg-info/SOURCES.txt` & `RapidMangaDL-0.2.5/RapidMangaDL.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-cx_setup.py
 setup.py
 RapidMangaDL.egg-info/PKG-INFO
 RapidMangaDL.egg-info/SOURCES.txt
 RapidMangaDL.egg-info/dependency_links.txt
 RapidMangaDL.egg-info/entry_points.txt
 RapidMangaDL.egg-info/requires.txt
 RapidMangaDL.egg-info/top_level.txt
```

### Comparing `RapidMangaDL-0.2.4/cx_setup.py` & `RapidMangaDL-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import sys
-from cx_Freeze import setup, Executable
+# setup.py
+from setuptools import setup, find_packages
+
 
 package_name = "RapidMangaDL"
-package_version = "0.1.3"
+package_version = "0.2.5"
 package_description = "Swiftly download manga from multiple sources."
 package_author = "sifat"
 package_author_email = "hossain0338@gmail.com"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
-base = None
-
-executables = [Executable("manga_dl/main.py", base=base, target_name="manga-dl")]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
@@ -32,33 +30,37 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Widget Sets",
     "Topic :: Utilities",
 ]
 
-project_urls = {
+prject_urls = {
     "Documentation": "https://github.com/shhossain/RapidMangaDL",
     "Issue Tracker": "https://github.com/shhossain/RapidMangaDL/issues",
     "Source Code": "https://github.com/shhossain/RapidMangaDL",
 }
 
 setup(
     name=package_name,
     version=package_version,
     description=package_description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=package_author,
     author_email=package_author_email,
     url="https://github.com/shhossain/RapidMangaDL",
-    packages=["manga_dl"],
+    packages=find_packages(),
     package_data={"manga_dl": ["public/*", "templates/*"]},
     include_package_data=True,
     install_requires=requirements,
+    entry_points={
+        "console_scripts": [
+            "manga-dl = manga_dl.main:main",
+        ]
+    },
     classifiers=classifiers,
     python_requires=">=3.6",
     license="MIT",
     keywords="manga downloader",
-    project_urls=project_urls,
-    executables=executables,
+    project_urls=prject_urls,
 )
```

### Comparing `RapidMangaDL-0.2.4/manga_dl/app.py` & `RapidMangaDL-0.2.5/manga_dl/app.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/main.py` & `RapidMangaDL-0.2.5/manga_dl/main.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga.py` & `RapidMangaDL-0.2.5/manga_dl/manga.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga_sources/__init__.py` & `RapidMangaDL-0.2.5/manga_dl/manga_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga_sources/base_source.py` & `RapidMangaDL-0.2.5/manga_dl/manga_sources/base_source.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga_sources/source1.py` & `RapidMangaDL-0.2.5/manga_dl/manga_sources/source1.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
                         author = ia[1].select(".text-muted")
                         author = [i.text for i in author]
 
                 # item-genre
                 genres = []
                 tgenres = item.select(".item-genre > span")
                 if tgenres:
-                    genres = [i.text for i in genres]
+                    genres = [i.text for i in tgenres]
 
                 # item-volch latest-chapter
                 latest_chapter = ""
                 tlatest_chapter = item.select_one(".item-volch > a")
                 if tlatest_chapter:
                     latest_chapter = tlatest_chapter.text.strip()  # type: ignore
```

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga_sources/source2.py` & `RapidMangaDL-0.2.5/manga_dl/manga_sources/source2.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/manga_sources/utils.py` & `RapidMangaDL-0.2.5/manga_dl/manga_sources/utils.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/bootstrap530.css` & `RapidMangaDL-0.2.5/manga_dl/public/bootstrap530.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/bootstrap530.js` & `RapidMangaDL-0.2.5/manga_dl/public/bootstrap530.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/error.png` & `RapidMangaDL-0.2.5/manga_dl/public/error.png`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/jquery321.js` & `RapidMangaDL-0.2.5/manga_dl/public/jquery321.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/loading-fast.gif` & `RapidMangaDL-0.2.5/manga_dl/public/loading-fast.gif`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/manga.js` & `RapidMangaDL-0.2.5/manga_dl/public/manga.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/search.js` & `RapidMangaDL-0.2.5/manga_dl/public/search.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/public/style.css` & `RapidMangaDL-0.2.5/manga_dl/public/style.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/templates/chapter.html` & `RapidMangaDL-0.2.5/manga_dl/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/templates/layout.html` & `RapidMangaDL-0.2.5/manga_dl/templates/layout.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/templates/manga.html` & `RapidMangaDL-0.2.5/manga_dl/templates/manga.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/templates/search.html` & `RapidMangaDL-0.2.5/manga_dl/templates/search.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/create_pdf.py` & `RapidMangaDL-0.2.5/manga_dl/tools/create_pdf.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/download.py` & `RapidMangaDL-0.2.5/manga_dl/tools/download.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/downloader2.py` & `RapidMangaDL-0.2.5/manga_dl/tools/downloader2.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/downloader3.py` & `RapidMangaDL-0.2.5/manga_dl/tools/downloader3.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/flask_cloudflared.py` & `RapidMangaDL-0.2.5/manga_dl/tools/flask_cloudflared.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/models.py` & `RapidMangaDL-0.2.5/manga_dl/tools/models.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.2.4/manga_dl/tools/utils.py` & `RapidMangaDL-0.2.5/manga_dl/tools/utils.py`

 * *Files identical despite different names*

