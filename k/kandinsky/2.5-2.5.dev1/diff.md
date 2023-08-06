# Comparing `tmp/kandinsky-2.5.tar.gz` & `tmp/kandinsky-2.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kandinsky-2.5.tar", last modified: Sun Aug  6 12:04:55 2023, max compression
+gzip compressed data, was "kandinsky-2.5.dev1.tar", last modified: Fri May 12 14:10:09 2023, max compression
```

## Comparing `kandinsky-2.5.tar` & `kandinsky-2.5.dev1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:55.008712 kandinsky-2.5/
--rw-rw-rw-   0        0        0     3050 2023-08-06 12:04:30.000000 kandinsky-2.5/FAQ.md
--rw-rw-rw-   0        0        0      681 2023-08-06 12:04:55.007712 kandinsky-2.5/PKG-INFO
--rw-rw-rw-   0        0        0     6626 2023-08-06 12:04:30.000000 kandinsky-2.5/README.md
--rw-rw-rw-   0        0        0     1835 2023-08-05 16:58:11.000000 kandinsky-2.5/changelog.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 12:04:55.010716 kandinsky-2.5/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-08-06 12:04:30.000000 kandinsky-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:54.858103 kandinsky-2.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:54.901103 kandinsky-2.5/src/kandinsky/
--rw-rw-rw-   0        0        0     3050 2023-07-28 10:06:45.000000 kandinsky-2.5/src/kandinsky/FAQ.md
--rw-rw-rw-   0        0        0     6626 2023-07-30 11:05:17.000000 kandinsky-2.5/src/kandinsky/README.md
--rw-rw-rw-   0        0        0     5122 2023-08-06 12:04:30.000000 kandinsky-2.5/src/kandinsky/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-08-02 16:29:20.000000 kandinsky-2.5/src/kandinsky/__init__.pyi
--rw-rw-rw-   0        0        0      243 2023-08-04 11:47:50.000000 kandinsky-2.5/src/kandinsky/__main__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:54.941253 kandinsky-2.5/src/kandinsky/util/
--rw-rw-rw-   0        0        0     2993 2023-08-06 11:46:08.000000 kandinsky-2.5/src/kandinsky/util/3d_demo.py
--rw-rw-rw-   0        0        0    12956 2023-08-02 20:42:03.000000 kandinsky-2.5/src/kandinsky/util/core.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:54.975493 kandinsky-2.5/src/kandinsky/util/data/
--rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.5/src/kandinsky/util/data/app.ico
--rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.5/src/kandinsky/util/data/app.png
--rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.5/src/kandinsky/util/data/battery0.png
--rw-rw-rw-   0        0        0      159 2023-04-04 18:53:23.000000 kandinsky-2.5/src/kandinsky/util/data/battery1.png
--rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.5/src/kandinsky/util/data/large_font.ttf
--rw-rw-rw-   0        0        0     5805 2023-03-27 21:29:01.000000 kandinsky-2.5/src/kandinsky/util/data/old_icons.zip
--rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.5/src/kandinsky/util/data/small_font.ttf
--rw-rw-rw-   0        0        0     4305 2023-06-24 18:00:59.000000 kandinsky-2.5/src/kandinsky/util/demo.py
--rw-rw-rw-   0        0        0     3201 2023-08-01 18:20:49.000000 kandinsky-2.5/src/kandinsky/util/mac_patcher.py
--rw-rw-rw-   0        0        0     3470 2022-08-20 21:28:54.000000 kandinsky-2.5/src/kandinsky/util/old_config.ini
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:55.005713 kandinsky-2.5/src/kandinsky/util/stuff/
--rw-rw-rw-   0        0        0      128 2023-05-03 14:32:56.000000 kandinsky-2.5/src/kandinsky/util/stuff/__init__.py
--rw-rw-rw-   0        0        0     2528 2023-07-17 20:18:57.000000 kandinsky-2.5/src/kandinsky/util/stuff/color.py
--rw-rw-rw-   0        0        0     1544 2023-08-02 20:54:44.000000 kandinsky-2.5/src/kandinsky/util/stuff/draw.py
--rw-rw-rw-   0        0        0    14205 2023-08-06 11:54:46.000000 kandinsky-2.5/src/kandinsky/util/stuff/gui.py
--rw-rw-rw-   0        0        0     6006 2023-08-02 19:57:06.000000 kandinsky-2.5/src/kandinsky/util/stuff/limiter.py
--rw-rw-rw-   0        0        0     1377 2023-07-16 14:36:13.000000 kandinsky-2.5/src/kandinsky/util/stuff/tests.py
--rw-rw-rw-   0        0        0     2953 2023-07-16 18:23:54.000000 kandinsky-2.5/src/kandinsky/util/stuff/vars.py
-drwxrwxrwx   0        0        0        0 2023-08-06 12:04:54.924255 kandinsky-2.5/src/kandinsky.egg-info/
--rw-rw-rw-   0        0        0      681 2023-08-06 12:04:54.000000 kandinsky-2.5/src/kandinsky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      992 2023-08-06 12:04:54.000000 kandinsky-2.5/src/kandinsky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 12:04:54.000000 kandinsky-2.5/src/kandinsky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-06 12:04:54.000000 kandinsky-2.5/src/kandinsky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 12:04:54.000000 kandinsky-2.5/src/kandinsky.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.398222 kandinsky-2.5.dev1/
+-rw-rw-rw-   0        0        0     1590 2022-08-29 17:59:39.000000 kandinsky-2.5.dev1/FAQ.md
+-rw-rw-rw-   0        0        0      636 2023-05-12 14:10:09.394226 kandinsky-2.5.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     6299 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/README.md
+-rw-rw-rw-   0        0        0      781 2023-05-09 20:21:54.000000 kandinsky-2.5.dev1/changelog.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 14:10:09.398222 kandinsky-2.5.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:08.890222 kandinsky-2.5.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.018221 kandinsky-2.5.dev1/src/kandinsky/
+-rw-rw-rw-   0        0        0     1580 2023-03-28 18:10:13.000000 kandinsky-2.5.dev1/src/kandinsky/FAQ.md
+-rw-rw-rw-   0        0        0     6299 2023-05-03 19:43:17.000000 kandinsky-2.5.dev1/src/kandinsky/README.md
+-rw-rw-rw-   0        0        0     4776 2023-05-12 14:09:36.000000 kandinsky-2.5.dev1/src/kandinsky/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-03-27 18:31:44.000000 kandinsky-2.5.dev1/src/kandinsky/__init__.pyi
+-rw-rw-rw-   0        0        0      244 2023-03-29 16:11:12.000000 kandinsky-2.5.dev1/src/kandinsky/__main__.py
+-rw-rw-rw-   0        0        0    10122 2023-05-11 21:04:09.000000 kandinsky-2.5.dev1/src/kandinsky/test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.150221 kandinsky-2.5.dev1/src/kandinsky/util/
+-rw-rw-rw-   0        0        0    12414 2023-05-11 21:08:44.000000 kandinsky-2.5.dev1/src/kandinsky/util/core.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.254223 kandinsky-2.5.dev1/src/kandinsky/util/data/
+-rw-rw-rw-   0        0        0     4286 2022-11-03 16:32:20.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/app.ico
+-rw-rw-rw-   0        0        0     1544 2023-03-08 20:36:09.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/app.png
+-rw-rw-rw-   0        0        0      146 2023-03-28 16:47:34.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/battery0.png
+-rw-rw-rw-   0        0        0      159 2023-04-04 18:53:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/battery1.png
+-rw-rw-rw-   0        0        0   226352 2022-08-25 19:34:57.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/large_font.ttf
+-rw-rw-rw-   0        0        0     5805 2023-03-27 21:29:01.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/old_icons.zip
+-rw-rw-rw-   0        0        0   220448 2023-03-27 20:37:08.000000 kandinsky-2.5.dev1/src/kandinsky/util/data/small_font.ttf
+-rw-rw-rw-   0        0        0     4308 2023-03-14 17:37:19.000000 kandinsky-2.5.dev1/src/kandinsky/util/demo.py
+-rw-rw-rw-   0        0        0     3470 2022-08-20 21:28:54.000000 kandinsky-2.5.dev1/src/kandinsky/util/old_config.ini
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.390222 kandinsky-2.5.dev1/src/kandinsky/util/stuff/
+-rw-rw-rw-   0        0        0      128 2023-05-03 14:32:56.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/__init__.py
+-rw-rw-rw-   0        0        0     2310 2023-04-28 14:04:16.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/color.py
+-rw-rw-rw-   0        0        0     1506 2023-05-10 19:04:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/draw.py
+-rw-rw-rw-   0        0        0    13161 2023-05-11 18:13:37.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/gui.py
+-rw-rw-rw-   0        0        0     5426 2023-03-27 17:46:33.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/ion.py
+-rw-rw-rw-   0        0        0     5214 2023-05-03 19:28:19.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/limiter.py
+-rw-rw-rw-   0        0        0      909 2023-03-30 11:58:23.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/tests.py
+-rw-rw-rw-   0        0        0     3472 2023-05-10 18:06:53.000000 kandinsky-2.5.dev1/src/kandinsky/util/stuff/vars.py
+drwxrwxrwx   0        0        0        0 2023-05-12 14:10:09.070222 kandinsky-2.5.dev1/src/kandinsky.egg-info/
+-rw-rw-rw-   0        0        0      636 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 14:10:08.000000 kandinsky-2.5.dev1/src/kandinsky.egg-info/top_level.txt
```

### Comparing `kandinsky-2.5/PKG-INFO` & `kandinsky-2.5.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: kandinsky
-Version: 2.5
+Version: 2.5.dev1
 Summary: A small module allowing to link the kandinsky module, from the Numworks, to a window.
 Home-page: https://github.com/ZetaMap/Kandinsky-Numworks
 Author: ZetaMap
 License: MIT
 Project-URL: GitHub Project, https://github.com/ZetaMap/Kandinsky-Numworks
 Project-URL: My GitHub Page, https://github.com/ZetaMap/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kandinsky-2.5/README.md` & `kandinsky-2.5.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,14 @@
 #### ***New method for this library, only on Computer***
 
 **quit():**
 * Parameters: **No parameters**
 * Description: Close manualy the window without notifying the user
 * Note: after that you cannot reopen the window, so a re-import of kandinsky will be required to get a new window
 
