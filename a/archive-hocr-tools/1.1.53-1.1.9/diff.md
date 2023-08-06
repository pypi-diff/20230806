# Comparing `tmp/archive-hocr-tools-1.1.53.tar.gz` & `tmp/archive-hocr-tools-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archive-hocr-tools-1.1.53.tar", last modified: Sun Aug  6 00:11:05 2023, max compression
+gzip compressed data, was "/home/merlijn/archive/archive-hocr-tools/dist/tmpulyt8lyw/archive-hocr-tools-1.1.9.tar", last modified: Mon Oct  4 21:06:27 2021, max compression
```

## Comparing `archive-hocr-tools-1.1.53.tar` & `archive-hocr-tools-1.1.9.tar`

### file list

```diff
@@ -1,54 +1,34 @@
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.837344 archive-hocr-tools-1.1.53/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.53/COPYING
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.53/LICENSE.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       52 2023-06-30 20:45:00.000000 archive-hocr-tools-1.1.53/MANIFEST.in
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      732 2023-08-06 00:11:05.837344 archive-hocr-tools-1.1.53/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      833 2023-06-22 10:00:12.000000 archive-hocr-tools-1.1.53/README
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      833 2023-06-22 10:00:12.000000 archive-hocr-tools-1.1.53/README.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.820677 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      732 2023-08-06 00:11:05.000000 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      940 2023-08-06 00:11:05.000000 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/SOURCES.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2023-08-06 00:11:05.000000 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/dependency_links.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      196 2023-08-06 00:11:05.000000 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/requires.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2023-08-06 00:11:05.000000 archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/top_level.txt
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.830677 archive-hocr-tools-1.1.53/bin/
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    24267 2023-06-22 01:18:04.000000 archive-hocr-tools-1.1.53/bin/abbyy-to-hocr
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1305 2023-06-28 18:47:13.000000 archive-hocr-tools-1.1.53/bin/fts-text-annotate
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2196 2023-07-10 20:42:03.000000 archive-hocr-tools-1.1.53/bin/fts-text-match
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3326 2023-06-22 00:17:27.000000 archive-hocr-tools-1.1.53/bin/hocr-combine-stream
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    10459 2023-06-22 09:50:52.000000 archive-hocr-tools-1.1.53/bin/hocr-confidence-filter
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1556 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/bin/hocr-extract-page
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1411 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/bin/hocr-flatten-pages
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1814 2023-07-10 20:09:39.000000 archive-hocr-tools-1.1.53/bin/hocr-fold-chars
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2409 2022-08-12 00:45:40.000000 archive-hocr-tools-1.1.53/bin/hocr-lookup-check
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      551 2021-01-07 22:43:12.000000 archive-hocr-tools-1.1.53/bin/hocr-lookup-create
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      888 2021-01-08 12:38:34.000000 archive-hocr-tools-1.1.53/bin/hocr-lookup-reconstruct
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    36747 2023-08-06 00:07:21.000000 archive-hocr-tools-1.1.53/bin/hocr-pagenumbers
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1214 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/bin/hocr-split-pages
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      594 2021-10-15 21:39:26.000000 archive-hocr-tools-1.1.53/bin/hocr-text
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      826 2021-01-08 13:40:53.000000 archive-hocr-tools-1.1.53/bin/hocr-text-paragraphs
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    27998 2023-06-16 20:00:09.000000 archive-hocr-tools-1.1.53/bin/hocr-to-epub
--rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    13500 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/bin/pdf-to-hocr
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1552 2023-06-22 09:53:25.000000 archive-hocr-tools-1.1.53/conftest.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.830677 archive-hocr-tools-1.1.53/docs/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      638 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.53/docs/Makefile
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.830677 archive-hocr-tools-1.1.53/docs/source/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1961 2022-04-16 05:05:04.000000 archive-hocr-tools-1.1.53/docs/source/conf.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4126 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.53/docs/source/index.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.53/docs/source/parse.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       83 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.53/docs/source/searching.rst
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      100 2021-10-05 09:04:50.000000 archive-hocr-tools-1.1.53/docs/source/text.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.834011 archive-hocr-tools-1.1.53/hocr/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2023-06-20 17:49:56.000000 archive-hocr-tools-1.1.53/hocr/__init__.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2023-08-06 00:11:05.834011 archive-hocr-tools-1.1.53/hocr/data/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     6951 2023-01-30 22:06:33.000000 archive-hocr-tools-1.1.53/hocr/data/abbyy-lang-map.csv
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    11418 2023-07-10 20:40:45.000000 archive-hocr-tools-1.1.53/hocr/fts.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    11330 2023-06-22 00:14:48.000000 archive-hocr-tools-1.1.53/hocr/parse.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3925 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/hocr/searching.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4886 2022-08-12 00:45:40.000000 archive-hocr-tools-1.1.53/hocr/text.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3791 2023-06-22 00:16:57.000000 archive-hocr-tools-1.1.53/hocr/util.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       23 2023-08-06 00:07:53.000000 archive-hocr-tools-1.1.53/hocr/version.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       61 2023-06-16 20:10:53.000000 archive-hocr-tools-1.1.53/pyproject.toml
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        0 2023-06-22 00:09:17.000000 archive-hocr-tools-1.1.53/requirements.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2023-08-06 00:11:05.837344 archive-hocr-tools-1.1.53/setup.cfg
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1924 2023-06-23 15:18:55.000000 archive-hocr-tools-1.1.53/setup.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      690 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      609 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/requires.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        5 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/top_level.txt
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/bin/
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)    23972 2021-08-06 18:07:47.000000 archive-hocr-tools-1.1.9/bin/abbyy-to-hocr
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1305 2021-02-03 13:57:49.000000 archive-hocr-tools-1.1.9/bin/fts-text-annotate
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1254 2021-06-28 13:26:24.000000 archive-hocr-tools-1.1.9/bin/fts-text-match
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     3037 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-combine-stream
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1565 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-extract-page
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     1831 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/bin/hocr-fold-chars
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2420 2021-01-08 15:17:51.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-check
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      551 2021-01-07 22:43:12.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-create
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      888 2021-01-08 12:38:34.000000 archive-hocr-tools-1.1.9/bin/hocr-lookup-reconstruct
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)     2562 2021-10-04 20:51:43.000000 archive-hocr-tools-1.1.9/bin/hocr-text
+-rwxr-xr-x   0 merlijn   (1000) merlijn   (1000)      826 2021-01-08 13:40:53.000000 archive-hocr-tools-1.1.9/bin/hocr-text-paragraphs
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/hocr/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       81 2021-06-28 13:26:24.000000 archive-hocr-tools-1.1.9/hocr/__init__.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     7765 2021-06-28 13:54:43.000000 archive-hocr-tools-1.1.9/hocr/fts.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8288 2021-10-04 20:51:43.000000 archive-hocr-tools-1.1.9/hocr/parse.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3908 2021-06-28 13:54:43.000000 archive-hocr-tools-1.1.9/hocr/searching.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4946 2021-06-28 13:12:11.000000 archive-hocr-tools-1.1.9/hocr/text.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2211 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/hocr/util.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       22 2021-10-04 21:05:07.000000 archive-hocr-tools-1.1.9/hocr/version.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/COPYING
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2021-06-28 12:40:44.000000 archive-hocr-tools-1.1.9/LICENSE.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      483 2020-10-31 10:07:13.000000 archive-hocr-tools-1.1.9/README
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       61 2021-10-04 20:43:57.000000 archive-hocr-tools-1.1.9/pyproject.toml
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/setup.cfg
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1451 2021-10-04 21:05:30.000000 archive-hocr-tools-1.1.9/setup.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      690 2021-10-04 21:06:27.000000 archive-hocr-tools-1.1.9/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `archive-hocr-tools-1.1.53/COPYING` & `archive-hocr-tools-1.1.9/COPYING`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/LICENSE.txt` & `archive-hocr-tools-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/PKG-INFO` & `archive-hocr-tools-1.1.9/archive_hocr_tools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: archive-hocr-tools
-Version: 1.1.53
+Version: 1.1.9
 Summary: hOCR (streaming) parsers and writers
 Home-page: https://github.com/internetarchive/archive-hocr-tools
