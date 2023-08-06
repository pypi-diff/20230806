# Comparing `tmp/LinkedList_575-1.0.0.tar.gz` & `tmp/LinkedList_575-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LinkedList_575-1.0.0.tar", last modified: Sun Aug  6 10:53:35 2023, max compression
+gzip compressed data, was "LinkedList_575-1.0.1.tar", last modified: Sun Aug  6 11:59:24 2023, max compression
```

## Comparing `LinkedList_575-1.0.0.tar` & `LinkedList_575-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 10:53:35.553305 LinkedList_575-1.0.0/
--rw-rw-rw-   0        0        0    35811 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-06 10:53:35.540203 LinkedList_575-1.0.0/LinkedList/
--rw-rw-rw-   0        0        0        0 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LinkedList/__init__.py
--rw-rw-rw-   0        0        0    34256 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LinkedList/base_list.py
--rw-rw-rw-   0        0        0    18242 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LinkedList/linked_list.py
--rw-rw-rw-   0        0        0     3081 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LinkedList/linked_list_iterator.py
--rw-rw-rw-   0        0        0     1229 2023-08-06 09:53:52.000000 LinkedList_575-1.0.0/LinkedList/node.py
-drwxrwxrwx   0        0        0        0 2023-08-06 10:53:35.551944 LinkedList_575-1.0.0/LinkedList_575.egg-info/
--rw-rw-rw-   0        0        0    22433 2023-08-06 10:53:35.000000 LinkedList_575-1.0.0/LinkedList_575.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-08-06 10:53:35.000000 LinkedList_575-1.0.0/LinkedList_575.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 10:53:35.000000 LinkedList_575-1.0.0/LinkedList_575.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 10:53:35.000000 LinkedList_575-1.0.0/LinkedList_575.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22433 2023-08-06 10:53:35.553305 LinkedList_575-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    21025 2023-08-06 10:43:57.000000 LinkedList_575-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-06 10:53:35.553305 LinkedList_575-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4335 2023-08-06 10:52:51.000000 LinkedList_575-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 11:59:24.814195 LinkedList_575-1.0.1/
+-rw-rw-rw-   0        0        0    35811 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-06 11:59:24.807250 LinkedList_575-1.0.1/LinkedList/
+-rw-rw-rw-   0        0        0        0 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LinkedList/__init__.py
+-rw-rw-rw-   0        0        0    34256 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LinkedList/base_list.py
+-rw-rw-rw-   0        0        0    18242 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LinkedList/linked_list.py
+-rw-rw-rw-   0        0        0     3081 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LinkedList/linked_list_iterator.py
+-rw-rw-rw-   0        0        0     1229 2023-08-06 09:53:52.000000 LinkedList_575-1.0.1/LinkedList/node.py
+drwxrwxrwx   0        0        0        0 2023-08-06 11:59:24.814195 LinkedList_575-1.0.1/LinkedList_575.egg-info/
+-rw-rw-rw-   0        0        0    22306 2023-08-06 11:59:24.000000 LinkedList_575-1.0.1/LinkedList_575.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-08-06 11:59:24.000000 LinkedList_575-1.0.1/LinkedList_575.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 11:59:24.000000 LinkedList_575-1.0.1/LinkedList_575.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 11:59:24.000000 LinkedList_575-1.0.1/LinkedList_575.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22306 2023-08-06 11:59:24.814195 LinkedList_575-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20898 2023-08-06 11:57:35.000000 LinkedList_575-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-06 11:59:24.827980 LinkedList_575-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4335 2023-08-06 11:57:35.000000 LinkedList_575-1.0.1/setup.py
```

### Comparing `LinkedList_575-1.0.0/LICENSE` & `LinkedList_575-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LinkedList_575-1.0.0/LinkedList/base_list.py` & `LinkedList_575-1.0.1/LinkedList/base_list.py`

 * *Files identical despite different names*

### Comparing `LinkedList_575-1.0.0/LinkedList/linked_list.py` & `LinkedList_575-1.0.1/LinkedList/linked_list.py`

 * *Files identical despite different names*

### Comparing `LinkedList_575-1.0.0/LinkedList/linked_list_iterator.py` & `LinkedList_575-1.0.1/LinkedList/linked_list_iterator.py`

 * *Files identical despite different names*

### Comparing `LinkedList_575-1.0.0/LinkedList/node.py` & `LinkedList_575-1.0.1/LinkedList/node.py`

 * *Files identical despite different names*

### Comparing `LinkedList_575-1.0.0/LinkedList_575.egg-info/PKG-INFO` & `LinkedList_575-1.0.1/LinkedList_575.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinkedList-575
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for LinkedList data structure.
 Home-page: https://github.com/Saqibs575/LinkedList
 Author: Saqib Shaikh
 Author-email: saquibs575@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/Saqibs575/LinkedList
 Project-URL: Bug Reports, https://github.com/Saqibs575/LinkedList/issues
