# Comparing `tmp/aurora-asi-lib-0.9.4.tar.gz` & `tmp/aurora-asi-lib-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora-asi-lib-0.9.4.tar", last modified: Tue Oct 26 17:12:04 2021, max compression
+gzip compressed data, was "aurora-asi-lib-0.9.5.tar", last modified: Tue Oct 26 21:12:19 2021, max compression
```

## Comparing `aurora-asi-lib-0.9.4.tar` & `aurora-asi-lib-0.9.5.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.765792 aurora-asi-lib-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-10-26 17:12:04.765792 aurora-asi-lib-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.757791 aurora-asi-lib-0.9.4/asilib/
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2144 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.761791 aurora-asi-lib-0.9.4/asilib/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/analysis/equal_area.py
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/analysis/keogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     9098 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/analysis/map.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/analysis/start_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.761791 aurora-asi-lib-0.9.4/asilib/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/conjunction_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/fisheye_image_arc.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/fisheye_image_omega_band.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/fisheye_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/keogram_field_line_resonance.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/keogram_steve.py
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/keogram_streamer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/map_arc.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/examples/map_steve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.761791 aurora-asi-lib-0.9.4/asilib/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5916 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/io/download_rego.py
--rw-r--r--   0 runner    (1001) docker     (121)     5882 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/io/download_themis.py
--rw-r--r--   0 runner    (1001) docker     (121)    23710 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/io/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     5146 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.761791 aurora-asi-lib-0.9.4/asilib/plot/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16133 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/plot/animate_fisheye.py
--rw-r--r--   0 runner    (1001) docker     (121)     7566 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/plot/plot_fisheye.py
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/plot/plot_keogram.py
--rw-r--r--   0 runner    (1001) docker     (121)    11303 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/plot/plot_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.765792 aurora-asi-lib-0.9.4/asilib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_download_rego.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_download_themis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_equal_area.py
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_keogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     4531 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_plot_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_plot_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/asilib/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 17:12:04.765792 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-10-26 17:12:04.000000 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-10-26 17:12:04.000000 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 17:12:04.000000 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-26 17:12:04.000000 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-26 17:12:04.000000 aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-10-26 17:12:04.765792 aurora-asi-lib-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-26 17:11:51.000000 aurora-asi-lib-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.485592 aurora-asi-lib-0.9.5/asilib/
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2144 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.485592 aurora-asi-lib-0.9.5/asilib/analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4968 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/analysis/equal_area.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/analysis/keogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9098 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/analysis/map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/analysis/start_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/asilib/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3791 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/conjunction_movie.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/fisheye_image_arc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/fisheye_image_omega_band.py
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/fisheye_movie.py
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/keogram_field_line_resonance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/keogram_steve.py
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/keogram_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/map_arc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      550 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/examples/map_steve.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/asilib/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13203 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/io/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22413 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/io/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5146 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/asilib/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16133 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/plot/animate_fisheye.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7566 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/plot/plot_fisheye.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3674 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/plot/plot_keogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11303 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/plot/plot_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/asilib/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_download_rego.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_download_themis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_equal_area.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3102 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_keogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4531 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1758 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_plot_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_plot_movie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4424 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/asilib/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-10-26 21:12:19.000000 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-10-26 21:12:19.000000 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 21:12:19.000000 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-26 21:12:19.000000 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-26 21:12:19.000000 aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-10-26 21:12:19.489592 aurora-asi-lib-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-26 21:12:11.000000 aurora-asi-lib-0.9.5/setup.py
```

### Comparing `aurora-asi-lib-0.9.4/LICENSE` & `aurora-asi-lib-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/PKG-INFO` & `aurora-asi-lib-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-asi-lib
-Version: 0.9.4
+Version: 0.9.5
 Summary: Easily download, plot, animate, and analyze auroral all sky imager (ASI) data.
 Home-page: https://github.com/mshumko/aurora-asi-lib
 Author: Mykhaylo Shumko
 Author-email: msshumko@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3.0
 Keywords: aurora, all sky imager, Red-line Emission Geospace Observatory, REGO,,Time History of Events and Macroscale Interactions during Substorms, THEMIS
 Platform: UNKNOWN
