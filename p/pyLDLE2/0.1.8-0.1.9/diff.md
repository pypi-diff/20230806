# Comparing `tmp/pyLDLE2-0.1.8.tar.gz` & `tmp/pyLDLE2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLDLE2-0.1.8.tar", last modified: Sat Jan 28 14:57:47 2023, max compression
+gzip compressed data, was "pyLDLE2-0.1.9.tar", last modified: Fri Feb  3 16:51:30 2023, max compression
```

## Comparing `pyLDLE2-0.1.8.tar` & `pyLDLE2-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxrwxr-x   0 dhruv     (1022) dhruv     (1022)        0 2023-01-28 14:57:47.599264 pyLDLE2-0.1.8/
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     1068 2022-08-01 17:24:40.000000 pyLDLE2-0.1.8/LICENSE
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     2559 2023-01-28 14:57:47.599264 pyLDLE2-0.1.8/PKG-INFO
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)      803 2022-08-01 17:24:29.000000 pyLDLE2-0.1.8/README.md
-drwxrwxr-x   0 dhruv     (1022) dhruv     (1022)        0 2023-01-28 14:57:47.599264 pyLDLE2-0.1.8/pyLDLE2/
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)        0 2022-08-01 17:24:29.000000 pyLDLE2-0.1.8/pyLDLE2/__init__.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     1702 2022-10-25 20:38:16.000000 pyLDLE2-0.1.8/pyLDLE2/_trash_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    27148 2022-08-31 17:47:51.000000 pyLDLE2-0.1.8/pyLDLE2/datasets.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     4912 2023-01-28 14:47:16.000000 pyLDLE2-0.1.8/pyLDLE2/gl_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    24735 2023-01-22 19:21:57.000000 pyLDLE2-0.1.8/pyLDLE2/global_reg_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    28674 2022-10-11 15:36:12.000000 pyLDLE2-0.1.8/pyLDLE2/global_views_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    17403 2022-09-15 15:44:08.000000 pyLDLE2-0.1.8/pyLDLE2/intermed_views_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     5009 2022-08-01 17:24:29.000000 pyLDLE2-0.1.8/pyLDLE2/ipge_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    24778 2022-11-07 17:46:33.000000 pyLDLE2-0.1.8/pyLDLE2/ldle_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    26996 2022-11-24 16:33:10.000000 pyLDLE2-0.1.8/pyLDLE2/local_views_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    12493 2023-01-22 19:21:09.000000 pyLDLE2-0.1.8/pyLDLE2/util_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    68903 2023-01-23 10:00:23.000000 pyLDLE2-0.1.8/pyLDLE2/visualize_.py
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)    19736 2022-10-04 05:48:17.000000 pyLDLE2-0.1.8/pyLDLE2/visualize_all.py
-drwxrwxr-x   0 dhruv     (1022) dhruv     (1022)        0 2023-01-28 14:57:47.599264 pyLDLE2-0.1.8/pyLDLE2.egg-info/
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)     2559 2023-01-28 14:57:47.000000 pyLDLE2-0.1.8/pyLDLE2.egg-info/PKG-INFO
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)      427 2023-01-28 14:57:47.000000 pyLDLE2-0.1.8/pyLDLE2.egg-info/SOURCES.txt
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)        1 2023-01-28 14:57:47.000000 pyLDLE2-0.1.8/pyLDLE2.egg-info/dependency_links.txt
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)        8 2023-01-28 14:57:47.000000 pyLDLE2-0.1.8/pyLDLE2.egg-info/top_level.txt
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)      989 2023-01-28 14:53:03.000000 pyLDLE2-0.1.8/pyproject.toml
--rw-rw-r--   0 dhruv     (1022) dhruv     (1022)       38 2023-01-28 14:57:47.599264 pyLDLE2-0.1.8/setup.cfg
+drwxr-xr-x   0 dhkohli    (501) staff       (20)        0 2023-02-03 16:51:30.715191 pyLDLE2-0.1.9/
+-rw-r--r--   0 dhkohli    (501) staff       (20)     1068 2022-07-21 17:01:48.000000 pyLDLE2-0.1.9/LICENSE
+-rw-r--r--   0 dhkohli    (501) staff       (20)     2559 2023-02-03 16:51:30.715027 pyLDLE2-0.1.9/PKG-INFO
+-rw-r--r--   0 dhkohli    (501) staff       (20)      803 2022-07-21 17:39:14.000000 pyLDLE2-0.1.9/README.md
+drwxr-xr-x   0 dhkohli    (501) staff       (20)        0 2023-02-03 16:51:30.714114 pyLDLE2-0.1.9/pyLDLE2/
+-rw-r--r--   0 dhkohli    (501) staff       (20)     4912 2023-01-28 15:01:57.000000 pyLDLE2-0.1.9/pyLDLE2/gl_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    24735 2023-01-28 15:01:57.000000 pyLDLE2-0.1.9/pyLDLE2/global_reg_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    28674 2022-11-25 16:17:05.000000 pyLDLE2-0.1.9/pyLDLE2/global_views_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    24778 2022-11-25 16:17:05.000000 pyLDLE2-0.1.9/pyLDLE2/ldle_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    26996 2022-11-25 16:17:05.000000 pyLDLE2-0.1.9/pyLDLE2/local_views_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    12493 2023-01-28 15:01:57.000000 pyLDLE2-0.1.9/pyLDLE2/util_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    68903 2023-01-28 15:01:57.000000 pyLDLE2-0.1.9/pyLDLE2/visualize_.py
+-rw-r--r--   0 dhkohli    (501) staff       (20)    19736 2022-11-25 16:17:05.000000 pyLDLE2-0.1.9/pyLDLE2/visualize_all.py
+drwxr-xr-x   0 dhkohli    (501) staff       (20)        0 2023-02-03 16:51:30.714843 pyLDLE2-0.1.9/pyLDLE2.egg-info/
+-rw-r--r--   0 dhkohli    (501) staff       (20)     2559 2023-02-03 16:51:30.000000 pyLDLE2-0.1.9/pyLDLE2.egg-info/PKG-INFO
+-rw-r--r--   0 dhkohli    (501) staff       (20)      324 2023-02-03 16:51:30.000000 pyLDLE2-0.1.9/pyLDLE2.egg-info/SOURCES.txt
+-rw-r--r--   0 dhkohli    (501) staff       (20)        1 2023-02-03 16:51:30.000000 pyLDLE2-0.1.9/pyLDLE2.egg-info/dependency_links.txt
+-rw-r--r--   0 dhkohli    (501) staff       (20)        8 2023-02-03 16:51:30.000000 pyLDLE2-0.1.9/pyLDLE2.egg-info/top_level.txt
+-rw-r--r--   0 dhkohli    (501) staff       (20)      989 2023-02-03 16:51:00.000000 pyLDLE2-0.1.9/pyproject.toml
+-rw-r--r--   0 dhkohli    (501) staff       (20)       38 2023-02-03 16:51:30.715246 pyLDLE2-0.1.9/setup.cfg
```

### Comparing `pyLDLE2-0.1.8/LICENSE` & `pyLDLE2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/PKG-INFO` & `pyLDLE2-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLDLE2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Low Distortion Local Eigenmaps and its variations.
 Author: Dhruv Kohli, Alex Cloninger, Gal Mishne
 License: MIT License
         
         Copyright (c) 2022, Dhruv Kohli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/chiggum/pyLDLE2
 Project-URL: Bug Tracker, https://github.com/chiggum/pyLDLE2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyLDLE2
 ========
 
 pyLDLE2 provides an implementation of our manifold learning algorithm [LDLE](http://jmlr.org/papers/v22/21-0131.html) and several variations of it.
```

### Comparing `pyLDLE2-0.1.8/README.md` & `pyLDLE2-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/gl_.py` & `pyLDLE2-0.1.9/pyLDLE2/gl_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/global_reg_.py` & `pyLDLE2-0.1.9/pyLDLE2/global_reg_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/global_views_.py` & `pyLDLE2-0.1.9/pyLDLE2/global_views_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/ldle_.py` & `pyLDLE2-0.1.9/pyLDLE2/ldle_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/local_views_.py` & `pyLDLE2-0.1.9/pyLDLE2/local_views_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/util_.py` & `pyLDLE2-0.1.9/pyLDLE2/util_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/visualize_.py` & `pyLDLE2-0.1.9/pyLDLE2/visualize_.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2/visualize_all.py` & `pyLDLE2-0.1.9/pyLDLE2/visualize_all.py`

 * *Files identical despite different names*

### Comparing `pyLDLE2-0.1.8/pyLDLE2.egg-info/PKG-INFO` & `pyLDLE2-0.1.9/pyLDLE2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLDLE2
-Version: 0.1.8
+Version: 0.1.9
 Summary: Low Distortion Local Eigenmaps and its variations.
 Author: Dhruv Kohli, Alex Cloninger, Gal Mishne
 License: MIT License
         
         Copyright (c) 2022, Dhruv Kohli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,15 +25,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/chiggum/pyLDLE2
 Project-URL: Bug Tracker, https://github.com/chiggum/pyLDLE2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyLDLE2
 ========
 
 pyLDLE2 provides an implementation of our manifold learning algorithm [LDLE](http://jmlr.org/papers/v22/21-0131.html) and several variations of it.
```

### Comparing `pyLDLE2-0.1.8/pyproject.toml` & `pyLDLE2-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
             "scs==3.2.0",
             "seaborn==0.11.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyLDLE2"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Dhruv Kohli, Alex Cloninger, Gal Mishne" },
 ]
 description = "Low Distortion Local Eigenmaps and its variations."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

