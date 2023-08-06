# Comparing `tmp/pypimaker-0.1.9.tar.gz` & `tmp/pypimaker-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypimaker-0.1.9.tar", last modified: Sat Jan  7 16:54:09 2023, max compression
+gzip compressed data, was "dist/pypimaker-1.0.0.tar", last modified: Sun Aug  6 01:59:20 2023, max compression
```

## Comparing `pypimaker-0.1.9.tar` & `pypimaker-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.489925 pypimaker-0.1.9/
--rw-r--r--   0 holly      (501) staff       (20)     1067 2023-01-06 23:58:32.000000 pypimaker-0.1.9/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)     4358 2023-01-07 16:54:09.489651 pypimaker-0.1.9/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     3593 2023-01-07 16:50:53.000000 pypimaker-0.1.9/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.486851 pypimaker-0.1.9/pypimaker.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)     4358 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      442 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       48 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       10 2023-01-07 16:54:09.000000 pypimaker-0.1.9/pypimaker.egg-info/top_level.txt
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-01-07 16:54:09.490007 pypimaker-0.1.9/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1192 2023-01-07 16:54:09.000000 pypimaker-0.1.9/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.487546 pypimaker-0.1.9/src/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1735 2023-01-07 04:47:12.000000 pypimaker-0.1.9/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)    12876 2023-01-07 16:50:51.000000 pypimaker-0.1.9/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)      889 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/reset.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.488470 pypimaker-0.1.9/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     6796 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/AuthorInfoSelector.py
--rw-r--r--   0 holly      (501) staff       (20)     3257 2023-01-07 04:13:54.000000 pypimaker-0.1.9/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     6588 2023-01-07 16:50:57.000000 pypimaker-0.1.9/src/ui/OptionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)      563 2023-01-06 23:58:32.000000 pypimaker-0.1.9/src/ui/navigation.py
--rw-r--r--   0 holly      (501) staff       (20)     7116 2023-01-07 05:53:05.000000 pypimaker-0.1.9/src/upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-01-07 16:54:09.489210 pypimaker-0.1.9/tests/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-01-06 23:58:32.000000 pypimaker-0.1.9/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2612 2023-01-07 05:44:13.000000 pypimaker-0.1.9/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     1420 2023-01-07 05:53:07.000000 pypimaker-0.1.9/tests/test_upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.707092 pypimaker-1.0.0/
+-rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 01:55:23.000000 pypimaker-1.0.0/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)     4331 2023-08-06 01:59:20.706874 pypimaker-1.0.0/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     3567 2023-08-06 01:58:09.000000 pypimaker-1.0.0/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.702223 pypimaker-1.0.0/pypimaker.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)     4331 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/top_level.txt
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:59:20.707170 pypimaker-1.0.0/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1347 2023-08-06 01:59:20.000000 pypimaker-1.0.0/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.703405 pypimaker-1.0.0/src/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.0/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.0/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)      923 2023-08-06 01:54:56.000000 pypimaker-1.0.0/src/reset.py
+-rw-r--r--   0 holly      (501) staff       (20)     7289 2023-08-06 01:54:58.000000 pypimaker-1.0.0/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.704773 pypimaker-1.0.0/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     7744 2023-08-06 01:54:40.000000 pypimaker-1.0.0/src/ui/AuthorInfoSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)     3887 2023-08-06 01:53:50.000000 pypimaker-1.0.0/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     8188 2023-08-06 01:54:48.000000 pypimaker-1.0.0/src/ui/OptionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.0/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.0/src/ui/navigation.py
+-rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 01:54:59.000000 pypimaker-1.0.0/src/upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.705480 pypimaker-1.0.0/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.0/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.0/tests/test_upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.706240 pypimaker-1.0.0/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.0/tests/ui/test_navigation.py
```

### Comparing `pypimaker-0.1.9/LICENSE` & `pypimaker-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 Copyright (c) 2022 Brian Davis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pypimaker-0.1.9/PKG-INFO` & `pypimaker-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 0.1.9
+Version: 1.0.0
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPI Maker
+
 > Software designed for simplifying PyPI Python package setups
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
 ## Getting Started
 
 ### Dependencies
@@ -32,25 +33,26 @@
 
 To install pypimaker, open a terminal window and run the following command:
 
 ```
 pip install pypimaker
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ## Generating Your PyPI Files
 
 To generate the files needed for your PyPI package, run the following command:
 
 ```
 pypimaker generate
 ```
 
 This will launch a graphical user interface that looks like the following:
+
 ![](https://github.com/bdavis222/pypimaker/blob/main/images/0.png)
 
 Inputting the information for your project will generate all of the files needed for uploading it to PyPI (`LICENSE`, `README.me`, `requirements.txt`, and `setup.py`). This can be re-run at any time to re-generate these files.
 
 ## Uploading Your Finished Project to PyPI
 
 If you don't yet have an account on PyPI, [register for one](https://pypi.org/account/register/). Once you've set up your account and you're ready to upload your package to PyPI (e.g., after you have updated the generated template `README.md` file to your liking), run the following command:
@@ -61,40 +63,38 @@
 
 You will be asked to enter your PyPI username and password (which you've registered previously) in the terminal. Your project will then be uploaded to PyPI, and others can download it using the following command:
 
 ```
 pip install <PROJECT_NAME>
 ```
 
-*(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)*
+_(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)_
 
 ## Resetting Your Project
 
 At any time, all of the files generated by PyPI Maker can be removed with the following command:
 
 ```
 pypimaker reset
 ```
 
 ## Making changes to your PyPI project
 
 To make changes and update your project, simply re-run `pypimaker upload`. Follow the steps in the terminal to incremement your version number and your update will be pushed to PyPI.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project._
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.9
-	 * Bug fixes
-* 0.1.0
-	 * Initial Release
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
 
 ## Development
 
@@ -106,8 +106,8 @@
 python -m unittest
 ```
 
 The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