```

### Comparing `aurora-asi-lib-0.9.4/README.md` & `aurora-asi-lib-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/__init__.py` & `aurora-asi-lib-0.9.5/asilib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import warnings
 import pathlib
 import configparser
 
-__version__ = '0.9.4'
+__version__ = '0.9.5'
 
 # Load the configuration settings.
 HERE = pathlib.Path(__file__).parent.resolve()
 settings = configparser.ConfigParser()
 settings.read(HERE / 'config.ini')
 
 try:
@@ -14,18 +14,16 @@
     ASI_DATA_DIR = pathlib.Path(ASI_DATA_DIR)
 except KeyError:  # Raised if config.ini does not have Paths.
     ASI_DATA_DIR = pathlib.Path.home() / 'asilib-data'
 
 config = {'ASILIB_DIR': HERE, 'ASI_DATA_DIR': ASI_DATA_DIR}
 
 # Import download programs.
-from asilib.io.download_rego import download_rego_img
-from asilib.io.download_rego import download_rego_skymap
-from asilib.io.download_themis import download_themis_img
-from asilib.io.download_themis import download_themis_skymap
+from asilib.io.download import download_image
+from asilib.io.download import download_skymap
 
 # Import the loading functions.
 from asilib.io.load import load_skymap
 from asilib.io.load import load_image
 from asilib.io.load import load_image_generator
 from asilib.io.load import get_frame  # Deprecated
 from asilib.io.load import get_frames  # Deprecated
```

### Comparing `aurora-asi-lib-0.9.4/asilib/__main__.py` & `aurora-asi-lib-0.9.5/asilib/__main__.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/analysis/equal_area.py` & `aurora-asi-lib-0.9.5/asilib/analysis/equal_area.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/analysis/keogram.py` & `aurora-asi-lib-0.9.5/asilib/analysis/keogram.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/analysis/map.py` & `aurora-asi-lib-0.9.5/asilib/analysis/map.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/examples/conjunction_movie.py` & `aurora-asi-lib-0.9.5/asilib/examples/conjunction_movie.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/examples/fisheye_image_omega_band.py` & `aurora-asi-lib-0.9.5/asilib/examples/fisheye_image_omega_band.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/examples/keogram_field_line_resonance.py` & `aurora-asi-lib-0.9.5/asilib/examples/keogram_field_line_resonance.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/examples/keogram_steve.py` & `aurora-asi-lib-0.9.5/asilib/examples/keogram_steve.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/examples/map_arc.py` & `aurora-asi-lib-0.9.5/asilib/examples/map_arc.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,16 @@
 
 time = datetime(2007, 3, 13, 5, 8, 45)
 asi_array_code = 'THEMIS'
 location_codes = ['FSIM', 'ATHA', 'TPAS', 'SNKQ']
 map_alt = 110
 min_elevation = 2
 
-# At this time asilib doesn't have an intuitive way to map multiple ASI images, so you need
-# to plot the first imager, and reuse the retuned subplot map to plot the other images.
-image_time, image, skymap, ax, pcolormesh_obj = asilib.plot_map(
-    asi_array_code, location_codes[0], time, map_alt, map_style='green', min_elevation=min_elevation
-)
+ax = asilib.create_cartopy_map(map_style='white', lon_bounds=(-160, -52), lat_bounds=(40, 82))
 
-for location_code in location_codes[1:]:
+for location_code in location_codes:
     asilib.plot_map(
         asi_array_code, location_code, time, map_alt, ax=ax, min_elevation=min_elevation
     )
 
 ax.set_title('Donovan et al. 2008 | First breakup of an auroral arc')
 plt.show()
