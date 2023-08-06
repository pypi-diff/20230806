# Comparing `tmp/tko-0.0.2.tar.gz` & `tmp/tko-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.0.2.tar", last modified: Thu Aug  3 15:57:38 2023, max compression
+gzip compressed data, was "tko-0.0.3.tar", last modified: Sat Aug  5 18:54:53 2023, max compression
```

## Comparing `tko-0.0.2.tar` & `tko-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-03 15:57:38.010346 tko-0.0.2/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.0.2/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.0.2/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2137 2023-08-03 15:57:38.013679 tko-0.0.2/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1422 2023-08-03 13:41:19.000000 tko-0.0.2/README.md
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-03 15:57:37.983678 tko-0.0.2/data/
--rw-r--r--   0 lion      (1000) lion      (1000)        9 2023-08-02 17:33:10.000000 tko-0.0.2/data/data_file
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.0.2/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2023-08-03 15:57:38.013679 tko-0.0.2/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3996 2023-08-03 14:43:47.000000 tko-0.0.2/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-03 15:57:37.980345 tko-0.0.2/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-03 15:57:38.000345 tko-0.0.2/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       21 2023-08-03 15:57:06.000000 tko-0.0.2/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6049 2023-08-03 03:37:09.000000 tko-0.0.2/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2772 2023-08-03 03:29:06.000000 tko-0.0.2/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1919 2023-08-03 03:29:06.000000 tko-0.0.2/src/tko/colored.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6806 2023-08-03 03:34:25.000000 tko-0.0.2/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5399 2023-08-03 03:35:52.000000 tko-0.0.2/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1015 2023-08-03 03:36:19.000000 tko-0.0.2/src/tko/enums.py
--rw-r--r--   0 lion      (1000) lion      (1000)      751 2023-08-03 03:36:30.000000 tko-0.0.2/src/tko/execution.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1169 2023-08-03 03:37:25.000000 tko-0.0.2/src/tko/label_factory.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5251 2023-08-03 03:38:28.000000 tko-0.0.2/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1330 2023-08-03 03:38:47.000000 tko-0.0.2/src/tko/param.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.0.2/src/tko/pattern_loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)      842 2023-08-03 03:40:33.000000 tko-0.0.2/src/tko/replacer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1212 2023-08-03 03:40:57.000000 tko-0.0.2/src/tko/report.py
--rw-r--r--   0 lion      (1000) lion      (1000)      643 2023-08-03 03:41:05.000000 tko-0.0.2/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1045 2023-08-03 03:41:19.000000 tko-0.0.2/src/tko/settings_parser.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5214 2023-08-03 15:54:07.000000 tko-0.0.2/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1619 2023-08-03 03:46:14.000000 tko-0.0.2/src/tko/symbol.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1274 2023-08-03 03:46:14.000000 tko-0.0.2/src/tko/unit.py
--rw-r--r--   0 lion      (1000) lion      (1000)      392 2023-08-03 03:46:39.000000 tko-0.0.2/src/tko/util.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2983 2023-08-03 03:47:04.000000 tko-0.0.2/src/tko/vpl_parser.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5379 2023-08-03 03:48:30.000000 tko-0.0.2/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3198 2023-08-03 03:50:26.000000 tko-0.0.2/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-03 15:57:38.010346 tko-0.0.2/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2137 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      709 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2023-08-03 15:57:37.000000 tko-0.0.2/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.059576 tko-0.0.3/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.0.3/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.0.3/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-05 18:54:53.059576 tko-0.0.3/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      422 2023-08-05 18:49:31.000000 tko-0.0.3/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.0.3/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2023-08-05 18:54:53.059576 tko-0.0.3/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3982 2023-08-05 15:02:11.000000 tko-0.0.3/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.046242 tko-0.0.3/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.052909 tko-0.0.3/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2023-08-05 18:54:13.000000 tko-0.0.3/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6596 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3330 2023-08-05 18:23:50.000000 tko-0.0.3/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3569 2023-08-05 17:47:30.000000 tko-0.0.3/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6767 2023-08-05 17:57:03.000000 tko-0.0.3/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5186 2023-08-05 17:51:49.000000 tko-0.0.3/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4684 2023-08-05 16:55:34.000000 tko-0.0.3/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8151 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.0.3/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      594 2023-08-05 17:03:33.000000 tko-0.0.3/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1222 2023-08-05 16:47:30.000000 tko-0.0.3/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5223 2023-08-05 17:49:27.000000 tko-0.0.3/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6480 2023-08-05 17:50:47.000000 tko-0.0.3/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3174 2023-08-05 18:09:28.000000 tko-0.0.3/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2023-08-05 18:54:53.056242 tko-0.0.3/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1137 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      506 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2023-08-05 18:54:53.000000 tko-0.0.3/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.0.2/LICENSE` & `tko-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.0.2/setup.py` & `tko-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,22 @@
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example: $ pip install sampleproject[dev]
     # Similar to `install_requires` above, these must be valid existing projects
     extras_require={'dev': ['check-manifest'],
                     'test': ['coverage'],
                     },  # Optional
 
