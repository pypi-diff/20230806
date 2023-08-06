# Comparing `tmp/cyberdrop-dl-4.2.98.tar.gz` & `tmp/cyberdrop-dl-4.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.98.tar", last modified: Thu Jun 22 05:44:06 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.99.tar", last modified: Thu Jun 22 05:50:29 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.98.tar` & `cyberdrop-dl-4.2.99.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.184882 cyberdrop-dl-4.2.98/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-22 05:44:06.184882 cyberdrop-dl-4.2.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.176883 cyberdrop-dl-4.2.98/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.180883 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.180883 cyberdrop-dl-4.2.98/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.180883 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.180883 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.184882 cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:44:06.176883 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:44:06.000000 cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-22 05:44:06.184882 cyberdrop-dl-4.2.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:43:57.000000 cyberdrop-dl-4.2.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.462754 cyberdrop-dl-4.2.99/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.466754 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.466754 cyberdrop-dl-4.2.99/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:50:29.466754 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:50:29.000000 cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-22 05:50:29.470754 cyberdrop-dl-4.2.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:50:20.000000 cyberdrop-dl-4.2.99/setup.py
```

### Comparing `cyberdrop-dl-4.2.98/LICENSE` & `cyberdrop-dl-4.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/PKG-INFO` & `cyberdrop-dl-4.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.98
+Version: 4.2.99
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.98 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.99 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.98/README.md` & `cyberdrop-dl-4.2.99/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class ShareXCrawler:
     def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
-        self.limiter = AsyncLimiter(8, 1)
+        self.limiter = AsyncLimiter(3, 1)
 
         self.error_writer = error_writer
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for ShareX scraper"""
         assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
```

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.99/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.98
+Version: 4.2.99
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.98 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.99 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.98/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.99/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.98/setup.cfg` & `cyberdrop-dl-4.2.99/setup.cfg`

 * *Files identical despite different names*