```

### Comparing `aurora-asi-lib-0.9.4/asilib/io/download_themis.py` & `aurora-asi-lib-0.9.5/asilib/io/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,161 @@
-import requests
-from datetime import datetime
-from typing import List, Union
+"""
+A set of utility functions for asilib.
+"""
 import dateutil.parser
 import pathlib
-import warnings
+from typing import List, Union
+import copy
+from datetime import timedelta, datetime
 
-import asilib
-import asilib.io.utils as utils
+from bs4 import BeautifulSoup
+import requests
+import numpy as np
 
-"""
-This program contains the Time History of Events and Macroscale Interactions during 
-Substorms (THEMIS) download functions that stream image and skymap data from the 
-themis.ssl.berkeley.edu and data.phys.ucalgary.ca servers. The data is saved to 
-asilib.config['ASI_DATA_DIR']/themis directory.
-"""
 
-IMG_BASE_URL = 'http://themis.ssl.berkeley.edu/data/themis/thg/l1/asi/'
-SKYMAP_BASE_URL = 'https://data.phys.ucalgary.ca/sort_by_project/THEMIS/asi/skymaps/'
+_time_type = Union[datetime, str]
+_time_range_type = List[_time_type]
 
-# Check and make a asilib.config['ASI_DATA_DIR']/themis/ directory if doesn't already exist.
-themis_dir = pathlib.Path(asilib.config['ASI_DATA_DIR'], 'themis')
-if not themis_dir.exists():
-    themis_dir.mkdir(parents=True)
-
-
-def download_themis_img(
-    location_code: str,
-    time: utils._time_type = None,
-    time_range: utils._time_range_type = None,
-    force_download: bool = False,
-    ignore_missing_data: bool = True,
-) -> List[pathlib.Path]:
+
+def _validate_time(time: _time_type) -> List[datetime]:
+    """
+    Validates tries to parse the time into datetime objects.
     """
-    Download one hourly THEMIS cdf file given the imager location and ``time``, or
-    multiple hourly files given ``time_range``.
+    if isinstance(time, str):
+        time = dateutil.parser.parse(time)
+    elif isinstance(time, (int, float)):
+        raise ValueError(f'Unknown time format, {time}')
+    return time
 
-    Parameters
-    ----------
-    location_code: str
-        The ASI station code, i.e. ``ATHA``
-    time: datetime.datetime or str
-        The date and time to download of the data. If str, ``time`` must be in the
-        ISO 8601 standard.
-    time_range: list of datetime.datetimes or stings
-        Defined the duration of data to download. Must be of length 2.
-    force_download: bool
-        If True, download the file even if it already exists. Useful if a prior
-        data download was incomplete.
-    ignore_missing_data: bool
-        Flag to ignore the FileNotFoundError that is raised when ASI
-        data is unavailable for that date-hour. Only used when
-        ``time_range`` is specified.
 
-    Returns
-    -------
-    download_paths: list
-        A list of pathlib.Path objects that contain the downloaded file
-        path(s).
+def _validate_time_range(time_range: _time_range_type) -> List[datetime]:
+    """
+    Validates tries to parse the time_range into datetime objects.
+    """
+    if time_range is None:
+        return None
 
-    Example
-    -------
-    from datetime import datetime
+    assert isinstance(
+        time_range, (list, tuple, np.ndarray)
+    ), "time_range must be a list, tuple, or np.ndarray."
+    assert len(time_range) == 2, "time_range must be a list or a tuple with start and end times."
 
-    import asilib
+    time_range_parsed = []
 
