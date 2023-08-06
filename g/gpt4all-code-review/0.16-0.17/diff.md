# Comparing `tmp/gpt4all-code-review-0.16.tar.gz` & `tmp/gpt4all-code-review-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.16.tar", last modified: Sat Aug  5 20:52:28 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.17.tar", last modified: Sun Aug  6 10:52:43 2023, max compression
```

## Comparing `gpt4all-code-review-0.16.tar` & `gpt4all-code-review-0.17.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.944386 gpt4all-code-review-0.16/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2744 2023-08-05 20:52:28.944252 gpt4all-code-review-0.16/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2458 2023-08-05 16:00:14.000000 gpt4all-code-review-0.16/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.943353 gpt4all-code-review-0.16/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.16/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     5977 2023-08-05 20:46:16.000000 gpt4all-code-review-0.16/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.944078 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2744 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 20:52:28.944420 gpt4all-code-review-0.16/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-05 20:47:50.000000 gpt4all-code-review-0.16/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.087830 gpt4all-code-review-0.17/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3323 2023-08-06 10:52:43.087537 gpt4all-code-review-0.17/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3037 2023-08-06 10:52:31.000000 gpt4all-code-review-0.17/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.086069 gpt4all-code-review-0.17/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.17/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     5977 2023-08-05 20:46:16.000000 gpt4all-code-review-0.17/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.087119 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3323 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-06 10:52:43.087878 gpt4all-code-review-0.17/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-06 10:52:31.000000 gpt4all-code-review-0.17/setup.py
```

### Comparing `gpt4all-code-review-0.16/PKG-INFO` & `gpt4all-code-review-0.17/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.16
+Version: 0.17
 Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
+[![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI format](https://img.shields.io/pypi/format/gpt4all-code-review.svg)](https://pypi.python.org/pypi/gpt4all-code-review/)
+ 
 # Code Review Automation Tool
 
 This program is designed to assist developers by automating the process of code review. By leveraging a pre-trained standalone machine learning model (e.g., GPT-4), it reads source code files and provides suggestions for improvements.
 
 ## Features
 
 - **File Scanning:** Ability to scan a single file or all files in the current directory.
```

### Comparing `gpt4all-code-review-0.16/README.md` & `gpt4all-code-review-0.17/gpt4all_code_review.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: gpt4all-code-review
+Version: 0.17
+Summary: A self-contained tool for code review powered by GPT4ALL.
+Home-page: https://github.com/chigwell/gpt4all-code-review
+Author: Evgenii Evstafev
+Author-email: chigwel@gmail.com
+Description-Content-Type: text/markdown
+
+[![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI format](https://img.shields.io/pypi/format/gpt4all-code-review.svg)](https://pypi.python.org/pypi/gpt4all-code-review/)
+ 
 # Code Review Automation Tool
 
 This program is designed to assist developers by automating the process of code review. By leveraging a pre-trained standalone machine learning model (e.g., GPT-4), it reads source code files and provides suggestions for improvements.
 
 ## Features
 
 - **File Scanning:** Ability to scan a single file or all files in the current directory.
```

### Comparing `gpt4all-code-review-0.16/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.17/gpt4all_code_review/gpt4all_code_review.py`

 * *Files identical despite different names*

### Comparing `gpt4all-code-review-0.16/gpt4all_code_review.egg-info/PKG-INFO` & `gpt4all-code-review-0.17/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-Metadata-Version: 2.1
-Name: gpt4all-code-review
-Version: 0.16
-Summary: A self-contained tool for code review powered by GPT4ALL.
-Home-page: https://github.com/chigwell/gpt4all-code-review
-Author: Evgenii Evstafev
-Author-email: chigwel@gmail.com
-Description-Content-Type: text/markdown
-
+[![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+[![PyPI format](https://img.shields.io/pypi/format/gpt4all-code-review.svg)](https://pypi.python.org/pypi/gpt4all-code-review/)
+ 
 # Code Review Automation Tool
 
 This program is designed to assist developers by automating the process of code review. By leveraging a pre-trained standalone machine learning model (e.g., GPT-4), it reads source code files and provides suggestions for improvements.
 
 ## Features
 
 - **File Scanning:** Ability to scan a single file or all files in the current directory.
```

### Comparing `gpt4all-code-review-0.16/setup.py` & `gpt4all-code-review-0.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.16',
+    version='0.17',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
```

