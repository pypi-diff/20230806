# Comparing `tmp/sgw_tools-1.96.tar.gz` & `tmp/sgw_tools-1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.96.tar", last modified: Wed Jun  7 21:24:51 2023, max compression
+gzip compressed data, was "sgw_tools-1.97.tar", last modified: Sun Aug  6 12:30:17 2023, max compression
```

## Comparing `sgw_tools-1.96.tar` & `sgw_tools-1.97.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 21:24:20.000000 sgw_tools-1.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 21:24:51.275636 sgw_tools-1.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-07 21:24:20.000000 sgw_tools-1.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:24:51.275636 sgw_tools-1.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-07 21:24:20.000000 sgw_tools-1.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-06-07 21:24:20.000000 sgw_tools-1.96/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 21:24:51.000000 sgw_tools-1.96/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:51.275636 sgw_tools-1.96/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:24:20.000000 sgw_tools-1.96/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-06-07 21:24:20.000000 sgw_tools-1.96/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 12:29:38.000000 sgw_tools-1.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:30:17.395610 sgw_tools-1.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-06 12:29:38.000000 sgw_tools-1.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:30:17.395610 sgw_tools-1.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 12:29:38.000000 sgw_tools-1.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-08-06 12:29:38.000000 sgw_tools-1.97/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 12:30:17.000000 sgw_tools-1.97/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:30:17.395610 sgw_tools-1.97/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:29:38.000000 sgw_tools-1.97/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-08-06 12:29:38.000000 sgw_tools-1.97/tests/test_biggraph.py
```

### Comparing `sgw_tools-1.96/LICENSE` & `sgw_tools-1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.96/PKG-INFO` & `sgw_tools-1.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.96
+Version: 1.97
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.96/setup.py` & `sgw_tools-1.97/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.96",
+    version="1.97",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.96/sgw_tools/__init__.py` & `sgw_tools-1.97/sgw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.96/sgw_tools/filters.py` & `sgw_tools-1.97/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.96/sgw_tools/graph.py` & `sgw_tools-1.97/sgw_tools/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         self._e[np.isclose(self._e, 0)] = 0
         e_min = np.min(self._e)
         assert e_min == self._e[0], "First eigenvalue is not the smallest"
         assert e_min >= 0, "Smallest eigenvalue is negative {}".format(e_min)
         e_nz = self._e[np.where(self._e>0)]
         if len(e_nz) > 0:
             self._lmin = e_nz[0]
+        else:
+            self._lmin = np.nan
 
         e_bound = self._get_upper_bound()
         self._e[np.isclose(self._e, e_bound)] = e_bound
         e_max = np.max(self._e)
         assert e_max == self._e[-1], "Last eigenvalue is not the largest"
         assert e_max <= e_bound, "Largest eigenvalue was {} but upper bound is {}".format(e_max, e_bound)
         self._lmax = e_max
```

### Comparing `sgw_tools-1.96/sgw_tools/graphs.py` & `sgw_tools-1.97/sgw_tools/graphs.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.96/sgw_tools/util.py` & `sgw_tools-1.97/sgw_tools/util.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.96/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.97/sgw_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw-tools
-Version: 1.96
+Version: 1.97
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.96/tests/test_biggraph.py` & `sgw_tools-1.97/tests/test_biggraph.py`

 * *Files identical despite different names*

