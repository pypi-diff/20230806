# Comparing `tmp/FiveMCipherFinder-2.3.0.tar.gz` & `tmp/FiveMCipherFinder-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-2.3.0.tar", last modified: Wed Jul 19 05:38:36 2023, max compression
+gzip compressed data, was "FiveMCipherFinder-2.4.0.tar", last modified: Sun Aug  6 00:46:05 2023, max compression
```

## Comparing `FiveMCipherFinder-2.3.0.tar` & `FiveMCipherFinder-2.4.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 05:38:36.000000 FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8278 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-19 05:38:36.954442 FiveMCipherFinder-2.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-07-19 05:38:25.000000 FiveMCipherFinder-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 00:46:05.000000 FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3604 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/cipherFinder/de_obfs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10507 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:46:05.293565 FiveMCipherFinder-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/tests/test_de_obfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-06 00:45:54.000000 FiveMCipherFinder-2.4.0/tests/test_finder.py
```

### Comparing `FiveMCipherFinder-2.3.0/FiveMCipherFinder.egg-info/PKG-INFO` & `FiveMCipherFinder-2.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-Metadata-Version: 2.1
-Name: FiveMCipherFinder
-Version: 2.3.0
-Summary: Finds Cipher in lua scripts.
-Home-page: https://github.com/exersalza/FivemCipherFinder
-Author: exersalza
-License: MIT
-Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
-Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FivemCipherFinder (v2.3.0)
+# FivemCipherFinder (v2.4.0)
 
 <div align="center">
