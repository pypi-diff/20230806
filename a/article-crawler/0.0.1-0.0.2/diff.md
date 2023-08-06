# Comparing `tmp/article_crawler-0.0.1.tar.gz` & `tmp/article_crawler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "article_crawler-0.0.1.tar", last modified: Sat Aug  5 12:03:45 2023, max compression
+gzip compressed data, was "article_crawler-0.0.2.tar", last modified: Sat Aug  5 12:31:57 2023, max compression
```

## Comparing `article_crawler-0.0.1.tar` & `article_crawler-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.579498 article_crawler-0.0.1/
--rw-r--r--   0 lty        (501) staff       (20)     1062 2023-08-05 07:54:16.000000 article_crawler-0.0.1/LICENSE
--rw-r--r--   0 lty        (501) staff       (20)     2588 2023-08-05 12:03:45.579355 article_crawler-0.0.1/PKG-INFO
--rw-r--r--   0 lty        (501) staff       (20)     1976 2023-08-05 11:53:34.000000 article_crawler-0.0.1/README.md
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.576762 article_crawler-0.0.1/article_crawler/
--rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 08:51:24.000000 article_crawler-0.0.1/article_crawler/__init__.py
--rw-r--r--   0 lty        (501) staff       (20)     2753 2023-08-05 09:48:17.000000 article_crawler-0.0.1/article_crawler/__main__.py
--rw-r--r--   0 lty        (501) staff       (20)     3963 2023-08-05 11:52:06.000000 article_crawler-0.0.1/article_crawler/article_crawler.py
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.577952 article_crawler-0.0.1/article_crawler/csdn/
--rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 08:53:03.000000 article_crawler-0.0.1/article_crawler/csdn/__init__.py
--rw-r--r--   0 lty        (501) staff       (20)     1015 2023-08-05 09:44:18.000000 article_crawler-0.0.1/article_crawler/csdn/csdn_crawler.py
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.578313 article_crawler-0.0.1/article_crawler/jianshu/
--rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:51.000000 article_crawler-0.0.1/article_crawler/jianshu/__init__.py
--rw-r--r--   0 lty        (501) staff       (20)      998 2023-08-05 09:44:18.000000 article_crawler-0.0.1/article_crawler/jianshu/jianshu_crawler.py
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.578635 article_crawler-0.0.1/article_crawler/juejin/
--rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:41.000000 article_crawler-0.0.1/article_crawler/juejin/__init__.py
--rw-r--r--   0 lty        (501) staff       (20)     1015 2023-08-05 09:44:18.000000 article_crawler-0.0.1/article_crawler/juejin/juejin_crawler.py
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.578981 article_crawler-0.0.1/article_crawler/zhihu/
--rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:58.000000 article_crawler-0.0.1/article_crawler/zhihu/__init__.py
--rw-r--r--   0 lty        (501) staff       (20)     1028 2023-08-05 09:44:18.000000 article_crawler-0.0.1/article_crawler/zhihu/zhihu_crawler.py
-drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:03:45.577627 article_crawler-0.0.1/article_crawler.egg-info/
--rw-r--r--   0 lty        (501) staff       (20)     2588 2023-08-05 12:03:45.000000 article_crawler-0.0.1/article_crawler.egg-info/PKG-INFO
--rw-r--r--   0 lty        (501) staff       (20)      609 2023-08-05 12:03:45.000000 article_crawler-0.0.1/article_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 lty        (501) staff       (20)        1 2023-08-05 12:03:45.000000 article_crawler-0.0.1/article_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 lty        (501) staff       (20)       21 2023-08-05 12:03:45.000000 article_crawler-0.0.1/article_crawler.egg-info/requires.txt
--rw-r--r--   0 lty        (501) staff       (20)       16 2023-08-05 12:03:45.000000 article_crawler-0.0.1/article_crawler.egg-info/top_level.txt
--rw-r--r--   0 lty        (501) staff       (20)       38 2023-08-05 12:03:45.579542 article_crawler-0.0.1/setup.cfg
--rw-r--r--   0 lty        (501) staff       (20)     1073 2023-08-05 07:51:27.000000 article_crawler-0.0.1/setup.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.927467 article_crawler-0.0.2/
+-rw-r--r--   0 lty        (501) staff       (20)     1062 2023-08-05 07:54:16.000000 article_crawler-0.0.2/LICENSE
+-rw-r--r--   0 lty        (501) staff       (20)     3466 2023-08-05 12:31:57.927329 article_crawler-0.0.2/PKG-INFO
+-rw-r--r--   0 lty        (501) staff       (20)     2854 2023-08-05 12:29:44.000000 article_crawler-0.0.2/README.md
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.925071 article_crawler-0.0.2/article_crawler/
+-rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 08:51:24.000000 article_crawler-0.0.2/article_crawler/__init__.py
+-rw-r--r--   0 lty        (501) staff       (20)     2753 2023-08-05 09:48:17.000000 article_crawler-0.0.2/article_crawler/__main__.py
+-rw-r--r--   0 lty        (501) staff       (20)     3963 2023-08-05 11:52:06.000000 article_crawler-0.0.2/article_crawler/article_crawler.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.925974 article_crawler-0.0.2/article_crawler/csdn/
+-rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 08:53:03.000000 article_crawler-0.0.2/article_crawler/csdn/__init__.py
+-rw-r--r--   0 lty        (501) staff       (20)     1015 2023-08-05 09:44:18.000000 article_crawler-0.0.2/article_crawler/csdn/csdn_crawler.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.926350 article_crawler-0.0.2/article_crawler/jianshu/
+-rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:51.000000 article_crawler-0.0.2/article_crawler/jianshu/__init__.py
+-rw-r--r--   0 lty        (501) staff       (20)      998 2023-08-05 09:44:18.000000 article_crawler-0.0.2/article_crawler/jianshu/jianshu_crawler.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.926753 article_crawler-0.0.2/article_crawler/juejin/
+-rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:41.000000 article_crawler-0.0.2/article_crawler/juejin/__init__.py
+-rw-r--r--   0 lty        (501) staff       (20)     1015 2023-08-05 09:44:18.000000 article_crawler-0.0.2/article_crawler/juejin/juejin_crawler.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.927096 article_crawler-0.0.2/article_crawler/zhihu/
+-rw-r--r--   0 lty        (501) staff       (20)        0 2023-08-05 09:02:58.000000 article_crawler-0.0.2/article_crawler/zhihu/__init__.py
+-rw-r--r--   0 lty        (501) staff       (20)     1028 2023-08-05 09:44:18.000000 article_crawler-0.0.2/article_crawler/zhihu/zhihu_crawler.py
+drwxr-xr-x   0 lty        (501) staff       (20)        0 2023-08-05 12:31:57.925768 article_crawler-0.0.2/article_crawler.egg-info/
+-rw-r--r--   0 lty        (501) staff       (20)     3466 2023-08-05 12:31:57.000000 article_crawler-0.0.2/article_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 lty        (501) staff       (20)      609 2023-08-05 12:31:57.000000 article_crawler-0.0.2/article_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 lty        (501) staff       (20)        1 2023-08-05 12:31:57.000000 article_crawler-0.0.2/article_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 lty        (501) staff       (20)       21 2023-08-05 12:31:57.000000 article_crawler-0.0.2/article_crawler.egg-info/requires.txt
+-rw-r--r--   0 lty        (501) staff       (20)       16 2023-08-05 12:31:57.000000 article_crawler-0.0.2/article_crawler.egg-info/top_level.txt
+-rw-r--r--   0 lty        (501) staff       (20)       38 2023-08-05 12:31:57.927507 article_crawler-0.0.2/setup.cfg
+-rw-r--r--   0 lty        (501) staff       (20)     1073 2023-08-05 12:31:45.000000 article_crawler-0.0.2/setup.py
```

### Comparing `article_crawler-0.0.1/LICENSE` & `article_crawler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/PKG-INFO` & `article_crawler-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-Metadata-Version: 2.1
-Name: article_crawler
-Version: 0.0.1
-Summary: A package for crawling markdown formatted articles from certain webpage and storing them locally.
-Author: ltyzzz (Tycho)
-Author-email: ltyzzz2000@gmail.com
-Keywords: python,markdown,pdf,article,crawler
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # Article Crawler
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/article-crawler.svg)](https://pypi.org/project/article-crawler/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/article-crawler?label=PyPI%20downloads)](https://pypi.org/project/article-crawler/)
+[![](https://img.shields.io/github/v/release/ltyzzzxxx/article_crawler?display_name=tag)](https://github.com/ltyzzzxxx/article_crawler/releases/tag/v0.0.1)
+[![](https://img.shields.io/github/stars/ltyzzzxxx/article_crawler)](https://github.com/ltyzzzxxx/article_crawler)
+[![](https://img.shields.io/github/forks/ltyzzzxxx/article_crawler)](https://github.com/ltyzzzxxx/article_crawler)
+[![](https://img.shields.io/github/issues/ltyzzzxxx/article_crawler)](https://github.com/ltyzzzxxx/article_crawler/issues)
+[![](https://img.shields.io/badge/license-MIT%20-yellow.svg)](https://github.com/ltyzzzxxx/article_crawler/issues)
+
 ## ✨ Introduction
 
 Article Crawler is a package used to crawl articles with Markdown format from a specific webpage and store them locally in HTML / Markdown formats.
 
 ## 🚀 Quick Start
 
 1. Install through `pip`
 
     ```python
-    pip install article_crawler
+    pip install article-crawler
     ```
 2. Usage
 
     Usage: `python3 -m article_crawler -u [url] -t [type] -o [output_folder] -c [class_] -i [id]`
 
     ```
     Options:
```

### Comparing `article_crawler-0.0.1/article_crawler/__main__.py` & `article_crawler-0.0.2/article_crawler/__main__.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler/article_crawler.py` & `article_crawler-0.0.2/article_crawler/article_crawler.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler/csdn/csdn_crawler.py` & `article_crawler-0.0.2/article_crawler/csdn/csdn_crawler.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler/jianshu/jianshu_crawler.py` & `article_crawler-0.0.2/article_crawler/jianshu/jianshu_crawler.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler/juejin/juejin_crawler.py` & `article_crawler-0.0.2/article_crawler/juejin/juejin_crawler.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler/zhihu/zhihu_crawler.py` & `article_crawler-0.0.2/article_crawler/zhihu/zhihu_crawler.py`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/article_crawler.egg-info/SOURCES.txt` & `article_crawler-0.0.2/article_crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `article_crawler-0.0.1/setup.py` & `article_crawler-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A package for crawling markdown formatted articles from certain webpage and storing them locally.'
 
 # Setting up
 setup(
     name="article_crawler",
     version=VERSION,
     author="ltyzzz (Tycho)",
```