-    | location_code = 'LUCK'
-    | time = datetime(2017, 4, 13, 5)
-    | asilib.download_themis_img(location_code, time)
-    """
-    if (time is None) and (time_range is None):
-        raise AttributeError('Neither time or time_range is specified.')
-    elif (time is not None) and (time_range is not None):
-        raise AttributeError('Both time and time_range can not be simultaneously specified.')
-
-    elif time is not None:
-        time = utils._validate_time(time)
-        download_path = _download_one_img_file(location_code, time, force_download)
-        download_paths = [
-            download_path
-        ]  # List for constancy with the time_range code chunk output.
-
-    elif time_range is not None:
-        time_range = utils._validate_time_range(time_range)
-        download_hours = utils._get_hours(time_range)
-        download_paths = []
-
-        for hour in download_hours:
-            try:
-                download_path = _download_one_img_file(location_code, hour, force_download)
-                download_paths.append(download_path)
-            except NotADirectoryError:
-                if ignore_missing_data:
-                    continue
-                else:
-                    raise
+    for t in time_range:
+        if isinstance(t, str):
+            time_range_parsed.append(dateutil.parser.parse(t))
+        elif isinstance(t, (int, float)):
+            raise ValueError(f'Unknown time format, {t}')
+        else:
+            time_range_parsed.append(t)
 
-    return download_paths
+    time_range_parsed.sort()
+    return time_range_parsed
 
 
-def download_themis_skymap(location_code: str, force_download: bool = False):
+def _get_hours(time_range: _time_range_type) -> List[datetime]:
     """
-    Download all of the THEMIS skymap IDL .sav files.
+    Helper function to figure out what date-hour times are between the times in time_range.
+    This function is useful to figure out what hourly ASI files to download.
+    """
+    # Modify time_range. If time_range[0] is not at the top of the hour, we zero the minutes
+    # seconds, and milliseconds. This helps with keeping the + 1 hour offsets aligned to the
+    # start of the hour.
+    current_hour = copy.copy(time_range[0].replace(minute=0, second=0, microsecond=0))
+    hours = []
+
+    # Not <= in while loop because we don't want to download the final hour if time_range[1] is,
+    # for example, 05:00:00 [HH:MM:SS].
+    while current_hour < time_range[1]:
+        hours.append(current_hour)
+        current_hour += timedelta(hours=1)
+    return hours
+
+
+def _stream_large_file(
+    url: str, save_path: Union[pathlib.Path, str], test_flag: bool = False
+) -> None:
+    """
+    Streams a file from url to save_path. In requests.get(), stream=True
+    sets up a generator to download a small chuck of data at a time,
+    instead of downloading the entire file into RAM first.
 
     Parameters
     ----------
-    location_code: str
-        The ASI station code, i.e. ``ATHA``
-    force_download: bool
-        If True, download the file even if it already exists. Useful if a prior
-        data download was incomplete.
+    url: str
+        The URL to the file.
+    save_path: str or pathlib.Path
+        The local save path for the file.
+    test_flag: bool (optional)
+        If True, the download will halt after one 5 Mb chunk of data is
+        downloaded.
 
     Returns
     -------
     None
-
-    Example
-    -------
-    import asilib
-
-    | location_code = 'LUCK'
-    | asilib.download_themis_skymap(location_code)
     """
-    # Create the skymap directory in data/themis/skymap/location_code
-    save_dir = asilib.config['ASI_DATA_DIR'] / 'themis' / 'skymap' / location_code.lower()
-    if not save_dir.is_dir():
-        save_dir.mkdir(parents=True)
-        print(f'Made directory at {save_dir}')
-
-    url = SKYMAP_BASE_URL + f'{location_code.lower()}/'
-
-    # Look for all of the skymap hyperlinks, go in each one of them, and
-    # download the .sav file.
-    skymap_folders_relative = utils._search_hrefs(url, search_pattern=location_code.lower())
-    download_paths = []
-
-    for skymap_folder in skymap_folders_relative:
-        skymap_folder_absolute = url + skymap_folder
+    r = requests.get(url, stream=True)
+    file_size = int(r.headers.get('content-length'))
+    downloaded_bites = 0
+
+    save_name = pathlib.Path(save_path).name
+
+    megabyte = 1024 * 1024
+
+    with open(save_path, 'wb') as f:
+        for data in r.iter_content(chunk_size=5 * megabyte):
+            f.write(data)
+            if test_flag:
+                return
+            # Update the downloaded % in the terminal.
+            downloaded_bites += len(data)
+            download_percent = round(100 * downloaded_bites / file_size)
+            download_str = "#" * (download_percent // 5)
+            print(f'Downloading {save_name}: |{download_str:<20}| {download_percent}%', end='\r')
+    print()  # Add a newline
+    return
+
+
+def _search_hrefs(url: str, search_pattern: str = '.cdf') -> List[str]:
+    """
+    Given a url string, this function returns all of the
+    hyper references (hrefs, or hyperlinks). If search_pattern is not
+    specified, a default '.cdf' value is assumed and this function
+    will return all hrefs with the CDF extension. If no hrefs containing
+    search_pattern are found, this function raises a NotADirectoryError.
+    The search is case-insensitive.
 