-  <h2> Visitors </h2>
-<img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
+    <h2> Visitors </h2>
+    <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
-[![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 - [Installation](#installation)
 - [Usage](#Usage)
 - [Troubleshooting](#Troubleshooting)
 - [Known false-positives](#known-false-positives)
+- [Contributing](#Contributing)
 - [Todo](#todo)
 - [Contact](#Contact)
 
 This is a Fivem Cipher finder for those that don't want Ciphers in their scripts :D
 
 The idea behind these scripts is to find one or more Cipher in your script files. 
 Currently, there is only the Python version available, but I will soon add the C++ variant.
 
 Desc:
 The script will walk through your Server's directories and scan, for example, `\x41\x42\x43`. When it found something it will write the line and trigger it into a Log file.
 
 ## Installation
-Py-Version: 3.8 and above
+Py-Version: 3.8 and above [Newest python version](https://python.org/downloads/)
 
+**Please make sure, that when you're on Windows based system, that you've added Python to your environment variables. You can test that with simply typing `python --version` into your CMD or Terminal**
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
+Also please consider using the pip way to install except **you know what you're doing**
+
 Make sure to read the [Troubleshooting](#Troubleshooting) page first before you add me on Discord.
 
-## Install instructions for Python
-Py-Version: 3.8 and above
 
-run `pip install FivemCipherFinder` or download the latest release and unpack it.
+### For manual installation
+
+I just put the commands here
+- `git clone https://github.com/exersalza/FivemCipherFinder.git && cd FivemCipherFinder`
+- `pip install -r req`
+- `python3 -m build . && pip install .`
+Then you can just type `find-cipher` in your server resources directory.
 
 ## Usage
 
 Syntax: `find-cipher [-h] [-p [PATH]] [-x [EXCLUDE_PATH ...]] [-n] [-v] [--v2]`
 Options are:
 - `-p|--path` -> Redirect the search from the current path `.` to another one.
 - `-x|--exclude` -> Exclude paths that you dont want to scan. 
@@ -68,25 +61,33 @@
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ### Troubleshooting
 
+**First things first, read the error/warning message**
+
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
 
 Also make sure (on Windows) that you have your python scripts folder inside your path variable. Should the folder be missing, it shows at the pip installation as a warning. [how to add something to the path variable](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
 
 
 ## Known-false-positives
 
 - `EasyAdmin`
 - `encrypted/obfuscated scripts`
 
+## Contributing
+
+Feel free to open a PR with your changes, as every PR the checks should run without a fail
+to run workflows localy please consider using [act](https://github.com/nektos/act)
+
+Use the manual installation guide for getting the project. [Installation](#Installation)
 
 ## ToDo
 - Detect cipher spreader
-- Add de obfuscator for detectet cipher
+- ~~Add de obfuscator for detectet cipher~~
 - ~~Find random generated character variable names~~
 
 ## Contact
 Discord: exersalza / exersalza[>'-']>#1337 | [DE/EN]
```

### Comparing `FiveMCipherFinder-2.3.0/LICENSE` & `FiveMCipherFinder-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.3.0/PKG-INFO` & `FiveMCipherFinder-2.4.0/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.3.0
+Version: 2.4.0
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# FivemCipherFinder (v2.3.0)
+# FivemCipherFinder (v2.4.0)
 
 <div align="center">
-  <h2> Visitors </h2>
-<img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
+    <h2> Visitors </h2>
+    <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
-[![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 - [Installation](#installation)
 - [Usage](#Usage)
 - [Troubleshooting](#Troubleshooting)
 - [Known false-positives](#known-false-positives)
+- [Contributing](#Contributing)
 - [Todo](#todo)
 - [Contact](#Contact)
 
 This is a Fivem Cipher finder for those that don't want Ciphers in their scripts :D
 
 The idea behind these scripts is to find one or more Cipher in your script files. 
 Currently, there is only the Python version available, but I will soon add the C++ variant.
 
 Desc:
 The script will walk through your Server's directories and scan, for example, `\x41\x42\x43`. When it found something it will write the line and trigger it into a Log file.
 
 ## Installation
-Py-Version: 3.8 and above
+Py-Version: 3.8 and above [Newest python version](https://python.org/downloads/)
 
+**Please make sure, that when you're on Windows based system, that you've added Python to your environment variables. You can test that with simply typing `python --version` into your CMD or Terminal**
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
+Also please consider using the pip way to install except **you know what you're doing**
+
 Make sure to read the [Troubleshooting](#Troubleshooting) page first before you add me on Discord.
 
-## Install instructions for Python
-Py-Version: 3.8 and above
 
-run `pip install FivemCipherFinder` or download the latest release and unpack it.
+### For manual installation
+
+I just put the commands here
+- `git clone https://github.com/exersalza/FivemCipherFinder.git && cd FivemCipherFinder`
+- `pip install -r req`
+- `python3 -m build . && pip install .`
+Then you can just type `find-cipher` in your server resources directory.
 
 ## Usage
 
 Syntax: `find-cipher [-h] [-p [PATH]] [-x [EXCLUDE_PATH ...]] [-n] [-v] [--v2]`
 Options are:
 - `-p|--path` -> Redirect the search from the current path `.` to another one.
 - `-x|--exclude` -> Exclude paths that you dont want to scan. 
@@ -68,25 +78,33 @@
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ### Troubleshooting
 
+**First things first, read the error/warning message**
+
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
 
 Also make sure (on Windows) that you have your python scripts folder inside your path variable. Should the folder be missing, it shows at the pip installation as a warning. [how to add something to the path variable](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
 
 
 ## Known-false-positives
 
 - `EasyAdmin`
 - `encrypted/obfuscated scripts`
 
+## Contributing
+
+Feel free to open a PR with your changes, as every PR the checks should run without a fail
+to run workflows localy please consider using [act](https://github.com/nektos/act)
+
+Use the manual installation guide for getting the project. [Installation](#Installation)
 
 ## ToDo
 - Detect cipher spreader
-- Add de obfuscator for detectet cipher
+- ~~Add de obfuscator for detectet cipher~~
 - ~~Find random generated character variable names~~
 
 ## Contact
 Discord: exersalza / exersalza[>'-']>#1337 | [DE/EN]
```

### Comparing `FiveMCipherFinder-2.3.0/README.md` & `FiveMCipherFinder-2.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,69 @@
-# FivemCipherFinder (v2.3.0)
+Metadata-Version: 2.1
+Name: FiveMCipherFinder
+Version: 2.4.0
+Summary: Finds Cipher in lua scripts.
+Home-page: https://github.com/exersalza/FivemCipherFinder
+Author: exersalza
+License: MIT
+Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
+Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FivemCipherFinder (v2.4.0)
 
 <div align="center">
-  <h2> Visitors </h2>
-<img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
+    <h2> Visitors </h2>
+    <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
-[![Pylint](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
+[![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 - [Installation](#installation)
 - [Usage](#Usage)
 - [Troubleshooting](#Troubleshooting)
 - [Known false-positives](#known-false-positives)
+- [Contributing](#Contributing)
 - [Todo](#todo)
 - [Contact](#Contact)
 
 This is a Fivem Cipher finder for those that don't want Ciphers in their scripts :D
 
 The idea behind these scripts is to find one or more Cipher in your script files. 
 Currently, there is only the Python version available, but I will soon add the C++ variant.
 
 Desc:
 The script will walk through your Server's directories and scan, for example, `\x41\x42\x43`. When it found something it will write the line and trigger it into a Log file.
 
 ## Installation
-Py-Version: 3.8 and above
+Py-Version: 3.8 and above [Newest python version](https://python.org/downloads/)
 
+**Please make sure, that when you're on Windows based system, that you've added Python to your environment variables. You can test that with simply typing `python --version` into your CMD or Terminal**
 run `pip install FivemCipherFinder` or download the latest release and unpack it.
 
+Also please consider using the pip way to install except **you know what you're doing**
+
 Make sure to read the [Troubleshooting](#Troubleshooting) page first before you add me on Discord.
 
-## Install instructions for Python
-Py-Version: 3.8 and above
 
-run `pip install FivemCipherFinder` or download the latest release and unpack it.
+### For manual installation
+
+I just put the commands here
+- `git clone https://github.com/exersalza/FivemCipherFinder.git && cd FivemCipherFinder`
+- `pip install -r req`
+- `python3 -m build . && pip install .`
+Then you can just type `find-cipher` in your server resources directory.
 
 ## Usage
 
 Syntax: `find-cipher [-h] [-p [PATH]] [-x [EXCLUDE_PATH ...]] [-n] [-v] [--v2]`
 Options are:
 - `-p|--path` -> Redirect the search from the current path `.` to another one.
 - `-x|--exclude` -> Exclude paths that you dont want to scan. 
@@ -51,25 +78,33 @@
 
 As you can see in the last example, you can exclude Directories so can prevent false-positives like `\[cars\],\[mlos\],easy-admin` but make sure you add `\` before curly and square brackets, otherwise your terminal will throw an error.
 
 The script logs found Cipher in a file names `CipherLog-HH-MM-SS.txt` so can easily find your log files.
 
 ### Troubleshooting
 
+**First things first, read the error/warning message**
+
 Should the installation with pip fail with the error code `externally-managed-environment`, add `--break-system-packages`. Pip changed something in their internals in the newer versions.
 
 Also make sure (on Windows) that you have your python scripts folder inside your path variable. Should the folder be missing, it shows at the pip installation as a warning. [how to add something to the path variable](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/)
 
 
 ## Known-false-positives
 
 - `EasyAdmin`
 - `encrypted/obfuscated scripts`
 
+## Contributing
+
+Feel free to open a PR with your changes, as every PR the checks should run without a fail
+to run workflows localy please consider using [act](https://github.com/nektos/act)
+
+Use the manual installation guide for getting the project. [Installation](#Installation)
 
 ## ToDo
 - Detect cipher spreader
-- Add de obfuscator for detectet cipher
+- ~~Add de obfuscator for detectet cipher~~
 - ~~Find random generated character variable names~~
 
 ## Contact
 Discord: exersalza / exersalza[>'-']>#1337 | [DE/EN]
```

### Comparing `FiveMCipherFinder-2.3.0/cipherFinder/finder.py` & `FiveMCipherFinder-2.4.0/cipherFinder/finder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,283 @@
 #!/bin/python3.11
 
 #  Copyright (c) 2022-2023 - exersalza
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
-#  of this software and associated documentation files (the "Software"), to deal
+#  of this software and associated documentation files (the "Software"), to deal # noqa
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
 #
-#  The above copyright notice and this permission notice shall be included in all
+#  The above copyright notice and this permission notice shall be included in all # noqa
 #  copies or substantial portions of the Software.
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, # noqa
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE # noqa
 #  SOFTWARE.
 from __future__ import annotations
 from datetime import datetime as dt
 
 import os
-import re
 import sys
 import platform
 import argparse
 import requests
 
 from gibberish_detector import detector
 
-REGEX = r'(((\\x|\\u)([a-fA-F0-9]{2})){2})'
-COLORS = ['\033[0m', '\033[91m', '\033[92m']
-RAW_BIG_MODEL = 'https://raw.githubusercontent.com/exersalza/FivemCipherFinder/main/big.model'
+from cipherFinder.de_obfs import de_obfs, do_regex
+
+REGEX = r"(((\\x|\\u)([a-fA-F0-9]{2}))+)"
+URL_REGEX = (
+    r"(https?://(www\.)?[-\w@:%.\+~#=]{2,256}\."
+    r"[a-z]{2,4}\b([-\w@:%\+.~#?&//=]*))"
+)
+COLORS = ["\033[0m", "\033[91m", "\033[92m"]
+RAW_BIG_MODEL = (
+    "https://raw.githubusercontent.com/exersalza/"
+    "FivemCipherFinder/main/big.model"
+)
 
 log = []
 
+
 def get_big_model_file() -> int:
-    # Check if the big.model file exists
-    if not os.path.exists('./big.model'):
-        with open('big.model', 'wb') as _file:
-            for chunk in requests.get(RAW_BIG_MODEL, 
-                                      stream=True, timeout=5) \
-                    .iter_content(chunk_size=8192):
-                if not chunk: continue
+    """Get the big.model file from GitHub.
 
-                _file.write(chunk)
+    Returns
+    -------
+    int :
+        status code
 
+    """
+    if os.path.exists("./big.model"):
+        os.remove("./big.model")
+
+    with open("big.model", "wb") as _file:
+        for chunk in requests.get(
+            RAW_BIG_MODEL, stream=True, timeout=5
+        ).iter_content(chunk_size=8192):
+            if not chunk:
+                continue
+
+            _file.write(chunk)
     return 0
 
 
 def validate_lines(lines: list) -> list[tuple]:
-    """ Validate the lines that are given through the 'lines' parameter.
+    """Validate the lines that are given through the 'lines' parameter.
 
     Parameters
     ----------
     lines : list
         The lines from the current read file.
 
     Returns
     -------
     list[tuple]
-        A list with infected lines 
+        A list with infected line
         (or false positives by AntiCheat or obfuscated code)
     """
 
     ret: list[tuple] = []
 
     for ln, line in enumerate(lines, start=1):  # ln: lineNumber
-        if re.findall(REGEX, rf'{line}', re.MULTILINE and re.IGNORECASE):
-            ret.append((ln, line))
-
+        # get all the lines that match the regex
+        if x := do_regex(line, REGEX):
+            ret.append((ln, line, de_obfs(x, line)))
     return ret
 
 
-def do_gibberish_check(lines: list) -> list[tuple[str, int]]:
-    """ Do a check if the given lines are making any sens.
+def do_gibberish_check(lines: list) -> list[tuple[str, int, str]]:
+    """Do a check if the given lines are making any sens.
     Can still throw false-positives
 
     Parameters
     ----------
     lines : list
         The lines from the current read file.
 
     Returns
     -------
-    list[tuple[str, int]]
+    list[tuple[str, int, str]]
         A Tuple List with infected lines or false positives
         as in `validate_lines`.
 
     """
 
-    det = detector.create_from_model('./big.model')  # should work for now
+    det = detector.create_from_model("./big.model")  # should work for now
     l_counter = 1
     matches = []
 
     for i in lines:
-        if 'local' in i and det.is_gibberish(rf'{i}'):
-            matches.append((l_counter, i))
+        if "local" in i and det.is_gibberish(rf"{i}"):
+            matches.append(
+                (l_counter, i, "Can't de obfuscate due to use of --v2")
+            )
 
         l_counter += 1
     return matches
 
 
-def check_file(d: str, file: str, count: int, args: argparse.Namespace) -> tuple[int, int]: 
-    """ Iterate over a file and check the lines
+def prepare_log_line(**kw) -> int:
+    """Prepares the string for the logging
+
+    Parameters
+    ----------
+    kw : str, Any
+        Somevalues listed below
+
+    Returns
+    -------
+    int
+        Returns the current count
+    """
+    d = kw.pop("d", ".")
+    ln = kw.pop("ln", "")
+    file = kw.pop("file", "poggers.lua")
+    line = kw.pop("line", "")
+    count = kw.pop("count", 0)
+    target = kw.pop("target", "")
+    logged = kw.pop("logged", {})
+
+    path = d.replace("\\", "/") + f"/{file}"
+    url = ""
+
+    if x := do_regex(target, URL_REGEX):
+        url = x[0][0]
+
+    # prevent printing stuff twice to the log file
+    if logged.get(path, -1) == ln:
+        return count
+
+    to_log = (
+        f"File: {path}\n"
+        f"LineNumber: {ln}\n"
+        f"Attacker URL: {url}\n"
+        f"DecodedLines: \n{'-'*10}\n{target}\n{'-'*10}"
+    )
+
+    if kw.pop("verbose", False):  # Log in console.
+        print(to_log)
+
+    log.append(to_log + f"\nTrigger Line:\n{line!r}\n{'-'*15}\n")
+    count += 1
+    logged[path] = ln
+    return count
+
+
+def check_file(
+    d: str, file: str, count: int, args: argparse.Namespace
+) -> tuple[int, int]:
+    """Iterate over a file and check the lines
 
     Parameters
     ----------
     d : str
         Give the path to the file e.g "/home/wildCiphers"
     file : str
         Give a file name to scan e.g "wildCipherInHere.lua"
     count: int
         Give the current cipher count.
     args: argparse.Namespace
         Give the arguments delieverd from the Cmd line.
-    
+
     Returns
     -------
     tuple[ret_code, count]
         A Tuple with the return code and the current cipher count.
     """
 
-    with open(f'{d}/{file}', 'r', encoding='utf-8') as f:
+    with open(f"{d}/{file}", "r", encoding="utf-8") as f:
         try:
             lines = f.readlines()
         except UnicodeDecodeError:
-            print(f'Can\'t decode `{d}/{file}`.')
+            print(f"Can't decode `{d}/{file}`. File is not utf-8")
             return 1, count
-        
+
         match = validate_lines(lines)
-        
+        logged = {}
+
         if args.v2:
             match += do_gibberish_check(lines)
 
-        if match:
-            for ln, line in match:
-                path = d.replace('\\', '/') + f'/{file}'
-                to_log = f'File: {path}\nLineNumber: {ln}\n'
+        if not match:
+            return 0, count
 
-                if args.verbose:  # Log in console.
-                    print(to_log)
+        for ln, line, target in match:
+            count = prepare_log_line(
+                d=d,
+                ln=ln,
+                file=file,
+                line=line,
+                count=count,
+                target=target,
+                logged=logged,
+                verbose=args.verbose,
+            )
+    return 0, count
 
 
-                log.append(to_log + f'Line: {line!r}\n----------------\n')
-                count += 1
-    return 0, count
+def write_log_file(**kw) -> int:
+    """Writes the logfile
 
+    Parameters
+    ----------
+    kw : dict
+        red : str : Colorcode for red
+        white : str : Colorcode for white
+        count : int : The found cipher count
+
+    Returns
+    -------
+    int
+        Statuscode
+    """
+    print(
+        f'{kw.pop("red")}Oh no, the program found a spy in your files x.x '
+        f"Check the CipherLog.txt for location and trigger. "
+        f'{kw.pop("count")} where found!'
+        f'{kw.pop("white")}\n#staysafe'
+    )
 
-def write_log_file(**kw) -> int: 
-    if kw.pop('args').no_log:
+    if kw.pop("args").no_log:
         return 0
 
-    with open(f'CipherLog-{dt.now():%H-%M-%S}.txt', 'w+', encoding='utf-8') as f:
+    with open(
+        f"CipherLog-{dt.now():%H-%M-%S}.txt", "w+", encoding="utf-8"
+    ) as f:
         f.writelines(log)
-        
-        print(f'{kw.pop("red")}Oh no, the program found a spy in your files x.x '
-          f'Check the CipherLog.txt for location and trigger. {kw.pop("count")} where found!'
-          f'{kw.pop("white")}\n#staysafe')
+
     return 0
 
 
 def main() -> int:
-    """ Validates lua files.
+    """Validates lua files.
 
     Usage:
     ------
     Run the program: `find-cipher [path] [exclude path] [OPTIONS...]`.
 
     args:
-        --path : Optional : 
-            Give the path to search, when no path is given, the 
+        --path : Optional :
+            Give the path to search, when no path is given, the
             current working directory will be used `.`
-        --exclude-path : Optional : 
+        --exclude-path : Optional :
             Exclude directory's where you don't want to search.
         --no-log: Optional :
             Don't create a log file, can be used hand in hand with --verbose
-        --verbose : Optional : 
+        --verbose : Optional :
             Print a Cipher directly to the Command line on found.
-        --v2 : Optional : 
+        --v2 : Optional :
             Uses an extra algorithm to find gibberish or randomly generated
             variable/function/table names. It can introduce more palse-positiv
             because of obfuscated scripts, but can help to find ciphers.
 
     Advertisement:
     --------------
     Get your beautiful Cipher today, just smack the play button and find some.
@@ -194,61 +287,113 @@
 
     Returns
     -------
     int
         Return code
     """
 
-    parser = argparse.ArgumentParser(description='Validates lua files.')
+    parser = argparse.ArgumentParser(description="Validates lua files.")
 
-    parser.add_argument('-p', '--path', nargs='?', default='.',
-                        help='Give the path to search, when no path is given, the current working directory will be used "."')
-    parser.add_argument('-x', '--exclude', nargs='*', default='',
-                        help='Exclude directories where you don\'t want to search.')
-    parser.add_argument('-n', '--no-log', action='store_true',
-                        help='Don\'t create a log file, can be used hand in hand with --verbose')
-    parser.add_argument('-v', '--verbose', action='store_true',
-                        help='Print a Cipher directly to the Command line on found.')
-    parser.add_argument('--v2', action='store_true',
-                        help='Uses an extra algorithm to find gibberish or randomly generated variable/function/table names. It can introduce more false-positives because of obfuscated scripts but can help find ciphers.')
+    parser.add_argument(
+        "-p",
+        "--path",
+        nargs="?",
+        default=".",
+        help="Give the path to search, when no path is given"
+        ', the current working directory will be used "."',
+    )
+
+    parser.add_argument(
+        "-x",
+        "--exclude",
+        nargs="*",
+        default="",
+        help="Exclude directories where you don't want to" " search.",
+    )
+
+    parser.add_argument(
+        "-n",
+        "--no-log",
+        action="store_true",
+        help="Don't create a log file, can be used hand in hand with -v",
+    )
+
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Print a Cipher directly to the Command line " " on found.",
+    )
+
+    parser.add_argument(
+        "--v2",
+        action="store_true",
+        help="Uses an extra algorithm to find gibberish "
+        "or randomly generated variable/function/table "
+        "names. It can introduce more false-positives "
+        "because of obfuscated scripts but "
+        "can help find ciphers.",
+    )
+
+    parser.add_argument(
+        "--no-del",
+        action="store_true",
+        help="Debug command to not delete the big.model "
+        "file after the script finishes.",
+    )
+
+    parser.add_argument(
+        "--get-train-file",
+        action="store_true",
+        help="Debug command to get the big.model file",
+    )
 
     args = parser.parse_args()
 
-    pattern = ''.join([(i.replace(',', ')|(') if '--' not in i else '') for i in args.exclude])
+    if args.get_train_file:
+        get_big_model_file()
+        return 0
+
+    pattern = "".join(
+        [
+            (i.replace(",", ")|(") if "--" not in i else "")
+            for i in args.exclude
+        ]
+    )
     local_path = args.path
-    count = 0 
+    count = 0
+
+    if args.v2:
+        # sure there are other ways, but python is doing python stuff.
+        get_big_model_file()
 
-    get_big_model_file()  # sure there are other ways, but python is doing python stuff.
-    
     for d, _, files in os.walk(local_path):
-        if pattern and re.findall(f'{"(" + pattern + ")"}', 
-                                  fr'{d}'.format(d=d), re.MULTILINE and re.IGNORECASE):
+        if pattern and do_regex(rf"{d}", f'{"(" + pattern + ")"}'):
             continue
 
         for file in files:
-            if '.lua' not in file:
+            if ".lua" not in file:
                 continue
 
             _, count = check_file(d, file, count, args)
+
     # Write log
-    
-    red = green = white = ''
+    red = green = white = ""
 
-    if 'linux' in platform.platform().lower():
+    if "linux" in platform.platform().lower():
         white, red, green = COLORS
-    
+
     try:
-        os.remove('big.model')
+        if not args.no_del:
+            os.remove("big.model")
     except FileNotFoundError:
         pass
 
     if log:
-        return write_log_file(white=white, red=red, 
-                              count=count, args=args)
-
-    print(f'{green}Nice! There were no Cipher\'s found!{white}')
+        return write_log_file(white=white, red=red, count=count, args=args)
 
+    print(f"{green}Nice! There were no Cipher's found!{white}")
     return 0
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `FiveMCipherFinder-2.3.0/setup.cfg` & `FiveMCipherFinder-2.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 2.3.0
+version = 2.4.0
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls =
```