-    package_data={'tko': ['package_data.dat'],
-                  },  # Optional, Data files included in your packages that need to be installed
+    #package_data={'tko': ['data/settings.cfg'], },  # Optional, Data files included in your packages that need to be installed
 
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    data_files=[('my_data', ['data/data_file'])],  # Optional
+    # data_files=[('my_data', ['data/data_file'])],  # Optional
 
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `ultralytics` which
```

### Comparing `tko-0.0.2/src/tko/__main__.py` & `tko-0.0.3/src/tko/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Console scripts
 
 import argparse
 import sys
 
 from .actions import Actions
-from .param import Param
-from .pattern_loader import PatternLoader
-from .enums import DiffMode
-from .report import Report
+from .basic import Param
+from .pattern import PatternLoader
+from .basic import DiffMode
+from .format import Report
 from .down import Down
+from .settings import SettingsParser
 
 
 class Main:
     @staticmethod
     def execute(args):
         Actions.exec(args.target_list)
 
@@ -22,35 +23,35 @@
             Report.set_terminal_size(args.width)
         PatternLoader.pattern = args.pattern
         param = Param.Basic().set_index(args.index)
         if args.quiet:
             param.set_diff_mode(DiffMode.QUIET)
         if args.vertical:
             param.set_up_down(True)
-        if Actions.run(args.target_list, param):
-            return 0
-        return 1
+        Actions.run(args.target_list, param)
 
     @staticmethod
     def list(args):
         if args.width is not None:
             Report.set_terminal_size(args.width)
         PatternLoader.pattern = args.pattern
         param = Param.Basic().set_index(args.index)
         Actions.list(args.target_list, param)
-        return 0
 
     @staticmethod
     def build(args):
         if args.width is not None:
             Report.set_terminal_size(args.width)
         PatternLoader.pattern = args.pattern
         manip = Param.Manip().set_unlabel(args.unlabel).set_to_sort(args.sort).set_to_number(args.number)
         Actions.build(args.target, args.target_list, manip, args.force)
-        return 0
+    
+    @staticmethod
+    def settings(args):
+        print("settings file at " + SettingsParser().get_settings_file())
 
     # @staticmethod
     # def rebuild(args):
     #     if args.width is not None:
     #         Report.set_terminal_size(args.width)
     #     PatternLoader.pattern = args.pattern
     #     manip = Param.Manip().set_unlabel(args.unlabel).set_to_sort(args.sort).set_to_number(args.number)
@@ -58,16 +59,22 @@
     #     return 0
 
     @staticmethod
     def update(_args):
         Down.update()
 
     @staticmethod
+    def down(args):
+        destiny = Down.create_problem_folder(args.disc, args.index, args.extension)
+        Down.entry_unpack(destiny, args.disc, args.index, args.extension)
+
+    @staticmethod
     def main():
         parent_basic = argparse.ArgumentParser(add_help=False)
+        # parent_basic.add_argument('--version', '-v', action='version', help='show version.')
         parent_basic.add_argument('--width', '-w', type=int, help="term width")
         parent_basic.add_argument('--index', '-i', metavar="I", type=int, help='run a specific index.')
         parent_basic.add_argument('--pattern', '-p', metavar="P", type=str, default='@.in @.sol',
                                   help='pattern load/save a folder, default: "@.in @.sol"')
 
         parent_manip = argparse.ArgumentParser(add_help=False)
         parent_manip.add_argument('--width', '-w', type=int, help="term width.")