-        # Lastly, research for the skymap .sav file.
-        skymap_name = utils._search_hrefs(skymap_folder_absolute, search_pattern=f'.sav')[0]
-        skymap_save_name = skymap_name.replace('-%2B', '')  # Replace the unicode '+'.
-
-        # Download if force_download=True or the file does not exist.
-        download_path = pathlib.Path(save_dir, skymap_save_name)
-        download_paths.append(download_path)
-        if force_download or (not download_path.is_file()):
-            utils._stream_large_file(skymap_folder_absolute + skymap_name, download_path)
-    return download_paths
-
-
-def _download_one_img_file(location_code, time, force_download):
-    """
-    Download one hour-long file.
-    """
-    # Add the location/year/month url folders onto the url
-    url = IMG_BASE_URL + f'{location_code.lower()}/{time.year}/{str(time.month).zfill(2)}/'
+    Parameters
+    ----------
+    url: str
+        A url in string format
+    search_pattern: str (optional)
+        Find the exact search_pattern text contained in the hrefs.
+        By default all hrefs matching the extension ".cdf" are returned.
 
-    search_pattern = f'{location_code.lower()}_{time.strftime("%Y%m%d%H")}'
-    file_names = utils._search_hrefs(url, search_pattern=search_pattern)
+    Returns
+    -------
+    hrefs: List(str)
+        A list of hrefs that contain the search_pattern.
 
-    server_url = url + file_names[0]
-    download_path = pathlib.Path(asilib.config['ASI_DATA_DIR'], 'themis', file_names[0])
-    if force_download or (not download_path.is_file()):
-        utils._stream_large_file(server_url, download_path)
-    return download_path
+    Raises
+    ------
+    NotADirectoryError
+        If a hyper reference (a folder or a file) is not found on the
+        server. This is raised if the data does not exist.
+    """
+    matched_hrefs = []
+
+    request = requests.get(url)
+    # request.status_code
+    soup = BeautifulSoup(request.content, 'html.parser')
+
+    for href in soup.find_all('a', href=True):
+        if search_pattern.lower() in href['href'].lower():
+            matched_hrefs.append(href['href'])
+    if len(matched_hrefs) == 0:
+        raise NotADirectoryError(
+            f'The url {url} does not contain any hyper '
+            f'references containing the search_pattern="{search_pattern}".'
+        )
+    return matched_hrefs
```

### Comparing `aurora-asi-lib-0.9.4/asilib/io/load.py` & `aurora-asi-lib-0.9.5/asilib/io/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from os import stat
 import pathlib
 from datetime import datetime, timedelta
 import dateutil.parser
-from typing import List, Union, Sequence, Tuple
+from typing import List, Tuple
 from copy import copy
 import warnings
 import re
 
 import pandas as pd
 import numpy as np
 import cdflib
 import scipy.io
-import matplotlib.pyplot as plt
 
-from asilib.io import download_rego
-from asilib.io import download_themis
+from asilib.io.download import download_image
+from asilib.io.download import download_skymap
 from asilib.io import utils
 import asilib
 
 
 def load_image(
     asi_array_code: str,
     location_code: str,
@@ -212,22 +211,17 @@
     | rego_skymap = asilib.load_skymap('REGO', 'GILL', '2018-10-01')
     """
     # Try to convert time to datetime object if it is a string.
     if isinstance(time, str):
         time = dateutil.parser.parse(time)
 
     if force_download:
