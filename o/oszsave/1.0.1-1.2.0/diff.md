# Comparing `tmp/oszsave-1.0.1.tar.gz` & `tmp/oszsave-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oszsave-1.0.1.tar", max compression
+gzip compressed data, was "oszsave-1.2.0.tar", max compression
```

## Comparing `oszsave-1.0.1.tar` & `oszsave-1.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13675 2023-08-03 20:05:29.287074 oszsave-1.0.1/oszsave.py
--rw-r--r--   0        0        0      386 2023-08-04 05:49:17.489632 oszsave-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6294 2023-08-04 05:52:24.947996 oszsave-1.0.1/README.md
--rw-r--r--   0        0        0     6544 1970-01-01 00:00:00.000000 oszsave-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    23818 2023-08-06 01:49:19.559274 oszsave-1.2.0/oszsave.py
+-rw-r--r--   0        0        0      404 2023-08-06 14:44:18.300134 oszsave-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6294 2023-08-04 05:52:24.947996 oszsave-1.2.0/README.md
+-rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 oszsave-1.2.0/PKG-INFO
```

### Comparing `oszsave-1.0.1/README.md` & `oszsave-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oszsave-1.0.1/PKG-INFO` & `oszsave-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: oszsave
-Version: 1.0.1
-Summary: A lightweight osu map downloader
-License: GNU GPL
+Version: 1.2.0
+Summary: A powerful osu map downloader
+License: GNU v3
 Author: forgedcore8
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: selenium (>=4.11.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align=center>
     
 # OSZsave - osu! Beatmap Downloader
     
 <img src="readme/oszsave.png"
```