@@ -111,28 +118,34 @@
         # parser_rb.set_defaults(func=Main.rebuild)
 
         # down
         parser_d = subparsers.add_parser('down', help='download test from remote repository.')
         parser_d.add_argument('disc', type=str, help=" [ fup | ed | poo ]")
         parser_d.add_argument('index', type=str, help="3 digits label like 021")
         parser_d.add_argument('extension', type=str, nargs = '?', default = "-", help="[ c | cpp | js | ts | py | java ]")
-        parser_d.set_defaults(func=Down.entry_args)
+        parser_d.set_defaults(func=Main.down)
 
         # update
         parser_u = subparsers.add_parser('update', help='update problem from repository.')
         parser_u.set_defaults(func=Main.update)
 
+        # settings
+        parser_s = subparsers.add_parser('settings', help='show settings.')
+        parser_s.set_defaults(func=Main.settings)
+
         args = parser.parse_args()
         if len(sys.argv) == 1:
             print("You must call a subcommand. Use --help for more information.")
         else:
             try:
                 args.func(args)
             except ValueError as e:
                 print(str(e))
 
 
 if __name__ == '__main__':
     try:
         Main.main()
+        sys.exit(0)
     except KeyboardInterrupt:
         print("\n\nKeyboard Interrupt")
+        sys.exit(1)
```

### Comparing `tko-0.0.2/src/tko/actions.py` & `tko-0.0.3/src/tko/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 from typing import List
 import subprocess
 
-from .param import Param
-from .runner import Runner
 from .wdir import Wdir
-from .execution import Execution
-from .enums import DiffMode, ExecutionResult
+from .basic import DiffMode, ExecutionResult, CompilerError, Param, Unit
 from .diff import Diff
-from .colored import Colored, Color
-from .report import Report
-from .symbol import Symbol
+from .format import Symbol, Colored, Color, Report
 from .writer import Writer
+from .solver import Solver
+from .runner import Runner
+
+
+
+class Execution:
+
+    def __init__(self):
+        pass
+
+    # run a unit using a solver and return if the result is correct
+    @staticmethod
+    def run_unit(solver: Solver, unit: Unit) -> ExecutionResult:
+        cmd = solver.executable.split(" ")
+        return_code, stdout, stderr = Runner.subprocess_run(cmd, unit.input)
+        unit.user = stdout + stderr
+        if return_code != 0:
+            unit.user += Symbol.execution
+            return ExecutionResult.EXECUTION_ERROR
+        if unit.user == unit.output:
+            return ExecutionResult.SUCCESS
+        return ExecutionResult.WRONG_OUTPUT
 
 
 class Actions:
 
     def __init__(self):
         pass
 
     @staticmethod
     def exec(target_list: List[str]):
         try:
             wdir = Wdir().set_target_list(target_list).build()
-        except Runner.CompileError as e:
+        except CompilerError as e:
             print(e)
             return 0
         
         if wdir.solver is None:
             print("\n" + Colored.paint("fail:", Color.RED) + " no solver found\n")
             return        
         
@@ -39,15 +56,15 @@
         print(wdir.resume())
         print(wdir.unit_list_resume())
 
     @staticmethod
     def run(target_list: List[str], param: Param.Basic) -> int:
         try:
             wdir = Wdir().set_target_list(target_list).build().filter(param)
-        except Runner.CompileError as e:
+        except CompilerError as e:
             print(e)
             return 0
         
         print(wdir.resume(), end="")
 
         if wdir.solver is None:
             print("\n" + Colored.paint("fail:", Color.RED) + " no solver found\n")
```

### Comparing `tko-0.0.2/src/tko/diff.py` & `tko-0.0.3/src/tko/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from typing import List, Optional, Tuple
 import io
 
-from .symbol import Symbol
-from .colored import Colored, Color
-from .unit import Unit
-from .report import Report
-
+from .format import Symbol, Colored, Color, Report
+from .basic import Unit
 
 class Diff:
 
     @staticmethod
     def render_white(text: Optional[str], color: Optional[Color] = None) -> Optional[str]:
         if text is None:
             return None
```

### Comparing `tko-0.0.2/src/tko/down.py` & `tko-0.0.3/src/tko/down.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from typing import Tuple
 import os
 import urllib.request
 import urllib.error
 import json
 