-To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
+To report a bug, visit the [issues page](https://github.com/bdavis222/pypimaker/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.9/README.md` & `pypimaker-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # PyPI Maker
+
 > Software designed for simplifying PyPI Python package setups
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
 ## Getting Started
 
 ### Dependencies
@@ -13,25 +14,26 @@
 
 To install pypimaker, open a terminal window and run the following command:
 
 ```
 pip install pypimaker
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ## Generating Your PyPI Files
 
 To generate the files needed for your PyPI package, run the following command:
 
 ```
 pypimaker generate
 ```
 
 This will launch a graphical user interface that looks like the following:
+
 ![](https://github.com/bdavis222/pypimaker/blob/main/images/0.png)
 
 Inputting the information for your project will generate all of the files needed for uploading it to PyPI (`LICENSE`, `README.me`, `requirements.txt`, and `setup.py`). This can be re-run at any time to re-generate these files.
 
 ## Uploading Your Finished Project to PyPI
 
 If you don't yet have an account on PyPI, [register for one](https://pypi.org/account/register/). Once you've set up your account and you're ready to upload your package to PyPI (e.g., after you have updated the generated template `README.md` file to your liking), run the following command:
@@ -42,40 +44,38 @@
 
 You will be asked to enter your PyPI username and password (which you've registered previously) in the terminal. Your project will then be uploaded to PyPI, and others can download it using the following command:
 
 ```
 pip install <PROJECT_NAME>
 ```
 
-*(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)*
+_(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)_
 
 ## Resetting Your Project
 
 At any time, all of the files generated by PyPI Maker can be removed with the following command:
 
 ```
 pypimaker reset
 ```
 
 ## Making changes to your PyPI project
 
 To make changes and update your project, simply re-run `pypimaker upload`. Follow the steps in the terminal to incremement your version number and your update will be pushed to PyPI.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project._
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.9
-	 * Bug fixes
-* 0.1.0
-	 * Initial Release
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
 
 ## Development
 
@@ -87,8 +87,8 @@
 python -m unittest
 ```
 
 The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
-To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
+To report a bug, visit the [issues page](https://github.com/bdavis222/pypimaker/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.9/pypimaker.egg-info/PKG-INFO` & `pypimaker-1.0.0/pypimaker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 0.1.9
+Version: 1.0.0
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPI Maker
+
 > Software designed for simplifying PyPI Python package setups
 
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?business=UA5NL9MJSFMVY)
 
 ## Getting Started
 
 ### Dependencies
@@ -32,25 +33,26 @@
 
 To install pypimaker, open a terminal window and run the following command:
 
 ```
 pip install pypimaker
 ```
 
-*(Note that the* `pip3` *command may be required instead of* `pip` *for some Python installations.)*
+_(Note that the_ `pip3` _command may be required instead of_ `pip` _for some Python installations.)_
 
 ## Generating Your PyPI Files
 
 To generate the files needed for your PyPI package, run the following command:
 
 ```
 pypimaker generate
 ```
 
 This will launch a graphical user interface that looks like the following:
+
 ![](https://github.com/bdavis222/pypimaker/blob/main/images/0.png)
 
 Inputting the information for your project will generate all of the files needed for uploading it to PyPI (`LICENSE`, `README.me`, `requirements.txt`, and `setup.py`). This can be re-run at any time to re-generate these files.
 
 ## Uploading Your Finished Project to PyPI
 
 If you don't yet have an account on PyPI, [register for one](https://pypi.org/account/register/). Once you've set up your account and you're ready to upload your package to PyPI (e.g., after you have updated the generated template `README.md` file to your liking), run the following command:
@@ -61,40 +63,38 @@
 
 You will be asked to enter your PyPI username and password (which you've registered previously) in the terminal. Your project will then be uploaded to PyPI, and others can download it using the following command:
 
 ```
 pip install <PROJECT_NAME>
 ```
 
-*(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)*
+_(Here, <PROJECT_NAME> is the name you selected when running `pypimaker generate`)_
 
 ## Resetting Your Project
 
 At any time, all of the files generated by PyPI Maker can be removed with the following command:
 
 ```
 pypimaker reset
 ```
 
 ## Making changes to your PyPI project
 
 To make changes and update your project, simply re-run `pypimaker upload`. Follow the steps in the terminal to incremement your version number and your update will be pushed to PyPI.
 
-*Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project.*
+_Note: the extraneous `+[CATransaction synchronize]` output in the terminal window is a known bug in macOS 13 that will not affect your project._
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-* 0.1.9
-	 * Bug fixes
-* 0.1.0
-	 * Initial Release
+- 1.0.0
+  - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
 
 ## Development
 
@@ -106,8 +106,8 @@
 python -m unittest
 ```
 
 The same test framework can optionally be added to your own project: If there is not yet a folder named `tests` in the top level of your project's directory structure, then a dialog window will pop up asking if you would like to include template unit tests in your project when running `pypimaker generate`. Confirming this selection will create a `tests` folder with individual unit tests inside, corresponding to each of the Python files in your project. Of course, until writing test cases within each of these test files, they won't actually test anything.
 
 ### Bug Reports and Feature Requests
 
-To report a bug, visit the [issues page](https://github.com/bdavis222/project_template/issues). New feature requests are also welcome!
+To report a bug, visit the [issues page](https://github.com/bdavis222/pypimaker/issues). New feature requests are also welcome!
```

### Comparing `pypimaker-0.1.9/setup.py` & `pypimaker-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
-	name='pypimaker', # Required
-    version='0.1.9', # Required 
+    name='pypimaker',  # Required
+    version='1.0.0', # Required 
     description='Software designed for simplifying PyPI Python package setups',
-	long_description=long_description,
-	long_description_content_type='text/markdown',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/pypimaker',
     author='Brian Davis',
-	classifiers=[ # Defined at https://pypi.org/classifiers/
-		'Intended Audience :: Developers',
-		'License :: OSI Approved :: MIT License',
-		'Programming Language :: Python :: 3',
-		'Operating System :: Unix',
-		'Operating System :: MacOS :: MacOS X',
-		'Operating System :: Microsoft :: Windows'
-	],
-	packages=find_packages(), # Required
-	py_modules=['tests', 'src.ui', 'src'], # Generated
-	python_requires='>=3.7, <4', 
-	project_urls={
-		'Bug Reports': 'https://github.com/bdavis222/pypimaker/issues',
-		'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
-		'Source': 'https://github.com/bdavis222/',
-	},
-	entry_points={
-		'console_scripts': [
-			'pypimaker = src.__main__:main'
-		]
-	}
-)
+        classifiers=[  # Defined at https://pypi.org/classifiers/
+            'Intended Audience :: Developers',
+            'License :: OSI Approved :: MIT License',
+            'Programming Language :: Python :: 3',
+            'Operating System :: Unix',
+            'Operating System :: MacOS :: MacOS X',
+            'Operating System :: Microsoft :: Windows'
+        ],
+    packages=find_packages(),  # Required
+    py_modules=['src', 'src.ui', 'tests'],  # Generated
+    python_requires='>=3.7, <4',
+    project_urls={
+        'Bug Reports': 'https://github.com/bdavis222/pypimaker/issues',
+        'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
+        'Source': 'https://github.com/bdavis222/',
+            },
+    entry_points={
+        'console_scripts': [
+            'pypimaker = src.__main__:main'
+        ]
+    }
+)
```

### Comparing `pypimaker-0.1.9/src/__main__.py` & `pypimaker-1.0.0/src/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,53 @@
 import argparse
 import sys
+
+from src import strings
 import src.files as files
 import src.reset as reset
 import src.upload as upload
 from src.ui import navigation
 from src.ui.OptionSelector import OptionSelector
 
-INVALID_ARGUMENT_TEXT = "Invalid argument given. Must be 'generate', 'upload', 'reset', \
-'fiximports', 'unfiximports', or 'help'."
 
-ARGS_DESCRIPTION_TEXT = "Enter command 'generate', 'upload', 'reset', 'fiximports', \
-'unfiximports', or 'help'"
+def main(argv=sys.argv):
+    parser = argparse.ArgumentParser(
+        description="Example input: pypimaker generate")
+    parser.add_argument(
+        "command",
+        type=str,
+        help=strings.ARGS_DESCRIPTION_TEXT,
+        nargs=1
+    )
+    userOption = "help" if len(sys.argv) == 1 else sys.argv[1]
+
+    if userOption in ["generate", "-g"]:
+        options = OptionSelector()
+        files.generate(
+            options.filepath,
+            options.projectName,
+            options.authorsArray,
+            options.emailsArray,
+            options.correspondingEmail,
+            options.githubUsername,
+            options.shortDescription,
+            options.classifier,
+            options.mainFunctionPath
+        )
 
-HELP_TEXT = "\nPyPI Maker\n----------\n\n\
-To run PyPI Maker, enter 'pypimaker' followed by a valid command.\n\
-Some examples:\n\n\
-   pypimaker generate\n\
-   pypimaker upload\n\
-   pypimaker -r\
-\n\nThe possible commands (or their aliases) are the following:\n\n\
-   generate  (-g)\n\
-   upload    (-u)\n\
-   reset     (-r)\n\
-   help      (-h)\n\n\
-See the documentation on GitHub or PyPI for more information.\n"
+    elif userOption in ["upload", "-u"]:
+        filepath = navigation.getDirectory()
+        upload.upload(filepath)
+
+    elif userOption in ["reset", "-r"]:
+        filepath = navigation.getDirectory()
+        reset.reset(filepath)
+
+    elif userOption in ["help", "-h"]:
+        print(strings.HELP_TEXT)
+
+    else:
+        print(strings.HELP_TEXT)
 
-def main(argv=sys.argv):
-	parser = argparse.ArgumentParser(description="Example input: pypimaker generate")
-	parser.add_argument(
-		"command", 
-		type=str, 
-		help=ARGS_DESCRIPTION_TEXT, 
-		nargs=1
-	)
-	userOption = "help" if len(sys.argv) == 1 else sys.argv[1]
-	
-	if userOption in ["generate", "-g"]:
-		options = OptionSelector()
-		files.generate(
-			options.filepath,
-			options.projectName,
-			options.authorsArray,
-			options.emailsArray,
-			options.correspondingEmail,
-			options.githubUsername,
-			options.shortDescription,
-			options.classifier
-		)
-	
-	elif userOption in ["upload", "-u"]:
-		filepath = navigation.getDirectory()
-		upload.upload(filepath)
-	
-	elif userOption in ["reset", "-r"]:
-		filepath = navigation.getDirectory()
-		reset.reset(filepath)
-	
-	elif userOption in ["help", "-h"]:
-		print(HELP_TEXT)
-	
-	else:
-		print(HELP_TEXT)
 
 if __name__ == '__main__':
-	main()
+    main()
```

### Comparing `pypimaker-0.1.9/src/reset.py` & `pypimaker-1.0.0/src/reset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import os
 import subprocess
+
 from src.ui.DialogWindow import ActionDialogWindow
 
 RESET_SELECTION_TEXT = "This will remove generated files.\nAre you sure you want to reset?"
 
+
 def reset(topLevelDirectory):
-    ActionDialogWindow("Are you sure?", RESET_SELECTION_TEXT, negativeAction=exit, mainWindow=True)
-    
-    filesToRemove = ["LICENSE", "README.md", "requirements.txt", "setup.py", ".gitignore"]
+    ActionDialogWindow("Are you sure?", RESET_SELECTION_TEXT,
+                       negativeAction=exit, mainWindow=True)
+
+    filesToRemove = ["LICENSE", "README.md",
+                     "requirements.txt", "setup.py", ".gitignore"]
     foldersToRemove = ["build", "dist"]
     for item in os.listdir(topLevelDirectory):
         if item.endswith("egg-info"):
             foldersToRemove.append(item)
-    
+
     for file in filesToRemove:
         commandArray = ["rm", topLevelDirectory + "/" + file]
         subprocess.run(commandArray, capture_output=True)
-    
+
     for folder in foldersToRemove:
         commandArray = ["rm", "-r", topLevelDirectory + "/" + folder]
         subprocess.run(commandArray, capture_output=True)
```

### Comparing `pypimaker-0.1.9/src/ui/AuthorInfoSelector.py` & `pypimaker-1.0.0/src/ui/AuthorInfoSelector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,182 @@
-import os
 import tkinter as tk
+
 from src.ui.DialogWindow import ActionDialogWindow, InfoDialogWindow
 
 MISSING_AUTHOR_NAMES_TEXT = "Some emails have missing author names.\nPlease fix and resubmit."
 MISSING_FIRST_NAME_TEXT = "Corresponding author name not given.\nSubmit with no authors?"
 MISSING_FIRST_AUTHOR_EMAIL_TEXT = "Email given for other(s), but not first author.\n\
 Use next email in list for correspondence?"
 
+
 class AuthorInfoSelector:
-	def __init__(self):
-		self.window = tk.Tk()
-		self.window.title("PyPI Maker")
-		centerX = (self.window.winfo_screenwidth() - 650) // 2
-		centerY = (self.window.winfo_screenheight() - 310) // 2
-		self.window.geometry(f"650x310+{centerX}+{centerY}")
-		
-		self.names = []
-		self.emails = []
-		self.correspondingEmail = ""
-		
-		labelPrimary = tk.Label(self.window, text="Corresponding Author")
-		
-		authorFrame1 = tk.Frame(self.window)
-		labelName1 = tk.Label(self.window, text="Name:")
-		self.entryName1 = tk.Entry(self.window, width=25)
-		labelEmail1 = tk.Label(self.window, text="Email:")
-		self.entryEmail1 = tk.Entry(self.window, width=25)
-		labelName1.pack(in_=authorFrame1, side=tk.LEFT)
-		self.entryName1.pack(in_=authorFrame1, side=tk.LEFT)
-		labelEmail1.pack(in_=authorFrame1, side=tk.LEFT)
-		self.entryEmail1.pack(in_=authorFrame1, side=tk.LEFT)
-		
-		labelOthers = tk.Label(self.window, text="Other Authors")
-		
-		authorFrame2 = tk.Frame(self.window)
-		labelName2 = tk.Label(self.window, text="Name:")
-		self.entryName2 = tk.Entry(self.window, width=25)
-		labelEmail2 = tk.Label(self.window, text="Email:")
-		self.entryEmail2 = tk.Entry(self.window, width=25)
-		labelName2.pack(in_=authorFrame2, side=tk.LEFT)
-		self.entryName2.pack(in_=authorFrame2, side=tk.LEFT)
-		labelEmail2.pack(in_=authorFrame2, side=tk.LEFT)
-		self.entryEmail2.pack(in_=authorFrame2, side=tk.LEFT)
-		
-		authorFrame3 = tk.Frame(self.window)
-		labelName3 = tk.Label(self.window, text="Name:")
-		self.entryName3 = tk.Entry(self.window, width=25)
-		labelEmail3 = tk.Label(self.window, text="Email:")
-		self.entryEmail3 = tk.Entry(self.window, width=25)
-		labelName3.pack(in_=authorFrame3, side=tk.LEFT)
-		self.entryName3.pack(in_=authorFrame3, side=tk.LEFT)
-		labelEmail3.pack(in_=authorFrame3, side=tk.LEFT)
-		self.entryEmail3.pack(in_=authorFrame3, side=tk.LEFT)
-		
-		authorFrame4 = tk.Frame(self.window)
-		labelName4 = tk.Label(self.window, text="Name:")
-		self.entryName4 = tk.Entry(self.window, width=25)
-		labelEmail4 = tk.Label(self.window, text="Email:")
-		self.entryEmail4 = tk.Entry(self.window, width=25)
-		labelName4.pack(in_=authorFrame4, side=tk.LEFT)
-		self.entryName4.pack(in_=authorFrame4, side=tk.LEFT)
-		labelEmail4.pack(in_=authorFrame4, side=tk.LEFT)
-		self.entryEmail4.pack(in_=authorFrame4, side=tk.LEFT)
-		
-		authorFrame5 = tk.Frame(self.window)
-		labelName5 = tk.Label(self.window, text="Name:")
-		self.entryName5 = tk.Entry(self.window, width=25)
-		labelEmail5 = tk.Label(self.window, text="Email:")
-		self.entryEmail5 = tk.Entry(self.window, width=25)
-		labelName5.pack(in_=authorFrame5, side=tk.LEFT)
-		self.entryName5.pack(in_=authorFrame5, side=tk.LEFT)
-		labelEmail5.pack(in_=authorFrame5, side=tk.LEFT)
-		self.entryEmail5.pack(in_=authorFrame5, side=tk.LEFT)
-		
-		authorFrame6 = tk.Frame(self.window)
-		labelName6 = tk.Label(self.window, text="Name:")
-		self.entryName6 = tk.Entry(self.window, width=25)
-		labelEmail6 = tk.Label(self.window, text="Email:")
-		self.entryEmail6 = tk.Entry(self.window, width=25)
-		labelName6.pack(in_=authorFrame6, side=tk.LEFT)
-		self.entryName6.pack(in_=authorFrame6, side=tk.LEFT)
-		labelEmail6.pack(in_=authorFrame6, side=tk.LEFT)
-		self.entryEmail6.pack(in_=authorFrame6, side=tk.LEFT)
-		
-		authorFrame7 = tk.Frame(self.window)
-		labelName7 = tk.Label(self.window, text="Name:")
-		self.entryName7 = tk.Entry(self.window, width=25)
-		labelEmail7 = tk.Label(self.window, text="Email:")
-		self.entryEmail7 = tk.Entry(self.window, width=25)
-		labelName7.pack(in_=authorFrame7, side=tk.LEFT)
-		self.entryName7.pack(in_=authorFrame7, side=tk.LEFT)
-		labelEmail7.pack(in_=authorFrame7, side=tk.LEFT)
-		self.entryEmail7.pack(in_=authorFrame7, side=tk.LEFT)
-		
-		authorFrame8 = tk.Frame(self.window)
-		labelName8 = tk.Label(self.window, text="Name:")
-		self.entryName8 = tk.Entry(self.window, width=25)
-		labelEmail8 = tk.Label(self.window, text="Email:")
-		self.entryEmail8 = tk.Entry(self.window, width=25)
-		labelName8.pack(in_=authorFrame8, side=tk.LEFT)
-		self.entryName8.pack(in_=authorFrame8, side=tk.LEFT)
-		labelEmail8.pack(in_=authorFrame8, side=tk.LEFT)
-		self.entryEmail8.pack(in_=authorFrame8, side=tk.LEFT)
-		
-		self.buttonDone = tk.Button(self.window, text="Done", command=self.checkDone, fg="blue")
-		
-		labelPrimary.pack()
-		authorFrame1.pack()
-		labelOthers.pack()
-		authorFrame2.pack()
-		authorFrame3.pack()
-		authorFrame4.pack()
-		authorFrame5.pack()
-		authorFrame6.pack()
-		authorFrame7.pack()
-		authorFrame8.pack()
-		self.buttonDone.pack()
-		
-		self.window.protocol("WM_DELETE_WINDOW", quit)
-		self.window.bind("<Return>", self.checkDoneWithReturnKey)
-		
-		self.window.mainloop()
-	
-	def checkDone(self):
-		names = [self.entryName1.get(), self.entryName2.get(), self.entryName3.get(), 
-			self.entryName4.get(), self.entryName5.get(), self.entryName6.get(), 
-			self.entryName7.get(), self.entryName8.get()]
-		emails = [self.entryEmail1.get(), self.entryEmail2.get(), self.entryEmail3.get(), 
-			self.entryEmail4.get(), self.entryEmail5.get(), self.entryEmail6.get(), 
-			self.entryEmail7.get(), self.entryEmail8.get()]
-		
-		noEmailsEntered = True
-		for name, email in zip(names, emails):
-			if email != "":
-				noEmailsEntered = False
-				if name == "":
-					InfoDialogWindow("Invalid entry", MISSING_AUTHOR_NAMES_TEXT)
-					return
-		
-		if names[0] == "":
-			ActionDialogWindow("Invalid entry", MISSING_FIRST_NAME_TEXT, 
-				positiveAction=self.doneWithNoAuthors)
-			return
-		
-		if emails[0] == "" and not noEmailsEntered:
-			ActionDialogWindow("Invalid entry", MISSING_FIRST_AUTHOR_EMAIL_TEXT)
-		
-		self.done(names, emails)
-	
-	def checkDoneWithReturnKey(self, event):        
-		self.checkDone()
-	
-	def done(self, names, emails):
-		self.names, self.emails = self.getFilteredNamesAndEmails(names, emails)
-		self.correspondingEmail = self.getCorrespondingEmail()
-		self.window.destroy()
-		self.window.quit()
-	
-	def doneWithNoAuthors(self):
-		self.names = []
-		self.emails = []
-		self.window.destroy()
-		self.window.quit()
-	
-	def getCorrespondingEmail(self):
-		for email in self.emails:
-			if email != "":
-				return email
-	
-	def getFilteredNamesAndEmails(self, names, emails):
-		filteredNames = []
-		filteredEmails = []
-		for index, name in enumerate(names):
-			if name != "":
-				filteredNames.append(names[index])
-				filteredEmails.append(emails[index])
-		return filteredNames, filteredEmails
+    def __init__(self):
+        self.window = tk.Tk()
+        self.window.title("PyPI Maker")
+        centerX = (self.window.winfo_screenwidth() - 650) // 2
+        centerY = (self.window.winfo_screenheight() - 310) // 2
+        self.window.geometry(f"650x310+{centerX}+{centerY}")
+
+        self.names = []
+        self.emails = []
+        self.correspondingEmail = ""
+
+        labelPrimary = tk.Label(self.window, text="Corresponding Author")
+
+        authorFrame1 = tk.Frame(self.window)
+        labelName1 = tk.Label(self.window, text="Name:")
+        self.entryName1 = tk.Entry(self.window, width=25)
+        labelEmail1 = tk.Label(self.window, text="Email:")
+        self.entryEmail1 = tk.Entry(self.window, width=25)
+        labelName1.pack(in_=authorFrame1, side=tk.LEFT)
+        self.entryName1.pack(in_=authorFrame1, side=tk.LEFT)
+        labelEmail1.pack(in_=authorFrame1, side=tk.LEFT)
+        self.entryEmail1.pack(in_=authorFrame1, side=tk.LEFT)
+
+        labelOthers = tk.Label(self.window, text="Other Authors")
+
+        authorFrame2 = tk.Frame(self.window)
+        labelName2 = tk.Label(self.window, text="Name:")
+        self.entryName2 = tk.Entry(self.window, width=25)
+        labelEmail2 = tk.Label(self.window, text="Email:")
+        self.entryEmail2 = tk.Entry(self.window, width=25)
+        labelName2.pack(in_=authorFrame2, side=tk.LEFT)
+        self.entryName2.pack(in_=authorFrame2, side=tk.LEFT)
+        labelEmail2.pack(in_=authorFrame2, side=tk.LEFT)
+        self.entryEmail2.pack(in_=authorFrame2, side=tk.LEFT)
+
+        authorFrame3 = tk.Frame(self.window)
+        labelName3 = tk.Label(self.window, text="Name:")
+        self.entryName3 = tk.Entry(self.window, width=25)
+        labelEmail3 = tk.Label(self.window, text="Email:")
+        self.entryEmail3 = tk.Entry(self.window, width=25)
+        labelName3.pack(in_=authorFrame3, side=tk.LEFT)
+        self.entryName3.pack(in_=authorFrame3, side=tk.LEFT)
+        labelEmail3.pack(in_=authorFrame3, side=tk.LEFT)
+        self.entryEmail3.pack(in_=authorFrame3, side=tk.LEFT)
+
+        authorFrame4 = tk.Frame(self.window)
+        labelName4 = tk.Label(self.window, text="Name:")
+        self.entryName4 = tk.Entry(self.window, width=25)
+        labelEmail4 = tk.Label(self.window, text="Email:")
+        self.entryEmail4 = tk.Entry(self.window, width=25)
+        labelName4.pack(in_=authorFrame4, side=tk.LEFT)
+        self.entryName4.pack(in_=authorFrame4, side=tk.LEFT)
+        labelEmail4.pack(in_=authorFrame4, side=tk.LEFT)
+        self.entryEmail4.pack(in_=authorFrame4, side=tk.LEFT)
+
+        authorFrame5 = tk.Frame(self.window)
+        labelName5 = tk.Label(self.window, text="Name:")
+        self.entryName5 = tk.Entry(self.window, width=25)
+        labelEmail5 = tk.Label(self.window, text="Email:")
+        self.entryEmail5 = tk.Entry(self.window, width=25)
+        labelName5.pack(in_=authorFrame5, side=tk.LEFT)
+        self.entryName5.pack(in_=authorFrame5, side=tk.LEFT)
+        labelEmail5.pack(in_=authorFrame5, side=tk.LEFT)
+        self.entryEmail5.pack(in_=authorFrame5, side=tk.LEFT)
+
+        authorFrame6 = tk.Frame(self.window)
+        labelName6 = tk.Label(self.window, text="Name:")
+        self.entryName6 = tk.Entry(self.window, width=25)
+        labelEmail6 = tk.Label(self.window, text="Email:")
+        self.entryEmail6 = tk.Entry(self.window, width=25)
+        labelName6.pack(in_=authorFrame6, side=tk.LEFT)
+        self.entryName6.pack(in_=authorFrame6, side=tk.LEFT)
+        labelEmail6.pack(in_=authorFrame6, side=tk.LEFT)
+        self.entryEmail6.pack(in_=authorFrame6, side=tk.LEFT)
+
+        authorFrame7 = tk.Frame(self.window)
+        labelName7 = tk.Label(self.window, text="Name:")
+        self.entryName7 = tk.Entry(self.window, width=25)
+        labelEmail7 = tk.Label(self.window, text="Email:")
+        self.entryEmail7 = tk.Entry(self.window, width=25)
+        labelName7.pack(in_=authorFrame7, side=tk.LEFT)
+        self.entryName7.pack(in_=authorFrame7, side=tk.LEFT)
+        labelEmail7.pack(in_=authorFrame7, side=tk.LEFT)
+        self.entryEmail7.pack(in_=authorFrame7, side=tk.LEFT)
+
+        authorFrame8 = tk.Frame(self.window)
+        labelName8 = tk.Label(self.window, text="Name:")
+        self.entryName8 = tk.Entry(self.window, width=25)
+        labelEmail8 = tk.Label(self.window, text="Email:")
+        self.entryEmail8 = tk.Entry(self.window, width=25)
+        labelName8.pack(in_=authorFrame8, side=tk.LEFT)
+        self.entryName8.pack(in_=authorFrame8, side=tk.LEFT)
+        labelEmail8.pack(in_=authorFrame8, side=tk.LEFT)
+        self.entryEmail8.pack(in_=authorFrame8, side=tk.LEFT)
+
+        self.buttonDone = tk.Button(
+            self.window, text="Done", command=self.checkDone, fg="blue")
+
+        labelPrimary.pack()
+        authorFrame1.pack()
+        labelOthers.pack()
+        authorFrame2.pack()
+        authorFrame3.pack()
+        authorFrame4.pack()
+        authorFrame5.pack()
+        authorFrame6.pack()
+        authorFrame7.pack()
+        authorFrame8.pack()
+        self.buttonDone.pack()
+
+        self.window.protocol("WM_DELETE_WINDOW", quit)
+        self.window.bind("<Return>", self.checkDoneWithReturnKey)
+
+        self.window.mainloop()
+
+    def checkDone(self):
+        names = [self.entryName1.get(), self.entryName2.get(), self.entryName3.get(),
+                 self.entryName4.get(), self.entryName5.get(), self.entryName6.get(),
+                 self.entryName7.get(), self.entryName8.get()]
+        emails = [self.entryEmail1.get(), self.entryEmail2.get(), self.entryEmail3.get(),
+                  self.entryEmail4.get(), self.entryEmail5.get(), self.entryEmail6.get(),
+                  self.entryEmail7.get(), self.entryEmail8.get()]
+
+        noEmailsEntered = True
+        for name, email in zip(names, emails):
+            if email != "":
+                noEmailsEntered = False
+                if name == "":
+                    InfoDialogWindow(
+                        "Invalid entry", MISSING_AUTHOR_NAMES_TEXT)
+                    return
+
+        if names[0] == "":
+            ActionDialogWindow("Invalid entry", MISSING_FIRST_NAME_TEXT,
+                               positiveAction=self.doneWithNoAuthors)
+            return
+
+        if emails[0] == "" and not noEmailsEntered:
+            ActionDialogWindow(
+                "Invalid entry", MISSING_FIRST_AUTHOR_EMAIL_TEXT)
+
+        self.done(names, emails)
+
+    def checkDoneWithReturnKey(self, event):
+        self.checkDone()
+
+    def done(self, names, emails):
+        self.names, self.emails = self.getFilteredNamesAndEmails(names, emails)
+        self.correspondingEmail = self.getCorrespondingEmail()
+        self.window.destroy()
+        self.window.quit()
+
+    def doneWithNoAuthors(self):
+        self.names = []
+        self.emails = []
+        self.window.destroy()
+        self.window.quit()
+
+    def getCorrespondingEmail(self):
+        for email in self.emails:
+            if email != "":
+                return email
+
+    def getFilteredNamesAndEmails(self, names, emails):
+        filteredNames = []
+        filteredEmails = []
+        for index, name in enumerate(names):
+            if name != "":
+                filteredNames.append(names[index])
+                filteredEmails.append(emails[index])
+        return filteredNames, filteredEmails
```

### Comparing `pypimaker-0.1.9/src/ui/DialogWindow.py` & `pypimaker-1.0.0/src/ui/DialogWindow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,97 @@
 import tkinter as tk
 
+
 class DialogWindow:
-	def __init__(self, title, message, positiveButtonText, negativeButtonText, 
-		positiveButtonAction=None, negativeButtonAction=None, windowWidth=300, windowHeight=140, 
-		positiveButtonColor="blue", negativeButtonColor="black", 
-		mainWindow=False):		
-		self.window = tk.Tk()
-		self.window.title(title)
-		centerX = (self.window.winfo_screenwidth() - windowWidth) // 2
-		centerY = (self.window.winfo_screenheight() - windowHeight) // 2
-		self.window.geometry(f"{windowWidth}x{windowHeight}+{centerX}+{centerY}")
-		
-		self.positiveButtonAction = positiveButtonAction
-		self.negativeButtonAction = negativeButtonAction
-		
-		spacer = tk.Label(self.window, text=" ")
-		messageText = tk.Label(self.window, text=message)
-		spacer2 = tk.Label(self.window, text=" ")
-		
-		buttonsFrame = tk.Frame(self.window)
-		
-		if positiveButtonAction is None:
-			positiveButton = tk.Button(self.window, text=positiveButtonText,
-				fg=positiveButtonColor, command=self.closeWindow)
-			self.window.bind("<Return>", self.closeWindowWithReturnKey)
-		else:
-			positiveButton = tk.Button(self.window, text=positiveButtonText, 
-				fg=positiveButtonColor, command=self.performPositiveAction)
-			self.window.bind("<Return>", self.performPositiveActionWithReturnKey)
-		
-		if negativeButtonAction is None:
-			negativeButton = tk.Button(self.window, text=negativeButtonText, 
-				fg=negativeButtonColor, command=self.closeWindow)
-			self.window.bind("<Escape>", self.closeWindowWithEscapeKey)
-		else:
-			negativeButton = tk.Button(self.window, text=negativeButtonText, 
-				fg=negativeButtonColor, command=self.performNegativeAction)
-			if negativeButtonAction == exit:
-				self.window.bind("<Escape>", self.performNegativeActionWithEscapeKey)
-		
-		negativeButton.pack(in_=buttonsFrame, side=tk.LEFT)
-		positiveButton.pack(in_=buttonsFrame, side=tk.LEFT)
-		
-		spacer.pack()
-		messageText.pack()
-		spacer2.pack()
-		buttonsFrame.pack()
-		
-		if mainWindow:
-			self.window.protocol("WM_DELETE_WINDOW", quit)
-		
-		self.window.mainloop()
-	
-	def closeWindow(self):
-		self.window.destroy()
-		self.window.quit()
-	
-	def closeWindowWithEscapeKey(self, event):
-		self.closeWindow()
-	
-	def closeWindowWithReturnKey(self, event):
-		self.closeWindow()
-	
-	def performPositiveAction(self):
-		self.closeWindow()
-		self.positiveButtonAction()
-	
-	def performPositiveActionWithReturnKey(self, event):
-		self.closeWindow()
-		self.positiveButtonAction()
-	
-	def performNegativeAction(self):
-		self.closeWindow()
-		self.negativeButtonAction()
-	
-	def performNegativeActionWithEscapeKey(self, event):
-		self.closeWindow()
-		self.negativeButtonAction()
+    def __init__(self, title, message, positiveButtonText, negativeButtonText,
+                 positiveButtonAction=None, negativeButtonAction=None, windowWidth=300, windowHeight=140,
+                 positiveButtonColor="blue", negativeButtonColor="black",
+                 mainWindow=False):
+        self.window = tk.Tk()
+        self.window.title(title)
+        centerX = (self.window.winfo_screenwidth() - windowWidth) // 2
+        centerY = (self.window.winfo_screenheight() - windowHeight) // 2
+        self.window.geometry(
+            f"{windowWidth}x{windowHeight}+{centerX}+{centerY}")
+
+        self.positiveButtonAction = positiveButtonAction
+        self.negativeButtonAction = negativeButtonAction
+
+        spacer = tk.Label(self.window, text=" ")
+        messageText = tk.Label(self.window, text=message)
+        spacer2 = tk.Label(self.window, text=" ")
+
+        buttonsFrame = tk.Frame(self.window)
+
+        if positiveButtonAction is None:
+            positiveButton = tk.Button(self.window, text=positiveButtonText,
+                                       fg=positiveButtonColor, command=self.closeWindow)
+            self.window.bind("<Return>", self.closeWindowWithReturnKey)
+        else:
+            positiveButton = tk.Button(self.window, text=positiveButtonText,
+                                       fg=positiveButtonColor, command=self.performPositiveAction)
+            self.window.bind(
+                "<Return>", self.performPositiveActionWithReturnKey)
+
+        if negativeButtonAction is None:
+            negativeButton = tk.Button(self.window, text=negativeButtonText,
+                                       fg=negativeButtonColor, command=self.closeWindow)
+            self.window.bind("<Escape>", self.closeWindowWithEscapeKey)
+        else:
+            negativeButton = tk.Button(self.window, text=negativeButtonText,
+                                       fg=negativeButtonColor, command=self.performNegativeAction)
+            if negativeButtonAction == exit:
+                self.window.bind(
+                    "<Escape>", self.performNegativeActionWithEscapeKey)
+
+        negativeButton.pack(in_=buttonsFrame, side=tk.LEFT)
+        positiveButton.pack(in_=buttonsFrame, side=tk.LEFT)
+
+        spacer.pack()
+        messageText.pack()
+        spacer2.pack()
+        buttonsFrame.pack()
+
+        if mainWindow:
+            self.window.protocol("WM_DELETE_WINDOW", quit)
+
+        self.window.mainloop()
+
+    def closeWindow(self):
+        self.window.destroy()
+        self.window.quit()
+
+    def closeWindowWithEscapeKey(self, event):
+        self.closeWindow()
+
+    def closeWindowWithReturnKey(self, event):
+        self.closeWindow()
+
+    def performPositiveAction(self):
+        self.closeWindow()
+        self.positiveButtonAction()
+
+    def performPositiveActionWithReturnKey(self, event):
+        self.closeWindow()
+        self.positiveButtonAction()
+
+    def performNegativeAction(self):
+        self.closeWindow()
+        self.negativeButtonAction()
+
+    def performNegativeActionWithEscapeKey(self, event):
+        self.closeWindow()
+        self.negativeButtonAction()
+
 
 class ActionDialogWindow(DialogWindow):
-	def __init__(self, title, message, positiveAction=None, negativeAction=None, 
-		negativeColor="red", mainWindow=False):
-		super().__init__(title, message, positiveButtonText="Confirm", negativeButtonText="Cancel",
-			positiveButtonAction=positiveAction, negativeButtonAction=negativeAction,
-			negativeButtonColor=negativeColor, mainWindow=mainWindow)
+    def __init__(self, title, message, positiveAction=None, negativeAction=None,
+                 negativeColor="red", mainWindow=False):
+        super().__init__(title, message, positiveButtonText="Confirm", negativeButtonText="Cancel",
+                         positiveButtonAction=positiveAction, negativeButtonAction=negativeAction,
+                         negativeButtonColor=negativeColor, mainWindow=mainWindow)
+
 
 class InfoDialogWindow(DialogWindow):
-	def __init__(self, title, message, negativeColor="black"):
-		super().__init__(title, message, positiveButtonText="Ok", negativeButtonText="Go back", 
-			negativeButtonColor=negativeColor)
+    def __init__(self, title, message, negativeColor="black"):
+        super().__init__(title, message, positiveButtonText="Ok", negativeButtonText="Go back",
+                         negativeButtonColor=negativeColor)
```

### Comparing `pypimaker-0.1.9/src/upload.py` & `pypimaker-1.0.0/src/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,189 +1,208 @@
 import os
 import subprocess
 import time
 
+from src import strings
+
+
 def upload(filepath):
     checkForRequiredFiles(filepath)
 
     checkWheelInstallation()
     checkTwineInstallation()
-    
+
     versionNumber = getValidVersionNumberForSetupFile(filepath)
     setNewSetupFileVersion(filepath, versionNumber)
 
     createDistributionFiles(filepath)
     uploadDistributionFiles(filepath)
     removeDistributionFiles(filepath)
 
+
 def checkForRequiredFiles(filepath):
     requiredFiles = ["LICENSE", "README.md", "requirements.txt", "setup.py"]
     topLevelDirectoryFiles = set(os.listdir(filepath))
     for file in requiredFiles:
         if file not in topLevelDirectoryFiles:
             print(f"{file} not yet created. Run generatefiles.py first!")
             quit()
-    
+
     if "build" in topLevelDirectoryFiles or "dist" in topLevelDirectoryFiles:
         print("Top-level folders cannot be named 'build' or 'dist'. Please change folder names.")
         quit()
 
+
 def checkWheelInstallation():
     try:
-        import wheel 
+        import wheel
     except:
         commandArray = ["pip", "install", "wheel"]
         commandArray2 = ["pip3", "install", "wheel"]
         try:
             subprocess.call(commandArray)
         except:
             subprocess.call(commandArray2)
         print()
 
+
 def checkTwineInstallation():
     try:
-        import twine 
+        import twine
     except:
         commandArray = ["pip", "install", "twine"]
         commandArray2 = ["pip3", "install", "twine"]
         try:
             subprocess.call(commandArray)
         except:
             subprocess.call(commandArray2)
         print()
 
+
 def getValidVersionNumberForSetupFile(filepath):
     currentSetupFileVersion = getSetupFileVersion(filepath)
-    currentPackageVersion = getCurrentPackageVersion(getPackageNameFromSetupFile(filepath))
+    currentPackageVersion = getCurrentPackageVersion(
+        getPackageNameFromSetupFile(filepath))
     if not versionNumberGreater(currentSetupFileVersion, currentPackageVersion):
         currentSetupFileVersion = getNewSetupFileVersion(currentPackageVersion)
     return currentSetupFileVersion
 
+
 def getSetupFileVersion(filepath):
     with open(filepath + "/setup.py", "r") as file:
         data = file.readlines()
-    
+
     for rawLine in data:
         line = rawLine.split()
         if not len(line):
             continue
-        
+
         if line[0].startswith("version"):
             fullLine = "".join(line)
             currentVersion = fullLine.split("'")[1]
             return currentVersion
-    
-    return DEFAULT_INITIAL_VERSION
+
+    return strings.DEFAULT_INITIAL_VERSION
+
 
 def getCurrentPackageVersion(packageName):
     commandArray = ['pip', 'install', f'{packageName}==nonVersionString']
     result = subprocess.run(commandArray, capture_output=True)
     errorMessage = str(result.stderr)
     if "versions:" not in errorMessage:
         return "0.0.0"
     versions = errorMessage.split("versions:")[-1].split(")")[0].split()
-    versions = [version[:-1] if version.endswith(",") else version for version in versions]
+    versions = [version[:-1]
+                if version.endswith(",") else version for version in versions]
     return "0.0.0" if versions == ["none"] else getLargestVersionNumber(versions)
 
+
 def getPackageNameFromSetupFile(filepath):
     with open(filepath + "/setup.py", "r") as file:
         data = file.readlines()
-    
+
     for rawLine in data:
         line = rawLine.split()
         if not len(line):
             continue
-        
+
         if line[0].startswith("name"):
             fullLine = "".join(line)
             packageName = fullLine.split("'")[1]
             return packageName
-    
+
     raise Exception("No package name found in setup.py")
 
+
 def versionNumberGreater(largerVersion, smallerVersion):
     largerVersionArray = [int(version) for version in largerVersion.split(".")]
-    smallerVersionArray = [int(version) for version in smallerVersion.split(".")]
+    smallerVersionArray = [int(version)
+                           for version in smallerVersion.split(".")]
     largerVersionFirst, largerVersionSecond, largerVersionThird = largerVersionArray
     smallerVersionFirst, smallerVersionSecond, smallerVersionThird = smallerVersionArray
-    
+
     if largerVersionFirst > smallerVersionFirst:
         return True
     elif largerVersionFirst < smallerVersionFirst:
         return False
-    
+
     if largerVersionSecond > smallerVersionSecond:
         return True
     elif largerVersionSecond < smallerVersionSecond:
         return False
-    
+
     return largerVersionThird > smallerVersionThird
 
+
 def getNewSetupFileVersion(currentPackageVersion):
     newVersion = ""
     while newVersion == "":
         newVersion = input(f"The current version number ({currentPackageVersion}) must be \
 incremented. Enter new version number: ")
-        
+
         if not isValidVersionNumber(newVersion):
             newVersion = ""
             continue
-        
+
         if not versionNumberGreater(newVersion, currentPackageVersion):
             newVersion = ""
             continue
-        
+
     print()
     return newVersion
 
+
 def getLargestVersionNumber(versions):
     maxVersion = "0.0.0"
     for version in versions:
         if versionNumberGreater(version, maxVersion):
             maxVersion = version
     return maxVersion
 
+
 def isValidVersionNumber(versionNumber):
     numberArray = versionNumber.split(".")
     if len(numberArray) != 3:
         return False
     try:
         int(numberArray[0])
         int(numberArray[1])
         int(numberArray[2])
         return True
     except:
         return False
 
+
 def setNewSetupFileVersion(filepath, newVersionNumber):
     versionNumberFound = False
     with open(filepath + "/setup.py", "r") as file:
         data = file.readlines()
-    
+
     for index, rawLine in enumerate(data):
         line = rawLine.split()
         if not len(line):
             continue
-        
+
         if line[0].startswith("version"):
             versionIndex = index
             versionNumberFound = True
             break
-    
+
     if not versionNumberFound:
         raise Exception("No version number found in setup.py")
-    
+
     data[versionIndex] = f"    version='{newVersionNumber}', # Required \n"
-    
+
     with open(filepath + "/setup.py", "w") as file:
         file.writelines(data)
 
+
 def createDistributionFiles(filepath):
     setupFilePath = filepath + "/setup.py"
-    
+
     commandArray = ["python", "setup.py", "sdist", "bdist_wheel"]
     commandArray2 = ["python3", "setup.py", "sdist", "bdist_wheel"]
     try:
         subprocess.call(commandArray, cwd=filepath)
     except:
         subprocess.call(commandArray2, cwd=filepath)
 
@@ -192,29 +211,32 @@
     count = 0
     while "dist" not in os.listdir(filepath):
         time.sleep(0.1)
         count += 1
         if count > 50:
             raise Exception("'dist' directory not created successfully")
 
+
 def uploadDistributionFiles(filepath):
     distPath = filepath + "/dist"
 
     count = 0
     while len(os.listdir(distPath)) < 2:
         time.sleep(0.1)
         count += 1
         if count > 50:
-            raise Exception("Files in 'dist' directory not created successfully")
+            raise Exception(
+                "Files in 'dist' directory not created successfully")
 
     commandArray = ["twine", "upload", distPath + "/*"]
     subprocess.call(commandArray)
 
+
 def removeDistributionFiles(filepath):
     foldersToRemove = ["build", "dist"]
     for item in os.listdir(filepath):
         if item.endswith("egg-info"):
             foldersToRemove.append(item)
-    
+
     for folder in foldersToRemove:
         commandArray = ["rm", "-r", filepath + "/" + folder]
         subprocess.run(commandArray, capture_output=True)
```

### Comparing `pypimaker-0.1.9/tests/test_upload.py` & `pypimaker-1.0.0/tests/test_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import unittest
+
 import src.upload as upload
 
 # This unit test uses Python's built-in unit testing framework
 # See https://docs.python.org/3/library/unittest.html for more information
 
+
 class UploadTest(unittest.TestCase):
     def test_correctlyDetectsLargerVersionNumber(self):
         self.assertTrue(upload.versionNumberGreater("1.0.12", "1.0.3"))
         self.assertTrue(upload.versionNumberGreater("1.1.2", "1.0.5"))
         self.assertTrue(upload.versionNumberGreater("0.1.2", "0.0.9"))
         self.assertFalse(upload.versionNumberGreater("0.0.2", "1.0.0"))
         self.assertFalse(upload.versionNumberGreater("5.4.3", "5.5.1"))
         self.assertFalse(upload.versionNumberGreater("1.0.2", "1.0.2"))
-    
+
     def test_getLargestVersionNumber(self):
-        versions = ["1.0.12", "1.0.3", "1.1.2", "1.0.5", "5.4.3", "5.5.1", "0.0.2", "1.0.0"]
+        versions = ["1.0.12", "1.0.3", "1.1.2",
+                    "1.0.5", "5.4.3", "5.5.1", "0.0.2", "1.0.0"]
         largest = upload.getLargestVersionNumber(versions)
         self.assertEqual(largest, "5.5.1")
-    
+
     def test_isValidVersionNumber(self):
         self.assertTrue(upload.isValidVersionNumber("0.0.1"))
         self.assertTrue(upload.isValidVersionNumber("0.12.519"))
         self.assertTrue(upload.isValidVersionNumber("9.0.1"))
         self.assertFalse(upload.isValidVersionNumber("1.0"))
         self.assertFalse(upload.isValidVersionNumber("0.4.g"))
         self.assertFalse(upload.isValidVersionNumber("test"))
 
+
 if __name__ == "__main__":
     unittest.main()
```

