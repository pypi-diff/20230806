# Comparing `tmp/yaspin-2.3.0.tar.gz` & `tmp/yaspin-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaspin-2.3.0.tar", max compression
+gzip compressed data, was "yaspin-2.4.0.tar", max compression
```

## Comparing `yaspin-2.3.0.tar` & `yaspin-2.4.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     5294 2023-01-06 14:30:58.853399 yaspin-2.3.0/HISTORY.rst
--rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-2.3.0/LICENSE
--rw-r--r--   0        0        0    11962 2023-01-06 13:03:28.924877 yaspin-2.3.0/README.rst
--rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-2.3.0/examples/advanced_colors.py
--rw-r--r--   0        0        0     1089 2023-01-06 14:17:51.704424 yaspin-2.3.0/examples/basic_usage.py
--rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/cli_spinners.py
--rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/colors.py
--rw-r--r--   0        0        0     4879 2023-01-06 14:18:08.246403 yaspin-2.3.0/examples/demo.py
--rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/dynamic_text.py
--rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/finalizers.py
--rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/hide_show.py
--rw-r--r--   0        0        0     1533 2022-07-19 10:41:34.971459 yaspin-2.3.0/examples/hide_show_prompt_toolkit.py
--rw-r--r--   0        0        0      482 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/reverse_spinner.py
--rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/right_spinner.py
--rw-r--r--   0        0        0     4030 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/signals.py
--rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-2.3.0/examples/spinner_properties.py
--rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-2.3.0/examples/timer_spinner.py
--rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-2.3.0/examples/write_method.py
--rw-r--r--   0        0        0     2411 2023-01-06 14:30:58.853399 yaspin-2.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/__init__.py
--rw-r--r--   0        0        0     6420 2022-07-19 10:41:34.977459 yaspin-2.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3025 2022-07-19 10:41:34.977459 yaspin-2.3.0/tests/test_attrs.py
--rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/test_finalizers.py
--rw-r--r--   0        0        0     7814 2022-07-19 10:41:34.978459 yaspin-2.3.0/tests/test_in_out.py
--rw-r--r--   0        0        0     1507 2022-07-19 10:41:34.979459 yaspin-2.3.0/tests/test_pipes.py
--rw-r--r--   0        0        0     3479 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/test_properties.py
--rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-2.3.0/tests/test_signals.py
--rw-r--r--   0        0        0      695 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/test_spinners.py
--rw-r--r--   0        0        0     1373 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/test_timer.py
--rw-r--r--   0        0        0     1217 2022-07-11 11:51:22.128125 yaspin-2.3.0/tests/test_yaspin.py
--rw-r--r--   0        0        0      218 2022-07-11 11:51:22.128125 yaspin-2.3.0/yaspin/__init__.py
--rw-r--r--   0        0        0     2600 2022-12-29 06:38:38.944572 yaspin-2.3.0/yaspin/api.py
--rw-r--r--   0        0        0      351 2023-01-06 13:20:39.670718 yaspin-2.3.0/yaspin/base_spinner.py
--rw-r--r--   0        0        0     2714 2023-01-06 14:18:08.250403 yaspin-2.3.0/yaspin/constants.py
--rw-r--r--   0        0        0    17976 2023-01-06 13:20:19.607734 yaspin-2.3.0/yaspin/core.py
--rw-r--r--   0        0        0    22348 2022-08-05 08:43:50.814201 yaspin-2.3.0/yaspin/data/spinners.json
--rw-r--r--   0        0        0      329 2023-01-06 13:20:42.551715 yaspin-2.3.0/yaspin/helpers.py
--rw-r--r--   0        0        0     1065 2022-07-11 11:51:22.129125 yaspin-2.3.0/yaspin/signal_handlers.py
--rw-r--r--   0        0        0      505 2022-07-11 11:51:22.129125 yaspin-2.3.0/yaspin/spinners.py
--rw-r--r--   0        0        0    13117 1970-01-01 00:00:00.000000 yaspin-2.3.0/setup.py
--rw-r--r--   0        0        0    14366 1970-01-01 00:00:00.000000 yaspin-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5419 2023-08-06 12:43:09.749394 yaspin-2.4.0/HISTORY.rst
+-rw-r--r--   0        0        0     1072 2022-07-11 11:51:22.114125 yaspin-2.4.0/LICENSE
+-rw-r--r--   0        0        0    11970 2023-08-06 12:43:09.749394 yaspin-2.4.0/README.rst
+-rw-r--r--   0        0        0      909 2023-01-06 13:49:42.862298 yaspin-2.4.0/examples/advanced_colors.py
+-rw-r--r--   0        0        0     1089 2023-08-06 12:02:54.701543 yaspin-2.4.0/examples/basic_usage.py
+-rw-r--r--   0        0        0      493 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/cli_spinners.py
+-rw-r--r--   0        0        0     1577 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/colors.py
+-rw-r--r--   0        0        0     4879 2023-01-06 14:18:08.246403 yaspin-2.4.0/examples/demo.py
+-rw-r--r--   0        0        0      552 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/dynamic_text.py
+-rw-r--r--   0        0        0      699 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/finalizers.py
+-rw-r--r--   0        0        0      621 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/hide_show.py
+-rw-r--r--   0        0        0     1532 2023-02-26 15:11:07.363981 yaspin-2.4.0/examples/hide_show_prompt_toolkit.py
+-rw-r--r--   0        0        0      481 2023-02-26 15:11:07.363981 yaspin-2.4.0/examples/reverse_spinner.py
+-rw-r--r--   0        0        0      415 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/right_spinner.py
+-rw-r--r--   0        0        0     4030 2023-08-06 12:02:54.702543 yaspin-2.4.0/examples/signals.py
+-rw-r--r--   0        0        0      854 2022-07-11 11:51:22.115125 yaspin-2.4.0/examples/spinner_properties.py
+-rw-r--r--   0        0        0      359 2022-07-19 11:35:29.002311 yaspin-2.4.0/examples/timer_spinner.py
+-rw-r--r--   0        0        0      452 2022-07-11 11:51:22.116125 yaspin-2.4.0/examples/write_method.py
+-rw-r--r--   0        0        0     2455 2023-08-06 12:43:09.750394 yaspin-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     7252 2023-08-06 12:43:09.750394 yaspin-2.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     3025 2022-07-19 10:41:34.977459 yaspin-2.4.0/tests/test_attrs.py
+-rw-r--r--   0        0        0      730 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_finalizers.py
+-rw-r--r--   0        0        0     7813 2023-02-26 15:11:07.365981 yaspin-2.4.0/tests/test_in_out.py
+-rw-r--r--   0        0        0     1507 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_pipes.py
+-rw-r--r--   0        0        0     3479 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_properties.py
+-rw-r--r--   0        0        0     2167 2022-07-19 10:41:34.979459 yaspin-2.4.0/tests/test_signals.py
+-rw-r--r--   0        0        0      695 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_spinners.py
+-rw-r--r--   0        0        0     1373 2022-07-11 11:51:22.128125 yaspin-2.4.0/tests/test_timer.py
+-rw-r--r--   0        0        0     1217 2023-08-06 12:02:54.704543 yaspin-2.4.0/tests/test_yaspin.py
+-rw-r--r--   0        0        0      218 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/__init__.py
+-rw-r--r--   0        0        0     2600 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/api.py
+-rw-r--r--   0        0        0      351 2023-08-06 12:02:54.704543 yaspin-2.4.0/yaspin/base_spinner.py
+-rw-r--r--   0        0        0     2749 2023-08-06 12:43:09.751394 yaspin-2.4.0/yaspin/constants.py
+-rw-r--r--   0        0        0    17974 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/core.py
+-rw-r--r--   0        0        0    26255 2023-08-06 12:43:09.751394 yaspin-2.4.0/yaspin/data/spinners.json
+-rw-r--r--   0        0        0      329 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/helpers.py
+-rw-r--r--   0        0        0     1065 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/signal_handlers.py
+-rw-r--r--   0        0        0      505 2023-08-06 12:02:54.705543 yaspin-2.4.0/yaspin/spinners.py
+-rw-r--r--   0        0        0    14175 1970-01-01 00:00:00.000000 yaspin-2.4.0/PKG-INFO
```

### Comparing `yaspin-2.3.0/HISTORY.rst` & `yaspin-2.4.0/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Release History
 ===============
 
