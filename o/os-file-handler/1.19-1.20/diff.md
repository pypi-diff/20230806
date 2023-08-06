# Comparing `tmp/os_file_handler-1.19.tar.gz` & `tmp/os_file_handler-1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os_file_handler-1.19.tar", last modified: Mon Dec 12 14:14:51 2022, max compression
+gzip compressed data, was "os_file_handler-1.20.tar", last modified: Sun Aug  6 10:06:00 2023, max compression
```

## Comparing `os_file_handler-1.19.tar` & `os_file_handler-1.20.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-12-12 14:14:51.567360 os_file_handler-1.19/
--rw-r--r--   0 ozshabbat   (501) staff       (20)     1065 2019-06-20 10:31:16.000000 os_file_handler-1.19/LICENSE.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)      726 2022-12-12 14:14:51.567421 os_file_handler-1.19/PKG-INFO
--rw-r--r--   0 ozshabbat   (501) staff       (20)    11365 2021-02-07 13:59:03.000000 os_file_handler-1.19/README.md
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-12-12 14:14:51.566769 os_file_handler-1.19/os_file_handler/
--rw-r--r--   0 ozshabbat   (501) staff       (20)    13815 2022-12-12 14:14:45.000000 os_file_handler-1.19/os_file_handler/file_handler.py
-drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2022-12-12 14:14:51.567236 os_file_handler-1.19/os_file_handler.egg-info/
--rw-r--r--   0 ozshabbat   (501) staff       (20)      726 2022-12-12 14:14:51.000000 os_file_handler-1.19/os_file_handler.egg-info/PKG-INFO
--rw-r--r--   0 ozshabbat   (501) staff       (20)      228 2022-12-12 14:14:51.000000 os_file_handler-1.19/os_file_handler.egg-info/SOURCES.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)        1 2022-12-12 14:14:51.000000 os_file_handler-1.19/os_file_handler.egg-info/dependency_links.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)       16 2022-12-12 14:14:51.000000 os_file_handler-1.19/os_file_handler.egg-info/top_level.txt
--rw-r--r--   0 ozshabbat   (501) staff       (20)       38 2022-12-12 14:14:51.567607 os_file_handler-1.19/setup.cfg
--rw-r--r--   0 ozshabbat   (501) staff       (20)     1489 2022-12-12 14:14:49.000000 os_file_handler-1.19/setup.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-08-06 10:06:00.379206 os_file_handler-1.20/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1065 2019-06-20 10:31:16.000000 os_file_handler-1.20/LICENSE.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      698 2023-08-06 10:06:00.379264 os_file_handler-1.20/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)    11365 2021-02-07 13:59:03.000000 os_file_handler-1.20/README.md
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-08-06 10:06:00.378541 os_file_handler-1.20/os_file_handler/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)    14585 2023-08-06 10:05:26.000000 os_file_handler-1.20/os_file_handler/file_handler.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-08-06 10:06:00.379104 os_file_handler-1.20/os_file_handler.egg-info/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      698 2023-08-06 10:06:00.000000 os_file_handler-1.20/os_file_handler.egg-info/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      228 2023-08-06 10:06:00.000000 os_file_handler-1.20/os_file_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)        1 2023-08-06 10:06:00.000000 os_file_handler-1.20/os_file_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       16 2023-08-06 10:06:00.000000 os_file_handler-1.20/os_file_handler.egg-info/top_level.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       38 2023-08-06 10:06:00.379451 os_file_handler-1.20/setup.cfg
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1489 2023-08-06 10:05:52.000000 os_file_handler-1.20/setup.py
```

### Comparing `os_file_handler-1.19/LICENSE.txt` & `os_file_handler-1.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `os_file_handler-1.19/PKG-INFO` & `os_file_handler-1.20/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: os_file_handler
-Version: 1.19
+Version: 1.20
 Summary: py file handling tools for os
 Home-page: https://github.com/osfunapps/os-file-handler-py
 Author: Oz Shabat
 Author-email: support@os-apps.com
 License: MIT
 Keywords: python,osfunapps,files,tools,utils
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `os_file_handler-1.19/README.md` & `os_file_handler-1.20/README.md`

 * *Files identical despite different names*

### Comparing `os_file_handler-1.19/os_file_handler/file_handler.py` & `os_file_handler-1.20/os_file_handler/file_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # this module meant to provide file handling functions
 #
 ###########################################################################
 
 import os
 import shutil
+import stat
 
 # will return the content of a directory (full paths)
 def get_dir_content(dir_path, recursive=False, collect_dirs=True, collect_files=True, ignored_files_arr=['.DS_Store'], sort_by_name=True):
     f_list = []
     d_list = []
     for path, dirs, files in os.walk(dir_path):
         if collect_dirs:
@@ -92,16 +93,28 @@
         filename = filename[:last_dot_idx]
     return filename
 
 
 # will remove a directory
 def remove_dir(path):
     if os.path.isdir(path):
-        shutil.rmtree(path)
+        # Make the directory writeable (and readable and executable, as necessary)
+        os.chmod(path, stat.S_IWRITE | stat.S_IREAD | stat.S_IEXEC)
+
+        # Now remove the contents
+        for root, dirs, files in os.walk(path, topdown=False):
+            # Make all files writeable
+            for name in files:
+                os.chmod(os.path.join(root, name), stat.S_IWRITE | stat.S_IREAD | stat.S_IEXEC)
+            # Make all subdirectories writeable
+            for name in dirs:
+                os.chmod(os.path.join(root, name), stat.S_IWRITE | stat.S_IREAD | stat.S_IEXEC)
 
+        # Now you can remove the directory
+        shutil.rmtree(path)
 
 # will remove a bunch of files in a list
 def remove_files(file_list):
     for file in file_list:
         remove_file(file)
 
 
@@ -321,18 +334,22 @@
     if ext[0] == '.':
         ext = ext[1:]
     for f in glob.glob(path + "/*." + ext):
         remove_file(f)
 
 
 # will remove a single file
-def remove_file(file):
-    if is_file_exists(file):
-        os.remove(file)
+def remove_file(path):
+
+    if os.path.isfile(path):
+        # Make the file writeable
+        os.chmod(path, stat.S_IWRITE | stat.S_IREAD)
 
+        # Now you can remove the file
+        os.remove(path)
 
 # will check if line exists in a file
 def is_line_exists_in_file(file, line_to_find):
     with open(file) as f:
         content = f.readlines()
         for line in content:
             if line_to_find in line:
```

### Comparing `os_file_handler-1.19/os_file_handler.egg-info/PKG-INFO` & `os_file_handler-1.20/os_file_handler.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: os-file-handler
-Version: 1.19
+Version: 1.20
 Summary: py file handling tools for os
 Home-page: https://github.com/osfunapps/os-file-handler-py
 Author: Oz Shabat
 Author-email: support@os-apps.com
 License: MIT
 Keywords: python,osfunapps,files,tools,utils
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `os_file_handler-1.19/setup.py` & `os_file_handler-1.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='os_file_handler',  # How you named your package folder (MyLib)
     packages=['os_file_handler'],  # Choose the same as "name"
-    version='1.19',  # Start with a small number and increase it with every change you make
+    version='1.20',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='py file handling tools for os',  # Give a short description about your library
     author='Oz Shabat',  # Type in your name
     author_email='support@os-apps.com',  # Type in your E-Mail
     url='https://github.com/osfunapps/os-file-handler-py',  # Provide either the link to your github or to your website
     keywords=['python', 'osfunapps', 'files', 'tools', 'utils'],  # Keywords that define your package best
     install_requires=[],
```

