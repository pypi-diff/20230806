# Comparing `tmp/pynterface-0.2.1.tar.gz` & `tmp/pynterface-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynterface-0.2.1.tar", last modified: Wed Jun 21 16:29:05 2023, max compression
+gzip compressed data, was "pynterface-0.2.2.tar", last modified: Sun Aug  6 03:47:14 2023, max compression
```

## Comparing `pynterface-0.2.1.tar` & `pynterface-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.627263 pynterface-0.2.1/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-05-04 02:59:32.000000 pynterface-0.2.1/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)       33 2023-05-14 03:48:17.000000 pynterface-0.2.1/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-06-21 16:29:05.627021 pynterface-0.2.1/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1156 2023-05-14 04:10:04.000000 pynterface-0.2.1/README.md
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.625453 pynterface-0.2.1/pynterface/
--rw-r--r--   0 vivaan     (501) staff       (20)      239 2023-06-21 16:28:17.000000 pynterface-0.2.1/pynterface/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3410 2023-06-21 16:26:51.000000 pynterface-0.2.1/pynterface/input.py
--rw-r--r--   0 vivaan     (501) staff       (20)     6438 2023-05-17 14:21:57.000000 pynterface-0.2.1/pynterface/loading.py
--rw-r--r--   0 vivaan     (501) staff       (20)     3367 2023-05-15 15:05:04.000000 pynterface-0.2.1/pynterface/menu.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5444 2023-05-14 18:25:39.000000 pynterface-0.2.1/pynterface/printing.py
--rw-r--r--   0 vivaan     (501) staff       (20)     5848 2023-05-15 14:51:42.000000 pynterface-0.2.1/pynterface/style.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-06-21 16:29:05.626601 pynterface-0.2.1/pynterface.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1484 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      301 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       11 2023-06-21 16:29:05.000000 pynterface-0.2.1/pynterface.egg-info/top_level.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-06-21 16:29:05.627348 pynterface-0.2.1/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      612 2023-05-14 04:04:56.000000 pynterface-0.2.1/setup.py
+drwxr-xr-x   0 vs         (501) staff       (20)        0 2023-08-06 03:47:14.880533 pynterface-0.2.2/
+-rw-r--r--   0 vs         (501) staff       (20)     1071 2023-08-06 03:16:38.000000 pynterface-0.2.2/LICENSE
+-rw-r--r--   0 vs         (501) staff       (20)       33 2023-08-06 03:16:38.000000 pynterface-0.2.2/MANIFEST.in
+-rw-r--r--   0 vs         (501) staff       (20)     1542 2023-08-06 03:47:14.880220 pynterface-0.2.2/PKG-INFO
+-rw-r--r--   0 vs         (501) staff       (20)     1175 2023-08-06 03:16:38.000000 pynterface-0.2.2/README.md
+drwxr-xr-x   0 vs         (501) staff       (20)        0 2023-08-06 03:47:14.877803 pynterface-0.2.2/pynterface/
+-rw-r--r--   0 vs         (501) staff       (20)      502 2023-08-06 03:45:59.000000 pynterface-0.2.2/pynterface/__init__.py
+-rw-r--r--   0 vs         (501) staff       (20)     3410 2023-08-06 03:16:38.000000 pynterface-0.2.2/pynterface/input.py
+-rw-r--r--   0 vs         (501) staff       (20)     6438 2023-08-06 03:16:38.000000 pynterface-0.2.2/pynterface/loading.py
+-rw-r--r--   0 vs         (501) staff       (20)     3367 2023-08-06 03:16:38.000000 pynterface-0.2.2/pynterface/menu.py
+-rw-r--r--   0 vs         (501) staff       (20)     5561 2023-08-06 03:26:05.000000 pynterface-0.2.2/pynterface/printing.py
+-rw-r--r--   0 vs         (501) staff       (20)     5848 2023-08-06 03:16:38.000000 pynterface-0.2.2/pynterface/style.py
+drwxr-xr-x   0 vs         (501) staff       (20)        0 2023-08-06 03:47:14.879605 pynterface-0.2.2/pynterface.egg-info/
+-rw-r--r--   0 vs         (501) staff       (20)     1542 2023-08-06 03:47:14.000000 pynterface-0.2.2/pynterface.egg-info/PKG-INFO
+-rw-r--r--   0 vs         (501) staff       (20)      301 2023-08-06 03:47:14.000000 pynterface-0.2.2/pynterface.egg-info/SOURCES.txt
+-rw-r--r--   0 vs         (501) staff       (20)        1 2023-08-06 03:47:14.000000 pynterface-0.2.2/pynterface.egg-info/dependency_links.txt
+-rw-r--r--   0 vs         (501) staff       (20)       11 2023-08-06 03:47:14.000000 pynterface-0.2.2/pynterface.egg-info/top_level.txt
+-rw-r--r--   0 vs         (501) staff       (20)       38 2023-08-06 03:47:14.880653 pynterface-0.2.2/setup.cfg
+-rw-r--r--   0 vs         (501) staff       (20)      612 2023-08-06 03:16:38.000000 pynterface-0.2.2/setup.py
```

### Comparing `pynterface-0.2.1/LICENSE` & `pynterface-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.1/PKG-INFO` & `pynterface-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.2.1
+Version: 0.2.2
 Summary: Terminal-Based Printing Tools!
