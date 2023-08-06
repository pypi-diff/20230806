# Comparing `tmp/uib_inf100_graphics-0.2.0.tar.gz` & `tmp/uib_inf100_graphics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uib_inf100_graphics-0.2.0.tar", last modified: Tue Jun 27 14:01:21 2023, max compression
+gzip compressed data, was "uib_inf100_graphics-0.3.0.tar", last modified: Sun Aug  6 19:04:49 2023, max compression
```

## Comparing `uib_inf100_graphics-0.2.0.tar` & `uib_inf100_graphics-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-06-27 14:01:21.800924 uib_inf100_graphics-0.2.0/
--rw-r--r--   0 torsteins   (501) staff       (20)     6835 2023-06-27 14:01:21.800770 uib_inf100_graphics-0.2.0/PKG-INFO
--rw-r--r--   0 torsteins   (501) staff       (20)     6072 2023-06-27 13:59:32.000000 uib_inf100_graphics-0.2.0/README.md
--rw-r--r--   0 torsteins   (501) staff       (20)      987 2023-06-27 12:30:36.000000 uib_inf100_graphics-0.2.0/pyproject.toml
--rw-r--r--   0 torsteins   (501) staff       (20)       38 2023-06-27 14:01:21.800970 uib_inf100_graphics-0.2.0/setup.cfg
-drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-06-27 14:01:21.797889 uib_inf100_graphics-0.2.0/src/
-drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-06-27 14:01:21.799432 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/
--rw-r--r--   0 torsteins   (501) staff       (20)       92 2023-06-27 11:55:14.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/__init__.py
--rw-r--r--   0 torsteins   (501) staff       (20)      144 2023-06-27 11:56:43.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/types.py
--rw-r--r--   0 torsteins   (501) staff       (20)    26006 2023-06-27 11:53:16.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/uib_inf100_graphics.py
--rw-r--r--   0 torsteins   (501) staff       (20)     7907 2023-06-27 11:51:07.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/version.py
-drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-06-27 14:01:21.800540 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/
--rw-r--r--   0 torsteins   (501) staff       (20)     6835 2023-06-27 14:01:21.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/PKG-INFO
--rw-r--r--   0 torsteins   (501) staff       (20)      409 2023-06-27 14:01:21.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/SOURCES.txt
--rw-r--r--   0 torsteins   (501) staff       (20)        1 2023-06-27 14:01:21.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/dependency_links.txt
--rw-r--r--   0 torsteins   (501) staff       (20)       31 2023-06-27 14:01:21.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/requires.txt
--rw-r--r--   0 torsteins   (501) staff       (20)       20 2023-06-27 14:01:21.000000 uib_inf100_graphics-0.2.0/src/uib_inf100_graphics.egg-info/top_level.txt
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.089635 uib_inf100_graphics-0.3.0/
+-rw-r--r--   0 torsteins   (501) staff       (20)     4657 2023-08-06 19:04:49.089474 uib_inf100_graphics-0.3.0/PKG-INFO
+-rw-r--r--   0 torsteins   (501) staff       (20)     3895 2023-08-06 10:59:13.000000 uib_inf100_graphics-0.3.0/README.md
+-rw-r--r--   0 torsteins   (501) staff       (20)      987 2023-06-27 12:30:36.000000 uib_inf100_graphics-0.3.0/pyproject.toml
+-rw-r--r--   0 torsteins   (501) staff       (20)       38 2023-08-06 19:04:49.089684 uib_inf100_graphics-0.3.0/setup.cfg
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.084965 uib_inf100_graphics-0.3.0/src/
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.085893 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/
+-rw-r--r--   0 torsteins   (501) staff       (20)       82 2023-08-06 10:59:13.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/__init__.py
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.087138 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/event_app/
+-rw-r--r--   0 torsteins   (501) staff       (20)       41 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/event_app/__init__.py
+-rw-r--r--   0 torsteins   (501) staff       (20)      144 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/event_app/types.py
+-rw-r--r--   0 torsteins   (501) staff       (20)    26016 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/event_app/uib_inf100_graphics.py
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.088133 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/helpers/
+-rw-r--r--   0 torsteins   (501) staff       (20)      104 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/helpers/__init__.py
+-rw-r--r--   0 torsteins   (501) staff       (20)     6849 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/helpers/image.py
+-rw-r--r--   0 torsteins   (501) staff       (20)       80 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/helpers/logger.py
+-rw-r--r--   0 torsteins   (501) staff       (20)    13030 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/helpers/text.py
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.089230 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/
+-rw-r--r--   0 torsteins   (501) staff       (20)    11248 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/Configuration.py
+-rw-r--r--   0 torsteins   (501) staff       (20)     7474 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/RecordingCanvas.py
+-rw-r--r--   0 torsteins   (501) staff       (20)     7499 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/SimplifiedFrame.py
+-rw-r--r--   0 torsteins   (501) staff       (20)       45 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/__init__.py
+-rw-r--r--   0 torsteins   (501) staff       (20)      498 2023-08-06 11:09:41.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/simple/globals.py
+-rw-r--r--   0 torsteins   (501) staff       (20)     8355 2023-08-06 10:59:13.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/version.py
+drwxr-xr-x   0 torsteins   (501) staff       (20)        0 2023-08-06 19:04:49.086561 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/
+-rw-r--r--   0 torsteins   (501) staff       (20)     4657 2023-08-06 19:04:49.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/PKG-INFO
+-rw-r--r--   0 torsteins   (501) staff       (20)      875 2023-08-06 19:04:49.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/SOURCES.txt
+-rw-r--r--   0 torsteins   (501) staff       (20)        1 2023-08-06 19:04:49.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/dependency_links.txt
+-rw-r--r--   0 torsteins   (501) staff       (20)       31 2023-08-06 19:04:49.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/requires.txt
+-rw-r--r--   0 torsteins   (501) staff       (20)       20 2023-08-06 19:04:49.000000 uib_inf100_graphics-0.3.0/src/uib_inf100_graphics.egg-info/top_level.txt
```

### Comparing `uib_inf100_graphics-0.2.0/pyproject.toml` & `uib_inf100_graphics-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/uib_inf100_graphics.py` & `uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/event_app/uib_inf100_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # uib_inf100_graphics.py
 
 # Require Python 3.10 or later
 import sys
 if ((sys.version_info[0] != 3) or (sys.version_info[1] < 10)):
     raise Exception('uib_inf100_graphics requires Python version 3.10 or later.')
 