-Download-URL: https://github.com/internetarchive/archive-hocr-tools/archive/1.1.53.tar.gz
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
+Download-URL: https://github.com/internetarchive/archive-hocr-tools/archive/1.1.9.tar.gz
 Keywords: hOCR,Internet Archive
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Provides-Extra: epub
-Provides-Extra: pdf
-Provides-Extra: pagenumber
 License-File: LICENSE.txt
 License-File: COPYING
+
+UNKNOWN
+
```

### Comparing `archive-hocr-tools-1.1.53/archive_hocr_tools.egg-info/PKG-INFO` & `archive-hocr-tools-1.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: archive-hocr-tools
-Version: 1.1.53
+Version: 1.1.9
 Summary: hOCR (streaming) parsers and writers
 Home-page: https://github.com/internetarchive/archive-hocr-tools
-Download-URL: https://github.com/internetarchive/archive-hocr-tools/archive/1.1.53.tar.gz
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
+Download-URL: https://github.com/internetarchive/archive-hocr-tools/archive/1.1.9.tar.gz
 Keywords: hOCR,Internet Archive
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Provides-Extra: epub
-Provides-Extra: pdf
-Provides-Extra: pagenumber
 License-File: LICENSE.txt
 License-File: COPYING
+
+UNKNOWN
+
```

### Comparing `archive-hocr-tools-1.1.53/bin/abbyy-to-hocr` & `archive-hocr-tools-1.1.9/bin/abbyy-to-hocr`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
 
-from xml.etree import ElementTree
+from lxml import etree
 
 from xml.sax.saxutils import escape as xmlescape
 
-from hocr.util import open_if_required, iterparse_tags, register_and_nuke_xhtml_namespace, elem_tostring
+from hocr.util import open_if_required
 
 import numpy as np
 
 import pkg_resources
 import csv
 import io
 
@@ -27,15 +27,15 @@
 # X Parse exact abbyy software version, other attributes, move those to hOCR files
 # / Test with different abbyy xml versions
 # X Test with unicode languages - also for writing direction and such -> maybe charParams.wordLeftMost can be used (if the first char is not wordLeftMost...)
 # X use <line fs="8.5" ...> (etc) for x_fsize for words?
 # X Add scan_res (from image or item metadata? meh)
 # X word confidence wordFromDictionary (?) + char confs?, 'suspicious' attribute
 # - Add lots of (strict) assertions to prevent silent bugs (unknown areas/types, etc)
-# - ocr_page image property - point to the some url for convenience (where do we
+# - ocr_page image property - point to the some url for convience (where do we
 #   get it from?)
 
 # Tested versions:
 #
 # - 'ABBYY FineReader 11.0 (Extended OCR)'
 # - 'ABBYY FineReader 11.0'
 # - 'ABBYY FineReader 9.0'
@@ -145,15 +145,15 @@
     Returns the version (producer) and the schema/namespace as a tuple.
     """
     fp = open_if_required(file_path)
 
     tags = ('{%s}document' % FINEREADER_6_SCHEMA,
             '{%s}document' % FINEREADER_11_SCHEMA)
 
-    doc = iterparse_tags(fp, tag=tags,
+    doc = etree.iterparse(fp, tag=tags,
                           events=('start',))
     for act, elem in doc:
         if elem.tag[-8:] == 'document':
             schema = elem.tag[:-8][1:-1] # Remove document, '{' and '}'
             producer = elem.attrib['producer']
             elem.clear()
             return producer, schema
@@ -170,19 +170,19 @@
     streaming manner.
 
     Args:
     * file_path (str): Path to abbyy file (if gzip, will get decompressed on the
                        fly)
 
     Returns:
-    Iterator returning a ElementTree.Element of the page.
+    Iterator returning a etree.Element of the page.
     """
     fp = open_if_required(file_path)
 
-    doc = iterparse_tags(fp, tag='{' + schema +'}page')
+    doc = etree.iterparse(fp, tag='{' + schema +'}page')
     for act, elem in doc:
         if elem.tag[-4:] == 'page':
             page = elem
             yield page
 
         elem.clear()
 
@@ -190,35 +190,35 @@
 def abbyy_process_text_block(pageno, NS, block, parent_block, dpi):
     """
     Process a <text> block.
 
     Args:
     * pageno (int): page number, zero indexed
     * NS (str): namespace of this XML as returned by abbyy_get_metadata
-    * block (ElementTree.Element): Abbyy XML block to process
-    * parent_block (ElementTree.Element): parent (target) element to add elements to.
+    * block (etree.Element): Abbyy XML block to process
+    * parent_block (etree.Element): parent (target) element to add elements to.
     * dpi (int): DPI/PPI of the page
     """
     # TODO: check writing direction correctness (do we want it per paragraph,
     # too?) - and then only report on the different writing directions per word
     # (if they are different from paragraph)
 
-    for par in block.findall('./x:text/x:par', namespaces={'x': NS}):
+    for par in block.xpath('./x:text/x:par', namespaces={'x': NS}):
         par_has_text = False
-        parelem = ElementTree.Element('p', attrib={'class': 'ocr_par'})
+        parelem = etree.Element('p', attrib={'class': 'ocr_par'})
 
         parelem.attrib['id'] = get_id(pageno, 'par')
 
         leftm = None
         topm = None
         rightm = None
         bottomm = None
 
-        for line in par.findall('./x:line', namespaces={'x': NS}):
-            children = list(line)
+        for line in par.xpath('./x:line', namespaces={'x': NS}):
+            children = line.getchildren()
 
             if len(children) < 1:
                 # If the line has no children, it does not have a formatting
                 # element and seems to be always empty, so let's skip it.
                 continue
 
             formatting = children[0] # XXX: hacky
@@ -235,15 +235,15 @@
                 bottomm = bottom
             else:
                 leftm = min(left, leftm)
                 topm = min(top, topm)
                 rightm = max(right, rightm)
                 bottomm = max(bottom, bottomm)
 
-            lineelem = ElementTree.Element('span', attrib={'class': 'ocr_line'})
+            lineelem = etree.Element('span', attrib={'class': 'ocr_line'})
 
             if 'lang' in formatting.attrib and formatting.attrib['lang'] != '':
                 mapped_lang = LANG_DATA.get(formatting.attrib['lang'], None)
                 if not mapped_lang:
                     raise Exception('Cannot map Abbyy language: %s', formatting.attrib['lang'])
                 lineelem.attrib['lang'] = mapped_lang
                 lineelem.attrib['{http://www.w3.org/XML/1998/namespace}lang'] = mapped_lang
@@ -312,15 +312,15 @@
     else:
         kv['ppageno'] = '0'
     kv['image'] = 'https://archive.org/todo' # TODO: some image path?
 
     dpi = int(abbyy_page.attrib['resolution'])
     kv['scan_res'] = '%d %d' % (dpi, dpi)
 
-    pageelem = ElementTree.Element('div', attrib={'class': 'ocr_page',
+    pageelem = etree.Element('div', attrib={'class': 'ocr_page',
         'id': page_id(pageno),
         'title': assemble_hocr_title_element(kv),
         })
 
     NS = schema
 
     # <xs:enumeration value="Text"/>
@@ -328,65 +328,65 @@
     # <xs:enumeration value="Picture"/>
     # <xs:enumeration value="Barcode"/>
     # <xs:enumeration value="Separator"/>
     # <xs:enumeration value="SeparatorsBox"/>
     # <xs:enumeration value="Checkmark"/>
     # <xs:enumeration value="GroupCheckmark"/>
     # Let's skip Separator etc atm
-    for block in abbyy_page.findall('./x:block',
+    for block in abbyy_page.xpath('./x:block',
                                   namespaces={'x': NS}):
         if block.attrib['blockType'] == 'Picture':
             # TODO: Can a Picture contain multiple <region>s?
             # Use ocr_photo, since ocr_image suggests the image is probably
             # better expressed in vector graphics, and we don't know.
-            blockelem = ElementTree.Element('div', attrib={'class': 'ocr_photo'})
+            blockelem = etree.Element('div', attrib={'class': 'ocr_photo'})
             kv = {}
             kv['bbox'] = kv['bbox'] = [block.attrib['l'], block.attrib['t'], block.attrib['r'], block.attrib['b']]
             blockelem.attrib['title'] = assemble_hocr_title_element(kv)
             blockelem.attrib['id'] = get_id(pageno, 'photo')
             pageelem.append(blockelem)
         elif block.attrib['blockType'] == 'Table':
             # XXX: div, span or table? https://groups.google.com/g/ocropus/c/-s33xn9fBGY
             #       <table class="ocr_table"> ... </table>
             #       or
             #       <span class="ocr_table"><table> ... </table></table>
-            tableelem = ElementTree.Element('table', attrib={'class': 'ocr_table'})
-            #tableelem = ElementTree.Element('div', attrib={'class': 'ocr_table'})
+            tableelem = etree.Element('table', attrib={'class': 'ocr_table'})
+            #tableelem = etree.Element('div', attrib={'class': 'ocr_table'})
             kv = {}
             kv['bbox'] = [block.attrib['l'], block.attrib['t'], block.attrib['r'], block.attrib['b']]
             tableelem.attrib['title'] = assemble_hocr_title_element(kv)
             tableelem.attrib['id'] = get_id(pageno, 'table')
 
-            for row in block.findall('./x:row', namespaces={'x': NS}):
-                rowelem = ElementTree.Element('tr')
-                for cell in row.findall('./x:cell', namespaces={'x': NS}):
-                    cellelem = ElementTree.Element('td')
+            for row in block.xpath('./x:row', namespaces={'x': NS}):
+                rowelem = etree.Element('tr')
+                for cell in row.xpath('./x:cell', namespaces={'x': NS}):
+                    cellelem = etree.Element('td')
                     abbyy_process_text_block(pageno, NS, cell, cellelem, dpi)
                     rowelem.append(cellelem)
 
                 tableelem.append(rowelem)
             pageelem.append(tableelem)
         elif block.attrib['blockType'] == 'Separator':
-            separatorelem = ElementTree.Element('div', attrib={'class': 'ocr_separator'})
+            separatorelem = etree.Element('div', attrib={'class': 'ocr_separator'})
             kv = {}
             kv['bbox'] = [block.attrib['l'], block.attrib['t'], block.attrib['r'], block.attrib['b']]
             separatorelem.attrib['title'] = assemble_hocr_title_element(kv)
             separatorelem.attrib['id'] = get_id(pageno, 'separator')
             pageelem.append(separatorelem)
         elif block.attrib['blockType'] == 'SeparatorsBox':
-            separatorelem = ElementTree.Element('div', attrib={'class': 'ocr_separator'})
+            separatorelem = etree.Element('div', attrib={'class': 'ocr_separator'})
             kv = {}
             kv['bbox'] = [block.attrib['l'], block.attrib['t'], block.attrib['r'], block.attrib['b']]
             separatorelem.attrib['title'] = assemble_hocr_title_element(kv)
             separatorelem.attrib['id'] = get_id(pageno, 'separator')
             pageelem.append(separatorelem)
         elif block.attrib['blockType'] == 'Text':
             kv = {}
             kv['bbox'] = [block.attrib['l'], block.attrib['t'], block.attrib['r'], block.attrib['b']]
-            blockelem = ElementTree.Element('div', attrib={'class': 'ocr_carea'})
+            blockelem = etree.Element('div', attrib={'class': 'ocr_carea'})
             blockelem.attrib['title'] = assemble_hocr_title_element(kv)
             blockelem.attrib['id'] = get_id(pageno, 'block')
 
             abbyy_process_text_block(pageno, NS, block, blockelem, dpi)
             pageelem.append(blockelem)
         else:
             # Let's error for now on other blockTypes
@@ -506,35 +506,35 @@
     """
     Process characters in a <line> element
 
     Args:
 
     * pageno (int): Page number, zero indexed
     * NS (str): namespace of this XML as returned by abbyy_get_metadata
-    * line (ElementTree.Element): line element to process
-    * lineelem (ElementTree.Element): target element
-    * formatting (ElementTree.Element): <formatting> element of the line
+    * line (etree.Element): line element to process
+    * lineelem (etree.Element): target element
+    * formatting (etree.Element): <formatting> element of the line
     * line_fontsize (int): font size of the line
 
     Returns:
 
-    Tuple of the last word element (ElementTree.Element) and a list of all the
+    Tuple of the last word element (etree.Element) and a list of all the
     bounding boxes of the characters encountered.
     """
-    wordelem = ElementTree.Element('span', attrib={'class': 'ocrx_word'})
+    wordelem = etree.Element('span', attrib={'class': 'ocrx_word'})
     charelem = None
     first_word = True
     word_start = True
     word_dict = False
 
     wordchar_bboxes = []
     wordchar_confs = []
     wordchar_suspicious = []
     all_wordchar_bboxes = []
-    for char in line.findall('./x:formatting/x:charParams', namespaces={'x': NS}):
+    for char in line.xpath('./x:formatting/x:charParams', namespaces={'x': NS}):
         # Abbyy sometimes has charParams without a character, let's just ignore
         # those all together (and hope they don't mess up our
         # wordFirst/wordStart etc detection)
         if char.text is None:
             continue
 
         # wordFirst for 11, wordStart for 6, 8, 9
@@ -551,15 +551,15 @@
                     if 'dir' in wordelem.attrib and wordelem.attrib['dir'] == 'rtl':
                         wordelem[-1].text += chr(0x200e)
 
                     _gather_word_data(pageno, wordelem, wordchar_bboxes,
                             wordchar_confs, wordchar_suspicious, word_dict,
                             formatting, line_fontsize)
 
-                wordelem = ElementTree.Element('span',
+                wordelem = etree.Element('span',
                                          attrib={'class': 'ocrx_word'})
 
             word_start = True
             wordchar_bboxes = []
             wordchar_confs = []
             wordchar_suspicious = []
 
@@ -569,15 +569,15 @@
         if 'wordLeftMost' in char.attrib and char.attrib['wordLeftMost'] == '1':
             # TODO: clean up this logic some (what if wordLeftMost doesn't exist)
             if word_start:
                 wordelem.attrib['dir'] = 'ltr'
             else:
                 wordelem.attrib['dir'] = 'rtl'
 
-        charelem = ElementTree.Element('span', attrib={'class': 'ocrx_cinfo'})
+        charelem = etree.Element('span', attrib={'class': 'ocrx_cinfo'})
         charelem.text = char.text
 
         if 'charConfidence' in char.attrib:
             conf = float(char.attrib['charConfidence'])
         else:
             conf = None
 
@@ -662,26 +662,24 @@
   </head>
   <body>
 ''' % xmlescape(producer))
 
     it = abbyy_page_iterator(filename, schema)
     for idx, p in enumerate(it):
         hocr_page = abbyy_page_to_hocr_page(p, schema, pageno=idx)
-        if hasattr(ElementTree, 'indent'):
-            ElementTree.indent(hocr_page, space=' ' * 2)
-        s = elem_tostring(hocr_page, short_empty_elements=True).decode('utf-8')
+        s = etree.tostring(hocr_page, pretty_print=True, method='xml',
+                           encoding='utf-8').decode('utf-8')
         print(s)
     print('''  </body>
 </html>
 ''')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Abbyy XML to character '
                                                  'based hOCR converter')
     parser.add_argument('-f', '--infile', help='Input file',
                         type=str, default=None)
     args = parser.parse_args()
     load_langs()
 
-    register_and_nuke_xhtml_namespace()
     process_files(args.infile)
```

