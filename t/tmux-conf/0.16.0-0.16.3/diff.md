# Comparing `tmp/tmux_conf-0.16.0.tar.gz` & `tmp/tmux_conf-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmux_conf-0.16.0.tar", last modified: Sun Jul  9 10:44:02 2023, max compression
+gzip compressed data, was "tmux_conf-0.16.3.tar", last modified: Sun Aug  6 00:04:22 2023, max compression
```

## Comparing `tmux_conf-0.16.0.tar` & `tmux_conf-0.16.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.800334 tmux_conf-0.16.0/
--rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/LICENSE
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-07-09 10:44:02.799896 tmux_conf-0.16.0/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/README.md
--rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-07-09 10:43:20.000000 tmux_conf-0.16.0/pyproject.toml
--rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-07-09 10:44:02.800508 tmux_conf-0.16.0/setup.cfg
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.784356 tmux_conf-0.16.0/src/
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.793074 tmux_conf-0.16.0/src/tmux_conf/
--rw-r--r--   0 jaclu      (501) staff       (20)      202 2022-12-16 01:20:21.000000 tmux_conf-0.16.0/src/tmux_conf/__init__.py
--rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-07-08 10:30:28.000000 tmux_conf-0.16.0/src/tmux_conf/constants.py
--rw-r--r--   0 jaclu      (501) staff       (20)     5394 2023-05-12 13:52:19.000000 tmux_conf-0.16.0/src/tmux_conf/embedded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-05-12 13:47:26.000000 tmux_conf-0.16.0/src/tmux_conf/exceptions.py
--rw-r--r--   0 jaclu      (501) staff       (20)    16598 2023-05-15 11:48:01.000000 tmux_conf-0.16.0/src/tmux_conf/plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    25531 2023-07-09 10:17:40.000000 tmux_conf-0.16.0/src/tmux_conf/tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4780 2023-04-25 08:10:55.000000 tmux_conf-0.16.0/src/tmux_conf/utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     3968 2023-05-12 20:08:07.000000 tmux_conf-0.16.0/src/tmux_conf/vers_check.py
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.795317 tmux_conf-0.16.0/src/tmux_conf.egg-info/
--rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/PKG-INFO
--rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/SOURCES.txt
--rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/dependency_links.txt
--rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-07-09 10:44:02.000000 tmux_conf-0.16.0/src/tmux_conf.egg-info/top_level.txt
-drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-07-09 10:44:02.799137 tmux_conf-0.16.0/tests/
--rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.0/tests/test_embeded_scripts.py
--rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-09 10:30:15.000000 tmux_conf-0.16.0/tests/test_plugins.py
--rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.0/tests/test_tmux_conf.py
--rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.0/tests/test_utils.py
--rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.0/tests/test_vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.141945 tmux_conf-0.16.3/
+-rw-r--r--   0 jaclu      (501) staff       (20)     1072 2022-12-16 01:20:21.000000 tmux_conf-0.16.3/LICENSE
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 00:04:22.141489 tmux_conf-0.16.3/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)     7332 2022-12-16 01:20:21.000000 tmux_conf-0.16.3/README.md
+-rw-r--r--   0 jaclu      (501) staff       (20)     1588 2023-08-06 00:02:20.000000 tmux_conf-0.16.3/pyproject.toml
+-rw-r--r--   0 jaclu      (501) staff       (20)       38 2023-08-06 00:04:22.142043 tmux_conf-0.16.3/setup.cfg
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.127995 tmux_conf-0.16.3/src/
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.134134 tmux_conf-0.16.3/src/tmux_conf/
+-rw-r--r--   0 jaclu      (501) staff       (20)      202 2023-08-05 13:31:39.000000 tmux_conf-0.16.3/src/tmux_conf/__init__.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      269 2023-08-06 00:02:08.000000 tmux_conf-0.16.3/src/tmux_conf/constants.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     5996 2023-08-05 22:44:17.000000 tmux_conf-0.16.3/src/tmux_conf/embedded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)      436 2023-05-12 13:47:26.000000 tmux_conf-0.16.3/src/tmux_conf/exceptions.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    16220 2023-08-05 22:50:14.000000 tmux_conf-0.16.3/src/tmux_conf/plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    23376 2023-08-05 23:58:54.000000 tmux_conf-0.16.3/src/tmux_conf/tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4791 2023-08-05 22:23:21.000000 tmux_conf-0.16.3/src/tmux_conf/utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4002 2023-08-05 22:20:58.000000 tmux_conf-0.16.3/src/tmux_conf/vers_check.py
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.137395 tmux_conf-0.16.3/src/tmux_conf.egg-info/
+-rw-r--r--   0 jaclu      (501) staff       (20)     7996 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/PKG-INFO
+-rw-r--r--   0 jaclu      (501) staff       (20)      519 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/SOURCES.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)        1 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/dependency_links.txt
+-rw-r--r--   0 jaclu      (501) staff       (20)       10 2023-08-06 00:04:22.000000 tmux_conf-0.16.3/src/tmux_conf.egg-info/top_level.txt
+drwxr-xr-x   0 jaclu      (501) staff       (20)        0 2023-08-06 00:04:22.140832 tmux_conf-0.16.3/tests/
+-rw-r--r--   0 jaclu      (501) staff       (20)     3775 2023-07-09 10:30:18.000000 tmux_conf-0.16.3/tests/test_embeded_scripts.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     8194 2023-07-11 08:30:17.000000 tmux_conf-0.16.3/tests/test_plugins.py
+-rw-r--r--   0 jaclu      (501) staff       (20)    15013 2023-07-09 10:30:02.000000 tmux_conf-0.16.3/tests/test_tmux_conf.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     4061 2023-07-09 10:30:07.000000 tmux_conf-0.16.3/tests/test_utils.py
+-rw-r--r--   0 jaclu      (501) staff       (20)     2915 2023-07-09 10:30:10.000000 tmux_conf-0.16.3/tests/test_vers_check.py
```

### Comparing `tmux_conf-0.16.0/LICENSE` & `tmux_conf-0.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/PKG-INFO` & `tmux_conf-0.16.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux_conf
-Version: 0.16.0
+Version: 0.16.3
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.0/README.md` & `tmux_conf-0.16.3/README.md`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/pyproject.toml` & `tmux_conf-0.16.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tmux_conf"
-version = "0.16.0"
+version = "0.16.3"
 authors = [
   { name="Jacob Lundqvist", email="Jacob.Lundqvist@gmail.com" },
 ]
 description = "Generates version checked tmux conf"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["tmux", "automation"]
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf/embedded_scripts.py` & `tmux_conf-0.16.3/src/tmux_conf/embedded_scripts.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,32 +29,50 @@
         conf_file = tilde_home_dir(conf_file)
         if conf_file[0] not in ("~", "/"):
             conf_file = tilde_home_dir(os.path.join(os.getcwd(), conf_file))
         self._conf_file = conf_file
 
         self._use_embedded_scripts = use_embedded_scripts
         self._scripts: list[str] = []
+        self.defined_scripts = []
         self._bash_scripts: list[str] = []
         self._bash_shell = ""  # Will only be set if needed
 
-    def create(self, scr_name: str, script, use_bash=False):
+    def create(
+        self,
+        scr_name: str,
+        script: list[str],
+        use_bash: bool = False,
+        built_in: bool = False,
+    ) -> None:
         """Creates a script, supplied as a list of lines
         script lines can be regular lines as string, or multi-line strings
 
+        built_in is set to True for scripts generated in this pip
+        then it is checked if such a script has already been created by
+        code using this, and if the scr_name has been used, this instance
+        of it is skipped
+
         Where the script should be run, just call run_it() with
         the script name, and code will be generated to call it the right way.
 
         calling self.run_it('activate_tpm')  will (depending on config file)
         insert code like:
           run "cut -c3- /home/jaclu/.tmux.conf | sh -s activate_tpm"
         or:
           run "/home/jaclu/.tmux/scripts/activate_tpm.sh"
 
         depending on self._use_embedded_scripts
         """
+        if built_in is False:
+            self.defined_scripts.append(scr_name)
+        else:
+            #  Allow users to override default scripts
+            if scr_name in self.defined_scripts:
+                return
         if self._use_embedded_scripts:
             if use_bash:
                 self._bash_scripts.append(scr_name)
             self._scripts += script
             self._scripts.append("")  # separator between scripts
         else:
             script_dir = self.get_dir()
@@ -95,27 +113,26 @@
                 cmd += "sh"
             cmd += f" -s {scr_name}"
         else:
             cmd += f"{self.get_dir()}/{scr_name}.sh"
         cmd += '"'
         return cmd
 
-    def content(self):
+    def content(self) -> list[str]:
         """Generates the code for embedded scripts to be written to
         the conf file"""
         if not (self._use_embedded_scripts and self._scripts):
             return []
 
         output = [
             """
         #======================================================
         #
         # EMBEDDED-SCRIPTS-STARTING-POINT
-        #
-        """
+        #"""
         ]
         #
         #  Embedded scripts starts at column 3, insert extra indention on
         #  each line
         #
         for script_line in self._scripts:
             mutlilines = script_line.split("\n")
@@ -130,15 +147,15 @@
                 for line in mutlilines:
                     output.append(f"# {line}")
             else:
                 output.append(f"# {script_line}")
         output.append('# "$@" #  This triggers the embedded script')
         return output
 
-    def get_dir(self):
+    def get_dir(self) -> str:
         """Retrieves the location where scripts should be saved"""
         if self._use_embedded_scripts:
             raise SyntaxError("get_dir() called when use_embedded_scripts is True")
 
         if tilde_home_dir(self._conf_file) == "~/.tmux.conf":
             scripts_dir = os.path.expanduser("~/.tmux/scripts")
         else:
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf/plugins.py` & `tmux_conf-0.16.3/src/tmux_conf/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if clear_plugins:
             #
             #  if plugins_display is set, it will terminate the app,
             #  so lets do this before
             #
             self.clear()
 
-    def found(self, short_name=True):
+    def found(self, short_name: bool = True) -> list[str]:
         """Returns a list of plugin names being used.
         If short_name is False will return the full name including
         source, this is needed when cloning the repo, but less desired
         when just checking if a given plugin is used in most cases.
         Since if a different fork of it is being used, the name would
         not match."""
         result = []
@@ -128,15 +128,15 @@
                     plugin_mthd,  # self.PLUGIN_MTHD
                     code,  # self.PLUGIN_STATIC_CODE
                 )
             else:
                 self._skipped_plugins.append((str(vers_min), plugin_name))
         self._skipped_plugins.sort()
 
-    def display_info(self):
+    def display_info(self) -> str:
         """List selected and ignored plugins, depending on param"""
         print(f"\n\t=====  tmux {self._vers.get()} - Plugins defined  =====")
         print(f" for: {__main__.__file__}")
 
         #
         #  First loop to find longest plugin name
         #
@@ -220,15 +220,15 @@
         print(f'{"Min":<{max_l_v}}|{" Plugin name":<{max_l_name}}')
         print(f'{"vers":<{max_l_v}}|\n')
         for vers, name in self._skipped_plugins:
             print(f"{vers:>{max_l_v}}  {name:<{max_l_name}}")
 
         sys.exit(0)
 
-    def parse(self):
+    def parse(self) -> list[Union[str, list[str]]]:
         """This package will use any plugin defining methods it can find.
         They will be sorted alphabetically by method name, normally the order
         of plugins do not matter, but if you do want to force the sorting,
         just change the method name accordingly.
 
         They are assumed to start with plugin_ and have the following format:
 
@@ -277,15 +277,15 @@
             #  or a clone.
             #
             output.append(self.mkscript_tpm_deploy())
             output.append(self._es.run_it(self._fnc_activate_tpm, in_bg=True))
         output.append("")  # spacer between sections
         return output
 
-    def get_env(self):
+    def get_env(self) -> tuple[str, str]:
         location = os.path.dirname(os.path.expanduser(self._conf_file))
         if location == os.path.expanduser("~"):
             #
             #  If conf file is default, plugins have a non standard location
             #
             if self._conf_file.find("tmate") > -1:
                 plugins_dir = os.path.expanduser("~/.tmate/plugins")
@@ -302,15 +302,15 @@
                 conf_base = os.path.dirname(location)
 
             plugins_dir = os.path.join(conf_base, "tmux", "plugins")
             tpm_env = os.path.expanduser(f'XDG_CONFIG_HOME="{conf_base}" ')
 
         return plugins_dir, tpm_env
 
-    def mkscript_manual_deploy(self):
+    def mkscript_manual_deploy(self) -> list[str]:
         """This script is run as tmux starts, all non-present
         plugins are installed, and an attempt is done to initialize
         each plugin.
         """
         output = []
         output.append(
             """
@@ -351,15 +351,15 @@
 }}""",
         ]
         self._es.create(
             self._fnc_activate_manually, activate_manually_sh, use_bash=True
         )
         return output
 
-    def mkscript_tpm_deploy(self):
+    def mkscript_tpm_deploy(self) -> list[str]:
         """If tpm is present, it is started.
         If not, it is installed and requested to install all
         defined plugins.
         """
         output = []
         output.append(
             """
@@ -370,37 +370,25 @@
         #======================================================
         """
         )
         #  os.makedirs(plugins_dir, exist_ok=True)
         plugins_dir, tpm_env = self.get_env()
         tpm_location = os.path.join(plugins_dir, "tpm")
         tpm_app = os.path.join(tpm_location, "tpm")
-
-        run_installed_tpm = f"{tpm_env}{tpm_app}"
-        if self._is_limited_host:
-            run_installed_tpm = f"""#
-        #  If you quickly shut down tmux whilst tpm is still running, things
-        #  can go wrong. On all normal systems, this is so instantaneous,
-        #  that it is not an issue, but on slow systems, this can take
-        #  a noticeable time, up to five seconds when running iSH for example,
-        #  so in such cases try to wait to exit until after "tpm completed!"
-        #  has been announced.
-        #
-        $TMUX_BIN display "Running tpm..."
-        {run_installed_tpm}
-        $TMUX_BIN display "tpm completed!" """
-
+        ind_tpm_working = "@tpm-working-indicator"
         activate_tpm_sh = [
             f"""
 {self._fnc_activate_tpm}() {{
     #
     #  Initialize already installed tpm if found
     #
     if [ -x "{tpm_app}" ]; then
-        {run_installed_tpm}
+        $TMUX_BIN set-environment -g  {ind_tpm_working} 1
+        {tpm_env}{tpm_app}
+        $TMUX_BIN set-environment -gu {ind_tpm_working}
         exit 0
     fi
 
     #  Create plugin dir if needed
     mkdir -p "{plugins_dir}"
 
     #  Remove potentially broken tpm install
@@ -432,15 +420,15 @@
         echo "Failed to run: {tpm_location}/bindings/install_plugins"
         exit 12
     fi
 
     $TMUX_BIN display "Plugin setup completed"
 }}""",
         ]
-        self._es.create(self._fnc_activate_tpm, activate_tpm_sh)
+        self._es.create(self._fnc_activate_tpm, activate_tpm_sh, built_in=True)
         return output
 
     def clear(self):
         """To minimize risk of some bug causing massive file deletion,
         file path is double checked.
         """
         plugins_dir = self.get_plugin_dir()
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf/tmux_conf.py` & `tmux_conf-0.16.3/src/tmux_conf/tmux_conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,58 +47,53 @@
     #
     #  My fork also reports more detailed progress on what plugin is
     #  processed
     #
     #  set this to 'jaclu/tpm' if you want to try that one!
     #  set it to '' if you do not want to use tpm at all.
     #
-    plugin_handler = "tmux-plugins/tpm"
+    plugin_handler: str = "tmux-plugins/tpm"
 
     #
     #  If true and tmux is < 3.1 thus not supporting -N bind notes
     #  this extracts the note and inserts it before the line as a comment.
     #  If false, the note is just discarded.
     #
-    use_notes_as_comments = True
+    use_notes_as_comments: bool = True
 
     #
     #  If false, scripts are saved in scripts/ inside the tmux conf dir
     #
-    use_embedded_scripts = True
+    use_embedded_scripts: bool = True
 
     #
     #  Indicates if this host is low on performance, don't enable
     #  demanding plugins etc, I use this on my iSH nodes.
     #  This must be set during __init__(). It is assumed to alreadt been
     #  set to the intended state when self.run() is done.
     #
     #  The only usage of this in this package is to propagate it to
     #  the plugin handler, indicating as plugins are installed and
     #  activated, since this might take a noticeable time on slowe nodes.
     #  It is also avaiable in derived plugin_ methods
     #
     #  Other usages of this is up to implementation classes
     #
-    is_limited_host = False
+    is_limited_host: bool = False
 
-    #
-    #  Default binary, if non given
-    #
-    tmux_bin = "tmux"
-
-    lib_version = __version__
+    lib_version: str = __version__
 
     def __init__(
         self,
         parse_cmd_line: bool = True,
         #
         #  if parse_cmd_line is True all other parameters are ignored
         #
         conf_file: str = "~/.tmux.conf",  # where to store conf file
-        tmux_bin: str = "tmux",
+        tmux_bin: str = "tmux",  #  Default binary, if none given
         tmux_version: str = "",
         replace_config: bool = False,  # replace config with no prompt
         clear_plugins: bool = False,  # remove all current plugins
         plugins_display: int = 0,  # Display info about plugins
         # then terminate
     ):
         if parse_cmd_line:
@@ -106,17 +101,15 @@
             conf_file = args.conf_file
             tmux_bin = args.tmux_bin
             tmux_version = args.forced_version
             replace_config = args.replace
             clear_plugins = args.clear_plugins
             plugins_display = args.plugins_display
 
-        if not tmux_bin:
-            # Use default for class
-            tmux_bin = self.tmux_bin
+        self.tmux_bin = ""
 
         #  cant use self.is_tmate() at this point, since self.tmux_bin
         #  is not yet set
         if tmux_bin.find("tmate") > -1:
             #  Set tmate defaults
             if not tmux_version:
                 tmux_version = "2.4"
@@ -132,36 +125,29 @@
         self.e_c_has_been_called = False
         self._write_stdout = False
 
         print(f"Processing: {__main__.__file__}")
 
         self.conf_file = verify_conf_file_usable(conf_file)
 
-        #
-        #  add the class to have the functionality needed during
-        #  self.find_tmux_bin(), it will later be called again with
-        #  the version details for the actually used version
-        #
-        # self.define_tmux_vers()
-
         self.find_tmux_bin(tmux_bin, requested_vers=tmux_version)
-        if tmux_version and (tmux_version != self.vers.get()):
+        if tmux_version and (tmux_version != self.vers.get()):  # type: ignore
             # self.define_tmux_vers(tmux_version)
             if not self.is_tmate():
                 #
                 #  Only display off version info when bin is tmux
                 #
                 print()
                 print(
                     "Config has been requested for another version of tmux,"
                     + " than the one used to generate this.\n"
                     + "Since the config file will point to the tmux used, "
                     + "this might cause problems\n"
-                    + f"\ttmux vers is:    {self.vers.get_actual()}\n"
-                    + f"\trequested vers:  {self.vers.get()}"
+                    + f"\ttmux vers is:    {self.vers.get_actual()}\n"  # type: ignore
+                    + f"\trequested vers:  {self.vers.get()}"  # type: ignore
                 )
                 print()
                 print("WARNING: Running this config with the current tmux")
                 print("         might give some errors!")
                 print()
         self.replace_config = replace_config
         self.plugins_display = plugins_display
@@ -175,15 +161,15 @@
         if not self.vers_ok("1.9") and self.plugin_handler:
             # tpm not available before 1.9, since it was defined, ensure
             # this is set to manual
             self.plugin_handler = "manual"
 
         self.plugins = Plugins(
             conf_file=self.conf_file,
-            vers_class=self.vers,
+            vers_class=self.vers,  # type: ignore
             es_class=self.es,
             plugin_handler=self.plugin_handler,
             clear_plugins=clear_plugins,
             plugins_display=plugins_display,
         )
         self.write_enable(
             False
@@ -281,16 +267,16 @@
         w("\n")
 
     # ================================================================
     #
     #  Some general methods that might be useful
     #
     # ================================================================
-    def vers_ok(self, vers) -> bool:
-        return self.vers.is_ok(vers)
+    def vers_ok(self, vers: str) -> bool:
+        return self.vers.is_ok(vers)  # type: ignore
 
     # ================================================================
     #
     #        Rest is mostly for internal usage
     #
     # ================================================================
 
@@ -340,37 +326,37 @@
         #
         #  Should be called as late as possible, to be able to have
         #  gathered all the intended embedded scripts.
         #
         for line in self.es.content():
             self.write(line)
 
-    def list_plugin_methods(self):
+    def list_plugin_methods(self) -> list[Callable[[], list[str]]]:
         """Support for plugins.py, provides a list of all plugin_... methods"""
         plugin_mthds: list[Callable[[], list[str]]] = []
         if self.plugin_handler:
             for item in dir(self):
                 if item.find("plugin_") or item == "plugin_handler":
                     continue
                 plugin_mthds.append(getattr(self, item))
         return plugin_mthds
 
-    def write_enable(self, state: bool):
+    def write_enable(self, state: bool) -> None:
         self._write_enabled = state
 
-    def conf_file_header(self):
+    def conf_file_header(self) -> None:
         """Creates the conf-file header & sets a few env variables about
         what tmux and config file is used, so that external commands
         know what to call if needed.
         """
         self.remove_conf_file()
         self._write_stdout = False
         self.write_enable(True)
 
-        print(f"Writing tmux {self.vers.get()} config to {self.conf_file}")
+        print(f"Writing tmux {self.vers.get()} config to {self.conf_file}")  # type: ignore
 
         w = self.write
         if self.use_embedded_scripts:
             w(
                 """# : << EMBEDDED-SCRIPTS-STARTING-POINT
             #
             # The above line tells embedded scripts where they start
@@ -380,44 +366,50 @@
         w(
             f"""#
         #  This config was created using
         #      https://github.com/jaclu/tmux-conf
         #
         #      Creation time: {datetime.now().strftime("%y-%m-%d %H:%M:%S")}
         #          tmux-conf: {self.lib_version}
-        #         Created on: {run_shell('hostname').strip()}
-        #        Source file: {__main__.__file__}
-        # """
+        #         Created on: {run_shell('hostname').strip()}"""
         )
-        if self.vers.get() != self.vers.get_actual():
-            w(f"#     actual version: ({self.vers.get_actual()})")
+        if self.vers.get() != self.vers.get_actual():  # type: ignore
+            w(f"#     actual version: ({self.vers.get_actual()})")  # type: ignore
+        w(f"#   For tmux version: {self.vers.get()}")  # type: ignore
         w(
-            f"""#   For tmux version: {self.vers.get()}
+            f"""#
         #
-        #  Since this is a compiled config file, please examine $TMUX_SOURCE
-        #  for what generated this. That is the right place for any changes
-        #  and to examine comments about what is generated and why.
-        #  This .conf file will frequently be over-written!
+        #  Three env variables defining this instance of tmux:
         #
-        TMUX_SOURCE="{__main__.__file__}"
+
+        #
+        #  When you might use various tmux instances or tmux is not in
+        #  path, the safe bet is to allways use $TMUX_BIN in a shell, not tmux!
+        #
+        TMUX_BIN="{self.tmux_bin}"
 
         #
         #  Helper pointitng to what conf file defines this env
+        #  If you want to source the config, especially if the config
+        #  might not be in the default location do:
+        #    $TMUX_BIN source $TMUX_CONF
         #
         TMUX_CONF="{self.conf_file}"
 
         #
-        #  tpm and other apps can use this env variable to use the
-        #  "right" tmux binary if you run multiple tmux versions.
+        #  Since this is a compiled config file, please examine $TMUX_SOURCE
+        #  for what generated this. That is the right place for any changes
+        #  and to examine comments about what is generated and why.
+        #  This .conf file will frequently be over-written!
         #
-        TMUX_BIN="{self.tmux_bin}"
+        TMUX_SOURCE="{__main__.__file__}"
         """
         )
 
-    def write(self, cmd: str = "", eol: str = "\n"):
+    def write(self, cmd: str = "", eol: str = "\n") -> None:
         """Writes tmux cmds to config file
 
         Filters out -N "note" statements if not supported, so they can
         always be supplied, regardless of tmux version.
 
         Can handle single and multi line commands, prints LF as a suffix.
         """
@@ -452,15 +444,15 @@
                     raise SyntaxError(
                         "Un-escaped back-ticks can not be present in "
                         + "the generated config when\n"
                         + "embedded_scripts are used!"
                     )
                 f.write(f"{line}{eol}")
 
-    def filter_note(self, line: str):
+    def filter_note(self, line: str) -> list[str]:
         """Returns list of lines, if notes are not supported
         first an empty spacer line, then the note as a comment,
         and finally the actual command without the note
         if self.use_notes_as_comments is False
         only the third line from above is returned
         """
 
@@ -497,65 +489,67 @@
             return ["", f"#  {note}", new_line]
 
         return [new_line]
 
     #
     #  Should conf file be replaced?
     #
-    def verify_replace(self):
+    def verify_replace(self) -> None:
         """Get verification that a config should be over-written
         the param replace_config=True skips this check
         """
         default_conf_file = os.path.expanduser("~/.tmux.conf")
         if self.conf_file == default_conf_file:
             self.check_replace_default_config()
         elif os.path.exists(self.conf_file):
             self.check_replace_custom_config()
 
-    def check_replace_default_config(self):
+    def check_replace_default_config(self) -> None:
         if os.path.isfile(self.conf_file) or os.path.islink(self.conf_file):
             confirmation = input(
                 "Do you wish to replace the default config file (y/n)?"
             )
         else:
             confirmation = input("Do you wish to create a default config file (y/n)?")
         if confirmation not in ("y", "Y"):
             print("Terminating...")
             sys.exit(1)
 
-    def check_replace_custom_config(self):
+    def check_replace_custom_config(self) -> None:
         confirmation = input(f"Do you wish to replace {self.conf_file} (y/n)?")
         if confirmation not in ("y", "Y"):
             print("Terminating...")
             sys.exit(1)
 
     #
     #  Selecting tmux bin
     #
-    def find_tmux_bin(self, cmd: str = "", requested_vers: str = "") -> bool:
+    def find_tmux_bin(self, cmd: str = "", requested_vers: str = "") -> None:
         """if tmux should use a specific version, when generating config
         set requested_vers parameter, if empy the actual version is used
+        if found, will set self.tmux_bin and more
+        if not Raises exception
         """
         if not cmd:
             #  Use the first that gives something
-            cmd = self.find_cmd_1() or self.find_cmd_2() or self.find_cmd_3()
+            cmd = self.find_cmd_1() or self.full_path_cmd() or self.find_cmd_3()
 
         if not cmd:
             raise TmuxConfNotTmuxCommand("No tmux command found")
         self.expand_cmd_path(cmd, requested_vers)
 
         # ==== 1 =
 
         if not self.tmux_bin:
             #  tmux not found abort
             print("ERROR could not find tmux binary, aborting")
             sys.exit(1)
-        return True
+        return
 
-    def find_cmd_1(self):
+    def find_cmd_1(self) -> str:
         """First check is to see if the tmux used to generate the
         previous config can be extracted.
         """
         cmd = ""
         if os.path.isfile(self.conf_file):
             s = f'grep "TMUX_BIN=" {self.conf_file} | cut -d= -f 2 | sed s/\\"//g'
             c = run_shell(s).strip()
@@ -564,58 +558,49 @@
             c2 = shutil.which(c)  # try to expand full path if not given
             if not c2:
                 return ""
             cmd = c2
             print(f"found {cmd} in conf file")
         return cmd
 
-    def find_cmd_2(self):
-        """Next check PATH"""
-        print("find_cmd_2()")
-        return self.full_path_cmd()
-
-    def find_cmd_3(self):
+    def find_cmd_3(self) -> str:
         """Finally try some likely locations"""
         cmd = ""
         for c in (
             "/usr/local/bin/tmux",
             "/home/linuxbrew/.linuxbrew/bin/tmux",
             "~/.asdf/shims/tmux",
         ):
             c2 = expanduser_plus(c)
             if is_executable(c2):
                 cmd = c2
+                print(f"found {cmd} manually")
                 break
         return cmd
 
-    def use_tmux_bin(self, tmux_bin="tmux", requested_vers=""):
+    def use_tmux_bin(self, tmux_bin: str = "tmux", requested_vers: str = "") -> bool:
         """Returns True if this was a valid tmux bin
         If this was the case self.tmux_bin & self.vers will have been set
         """
         parts = run_shell(f"{tmux_bin} -V").split(" ")
         if len(parts) != 2 or parts[0] not in ("tmux", "tmate"):
             raise TmuxConfNotTmuxCommand("{tmux} Doesnt seem to be a tmux binary")
-        #
-        #  Ensure version generated for a previous tmux bin is not still
-        #  arround
-        #
-        self.vers = None
 
         vers = VersionCheck(actual_vers=parts[1], requested_vers=requested_vers)
         # except TmuxConfInvalidTmuxVersion:
         #     print("{parts[[1]} Doesnt seem to be a valid tmux version")
         #     return False
         self.tmux_bin = tmux_bin
         self.vers = vers
         return True
 
     #
     #  Various attempt at finding the tmux bin
     #
-    def expand_cmd_path(self, cmd, requested_vers=""):
+    def expand_cmd_path(self, cmd: str, requested_vers: str = "") -> None:
         """If this is an asdf tmux, we need to translate path from shim
         to actual bin, in order to ptoperly detect version, but make sure
         not to expand an asdf path that has already been processed!
 
         Any process starting in the same dir as tmux was started will
         inherrit potential local asdf tmux selection, but processes
         starting in other dirs will use asdf default version.
@@ -636,87 +621,25 @@
                 print(f"ERROR: asdf tmux does not seem to be valid: {cmd}")
                 sys.exit(1)
             #
             #  Convert asdf shim into absolute path
             #
             cmd_asdf = (
                 f'{cmd.split("shims/")[0]}installs/tmux/'
-                f'{self.vers.get().split("-",maxsplit=1)[0]}/bin/tmux'
+                f'{self.vers.get().split("-",maxsplit=1)[0]}/bin/tmux'  # type: ignore
             )
             self.use_tmux_bin(cmd_asdf)
 
-    def full_path_cmd(self, cmd="tmux"):
+    def full_path_cmd(self, cmd: str = "tmux") -> str:
         c = run_shell(f"command -v {cmd}")
         if c and c.lower().find("not found") < 0:
             cmd = c
             print(f"found {cmd} in PATH")
         return cmd
 
-    def remove_conf_file(self):
+    def remove_conf_file(self) -> None:
         if os.path.exists(self.conf_file):
             #  Ensure we start with an empty file
             os.remove(self.conf_file)
 
-    # def extract_tmux_vers(self, vers_str_in):
-    #     parts = vers_str_in.split(".")
-    #     if len(parts) != 2:
-    #         raise TmuxConfInvalidTmuxVersion("Version string is not two parts separated by '.'")
-    #     try:
-    #         maj = int(parts[0])
-    #     except ValueError as exc:
-    #         raise TmuxConfInvalidTmuxVersion(
-    #             f"First part of version string is not int: {parts[0]}"
-    #         ) from exc
-
-    #     #  loop over parts[1] as long as each char is an int, then
-    #     #  ensure next char is a-z
-    #     return maj, min
-
-    # def use_tmux_bin(self, cmd: str):
-    #     """Verify this is a valid tmux, and store its path & version
-
-    #     self.tmux_bin   The tmux used
-    #     self.tmux_vers  The version used
-
-    #     """
-    #     # Do a basic sanity check
-    #     if self.is_tmux_bin(cmd):
-    #         self.tmux_bin = cmd
-    #         self.define_tmux_vers(tmux_bin=cmd)
-    #     else:
-    #         sys.exit(f"ERROR: tmux bin seems invalid: {cmd}")
-
-    def is_tmate(self):
+    def is_tmate(self) -> bool:
         return self.tmux_bin.find("tmate") > -1
-
-    # def is_tmux_bin(self, cmd: str) -> bool:
-    #     """Only checks if the requested bin seems to be a tmux or tmate,
-    #     checking name and doing simplified version check, ie if
-    #     the second part of version is int"""
-    #     if not cmd:
-    #         raise SyntaxError("cmd empty")
-    #     c = shutil.which(cmd)
-    #     if not c:
-    #         raise SyntaxError(f"tmux cmd not found: {cmd}")
-    #     cmd = c
-    #     output = run_shell(f"{cmd} -V")
-    #     name, v = output.split()
-    #     if name not in ("tmux", "tmate"):
-    #         return False
-    #     # i, _ = self.vers.get_sub_vers(v.split(".")[1])
-    #     i = v.split(".")[0]
-    #     try:
-    #         int(i)
-    #     except ValueError:
-    #         return False
-    #     return True
-
-    # #  TODO: use a better name
-    # def define_tmux_vers(self, vers="", tmux_bin: str = "tmux"):
-    #     if not tmux_bin:
-    #         tmux_bin = self.tmux_bin
-    #     vers_found = run_shell(f"{tmux_bin} -V | cut -d' ' -f2")
-    #     if not vers_found:
-    #         raise FileNotFoundError(
-    #             f"tmux: [{tmux_bin}] does not seem to be a tmux bin"
-    #         )
-    #     self.vers = VersionCheck(vers_found, vers)
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf/utils.py` & `tmux_conf-0.16.3/src/tmux_conf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 def is_executable(cmd: str) -> bool:
     fpath = os.path.expanduser(cmd)
     return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
 
 
-def parse_cmdline(args):
+def parse_cmdline(args: list[str]):
     parser = argparse.ArgumentParser(
         description="This tmux conf compiler generates configs for tmux "
         + "versions 1.5 and up."
     )
 
     #  Prints tmux-conf version info then exits
     parser.add_argument(
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf/vers_check.py` & `tmux_conf-0.16.3/src/tmux_conf/vers_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  Class that handles version checking
 #
 #  See the README.md in the repository for more info
 #
 
 
 class VersionCheck:
-    def __init__(self, actual_vers, requested_vers=None):
+    def __init__(self, actual_vers: str, requested_vers: str = ""):
         self._vers_actual = self.normalize_vers(actual_vers)
         if requested_vers:
             self._vers = self.normalize_vers(requested_vers)
         else:
             self._vers = self._vers_actual
         #
         #  For performance, the version parts are pre-calculated
@@ -43,15 +43,15 @@
         """The version used for generating the config"""
         return self._vers
 
     def get_actual(self):
         """The version of the tmux bin"""
         return self._vers_actual
 
-    def is_ok(self, vers) -> bool:
+    def is_ok(self, vers: str) -> bool:
         """Checks version vs current tmux environment
         Param is forgiving, can be int, float or string.
         When given as int .0 is appended
         In many cases a float is sufficient, like 2.8, 3.0 etc
         Some versions have character suffixes like 3.3a, then a string
         param is needed. Internally version refs are allways treated as
         strings.
@@ -74,15 +74,15 @@
         r = True
         if vers_min > self.v_min:
             r = False
         elif vers_min == self.v_min and suffix > self.v_suffix:
             r = False
         return r
 
-    def get_sub_vers(self, v2: str):
+    def get_sub_vers(self, v2: str) -> tuple[int, str]:
         int_part = ""
         for c in v2:
             try:
                 int(c)
             except ValueError:
                 break
             int_part += c
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf.egg-info/PKG-INFO` & `tmux_conf-0.16.3/src/tmux_conf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmux-conf
-Version: 0.16.0
+Version: 0.16.3
 Summary: Generates version checked tmux conf
 Author-email: Jacob Lundqvist <Jacob.Lundqvist@gmail.com>
 Project-URL: Homepage, https://github.com/jaclu/tmux-conf
 Project-URL: documentation, https://github.com/jaclu/tmux-conf
 Project-URL: repository, https://github.com/jaclu/tmux-conf
 Project-URL: Bug Tracker, https://github.com/jaclu/tmux-conf/issues
 Keywords: tmux,automation
```

### Comparing `tmux_conf-0.16.0/src/tmux_conf.egg-info/SOURCES.txt` & `tmux_conf-0.16.3/src/tmux_conf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/tests/test_embeded_scripts.py` & `tmux_conf-0.16.3/tests/test_embeded_scripts.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/tests/test_plugins.py` & `tmux_conf-0.16.3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/tests/test_tmux_conf.py` & `tmux_conf-0.16.3/tests/test_tmux_conf.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/tests/test_utils.py` & `tmux_conf-0.16.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmux_conf-0.16.0/tests/test_vers_check.py` & `tmux_conf-0.16.3/tests/test_vers_check.py`

 * *Files identical despite different names*

