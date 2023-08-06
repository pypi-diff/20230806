# Comparing `tmp/tmux_conf-0.16.3.tar.gz` & `tmp/tmux_conf-0.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmux_conf-0.16.3.tar", last modified: Sun Aug  6 00:04:22 2023, max compression
+gzip compressed data, was "/usr/local/my_tmux_conf/local_tmux_conf/dist/.tmp-wb7yz3dd/tmux_conf-0.16.4.tar", last modified: Sun Aug  6 02:20:01 2023, max compression
```

## Comparing `tmux_conf-0.16.3.tar` & `tmux_conf-0.16.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.141945 tmux_conf-0.16.3/
--rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.3/LICENSE
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 00:04:22.141489 tmux_conf-0.16.3/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.3/README.md
--rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-08-06 00:02:20.000000 tmux_conf-0.16.3/pyproject.toml
--rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-08-06 00:04:22.142043 tmux_conf-0.16.3/setup.cfg
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.127995 tmux_conf-0.16.3/src/
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.134134 tmux_conf-0.16.3/src/tmux_conf/
--rw-r--r--   0 jaclu      (501) staff       (20)      202 2023-08-05 13:31:39.000000 tmux_conf-0.16.3/src/tmux_conf/__init__.py
--rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-08-06 00:02:08.000000 tmux_conf-0.16.3/src/tmux_conf/constants.py
--rw-r--r--   0 jaclu      (501) staff       (20)     5996 2023-08-05 22:44:17.000000 tmux_conf-0.16.3/src/tmux_conf/embedded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-05-12 13:47:26.000000 tmux_conf-0.16.3/src/tmux_conf/exceptions.py
--rw-r--r--   0 jaclu      (501) staff       (20)    16220 2023-08-05 22:50:14.000000 tmux_conf-0.16.3/src/tmux_conf/plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    23376 2023-08-05 23:58:54.000000 tmux_conf-0.16.3/src/tmux_conf/tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4791 2023-08-05 22:23:21.000000 tmux_conf-0.16.3/src/tmux_conf/utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4002 2023-08-05 22:20:58.000000 tmux_conf-0.16.3/src/tmux_conf/vers_check.py
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.137395 tmux_conf-0.16.3/src/tmux_conf.egg-info/
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/top_level.txt
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.140832 tmux_conf-0.16.3/tests/
--rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.3/tests/test_embeded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-11 08:30:17.000000 tmux_conf-0.16.3/tests/test_plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.3/tests/test_tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.3/tests/test_utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.3/tests/test_vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/
+-rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.4/LICENSE
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.4/README.md
+-rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-08-06 02:08:34.000000 tmux_conf-0.16.4/pyproject.toml
+-rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/setup.cfg
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf/
+-rw-r--r--   0 jaclu      (501) staff       (20)      202 2023-08-05 13:31:39.000000 tmux_conf-0.16.4/src/tmux_conf/__init__.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-08-06 02:08:26.000000 tmux_conf-0.16.4/src/tmux_conf/constants.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     5939 2023-08-06 01:57:04.000000 tmux_conf-0.16.4/src/tmux_conf/embedded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-08-06 01:51:53.000000 tmux_conf-0.16.4/src/tmux_conf/exceptions.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15977 2023-08-06 01:56:47.000000 tmux_conf-0.16.4/src/tmux_conf/plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    23393 2023-08-06 01:56:54.000000 tmux_conf-0.16.4/src/tmux_conf/tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4780 2023-08-06 01:47:51.000000 tmux_conf-0.16.4/src/tmux_conf/utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     3983 2023-08-06 01:59:30.000000 tmux_conf-0.16.4/src/tmux_conf/vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf.egg-info/
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 02:20:01.000000 tmux_conf-0.16.4/tests/
+-rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.4/tests/test_embeded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-11 08:30:17.000000 tmux_conf-0.16.4/tests/test_plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.4/tests/test_tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.4/tests/test_utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.4/tests/test_vers_check.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tmux_conf-0.16.3/LICENSE` & `tmux_conf-0.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/PKG-INFO` & `tmux_conf-0.16.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux_conf
-Version: 0.16.3
+Version: 0.16.4
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.3/README.md` & `tmux_conf-0.16.4/README.md`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/pyproject.toml` & `tmux_conf-0.16.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tmux_conf"
-version = "0.16.3"
+version = "0.16.4"
 authors = [
   { name="Jacob Lundqvist", email="Jacob.Lundqvist@gmail.com" },
 ]
 description = "Generates version checked tmux conf"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["tmux", "automation"]
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf/embedded_scripts.py` & `tmux_conf-0.16.4/src/tmux_conf/embedded_scripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 from .constants import XDG_CONFIG_HOME
 from .utils import run_shell, tilde_home_dir
 
 
 class EmbeddedScripts:
     """Handles scripts, either embedded or stored in scripts/ as external"""
 
-    def __init__(self, conf_file: str, use_embedded_scripts: bool):
+    def __init__(self, conf_file, use_embedded_scripts):
         #  Ensure conf file is using ~ or full path if ~ not applicable
         conf_file = tilde_home_dir(conf_file)
         if conf_file[0] not in ("~", "/"):
             conf_file = tilde_home_dir(os.path.join(os.getcwd(), conf_file))
         self._conf_file = conf_file
 
         self._use_embedded_scripts = use_embedded_scripts
-        self._scripts: list[str] = []
+        self._scripts = []
         self.defined_scripts = []
-        self._bash_scripts: list[str] = []
+        self._bash_scripts = []
         self._bash_shell = ""  # Will only be set if needed
 
     def create(
         self,
         scr_name: str,
-        script: list[str],
+        script,
         use_bash: bool = False,
         built_in: bool = False,
     ) -> None:
         """Creates a script, supplied as a list of lines
         script lines can be regular lines as string, or multi-line strings
 
         built_in is set to True for scripts generated in this pip
@@ -113,15 +113,15 @@
                 cmd += "sh"
             cmd += f" -s {scr_name}"
         else:
             cmd += f"{self.get_dir()}/{scr_name}.sh"
         cmd += '"'
         return cmd
 
-    def content(self) -> list[str]:
+    def content(self):
         """Generates the code for embedded scripts to be written to
         the conf file"""
         if not (self._use_embedded_scripts and self._scripts):
             return []
 
         output = [
             """
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf/plugins.py` & `tmux_conf-0.16.4/src/tmux_conf/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 #
 #  See the README.md in the repository for more info
 #
 
 import os
 import shutil
 import sys
-from collections.abc import Callable
-from typing import Union
 
 import __main__
 
 from .constants import XDG_CONFIG_HOME
 from .embedded_scripts import EmbeddedScripts
 from .vers_check import VersionCheck
 
@@ -44,38 +42,36 @@
         self._conf_file = conf_file
         self._vers = vers_class
         self._es = es_class
         self._plugin_handler = plugin_handler
 
         self._is_limited_host = False
 
-        self._used_plugins: dict[str, tuple[str, Callable[[], list[str]], str]] = {}
+        self._used_plugins = {}
         # self._used_plugins: dict[
         #     str, tuple[str, Callable[[], tuple[str, str, str]], str]
         # ] = {}  # plugins that will be used
         #: dict[
         #    str, tuple[str, classmethod, str]
         # ]
-        self._skipped_plugins: list[
-            tuple[str, str]
-        ] = []  # plugins incompatible with this version
+        self._skipped_plugins = []  # plugins incompatible with this version
         self._fnc_activate_tpm = "activate_tpm"
         self._fnc_activate_manually = "activate_plugins_mamually"
 
         if plugins_display not in [0, 1, 2, 3]:
             raise ValueError("plugins_display must be one of: 0, 1, 2, 3")
         self._plugins_display = plugins_display
         if clear_plugins:
             #
             #  if plugins_display is set, it will terminate the app,
             #  so lets do this before
             #
             self.clear()
 
-    def found(self, short_name: bool = True) -> list[str]:
+    def found(self, short_name: bool = True):
         """Returns a list of plugin names being used.
         If short_name is False will return the full name including
         source, this is needed when cloning the repo, but less desired
         when just checking if a given plugin is used in most cases.
         Since if a different fork of it is being used, the name would
         not match."""
         result = []
@@ -105,15 +101,15 @@
         plugin init, to help indicating when all the plugins are setup.
         Om normalish system, this is close to instantaneous, so step by
         step progress is not really meaningful.
         """
         self._is_limited_host = is_limited
         return self._is_limited_host
 
-    def scan(self, plugin_methods) -> None:
+    def scan(self, plugin_methods):  # list[Callable[[], list[str]]]) -> None:
         """Investigate all defined plugin methods, and determine if a
         given plugin can be used depending on running tmux"""
         duplicate_check = []
         for plugin_mthd in plugin_methods:
             plugin_name, vers_min, code = plugin_mthd()
             if plugin_name in duplicate_check:
                 print(f'ERROR: plugin "{plugin_name}" defined more than once:')
@@ -220,15 +216,15 @@
         print(f'{"Min":<{max_l_v}}|{" Plugin name":<{max_l_name}}')
         print(f'{"vers":<{max_l_v}}|\n')
         for vers, name in self._skipped_plugins:
             print(f"{vers:>{max_l_v}}  {name:<{max_l_name}}")
 
         sys.exit(0)
 
-    def parse(self) -> list[Union[str, list[str]]]:
+    def parse(self):
         """This package will use any plugin defining methods it can find.
         They will be sorted alphabetically by method name, normally the order
         of plugins do not matter, but if you do want to force the sorting,
         just change the method name accordingly.
 
         They are assumed to start with plugin_ and have the following format:
 
@@ -242,15 +238,15 @@
         all normal tmux-conf functionality is available.
 
         Here are a few examples:
         """
         if not (self._used_plugins):
             return []
 
-        output: list[Union[str, list[str]]] = []
+        output = []
 
         #
         #  First ensure that plugin code that needs to process the
         #  environment is done and output is written to config.
         #
         for name, info in self._used_plugins.items():
             info[1]()
@@ -277,15 +273,15 @@
             #  or a clone.
             #
             output.append(self.mkscript_tpm_deploy())
             output.append(self._es.run_it(self._fnc_activate_tpm, in_bg=True))
         output.append("")  # spacer between sections
         return output
 
-    def get_env(self) -> tuple[str, str]:
+    def get_env(self):
         location = os.path.dirname(os.path.expanduser(self._conf_file))
         if location == os.path.expanduser("~"):
             #
             #  If conf file is default, plugins have a non standard location
             #
             if self._conf_file.find("tmate") > -1:
                 plugins_dir = os.path.expanduser("~/.tmate/plugins")
@@ -302,15 +298,15 @@
                 conf_base = os.path.dirname(location)
 
             plugins_dir = os.path.join(conf_base, "tmux", "plugins")
             tpm_env = os.path.expanduser(f'XDG_CONFIG_HOME="{conf_base}" ')
 
         return plugins_dir, tpm_env
 
-    def mkscript_manual_deploy(self) -> list[str]:
+    def mkscript_manual_deploy(self):
         """This script is run as tmux starts, all non-present
         plugins are installed, and an attempt is done to initialize
         each plugin.
         """
         output = []
         output.append(
             """
@@ -351,15 +347,15 @@
 }}""",
         ]
         self._es.create(
             self._fnc_activate_manually, activate_manually_sh, use_bash=True
         )
         return output
 
-    def mkscript_tpm_deploy(self) -> list[str]:
+    def mkscript_tpm_deploy(self):
         """If tpm is present, it is started.
         If not, it is installed and requested to install all
         defined plugins.
         """
         output = []
         output.append(
             """
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf/tmux_conf.py` & `tmux_conf-0.16.4/src/tmux_conf/tmux_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 #
 #  See the README.md in the repository for more info
 #
 #  All paths stored internally are done so with ~ expanded
 #
 
 
+# from datetime import datetime
+import datetime
 import os
 import shutil
 import sys
 from collections.abc import Callable
-from datetime import datetime
 
 import __main__
 
 from .constants import __version__
 from .embedded_scripts import EmbeddedScripts
 from .exceptions import TmuxConfNotTmuxCommand
 from .plugins import Plugins
@@ -85,15 +86,15 @@
     def __init__(
         self,
         parse_cmd_line: bool = True,
         #
         #  if parse_cmd_line is True all other parameters are ignored
         #
         conf_file: str = "~/.tmux.conf",  # where to store conf file
-        tmux_bin: str = "tmux",  #  Default binary, if none given
+        tmux_bin: str = "tmux",  # Default binary, if none given
         tmux_version: str = "",
         replace_config: bool = False,  # replace config with no prompt
         clear_plugins: bool = False,  # remove all current plugins
         plugins_display: int = 0,  # Display info about plugins
         # then terminate
     ):
         if parse_cmd_line:
@@ -326,15 +327,15 @@
         #
         #  Should be called as late as possible, to be able to have
         #  gathered all the intended embedded scripts.
         #
         for line in self.es.content():
             self.write(line)
 
-    def list_plugin_methods(self) -> list[Callable[[], list[str]]]:
+    def list_plugin_methods(self):  # -> list[Callable[[], list[str]]]:
         """Support for plugins.py, provides a list of all plugin_... methods"""
         plugin_mthds: list[Callable[[], list[str]]] = []
         if self.plugin_handler:
             for item in dir(self):
                 if item.find("plugin_") or item == "plugin_handler":
                     continue
                 plugin_mthds.append(getattr(self, item))
@@ -364,15 +365,15 @@
             )
 
         w(
             f"""#
         #  This config was created using
         #      https://github.com/jaclu/tmux-conf
         #
-        #      Creation time: {datetime.now().strftime("%y-%m-%d %H:%M:%S")}
+        #      Creation time: {datetime.datetime.now().strftime("%y-%m-%d %H:%M:%S")}
         #          tmux-conf: {self.lib_version}
         #         Created on: {run_shell('hostname').strip()}"""
         )
         if self.vers.get() != self.vers.get_actual():  # type: ignore
             w(f"#     actual version: ({self.vers.get_actual()})")  # type: ignore
         w(f"#   For tmux version: {self.vers.get()}")  # type: ignore
         w(
@@ -444,15 +445,15 @@
                     raise SyntaxError(
                         "Un-escaped back-ticks can not be present in "
                         + "the generated config when\n"
                         + "embedded_scripts are used!"
                     )
                 f.write(f"{line}{eol}")
 
-    def filter_note(self, line: str) -> list[str]:
+    def filter_note(self, line: str):
         """Returns list of lines, if notes are not supported
         first an empty spacer line, then the note as a comment,
         and finally the actual command without the note
         if self.use_notes_as_comments is False
         only the third line from above is returned
         """
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf/utils.py` & `tmux_conf-0.16.4/src/tmux_conf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 def is_executable(cmd: str) -> bool:
     fpath = os.path.expanduser(cmd)
     return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
 
 
-def parse_cmdline(args: list[str]):
+def parse_cmdline(args):
     parser = argparse.ArgumentParser(
         description="This tmux conf compiler generates configs for tmux "
         + "versions 1.5 and up."
     )
 
     #  Prints tmux-conf version info then exits
     parser.add_argument(
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf/vers_check.py` & `tmux_conf-0.16.4/src/tmux_conf/vers_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         r = True
         if vers_min > self.v_min:
             r = False
         elif vers_min == self.v_min and suffix > self.v_suffix:
             r = False
         return r
 
-    def get_sub_vers(self, v2: str) -> tuple[int, str]:
+    def get_sub_vers(self, v2: str):
         int_part = ""
         for c in v2:
             try:
                 int(c)
             except ValueError:
                 break
             int_part += c
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf.egg-info/PKG-INFO` & `tmux_conf-0.16.4/src/tmux_conf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux-conf
-Version: 0.16.3
+Version: 0.16.4
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.3/src/tmux_conf.egg-info/SOURCES.txt` & `tmux_conf-0.16.4/src/tmux_conf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/tests/test_embeded_scripts.py` & `tmux_conf-0.16.4/tests/test_embeded_scripts.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/tests/test_plugins.py` & `tmux_conf-0.16.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/tests/test_tmux_conf.py` & `tmux_conf-0.16.4/tests/test_tmux_conf.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/tests/test_utils.py` & `tmux_conf-0.16.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.3/tests/test_vers_check.py` & `tmux_conf-0.16.4/tests/test_vers_check.py`

 * *Files identical despite different names*

