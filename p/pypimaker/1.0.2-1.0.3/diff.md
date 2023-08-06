# Comparing `tmp/pypimaker-1.0.2.tar.gz` & `tmp/pypimaker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypimaker-1.0.2.tar", last modified: Sun Aug  6 02:15:44 2023, max compression
+gzip compressed data, was "dist/pypimaker-1.0.3.tar", last modified: Sun Aug  6 05:04:40 2023, max compression
```

## Comparing `pypimaker-1.0.2.tar` & `pypimaker-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164899 pypimaker-1.0.2/
--rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 02:11:19.000000 pypimaker-1.0.2/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:15:44.164739 pypimaker-1.0.2/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     3589 2023-08-06 02:14:12.000000 pypimaker-1.0.2/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.161964 pypimaker-1.0.2/pypimaker.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 02:15:44.000000 pypimaker-1.0.2/pypimaker.egg-info/top_level.txt
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 02:15:44.164957 pypimaker-1.0.2/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1339 2023-08-06 02:15:43.000000 pypimaker-1.0.2/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.162912 pypimaker-1.0.2/src/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.2/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.2/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)      862 2023-08-06 02:09:48.000000 pypimaker-1.0.2/src/reset.py
--rw-r--r--   0 holly      (501) staff       (20)     7729 2023-08-06 02:13:45.000000 pypimaker-1.0.2/src/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.163815 pypimaker-1.0.2/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     7472 2023-08-06 02:07:27.000000 pypimaker-1.0.2/src/ui/AuthorInfoSelector.py
--rw-r--r--   0 holly      (501) staff       (20)     3859 2023-08-06 02:08:23.000000 pypimaker-1.0.2/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     8246 2023-08-06 02:08:20.000000 pypimaker-1.0.2/src/ui/OptionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.2/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.2/src/ui/navigation.py
--rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 02:09:51.000000 pypimaker-1.0.2/src/upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164250 pypimaker-1.0.2/tests/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.2/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.2/tests/test_upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:15:44.164519 pypimaker-1.0.2/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.2/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.2/tests/ui/test_navigation.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.369444 pypimaker-1.0.3/
+-rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 05:03:46.000000 pypimaker-1.0.3/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 05:04:40.369275 pypimaker-1.0.3/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     3589 2023-08-06 05:03:45.000000 pypimaker-1.0.3/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.366735 pypimaker-1.0.3/pypimaker/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 05:03:52.000000 pypimaker-1.0.3/pypimaker/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1376 2023-08-06 05:03:51.000000 pypimaker-1.0.3/pypimaker/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)     9987 2023-08-06 05:03:51.000000 pypimaker-1.0.3/pypimaker/files.py
+-rw-r--r--   0 holly      (501) staff       (20)      874 2023-08-06 05:03:50.000000 pypimaker-1.0.3/pypimaker/reset.py
+-rw-r--r--   0 holly      (501) staff       (20)     7734 2023-08-06 05:03:48.000000 pypimaker-1.0.3/pypimaker/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.368274 pypimaker-1.0.3/pypimaker/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     7484 2023-08-06 05:03:53.000000 pypimaker-1.0.3/pypimaker/ui/AuthorInfoSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)     3859 2023-08-06 05:03:49.000000 pypimaker-1.0.3/pypimaker/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     8270 2023-08-06 05:03:47.000000 pypimaker-1.0.3/pypimaker/ui/OptionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.3/pypimaker/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1701 2023-08-06 05:03:47.000000 pypimaker-1.0.3/pypimaker/ui/navigation.py
+-rw-r--r--   0 holly      (501) staff       (20)     7130 2023-08-06 05:03:50.000000 pypimaker-1.0.3/pypimaker/upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.367490 pypimaker-1.0.3/pypimaker.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 05:04:40.000000 pypimaker-1.0.3/pypimaker.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      572 2023-08-06 05:04:40.000000 pypimaker-1.0.3/pypimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 05:04:40.000000 pypimaker-1.0.3/pypimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       54 2023-08-06 05:04:40.000000 pypimaker-1.0.3/pypimaker.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       16 2023-08-06 05:04:40.000000 pypimaker-1.0.3/pypimaker.egg-info/top_level.txt
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 05:04:40.369543 pypimaker-1.0.3/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1365 2023-08-06 05:04:40.000000 pypimaker-1.0.3/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.368735 pypimaker-1.0.3/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.3/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2909 2023-08-06 05:03:53.000000 pypimaker-1.0.3/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     1441 2023-08-06 05:03:54.000000 pypimaker-1.0.3/tests/test_upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 05:04:40.369026 pypimaker-1.0.3/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.3/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1288 2023-08-06 05:03:55.000000 pypimaker-1.0.3/tests/ui/test_navigation.py
```

### Comparing `pypimaker-1.0.2/LICENSE` & `pypimaker-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.2/PKG-INFO` & `pypimaker-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.2
+Version: 1.0.3
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
 
