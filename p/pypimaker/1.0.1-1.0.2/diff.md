# Comparing `tmp/pypimaker-1.0.1.tar.gz` & `tmp/pypimaker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypimaker-1.0.1.tar", last modified: Sun Aug  6 02:11:25 2023, max compression
+gzip compressed data, was "dist/pypimaker-1.0.2.tar", last modified: Sun Aug  6 02:15:44 2023, max compression
```

## Comparing `pypimaker-1.0.1.tar` & `pypimaker-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455730 pypimaker-1.0.1/
--rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 02:11:19.000000 pypimaker-1.0.1/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:11:25.455575 pypimaker-1.0.1/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     3589 2023-08-06 02:10:11.000000 pypimaker-1.0.1/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.452862 pypimaker-1.0.1/pypimaker.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/top_level.txt
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 02:11:25.455792 pypimaker-1.0.1/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1343 2023-08-06 02:11:25.000000 pypimaker-1.0.1/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.453858 pypimaker-1.0.1/src/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.1/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.1/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)      862 2023-08-06 02:09:48.000000 pypimaker-1.0.1/src/reset.py
--rw-r--r--   0 holly      (501) staff       (20)     7723 2023-08-06 02:09:43.000000 pypimaker-1.0.1/src/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.454576 pypimaker-1.0.1/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     7472 2023-08-06 02:07:27.000000 pypimaker-1.0.1/src/ui/AuthorInfoSelector.py
--rw-r--r--   0 holly      (501) staff       (20)     3859 2023-08-06 02:08:23.000000 pypimaker-1.0.1/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     8246 2023-08-06 02:08:20.000000 pypimaker-1.0.1/src/ui/OptionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.1/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.1/src/ui/navigation.py
--rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 02:09:51.000000 pypimaker-1.0.1/src/upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455034 pypimaker-1.0.1/tests/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.1/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.1/tests/test_upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455348 pypimaker-1.0.1/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.1/tests/ui/test_navigation.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164899 pypimaker-1.0.2/
+-rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 02:11:19.000000 pypimaker-1.0.2/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:15:44.164739 pypimaker-1.0.2/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     3589 2023-08-06 02:14:12.000000 pypimaker-1.0.2/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.161964 pypimaker-1.0.2/pypimaker.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/top_level.txt
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 02:15:44.164957 pypimaker-1.0.2/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1339 2023-08-06 02:15:43.000000 pypimaker-1.0.2/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.162912 pypimaker-1.0.2/src/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.2/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.2/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)      862 2023-08-06 02:09:48.000000 pypimaker-1.0.2/src/reset.py
+-rw-r--r--   0 holly      (501) staff       (20)     7729 2023-08-06 02:13:45.000000 pypimaker-1.0.2/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.163815 pypimaker-1.0.2/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     7472 2023-08-06 02:07:27.000000 pypimaker-1.0.2/src/ui/AuthorInfoSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)     3859 2023-08-06 02:08:23.000000 pypimaker-1.0.2/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     8246 2023-08-06 02:08:20.000000 pypimaker-1.0.2/src/ui/OptionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.2/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.2/src/ui/navigation.py
+-rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 02:09:51.000000 pypimaker-1.0.2/src/upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164250 pypimaker-1.0.2/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.2/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.2/tests/test_upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164519 pypimaker-1.0.2/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.2/tests/ui/test_navigation.py
```

### Comparing `pypimaker-1.0.1/LICENSE` & `pypimaker-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/PKG-INFO` & `pypimaker-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -85,15 +85,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-- 1.0.1
+- 1.0.2
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.1/README.md` & `pypimaker-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-- 1.0.1
+- 1.0.2
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.1/pypimaker.egg-info/PKG-INFO` & `pypimaker-1.0.2/pypimaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.1
+Version: 1.0.2
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -85,15 +85,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-- 1.0.1
+- 1.0.2
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.1/setup.py` & `pypimaker-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='pypimaker',  # Required
-    version='1.0.1', # Required 
+    version='1.0.2', # Required 
     description='Software designed for simplifying PyPI Python package setups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/pypimaker',
     author='Brian Davis',
         classifiers=[  # Defined at https://pypi.org/classifiers/
             'Intended Audience :: Developers',
@@ -29,9 +29,9 @@
         'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
         'Source': 'https://github.com/bdavis222/',
     },
     entry_points={
         'console_scripts': [
             'pypimaker = src.__main__:main'
         ]
-        }
+    }
 )
```

### Comparing `pypimaker-1.0.1/src/__main__.py` & `pypimaker-1.0.2/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/files.py` & `pypimaker-1.0.2/src/files.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/reset.py` & `pypimaker-1.0.2/src/reset.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/strings.py` & `pypimaker-1.0.2/src/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 The possible commands (or their aliases) are the following:
 
    generate  (-g)
    upload    (-u)
    reset     (-r)
    help      (-h)
 
-See the documentation on GitHub (github.com/bdavis222/pypimaker) for more information.
+See the documentation on GitHub for more information:
+https://github.com/bdavis222/pypimaker
 """
 
 DEFAULT_INITIAL_VERSION = "0.1.0"
 
 PROJECT_DESCRIPTION_TEXT = 'One-sentence Project Description (e.g., "Software designed for..."):'
 SELECT_FOLDER_TEXT = "Select the top-level folder containing your Python project"
 PROJECT_NAME_DESCRIPTION_TEXT = '(Your package will be installed with the "pip install \
```

### Comparing `pypimaker-1.0.1/src/ui/AuthorInfoSelector.py` & `pypimaker-1.0.2/src/ui/AuthorInfoSelector.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/ui/DialogWindow.py` & `pypimaker-1.0.2/src/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/ui/OptionSelector.py` & `pypimaker-1.0.2/src/ui/OptionSelector.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/ui/navigation.py` & `pypimaker-1.0.2/src/ui/navigation.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/src/upload.py` & `pypimaker-1.0.2/src/upload.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/tests/test_files.py` & `pypimaker-1.0.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/tests/test_upload.py` & `pypimaker-1.0.2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.1/tests/ui/test_navigation.py` & `pypimaker-1.0.2/tests/ui/test_navigation.py`

 * *Files identical despite different names*