+2.4.0 / 2023-08-06
+------------------
+
+* Add Python 3.12 support
+* Update cli-spinners to ``v2.9.0``
+* Update dependencies
+
+
 2.3.0 / 2023-01-06
 ------------------
 
 * Add Python 3.11 support (#217)
 * Simple type hints for better IDE completions (#214)
 * Replace ``termcolor-whl`` with renewed ``termcolor`` (#218)
 * Support new colors and highlights from ``termcolor`` v2.2.0 (#218)
```

### Comparing `yaspin-2.3.0/LICENSE` & `yaspin-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/README.rst` & `yaspin-2.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 .. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/shark.gif
 
 
 Features
 --------
 
-- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*), **PyPy**
+- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
 - Supports all (70+) spinners from `cli-spinners`_
 - Supports all *colors*, *highlights*, *attributes* and their mixes from `termcolor`_ library
 - Easy to combine with other command-line libraries, e.g. `prompt-toolkit`_
 - Flexible API, easy to integrate with existing code
 - User-friendly API for handling POSIX `signals`_
 - Safe **pipes** and **redirects**:
```

### Comparing `yaspin-2.3.0/examples/advanced_colors.py` & `yaspin-2.4.0/examples/advanced_colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/basic_usage.py` & `yaspin-2.4.0/examples/basic_usage.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/colors.py` & `yaspin-2.4.0/examples/colors.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/demo.py` & `yaspin-2.4.0/examples/demo.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/dynamic_text.py` & `yaspin-2.4.0/examples/dynamic_text.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/finalizers.py` & `yaspin-2.4.0/examples/finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/hide_show.py` & `yaspin-2.4.0/examples/hide_show.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/hide_show_prompt_toolkit.py` & `yaspin-2.4.0/examples/hide_show_prompt_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 print = print_formatted_text
 
 # build a basic prompt_toolkit style for styling the HTML wrapped text
 style = Style.from_dict({"msg": "#4caf50 bold", "sub-msg": "#616161 italic"})
 
 
 with yaspin(text="Downloading images") as sp:
-
     # task 1
     time.sleep(1)
     with sp.hidden():
         print(
             HTML("<b>></b> <msg>image 1</msg> <sub-msg>download complete</sub-msg>"),
             style=style,
         )
```

### Comparing `yaspin-2.3.0/examples/signals.py` & `yaspin-2.4.0/examples/signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/examples/spinner_properties.py` & `yaspin-2.4.0/examples/spinner_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/pyproject.toml` & `yaspin-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "yaspin"
-version = "2.3.0"
+version = "2.4.0"
 description = "Yet Another Terminal Spinner"
 license = "MIT"
-authors = ["Pavlo Dmytrenko <mail@pavdmyt.com>"]
+authors = ["Pavlo Dmytrenko <pavdmyt@aiven.io>"]
 readme = "README.rst"
 homepage = "https://github.com/pavdmyt/yaspin"
 repository = "https://github.com/pavdmyt/yaspin"
 documentation = "https://github.com/pavdmyt/yaspin/blob/master/README.rst"
 keywords = ["spinner", "console", "terminal", "loader", "indicator"]
 include = [
     { path = "tests", format = "sdist" },
@@ -31,14 +31,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: User Interfaces",
     "Topic :: System :: Logging",
@@ -49,22 +50,22 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 termcolor = "^2.2"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3"
+black = "^23.0"
 twine = "^4.0"
 flake8 = "^5.0"
 isort = "^5.10"
-pytest = "^7.1.2"
-pytest-xdist = "^2.5"
-pytest-cov = "^3.0"
-pylint = "^2.14"
+pytest = "^7.2"
+pytest-xdist = "^3.2"
+pytest-cov = "^4.0"
+pylint = "^2.16"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pavdmyt/yaspin/issues"
 "Changelog" = "https://github.com/pavdmyt/yaspin/releases"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `yaspin-2.3.0/tests/conftest.py` & `yaspin-2.4.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -139,14 +139,24 @@
         ("red", "red"),
         ("green", "green"),
         ("yellow", "yellow"),
         ("blue", "blue"),
         ("magenta", "magenta"),
         ("cyan", "cyan"),
         ("white", "white"),
+        # New highlights (from termcolor v2.2.0)
+        ("black", "black"),
+        ("dark_grey", "dark_grey"),
+        ("light_grey", "light_grey"),
+        ("light_red", "light_red"),
+        ("light_green", "light_green"),
+        ("light_yellow", "light_yellow"),
+        ("light_blue", "light_blue"),
+        ("light_magenta", "light_magenta"),
+        ("light_cyan", "light_cyan"),
         # Unsupported text colors
         ("Red", ValueError()),
         ("orange", ValueError()),
     ],
 )
 def color_test_cases(request):
     return request.param
@@ -163,14 +173,24 @@
         ("on_red", "on_red"),
         ("on_green", "on_green"),
         ("on_yellow", "on_yellow"),
         ("on_blue", "on_blue"),
         ("on_magenta", "on_magenta"),
         ("on_cyan", "on_cyan"),
         ("on_white", "on_white"),
+        # New highlights (from termcolor v2.2.0)
+        ("on_black", "on_black"),
+        ("on_dark_grey", "on_dark_grey"),
+        ("on_light_grey", "on_light_grey"),
+        ("on_light_red", "on_light_red"),
+        ("on_light_green", "on_light_green"),
+        ("on_light_yellow", "on_light_yellow"),
+        ("on_light_blue", "on_light_blue"),
+        ("on_light_magenta", "on_light_magenta"),
+        ("on_light_cyan", "on_light_cyan"),
         # Unsupported highlights
         ("on_foo", ValueError()),
     ],
 )
 def on_color_test_cases(request):
     return request.param
```

### Comparing `yaspin-2.3.0/tests/test_attrs.py` & `yaspin-2.4.0/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_finalizers.py` & `yaspin-2.4.0/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_in_out.py` & `yaspin-2.4.0/tests/test_in_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     sp.stop()
 
 
 @pytest.mark.parametrize(
     "obj, obj_str",
     [
         ("foo", "foo"),
-        (dict(cat="meow"), "{'cat': 'meow'}"),
+        ({"cat": "meow"}, "{'cat': 'meow'}"),
         (23, "23"),
         (["foo", "bar", "'", 23], """['foo', 'bar', "'", 23]"""),
     ],
 )
 def test_write_non_str_objects(monkeypatch, capsys, obj, obj_str, isatty_fixture):
     monkeypatch.setattr(sys.stdout, "isatty", lambda: isatty_fixture)
     sp = yaspin()
```

### Comparing `yaspin-2.3.0/tests/test_pipes.py` & `yaspin-2.4.0/tests/test_pipes.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_properties.py` & `yaspin-2.4.0/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_signals.py` & `yaspin-2.4.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_spinners.py` & `yaspin-2.4.0/tests/test_spinners.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_timer.py` & `yaspin-2.4.0/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/tests/test_yaspin.py` & `yaspin-2.4.0/tests/test_yaspin.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/yaspin/api.py` & `yaspin-2.4.0/yaspin/api.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/yaspin/constants.py` & `yaspin-2.4.0/yaspin/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     "arc",
     "arrow",
     "arrow2",
     "arrow3",
     "balloon",
     "balloon2",
     "betaWave",
+    "binary",
     "bluePulse",
     "bounce",
     "bouncingBall",
     "bouncingBar",
     "boxBounce",
     "boxBounce2",
     "christmas",
@@ -88,14 +89,15 @@
     "dots5",
     "dots6",
     "dots7",
     "dots8",
     "dots8Bit",
     "dots9",
     "dqpb",
+    "dwarfFortress",
     "earth",
     "fingerDance",
     "fistBump",
     "flip",
     "grenade",
     "growHorizontal",
     "growVertical",
```

### Comparing `yaspin-2.3.0/yaspin/core.py` & `yaspin-2.4.0/yaspin/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,14 @@
         self.stop()
         with self._stdout_lock:
             sys.stdout.write(self._last_frame)
             self._cur_line_len = 0
 
     def _spin(self):
         while not self._stop_spin.is_set():
-
             if self._hide_spin.is_set():
                 # Wait a bit to avoid wasting cycles
                 time.sleep(self._interval)
                 continue
 
             # Compose output
             spin_phase = next(self._cycle)
@@ -515,15 +514,14 @@
         uframes_seq = None  # sequence of unicode frames
 
         if isinstance(spinner.frames, str):
             uframes = spinner.frames
 
         # TODO (pavdmyt): support any type that implements iterable
         if isinstance(spinner.frames, (list, tuple)):
-
             # Empty ``spinner.frames`` is handled by ``Yaspin._set_spinner``
             if spinner.frames and isinstance(spinner.frames[0], bytes):
                 uframes_seq = [to_unicode(frame) for frame in spinner.frames]
             else:
                 uframes_seq = spinner.frames
 
         _frames = uframes or uframes_seq
```

### Comparing `yaspin-2.3.0/yaspin/signal_handlers.py` & `yaspin-2.4.0/yaspin/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `yaspin-2.3.0/setup.py` & `yaspin-2.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,518 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: yaspin
+Version: 2.4.0
+Summary: Yet Another Terminal Spinner
+Home-page: https://github.com/pavdmyt/yaspin
+License: MIT
+Keywords: spinner,console,terminal,loader,indicator
+Author: Pavlo Dmytrenko
+Author-email: pavdmyt@aiven.io
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Other Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: System :: Logging
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
+Classifier: Topic :: Utilities
+Requires-Dist: termcolor (>=2.2,<3.0)
+Project-URL: Bug Tracker, https://github.com/pavdmyt/yaspin/issues
+Project-URL: Changelog, https://github.com/pavdmyt/yaspin/releases
+Project-URL: Documentation, https://github.com/pavdmyt/yaspin/blob/master/README.rst
+Project-URL: Repository, https://github.com/pavdmyt/yaspin
+Description-Content-Type: text/x-rst
 
-packages = \
-['yaspin']
+|Logo|
 
-package_data = \
-{'': ['*'], 'yaspin': ['data/*']}
+=====================================================================
+``yaspin``: **Y**\ et **A**\ nother Terminal **Spin**\ ner for Python
+=====================================================================
 
-install_requires = \
-['termcolor>=2.2,<3.0']
-
-setup_kwargs = {
-    'name': 'yaspin',
-    'version': '2.3.0',
-    'description': 'Yet Another Terminal Spinner',
-    'long_description': '|Logo|\n\n=====================================================================\n``yaspin``: **Y**\\ et **A**\\ nother Terminal **Spin**\\ ner for Python\n=====================================================================\n\n|Coverage| |pypi| |black-fmt|\n\n|Versions| |Wheel| |Examples|\n\n|DownloadsTot| |DownloadsW|\n\n\n``Yaspin`` provides a full-featured terminal spinner to show the progress during long-hanging operations.\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/demo.gif\n\nIt is easy to integrate into existing codebase by using it as a `context manager`_\nor as a function `decorator`_:\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    # Context manager:\n    with yaspin():\n        time.sleep(3)  # time consuming code\n\n    # Function decorator:\n    @yaspin(text="Loading...")\n    def some_operations():\n        time.sleep(3)  # time consuming code\n\n    some_operations()\n\n\n**Yaspin** also provides an intuitive and powerful API. For example, you can easily summon a shark:\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    with yaspin().white.bold.shark.on_blue as sp:\n        sp.text = "White bold shark in a blue sea"\n        time.sleep(5)\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/shark.gif\n\n\nFeatures\n--------\n\n- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*), **PyPy**\n- Supports all (70+) spinners from `cli-spinners`_\n- Supports all *colors*, *highlights*, *attributes* and their mixes from `termcolor`_ library\n- Easy to combine with other command-line libraries, e.g. `prompt-toolkit`_\n- Flexible API, easy to integrate with existing code\n- User-friendly API for handling POSIX `signals`_\n- Safe **pipes** and **redirects**:\n\n.. code-block:: bash\n\n    $ python script_that_uses_yaspin.py > script.log\n    $ python script_that_uses_yaspin.py | grep ERROR\n\n\nInstallation\n------------\n\nFrom `PyPI`_ using ``pip`` package manager:\n\n.. code-block:: bash\n\n    pip install --upgrade yaspin\n\n\nOr install the latest sources from GitHub:\n\n.. code-block:: bash\n\n    pip install https://github.com/pavdmyt/yaspin/archive/master.zip\n\n\nUsage\n-----\n\nBasic Example\n/////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/basic_example.gif\n\n.. code:: python\n\n    import time\n    from random import randint\n    from yaspin import yaspin\n\n    with yaspin(text="Loading", color="yellow") as spinner:\n        time.sleep(2)  # time consuming code\n\n        success = randint(0, 1)\n        if success:\n            spinner.ok("✅ ")\n        else:\n            spinner.fail("💥 ")\n\n\nIt is also possible to control spinner manually:\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    spinner = yaspin()\n    spinner.start()\n\n    time.sleep(3)  # time consuming tasks\n\n    spinner.stop()\n\n\nRun any spinner from `cli-spinners`_\n////////////////////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/cli_spinners.gif\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n    from yaspin.spinners import Spinners\n\n    with yaspin(Spinners.earth, text="Earth") as sp:\n        time.sleep(2)                # time consuming code\n\n        # change spinner\n        sp.spinner = Spinners.moon\n        sp.text = "Moon"\n\n        time.sleep(2)                # time consuming code\n\n\nAny Colour You Like `🌈`_\n/////////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/basic_colors.gif\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    with yaspin(text="Colors!") as sp:\n        # Support all basic termcolor text colors\n        colors = ("red", "green", "yellow", "blue", "magenta", "cyan", "white")\n\n        for color in colors:\n            sp.color, sp.text = color, color\n            time.sleep(1)\n\n\nAdvanced colors usage\n/////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/advanced_colors.gif\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n    from yaspin.spinners import Spinners\n\n    text = "Bold blink magenta spinner on cyan color"\n    with yaspin().bold.blink.magenta.bouncingBall.on_cyan as sp:\n        sp.text = text\n        time.sleep(3)\n\n    # The same result can be achieved by passing arguments directly\n    with yaspin(\n        Spinners.bouncingBall,\n        color="magenta",\n        on_color="on_cyan",\n        attrs=["bold", "blink"],\n    ) as sp:\n        sp.text = text\n        time.sleep(3)\n\n\nRun any spinner you want\n////////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/custom_spinners.gif\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin, Spinner\n\n    # Compose new spinners with custom frame sequence and interval value\n    sp = Spinner(["😸", "😹", "😺", "😻", "😼", "😽", "😾", "😿", "🙀"], 200)\n\n    with yaspin(sp, text="Cat!"):\n        time.sleep(3)  # cat consuming code :)\n\n\nChange spinner properties on the fly\n////////////////////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/sp_properties.gif\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n    from yaspin.spinners import Spinners\n\n    with yaspin(Spinners.noise, text="Noise spinner") as sp:\n        time.sleep(2)\n\n        sp.spinner = Spinners.arc  # spinner type\n        sp.text = "Arc spinner"    # text along with spinner\n        sp.color = "green"         # spinner color\n        sp.side = "right"          # put spinner to the right\n        sp.reversal = True         # reverse spin direction\n\n        time.sleep(2)\n\n\nSpinner with timer\n//////////////////\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    with yaspin(text="elapsed time", timer=True) as sp:\n        time.sleep(3.1415)\n        sp.ok()\n\n\nDynamic text\n////////////\n\n.. code:: python\n\n    import time\n    from datetime import datetime\n    from yaspin import yaspin\n\n    class TimedText:\n        def __init__(self, text):\n            self.text = text\n            self._start = datetime.now()\n\n        def __str__(self):\n            now = datetime.now()\n            delta = now - self._start\n            return f"{self.text} ({round(delta.total_seconds(), 1)}s)"\n\n    with yaspin(text=TimedText("time passed:")):\n        time.sleep(3)\n\n\nWriting messages\n////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/write_text.gif\n\nYou should not write any message in the terminal using ``print`` while spinner is open.\nTo write messages in the terminal without any collision with ``yaspin`` spinner, a ``.write()`` method is provided:\n\n.. code:: python\n\n    import time\n    from yaspin import yaspin\n\n    with yaspin(text="Downloading images", color="cyan") as sp:\n        # task 1\n        time.sleep(1)\n        sp.write("> image 1 download complete")\n\n        # task 2\n        time.sleep(2)\n        sp.write("> image 2 download complete")\n\n        # finalize\n        sp.ok("✔")\n\n\nIntegration with other libraries\n////////////////////////////////\n\n.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/hide_show.gif\n\nUtilizing ``hidden`` context manager it is possible to toggle the display of\nthe spinner in order to call custom methods that write to the terminal. This is\nhelpful for allowing easy usage in other frameworks like `prompt-toolkit`_.\nUsing the powerful ``print_formatted_text`` function allows you even to apply\nHTML formats and CSS styles to the output:\n\n.. code:: python\n\n    import sys\n    import time\n\n    from yaspin import yaspin\n    from prompt_toolkit import HTML, print_formatted_text\n    from prompt_toolkit.styles import Style\n\n    # override print with feature-rich ``print_formatted_text`` from prompt_toolkit\n    print = print_formatted_text\n\n    # build a basic prompt_toolkit style for styling the HTML wrapped text\n    style = Style.from_dict({\n        \'msg\': \'#4caf50 bold\',\n        \'sub-msg\': \'#616161 italic\'\n    })\n\n\n    with yaspin(text=\'Downloading images\') as sp:\n        # task 1\n        time.sleep(1)\n        with sp.hidden():\n            print(HTML(\n                u\'<b>></b> <msg>image 1</msg> <sub-msg>download complete</sub-msg>\'\n            ), style=style)\n\n        # task 2\n        time.sleep(2)\n        with sp.hidden():\n            print(HTML(\n                u\'<b>></b> <msg>image 2</msg> <sub-msg>download complete</sub-msg>\'\n            ), style=style)\n\n        # finalize\n        sp.ok()\n\n\nHandling POSIX `signals`_\n/////////////////////////\n\nHandling keyboard interrupts (pressing Control-C):\n\n.. code:: python\n\n    import time\n\n    from yaspin import kbi_safe_yaspin\n\n\n    with kbi_safe_yaspin(text="Press Control+C to send SIGINT (Keyboard Interrupt) signal"):\n        time.sleep(5)  # time consuming code\n\n\nHandling other types of signals:\n\n.. code:: python\n\n    import os\n    import time\n    from signal import SIGTERM, SIGUSR1\n\n    from yaspin import yaspin\n    from yaspin.signal_handlers import default_handler, fancy_handler\n\n\n    sigmap = {SIGUSR1: default_handler, SIGTERM: fancy_handler}\n    with yaspin(sigmap=sigmap, text="Handling SIGUSR1 and SIGTERM signals") as sp:\n        sp.write("Send signals using `kill` command")\n        sp.write("E.g. $ kill -USR1 {0}".format(os.getpid()))\n        time.sleep(20)  # time consuming code\n\n\nMore `examples`_.\n\n\nDevelopment\n-----------\n\nClone the repository:\n\n.. code-block:: bash\n\n    git clone https://github.com/pavdmyt/yaspin.git\n\n\nInstall dev dependencies:\n\n.. code-block:: bash\n\n    poetry install\n\n    # if you don\'t have poetry installed:\n    pip install -r requirements.txt\n\n\nLint code:\n\n.. code-block:: bash\n\n    make lint\n\n\nFormat code:\n\n.. code-block:: bash\n\n    make black-fmt\n\n\nRun tests:\n\n.. code-block:: bash\n\n    make test\n\n\nContributing\n------------\n\n1. Fork it!\n2. Create your feature branch: ``git checkout -b my-new-feature``\n3. Commit your changes: ``git commit -m \'Add some feature\'``\n4. Push to the branch: ``git push origin my-new-feature``\n5. Submit a pull request\n6. Make sure tests are passing\n\n\nLicense\n-------\n\n* MIT - Pavlo Dmytrenko; https://twitter.com/pavdmyt\n* Contains data from `cli-spinners`_: MIT License, Copyright (c) Sindre Sorhus sindresorhus@gmail.com (sindresorhus.com)\n\n\n.. |Logo| image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/static/logo_80.png\n   :alt: yaspin Logo\n.. |Coverage| image:: https://codecov.io/gh/pavdmyt/yaspin/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/pavdmyt/yaspin\n.. |pypi| image:: https://img.shields.io/pypi/v/yaspin.svg\n   :target: https://pypi.org/project/yaspin/\n.. |Versions| image:: https://img.shields.io/pypi/pyversions/yaspin.svg\n   :target: https://pypi.org/project/yaspin/\n.. |Wheel| image:: https://img.shields.io/pypi/wheel/yaspin.svg\n   :target: https://pypi.org/project/yaspin/\n.. |Examples| image:: https://img.shields.io/badge/learn%20by-examples-0077b3.svg\n   :target: https://github.com/pavdmyt/yaspin/tree/master/examples\n.. |black-fmt| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/ambv/black\n.. |DownloadsTot| image:: https://pepy.tech/badge/yaspin\n   :target: https://pepy.tech/project/yaspin\n.. |DownloadsW| image:: https://pepy.tech/badge/yaspin/week\n   :target: https://pepy.tech/project/yaspin\n\n\n.. _context manager: https://docs.python.org/3/reference/datamodel.html#context-managers\n.. _decorator: https://www.thecodeship.com/patterns/guide-to-python-function-decorators/\n.. _cli-spinners: https://github.com/sindresorhus/cli-spinners\n.. _termcolor: https://pypi.org/project/termcolor/\n.. _PyPI: https://pypi.org/\n.. _🌈: https://en.wikipedia.org/wiki/Any_Colour_You_Like\n.. _examples: https://github.com/pavdmyt/yaspin/tree/master/examples\n.. _prompt-toolkit: https://github.com/jonathanslenders/python-prompt-toolkit/\n.. _signals: https://www.computerhope.com/unix/signals.htm\n',
-    'author': 'Pavlo Dmytrenko',
-    'author_email': 'mail@pavdmyt.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pavdmyt/yaspin',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+|Coverage| |pypi| |black-fmt|
 
+|Versions| |Wheel| |Examples|
+
+|DownloadsTot| |DownloadsW|
+
+
+``Yaspin`` provides a full-featured terminal spinner to show the progress during long-hanging operations.
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/demo.gif
+
+It is easy to integrate into existing codebase by using it as a `context manager`_
+or as a function `decorator`_:
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    # Context manager:
+    with yaspin():
+        time.sleep(3)  # time consuming code
+
+    # Function decorator:
+    @yaspin(text="Loading...")
+    def some_operations():
+        time.sleep(3)  # time consuming code
+
+    some_operations()
+
+
+**Yaspin** also provides an intuitive and powerful API. For example, you can easily summon a shark:
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    with yaspin().white.bold.shark.on_blue as sp:
+        sp.text = "White bold shark in a blue sea"
+        time.sleep(5)
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/shark.gif
+
+
+Features
+--------
+
+- Runs at all major **CPython** versions (*3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*), **PyPy**
+- Supports all (70+) spinners from `cli-spinners`_
+- Supports all *colors*, *highlights*, *attributes* and their mixes from `termcolor`_ library
+- Easy to combine with other command-line libraries, e.g. `prompt-toolkit`_
+- Flexible API, easy to integrate with existing code
+- User-friendly API for handling POSIX `signals`_
+- Safe **pipes** and **redirects**:
+
+.. code-block:: bash
+
+    $ python script_that_uses_yaspin.py > script.log
+    $ python script_that_uses_yaspin.py | grep ERROR
+
+
+Installation
+------------
+
+From `PyPI`_ using ``pip`` package manager:
+
+.. code-block:: bash
+
+    pip install --upgrade yaspin
+
+
+Or install the latest sources from GitHub:
+
+.. code-block:: bash
+
+    pip install https://github.com/pavdmyt/yaspin/archive/master.zip
+
+
+Usage
+-----
+
+Basic Example
+/////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/basic_example.gif
+
+.. code:: python
+
+    import time
+    from random import randint
+    from yaspin import yaspin
+
+    with yaspin(text="Loading", color="yellow") as spinner:
+        time.sleep(2)  # time consuming code
+
+        success = randint(0, 1)
+        if success:
+            spinner.ok("✅ ")
+        else:
+            spinner.fail("💥 ")
+
+
+It is also possible to control spinner manually:
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    spinner = yaspin()
+    spinner.start()
+
+    time.sleep(3)  # time consuming tasks
+
+    spinner.stop()
+
+
+Run any spinner from `cli-spinners`_
+////////////////////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/cli_spinners.gif
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+    from yaspin.spinners import Spinners
+
+    with yaspin(Spinners.earth, text="Earth") as sp:
+        time.sleep(2)                # time consuming code
+
+        # change spinner
+        sp.spinner = Spinners.moon
+        sp.text = "Moon"
+
+        time.sleep(2)                # time consuming code
+
+
+Any Colour You Like `🌈`_
+/////////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/basic_colors.gif
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    with yaspin(text="Colors!") as sp:
+        # Support all basic termcolor text colors
+        colors = ("red", "green", "yellow", "blue", "magenta", "cyan", "white")
+
+        for color in colors:
+            sp.color, sp.text = color, color
+            time.sleep(1)
+
+
+Advanced colors usage
+/////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/advanced_colors.gif
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+    from yaspin.spinners import Spinners
+
+    text = "Bold blink magenta spinner on cyan color"
+    with yaspin().bold.blink.magenta.bouncingBall.on_cyan as sp:
+        sp.text = text
+        time.sleep(3)
+
+    # The same result can be achieved by passing arguments directly
+    with yaspin(
+        Spinners.bouncingBall,
+        color="magenta",
+        on_color="on_cyan",
+        attrs=["bold", "blink"],
+    ) as sp:
+        sp.text = text
+        time.sleep(3)
+
+
+Run any spinner you want
+////////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/custom_spinners.gif
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin, Spinner
+
+    # Compose new spinners with custom frame sequence and interval value
+    sp = Spinner(["😸", "😹", "😺", "😻", "😼", "😽", "😾", "😿", "🙀"], 200)
+
+    with yaspin(sp, text="Cat!"):
+        time.sleep(3)  # cat consuming code :)
+
+
+Change spinner properties on the fly
+////////////////////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/sp_properties.gif
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+    from yaspin.spinners import Spinners
+
+    with yaspin(Spinners.noise, text="Noise spinner") as sp:
+        time.sleep(2)
+
+        sp.spinner = Spinners.arc  # spinner type
+        sp.text = "Arc spinner"    # text along with spinner
+        sp.color = "green"         # spinner color
+        sp.side = "right"          # put spinner to the right
+        sp.reversal = True         # reverse spin direction
+
+        time.sleep(2)
+
+
+Spinner with timer
+//////////////////
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    with yaspin(text="elapsed time", timer=True) as sp:
+        time.sleep(3.1415)
+        sp.ok()
+
+
+Dynamic text
+////////////
+
+.. code:: python
+
+    import time
+    from datetime import datetime
+    from yaspin import yaspin
+
+    class TimedText:
+        def __init__(self, text):
+            self.text = text
+            self._start = datetime.now()
+
+        def __str__(self):
+            now = datetime.now()
+            delta = now - self._start
+            return f"{self.text} ({round(delta.total_seconds(), 1)}s)"
+
+    with yaspin(text=TimedText("time passed:")):
+        time.sleep(3)
+
+
+Writing messages
+////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/write_text.gif
+
+You should not write any message in the terminal using ``print`` while spinner is open.
+To write messages in the terminal without any collision with ``yaspin`` spinner, a ``.write()`` method is provided:
+
+.. code:: python
+
+    import time
+    from yaspin import yaspin
+
+    with yaspin(text="Downloading images", color="cyan") as sp:
+        # task 1
+        time.sleep(1)
+        sp.write("> image 1 download complete")
+
+        # task 2
+        time.sleep(2)
+        sp.write("> image 2 download complete")
+
+        # finalize
+        sp.ok("✔")
+
+
+Integration with other libraries
+////////////////////////////////
+
+.. image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/gifs/hide_show.gif
+
+Utilizing ``hidden`` context manager it is possible to toggle the display of
+the spinner in order to call custom methods that write to the terminal. This is
+helpful for allowing easy usage in other frameworks like `prompt-toolkit`_.
+Using the powerful ``print_formatted_text`` function allows you even to apply
+HTML formats and CSS styles to the output:
+
+.. code:: python
+
+    import sys
+    import time
+
+    from yaspin import yaspin
+    from prompt_toolkit import HTML, print_formatted_text
+    from prompt_toolkit.styles import Style
+
+    # override print with feature-rich ``print_formatted_text`` from prompt_toolkit
+    print = print_formatted_text
+
+    # build a basic prompt_toolkit style for styling the HTML wrapped text
+    style = Style.from_dict({
+        'msg': '#4caf50 bold',
+        'sub-msg': '#616161 italic'
+    })
+
+
+    with yaspin(text='Downloading images') as sp:
+        # task 1
+        time.sleep(1)
+        with sp.hidden():
+            print(HTML(
+                u'<b>></b> <msg>image 1</msg> <sub-msg>download complete</sub-msg>'
+            ), style=style)
+
+        # task 2
+        time.sleep(2)
+        with sp.hidden():
+            print(HTML(
+                u'<b>></b> <msg>image 2</msg> <sub-msg>download complete</sub-msg>'
+            ), style=style)
+
+        # finalize
+        sp.ok()
+
+
+Handling POSIX `signals`_
+/////////////////////////
+
+Handling keyboard interrupts (pressing Control-C):
+
+.. code:: python
+
+    import time
+
+    from yaspin import kbi_safe_yaspin
+
+
+    with kbi_safe_yaspin(text="Press Control+C to send SIGINT (Keyboard Interrupt) signal"):
+        time.sleep(5)  # time consuming code
+
+
+Handling other types of signals:
+
+.. code:: python
+
+    import os
+    import time
+    from signal import SIGTERM, SIGUSR1
+
+    from yaspin import yaspin
+    from yaspin.signal_handlers import default_handler, fancy_handler
+
+
+    sigmap = {SIGUSR1: default_handler, SIGTERM: fancy_handler}
+    with yaspin(sigmap=sigmap, text="Handling SIGUSR1 and SIGTERM signals") as sp:
+        sp.write("Send signals using `kill` command")
+        sp.write("E.g. $ kill -USR1 {0}".format(os.getpid()))
+        time.sleep(20)  # time consuming code
+
+
+More `examples`_.
+
+
+Development
+-----------
+
+Clone the repository:
+
+.. code-block:: bash
+
+    git clone https://github.com/pavdmyt/yaspin.git
+
+
+Install dev dependencies:
+
+.. code-block:: bash
+
+    poetry install
+
+    # if you don't have poetry installed:
+    pip install -r requirements.txt
+
+
+Lint code:
+
+.. code-block:: bash
+
+    make lint
+
+
+Format code:
+
+.. code-block:: bash
+
+    make black-fmt
+
+
+Run tests:
+
+.. code-block:: bash
+
+    make test
+
+
+Contributing
+------------
+
+1. Fork it!
+2. Create your feature branch: ``git checkout -b my-new-feature``
+3. Commit your changes: ``git commit -m 'Add some feature'``
+4. Push to the branch: ``git push origin my-new-feature``
+5. Submit a pull request
+6. Make sure tests are passing
+
+
+License
+-------
+
+* MIT - Pavlo Dmytrenko; https://twitter.com/pavdmyt
+* Contains data from `cli-spinners`_: MIT License, Copyright (c) Sindre Sorhus sindresorhus@gmail.com (sindresorhus.com)
+
+
+.. |Logo| image:: https://raw.githubusercontent.com/pavdmyt/yaspin/master/static/logo_80.png
+   :alt: yaspin Logo
+.. |Coverage| image:: https://codecov.io/gh/pavdmyt/yaspin/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/pavdmyt/yaspin
+.. |pypi| image:: https://img.shields.io/pypi/v/yaspin.svg
+   :target: https://pypi.org/project/yaspin/
+.. |Versions| image:: https://img.shields.io/pypi/pyversions/yaspin.svg
+   :target: https://pypi.org/project/yaspin/
+.. |Wheel| image:: https://img.shields.io/pypi/wheel/yaspin.svg
+   :target: https://pypi.org/project/yaspin/
+.. |Examples| image:: https://img.shields.io/badge/learn%20by-examples-0077b3.svg
+   :target: https://github.com/pavdmyt/yaspin/tree/master/examples
+.. |black-fmt| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/ambv/black
+.. |DownloadsTot| image:: https://pepy.tech/badge/yaspin
+   :target: https://pepy.tech/project/yaspin
+.. |DownloadsW| image:: https://pepy.tech/badge/yaspin/week
+   :target: https://pepy.tech/project/yaspin
+
+
+.. _context manager: https://docs.python.org/3/reference/datamodel.html#context-managers
+.. _decorator: https://www.thecodeship.com/patterns/guide-to-python-function-decorators/
+.. _cli-spinners: https://github.com/sindresorhus/cli-spinners
+.. _termcolor: https://pypi.org/project/termcolor/
+.. _PyPI: https://pypi.org/
+.. _🌈: https://en.wikipedia.org/wiki/Any_Colour_You_Like
+.. _examples: https://github.com/pavdmyt/yaspin/tree/master/examples
+.. _prompt-toolkit: https://github.com/jonathanslenders/python-prompt-toolkit/
+.. _signals: https://www.computerhope.com/unix/signals.htm
 
-setup(**setup_kwargs)
```