-- 1.0.2
+- 1.0.3
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.2/README.md` & `pypimaker-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
-- 1.0.2
+- 1.0.3
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.2/pypimaker.egg-info/PKG-INFO` & `pypimaker-1.0.3/pypimaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.2
+Version: 1.0.3
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
 
-- 1.0.2
+- 1.0.3
   - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.2/setup.py` & `pypimaker-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='pypimaker',  # Required
-    version='1.0.2', # Required 
+    version='1.0.3', # Required 
     description='Software designed for simplifying PyPI Python package setups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/pypimaker',
     author='Brian Davis',
         classifiers=[  # Defined at https://pypi.org/classifiers/
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3',
             'Operating System :: Unix',
             'Operating System :: MacOS :: MacOS X',
             'Operating System :: Microsoft :: Windows'
         ],
     packages=find_packages(),  # Required
-    py_modules=['src', 'src.ui', 'tests'],  # Generated
+    py_modules=['pypimaker', 'pypimaker.ui', 'tests'],  # Generated
     python_requires='>=3.7, <4',
     project_urls={
         'Bug Reports': 'https://github.com/bdavis222/pypimaker/issues',
         'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
         'Source': 'https://github.com/bdavis222/',
-    },
+        },
     entry_points={
         'console_scripts': [
-            'pypimaker = src.__main__:main'
+            'pypimaker = pypimaker.__main__:main'
         ]
-    }
+        }
 )
```

### Comparing `pypimaker-1.0.2/src/__main__.py` & `pypimaker-1.0.3/pypimaker/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import sys
 