-**display():**
-* Parameters: **No parameters**
-* Description: Refresh manually the window and display changes
-* Note: **⚠️Method added only for MacOS, because library cannot refresh automatically the window in another Thread. <br>
-It will be necessary to call this method from time to time to keep it alive.⚠️**
-
 #### ***New methods added by Omega (previous methods are also added)***
 
 **draw_line()**
 * Parameters: ``x1``, ``y1``, ``x2``, ``y2``, ``color``
 * Description: Draw a line at (x1, y1) to (x2, y2)
 
 **wait_vblank()**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kandinsky-2.5/setup.py` & `kandinsky-2.5.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 # AUTO GENERATED FILE. DO NOT EDIT!
-from setuptools import setup
-setup(**{'name': 'kandinsky', 'version': '2.5', 'author': 'ZetaMap', 'description': 'A small module allowing to link the kandinsky module, from the Numworks, to a window.', 'license': 'MIT', 'long_description': '', 'long_description_content_type': 'text/markdown', 'url': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'project_urls': {'GitHub Project': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'My GitHub Page': 'https://github.com/ZetaMap/'}, 'classifiers': ['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License', 'Operating System :: Microsoft :: Windows', 'Operating System :: Unix', 'Operating System :: MacOS :: MacOS X'], 'package_dir': {'': 'src'}, 'include_dirs': ['kandinsky'], 'install_requires': ['pysdl2', 'pysdl2-dll'], 'include_package_data': True, 'python_requires': '>=3.6'})
+from setuptools import setup 
+setup(**{'name': 'kandinsky', 'version': '2.5.dev1', 'author': 'ZetaMap', 'description': 'A small module allowing to link the kandinsky module, from the Numworks, to a window.', 'license': 'MIT', 'long_description': '', 'long_description_content_type': 'text/markdown', 'url': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'project_urls': {'GitHub Project': 'https://github.com/ZetaMap/Kandinsky-Numworks', 'My GitHub Page': 'https://github.com/ZetaMap/'}, 'classifiers': ['Programming Language :: Python :: 3', 'License :: OSI Approved :: MIT License', 'Operating System :: Microsoft :: Windows', 'Operating System :: Unix'], 'package_dir': {'': 'src'}, 'include_dirs': ['kandinsky'], 'install_requires': ['pysdl2', 'pysdl2-dll'], 'include_package_data': True, 'python_requires': '>=3.6'})
```

### Comparing `kandinsky-2.5/src/kandinsky/README.md` & `kandinsky-2.5.dev1/src/kandinsky/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,14 @@
 #### ***New method for this library, only on Computer***
 
 **quit():**
 * Parameters: **No parameters**
 * Description: Close manualy the window without notifying the user
 * Note: after that you cannot reopen the window, so a re-import of kandinsky will be required to get a new window
 