-from .settings_parser import SettingsParser
-
+from .settings import SettingsParser
 
 class Down:
 
     @staticmethod
     def update():
         if os.path.isfile(".info"):
             data = open(".info", "r").read().split("\n")[0]
             data = data.split(" ")
             discp = data[0]
             label = data[1]
             ext = data[2]
             Down.entry_unpack(".", discp, label, ext)
         else:
             print("No .info file found, skipping update...")
-    
-    @staticmethod
-    def entry_args(args):
-        destiny = Down.create_problem_folder(args.disc, args.index, args.extension)
-        Down.entry_unpack(destiny, args.disc, args.index, args.extension)
 
     @staticmethod
     def create_file(content, path, label=""):
         with open(path, "w") as f:
             f.write(content)
         print(path, label)
 
@@ -86,15 +80,15 @@
         info_file = os.path.join(destiny, ".info")
         with open(info_file, "w") as f:
             f.write(disc + " " + index + " " + ext + "\n")
         return destiny
 
     @staticmethod
     def entry_unpack(destiny, disc, index, ext):
-        discp_url = SettingsParser.get_repository(disc)
+        discp_url = SettingsParser().get_repository(disc)
         if discp_url is None:
             print("discipline not found")
             return
         
         index_url = discp_url + index + "/"
         cache_url = index_url + ".cache/"
```

### Comparing `tko-0.0.2/src/tko/loader.py` & `tko-0.0.3/src/tko/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,100 @@
 from typing import List, Tuple, Optional
 import re
 import os
-from .unit import Unit
-from .vpl_parser import VplParser
-from .pattern_loader import PatternLoader
+
+from .basic import Unit
+from .pattern import PatternLoader
+
+
+class VplParser:
+    @staticmethod
+    def finish(text):
+        return text if text.endswith("\n") else text + "\n"
+
+    @staticmethod
+    def unwrap(text):
+        while text.endswith("\n"):
+            text = text[:-1]
+        if text.startswith("\"") and text.endswith("\""):
+            text = text[1:-1]
+        return VplParser.finish(text)
+
+    @staticmethod
+    class CaseData:
+        def __init__(self, case="", inp="", outp="", grade: Optional[int] = None):
+            self.case: str = case
+            self.input: str = VplParser.finish(inp)
+            self.output: str = VplParser.unwrap(VplParser.finish(outp))
+            self.grade: Optional[int] = grade
+
+        def __str__(self):
+            return "case=" + self.case + '\n' \
+                   + "input=" + self.input \
+                   + "output=" + self.output \
+                   + "gr=" + str(self.grade)
+
+    regex_vpl_basic = r"case= *([ \S]*) *\n *input *=(.*?)^ *output *=(.*)"
+    regex_vpl_extended = r"case= *([ \S]*) *\n *input *=(.*?)^ *output *=(.*?)^ *grade *reduction *= *(\S*)% *\n?"
+
+    @staticmethod
+    def filter_quotes(x):
+        return x[1:-2] if x.startswith('"') else x
+
+    @staticmethod
+    def split_cases(text: str) -> List[str]:
+        regex = r"^ *[Cc]ase *="
+        subst = "case="
+        text = re.sub(regex, subst, text, 0, re.MULTILINE | re.DOTALL)
+        return ["case=" + t for t in text.split("case=")][1:]
+
+    @staticmethod
+    def extract_extended(text) -> Optional[CaseData]:
+        f = re.match(VplParser.regex_vpl_extended, text, re.MULTILINE | re.DOTALL)
+        if f is None:
+            return None
+        try:
+            gr = int(f.group(4))
+        except ValueError:
+            gr = None
+        return VplParser.CaseData(f.group(1), f.group(2), f.group(3), gr)
+
+    @staticmethod
+    def extract_basic(text) -> Optional[CaseData]:
+        m = re.match(VplParser.regex_vpl_basic, text, re.MULTILINE | re.DOTALL)
+        if m is None:
+            return None
+        return VplParser.CaseData(m.group(1), m.group(2), m.group(3), None)
+
+    @staticmethod
+    def parse_vpl(content: str) -> List[CaseData]:
+        text_cases = VplParser.split_cases(content)
+        seq: List[VplParser.CaseData] = []
+
+        for text in text_cases:
+            case = VplParser.extract_extended(text)
+            if case is not None:
+                seq.append(case)
+                continue
+            case = VplParser.extract_basic(text)
+            if case is not None:
+                seq.append(case)
+                continue
+            print("invalid case: " + text)
+            exit(1)
+        return seq
+
+    @staticmethod
+    def to_vpl(unit: CaseData):
+        text = "case=" + unit.case + "\n"
+        text += "input=" + unit.input
+        text += "output=\"" + unit.output + "\"\n"
+        if unit.grade is not None:
+            text += "grade reduction=" + str(unit.grade) + "%\n"
+        return text
 
 
 class Loader:
     regex_tio = r"^ *>>>>>>>> *(.*?)\n(.*?)^ *======== *\n(.*?)^ *<<<<<<<< *\n?"
 
     def __init__(self):
         pass