-from src import strings
-import src.files as files
-import src.reset as reset
-import src.upload as upload
-from src.ui import navigation
-from src.ui.OptionSelector import OptionSelector
+from pypimaker import strings
+import pypimaker.files as files
+import pypimaker.reset as reset
+import pypimaker.upload as upload
+from pypimaker.ui import navigation
+from pypimaker.ui.OptionSelector import OptionSelector
 
 
 def main(argv=sys.argv):
     parser = argparse.ArgumentParser(
         description="Example input: pypimaker generate")
     parser.add_argument(
         "command",
```

### Comparing `pypimaker-1.0.2/src/files.py` & `pypimaker-1.0.3/pypimaker/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import os
 import subprocess
 
-from src import strings
-from src.ui.DialogWindow import DialogWindow
+from pypimaker import strings
+from pypimaker.ui.DialogWindow import DialogWindow
 
 
 def generate(filepath, projectName, authorsArray, emailsArray, correspondingEmail, githubUsername,
              shortDescription, classifier, mainFunctionPath):
     checkForUnitTests(filepath)
     generateRequirementsFile(filepath)
     generateGitIgnoreFile(filepath)
@@ -73,17 +73,19 @@
     return newPaths
 
 
 def createTestFiles(filepath, newPaths, importStrings):
     startingIndex = len(filepath.split("/"))
     for path, importString in zip(newPaths, importStrings):
         directory = "/".join(path.split("/")[:-1])
+        filename = path.split("/")[-1].split(".")[0]
+        camelArray = [word.capitalize() for word in filename.split("_")]
         contents = strings.TEST_FILE_CONTENTS.format(
             importString=importString,
-            moduleName=path.split("/")[-1].split(".")[0].capitalize()
+            camelName="".join(camelArray)
         )
 
         subprocess.call(["mkdir", "-p", directory])
 
         filename = path.split("/")[-1]
         newPathName = "".join([directory, "/", "test_", filename])
         with open(newPathName, "w") as file:
```

### Comparing `pypimaker-1.0.2/src/reset.py` & `pypimaker-1.0.3/pypimaker/reset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 
-from src import strings
-from src.ui.DialogWindow import ActionDialogWindow
+from pypimaker import strings
+from pypimaker.ui.DialogWindow import ActionDialogWindow
 
 
 def reset(topLevelDirectory):
     ActionDialogWindow("Are you sure?", strings.RESET_SELECTION_TEXT,
                        negativeAction=exit, mainWindow=True)
 
     filesToRemove = ["LICENSE", "README.md",
```

### Comparing `pypimaker-1.0.2/src/strings.py` & `pypimaker-1.0.3/pypimaker/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 TEST_FILE_CONTENTS = '''import unittest
 {importString}
 
 # This unit test uses Python's built-in unit testing framework
 # See https://docs.python.org/3/library/unittest.html for more information
 
-class {moduleName}Test(unittest.TestCase):
+class {camelName}Test(unittest.TestCase):
     def test_condition_doesThis_whenThis(self):
         pass
 
 if __name__ == "__main__":
     unittest.main()
 '''
 
@@ -132,15 +132,15 @@
 
 ## Development
 
 To contribute, download or clone the project. From the top level of the project's folder structure, \
 one can use the following command to run a local version of the software (e.g., for UI testing):
 
 ```
-python -m src
+python -m pypimaker
 ```
 
 *(Note that the* `python3` *command may be required instead of* `python` *for some Python installations.)*
 
 ### Testing
 
 Unit tests for this software were written for use with [Python's built-in unittest \
```

### Comparing `pypimaker-1.0.2/src/ui/AuthorInfoSelector.py` & `pypimaker-1.0.3/pypimaker/ui/AuthorInfoSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import tkinter as tk
 
-from src import strings
-from src.ui.DialogWindow import ActionDialogWindow, InfoDialogWindow
+from pypimaker import strings
+from pypimaker.ui.DialogWindow import ActionDialogWindow, InfoDialogWindow
 
 
 class AuthorInfoSelector:
     def __init__(self):
         self.window = tk.Tk()
         self.window.title("PyPI Maker")
         centerX = (self.window.winfo_screenwidth() - 650) // 2
```

### Comparing `pypimaker-1.0.2/src/ui/DialogWindow.py` & `pypimaker-1.0.3/pypimaker/ui/DialogWindow.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.2/src/ui/OptionSelector.py` & `pypimaker-1.0.3/pypimaker/ui/OptionSelector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tkinter as tk
 from tkinter import filedialog
 
-from src import strings
-import src.ui.navigation as navigation
-from src.ui.AuthorInfoSelector import AuthorInfoSelector
-from src.ui.DialogWindow import ActionDialogWindow, DialogWindow, InfoDialogWindow
+from pypimaker import strings
+import pypimaker.ui.navigation as navigation
+from pypimaker.ui.AuthorInfoSelector import AuthorInfoSelector
+from pypimaker.ui.DialogWindow import ActionDialogWindow, DialogWindow, InfoDialogWindow
 
 EMPTY_DIRECTORY_SET = set(["", " ", "/"])
 
 
 class OptionSelector:
     def __init__(self):
         self.window = tk.Tk()
```

### Comparing `pypimaker-1.0.2/src/ui/navigation.py` & `pypimaker-1.0.3/pypimaker/ui/navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import tkinter as tk
 from tkinter import filedialog
 
-from src import strings
+from pypimaker import strings
 
 
 def getDirectory():
     filepath = ""
     tk.Tk().withdraw()
     chosenFolder = filedialog.askdirectory(
         initialdir=filepath, title=strings.SELECT_FOLDER_TEXT)
```

### Comparing `pypimaker-1.0.2/src/upload.py` & `pypimaker-1.0.3/pypimaker/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import time
 
-from src import strings
+from pypimaker import strings
 
 
 def upload(filepath):
     checkForRequiredFiles(filepath)
 
     checkWheelInstallation()
     checkTwineInstallation()
```

### Comparing `pypimaker-1.0.2/tests/test_files.py` & `pypimaker-1.0.3/tests/test_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-import src.files as files
+import pypimaker.files as files
 
 # This unit test uses Python's built-in unit testing framework
 # See https://docs.python.org/3/library/unittest.html for more information
 
 
 class FilesTest(unittest.TestCase):
     def test_getNamesAndEmailsVerticallySpaced_spacesInfoProperly(self):
```

### Comparing `pypimaker-1.0.2/tests/test_upload.py` & `pypimaker-1.0.3/tests/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-import src.upload as upload
+import pypimaker.upload as upload
 
 # This unit test uses Python's built-in unit testing framework
 # See https://docs.python.org/3/library/unittest.html for more information
 
 
 class UploadTest(unittest.TestCase):
     def test_correctlyDetectsLargerVersionNumber(self):
```

### Comparing `pypimaker-1.0.2/tests/ui/test_navigation.py` & `pypimaker-1.0.3/tests/ui/test_navigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
-from src import strings
-import src.ui.navigation as navigation
+from pypimaker import strings
+import pypimaker.ui.navigation as navigation
 
 # This unit test uses Python's built-in unit testing framework
 # See https://docs.python.org/3/library/unittest.html for more information
 
 
 class NavigationTest(unittest.TestCase):
     def test_getPathFromBase(self):
```