-        if asi_array_code.lower() == 'themis':
-            skymap_paths = download_themis.download_themis_skymap(
-                location_code, force_download=force_download
-            )
-        elif asi_array_code.lower() == 'rego':
-            skymap_paths = download_rego.download_rego_skymap(
-                location_code, force_download=force_download
-            )
+        skymap_paths = download_skymap(asi_array_code.lower(),
+            location_code, force_download=force_download
+        )
 
     else:
         # If the user does not want to force download skymap files,
         # look for the appropriate file on the computer. If a local
         # skymap file is not found, download them all and look for the
         # appropriate file.
         skymap_dir = pathlib.Path(
@@ -235,22 +229,17 @@
         )
         skymap_paths = sorted(
             list(skymap_dir.rglob(f'{asi_array_code.lower()}_skymap_{location_code.lower()}*'))
         )
 
         # Download skymap files if they are not downloaded yet.
         if len(skymap_paths) == 0:
-            if asi_array_code.lower() == 'themis':
-                skymap_paths = download_themis.download_themis_skymap(
-                    location_code, force_download=force_download
-                )
-            elif asi_array_code.lower() == 'rego':
-                skymap_paths = download_rego.download_rego_skymap(
-                    location_code, force_download=force_download
-                )
+            skymap_paths = download_skymap(asi_array_code.lower(),
+                location_code, force_download=force_download
+            )
 
     skymap_dates = _extract_skymap_dates(skymap_paths)
 
     # Find the skymap_date that is closest and before time.
     # For reference: dt > 0 when time is after skymap_date.
     dt = np.array([(time - skymap_date).total_seconds() for skymap_date in skymap_dates])
     dt[dt < 0] = np.inf  # Mask out all skymap_dates after time.
