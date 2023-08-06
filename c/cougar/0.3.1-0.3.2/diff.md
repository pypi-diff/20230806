# Comparing `tmp/cougar-0.3.1.tar.gz` & `tmp/cougar-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cougar-0.3.1.tar", last modified: Sun Aug  6 07:10:07 2023, max compression
+gzip compressed data, was "cougar-0.3.2.tar", last modified: Sun Aug  6 07:18:22 2023, max compression
```

## Comparing `cougar-0.3.1.tar` & `cougar-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:10:07.344910 cougar-0.3.1/
--rw-r--r--   0 runner     (501) staff       (20)    11357 2023-08-06 07:09:39.000000 cougar-0.3.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1451 2023-08-06 07:10:07.344455 cougar-0.3.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      401 2023-08-06 07:09:39.000000 cougar-0.3.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:10:07.340452 cougar-0.3.1/cougar/
--rw-r--r--   0 runner     (501) staff       (20)      287 2023-08-06 07:09:39.000000 cougar-0.3.1/cougar/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:10:07.343411 cougar-0.3.1/cougar/numpy/
--rw-r--r--   0 runner     (501) staff       (20)       26 2023-08-06 07:09:39.000000 cougar-0.3.1/cougar/numpy/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1470 2023-08-06 07:09:39.000000 cougar-0.3.1/cougar/numpy/functional.py
--rw-r--r--   0 runner     (501) staff       (20)     2335 2023-08-06 07:09:39.000000 cougar-0.3.1/cougar/rolling.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:10:07.342517 cougar-0.3.1/cougar.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1451 2023-08-06 07:10:07.000000 cougar-0.3.1/cougar.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      296 2023-08-06 07:10:07.000000 cougar-0.3.1/cougar.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-08-06 07:10:07.000000 cougar-0.3.1/cougar.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2023-08-06 07:10:07.000000 cougar-0.3.1/cougar.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-08-06 07:10:07.000000 cougar-0.3.1/cougar.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      978 2023-08-06 07:09:39.000000 cougar-0.3.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-08-06 07:10:07.345030 cougar-0.3.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1360 2023-08-06 07:09:59.000000 cougar-0.3.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:10:07.344018 cougar-0.3.1/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-08-06 07:09:39.000000 cougar-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:18:22.019688 cougar-0.3.2/
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2023-08-06 07:16:28.000000 cougar-0.3.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1451 2023-08-06 07:18:22.019222 cougar-0.3.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      401 2023-08-06 07:16:28.000000 cougar-0.3.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:18:22.015081 cougar-0.3.2/cougar/
+-rw-r--r--   0 runner     (501) staff       (20)      277 2023-08-06 07:16:28.000000 cougar-0.3.2/cougar/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:18:22.018212 cougar-0.3.2/cougar/numpy/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2023-08-06 07:16:28.000000 cougar-0.3.2/cougar/numpy/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1470 2023-08-06 07:16:28.000000 cougar-0.3.2/cougar/numpy/functional.py
+-rw-r--r--   0 runner     (501) staff       (20)     2335 2023-08-06 07:16:28.000000 cougar-0.3.2/cougar/rolling.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:18:22.017297 cougar-0.3.2/cougar.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1451 2023-08-06 07:18:21.000000 cougar-0.3.2/cougar.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      296 2023-08-06 07:18:22.000000 cougar-0.3.2/cougar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-08-06 07:18:21.000000 cougar-0.3.2/cougar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2023-08-06 07:18:21.000000 cougar-0.3.2/cougar.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-08-06 07:18:21.000000 cougar-0.3.2/cougar.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      978 2023-08-06 07:16:29.000000 cougar-0.3.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-08-06 07:18:22.019813 cougar-0.3.2/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1360 2023-08-06 07:18:12.000000 cougar-0.3.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-08-06 07:18:22.018741 cougar-0.3.2/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-08-06 07:16:30.000000 cougar-0.3.2/tests/__init__.py
```

### Comparing `cougar-0.3.1/LICENSE` & `cougar-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cougar-0.3.1/PKG-INFO` & `cougar-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Description: # cougar
```

### Comparing `cougar-0.3.1/cougar/numpy/functional.py` & `cougar-0.3.2/cougar/numpy/functional.py`

 * *Files identical despite different names*

### Comparing `cougar-0.3.1/cougar/rolling.c` & `cougar-0.3.2/cougar/rolling.c`

 * *Files identical despite different names*

### Comparing `cougar-0.3.1/cougar.egg-info/PKG-INFO` & `cougar-0.3.2/cougar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cougar
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Yunchong Gan
 Author-email: yunchong@pku.edu.cn
 License: UNKNOWN
 Description: # cougar
```

### Comparing `cougar-0.3.1/pyproject.toml` & `cougar-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cougar-0.3.1/setup.py` & `cougar-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import Extension, find_packages, setup
 
 project_dir = Path(__file__).parent.resolve()
 long_description = (project_dir / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cougar",
-    version="0.3.1",
+    version="0.3.2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yunchong Gan",
     author_email="yunchong@pku.edu.cn",
     packages=find_packages(),
     requires=["numpy"],
     install_requires=["numpy"],
```