### Comparing `archive-hocr-tools-1.1.53/bin/fts-text-annotate` & `archive-hocr-tools-1.1.9/bin/fts-text-annotate`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-combine-stream` & `archive-hocr-tools-1.1.9/bin/hocr-combine-stream`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
 from glob import glob
 
-from xml.etree import ElementTree
-ElementTree.register_namespace('', 'http://www.w3.org/1999/xhtml')
+from lxml import etree
 
 from hocr.parse import hocr_page_iterator
-from hocr.util import register_and_nuke_xhtml_namespace, get_header_footer, \
-        HOCR_SCHEMA, elem_tostring
+from hocr.util import get_header_footer
 
 
 def process_files(files_to_process):
     top, bottom = get_header_footer(files_to_process[0])
 
     sys.stdout.buffer.write(top)
 
@@ -25,64 +23,57 @@
 
             page.attrib['id'] = 'page_%.06d' % page_no
             block_no = 0
             par_no = 0
             line_no = 0
             word_no = 0
 
-            blocks = page.findall("*[@class='ocr_carea']")
+            blocks = page.xpath("*[@class='ocr_carea']")
             for block in blocks:
                 block.attrib['id'] = 'block_%.06d_%.06d' % (page_no,
                                                             block_no)
 
-                paragraphs = block.findall("*[@class='ocr_par']")
+                paragraphs = block.xpath("*[@class='ocr_par']")
                 for par in paragraphs:
                     par.attrib['id'] = 'par_%.06d_%.06d' % (page_no,
                                                             par_no)
 
