# Comparing `tmp/pypimaker-1.0.0.tar.gz` & `tmp/pypimaker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypimaker-1.0.0.tar", last modified: Sun Aug  6 01:59:20 2023, max compression
+gzip compressed data, was "dist/pypimaker-1.0.1.tar", last modified: Sun Aug  6 02:11:25 2023, max compression
```

## Comparing `pypimaker-1.0.0.tar` & `pypimaker-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.707092 pypimaker-1.0.0/
--rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 01:55:23.000000 pypimaker-1.0.0/LICENSE
--rw-r--r--   0 holly      (501) staff       (20)     4331 2023-08-06 01:59:20.706874 pypimaker-1.0.0/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)     3567 2023-08-06 01:58:09.000000 pypimaker-1.0.0/README.md
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.702223 pypimaker-1.0.0/pypimaker.egg-info/
--rw-r--r--   0 holly      (501) staff       (20)     4331 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/PKG-INFO
--rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/SOURCES.txt
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/dependency_links.txt
--rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/entry_points.txt
--rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 01:59:20.000000 pypimaker-1.0.0/pypimaker.egg-info/top_level.txt
--rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 01:59:20.707170 pypimaker-1.0.0/setup.cfg
--rw-r--r--   0 holly      (501) staff       (20)     1347 2023-08-06 01:59:20.000000 pypimaker-1.0.0/setup.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.703405 pypimaker-1.0.0/src/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/src/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.0/src/__main__.py
--rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.0/src/files.py
--rw-r--r--   0 holly      (501) staff       (20)      923 2023-08-06 01:54:56.000000 pypimaker-1.0.0/src/reset.py
--rw-r--r--   0 holly      (501) staff       (20)     7289 2023-08-06 01:54:58.000000 pypimaker-1.0.0/src/strings.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.704773 pypimaker-1.0.0/src/ui/
--rw-r--r--   0 holly      (501) staff       (20)     7744 2023-08-06 01:54:40.000000 pypimaker-1.0.0/src/ui/AuthorInfoSelector.py
--rw-r--r--   0 holly      (501) staff       (20)     3887 2023-08-06 01:53:50.000000 pypimaker-1.0.0/src/ui/DialogWindow.py
--rw-r--r--   0 holly      (501) staff       (20)     8188 2023-08-06 01:54:48.000000 pypimaker-1.0.0/src/ui/OptionSelector.py
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.0/src/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.0/src/ui/navigation.py
--rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 01:54:59.000000 pypimaker-1.0.0/src/upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.705480 pypimaker-1.0.0/tests/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/tests/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.0/tests/test_files.py
--rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.0/tests/test_upload.py
-drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 01:59:20.706240 pypimaker-1.0.0/tests/ui/
--rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.0/tests/ui/__init__.py
--rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.0/tests/ui/test_navigation.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455730 pypimaker-1.0.1/
+-rw-r--r--   0 holly      (501) staff       (20)     1068 2023-08-06 02:11:19.000000 pypimaker-1.0.1/LICENSE
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:11:25.455575 pypimaker-1.0.1/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)     3589 2023-08-06 02:10:11.000000 pypimaker-1.0.1/README.md
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.452862 pypimaker-1.0.1/pypimaker.egg-info/
+-rw-r--r--   0 holly      (501) staff       (20)     4353 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/PKG-INFO
+-rw-r--r--   0 holly      (501) staff       (20)      506 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/SOURCES.txt
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/dependency_links.txt
+-rw-r--r--   0 holly      (501) staff       (20)       48 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/entry_points.txt
+-rw-r--r--   0 holly      (501) staff       (20)       10 2023-08-06 02:11:25.000000 pypimaker-1.0.1/pypimaker.egg-info/top_level.txt
+-rw-r--r--   0 holly      (501) staff       (20)       38 2023-08-06 02:11:25.455792 pypimaker-1.0.1/setup.cfg
+-rw-r--r--   0 holly      (501) staff       (20)     1343 2023-08-06 02:11:25.000000 pypimaker-1.0.1/setup.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.453858 pypimaker-1.0.1/src/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/src/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1340 2023-08-06 01:54:50.000000 pypimaker-1.0.1/src/__main__.py
+-rw-r--r--   0 holly      (501) staff       (20)     9877 2023-08-06 01:54:52.000000 pypimaker-1.0.1/src/files.py
+-rw-r--r--   0 holly      (501) staff       (20)      862 2023-08-06 02:09:48.000000 pypimaker-1.0.1/src/reset.py
+-rw-r--r--   0 holly      (501) staff       (20)     7723 2023-08-06 02:09:43.000000 pypimaker-1.0.1/src/strings.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.454576 pypimaker-1.0.1/src/ui/
+-rw-r--r--   0 holly      (501) staff       (20)     7472 2023-08-06 02:07:27.000000 pypimaker-1.0.1/src/ui/AuthorInfoSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)     3859 2023-08-06 02:08:23.000000 pypimaker-1.0.1/src/ui/DialogWindow.py
+-rw-r--r--   0 holly      (501) staff       (20)     8246 2023-08-06 02:08:20.000000 pypimaker-1.0.1/src/ui/OptionSelector.py
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-08-06 01:53:53.000000 pypimaker-1.0.1/src/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1695 2023-08-06 01:54:46.000000 pypimaker-1.0.1/src/ui/navigation.py
+-rw-r--r--   0 holly      (501) staff       (20)     7124 2023-08-06 02:09:51.000000 pypimaker-1.0.1/src/upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455034 pypimaker-1.0.1/tests/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/tests/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     2903 2023-08-06 01:55:05.000000 pypimaker-1.0.1/tests/test_files.py
+-rw-r--r--   0 holly      (501) staff       (20)     1435 2023-08-06 01:55:07.000000 pypimaker-1.0.1/tests/test_upload.py
+drwxr-xr-x   0 holly      (501) staff       (20)        0 2023-08-06 02:11:25.455348 pypimaker-1.0.1/tests/ui/
+-rw-r--r--   0 holly      (501) staff       (20)        1 2023-07-28 21:05:45.000000 pypimaker-1.0.1/tests/ui/__init__.py
+-rw-r--r--   0 holly      (501) staff       (20)     1276 2023-08-06 01:55:09.000000 pypimaker-1.0.1/tests/ui/test_navigation.py
```

### Comparing `pypimaker-1.0.0/LICENSE` & `pypimaker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/PKG-INFO` & `pypimaker-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -85,14 +85,16 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
+- 1.0.1
+  - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.0/README.md` & `pypimaker-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
+- 1.0.1
+  - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.0/pypimaker.egg-info/PKG-INFO` & `pypimaker-1.0.1/pypimaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypimaker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Software designed for simplifying PyPI Python package setups
 Home-page: https://github.com/bdavis222/pypimaker
 Author: Brian Davis
 Project-URL: Bug Reports, https://github.com/bdavis222/pypimaker/issues
 Project-URL: Funding, https://www.paypal.com/donate/?business=UA5NL9MJSFMVY
 Project-URL: Source, https://github.com/bdavis222/
 Classifier: Intended Audience :: Developers