-**display():**
-* Parameters: **No parameters**
-* Description: Refresh manually the window and display changes
-* Note: **⚠️Method added only for MacOS, because library cannot refresh automatically the window in another Thread. <br>
-It will be necessary to call this method from time to time to keep it alive.⚠️**
-
 #### ***New methods added by Omega (previous methods are also added)***
 
 **draw_line()**
 * Parameters: ``x1``, ``y1``, ``x2``, ``y2``, ``color``
 * Description: Draw a line at (x1, y1) to (x2, y2)
 
 **wait_vblank()**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kandinsky-2.5/src/kandinsky/__init__.py` & `kandinsky-2.5.dev1/src/kandinsky/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-"""A small module allowing to link the kandinsky module, from the Numworks, to a Windows window.
+"""A small module allowing to link the kandinsky module, from the Numworks, to a Windows window. 
 Useful if you want to test your program without putting it on the calculator.
 The [GitHub project](https://github.com/ZetaMap/Kandinsky-Numworks), and if you have any questions, check out the [FAQ](https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/FAQ.md)
 In addition, this module also emulates the drawing speed, and has [many other features](https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/README.md#additional-features).
 """
 
-import sys # test is macos to patch the module
-try:
-  if sys.platform == 'darwin': from .util.mac_patcher import Core as __Core, display
-  else: from .util.core import Core as __Core
+try: from .util.core import Core as __Core
 except ImportError as e:
-  if "relative import" not in e.msg:
+  if "relative import" not in e.msg: 
     raise
-  if sys.platform == 'darwin': from util.mac_patcher import Core as __Core, display
-  else: from util.core import Core as __Core
+  from util.core import Core as __Core
 
 __name__ = "kandinsky"
-__version__ = "2.5"
-try: 
-  with open("README.md", encoding="utf-8") as f: __doc__ = f.read()
-  del f
+__version__ = "2.5.dev1"
+try: __doc__ = open("README.md").read()
 except (FileNotFoundError, OSError): __doc__ = "<unknown>"
-__all__ = [
-  #numworks
-  "get_pixel",
-  "set_pixel",
-  "color",
+__all__ = [ 
+  #numworks 
+  "get_pixel", 
+  "set_pixel", 
+  "color", 
   "draw_string",
   "fill_rect",
 
   #only for PC
   "quit",
 
   #omega
@@ -40,54 +34,51 @@
 
   #upsilon
   "draw_circle",
   "fill_circle",
   "fill_polygon",
   "get_palette"
 ]
-if sys.platform == 'darwin': __all__.append("display")
 __Core = __Core()
 
-# No more need of this
-del sys
 
 # Numworks basic methods
 def get_pixel(x, y, /):
   """Return pixel (x, y) color"""
   pixel, err = __Core.event_fire(__Core.get_pixel, x, y)
   if err != None:
     raise err
   return pixel
-
+  
 def set_pixel(x, y, color, /):
   """Color pixel (x, y)"""
   _, err = __Core.event_fire(__Core.set_pixel, x, y, color)
   if err != None:
     raise err
 
 def color(r, g=None, b=None, /):
   """Define a rgb color"""
   color, err = __Core.event_fire(__Core.color,r, g, b)
   if err != None:
     raise err
   return color
 
 # Argument added by Omega
-if __Core.OS_MODE != 1:
+if __Core.OS_MODE > 1:
   def draw_string(text, x, y, color=(0,0,0), background=(248,252,248), font=False, /):
     """Display a text from pixel (x, y)"""
     _, err = __Core.event_fire(__Core.draw_string, text, x, y, color, background, font)
     if err != None:
-      raise err
+      raise err  
 else :
   def draw_string(text, x, y, color=(0,0,0), background=(248,252,248), /):
     """Display a text from pixel (x, y)"""
     _, err = __Core.event_fire(__Core.draw_string, text, x, y, color, background)
     if err != None:
-      raise err
+      raise err  
 
 def fill_rect(x, y, width, height, color, /):
   """Fill a rectangle at pixel (x, y)"""
   _, err = __Core.event_fire(__Core.fill_rect, x, y, width, height, color)
   if err != None:
     raise err
 
@@ -148,28 +139,28 @@
     raise err
   return pal
 
 
 ######### Clean #########
 # delete methods according to OS
 # in pc mode, do not delete anything
-if __Core.OS_MODE:
+if __Core.OS_MODE: 
   # upsilon moved this method and epsilon don't have this
   if __Core.OS_MODE != 2:
     __all__.remove("get_keys")
     del get_keys
 
   # delete upsilon methods
-  if __Core.OS_MODE < 3:
+  if __Core.OS_MODE < 3: 
     __all__.remove("draw_circle")
     __all__.remove("fill_circle")
     __all__.remove("fill_polygon")
     __all__.remove("get_palette")
     del draw_circle, fill_circle,  fill_polygon, get_palette
-
+ 
   # delete omega methods
-  if __Core.OS_MODE < 2:
+  if __Core.OS_MODE < 2: 
     __all__.remove("draw_line")
     __all__.remove("wait_vblank")
     __all__.remove("small_font")
     __all__.remove("large_font")
     del draw_line, wait_vblank, small_font, large_font
```

### Comparing `kandinsky-2.5/src/kandinsky/__init__.pyi` & `kandinsky-2.5.dev1/src/kandinsky/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from typing import Tuple, List, Union, Optional, Dict, MutableSet
-import sys
 
-ColorInput = Union[Tuple[int, int, int], List[int, int, int], str, float]
+ColorInput = Union[Tuple[int, int, int], List[int, int, int], str]
 ColorOutput = Tuple[int, int, int]
 
 def get_pixel(x: int, y: int) -> ColorOutput: ...
 def set_pixel(x: int, y: int, color: ColorInput) -> None: ...
 def color(color: ColorInput) -> ColorOutput: ...
 def color(r: int, g: int, b: int) -> ColorOutput: ...
-def draw_string(text: str, x: int, y: int, color: Optional[ColorInput]=(0, 0, 0),
+def draw_string(text: str, x: int, y: int, color: Optional[ColorInput]=(0, 0, 0), 
                 background: Optional[ColorInput]=(248, 252, 248), font: bool=False) -> None: ...
 def fill_rect(x: int, y: int, width: int, height: int, color: ColorInput) -> None: ...
 
-# Special methods, only in pc
+# Special method, only in pc
 def quit() -> None: ...
-if sys.platform == 'darwin': # Method only for macos
-  def display() -> None: ...
 
 # Methods for other os
 def draw_line(x1: int, y1: int, x2: int, y2: int, color: ColorInput) -> None: ...
 def wait_vblank() -> None: ...
 def get_keys() -> MutableSet[str]: ...
 small_font: bool = ...
 large_font: bool = ...
```

### Comparing `kandinsky-2.5/src/kandinsky/util/core.py` & `kandinsky-2.5.dev1/src/kandinsky/util/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,143 +1,132 @@
 ######### Imports #########
-import sys, os
+from os import environ, name
 
 try: from tkinter import Tk
 except ImportError as e:
-  e.msg = "tkinter is not installed. "
-  if sys.platform == "win32": e.msg += "please reinstall python with complements modules"
-  elif sys.platform == "darwin": e.msg += "install it with 'brew install python-tk'"
-  else: e.msg += "install it with 'sudo apt install python3-tk'"
+  e.msg = "tkinter is not installed. "+("please reinstall python with complements modules" if name == "nt" else "install it with 'sudo apt install python3-tk'")
   raise
 
 import warnings
-warnings.filters = [] # Reset filters because some default appear in, and HIS DON'T PRINT MY WARNINGS!!
-warnings.filterwarnings('ignore', category=UserWarning) # Disable SDL warning
+warnings.filterwarnings('ignore', category=UserWarning) # Disable SDL warning 
 try:
   import sdl2dll
   from sdl2.ext import init, quit as sdl_quit, ttf, image
   from sdl2._internal import prettywarn
 
-  # I'm forced to not initialise the video for now,
-  # due to MacOS causing a C++ crash if tkinter is initialized after SDL
-  init(video=False)
+  init()
   ttf._ttf_init()
   image._sdl_image_init()
 
 except (ImportError, RuntimeError) as e:
   e.msg = """PySDL2 or PySDL2-dll module is not installed on your system, and kandinsky depend to it.
 >>> To install, follow steps on the GitHub project: https://github.com/ZetaMap/Kandinsky-Numworks
->>> or type 'pip3 install -U pysdl2 pysdl2-dll"""
+>>> or type 'pip install -U pysdl2 pysdl2-dll"""
   raise
 
 try: import ion
 except ImportError: ION_PRESENT = False
-else:
-  # Another module is called ion, so verify default function to see if it's the right module
-  ION_PRESENT = hasattr(ion, "keydown")
-  if not ION_PRESENT:
-    prettywarn("ion is installed but no basic methods found. "
-               "Are you sure you have installed the correct module? "
-               "His pypi name is 'ion-numworks'.", ImportWarning)
-
+else: 
   # In older version i forgot to define __version__ field
   # so if is not defined, is an outdated version.
   # Or verify if version is good
-  elif not hasattr(ion, "__version__") or tuple([int(i) for i in ion.__version__.split('.') if i.isdecimal()]) < (2, 0):
-    prettywarn("outdated version of 'ion-numworks', please update it", ImportWarning)
+  if not hasattr(ion, "__version__") or tuple([int(i) for i in ion.__version__.split('.') if i.isdecimal()]) < (1, 2, 3):
+    # idk why but warning don't print, so will show it manually
+    print("ImportWarning: outdated version of 'Ion-numworks', please update it")
     ION_PRESENT = False
 
+  # Another module is called ion, so do a little test to see if it's the right module
+  else: ION_PRESENT = hasattr(ion, "keydown") 
+
 from threading import Thread, main_thread
 from math import sqrt
 from .stuff import *
 
 
 ######### Environ config #########
-DEBUG = 'KANDINSKY_ENABLE_DEBUG' in os.environ #or True
+DEBUG = 'KANDINSKY_ENABLE_DEBUG' in environ #or True 
 
-NO_GUI = 'KANDINSKY_NO_GUI' in os.environ
+NO_GUI = 'KANDINSKY_NO_GUI' in environ
 
 # '0': PC, '1': Numworks, '2': Omega, '3': Upsilon
-mode = os.environ.get('KANDINSKY_OS_MODE')
-if mode and mode.isdecimal(): Vars.selected_os = int(mode) if 0 <= int(mode) < len(Config.os_list) else Config.default_os
+os = environ.get('KANDINSKY_OS_MODE')
+if os and os.isdecimal(): Vars.selected_os = int(os) if 0 <= int(os) < len(Config.os_list) else Config.default_os
 
 # '0': n0100, '1': n0110, '2': n0120
-model = os.environ.get('KANDINSKY_MODEL_MODE')
+model = environ.get('KANDINSKY_MODEL_MODE')
 if model and model.isdecimal(): Vars.selected_model = int(model) if 0 <= int(model) < len(Config.model_list) else Config.default_model
 
-if 'KANDINSKY_SCREEN_SIZE' in os.environ:
-  screen = os.environ['KANDINSKY_SCREEN_SIZE'].split('x')
-
-  if len(screen) != 2:
+if 'KANDINSKY_SCREEN_SIZE' in environ:
+  screen = environ['KANDINSKY_SCREEN_SIZE'].split('x')
+  
+  if len(screen) != 2: 
     raise \
       ValueError("invalid screen format. format to use: '<width>x<height>'")
-
+  
   for i in range(2):
-    if not screen[i].isdecimal() or int(screen[i]) < 0:
+    if not screen[i].isdecimal() or int(screen[i]) < 0: 
       raise \
         ValueError("screen dimensions must be positive integers")
     screen[i] = int(screen[i])
-
+    
   screen[1] -= Vars.head_size
   if screen[0] < Vars.screen[0] or screen[1] < Vars.screen[1]:
     raise \
       ValueError(f"screen dimensions must be greater than {Vars.screen[0]}x{Vars.screen[1]+Vars.head_size}")
-
+  
   Vars.screen = tuple(screen)
 
-zoom = os.environ.get('KANDINSKY_ZOOM_RATIO')
+zoom = environ.get('KANDINSKY_ZOOM_RATIO')
 if zoom and zoom.isdecimal() and 1 <= int(zoom) <= Config.zoom_max: Vars.zoom_ratio = int(zoom)
 
 # Experimental way to get more real emulation of numworks
 import threading
-USE_HEAP = 'KANDINSKY_USE_HEAP' in os.environ and hasattr(threading, "get_native_id")
+USE_HEAP = 'KANDINSKY_USE_HEAP' in environ and hasattr(threading, "get_native_id")
 # same problem than warning of ion
-if USE_HEAP: prettywarn("python heap limitator is an experimental feature, so it can crach python several times", ImportWarning)
-
+if USE_HEAP: print("ResourceWarning: python heap limitator is an experimental feature, so it can crach python several times")
 
 ######### Cleanup #########
-del mode, model, zoom, init, sys, os, sdl2dll, ttf, image, warnings, threading, #prettywarn
+del environ, name, os, model, zoom, init, sdl2dll, ttf, image, warnings, threading, #prettywarn
 
 
 ######### Main code #########
 __all__ = ["Core"]
 
-class Core(Thread):
-  stopped = False
+class Core(Thread): 
+  stoped = False
   asknoclose = False
   OS_MODE = Config.default_os
 
   def __init__(self):
     Gui.paused = Gui.already_paused = True # Pause events to give the time of thread to initialize
 
     super().__init__(None, self.event_loop, Vars.app_name.replace(' ', '')+self.__class__.__name__)
     self.start()
     while Gui.paused and self.is_alive(): usleep(100) # Wait a little to synchronize it
 
   def quit_app(self, *_):
-    if not self.stopped:
-      self.stopped = True
+    if not self.stoped:
+      self.stoped = True 
       Gui.paused = False # Now all calls of kandinsky raise an error
 
-      usleep(10**4) # Wait a little to give time to draw methods finished
       Gui.destroy()
       sdl_quit()
 
   def print_debug(self, type, *messages, type_length=5, **args):
-    if DEBUG:
+    if DEBUG: 
       print("DEBUG: ", end='')
       print(type+' '*(type_length-len(type))+':', *messages, **args)
 
   def verify(self, method, *args, **kwargs):
-    self.print_debug("Event", " "+method.__name__, (*args, *[f"{k}={repr(v)}" for k, v in kwargs.items()]), sep='')
+    self.print_debug("Event", " "+method.__name__, (*args, *[f"{k}={'v' if type(v) == str else v}" for k, v in kwargs.items()]), sep='')
 
     if Gui.paused: self.print_debug("Pause", "waiting...")
     while Gui.paused and self.is_alive(): usleep(1000)
 
-    if self.stopped: raise RuntimeError("kandinsky window destroyed")
+    if self.stoped: raise RuntimeError("kandinsky window destroyed")
     elif not self.is_alive(): raise RuntimeError(f"an internal error has occurred. Stack trace is before this it.")
 
   def sleep(self, delay_us):
     if USE_HEAP and Gui.heap_set: return # No need to sleep
 
     ratio = Gui.data.model*Gui.data.ratio
     delay = int(delay_us*ratio)
@@ -145,193 +134,193 @@
     self.print_debug("Delay", "input =", delay_us, "µs, ratio ≃", str(round(ratio, 6))+", output =", delay, "µs")
     if ratio > 0: usleep(delay)
 
 ### methods
   def get_pixel(self, x, y):
     Tests.int(x, y)
 
-    if x < 0 or x >= Vars.screen[0] or y < 0 or y >= Vars.screen[1]: color = Colors.black
+    if y < 0 or y > Vars.screen[0] or x < 0 or x > Vars.screen[1]: color = Colors.black
     else: color = Colors.convert(Draw.get_at(Gui.drawable, x, y))
 
     self.sleep(77)
     return color
 
   def set_pixel(self, x, y, color):
     Tests.int(x, y)
 
     Draw.pixel(Gui.drawable, Colors.convert(color), x, y)
-    self.sleep(96)
+    self.sleep(130)
 
   def color(self, r, g, b):
     if g is None and b is None: color = Colors.convert(r)
-    elif g is not None and b is not None:
+    elif g is not None and b is not None: 
       Tests.int(r, g, b)
       color = Colors.convert((r, g, b))
     else: raise TypeError("color takes 1 or 3 arguments")
 
     self.sleep(100)
     return color
 
   def draw_string(self, text, x, y, color, background, font=False):
     Tests.str(text)
     Tests.int(x, y)
-
+    
     color = Colors.convert(color)
     background = Colors.convert(background)
     bs = (7, 14) if font else (10,18)
     font = Config.small_font if font else Config.large_font
     if '\0' in text: text = text[:text.index('\0')]
 
-    for i, l in enumerate(text.replace('\r', '').replace('\f', '\x01').replace('\b', '\x01').replace('\v', '\x01').replace('\t', "    ").split('\n')):
+    for i, l in enumerate(text.replace('\r', '').replace('\f', '\x01').replace('\b', '\x01').replace('\v', '\x01').replace('\t', "    ").splitlines()): 
       Draw.rect(Gui.drawable, background, (x*(not i), y+i*bs[1], len(l)*bs[0], bs[1]))
       Draw.string(Gui.drawable, font, l, x*(not i), y+i*bs[1]-2, color)
     self.sleep(86*(len(text)+(len(text)>=5)//1.2))
-
+  
   def fill_rect(self, x, y, width, height, color):
     Tests.int(x, y, width, height)
-
+  
     if width < 0:  x, width = x+width, -width
     if height < 0: y, height = y+height, -height
-
+    
     Draw.rect(Gui.drawable, Colors.convert(color), (x, y, width, height))
     self.sleep(130+width*height/20+width*height*0.02)
 
   def wait_vblank(self):
     """why this?"""
     while not self.refreshed: usleep(100)
 
   def get_keys(self):
     """Don't tell me about this XD, it's omega"""
     # Raise an error if Ion-Numworks is not installed
-    if not ION_PRESENT: raise NotImplementedError("please install or upgrade 'ion-numworks' before using this method")
+    if not ION_PRESENT: raise NotImplementedError("please install or update the module 'Ion-numworks' before using this method")
     return ion.get_keys()
 
   def draw_line(self, x1, y1, x2, y2, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_line.cpp"""
     Tests.int(x1, y1, x2, y2)
     color = Colors.convert(color)
 
     s = abs(y2-y1) > abs(x2-x1)
     if s: x1, y1, x2, y2 = y1, x1, y2, x2
     if x1 > x2: x1, x2, y1, y2 = x2, x1, y2, y1
     g = 1 if x2 == x1 else (y2-y1)/(x2-x1)
 
     for x in range(x1, x2):
       ty = int(y1+g*(x-x1))
-      Draw.pixel(Gui.drawable, color, *((ty, x) if s else (x, ty)))  
+      Draw.pixel(Gui.drawable, color, *((ty, x) if s else (x, ty)))
 
-    self.sleep(1)
+    self.sleep(111) # TODO: calculate speed
 
   def draw_circle(self, x, y, r, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_circle.cpp"""
     Tests.int(x, y, r)
-
+    
     color = Colors.convert(color)
-    xc, yc, m = 0, abs(r), 5-4*abs(r)
+    xc, yc, m = 0, abs(r), 5-4*abs(r) 
 
     while xc <= yc:
       Draw.pixel(Gui.drawable, color, xc+x, yc+y)
       Draw.pixel(Gui.drawable, color, yc+x, xc+y)
       Draw.pixel(Gui.drawable, color, -xc+x, yc+y)
       Draw.pixel(Gui.drawable, color, -yc+x, xc+y)
       Draw.pixel(Gui.drawable, color, xc+x, -yc+y)
       Draw.pixel(Gui.drawable, color, yc+x, -xc+y)
       Draw.pixel(Gui.drawable, color, -xc+x, -yc+y)
       Draw.pixel(Gui.drawable, color, -yc+x, -xc+y)
-
+      
       if m > 0: yc, m = yc-1, m-8*yc
-      xc, m = xc+1, m+8*xc+4
+      xc, m = xc+1, m+8*xc+4 
 
-    self.sleep(sqrt(r)*(10*sqrt(10)*sqrt(r)-r))
+    self.sleep(222) # TODO: calculate speed
 
   def fill_circle(self, x, y, r, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_circle.cpp"""
     Tests.int(x, y, r)
     color = Colors.convert(color)
 
     r = abs(r)
     for i in range(x-r, x+r):
       semi = int(sqrt(r**2-(x-i)**2))
       Draw.rect(Gui.drawable, color, (i, y-semi, 1, semi*2))
 
-    self.sleep(sqrt(r)*(r+10*sqrt(10)*sqrt(r)-10))
+    self.sleep(333) # TODO: calculate speed
 
   def fill_polygon(self, points, color):
     """https://github.com/UpsilonNumworks/Upsilon/blob/upsilon-dev/kandinsky/src/context_polygon.cpp"""
     Tests.list(points)
     if len(points) < 3: raise ValueError("polygon must have least 3 points")
     tests = [[len(i) for v in i if len(i) != 2 or not Tests.int(v)] for i in points if Tests.list(i)]
     if len(tests) and len(tests[0]): raise ValueError("requested length 2 but object has length "+str(tests[0][0]))
-
+    
     color = Colors.convert(color)
-    points = list(points)
     points_size = len(points)
 
-    for y in range(min([[0,Vars.screen[0]]]+points, key=lambda v: v[1])[1], max([[0,0]]+points, key=lambda v: v[1])[1]):
+    for y in range(min([0,Vars.screen[0]]+points, key=lambda v: v[1]), max([0,0]+points, key=lambda v: v[1])):
       switches = []
       last_point = points_size-1
 
       for i in range(points_size):
         point_y, last_point_y = points[i][1], points[last_point][1]
         if ((point_y < y and last_point_y >= y) or (last_point_y < y and point_y >= y)) and point_y != last_point_y:
           switches.append(round(points[i][0]+1*(y-point_y)/(last_point_y-point_y)*(points[last_point][0]-points[i][0])))
         last_point = i
 
       switches.sort()
       for x in range(0, len(switches), 2):
         if switches[x] >= Vars.screen[1]*2: break
         if switches[x+1] > 0: Draw.rect(Gui.drawable, color, (switches[x], y, switches[x+1]-switches[x], 1))
 
-    self.sleep(len(points))
+    self.sleep(444) # TODO: calculate speed
 
   def get_palette():
-    return {"Toolbar":        Gui.data.color,
-            "AccentText":     (0, 132, 120),
-            "HomeBackground": Colors.white,
+    return {"Toolbar":        Gui.data.color, 
+            "AccentText":     (0, 132, 120), 
+            "HomeBackground": Colors.white, 
             "PrimaryText":    Colors.black,
             "SecondaryText":  (104, 108, 104)}
 ###
 
   def event_loop(self):
+    root = Tk()
     if USE_HEAP: Gui._main_thread_pid = self.native_id
-
+    
     try:
-      Gui(Tk())
+      Gui(root)
       Gui.config(not NO_GUI)
     except RuntimeError as e:
       # Handle multiple import of library
       # Library cannot open new tkinter root windows while another is opened but it can open another if previous is destroyed
       # Note: no data from the previous window can be restored to new one
-      if "main thread is not in main loop" in e.args[0]: prettywarn("multiple import of kandinsky is not permitted", ImportWarning)
+      if "main thread is not in main loop" in e.args[0]: prettywarn("multiple creation of window is not permitted", ImportWarning)
       else: self.print_debug("ERROR", type(e).__name__+": "+e.args[0])
       return
 
     self.OS_MODE = Gui.os_mode.get()
     # Bind more event
-    Gui.tkmaster.protocol("WM_DELETE_WINDOW", self.quit_app)
-    Gui.tkmaster.bind("<Control-q>", self.quit_app)
+    root.protocol("WM_DELETE_WINDOW", self.quit_app)
+    root.bind("<Control-q>", self.quit_app)
 
     Gui.paused = Gui.already_paused = False # Initialization finished, unpause events
 
     while True:
-      if self.stopped:
-        self.quit_app()
-        return
+      if self.stoped:
+        self.quit_app() 
+        return  
       elif not self.asknoclose and not main_thread().is_alive():
-        if Gui.askscriptend(): self.stopped = True
+        if Gui.askscriptend(): self.stoped = True
         else: self.asknoclose = True
-
+      
       self.refreshed = False
       try: Gui.refresh()
       except AttributeError: pass
-      except RuntimeError: self.stopped = True
+      except RuntimeError: self.stoped = True
       usleep(1000)
       self.refreshed = True
 
   def event_fire(self, method, *arg, **kwargs):
-    try:
+    try: 
       self.verify(method, *arg, **kwargs)
       return method(*arg, **kwargs), None
-    except (Exception, BaseException) as e:
+    except (Exception, BaseException) as e: 
       return None, Exception.with_traceback(
-        KeyboardInterrupt(type(e).__name__+": "+' '.join(e.args)) if isinstance(e, RuntimeError) else e,
+        KeyboardInterrupt(type(e).__name__+": "+' '.join(e.args)) if isinstance(e, RuntimeError) else e, 
         e.__traceback__.tb_next if DEBUG else None)
```

### Comparing `kandinsky-2.5/src/kandinsky/util/data/app.ico` & `kandinsky-2.5.dev1/src/kandinsky/util/data/app.ico`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/data/app.png` & `kandinsky-2.5.dev1/src/kandinsky/util/data/app.png`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/data/large_font.ttf` & `kandinsky-2.5.dev1/src/kandinsky/util/data/large_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/data/old_icons.zip` & `kandinsky-2.5.dev1/src/kandinsky/util/data/old_icons.zip`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/data/small_font.ttf` & `kandinsky-2.5.dev1/src/kandinsky/util/data/small_font.ttf`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/demo.py` & `kandinsky-2.5.dev1/src/kandinsky/util/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DECODE=lambda v: ((v&0xfff000)>>12, v&0xfff)
 class Snake:
  c=[(50,50,50),(240,240,240),(0,255,0),"green","red","blue","#7ea2ce"]
  def __init__(s,leader_board=(),speed=10,power=2,size=10,score=1,inf_snake=False,gost=False,darkmode=True,rainbow=False,walls=True):
   if inf_snake: power=float("inf")
   if not darkmode: s.c[0],s.c[1]=s.c[1],s.c[0]
   try: from kandinsky import get_keys
-  except ImportError:
+  except ImportError: 
    try: from ion import get_keys
    except ImportError: s.c[6]="#ffb531"
    else: s.c[6]="#c53431"
   s.lb,s.s,s.p,s.m,s.ti,s.g,s.go,s.r,s.w,s.bo=leader_board,1/speed,power,score,size,(320//size-1,220//size-1),gost,rainbow,walls,bool(walls)
  def nc(s):
   s.ch=[ri(s.bo,s.g[i]-s.bo) for i in range(2)]
   while s.ch[0]<<12|s.ch[1] in s.b: s.ch=[ri(s.bo,s.g[i]-s.bo) for i in range(2)]
@@ -101,15 +101,15 @@
    l=['>'*i+' '*(4-i)+s.lb[0][0]+':'+' '*(s.te-len(s.lb[0][0])+2)+str(s.lb[0][1])+' '*(4-i)+'<'*i for i in range(4)]
    while not kd(4) and not kd(17):
     for i in l:
      sl(0.2)
      if kd(4) or kd(17): break
      ds(i,20,52,s.c[6],s.c[0])
   except KeyboardInterrupt: pass
-
+  
 Snake(( # Leader board: ("name", score),
  ("Alteur",38),
  ("ZetaMap",30),
  ("Nios",23),
  ("Alpha6Frost",17),
 
 ), # Game settings: power, speed, size, score, inf_snake, darkmode, rainbow, gost, walls
```

### Comparing `kandinsky-2.5/src/kandinsky/util/old_config.ini` & `kandinsky-2.5.dev1/src/kandinsky/util/old_config.ini`

 * *Files identical despite different names*

### Comparing `kandinsky-2.5/src/kandinsky/util/stuff/color.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/color.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,30 +21,27 @@
   orange  = (248, 132, 24)
   purple  = (104, 44,  120)
   grey    = (160, 164, 160)
   gray    = grey
   cyan    = (0,   252, 248)
   magenta = (248, 4,   136)
   COLORS = {k: v for k, v in locals().items() if not k.startswith('_')}
+  
+  fix = lambda r, g, b: (((r>>3)&0x1f)<<3 if Vars.selected_os > 1 else Colors.expand((r>>3)&0x1f, 5),
+                            ((g>>2)&0x3f)<<2 if Vars.selected_os > 1 else Colors.expand((g>>2)&0x3f, 6),
+                            ((b>>3)&0x1f)<<3 if Vars.selected_os > 1 else Colors.expand((b>>3)&0x1f, 5))
+  expand = lambda v, nBits: (v<<(8-nBits)) | (v>>(nBits-(8-nBits)))
+  #TODO: make a __get_attribute__ to do invisible expand for numworks
 
-  fix = lambda r, g, b, expand=Vars.selected_os <= 1: (
-    (Colors.expand((r>>3)&0x1f, 5) if expand else ((r>>3)&0x1f)<<3),
-    (Colors.expand((g>>2)&0x3f, 6) if expand else ((g>>2)&0x3f)<<2),
-    (Colors.expand((b>>3)&0x1f, 5) if expand else ((b>>3)&0x1f)<<3))
-  fix2 = lambda *values, expand=Vars.selected_os <= 1: (
-    tuple(Colors.expand(Colors.contract(c, i%2, 3), 5+i%2) for i, c in enumerate(*values)) 
-      if expand else
-    tuple(Colors.contract(c, i%2, 3)<<(3-i%2) for i, c in enumerate(*values)))
-  contract = lambda v, nBits, length=8: (v>>(length-nBits))&(2**(4+length-nBits)-1)
-  expand = lambda v, nBits, length=8: (v<<(length-nBits))|(v>>(nBits-(length-nBits)))
+    
 
   def convert(rgbOrName):
     _type = type(rgbOrName)
-
-    if _type == str:
+    
+    if _type == str: 
       if rgbOrName in Colors.COLORS: return Colors.fix(*Colors.COLORS[rgbOrName])
       elif rgbOrName.startswith('#'):
         if len(rgbOrName) != 7: raise ValueError("RGB hex values are 6 bytes long")
 
         try: return Colors.fix(*[int(rgbOrName[i:i+2], 16) for i in range(1, len(rgbOrName), 2)])
         except ValueError as e:
           e.args = (f"invalid literal for int() with base 16: '{rgbOrName[1:]}'",)
@@ -53,13 +50,13 @@
         try: ratio = float(rgbOrName)
         except ValueError as e:
           e.args = ("invalid syntax for number",)
           raise
         else:
           if 0 <= ratio <= 1: return tuple([int(255*ratio) for _ in range(3)])
           else: raise ValueError("Gray levels are between 0.0 and 1.0")
-
+    
     elif _type == int: raise ValueError("Int are not colors")
 
     Tests.list(rgbOrName)
     if len(rgbOrName) != 3: raise ValueError("Color needs 3 components")
     return Colors.fix(*[int(c) for c in rgbOrName if type(c) == float or Tests.int(c)])
```

### Comparing `kandinsky-2.5/src/kandinsky/util/stuff/draw.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/draw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sdl2 import SDL_Rect, SDL_FillRect, SDL_BlitSurface, SDL_BlitScaled, SDL_CreateRGBSurfaceWithFormat, SDL_PIXELFORMAT_RGB888
 from sdl2.ext import prepare_color
-from ctypes import cast, byref, POINTER, c_uint32, c_uint8
+from ctypes import cast, byref, POINTER, c_uint, c_uint8
 from .vars import Vars
 
 __all__ = ["Draw"]
 
 
 class Draw:
   new_area = lambda *area: SDL_Rect(*[int(i*Vars.zoom_ratio) for i in (area[0] if len(area)==1 and type(area[0]) in (list, tuple) else area)])
@@ -12,9 +12,9 @@
   blit = lambda dest, source, area=None: SDL_BlitSurface(source, None, dest, Draw.new_area(area) if area else None)
   blit_scaled = lambda dest, source, area=None: SDL_BlitScaled(source, None, dest, Draw.new_area(area+(source.w, source.h) if len(area) == 2 else area) if area else None)
   rect = lambda dest, color, area=None: SDL_FillRect(dest, Draw.new_area(area) if area else None, prepare_color(color, dest))
   pixel = lambda dest, color, x, y: SDL_FillRect(dest, Draw.new_area(x, y, 1, 1), prepare_color(color, dest))
   string = lambda dest, font, text, x, y, color=None: Draw.blit_scaled(dest, font.render(text, color=color), (x, y))
 
   def get_at(source, x, y):
-    pixel = cast(byref(cast(source.pixels, POINTER(c_uint8)).contents, source.pitch*Vars.zoom_ratio*y+x*Vars.zoom_ratio*source.format.contents.BytesPerPixel), POINTER(c_uint32)).contents.value
+    pixel = cast(byref(cast(source.pixels, POINTER(c_uint8)).contents, (source.w*y+x)*source.format.contents.BytesPerPixel), POINTER(c_uint)).contents.value
     return (pixel&0xff0000)>>8, (pixel&0x00ff00)>>4, (pixel&0x0000ff)>>0
```

### Comparing `kandinsky-2.5/src/kandinsky/util/stuff/gui.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/gui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from tkinter import Tk, Frame, Menu, IntVar
 
 from tkinter.dialog import Dialog
 from tkinter.filedialog import asksaveasfilename
 from tkinter.font import Font
 
 from sdl2 import SDL_CreateWindowFrom, SDL_DestroyWindow, SDL_FreeSurface#, SDL_WINDOW_OPENGL
-from sdl2.ext import Window, load_img, init
+from sdl2.ext import Window, load_img
 
 from os import getcwd, system
 from webbrowser import open as open_link, register_standard_browsers  # To open links in help menu
-register_standard_browsers() # register now to avoid a long wait when opening a link
+register_standard_browsers() # register now to avoid a long wait when links open
 del register_standard_browsers
 from datetime import datetime
 
 # Internal
 from .vars import *
 from .draw import Draw
 from .color import Colors
@@ -33,28 +33,25 @@
   def created():
     if not Gui.tkmaster: raise RuntimeError("Gui: an instance must be created")
 
   def _unpause_after_wrapper(method):
     def _wrap(*a, **k):
       method(*a, **k)
       if not Gui.already_paused: Gui.paused = False
-
+    
     _wrap.__name__ = method.__name__
     return _wrap
 
   # Patched menu buttons to unpause script when is clicked
   _add_command = lambda menu, **kwargs: menu.add_command(**dict([(k, Gui._unpause_after_wrapper(v)) if "command" in k else (k, v) for k, v in kwargs.items()]))
   _add_radiobutton = lambda menu, **kwargs: menu.add_radiobutton(**dict([(k, Gui._unpause_after_wrapper(v)) if "command" in k else (k, v) for k, v in kwargs.items()]))
 
   def __init__(_, tkmaster):
-    # This is now, the video subsystem of SDL will be initialized
-    init(video=True)
-
     Gui.tkmaster = tkmaster
-    if Vars.is_linux:
+    if Vars.is_linux: 
       Gui.linux_menu_font = Font(tkmaster, family="SegoeUI", size=9)
       Gui.tkmaster.option_add("*font", Gui.linux_menu_font)
     Gui.data = StateData()
 
     # Create frame area, sdl2 windows and pack everything
     Gui.head_frame = Frame(tkmaster)
     Gui.screen_frame = Frame(tkmaster)
@@ -67,83 +64,69 @@
     Gui.menu = Menu(tkmaster)
     # Menus
     ## Help menu
     about = Menu(tearoff=False)
     Gui._add_command(about, label="GitHub project",     command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks"))
     Gui._add_command(about, label="Documentation",      command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks#usable-content"))
     Gui._add_command(about, label="An issue? Open one", command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/issues/new"))
-    Gui._secret_var = 0
-    def secret():
-      Gui._secret_var += 1
-      open_link("https://github.com/ZetaMap")
-      if Gui._secret_var == 3:
-        about.add_separator()
-        the_secret = lambda: system(f"start pythonw {Vars.path}../3d_demo.py") if Vars.is_windows else system(f"python3 {Vars.path}../3d_demo.py &")
-        Gui._add_command(about, label="3D engine demo", command=the_secret)
-    Gui._add_command(about, label="Made by ZetaMap",    command=secret)
+    Gui._add_command(about, label="Made by ZetaMap",    command=lambda: open_link("https://github.com/ZetaMap"))
     Gui.menu.add_cascade(label="About", menu=about)
 
     ## Help menu
     help = Menu(tearoff=False)
-    shortcuts = Menu(tearoff=False)
+    sortcut = Menu(tearoff=False)
 
-    Gui._add_command(shortcuts, label="CTRL+Q: Close window",    state="disabled", activebackground="#F0F0F0")
-    Gui._add_command(shortcuts, label="CTRL+O: change OS",       state="disabled", activebackground="#F0F0F0")
-    Gui._add_command(shortcuts, label="CTRL+M: change Model",    state="disabled", activebackground="#F0F0F0")
-    Gui._add_command(shortcuts, label="CTRL+S: take screenshot", state="disabled", activebackground="#F0F0F0")
-    Gui._add_command(shortcuts, label="CTRL+P: pause/resume",    state="disabled", activebackground="#F0F0F0")
-    Gui._add_command(shortcuts, label="CTRL+Z: change zoom",     state="disabled", activebackground="#F0F0F0")
-    help.add_cascade(label="Shortcuts", menu=shortcuts)
+    Gui._add_command(sortcut, label="CTRL+Q: Close window",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+O: change OS",       state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+M: change Model",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+S: take screenshot", state="disabled", activebackground="#F0F0F0")    
+    Gui._add_command(sortcut, label="CTRL+P: pause/resume",    state="disabled", activebackground="#F0F0F0")
+    Gui._add_command(sortcut, label="CTRL+Z: change zoom",     state="disabled", activebackground="#F0F0F0")
+    help.add_cascade(label="Shortcut", menu=sortcut)
 
     help.add_separator()
-    Gui._add_command(help, label="Ion keyboard", command=lambda: open_link("https://github.com/ZetaMap/Ion-Numworks#associated-keyboard-keys"))
+    Gui._add_command(help, label="Ion keyboard", command=lambda: open_link("https://github.com/ZetaMap/Ion-Numworks#keys"))
     Gui._add_command(help, label="Check FAQ",    command=lambda: open_link("https://github.com/ZetaMap/Kandinsky-Numworks/blob/main/FAQ.md"))
     Gui.menu.add_cascade(label="Help", menu=help)
 
     ## Options menu
     Gui.options = Menu(tearoff=False)
 
     ## OS menu
     Gui.os_mode = IntVar(value=Vars.selected_os)
     new = Menu(tearoff=False)
-    for i, mode in enumerate(Config.os_list):
+    for i, mode in enumerate(Config.os_list): 
       Gui._add_radiobutton(new, label=mode["name"], variable=Gui.os_mode, value=i, command=Gui.update_data)
-      mode["battery"] = load_img(Vars.path+mode["battery"])
-    new.add_separator()
-    Gui._add_command(new, label="Initial mode: "+Config.os_list[Vars.selected_os]["name"],
-                          state="disabled", activebackground="#F0F0F0")
+      Config.os_list[i]["battery"] = load_img(Vars.path+Config.os_list[i]["battery"])
     Gui.options.add_cascade(accelerator="CTRL+O", label="OS", menu=new)
 
     ## Model menu
     Gui.model_mode = IntVar(value=Vars.selected_model)
     new = Menu(tearoff=False)
-    for i, mode in enumerate(Config.model_list):
-      Gui._add_radiobutton(new, label=mode["name"], variable=Gui.model_mode, value=i, command=Gui.update_data,
+    for i, mode in enumerate(Config.model_list): 
+      Gui._add_radiobutton(new, label=mode["name"], variable=Gui.model_mode, value=i, command=Gui.update_data, 
         **({"state": "disabled", "activebackground": "#F0F0F0"} if mode.get("disabled", False) else {}))
     Gui.options.add_cascade(accelerator="CTRL+M", label="Model", menu=new)
-    new.add_separator()
-    Gui._add_command(new, label="Initial model: "+Config.model_list[Vars.selected_model]["name"],
-                          state="disabled", activebackground="#F0F0F0")
 
     Gui.zoom = IntVar(value=Vars.zoom_ratio)
     Gui.increase_font = IntVar()
     Gui.zoom.trace_add("write", Gui.set_zoom)
     Gui.increase_font.trace_add("write", Gui.set_zoom)
     new = Menu(tearoff=False)
     for i in range(Config.zoom_max): Gui._add_radiobutton(new, label=f"x{i+1}", variable=Gui.zoom, value=i+1)
-    if Vars.is_linux: new.add_checkbutton(label="Increase font size", variable=Gui.increase_font)
+    if not Vars.is_windows: new.add_checkbutton(label="Increase font size", variable=Gui.increase_font)
     Gui.options.add_cascade(accelerator="CTRL+Z", label="Zoom", menu=new)
 
     Gui.options.add_separator()
 
     ## Screenshot button
-    Gui.options.add_command(accelerator="CTRL+S", label="Screenshot", command=Gui.askscreenshot)
+    Gui.options.add_command(accelerator="CTRL+S", label="Screenshot", command=Gui.screenshot)
 
     ## Pause button
-    def state(states=["Pause", "Resume"]):
+    def state(states=["Pause", "Resume"]): 
       Gui.already_paused = not Gui.already_paused
       Gui.paused = Gui.already_paused
       Gui.options.entryconfig(states[not Gui.already_paused], label=states[Gui.already_paused])
     Gui.options.add_command(accelerator="CTRL+P", label="Pause", command=state)
 
     Gui.menu.add_cascade(label="Options", menu=Gui.options)
 
@@ -161,31 +144,26 @@
       return
 
     SDL_DestroyWindow(Gui.head.window)
     SDL_DestroyWindow(Gui.screen.window)
     Gui.head_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.head_size*Vars.zoom_ratio)
     Gui.screen_frame.config(width=Vars.screen[0]*Vars.zoom_ratio, height=Vars.screen[1]*Vars.zoom_ratio)
     Gui.tkmaster.update()
-    Gui.head.window = SDL_CreateWindowFrom(Gui.get_widget_id(Gui.head_frame))
-    Gui.screen.window = SDL_CreateWindowFrom(Gui.get_widget_id(Gui.screen_frame))
+    Gui.head.window = SDL_CreateWindowFrom(Gui.head_frame.winfo_id())
+    Gui.screen.window = SDL_CreateWindowFrom(Gui.screen_frame.winfo_id())
     Gui.screen_surf = Gui.screen.get_surface()
-
+    
     last_drawable = Gui.drawable
     Gui.drawable = Draw.new_surface(*Vars.screen)
-    Draw.rect(Gui.drawable, Colors.fix2(Colors.white))
     Draw.blit_scaled(Gui.drawable, last_drawable)
     Gui.update_data()
 
     Gui.center_window()
     if not Gui.already_paused: Gui.paused = False
 
-  def get_widget_id(widget):
-    """Method to get id of widget, will be replaced by mac_patcher.py if needed"""
-    return widget.winfo_id()
-
   def destroy():
     Gui.created()
 
     SDL_FreeSurface(Gui.drawable)
     Gui.head.close()
     Gui.screen.close()
     Gui.tkmaster.quit()
@@ -201,32 +179,32 @@
       Gui.update_data()
 
   def update_data():
     Gui.created()
     if Gui.head.window is None: return
 
     Gui.data(**Config.os_list[Gui.os_mode.get()], model=Config.model_list[Gui.model_mode.get()]["ratio"])
-    Gui.head_surface = Draw.new_surface(Vars.screen[0], Vars.head_size)
+    Gui.head_surface = Draw.new_surface(Vars.screen[0],Vars.head_size)
 
     Draw.rect(Gui.head_surface, Gui.data.color)
     Draw.string(Gui.head_surface, Config.small_font, Gui.data.unit, 5, 0)
     Draw.string(Gui.head_surface, Config.small_font, "PYTHON", Vars.screen[0]//2-21, 1)
     x = Vars.screen[0]-20
     if Gui.data.clock:
       Draw.string(Gui.head_surface, Config.small_font, datetime.now().strftime("%H:%M"), x-20, 1)
       x -= 40
     Draw.blit_scaled(Gui.head_surface, Gui.data.battery, (x, 4))
     # try to blit it now on screen
     try: Draw.blit(Gui.head.get_surface(), Gui.head_surface)
     except: pass
 
     # Set new heap of python
-    if Gui._main_thread_pid:
+    if Gui._main_thread_pid: 
       try: limiter.set_heap(Gui._main_thread_pid, Gui.data.heap)
-      except (AssertionError, OSError): Gui.heap_set = False
+      except (AssertionError, OSError): raise #Gui.heap_set = False
       else: Gui.heap_set = True
 
   def config(create_gui=False):
     Gui.created()
 
     # Config main window
     Gui.tkmaster.title(Vars.app_name)
@@ -238,28 +216,28 @@
     if create_gui: Gui.tkmaster.config(menu=Gui.menu)
     Gui.tkmaster.eval('tk::PlaceWindow . center') # I must keep this otherwise the SDL windows do not configure correctly
     Gui.center_window()
 
     # Bind shorcuts
     Gui.tkmaster.bind("<Control-o>", lambda _: Gui.update_value(Gui.os_mode, Config.os_list))
     Gui.tkmaster.bind("<Control-m>", lambda _: Gui.update_value(Gui.model_mode, Config.model_list))
-    Gui.tkmaster.bind("<Control-s>", lambda _: Gui.askscreenshot())
-    def state(*_, states=["Pause", "Resume"]):
+    Gui.tkmaster.bind("<Control-s>", lambda _: Gui.screenshot())
+    def state(*_, states=["Pause", "Resume"]): 
       Gui.already_paused = not Gui.already_paused
       Gui.paused = Gui.already_paused
       Gui.options.entryconfig(states[not Gui.already_paused], label=states[Gui.already_paused])
     Gui.tkmaster.bind("<Control-p>", state)
     Gui.tkmaster.bind("<Control-z>", lambda _: Gui.update_value(Gui.zoom, [{}]*(Config.zoom_max+1), 1))
 
     ### Windows patchs
     if Vars.is_windows:
       # Bind events to pause, if dragged or user interact with gui
       def drag_event(e):
         if e.widget is Gui.tkmaster:
-          if Gui._drag_window_event_id:
+          if Gui._drag_window_event_id: 
             Gui.tkmaster.after_cancel(Gui._drag_window_event_id)
             Gui.paused = True
           Gui._drag_window_event_id = Gui.tkmaster.after(200, drag_event_stop)
       def drag_event_stop():
         Gui._drag_window_event_id = ''
         if not Gui.already_paused: Gui.paused = False
       drag_event_stop()
@@ -278,50 +256,50 @@
     Gui.update_data() # Set default data
     Gui.refresh() # Refresh SDL windows and Tkinter frames
 
   def center_window():
     Gui.created()
     Gui.tkmaster.geometry(f"+{max(0, Gui.tkmaster.winfo_screenwidth() //2-Gui.tkmaster.winfo_width() //2)}"
                           f"+{max(0, Gui.tkmaster.winfo_screenheight()//2-Gui.tkmaster.winfo_height()//2)}")
-
+    
   def refresh():
     Gui.created()
-
+    
     Gui.head.refresh()
     Draw.rect(Gui.screen_surf, Colors.black)
     Draw.blit(Gui.screen_surf, Gui.drawable)
     Gui.screen.refresh()
-    Gui.tkmaster.update_idletasks()
+    Gui.tkmaster.update_idletasks()  
     Gui.tkmaster.update()
 
-  def askscreenshot():
+  def screenshot():
     Gui.created()
-    Gui.paused = True # Pause events
+    Gui.paused = True # Pause events 
     file = (getcwd().replace("\\\\", "\\"), datetime.now().strftime("Screenshot_%Y%m%d-%H%M%S.png"))
 
     # Create new surface to blit head and screen into
     surf = Draw.new_surface(Vars.screen[0], Vars.head_size+Vars.screen[1])
     Draw.blit(surf, Gui.head_surface)
     Draw.blit(surf, Gui.drawable, (0, Vars.head_size))
-
+    
     try: error = Config.save_image(surf, file[1]) < 0
     except: error = 1
 
     conf = {"title": "Screenshot", "text": "Screenshot saved at: \n"+('\\' if Vars.is_windows else '/').join(file), "bitmap": "info", "default": 1, "strings": ("Open folder", "OK")}
     if error: conf.update({"text": "Error, can't write in folder: \n"+file[0], "bitmap": "error", "strings": ("Save as", "OK")})
 
     if not Dialog(Gui.tkmaster, conf).num:
-      if error:
+      if error: 
         file = asksaveasfilename(defaultextension="png", filetypes=Vars.image_formats, initialfile=file[1], title="Save screenshot at")
-        if file != '':
+        if file != '': 
           try: Config.save_image(surf, file)
           except: pass
       else: system(f"{'explorer' if Vars.is_windows else 'open' if Vars.is_macos else 'xdg-open'} \"{file[0]}\" 2> {'nul' if Vars.is_windows else '/dev/null'}")
 
     SDL_FreeSurface(surf) # destroy screenshot surface
     if not Gui.already_paused: Gui.paused = False # Screenshot finished, unpause events
 
   def askscriptend():
     return not Dialog(Gui.tkmaster, {
-      "title": "Script end", "text": "Script finished! \nClose window?".ljust(50),
+      "title": "Script end", "text": "Script finished! \nClose window?".ljust(50), 
       "bitmap": "question", "default": 0, "strings": ("Yes", "No")
     }).num
```

### Comparing `kandinsky-2.5/src/kandinsky/util/stuff/limiter.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/limiter.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,31 +128,7 @@
     prettywarn("libc6 library is not installed. Using time module to do usleep (emulation will be less accurate)", RuntimeWarning)
     usleep = lambda us: _time.sleep(us/10e6)
 
 else:
   # MacOS don't have libc6 library and idk for other OS so just do a normal sleep
   import time as _time
   usleep = lambda us: _time.sleep(us/10e6)
-
-
-
-# Other stuff, 
-# because there is a bug when window changing monitor 
-# (only on macos... again... this is a poor platform)
-def get_monitors():
-  import ctypes
-  class RECT(ctypes.Structure):
-    _fields_ = [
-      ('left', ctypes.c_long),
-      ('top', ctypes.c_long),
-      ('right', ctypes.c_long),
-      ('bottom', ctypes.c_long)
-      ]
-    def dump(self):
-      return [int(val) for val in (self.left, self.top, self.right, self.bottom)]
-
-  retval = {}
-  def cb(hMonitor, hdcMonitor, lprcMonitor, dwData):
-    retval.update({hMonitor: lprcMonitor.contents.dump()})
-    return True
-  ctypes.windll.user32.EnumDisplayMonitors(0, 0, ctypes.WINFUNCTYPE(ctypes.c_int, ctypes.c_ulong, ctypes.c_ulong, ctypes.POINTER(RECT), ctypes.c_double)(cb), 0)
-  return retval
```

### Comparing `kandinsky-2.5/src/kandinsky/util/stuff/vars.py` & `kandinsky-2.5.dev1/src/kandinsky/util/stuff/vars.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,39 +3,70 @@
 from sdl2.ext.ttf import FontManager
 
 import sys, os
 
 __all__ = [
   "Vars",
   "Config",
-  "StateData"
+  "StateData" 
 ]
 
+"""
+benchmarks:
+ - epsilon:
+   - set_pixel: 130 µs
+   - 100*100: fill_rect: 750 µs
+   - 1*1: fill_rect: 130 µs
+   - draw_string: 640 µs
+   - get_pixel: 77 µs
+   - color: 180 µs
+
+ - omega:
+   - set_pixel: 63 µs
+   - 100*100: fill_rect: 740 µs
+   - 1*1: fill_rect: 67 µs
+   - draw_string: 443 µs
+   - get_pixel: 60 µs
+   - color: 168 µs
+
+ - upsilon:
+   - set_pixel: 80 µs
+   - 100*100: fill_rect: 753 µs
+   - 1*1: fill_rect: 109 µs
+   - draw_string: 426 µs
+   - get_pixel: 76 µs
+   - color: 210 µs
+
+magic draw ratio (first draw):
+  - epsilon: 02:17.713
+  - omega: 02:07.797
+  - upsilon: 02:22.141
+"""
 
 class Vars:
   base_name = __module__.split('.')[1]
   path = __file__[:__file__.rindex(base_name)+len(base_name)+1]+"data/"
   # Test if path is correct
   if not os.path.exists(path): path = __file__[:__file__.rindex(base_name)]+"data/"
 
-  is_windows = sys.platform.startswith("win")
-  is_macos = sys.platform.startswith("darwin")
-  is_linux = sys.platform.startswith("linux") or (not is_windows and not is_macos)
+  is_windows = sys.platform == "win32"
+  is_linux = sys.platform == "linux"
+  is_macos = sys.platform == "darwin"
   app_name = "Kandinsky Emulator"
   head_size = 18
   screen = (320, 222)
   zoom_ratio = selected_os = selected_model = 1
 
   image_formats = [("PNG", ".png"), ("Bitmap", ".bmp"), ("All files", ".*")]
   if not is_macos: image_formats.insert(1, ("JPEG", (".jpg", ".jpeg")))
 
 
 class Config:
   open = lambda path, mode='w': SDL_RWFromFile(path.encode("utf-8"), bytes(mode, "utf-8"))
-  save_image = lambda surface, path: (SDL_SaveBMP_RW(surface, Config.open(path), 1) if path.endswith(".bmp") else
+  save_image = lambda surface, path: (SDL_SaveBMP_RW(surface, Config.open(path), 1) if path.endswith(".bmp") else 
                                       IMG_SaveJPG_RW(surface, Config.open(path), 1, 70) if not Vars.is_macos and path.endswith((".jpg", ".jpeg")) else
                                       IMG_SavePNG_RW(surface, Config.open(path), 1))
 
   large_font = FontManager(Vars.path+"large_font.ttf", size=16)
   small_font = FontManager(Vars.path+"small_font.ttf", size=12)
 
   os_list = (                          #heap in byte, -1=infinite
@@ -50,25 +81,29 @@
     {"name": "n0120", "ratio": 0, "disabled": True},
   )
 
   default_os = 1
   default_model = 1
   zoom_max = 4
 
-# Class to store some data
+# Class for some data
 class StateData:
+  __field_name__ = ""
+
   def __init__(self, **content):
     self(**content)
 
   def __call__(self, **content):
-    self.__dict__.update(content)
+    for k, v in content.items(): setattr(self, k, v)
     return self
 
   def __str__(self):
-    return "{}({})".format(__class__.__name__, ', '.join(f"{k}={repr(v)}" for k, v in self.__dict__.items() if not k.startswith("__")))
+    return "<{} ({})>".format(__class__.__name__, self.__dict__)
+
+  def __repr__(self):
+    return self.__str__()
 
-  __repr__ = __str__
+  def has(self, name):
+    return hasattr(self, name)
 
-  def __contains__(self, name):
-    if type(name) != str: raise TypeError("attribute name must be an str")
-    if not name: raise ValueError("empty attribute name")
-    return name in self.__dict__
+  def get(self, name, default=None):
+    return getattr(self, name, default)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kandinsky-2.5/src/kandinsky.egg-info/PKG-INFO` & `kandinsky-2.5.dev1/src/kandinsky.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: kandinsky
-Version: 2.5
+Version: 2.5.dev1
 Summary: A small module allowing to link the kandinsky module, from the Numworks, to a window.
 Home-page: https://github.com/ZetaMap/Kandinsky-Numworks
 Author: ZetaMap
 License: MIT
 Project-URL: GitHub Project, https://github.com/ZetaMap/Kandinsky-Numworks
 Project-URL: My GitHub Page, https://github.com/ZetaMap/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `kandinsky-2.5/src/kandinsky.egg-info/SOURCES.txt` & `kandinsky-2.5.dev1/src/kandinsky.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 changelog.txt
 setup.py
 src/kandinsky/FAQ.md
 src/kandinsky/README.md
 src/kandinsky/__init__.py
 src/kandinsky/__init__.pyi
 src/kandinsky/__main__.py
+src/kandinsky/test.py
 src/kandinsky.egg-info/PKG-INFO
 src/kandinsky.egg-info/SOURCES.txt
 src/kandinsky.egg-info/dependency_links.txt
 src/kandinsky.egg-info/requires.txt
 src/kandinsky.egg-info/top_level.txt
-src/kandinsky/util/3d_demo.py
 src/kandinsky/util/core.py
 src/kandinsky/util/demo.py
-src/kandinsky/util/mac_patcher.py
 src/kandinsky/util/old_config.ini
 src/kandinsky/util/data/app.ico
 src/kandinsky/util/data/app.png
 src/kandinsky/util/data/battery0.png
 src/kandinsky/util/data/battery1.png
 src/kandinsky/util/data/large_font.ttf
 src/kandinsky/util/data/old_icons.zip
 src/kandinsky/util/data/small_font.ttf
 src/kandinsky/util/stuff/__init__.py
 src/kandinsky/util/stuff/color.py
 src/kandinsky/util/stuff/draw.py
 src/kandinsky/util/stuff/gui.py
+src/kandinsky/util/stuff/ion.py
 src/kandinsky/util/stuff/limiter.py
 src/kandinsky/util/stuff/tests.py
 src/kandinsky/util/stuff/vars.py
```

