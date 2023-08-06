# Comparing `tmp/pytexutils-0.0.2.tar.gz` & `tmp/pytexutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytexutils-0.0.2.tar", last modified: Sun Aug  6 15:46:09 2023, max compression
+gzip compressed data, was "pytexutils-0.0.3.tar", last modified: Sun Aug  6 15:59:34 2023, max compression
```

## Comparing `pytexutils-0.0.2.tar` & `pytexutils-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      323 2023-08-06 15:46:09.000000 pytexutils-0.0.2/PKG-INFO
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      812 2023-08-06 15:41:31.000000 pytexutils-0.0.2/README.md
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      192 2023-08-06 15:37:58.000000 pytexutils-0.0.2/pytexutils/__init__.py
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils/figures/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      111 2023-08-06 15:38:09.000000 pytexutils-0.0.2/pytexutils/figures/__init__.py
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     1879 2023-08-06 14:17:32.000000 pytexutils-0.0.2/pytexutils/figures/make_image.py
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     2506 2023-08-06 14:17:36.000000 pytexutils-0.0.2/pytexutils/figures/make_tabular_image.py
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils/tables/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       76 2023-08-06 15:38:23.000000 pytexutils-0.0.2/pytexutils/tables/__init__.py
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     3715 2023-08-06 13:32:28.000000 pytexutils-0.0.2/pytexutils/tables/make_table.py
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      323 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/PKG-INFO
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      446 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/SOURCES.txt
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        1 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/dependency_links.txt
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        6 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/requires.txt
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       17 2023-08-06 15:46:09.000000 pytexutils-0.0.2/pytexutils.egg-info/top_level.txt
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       38 2023-08-06 15:46:09.000000 pytexutils-0.0.2/setup.cfg
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     2095 2023-08-06 15:45:54.000000 pytexutils-0.0.2/setup.py
-drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:46:09.000000 pytexutils-0.0.2/tests/
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-05 16:13:01.000000 pytexutils-0.0.2/tests/__init__.py
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      878 2023-08-06 15:37:36.000000 pytexutils-0.0.2/tests/test_make_figure.py
--rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      681 2023-08-06 15:27:51.000000 pytexutils-0.0.2/tests/test_make_table.py
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.977723 pytexutils-0.0.3/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     1072 2023-08-05 17:21:26.000000 pytexutils-0.0.3/LICENSE
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      306 2023-08-06 15:59:34.977097 pytexutils-0.0.3/PKG-INFO
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      812 2023-08-06 15:41:31.000000 pytexutils-0.0.3/README.md
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.961300 pytexutils-0.0.3/pytexutils/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      192 2023-08-06 15:37:58.000000 pytexutils-0.0.3/pytexutils/__init__.py
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.970799 pytexutils-0.0.3/pytexutils/figures/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      111 2023-08-06 15:38:09.000000 pytexutils-0.0.3/pytexutils/figures/__init__.py
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     1879 2023-08-06 14:17:32.000000 pytexutils-0.0.3/pytexutils/figures/make_image.py
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     2506 2023-08-06 14:17:36.000000 pytexutils-0.0.3/pytexutils/figures/make_tabular_image.py
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.973081 pytexutils-0.0.3/pytexutils/tables/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       76 2023-08-06 15:38:23.000000 pytexutils-0.0.3/pytexutils/tables/__init__.py
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     3715 2023-08-06 13:32:28.000000 pytexutils-0.0.3/pytexutils/tables/make_table.py
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.967684 pytexutils-0.0.3/pytexutils.egg-info/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      306 2023-08-06 15:59:34.000000 pytexutils-0.0.3/pytexutils.egg-info/PKG-INFO
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      454 2023-08-06 15:59:34.000000 pytexutils-0.0.3/pytexutils.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        1 2023-08-06 15:59:34.000000 pytexutils-0.0.3/pytexutils.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        6 2023-08-06 15:59:34.000000 pytexutils-0.0.3/pytexutils.egg-info/requires.txt
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       17 2023-08-06 15:59:34.000000 pytexutils-0.0.3/pytexutils.egg-info/top_level.txt
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)       38 2023-08-06 15:59:34.977905 pytexutils-0.0.3/setup.cfg
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)     2261 2023-08-06 15:59:31.000000 pytexutils-0.0.3/setup.py
+drwxr-xr-x   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-06 15:59:34.975777 pytexutils-0.0.3/tests/
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)        0 2023-08-05 16:13:01.000000 pytexutils-0.0.3/tests/__init__.py
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      878 2023-08-06 15:37:36.000000 pytexutils-0.0.3/tests/test_make_figure.py
+-rw-r--r--   0 alessandrosebastianelli   (501) staff       (20)      679 2023-08-06 15:58:03.000000 pytexutils-0.0.3/tests/test_make_table.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytexutils-0.0.2/README.md` & `pytexutils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytexutils-0.0.2/pytexutils/figures/make_image.py` & `pytexutils-0.0.3/pytexutils/figures/make_image.py`

 * *Files identical despite different names*

### Comparing `pytexutils-0.0.2/pytexutils/figures/make_tabular_image.py` & `pytexutils-0.0.3/pytexutils/figures/make_tabular_image.py`

 * *Files identical despite different names*

### Comparing `pytexutils-0.0.2/pytexutils/tables/make_table.py` & `pytexutils-0.0.3/pytexutils/tables/make_table.py`

 * *Files identical despite different names*

### Comparing `pytexutils-0.0.2/tests/test_make_figure.py` & `pytexutils-0.0.3/tests/test_make_figure.py`

 * *Files identical despite different names*

### Comparing `pytexutils-0.0.2/tests/test_make_table.py` & `pytexutils-0.0.3/tests/test_make_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 sys.path += ['.']
 
-from pylatexutils.tables.make_table import make_table
+from pytexutils.tables.make_table import make_table
 import numpy as np
 import os
 
 if __name__ == '__main__':
 
     columns_name = ['A', 'B', 'C']
     data         = np.array(
```