-                    for line in list(par):
+                    for line in par.getchildren():
                         line.attrib['id'] = 'line_%.06d_%.06d' % (page_no,
                                                                   line_no)
 
-                        words = line.findall("*[@class='ocrx_word']")
+                        words = line.xpath("*[@class='ocrx_word']")
                         for word in words:
                             word.attrib['id'] = 'word_%.06d_%.06d' % \
                                     (page_no, word_no)
 
                             word_no += 1
 
                         line_no += 1
 
                     par_no += 1
 
                 block_no += 1
 
             page_no += 1
 
-            page.tail = None
-            s = elem_tostring(page).decode('utf-8')
-
+            s = etree.tostring(page, pretty_print=True, method='xml',
+                               encoding='utf-8').decode('utf-8')
             # Let's Remove the xmlns in the div.
-            # Yes, this is ugly, but we used to do it, so let's stay
-            # compatible with the lxml code. Also, I don't know a more clean way
-            # to do this.
-            # Let's also add two spaces for indentation for the first
+            # Yes, this is horrible, but cleanup_namespaces doesn't help
+            # since as far as tostring knows, this is the root.
+            # Let's also add two spaces for indendation for the first
             # page, and one for all the other pages.
-
-            # XXX: Can we remove this attribute perhaps from the ocr_page?
             if page_no == 1:
                 s = '  ' + \
                     s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
             else:
                 s = ' ' + \
                     s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
 
