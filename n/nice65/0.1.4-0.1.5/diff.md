# Comparing `tmp/nice65-0.1.4.tar.gz` & `tmp/nice65-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.1.4.tar", last modified: Sat Aug  5 21:43:26 2023, max compression
+gzip compressed data, was "nice65-0.1.5.tar", last modified: Sat Aug  5 21:47:29 2023, max compression
```

## Comparing `nice65-0.1.4.tar` & `nice65-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:43:26.014564 nice65-0.1.4/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.4/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     4152 2023-08-05 21:43:26.014564 nice65-0.1.4/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3732 2023-08-05 21:42:07.000000 nice65-0.1.4/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:43:26.014564 nice65-0.1.4/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.4/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.4/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)    10228 2023-08-05 21:38:41.000000 nice65-0.1.4/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:43:26.014564 nice65-0.1.4/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     4152 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 21:43:25.000000 nice65-0.1.4/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 21:43:13.000000 nice65-0.1.4/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 21:43:26.014564 nice65-0.1.4/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:47:29.494564 nice65-0.1.5/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.1.5/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     4152 2023-08-05 21:47:29.494564 nice65-0.1.5/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3732 2023-08-05 21:47:01.000000 nice65-0.1.5/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:47:29.494564 nice65-0.1.5/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.1.5/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.1.5/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     9890 2023-08-05 21:46:12.000000 nice65-0.1.5/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-05 21:47:29.494564 nice65-0.1.5/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     4152 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-05 21:47:29.000000 nice65-0.1.5/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-05 21:47:23.000000 nice65-0.1.5/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-05 21:47:29.494564 nice65-0.1.5/setup.cfg
```

### Comparing `nice65-0.1.4/LICENSE` & `nice65-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.1.4/PKG-INFO` & `nice65-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.4
+Version: 0.1.5
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.1.4/README.md` & `nice65-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nice65-0.1.4/nice65/app.py` & `nice65-0.1.5/nice65/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     'bra', 'phx', 'phy', 'plx', 'ply',
     'rmb0', 'rmb1', 'rmb2', 'rmb3', 'rmb4', 'rmb5', 'rmb6', 'rmb7',
     'smb0', 'smb1', 'smb2', 'smb3', 'smb4', 'smb5', 'smb6', 'smb7',
     'stp', 'stz', 'trb', 'tsb', 'wai',
     # fmt: on
 ]
 
-# COL1_COMMANDS = {'segment', 'zeropage', 'data', 'code', 'bss', 'include', 'import', 'importzp', 'export', 'exportzp'}
+COL1_COMMANDS = {'segment', 'zeropage', 'data', 'code', 'bss', 'include', 'import', 'importzp', 'export', 'exportzp'}
 
 instructions = INSTRUCTIONS + CMOS_INSTRUCTIONS
 
 instructions_def = " | ".join(['"' + instr + '"i' for instr in instructions])
 
 
 def main():
@@ -79,20 +79,14 @@
     parser.add_argument(
         "-l",
         "--colonless-labels",
         help="Allow labels without a colon (this option breaks macros, use with legacy code only)",
         action="store_true",
     )
     parser.add_argument(
-        "-i",
-        "--indent-control-commands",
-        help="Add indents to control commands even if they start at first column",
-        action="store_true",
-    )
-    parser.add_argument(
         "-v",
         "--version",
         help="Show version",
         nargs=0,
         action=Version,
     )
     args = parser.parse_args()
@@ -142,33 +136,32 @@
 
     if args.recursive:
         for root, _, files in os.walk(args.infile):
             for file in files:
                 if fnmatch.fnmatch(file, args.pattern):
                     path = os.path.join(root, file)
                     print("Fixing", path, file=sys.stderr)
-                    fix(grammar, path, None, True, args.colonless_labels, args.indent_control_commands)
+                    fix(grammar, path, None, True, args.colonless_labels)
     else:
         fix(
             grammar,
             args.infile,
             args.outfile,
             args.modify_in_place,
             args.colonless_labels,
-            args.indent_control_commands,
         )
 
 
 class Version(Action):
     def __call__(self, parser, namespace, values, option_string):
         print('nice65 version', metadata.version("nice65"), file=sys.stderr)
         parser.exit()
 
 
-def fix(grammar, infile, outfile, modify_in_place, colonless_labels, indent_control_commands):
+def fix(grammar, infile, outfile, modify_in_place, colonless_labels):
     if infile == "-":
         content = sys.stdin.read()
     else:
         with open(infile, "r") as fobj:
             content = fobj.read()
             options_match = re.findall(r'^[ \t]*;\s*nice65:([^\n]+)$', content, re.MULTILINE)
             if options_match:
@@ -227,18 +220,21 @@
                 else:
                     padding = "\n" + " " * 8
 
                 statement = child.children[0]
 
                 if statement.data == "control_command":
                     name = statement.children[0].strip()
-                    if not len(string) and not indent_control_commands:
-                        # If this is the first statement in line and indent_control_commands is not set - don't indent
-                        padding = ''
-                    string += padding + "." + name.lower() + " " + " ".join(statement.children[1:])
+                    string += (
+                        (padding if name not in COL1_COMMANDS else '')
+                        + "."
+                        + name.lower()
+                        + " "
+                        + " ".join(statement.children[1:])
+                    )
                 elif statement.data == "macro_start":
                     name = statement.children[0].strip()
                     string += ".macro ".ljust(8, ' ') + name + " " + ", ".join(map(str.strip, statement.children[1:]))
                 elif statement.data == "macro_end":
                     string += ".endmacro"
                 elif statement.data == "asm_statement":
                     mnemonic = statement.children[0]
```

### Comparing `nice65-0.1.4/nice65.egg-info/PKG-INFO` & `nice65-0.1.5/nice65.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.1.4
+Version: 0.1.5
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.1.4/pyproject.toml` & `nice65-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