```

### Comparing `tko-0.0.2/src/tko/pattern_loader.py` & `tko-0.0.3/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.0.2/src/tko/runner.py` & `tko-0.0.3/src/tko/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class Runner:
 
     def __init__(self):
         pass
 
-    class CompileError(Exception):
-        pass
-
     @staticmethod
     def subprocess_run(cmd_list: List[str], input_data: str = "") -> Tuple[int, Any, Any]:
         try:
             p = subprocess.Popen(cmd_list, stdout=PIPE, stdin=PIPE, stderr=PIPE, universal_newlines=True)
             stdout, stderr = p.communicate(input=input_data)
             return p.returncode, stdout, stderr
         except FileNotFoundError:
```

### Comparing `tko-0.0.2/src/tko/settings_parser.py` & `tko-0.0.3/src/tko/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import os
 import configparser
 from appdirs import user_data_dir
 
-
 class SettingsParser:
-    settings_file = os.path.join(user_data_dir("tkj"), "settings.cfg")
 
     default_cfg_content = """[REP]
 fup = https://raw.githubusercontent.com/qxcodefup/arcade/master/base/
 ed = https://raw.githubusercontent.com/qxcodeed/arcade/master/base/
 poo = https://raw.githubusercontent.com/qxcodepoo/arcade/master/base/
 """
 
-    @staticmethod
-    def get_repository(disc):
-        if not os.path.isfile(SettingsParser.settings_file):
-            SettingsParser.create_default_settings_file()
-        with open(SettingsParser.settings_file, "r") as f:
-            parser = configparser.ConfigParser()
-            parser.read(SettingsParser.settings_file)
-            return parser["REP"][disc]
-
-    @staticmethod
-    def create_default_settings_file():
-        if not os.path.isdir(user_data_dir("tkj")):
-            os.mkdir(user_data_dir("tkj"))
-        with open(SettingsParser.settings_file, "w") as f:
-            f.write(SettingsParser.default_cfg_content)
+    def __init__(self):
+        self.package_name = "tko"
+        self.filename = "settings.cfg"
+        self.settings_dir = user_data_dir(self.package_name)
+        self.settings_file = os.path.join(self.settings_dir, self.filename)
+
+    def get_repository(self, disc):
+        if not os.path.isfile(self.settings_file):
+            self.create_default_settings_file()
+        parser = configparser.ConfigParser()
+        parser.read(self.settings_file)
+        return parser["REP"][disc]
+
+    def create_default_settings_file(self):
+        if not os.path.isdir(self.settings_dir):
+            os.mkdir(self.settings_dir)
+        with open(self.settings_file, "w") as f:
+            f.write(self.default_cfg_content)
+
+    def get_settings_file(self):
+        if not os.path.isfile(self.settings_file):
+            self.create_default_settings_file()
+        return self.settings_file
```

### Comparing `tko-0.0.2/src/tko/solver.py` & `tko-0.0.3/src/tko/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import tempfile
 
 import os
 from typing import List
 from shutil import which
 
+from .basic import CompilerError
 from .runner import Runner
 
 
 def check_tool(name):
     if which(name) is None:
-        raise Runner.CompileError("fail: " + name + " executable not found")
+        raise CompilerError("fail: " + name + " executable not found")
 
 class Solver:
     def __init__(self, solver_list: List[str]):
         self.path_list: List[str] = [Solver.__add_dot_bar(path) for path in solver_list]
         
         self.temp_dir = tempfile.mkdtemp()
         # print("Tempdir for execution: " + self.temp_dir)
@@ -62,15 +63,15 @@
         
 
         cmd = ["javac"] + self.path_list + ['-d', self.temp_dir]
         return_code, stdout, stderr = Runner.subprocess_run(cmd)
         print(stdout)
         print(stderr)
         if return_code != 0:
-            raise Runner.CompileError(stdout + stderr)
+            raise CompilerError(stdout + stderr)
         # solver = solver.split(os.sep)[-1]  # getting only the filename
         self.executable = "java -cp " + self.temp_dir + " " + filename[:-5]  # removing the .java
 
     def __prepare_js(self):
         check_tool("node")
 
         import_str = (r'let __lines = require("fs").readFileSync(0).toString().split("\n"); let input = () => '
@@ -100,29 +101,29 @@
         source_list = self.path_list
         # print("Using the following source files: " + str([os.path.basename(x) for x in source_list]))
         # compile the ts file
         cmd = ["esbuild"] + source_list + ["--outdir=" + self.temp_dir, "--format=cjs", "--log-level=error"]
         return_code, stdout, stderr = Runner.subprocess_run(cmd)
         print(stdout + stderr)
         if return_code != 0:
-            raise Runner.CompileError(stdout + stderr)
+            raise CompilerError(stdout + stderr)
         jsfile = os.path.join(self.temp_dir, filename[:-3] + ".js")
         self.executable = "node " + jsfile  # renaming solver to main
     
     def __prepare_c_cpp(self, pre_args: List[str], pos_args: list[str]):
         # solver = self.path_list[0]
         tempdir = self.temp_dir
         source_list = self.path_list
         # print("Using the following source files: " + str([os.path.basename(x) for x in source_list]))
         
         exec_path = os.path.join(tempdir, ".a.out")
         cmd = pre_args + source_list + ["-o", exec_path] + pos_args
         return_code, stdout, stderr = Runner.subprocess_run(cmd)
         if return_code != 0:
-            raise Runner.CompileError(stdout + stderr)
+            raise CompilerError(stdout + stderr)
         self.executable = exec_path
 
     def __prepare_c(self):
         check_tool("gcc")
         pre = ["gcc", "-Wall"]
         pos = ["-lm", "-lutil"]
         self.__prepare_c_cpp(pre, pos)
```

### Comparing `tko-0.0.2/src/tko/wdir.py` & `tko-0.0.3/src/tko/wdir.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,59 @@
 from typing import List, Optional
 import math
 import os
 
-from .enums import IdentifierType, Identifier
+from .basic import IdentifierType, Identifier, Unit, Param
 from .loader import Loader
 from .solver import Solver
-from .unit import Unit
-from .param import Param
-from .label_factory import LabelFactory
-from .symbol import Symbol
-from .colored import Colored, Color
+from .format import Symbol, Colored, Color
 
+# generate label for cases
+class LabelFactory:
+    def __init__(self):
+        self._label = ""
+        self._index = -1
+
+    def index(self, value: int):
+        try:
+            self._index = int(value)
+        except ValueError:
+            raise ValueError("Index on label must be a integer")
+        return self
+
+    def label(self, value: str):
+        self._label = value
+        return self
+
+    def generate(self):
+        label = LabelFactory.trim_spaces(self._label)
+        label = LabelFactory.remove_old_index(label)
+        if self._index != -1:
+            index = str(self._index).zfill(2)
+            if label != "":
+                return index + " " + label
+            else:
+                return index
+        return label
+
+    @staticmethod
+    def trim_spaces(text):
+        parts = text.split(" ")
+        parts = [word for word in parts if word != '']
+        return " ".join(parts)
+
+    @staticmethod
+    def remove_old_index(label):
+        split_label = label.split(" ")
+        if len(split_label) > 0:
+            try:
+                int(split_label[0])
+                return " ".join(split_label[1:])
+            except ValueError:
+                return label
 
 class Wdir:
     def __init__(self):
         self.solver: Optional[Solver] = None
         self.source_list: List[str] = []
         self.pack_list: List[List[Unit]] = []
         self.unit_list: List[Unit] = []
```

### Comparing `tko-0.0.2/src/tko/writer.py` & `tko-0.0.3/src/tko/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List
 import os
 
-from .pattern_loader import PatternLoader
-from .unit import Unit
-from .enums import IdentifierType, Identifier
+from .pattern import PatternLoader
+from .basic import IdentifierType, Identifier, Unit
 
 
 class Writer:
 
     def __init__(self):
         pass
```

