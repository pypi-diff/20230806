# Comparing `tmp/HaploDynamics-0.1b1.tar.gz` & `tmp/HaploDynamics-0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b1.tar", last modified: Sun Aug  6 18:42:58 2023, max compression
+gzip compressed data, was "HaploDynamics-0.1b2.tar", last modified: Sun Aug  6 18:47:44 2023, max compression
```

## Comparing `HaploDynamics-0.1b1.tar` & `HaploDynamics-0.1b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:42:58.149832 HaploDynamics-0.1b1/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:42:58.149832 HaploDynamics-0.1b1/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-06 17:58:56.000000 HaploDynamics-0.1b1/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-06 18:02:03.000000 HaploDynamics-0.1b1/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:42:58.149832 HaploDynamics-0.1b1/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-06 17:21:31.000000 HaploDynamics-0.1b1/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-06 17:50:46.000000 HaploDynamics-0.1b1/HaploDX/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:42:58.149832 HaploDynamics-0.1b1/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:42:58.000000 HaploDynamics-0.1b1/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      301 2023-08-06 18:42:58.000000 HaploDynamics-0.1b1/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-06 18:42:58.000000 HaploDynamics-0.1b1/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-06 18:42:58.000000 HaploDynamics-0.1b1/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       18 2023-08-06 18:42:58.000000 HaploDynamics-0.1b1/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-06 17:21:31.000000 HaploDynamics-0.1b1/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:42:58.149832 HaploDynamics-0.1b1/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     7514 2023-08-06 17:21:31.000000 HaploDynamics-0.1b1/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-06 18:42:58.153832 HaploDynamics-0.1b1/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-06 18:40:50.000000 HaploDynamics-0.1b1/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/Framework/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-06 17:58:56.000000 HaploDynamics-0.1b2/Framework/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-06 18:02:03.000000 HaploDynamics-0.1b2/Framework/future.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/HaploDX/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/HaploDX/HaploDX.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-06 17:50:46.000000 HaploDynamics-0.1b2/HaploDX/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      301 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       18 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)     7514 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-06 18:46:05.000000 HaploDynamics-0.1b2/setup.py
```

### Comparing `HaploDynamics-0.1b1/HaploDX/HaploDX.py` & `HaploDynamics-0.1b2/HaploDX/HaploDX.py`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b1/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.1b2/HaploDynamics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b1
+Version: 0.1b2
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.1.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b1 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b2 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.1.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b1/LICENSE` & `HaploDynamics-0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b1/PKG-INFO` & `HaploDynamics-0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b1
+Version: 0.1b2
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.1.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b1 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b2 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.1.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `HaploDynamics-0.1b1/README.md` & `HaploDynamics-0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b1/setup.py` & `HaploDynamics-0.1b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDX','Framework']),
-  version = 'v0.1-beta.1',
+  version = 'v0.1-beta.2',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.1.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