@@ -522,54 +511,39 @@
     | import asilib
     |
     | asi_file_path = asilib._find_img_path('REGO', 'GILL', '2016-10-29T04')
     """
     time = utils._validate_time(time)
 
     if force_download:
-        if asi_array_code.lower() == 'themis':
-            file_path = download_themis.download_themis_img(
-                location_code, time=time, force_download=force_download
-            )[0]
-        elif asi_array_code.lower() == 'rego':
-            file_path = download_rego.download_rego_img(
-                location_code, time=time, force_download=force_download
-            )[0]
+        file_path = download_image(asi_array_code.lower(), 
+            location_code, time=time, force_download=force_download
+        )[0]
     else:
         # If the user does not want to force a download, look for a file on the
         # computer. If a local file is not found, try to download one.
         search_path = pathlib.Path(asilib.config['ASI_DATA_DIR'], asi_array_code.lower())
         if asi_array_code.lower() == 'themis':
             search_pattern = f'*asf*{location_code.lower()}*{time.strftime("%Y%m%d%H")}*'
         elif asi_array_code.lower() == 'rego':
             search_pattern = f'*rgf*{location_code.lower()}*{time.strftime("%Y%m%d%H")}*'
         matched_paths = list(search_path.rglob(search_pattern))
 
         if len(matched_paths) == 1:  # A local file found
             file_path = matched_paths[0]
 
         elif len(matched_paths) == 0:  # No local file found
-            if asi_array_code.lower() == 'themis':
-                try:
-                    file_path = download_themis.download_themis_img(
-                        location_code, time=time, force_download=force_download
-                    )[0]
-                except NotADirectoryError:
-                    raise FileNotFoundError(
-                        f'THEMIS ASI data not found for location_code={location_code} at {time}'
-                    )
-            elif asi_array_code.lower() == 'rego':
-                try:
-                    file_path = download_rego.download_rego_img(
-                        location_code, time=time, force_download=force_download
-                    )[0]
-                except NotADirectoryError:
-                    raise FileNotFoundError(
-                        f'REGO ASI data not found for location_code={location_code} at {time}'
-                    )
+            try:
+                file_path = download_image(asi_array_code.lower(),
+                    location_code, time=time, force_download=force_download
+                )[0]
+            except NotADirectoryError:
+                raise FileNotFoundError(
+                    f'{asi_array_code.upper()} ASI data not found for location_code={location_code} at {time}'
+                )
         else:  # Multiple files found?
             raise ValueError(f"Not sure what happend here. I found {matched_paths} matching paths.")
 
     return file_path
 
 
 def _get_epoch(cdf_obj, time_key, hour_date_time, asi_array_code, location_code):
```

### Comparing `aurora-asi-lib-0.9.4/asilib/plot/animate_fisheye.py` & `aurora-asi-lib-0.9.5/asilib/plot/animate_fisheye.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/plot/plot_fisheye.py` & `aurora-asi-lib-0.9.5/asilib/plot/plot_fisheye.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/plot/plot_keogram.py` & `aurora-asi-lib-0.9.5/asilib/plot/plot_keogram.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/plot/plot_map.py` & `aurora-asi-lib-0.9.5/asilib/plot/plot_map.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_download_rego.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_download_rego.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 import unittest
-import requests
 import pathlib
 from datetime import datetime
 
-from asilib.io import download_rego
 import asilib
 
 """
 Unit tests to check that the functions in download_rego.py are working correctly.
 Run with "python3 test_download_rego.py -v" for the verbose output.
 """
 
 
 class TestDownloadRego(unittest.TestCase):
     def setUp(self):
         """Set up a few variables."""
-        # http://themis.ssl.berkeley.edu/data/themis/thg/l1/reg/luck/2020/08/clg_l1_rgf_luck_2020080104_v01.cdf
         self.day = datetime(2020, 8, 1, 4)
         self.location_code = 'Luck'
-        self.url = (
-            download_rego.IMG_BASE_URL
-            + f'{self.location_code.lower()}/{self.day.year}/{str(self.day.month).zfill(2)}/'
-        )
+        self.asi_array_code = 'rEGO'
         return
 
     def test_download_img(self):
         """
-        Test the full REGO data downloader and download an hour file
+        Test the REGO data downloader to download an hour file
         clg_l1_rgf_luck_2020080104_v01.cdf to ./rego/.
         """
         image_dir = pathlib.Path(asilib.config['ASI_DATA_DIR'], 'rego')
         image_path = image_dir / 'clg_l1_rgf_luck_2020080104_v01.cdf'
 
-        download_rego.download_rego_img(self.location_code, time=self.day, force_download=True)
+        save_path = asilib.download_image(self.asi_array_code, self.location_code, time=self.day, 
+            force_download=True)
 
+        assert image_path == save_path[0]
         assert image_path.is_file()
         return
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_download_themis.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_download_themis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import unittest
 import requests
 import pathlib
 from datetime import datetime
 
-from asilib.io import download_themis
 import asilib
 
 """