+Home-page: UNKNOWN
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynterface
 
 [![PyPi Version](https://badgen.net/pypi/v/pynterface/)](https://pypi.org/project/pynterface)
 [![Documentation Status](https://readthedocs.org/projects/pynterface/badge/?version=latest)](https://pynterface.readthedocs.io/en/latest/?badge=latest)
 
 A module to deal with terminal-based input and output! This package is available on PyPI [here](https://pypi.org/project/pynterface/).
 
 ## Why Use This?
-This package has many features that helps make coding user inputs easier and terminal outputs more pretty. You can do many things with either regard, with one line!
+This package has many features that help make implementing user inputs easier and terminal outputs much cleaner. You can do many things with either regard, usually with a single line!
 
 ## Installation 
 To install, simply run the following:
 ```
 $ pip install pynterface
 ```
 
@@ -35,7 +37,9 @@
 Full documentation can be found on the [readthedocs](https://pynterface.readthedocs.io/en/latest/index.html) site for the module.
 
 ## Contribution
 For adding features, pull requests are greatly appreciated. If you have an idea, please open an issue! Feel free to message me on my email singhvi.vivaan@gmail.com if you have any concerns!
 
 ## License
 This project is released under the MIT license.
+
+
```

### Comparing `pynterface-0.2.1/README.md` & `pynterface-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPi Version](https://badgen.net/pypi/v/pynterface/)](https://pypi.org/project/pynterface)
 [![Documentation Status](https://readthedocs.org/projects/pynterface/badge/?version=latest)](https://pynterface.readthedocs.io/en/latest/?badge=latest)
 
 A module to deal with terminal-based input and output! This package is available on PyPI [here](https://pypi.org/project/pynterface/).
 
 ## Why Use This?
-This package has many features that helps make coding user inputs easier and terminal outputs more pretty. You can do many things with either regard, with one line!
+This package has many features that help make implementing user inputs easier and terminal outputs much cleaner. You can do many things with either regard, usually with a single line!
 
 ## Installation 
 To install, simply run the following:
 ```
 $ pip install pynterface
 ```
```

### Comparing `pynterface-0.2.1/pynterface/input.py` & `pynterface-0.2.2/pynterface/input.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.1/pynterface/loading.py` & `pynterface-0.2.2/pynterface/loading.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.1/pynterface/menu.py` & `pynterface-0.2.2/pynterface/menu.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.1/pynterface/printing.py` & `pynterface-0.2.2/pynterface/printing.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - 'Smooth' print a message
 - Center text
 - Apply a gradient to text or background
 """
 
 import os
 import re
-from typing import Any, Iterable
+from typing import Any, Iterable, Union
 from time import sleep
 from .style import Color, Background 
 
 # \033[ followed by a combo of numbers and ; ended with a single letter
 __ANSI_PATTERN = "\033\[[0-9|;]*[a-z|A-Z]"
 __CENTERED_FORBIDDEN_CHARS = "[\t]"
 __UNIQUE_CHAR_LENGTHS = {
@@ -51,15 +51,15 @@
         if re.search(__ANSI_PATTERN, message) == None:    # delay only if ansi
             sleep(delay/1000)       
         print(char, end="")
         
     # prints the end (optional)
     print(end, end="")
 
-def centered(message: str | Iterable[str], margin: int = 2) -> str:
+def centered(message: Union[str, Iterable[str]], margin: int = 2) -> str:
     """
     Centers several lines of text.
     """
     
     assert isinstance(message, (str, Iterable)), "Messages must be iterable."
     assert isinstance(margin, int), "Margin must be an integer."
 
@@ -147,15 +147,19 @@
     if mode == "text": method = Color
     elif mode == "background": method = Background
     
     # splits depending on the types
     if isinstance(message, str): messages = message.split("\n")
     else: messages = [*message]
 
+    # get the method rest
+    reset_code = method.RESET_COLOR if method == Color else method.RESET_BACKGROUND
+
+    # perform gradient calculations
     messages = [__split_esc_chars(line) for line in messages]
     max_len = max([len(s) for s in messages]) - 1
     rgb_vals = [tuple([get_value(left_rgb[ii], right_rgb[ii], i, max_len) for ii in range(3)]) for i in range(max_len+1)]
-    output = f"{method.RESET_COLOR if method == Color else method.RESET_BACKGROUND}\n".join(            # joins the lines by a reset color/background
+    output = f"{reset_code}\n".join(            # joins the lines by a reset color/background
         ["".join([method.RGB(rgb_vals[i]) + line[i] for i in range(len(line))]) for line in messages]   # creates the line
     )
 
-    return output
+    return output + reset_code
```

### Comparing `pynterface-0.2.1/pynterface/style.py` & `pynterface-0.2.2/pynterface/style.py`

 * *Files identical despite different names*

### Comparing `pynterface-0.2.1/pynterface.egg-info/PKG-INFO` & `pynterface-0.2.2/pynterface.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pynterface
-Version: 0.2.1
+Version: 0.2.2
 Summary: Terminal-Based Printing Tools!
+Home-page: UNKNOWN
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pynterface.readthedocs.io/en/latest/
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pynterface
 
 [![PyPi Version](https://badgen.net/pypi/v/pynterface/)](https://pypi.org/project/pynterface)
 [![Documentation Status](https://readthedocs.org/projects/pynterface/badge/?version=latest)](https://pynterface.readthedocs.io/en/latest/?badge=latest)
 
 A module to deal with terminal-based input and output! This package is available on PyPI [here](https://pypi.org/project/pynterface/).
 
 ## Why Use This?
-This package has many features that helps make coding user inputs easier and terminal outputs more pretty. You can do many things with either regard, with one line!
+This package has many features that help make implementing user inputs easier and terminal outputs much cleaner. You can do many things with either regard, usually with a single line!
 
 ## Installation 
 To install, simply run the following:
 ```
 $ pip install pynterface
 ```
 
@@ -35,7 +37,9 @@
 Full documentation can be found on the [readthedocs](https://pynterface.readthedocs.io/en/latest/index.html) site for the module.
 
 ## Contribution
 For adding features, pull requests are greatly appreciated. If you have an idea, please open an issue! Feel free to message me on my email singhvi.vivaan@gmail.com if you have any concerns!
 
 ## License
 This project is released under the MIT license.
+
+
```

### Comparing `pynterface-0.2.1/setup.py` & `pynterface-0.2.2/setup.py`

 * *Files identical despite different names*