-            # Start on a new line
-            s += '\n'
-
             s = s.encode('utf-8')
             sys.stdout.buffer.write(s)
 
     sys.stdout.buffer.write(bottom)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Combine hOCR files '
@@ -90,14 +81,14 @@
     parser.add_argument('-g', '--glob', help='Glob of files to parse',
                         type=str, default=None)
     args = parser.parse_args()
 
     files_to_process = glob(args.glob)
 
     if not len(files_to_process):
+        import sys
         print('No files to process!', file=sys.stderr)
         sys.exit(1)
 
     files_to_process = sorted(files_to_process)
 
-    register_and_nuke_xhtml_namespace()
     process_files(files_to_process)
```

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-extract-page` & `archive-hocr-tools-1.1.9/bin/hocr-extract-page`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 
 import sys
 import argparse
 
+from lxml import etree
+
 from hocr.searching import hocr_load_lookup_table, hocr_lookup_page_by_dat
 from hocr.parse import hocr_page_iterator
-from hocr.util import open_if_required, get_header_footer, elem_tostring, register_and_nuke_xhtml_namespace
+from hocr.util import open_if_required, get_header_footer
 
 def process_file(filepath, pageno, tablepath):
     fd = open_if_required(filepath)
     top, bottom = get_header_footer(fd)
 
     sys.stdout.buffer.write(top)
 
@@ -20,15 +22,16 @@
         dat = lookup_table[pageno]
         page = hocr_lookup_page_by_dat(fp, dat)
     else:
         for idx, page in enumerate(hocr_page_iterator(fd)):
             if idx == pageno:
                 break
 
