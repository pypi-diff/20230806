# Comparing `tmp/win-basic-tools-0.4.0.tar.gz` & `tmp/win-basic-tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win-basic-tools-0.4.0.tar", last modified: Sun Aug  6 09:13:51 2023, max compression
+gzip compressed data, was "win-basic-tools-0.4.1.tar", last modified: Sun Aug  6 15:47:37 2023, max compression
```

## Comparing `win-basic-tools-0.4.0.tar` & `win-basic-tools-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/
--rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1785 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.4.0/README.md
--rw-rw-rw-   0        0        0     1075 2023-07-18 06:25:40.000000 win-basic-tools-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 09:13:50.996150 win-basic-tools-0.4.0/win_basic_tools/
--rw-rw-rw-   0        0        0     9936 2023-07-18 06:09:09.000000 win-basic-tools-0.4.0/win_basic_tools/__init__.py
--rw-rw-rw-   0        0        0      305 2023-07-18 03:23:45.000000 win-basic-tools-0.4.0/win_basic_tools/__main__.py
--rw-rw-rw-   0        0        0     2137 2023-08-06 09:12:17.000000 win-basic-tools-0.4.0/win_basic_tools/setup_cmd.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:13:50.996150 win-basic-tools-0.4.0/win_basic_tools.egg-info/
--rw-rw-rw-   0        0        0     1785 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:47:37.822200 win-basic-tools-0.4.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1785 2023-08-06 15:47:37.820147 win-basic-tools-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1117 2023-08-06 15:46:45.000000 win-basic-tools-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:47:37.822760 win-basic-tools-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:47:37.799819 win-basic-tools-0.4.1/win_basic_tools/
+-rw-rw-rw-   0        0        0     9990 2023-08-06 10:51:34.000000 win-basic-tools-0.4.1/win_basic_tools/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-07-18 03:23:45.000000 win-basic-tools-0.4.1/win_basic_tools/__main__.py
+-rw-rw-rw-   0        0        0     2137 2023-08-06 09:12:17.000000 win-basic-tools-0.4.1/win_basic_tools/setup_cmd.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:47:37.816360 win-basic-tools-0.4.1/win_basic_tools.egg-info/
+-rw-rw-rw-   0        0        0     1785 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-06 15:47:37.000000 win-basic-tools-0.4.1/win_basic_tools.egg-info/top_level.txt
```

### Comparing `win-basic-tools-0.4.0/LICENSE` & `win-basic-tools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.4.0/PKG-INFO` & `win-basic-tools-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Cli tool for listing the directory.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 License: MIT
 Project-URL: Home-page, https://github.com/HenriquedoVal/win-basic-tools
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `win-basic-tools-0.4.0/README.md` & `win-basic-tools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.4.0/pyproject.toml` & `win-basic-tools-0.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'win-basic-tools'
-version = '0.4.0'
+version = '0.4.1'
 authors = [
   {name = 'Henrique do Val'},
   {email = 'henrique.val@hotmail.com'}
 ]
 
 description = 'Cli tool for listing the directory.'
 readme = {file = "README.md", content-type = 'text/markdown'}
 requires-python = '>=3.6'
 license = {text = 'MIT'}
+dependencies = [
+  'colorama>=0.4.6'
+]
 
 classifiers = [
   'Programming Language :: Python :: 3 :: Only',
   'Programming Language :: Python :: Implementation :: CPython',
   'Programming Language :: Python :: Implementation :: PyPy',
   'License :: OSI Approved :: MIT License',
   'Development Status :: 4 - Beta',
@@ -31,8 +34,8 @@
 [project.urls]
 Home-page = "https://github.com/HenriquedoVal/win-basic-tools"
 
 [project.scripts]
 win-basic-tools = 'win_basic_tools.setup_cmd:main'
 
 [tool.setuptools.packages.find]
-include = ["win-basic-tools"]
+include = ["win_basic_tools"]
```

### Comparing `win-basic-tools-0.4.0/win_basic_tools/__init__.py` & `win-basic-tools-0.4.1/win_basic_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,18 @@
             + total_size
             + pad
             + f'{self.files} {f}, {self.dirs} {d}',
             end='', file=self.out
         )
 
     def _print_headers(self, pad):
-        res = Fore.GREEN + ' ' * 3 + 'Mode ' + pad
+        res = ' ' * 3 + 'Mode ' + pad
+
+        if self.opt.colors:
+            res = Fore.GREEN + res
 
         for _opt in ('ctime', 'mtime', 'atime'):
             if getattr(self.opt, _opt):
                 res += _opt.capitalize().center(
                     10 + 9 * int(self.opt.hour)) + pad
 
         res += '   Size' + pad + 'Name' + Style.RESET_ALL
```

### Comparing `win-basic-tools-0.4.0/win_basic_tools/setup_cmd.py` & `win-basic-tools-0.4.1/win_basic_tools/setup_cmd.py`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.4.0/win_basic_tools.egg-info/PKG-INFO` & `win-basic-tools-0.4.1/win_basic_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Cli tool for listing the directory.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 License: MIT
 Project-URL: Home-page, https://github.com/HenriquedoVal/win-basic-tools
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