-Unit tests to check that the functions in download_themis.py are working correctly.
+Unit tests to check that the functions in download.py are working correctly.
 Run with "python3 test_download_themis.py -v" for the verbose output.
 """
 
 
 class TestDownloadThemis(unittest.TestCase):
     def setUp(self):
         """Set up a few variables."""
         self.day = datetime(2016, 10, 29, 4)
         self.location_code = 'Gill'
+        self.asi_array_code = 'THEMIs'
+
         self.url = (
-            download_themis.IMG_BASE_URL
+            'http://themis.ssl.berkeley.edu/data/themis/thg/l1/asi/'
             + f'{self.location_code.lower()}/{self.day.year}/{str(self.day.month).zfill(2)}/'
         )
         return
 
     def test_server_response(self):
         """Check that the server responds without an error."""
         r = requests.get(self.url)
         status_code = r.status_code
         # Check that the server status code is not
         # between 400-599 (error).
         self.assertNotEqual(status_code // 100, 4)
         self.assertNotEqual(status_code // 100, 5)
         return
 
-    def test_download_themis_img_one_file(self):
+    def test_download_img(self):
         """
         Test the full THEMIS data downloader and download an hour file
         clg_l1_rgf_luck_2020080104_v01.cdf to ./themis/.
         """
         temp_image_dir = pathlib.Path(asilib.config['ASI_DATA_DIR'], 'themis')
         temp_image_path = temp_image_dir / 'thg_l1_asf_gill_2016102904_v01.cdf'
 
-        download_themis.download_themis_img(self.location_code, self.day, force_download=True)
+        save_path = asilib.download_image(self.asi_array_code, self.location_code, time=self.day, 
+            force_download=True)
 
-        self.assertTrue(temp_image_path.is_file())
+        assert temp_image_path == save_path[0]
+        assert temp_image_path.is_file()
         return
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_equal_area.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_equal_area.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_keogram.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_keogram.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_load.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_map.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_plot_map.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_plot_map.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_plot_movie.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_plot_movie.py`

 * *Files identical despite different names*

### Comparing `aurora-asi-lib-0.9.4/asilib/tests/test_utils.py` & `aurora-asi-lib-0.9.5/asilib/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class TestUtils(unittest.TestCase):
     def setUp(self):
         """Set up a few variables."""
         # http://themis.ssl.berkeley.edu/data/themis/thg/l1/reg/luck/2020/08/clg_l1_rgf_luck_2020080104_v01.cdf
         self.day = datetime(2020, 8, 1, 4)
         self.location_code = 'LuCk'
         self.url = (
-            asilib.io.download_rego.IMG_BASE_URL
+            'http://themis.ssl.berkeley.edu/data/themis/thg/l1/reg/'
             + f'{self.location_code.lower()}/{self.day.year}/{str(self.day.month).zfill(2)}/'
         )
         return
 
     def test_server_response(self):
         """Check that the server responds without an error, 400-599 status_codes."""
         r = requests.get(self.url)
```

### Comparing `aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/PKG-INFO` & `aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-asi-lib
-Version: 0.9.4
+Version: 0.9.5
 Summary: Easily download, plot, animate, and analyze auroral all sky imager (ASI) data.
 Home-page: https://github.com/mshumko/aurora-asi-lib
 Author: Mykhaylo Shumko
 Author-email: msshumko@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3.0
 Keywords: aurora, all sky imager, Red-line Emission Geospace Observatory, REGO,,Time History of Events and Macroscale Interactions during Substorms, THEMIS
 Platform: UNKNOWN
```

### Comparing `aurora-asi-lib-0.9.4/aurora_asi_lib.egg-info/SOURCES.txt` & `aurora-asi-lib-0.9.5/aurora_asi_lib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 asilib/examples/fisheye_movie.py
 asilib/examples/keogram_field_line_resonance.py
 asilib/examples/keogram_steve.py
 asilib/examples/keogram_streamer.py
 asilib/examples/map_arc.py
 asilib/examples/map_steve.py
 asilib/io/__init__.py
-asilib/io/download_rego.py
-asilib/io/download_themis.py
+asilib/io/download.py
 asilib/io/load.py
 asilib/io/utils.py
 asilib/plot/__init__.py
 asilib/plot/animate_fisheye.py
 asilib/plot/plot_fisheye.py
 asilib/plot/plot_keogram.py
 asilib/plot/plot_map.py
```

### Comparing `aurora-asi-lib-0.9.4/setup.cfg` & `aurora-asi-lib-0.9.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aurora-asi-lib
-version = 0.9.4
+version = 0.9.5
 url = https://github.com/mshumko/aurora-asi-lib
 author = Mykhaylo Shumko
 author_email = msshumko@gmail.com
 description = Easily download, plot, animate, and analyze auroral all sky imager (ASI) data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 licence_file = LICENSE
```