-    s = elem_tostring(page).decode('utf-8')
+    s = etree.tostring(page, pretty_print=True, method='xml',
+                       encoding='utf-8').decode('utf-8')
 
     s = ' ' + s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
     s = s.encode('utf-8')
     sys.stdout.buffer.write(s)
 
     sys.stdout.buffer.write(bottom)
 
@@ -39,10 +42,9 @@
                         type=str, default=None)
     parser.add_argument('-t', '--table', help='Table to use',
                         type=str, default=None)
     parser.add_argument('-p', '--page', help='Page number to extract (zero based)',
                         type=int, default=None)
     args = parser.parse_args()
 
-    register_and_nuke_xhtml_namespace()
     process_file(args.infile, args.page, args.table)
```

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-flatten-pages` & `archive-hocr-tools-1.1.9/bin/hocr-fold-chars`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 #!/usr/bin/env python
 
 import sys
-import re
-
 import argparse
 
+from lxml import etree
+
 from hocr.parse import hocr_page_iterator
-from hocr.util import open_if_required, get_header_footer, elem_tostring, register_and_nuke_xhtml_namespace
+from hocr.util import open_if_required, get_header_footer
 
-rem = re.compile("<div class=['\"]ocr_page['\"].*>")
 
-def process_file(filepath):
-    fd = open_if_required(filepath)
+def process_files(infile):
+    fd = open_if_required(infile)
     top, bottom = get_header_footer(fd)
 
-    # Idea: strip ending for first page, add ending to last page?
-
-    first = True
+    sys.stdout.buffer.write(top)
 
-    print(top.decode('utf-8'))
-    for pageno, page in enumerate(hocr_page_iterator(fd)):
+    page_no = 0
 
-        s = elem_tostring(page).decode('utf-8')
-
-        s = ' ' + s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
-
-        if first:
-            # Remove the last </div> of the first page
-            idx = s.rindex('</div>')
-            s = s[:idx]
-            first = False
+    fd.seek(0)
+    for page in hocr_page_iterator(fd):
+        words = page.xpath(".//*[@class='ocrx_word']")
+        for word in words:
+            chars = word.xpath("*[@class='ocrx_cinfo']")
+            txt = ''
+            for char in chars:
+                txt += char.text
+
+            ch = word.getchildren()
+            for c in ch:
+                word.remove(c)
+            word.text = txt
+
+        s = etree.tostring(page, pretty_print=True, method='xml',
+                           encoding='utf-8').decode('utf-8')
+        # Let's Remove the xmlns in the div.
+        # Yes, this is horrible, but cleanup_namespaces doesn't help
+        # since as far as tostring knows, this is the root.
+        # Let's also add two spaces for indendation for the first
+        # page, and one for all the other pages.
+        if page_no == 1:
+            s = '  ' + \
+                s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
         else:
-            # XXX: This assumes that <div class="ocr_page"> is the only html
-            # element on the line (!)
-            s = re.sub(rem, '', s, count=1)
-
-        print(s)
+            s = ' ' + \
+                s.replace(' xmlns="http://www.w3.org/1999/xhtml"', '')
 
-    print(bottom.decode('utf-8'))
+        s = s.encode('utf-8')
+        sys.stdout.buffer.write(s)
 
+    sys.stdout.buffer.write(bottom)
 
 if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='hOCR page flatten (combine several pages into one page)')