@@ -85,14 +85,16 @@
 
 ## Authors
 
 Brian Davis
 
 ## Release History
 
+- 1.0.1
+  - Bug fixes
 - 1.0.0
   - Initial Release
 
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](https://github.com/bdavis222/pypimaker/blob/main/LICENSE) file for details.
```

### Comparing `pypimaker-1.0.0/setup.py` & `pypimaker-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='pypimaker',  # Required
-    version='1.0.0', # Required 
+    version='1.0.1', # Required 
     description='Software designed for simplifying PyPI Python package setups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/bdavis222/pypimaker',
     author='Brian Davis',
         classifiers=[  # Defined at https://pypi.org/classifiers/
             'Intended Audience :: Developers',
@@ -24,14 +24,14 @@
     packages=find_packages(),  # Required
     py_modules=['src', 'src.ui', 'tests'],  # Generated
     python_requires='>=3.7, <4',
     project_urls={
         'Bug Reports': 'https://github.com/bdavis222/pypimaker/issues',
         'Funding': 'https://www.paypal.com/donate/?business=UA5NL9MJSFMVY',
         'Source': 'https://github.com/bdavis222/',
-            },
+    },
     entry_points={
         'console_scripts': [
             'pypimaker = src.__main__:main'
         ]
-    }
+        }
 )
