# Comparing `tmp/pyecosystem-0.0.1.tar.gz` & `tmp/pyecosystem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecosystem-0.0.1.tar", last modified: Sun Aug  6 09:08:28 2023, max compression
+gzip compressed data, was "pyecosystem-0.0.2.tar", last modified: Sun Aug  6 09:36:42 2023, max compression
```

## Comparing `pyecosystem-0.0.1.tar` & `pyecosystem-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-05 13:20:31.000000 pyecosystem-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      600 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-06 09:08:28.006286 pyecosystem-0.0.1/data/
--rw-rw-rw-   0        0        0       19 2023-07-06 11:29:41.000000 pyecosystem-0.0.1/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/data/xml/
--rw-rw-rw-   0        0        0    20518 2023-07-06 06:51:00.000000 pyecosystem-0.0.1/data/xml/XMLNode.py
--rw-rw-rw-   0        0        0     9165 2023-07-05 13:23:04.000000 pyecosystem-0.0.1/data/xml/XMLParser.py
--rw-rw-rw-   0        0        0    12304 2023-07-06 07:34:36.000000 pyecosystem-0.0.1/data/xml/XMLPath.py
--rw-rw-rw-   0        0        0     9911 2023-07-04 13:04:14.000000 pyecosystem-0.0.1/data/xml/XMLTree.py
--rw-rw-rw-   0        0        0      145 2023-07-05 13:22:34.000000 pyecosystem-0.0.1/data/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/pyecosystem.egg-info/
--rw-rw-rw-   0        0        0      600 2023-08-06 09:08:27.000000 pyecosystem-0.0.1/pyecosystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-08-06 09:08:27.000000 pyecosystem-0.0.1/pyecosystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:08:27.000000 pyecosystem-0.0.1/pyecosystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-06 09:08:27.000000 pyecosystem-0.0.1/pyecosystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-08-06 09:08:10.000000 pyecosystem-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:08:28.021875 pyecosystem-0.0.1/workflow/
--rw-rw-rw-   0        0        0      112 2023-08-04 07:30:36.000000 pyecosystem-0.0.1/workflow/Errors.py
--rw-rw-rw-   0        0        0     3193 2023-08-06 08:11:10.000000 pyecosystem-0.0.1/workflow/Executable.py
--rw-rw-rw-   0        0        0      416 2023-08-04 10:09:38.000000 pyecosystem-0.0.1/workflow/Step.py
--rw-rw-rw-   0        0        0     3114 2023-08-06 08:13:11.000000 pyecosystem-0.0.1/workflow/Workflow.py
--rw-rw-rw-   0        0        0        0 2023-08-06 08:03:33.000000 pyecosystem-0.0.1/workflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:36:42.568541 pyecosystem-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-05 13:20:31.000000 pyecosystem-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      845 2023-08-06 09:36:42.568541 pyecosystem-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 09:36:42.537325 pyecosystem-0.0.2/data/
+-rw-rw-rw-   0        0        0       19 2023-07-06 11:29:41.000000 pyecosystem-0.0.2/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:36:42.552953 pyecosystem-0.0.2/data/xml/
+-rw-rw-rw-   0        0        0    20518 2023-07-06 06:51:00.000000 pyecosystem-0.0.2/data/xml/XMLNode.py
+-rw-rw-rw-   0        0        0     9165 2023-07-05 13:23:04.000000 pyecosystem-0.0.2/data/xml/XMLParser.py
+-rw-rw-rw-   0        0        0    12304 2023-07-06 07:34:36.000000 pyecosystem-0.0.2/data/xml/XMLPath.py
+-rw-rw-rw-   0        0        0     9911 2023-07-04 13:04:14.000000 pyecosystem-0.0.2/data/xml/XMLTree.py
+-rw-rw-rw-   0        0        0      145 2023-07-05 13:22:34.000000 pyecosystem-0.0.2/data/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:36:42.552953 pyecosystem-0.0.2/pyecosystem.egg-info/
+-rw-rw-rw-   0        0        0      845 2023-08-06 09:36:42.000000 pyecosystem-0.0.2/pyecosystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-08-06 09:36:42.000000 pyecosystem-0.0.2/pyecosystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:36:42.000000 pyecosystem-0.0.2/pyecosystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-06 09:36:42.000000 pyecosystem-0.0.2/pyecosystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-06 09:36:42.000000 pyecosystem-0.0.2/pyecosystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:36:42.568541 pyecosystem-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-08-06 09:36:18.000000 pyecosystem-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:36:42.552953 pyecosystem-0.0.2/workflow/
+-rw-rw-rw-   0        0        0      112 2023-08-04 07:30:36.000000 pyecosystem-0.0.2/workflow/Errors.py
+-rw-rw-rw-   0        0        0     3193 2023-08-06 08:11:10.000000 pyecosystem-0.0.2/workflow/Executable.py
+-rw-rw-rw-   0        0        0      416 2023-08-04 10:09:38.000000 pyecosystem-0.0.2/workflow/Step.py
+-rw-rw-rw-   0        0        0     3114 2023-08-06 08:13:11.000000 pyecosystem-0.0.2/workflow/Workflow.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 08:03:33.000000 pyecosystem-0.0.2/workflow/__init__.py
```

### Comparing `pyecosystem-0.0.1/LICENSE` & `pyecosystem-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/data/xml/XMLNode.py` & `pyecosystem-0.0.2/data/xml/XMLNode.py`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/data/xml/XMLParser.py` & `pyecosystem-0.0.2/data/xml/XMLParser.py`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/data/xml/XMLPath.py` & `pyecosystem-0.0.2/data/xml/XMLPath.py`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/data/xml/XMLTree.py` & `pyecosystem-0.0.2/data/xml/XMLTree.py`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/setup.py` & `pyecosystem-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from setuptools import setup, find_packages
 
 # Same content as provided in the previous setup.py example
 
 setup(
     name="pyecosystem",
-    version="0.0.1",
+    version="0.0.2",
     author="Smeet Kevadiya",
     author_email="",
     description="an ecosystem of various data transformers, structure builders, manipulators, workflows",
     long_description="an ecosystem of various data transformers, structure builders, manipulators, workflows",
     long_description_content_type="text/markdown",
-    url="https://github.com/kevadiyasmt/ecosystem",
+    url="https://github.com/kevadiyasmt/pyecosystem",
     packages=find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
+		'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
-        # List any dependencies here
+        'asyncio'
     ],
     python_requires=">=3.7",
 )
```

### Comparing `pyecosystem-0.0.1/workflow/Executable.py` & `pyecosystem-0.0.2/workflow/Executable.py`

 * *Files identical despite different names*

### Comparing `pyecosystem-0.0.1/workflow/Workflow.py` & `pyecosystem-0.0.2/workflow/Workflow.py`

 * *Files identical despite different names*