-from .version import __version__, __last_updated__
+from uib_inf100_graphics.version import __version__, __last_updated__
 
 # Track version and file update timestamp
 MAJOR_VERSION = int(__version__.split('.')[0])
 MINOR_VERSION = float(__version__[(__version__.index('.')+1):])
 LAST_UPDATED  = __last_updated__
 
 from typing import Any
@@ -196,29 +196,29 @@
         app._running = False
         app._root.quit() # break out of root.mainloop() without closing window!
 
     def __setattr__(app, attr, val):
         d = app.__dict__
         d[attr] = val
         canvas = d.get('_canvas', None)
-        if (d.get('running', False) and
-            d.get('mvc_check', False) and
-            (canvas is not None) and
-            canvas.in_redraw_all):
+        if (d.get('running', False)
+                and d.get('mvc_check', False)
+                and (canvas is not None) 
+                and canvas.in_redraw_all):
             app._mvc_violation(f'you may not change app.{attr} in the model while in redraw_all (the view)')
 
     def _print_user_traceback(app, exception, tb):
         stack = traceback.extract_tb(tb)
         lines = traceback.format_list(stack)
         in_redraw_all_wrapper = False
         print_lines = [ ]
         for line in lines:
-            if (('"uib_inf100_graphics.py"' not in line) and
-                ('/uib_inf100_graphics.py' not in line) and
-                ('\\uib_inf100_graphics.py' not in line) and
+            if (('uib_inf100_graphics' not in line) and
+                ('/uib_inf100_graphics/' not in line) and
+                ('\\uib_inf100_graphics\\' not in line) and
                 ('/tkinter/' not in line) and
                 ('\\tkinter\\' not in line)):
                 print_lines.append(line)
             if ('redraw_all_wrapper' in line):
                 in_redraw_all_wrapper = True
         if (len(print_lines) == 0):
             # No user code in trace, so we have to use all the code (bummer),
@@ -260,15 +260,15 @@
     @_safe_method
     def _redraw_all_wrapper(app):
         if (not app._running): return
         if ('deferred_redraw_all' in app._afterIdMap): return # wait for pending call
         app._canvas.in_redraw_all = True
         app._canvas.delete(ALL)
         width,outline = (10,'red') if app._paused else (0,'white')
-        app._canvas.create_rectangle(0, 0, app.width, app.height, fill='white', width=width, outline=outline)
+        app._canvas.create_rectangle(0, 0, app.width, app.height, width=width, outline=outline)
         app._canvas.logged_drawing_calls = [ ]
         app._canvas.log_drawing_calls = app._log_drawing_calls
         hash1 = get_hash(app) if app._mvc_check else None
         try:
             app.redraw_all(app._canvas)
             hash2 = get_hash(app) if app._mvc_check else None
             if (hash1 != hash2):
```

### Comparing `uib_inf100_graphics-0.2.0/src/uib_inf100_graphics/version.py` & `uib_inf100_graphics-0.3.0/src/uib_inf100_graphics/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # version.py
 import datetime
 
-__version__ = "0.2.0"
-__last_updated__ = datetime.date(year=2023, month=6, day=27)
+__version__ = "0.3.0"
+__last_updated__ = datetime.date(year=2023, month=8, day=6)
+
+
+# Version 0.3.0
+#  * Added the simple subpackage which provides an iterative interface
+#    to the graphics package. This is intended to be used by students who
+#    are not yet familiar with event-driven programming.
+#  * Added helpers subpackage with text_in_box and image_in_box functions
+#  * Moved the event-driven app to eventapp subpackage
+#  * Created examples folder with some first examples, particularly for the
+#    simple subpackage
+
 
 # Version 0.2.0
 #  * Added types for run_app -method (constructor of TopLevelApp) and types
 #    App, MouseEvent and KeyEvent that may be helpful for users who want to
 #    use type hints in their own code
 
 # Version 0.1.0
```