```

### Comparing `pypimaker-1.0.0/src/__main__.py` & `pypimaker-1.0.1/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/src/files.py` & `pypimaker-1.0.1/src/files.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/src/reset.py` & `pypimaker-1.0.1/src/reset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import subprocess
 
+from src import strings
 from src.ui.DialogWindow import ActionDialogWindow
 
-RESET_SELECTION_TEXT = "This will remove generated files.\nAre you sure you want to reset?"
-
 
 def reset(topLevelDirectory):
-    ActionDialogWindow("Are you sure?", RESET_SELECTION_TEXT,
+    ActionDialogWindow("Are you sure?", strings.RESET_SELECTION_TEXT,
                        negativeAction=exit, mainWindow=True)
 
     filesToRemove = ["LICENSE", "README.md",
                      "requirements.txt", "setup.py", ".gitignore"]
     foldersToRemove = ["build", "dist"]
     for item in os.listdir(topLevelDirectory):
         if item.endswith("egg-info"):
```

### Comparing `pypimaker-1.0.0/src/strings.py` & `pypimaker-1.0.1/src/strings.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 The possible commands (or their aliases) are the following:
 
    generate  (-g)
    upload    (-u)
    reset     (-r)
    help      (-h)
 
-See the documentation on GitHub or PyPI for more information.
+See the documentation on GitHub (github.com/bdavis222/pypimaker) for more information.
 """
 
 DEFAULT_INITIAL_VERSION = "0.1.0"
 
 PROJECT_DESCRIPTION_TEXT = 'One-sentence Project Description (e.g., "Software designed for..."):'
 SELECT_FOLDER_TEXT = "Select the top-level folder containing your Python project"
 PROJECT_NAME_DESCRIPTION_TEXT = '(Your package will be installed with the "pip install \
@@ -33,14 +33,21 @@
 PROJECT_FOLDER_NOT_CHOSEN_TEXT = "You must select your project \nusing the Browse button."
 PROJECT_NAME_NOT_CHOSEN_TEXT = "Project Name is a required field.\nUse folder name as project name?"
 
 NO_MAIN_FUNCTION_TITLE = "Main function not found"
 MUST_SELECT_MAIN_FILE = 'No "main" function found.\nChoose a file containing\nthe main entry point function?'
 NO_MAIN_FOUND_AFTER_SELECTION_TEXT = 'The selected file does not contain\na function named "main" for your project.'
 
+MISSING_AUTHOR_NAMES_TEXT = "Some emails have missing author names.\nPlease fix and resubmit."
+MISSING_FIRST_NAME_TEXT = "Corresponding author name not given.\nSubmit with no authors?"
+MISSING_FIRST_AUTHOR_EMAIL_TEXT = "Email given for other(s), but not first author.\n\
+Use next email in list for correspondence?"
+
+RESET_SELECTION_TEXT = "This will remove generated files.\nAre you sure you want to reset?"
+
 UNIT_TEST_CREATION_PROMPT_TEXT = '''Create template unit test files?
 These will be placed in a "tests" folder
 within your main project folder.'''
 
 TEST_FILE_CONTENTS = '''import unittest
 {importString}
```

### Comparing `pypimaker-1.0.0/src/ui/AuthorInfoSelector.py` & `pypimaker-1.0.1/src/ui/AuthorInfoSelector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import tkinter as tk
 
+from src import strings
 from src.ui.DialogWindow import ActionDialogWindow, InfoDialogWindow
 
-MISSING_AUTHOR_NAMES_TEXT = "Some emails have missing author names.\nPlease fix and resubmit."
-MISSING_FIRST_NAME_TEXT = "Corresponding author name not given.\nSubmit with no authors?"
-MISSING_FIRST_AUTHOR_EMAIL_TEXT = "Email given for other(s), but not first author.\n\
-Use next email in list for correspondence?"
-
 
 class AuthorInfoSelector:
     def __init__(self):
         self.window = tk.Tk()
         self.window.title("PyPI Maker")
         centerX = (self.window.winfo_screenwidth() - 650) // 2
         centerY = (self.window.winfo_screenheight() - 310) // 2
@@ -134,29 +130,29 @@
 
         noEmailsEntered = True
         for name, email in zip(names, emails):
             if email != "":
                 noEmailsEntered = False
                 if name == "":
                     InfoDialogWindow(
-                        "Invalid entry", MISSING_AUTHOR_NAMES_TEXT)
+                        "Invalid entry", strings.MISSING_AUTHOR_NAMES_TEXT)
                     return
 
         if names[0] == "":
-            ActionDialogWindow("Invalid entry", MISSING_FIRST_NAME_TEXT,
+            ActionDialogWindow("Invalid entry", strings.MISSING_FIRST_NAME_TEXT,
                                positiveAction=self.doneWithNoAuthors)
             return
 
         if emails[0] == "" and not noEmailsEntered:
             ActionDialogWindow(
-                "Invalid entry", MISSING_FIRST_AUTHOR_EMAIL_TEXT)
+                "Invalid entry", strings.MISSING_FIRST_AUTHOR_EMAIL_TEXT)
 
         self.done(names, emails)
 
-    def checkDoneWithReturnKey(self, event):
+    def checkDoneWithReturnKey(self, _):
         self.checkDone()
 
     def done(self, names, emails):
         self.names, self.emails = self.getFilteredNamesAndEmails(names, emails)
         self.correspondingEmail = self.getCorrespondingEmail()
         self.window.destroy()
         self.window.quit()
```

### Comparing `pypimaker-1.0.0/src/ui/DialogWindow.py` & `pypimaker-1.0.1/src/ui/DialogWindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tkinter as tk
 
 
 class DialogWindow:
     def __init__(self, title, message, positiveButtonText, negativeButtonText,
-                 positiveButtonAction=None, negativeButtonAction=None, windowWidth=300, windowHeight=140,
-                 positiveButtonColor="blue", negativeButtonColor="black",
+                 positiveButtonAction=None, negativeButtonAction=None, windowWidth=300,
+                 windowHeight=140, positiveButtonColor="blue", negativeButtonColor="black",
                  mainWindow=False):
         self.window = tk.Tk()
         self.window.title(title)
         centerX = (self.window.winfo_screenwidth() - windowWidth) // 2
         centerY = (self.window.winfo_screenheight() - windowHeight) // 2
         self.window.geometry(
             f"{windowWidth}x{windowHeight}+{centerX}+{centerY}")
@@ -19,26 +19,28 @@
         spacer = tk.Label(self.window, text=" ")
         messageText = tk.Label(self.window, text=message)
         spacer2 = tk.Label(self.window, text=" ")
 
         buttonsFrame = tk.Frame(self.window)
 
         if positiveButtonAction is None:
-            positiveButton = tk.Button(self.window, text=positiveButtonText,
-                                       fg=positiveButtonColor, command=self.closeWindow)
+            positiveButton = tk.Button(
+                self.window, text=positiveButtonText, fg=positiveButtonColor,
+                command=self.closeWindow)
             self.window.bind("<Return>", self.closeWindowWithReturnKey)
         else:
             positiveButton = tk.Button(self.window, text=positiveButtonText,
                                        fg=positiveButtonColor, command=self.performPositiveAction)
             self.window.bind(
                 "<Return>", self.performPositiveActionWithReturnKey)
 
         if negativeButtonAction is None:
-            negativeButton = tk.Button(self.window, text=negativeButtonText,
-                                       fg=negativeButtonColor, command=self.closeWindow)
+            negativeButton = tk.Button(
+                self.window, text=negativeButtonText, fg=negativeButtonColor,
+                command=self.closeWindow)
             self.window.bind("<Escape>", self.closeWindowWithEscapeKey)
         else:
             negativeButton = tk.Button(self.window, text=negativeButtonText,
                                        fg=negativeButtonColor, command=self.performNegativeAction)
             if negativeButtonAction == exit:
                 self.window.bind(
                     "<Escape>", self.performNegativeActionWithEscapeKey)
@@ -56,33 +58,33 @@
 
         self.window.mainloop()
 
     def closeWindow(self):
         self.window.destroy()
         self.window.quit()
 
-    def closeWindowWithEscapeKey(self, event):
+    def closeWindowWithEscapeKey(self, _):
         self.closeWindow()
 
-    def closeWindowWithReturnKey(self, event):
+    def closeWindowWithReturnKey(self, _):
         self.closeWindow()
 
     def performPositiveAction(self):
         self.closeWindow()
         self.positiveButtonAction()
 
-    def performPositiveActionWithReturnKey(self, event):
+    def performPositiveActionWithReturnKey(self, _):
         self.closeWindow()
         self.positiveButtonAction()
 
     def performNegativeAction(self):
         self.closeWindow()
         self.negativeButtonAction()
 
-    def performNegativeActionWithEscapeKey(self, event):
+    def performNegativeActionWithEscapeKey(self, _):
         self.closeWindow()
         self.negativeButtonAction()
 
 
 class ActionDialogWindow(DialogWindow):
     def __init__(self, title, message, positiveAction=None, negativeAction=None,
                  negativeColor="red", mainWindow=False):
```

### Comparing `pypimaker-1.0.0/src/ui/OptionSelector.py` & `pypimaker-1.0.1/src/ui/OptionSelector.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from tkinter import filedialog
 
 from src import strings
 import src.ui.navigation as navigation
 from src.ui.AuthorInfoSelector import AuthorInfoSelector
 from src.ui.DialogWindow import ActionDialogWindow, DialogWindow, InfoDialogWindow
 
+EMPTY_DIRECTORY_SET = set(["", " ", "/"])
+
 
 class OptionSelector:
     def __init__(self):
         self.window = tk.Tk()
         self.window.title("PyPI Maker")
         centerX = (self.window.winfo_screenwidth() - 650) // 2
         centerY = (self.window.winfo_screenheight() - 250) // 2
@@ -93,29 +95,29 @@
         self.window.mainloop()
 
     def browseFolders(self):
         chosenFolder = filedialog.askdirectory(
             initialdir=self.filepath,
             title=strings.SELECT_FOLDER_TEXT
         )
-        if chosenFolder not in ["", " ", "/"]:
+        if chosenFolder not in EMPTY_DIRECTORY_SET:
             if not navigation.hasPyFiles(chosenFolder):
                 InfoDialogWindow(
                     "No Python files found",
                     strings.NO_PYTHON_FILES_IN_PROJECT_FOLDER_TEXT
                 )
                 return
             self.filepath = chosenFolder
         else:
             self.filepath = ""
         self.showFilepath()
         self.window.focus_force()
 
     def checkDone(self):
-        if self.filepath in ["", " ", "/"]:
+        if self.filepath in EMPTY_DIRECTORY_SET:
             InfoDialogWindow(
                 "Missing info", strings.PROJECT_FOLDER_NOT_CHOSEN_TEXT)
             return
 
         if not navigation.hasMainFunctionInSrc(self.filepath):
             DialogWindow(
                 strings.NO_MAIN_FUNCTION_TITLE,
@@ -199,15 +201,15 @@
         self.closeWindow()
         authorInfoSelector = AuthorInfoSelector()
         self.authorsArray = authorInfoSelector.names
         self.emailsArray = authorInfoSelector.emails
         self.correspondingEmail = authorInfoSelector.correspondingEmail
 
     def showFilepath(self):
-        if self.filepath in ["", " ", "/"]:
+        if self.filepath in EMPTY_DIRECTORY_SET:
             self.labelSelectedPath.configure(
                 text=strings.SELECT_FOLDER_TEXT, fg="red", bg="white")
         else:
             displayedFilepath = self.filepath
             if len(displayedFilepath) > 50:
                 displayedFilepath = "..." + displayedFilepath[-50:]
             self.labelSelectedPath.configure(
```

### Comparing `pypimaker-1.0.0/src/ui/navigation.py` & `pypimaker-1.0.1/src/ui/navigation.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/src/upload.py` & `pypimaker-1.0.1/src/upload.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/tests/test_files.py` & `pypimaker-1.0.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/tests/test_upload.py` & `pypimaker-1.0.1/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `pypimaker-1.0.0/tests/ui/test_navigation.py` & `pypimaker-1.0.1/tests/ui/test_navigation.py`

 * *Files identical despite different names*