-    parser.add_argument('-f', '--infile', help='Filename to read',
+    parser = argparse.ArgumentParser(description='Fold character-based hOCR '
+                                                 'into word-based hOCR')
+    parser.add_argument('-f', '--infile', help='Input file',
                         type=str, default=None)
     args = parser.parse_args()
 
-    register_and_nuke_xhtml_namespace()
-    process_file(args.infile)
+    process_files(args.infile)
```

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-lookup-check` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-check`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 
+import sys
 import argparse
 
 from hocr.parse import hocr_page_to_word_data_fast
 from hocr.searching import hocr_load_lookup_table, hocr_lookup_page_by_dat, \
         hocr_lookup_by_plaintext_offset
 from hocr.util import open_if_required
 from hocr.text import hocr_paragraph_text
```

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-lookup-create` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-create`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-lookup-reconstruct` & `archive-hocr-tools-1.1.9/bin/hocr-lookup-reconstruct`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/bin/hocr-text-paragraphs` & `archive-hocr-tools-1.1.9/bin/hocr-text-paragraphs`

 * *Files identical despite different names*

### Comparing `archive-hocr-tools-1.1.53/hocr/parse.py` & `archive-hocr-tools-1.1.9/hocr/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import gzip
 import re
 
-from .util import open_if_required, iterparse_tags, HOCR_SCHEMA
+from lxml import etree
+
+from .util import open_if_required
 
 
 WRITING_DIRECTION_UNSPECIFIED = 0
 WRITING_DIRECTION_LEFT_TO_RIGHT = 1
 WRITING_DIRECTION_RIGHT_TO_LEFT = 2
 WRITING_DIRECTION_TOP_TO_BOTTOM = 3
 
@@ -28,25 +30,29 @@
 
     Args:
 
     * fd_or_path: open file to operate on, or a path (str).
 
     Returns:
 
-    * Iterator returning a ElementTree.Element hOCR page.
+    * Iterator returning a etree.Element hOCR page.
     """
     fp = open_if_required(fd_or_path)
 
     # Seek to start
-    fp.seek(0)
-
-    tags = {HOCR_SCHEMA + 'div', 'div'}
-    doc = iterparse_tags(fp, tag=tags)
+    # TODO: We should make tools call seek if they should, rather than having
+    # this function call seek()
+    # Do not remove this for now
+    #fp.seek(0)
+
+    # TODO: Add gzip loading, specify what file_like should be (I suggest just
+    # file descriptor or just path)
+    doc = etree.iterparse(fp, tag='{http://www.w3.org/1999/xhtml}div')
     for act, elem in doc:
-        if elem.attrib['class'] == 'ocr_page':
+        if elem.tag[-3:] == 'div' and elem.attrib['class'] == 'ocr_page':
             page = elem
             yield page
 
             elem.clear()
 
 
 def hocr_page_get_dimensions(hocr_page):
@@ -100,15 +106,15 @@
     Args:
 
     * hocr_page: a single hocr_page as returned by hocr_page_iterator
     * (optional) scaler: a scalar to scale font sizes by
 
     Returns:
 
-    A list of paragraphs, each paragraph containing a list of lines, and each
+    A list of paragraph, each paragraph containing a list of lines, and each
     line containing a list of words, plus properties.
 
     Paragraphs have the following attributes:
 
     * `'lines'`: the lines that form this paragraph
 
     Lines have the following attributes:
@@ -123,23 +129,22 @@
     * `'bbox'`: bounding box (tuple of 4 floats)
     * `'fontsize'`: fontsize as a float, or 0.
     * `'writing_direction'`: See WRITING_DIRECTION_* constants
     * `'confidence'`: word confidence, 0 - 100
     """
     paragraphs = []
 
-    for par in hocr_page.findall('.//*[@class="ocrx_block"]') + hocr_page.findall('.//*[@class="ocr_par"]'):
+    for par in hocr_page.xpath('.//*[@class="ocr_par"]'):
         paragraph_data = {'lines': []}
 
         paragraph_writing_direction = WRITING_DIRECTION_UNSPECIFIED
         if 'dir' in par.attrib:
             paragraph_writing_direction = wdmap[par.attrib['dir']]
 
-        # We assume that the direct children are all the lines
-        for line in list(par):
+        for line in par.getchildren():
             line_data = {}
 
             linebox = BBOX_REGEX.search(line.attrib['title']).group(1).split()
             baseline = BASELINE_REGEX.search(line.attrib['title'])
             if baseline is not None:
                 baseline = baseline.group(1).split()
             else:
@@ -148,46 +153,28 @@
             linebox = [float(i) for i in linebox]
             baseline = [float(i) for i in baseline]
 
             line_data['bbox'] = linebox
             line_data['baseline'] = baseline
 
             word_data = []
-            for word in line.findall('.//*[@class="ocrx_word"]'):
+            for word in line.xpath('.//*[@class="ocrx_word"]'):
                 rawtext = ''
                 wordbased = True
-                for char in word.findall('.//*[@class="ocrx_cinfo"]'):
+                for char in word.xpath('.//*[@class="ocrx_cinfo"]'):
                     rawtext += char.text
                     wordbased = False
 
                 if wordbased:
-                    wword = word
-                    # Words may contains additional nodes like <em>
-                    while True:
-                        children = list(wword)
-                        if len(children) == 0:
-                            break
-
-                        if len(children) > 1:
-                            raise ValueError('Not character based but word has multiple children?')
-
-                        wword = children[0]
-
-                    rawtext = wword.text
-
-                    if wword.text is None:
-                        raise ValueError('Word with no text value?')
+                    rawtext = word.text
 
                 box = BBOX_REGEX.search(word.attrib['title']).group(1).split()
                 box = [float(i) for i in box]
 
-                conf = None
-                m = X_WCONF_REGEX.search(word.attrib['title'])
-                if m:
-                    conf = int(m.group(1).split()[0])
+                conf = int(X_WCONF_REGEX.search(word.attrib['title']).group(1).split()[0])
 
                 f_sizeraw = X_FSIZE_REGEX.search(word.attrib['title'])
                 if f_sizeraw:
                     x_fsize = float(f_sizeraw.group(1))
                     x_fsize *= scaler
                 else:
                     x_fsize = 0. # Will get fixed later on, in pdfrenderer at least
@@ -207,67 +194,14 @@
             #print('Line words:', word_data)
             paragraph_data['lines'].append(line_data)
 
         paragraphs.append(paragraph_data)
 
     return paragraphs
 
-def hocr_page_to_photo_data(hocr_page, minimum_page_area_pct=10):
-    """
-    Parses a single hocr_page into photo data.
-
-    Args:
-
-    * hocr_page: a single hocr_page as returned by hocr_page_iterator
-    * (optional) minimum_page_area_pct: a minimum percentage of the page area the picture should inhabit
-
-    Returns:
-
-    A list of bounding boxes where photos were found
-    """
-
-    # Get the actual boxes from the page
-    photo_boxes = []
-    for photo in hocr_page.findall('.//*[@class="ocr_photo"]'):
-        box = BBOX_REGEX.search(photo.attrib['title']).group(1).split()
-        box = [float(i) for i in box]
-        photo_boxes.append(box)
-
-    # Helper function to determine if there are nested boxes
-    def box_contains_box(box_a, box_b):
-        return box_a[0] <= box_b[0] and box_a[1] <= box_b[1] \
-           and box_a[2] >= box_b[2] and box_a[3] >= box_b[3]
-
-    # Clean up the box data a bit
-    cleaned_photo_boxes = list(photo_boxes)
-    dim = hocr_page_get_dimensions(hocr_page)
-    area_page = dim[0]*dim[1]
-    for box_a in photo_boxes:
-        # Image must cover at least minimum_page_area_pct of page
-        width, height = box_a[2]-box_a[0], box_a[3]-box_a[1]
-        area_box = width*height
-        if area_box < area_page*(minimum_page_area_pct/100.):
-            try:
-                cleaned_photo_boxes.remove(box_a)
-                #print("Box %s is too small, removing" % (box_a))
-            except: # Already removed
-                pass
-
-        # Nested boxes are redundant
-        for box_b in photo_boxes:
-            if box_a == box_b:
-                continue
-            if box_contains_box(box_a, box_b):
-                try:
-                    cleaned_photo_boxes.remove(box_b)
-                    #print("Box %s is fully inside box %s, removing" % (box_b, box_a))
-                except: # Already removed
-                    pass
-
-    return cleaned_photo_boxes
 
 def get_title_attrs(title):
     # Assume Tesseract generated hOCR, where every ';' has a space after it
     sub_title = title.split('; ')
     box = None
     conf = None
 
@@ -310,55 +244,40 @@
     * `'bbox'`: bounding box (tuple of 4 floats)
     * `'confidence'`: word confidence, 0 - 100
     """
     paragraphs = []
 
     has_ocrx_cinfo = 0
 
-    for par in hocr_page.findall('.//*[@class="ocr_par"]') + hocr_page.findall('.//*[@class="ocrx_block"]'):
+    for par in hocr_page.xpath('.//*[@class="ocr_par"]'):
         paragraph_data = {'lines': []}
 
-        # We assume that the direct children are all the lines
-        for line in list(par):
+        for line in par.getchildren():
             line_data = {}
 
             word_data = []
-            for word in line.findall('.//*[@class="ocrx_word"]'):
+            for word in line.xpath('.//*[@class="ocrx_word"]'):
                 title = word.attrib['title']
 
                 box, conf = get_title_attrs(title)
 
                 rawtext = ''
                 wordbased = True
                 if has_ocrx_cinfo < 2:
-                    for char in word.findall('.//*[@class="ocrx_cinfo"]'):
+                    for char in word.xpath('.//*[@class="ocrx_cinfo"]'):
                         rawtext += char.text
                         wordbased = False
                         has_ocrx_cinfo = 1
 
                 if has_ocrx_cinfo == 0:
                     has_ocrx_cinfo = 2
 
                 if wordbased:
-                    # Words may contains additional nodes like <em>
-                    while True:
-                        children = list(word)
-                        if len(children) == 0:
-                            break
-
-                        if len(children) > 1:
-                            raise ValueError('Not character based but word has multiple children?')
-
-                        word = children[0]
-
                     rawtext = word.text
 
-                    if word.text is None:
-                        raise ValueError('Word with no text value?')
-
                 word_data.append({'bbox': box, 'text': rawtext,
                                   'confidence': conf})
 
 
             line_data['words'] = word_data
             paragraph_data['lines'].append(line_data)
```

### Comparing `archive-hocr-tools-1.1.53/hocr/searching.py` & `archive-hocr-tools-1.1.9/hocr/searching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from xml.etree import ElementTree
+from lxml import etree
 
 from .util import open_if_required
 from .parse import hocr_page_iterator, hocr_page_to_word_data_fast
 from .text import hocr_get_xml_page_offsets, hocr_get_plaintext_page_offsets, \
         hocr_page_text_from_word_data, get_paragraph_hocr_words
 
 
@@ -68,15 +68,15 @@
     * fp: file pointer to hOCR file
     * `dat`: lookup table entry for the page
     """
     xstart, xend = dat[2:4]
 
     fp.seek(xstart)
     xml = fp.read(xend-xstart)
-    root = ElementTree.fromstring(xml)
+    root = etree.fromstring(xml)
     return root
 
 
 def hocr_lookup_page_by_plaintext_offset(fp, page_lookup_data, pos_bytes_plain):
     """
     Get the XML for a specific hOCR page that corresponds to the plaintext
     offset as specified in pos_bytes_plain.
```

### Comparing `archive-hocr-tools-1.1.53/hocr/text.py` & `archive-hocr-tools-1.1.9/hocr/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import xml.parsers.expat
 
 from .util import open_if_required
-from .parse import hocr_page_to_word_data_fast, hocr_page_iterator
+from .parse import hocr_page_to_word_data, hocr_page_to_word_data_fast, \
+        hocr_page_iterator, hocr_page_get_dimensions
 
 
 def hocr_paragraph_text(paragraph):
     """
     Reconstruct text that matches the FTS text from a hOCR paragraph.
     Returns a tuple, first item in the tuple is the text, the second is a
     boolean, indicating if this paragraph is to be merged into the next one, see
```

### Comparing `archive-hocr-tools-1.1.53/setup.py` & `archive-hocr-tools-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,26 +18,18 @@
       keywords=['hOCR', 'Internet Archive'],
       license='AGPL-3.0',
       scripts=['bin/hocr-combine-stream', 'bin/hocr-fold-chars',
                'bin/hocr-text', 'bin/fts-text-annotate',
                'bin/fts-text-match', 'bin/hocr-lookup-check',
                'bin/hocr-lookup-create', 'bin/hocr-lookup-reconstruct',
                'bin/hocr-text-paragraphs', 'bin/hocr-extract-page',
-               'bin/abbyy-to-hocr', 'bin/hocr-split-pages',
-               'bin/hocr-flatten-pages', 'bin/hocr-confidence-filter',
-               'bin/hocr-to-epub', 'bin/pdf-to-hocr',
-               'bin/hocr-pagenumbers'],
+               'bin/abbyy-to-hocr'],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Programming Language :: Python :: 3',
       ],
       python_requires='>=3.6',
       include_package_data=True,
-      install_requires=[],
-      extras_require={
-          'epub': ['ebooklib==0.17.1', 'internetarchive-deriver-module==1.0.1', 'iso639==0.1.4'],
-          'pdf': ['PyMuPDF==1.22.5', 'numpy==1.21.3'],
-          'pagenumber': ['viterbi-trellis==0.0.3', 'roman>=3.3', 'numpy>=1.21.3', 'scikit-learn>=1.2.2'],
-      },
+      install_requires=['lxml'],
       package_data={'hocr': ['data/*']})
```

