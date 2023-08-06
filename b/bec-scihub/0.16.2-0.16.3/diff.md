# Comparing `tmp/bec_scihub-0.16.2.tar.gz` & `tmp/bec_scihub-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.16.2.tar", last modified: Sat Aug  5 09:29:51 2023, max compression
+gzip compressed data, was "bec_scihub-0.16.3.tar", last modified: Sun Aug  6 17:53:15 2023, max compression
```

## Comparing `bec_scihub-0.16.2.tar` & `bec_scihub-0.16.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.774346 bec_scihub-0.16.2/
--rw-r--r--   0 root         (0) root         (0)      478 2023-08-05 09:29:51.774346 bec_scihub-0.16.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.773346 bec_scihub-0.16.2/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-05 09:29:51.000000 bec_scihub-0.16.2/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.770346 bec_scihub-0.16.2/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.16.2/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.771346 bec_scihub-0.16.2/scihub/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.16.2/scihub/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.16.2/scihub/cli/launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.772346 bec_scihub-0.16.2/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.16.2/scihub/scibec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scibec/config_handler.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scibec/scibec.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scibec/scibec_connector.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.16.2/scihub/scibec/scibec_validator.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 09:29:51.772346 bec_scihub-0.16.2/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.16.2/scihub/scilog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.16.2/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-08-05 09:29:51.774346 bec_scihub-0.16.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1758 2023-08-05 09:29:46.000000 bec_scihub-0.16.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.644174 bec_scihub-0.16.3/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-06 17:53:15.644174 bec_scihub-0.16.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.643174 bec_scihub-0.16.3/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-06 17:53:15.000000 bec_scihub-0.16.3/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.641174 bec_scihub-0.16.3/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.16.3/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.641174 bec_scihub-0.16.3/scihub/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.16.3/scihub/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.16.3/scihub/cli/launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.642174 bec_scihub-0.16.3/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.16.3/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.16.3/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-06 17:53:15.642174 bec_scihub-0.16.3/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.16.3/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.16.3/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-08-06 17:53:15.644174 bec_scihub-0.16.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2023-08-06 17:53:08.000000 bec_scihub-0.16.3/setup.py
```

### Comparing `bec_scihub-0.16.2/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.16.3/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/cli/launch.py` & `bec_scihub-0.16.3/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scibec/config_handler.py` & `bec_scihub-0.16.3/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scibec/scibec.py` & `bec_scihub-0.16.3/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scibec/scibec_connector.py` & `bec_scihub-0.16.3/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.16.3/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scibec/scibec_validator.py` & `bec_scihub-0.16.3/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scihub.py` & `bec_scihub-0.16.3/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/scihub/scilog/scilog.py` & `bec_scihub-0.16.3/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/setup.cfg` & `bec_scihub-0.16.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.16.2/setup.py` & `bec_scihub-0.16.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "0.16.2"
+__version__ = "0.16.3"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

