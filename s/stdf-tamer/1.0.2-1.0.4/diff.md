# Comparing `tmp/stdf_tamer-1.0.2.tar.gz` & `tmp/stdf_tamer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf_tamer-1.0.2.tar", last modified: Wed Jul 26 08:18:01 2023, max compression
+gzip compressed data, was "stdf_tamer-1.0.4.tar", last modified: Sun Aug  6 08:51:26 2023, max compression
```

## Comparing `stdf_tamer-1.0.2.tar` & `stdf_tamer-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11558 2023-07-06 13:14:13.436374 stdf_tamer-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0      422 2023-07-25 14:39:05.133046 stdf_tamer-1.0.2/README.md
--rw-r--r--   0        0        0     1140 2023-07-26 08:18:01.028076 stdf_tamer-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      151 2022-12-19 08:36:15.991971 stdf_tamer-1.0.2/src/_ams_rw_stdf_writer_state.py
--rw-r--r--   0        0        0    24533 2023-07-23 10:26:23.075896 stdf_tamer-1.0.2/src/ams_rw_stdf.py
--rw-r--r--   0        0        0    16086 2023-07-22 10:05:33.495555 stdf_tamer-1.0.2/src/ams_rw_stdf_writer.py
--rw-r--r--   0        0        0     4332 2023-07-26 08:16:30.332928 stdf_tamer-1.0.2/src/converter.py
--rw-r--r--   0        0        0     1549 2023-03-09 16:19:36.796549 stdf_tamer-1.0.2/src/create_index_at_dropzone.py
--rw-r--r--   0        0        0      488 2022-12-19 08:36:10.856733 stdf_tamer-1.0.2/src/example.py
--rw-r--r--   0        0        0     2148 2023-07-26 08:16:38.739875 stdf_tamer-1.0.2/src/simulator.py
--rw-r--r--   0        0        0      729 2023-07-26 08:16:17.374740 stdf_tamer-1.0.2/src/stdfanalyser.py
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 stdf_tamer-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-07-06 13:14:13.436374 stdf_tamer-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      422 2023-07-25 14:39:05.133046 stdf_tamer-1.0.4/README.md
+-rw-r--r--   0        0        0     1140 2023-08-06 08:51:26.948462 stdf_tamer-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      151 2022-12-19 08:36:15.991971 stdf_tamer-1.0.4/src/_ams_rw_stdf_writer_state.py
+-rw-r--r--   0        0        0    24533 2023-07-23 10:26:23.075896 stdf_tamer-1.0.4/src/ams_rw_stdf.py
+-rw-r--r--   0        0        0    16086 2023-07-22 10:05:33.495555 stdf_tamer-1.0.4/src/ams_rw_stdf_writer.py
+-rw-r--r--   0        0        0     5033 2023-08-06 08:38:56.426591 stdf_tamer-1.0.4/src/converter.py
+-rw-r--r--   0        0        0     1549 2023-03-09 16:19:36.796549 stdf_tamer-1.0.4/src/create_index_at_dropzone.py
+-rw-r--r--   0        0        0      488 2022-12-19 08:36:10.856733 stdf_tamer-1.0.4/src/example.py
+-rw-r--r--   0        0        0     2148 2023-07-26 08:36:17.719367 stdf_tamer-1.0.4/src/simulator.py
+-rw-r--r--   0        0        0      729 2023-07-26 08:16:17.374740 stdf_tamer-1.0.4/src/stdfanalyser.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 stdf_tamer-1.0.4/PKG-INFO
```

### Comparing `stdf_tamer-1.0.2/LICENSE.txt` & `stdf_tamer-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/pyproject.toml` & `stdf_tamer-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 requires-python = ">=3.8.0"
 readme = "README.md"
 keywords = [
     "STDF",
     "ATE",
 ]
-version = "1.0.2"
+version = "1.0.4"
 
 [project.license]
 text = "apache 2.0"
 
 [project.urls]
 Homepage = "https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer"
 Repository = "https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer"
```

### Comparing `stdf_tamer-1.0.2/src/ams_rw_stdf.py` & `stdf_tamer-1.0.4/src/ams_rw_stdf.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/src/ams_rw_stdf_writer.py` & `stdf_tamer-1.0.4/src/ams_rw_stdf_writer.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/src/create_index_at_dropzone.py` & `stdf_tamer-1.0.4/src/create_index_at_dropzone.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/src/simulator.py` & `stdf_tamer-1.0.4/src/simulator.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/src/stdfanalyser.py` & `stdf_tamer-1.0.4/src/stdfanalyser.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.2/PKG-INFO` & `stdf_tamer-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdf-tamer
-Version: 1.0.2
+Version: 1.0.4
 Summary: a stdf reader/writer/analyser/converter and robotframework library
 Keywords: STDF ATE
 Author: Labor DC jona
 Author-Email: Franz Haas <franz.haas@ams-osram.com>
 License: apache 2.0
 Project-URL: Homepage, https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer
 Project-URL: Repository, https://gittf.ams-osram.info/labor-rapperswil-jona/ams-tamer
```