@@ -32,26 +32,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## **LinkedList : Simple and efficient way to access LinkedList in python** <br>
-[![PyPI version](https://badge.fury.io/py/singly-linkedlist.svg)](https://badge.fury.io/py/singly-linkedlist) 
-[![PyPI](https://img.shields.io/pypi/v/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - License](https://img.shields.io/pypi/l/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Status](https://img.shields.io/pypi/status/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
+[![PyPI version](https://badge.fury.io/py/LinkedList-575.svg)](https://badge.fury.io/py/LinkedList-575) 
+[![PyPI](https://img.shields.io/pypi/v/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - License](https://img.shields.io/pypi/l/LinkedList-575)](https://pypi.org/project/LinkedList_575/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linkedlist-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - Status](https://img.shields.io/pypi/status/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
 
-![GitHub](https://img.shields.io/github/license/Saqibs575/example)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/example?label=Pull%20Requests)](https://github.com/Saqibs575/example/pulls)
-[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/example?label=GitHub%20Issues)](https://github.com/Saqibs575/example/issues)
+![GitHub](https://img.shields.io/github/license/Saqibs575/LinkedList)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/LinkedList?label=Pull%20Requests)](https://github.com/Saqibs575/LinkedList/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/LinkedList?label=GitHub%20Issues)](https://github.com/Saqibs575/LinkedList/issues)
 [![GitHub closed issues](https://img.shields.io/github/issues-closed/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/issues?q=is%3Aissue+is%3Aclosed)
-[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/example)](https://github.com/Saqibs575/example/commits/main)
+[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/commits/main)
 [![GitHub contributors](https://img.shields.io/github/contributors/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/graphs/contributors)
 [![GitHub code size](https://img.shields.io/github/languages/code-size/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 [![GitHub stars](https://img.shields.io/github/stars/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/network)
 [![GitHub top language](https://img.shields.io/github/languages/top/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 
 -----------------------------
```

### Comparing `LinkedList_575-1.0.0/PKG-INFO` & `LinkedList_575-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LinkedList_575
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for LinkedList data structure.
 Home-page: https://github.com/Saqibs575/LinkedList
 Author: Saqib Shaikh
 Author-email: saquibs575@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/Saqibs575/LinkedList
 Project-URL: Bug Reports, https://github.com/Saqibs575/LinkedList/issues
@@ -32,26 +32,25 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## **LinkedList : Simple and efficient way to access LinkedList in python** <br>
-[![PyPI version](https://badge.fury.io/py/singly-linkedlist.svg)](https://badge.fury.io/py/singly-linkedlist) 
-[![PyPI](https://img.shields.io/pypi/v/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - License](https://img.shields.io/pypi/l/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Status](https://img.shields.io/pypi/status/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
+[![PyPI version](https://badge.fury.io/py/LinkedList-575.svg)](https://badge.fury.io/py/LinkedList-575) 
+[![PyPI](https://img.shields.io/pypi/v/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - License](https://img.shields.io/pypi/l/LinkedList-575)](https://pypi.org/project/LinkedList_575/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linkedlist-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - Status](https://img.shields.io/pypi/status/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
 
-![GitHub](https://img.shields.io/github/license/Saqibs575/example)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/example?label=Pull%20Requests)](https://github.com/Saqibs575/example/pulls)
-[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/example?label=GitHub%20Issues)](https://github.com/Saqibs575/example/issues)
+![GitHub](https://img.shields.io/github/license/Saqibs575/LinkedList)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/LinkedList?label=Pull%20Requests)](https://github.com/Saqibs575/LinkedList/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/LinkedList?label=GitHub%20Issues)](https://github.com/Saqibs575/LinkedList/issues)
 [![GitHub closed issues](https://img.shields.io/github/issues-closed/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/issues?q=is%3Aissue+is%3Aclosed)
-[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/example)](https://github.com/Saqibs575/example/commits/main)
+[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/commits/main)
 [![GitHub contributors](https://img.shields.io/github/contributors/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/graphs/contributors)
 [![GitHub code size](https://img.shields.io/github/languages/code-size/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 [![GitHub stars](https://img.shields.io/github/stars/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/network)
 [![GitHub top language](https://img.shields.io/github/languages/top/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 
 -----------------------------
```

### Comparing `LinkedList_575-1.0.0/README.md` & `LinkedList_575-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 ## **LinkedList : Simple and efficient way to access LinkedList in python** <br>
-[![PyPI version](https://badge.fury.io/py/singly-linkedlist.svg)](https://badge.fury.io/py/singly-linkedlist) 
-[![PyPI](https://img.shields.io/pypi/v/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - License](https://img.shields.io/pypi/l/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
-[![PyPI - Status](https://img.shields.io/pypi/status/singly_linkedlist)](https://pypi.org/project/singly_linkedlist/)
+[![PyPI version](https://badge.fury.io/py/LinkedList-575.svg)](https://badge.fury.io/py/LinkedList-575) 
+[![PyPI](https://img.shields.io/pypi/v/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - License](https://img.shields.io/pypi/l/LinkedList-575)](https://pypi.org/project/LinkedList_575/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/linkedlist-575)](https://pypi.org/project/LinkedList-575/)
+[![PyPI - Status](https://img.shields.io/pypi/status/LinkedList-575)](https://pypi.org/project/LinkedList-575/)
 
-![GitHub](https://img.shields.io/github/license/Saqibs575/example)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/example?label=Pull%20Requests)](https://github.com/Saqibs575/example/pulls)
-[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/example?label=GitHub%20Issues)](https://github.com/Saqibs575/example/issues)
+![GitHub](https://img.shields.io/github/license/Saqibs575/LinkedList)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/Saqibs575/LinkedList?label=Pull%20Requests)](https://github.com/Saqibs575/LinkedList/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/Saqibs575/LinkedList?label=GitHub%20Issues)](https://github.com/Saqibs575/LinkedList/issues)
 [![GitHub closed issues](https://img.shields.io/github/issues-closed/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/issues?q=is%3Aissue+is%3Aclosed)
-[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/example)](https://github.com/Saqibs575/example/commits/main)
+[![GitHub last commit](https://img.shields.io/github/last-commit/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/commits/main)
 [![GitHub contributors](https://img.shields.io/github/contributors/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/graphs/contributors)
 [![GitHub code size](https://img.shields.io/github/languages/code-size/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 [![GitHub stars](https://img.shields.io/github/stars/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList/network)
 [![GitHub top language](https://img.shields.io/github/languages/top/Saqibs575/LinkedList)](https://github.com/Saqibs575/LinkedList)
 
 -----------------------------
```

### Comparing `LinkedList_575-1.0.0/setup.py` & `LinkedList_575-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if '-e .' in requirements:
         return requirements[:-1]
     else:
         return requirements
 
 
 DIR_NAME = Path(__file__).parent
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 AUTHOR = 'Saqib Shaikh'
 REPO_NAME = 'LinkedList'
 PROJECT_NAME = 'LinkedList_575'
 AUTHOR_USER_NAME = 'Saqibs575'
 AUTHOR_EMAIL = 'saquibs575@gmail.com'
 LICENSE = 'GNU General Public License v3.0'
 LONG_DESCRIPTION = (DIR_NAME / "README.md").read_text()
```

