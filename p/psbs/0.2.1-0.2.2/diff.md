# Comparing `tmp/psbs-0.2.1.tar.gz` & `tmp/psbs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.2.1.tar", last modified: Fri Aug  4 20:38:03 2023, max compression
+gzip compressed data, was "psbs-0.2.2.tar", last modified: Sun Aug  6 15:07:41 2023, max compression
```

## Comparing `psbs-0.2.1.tar` & `psbs-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 20:38:03.653699 psbs-0.2.1/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.1/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-04 20:38:03.653848 psbs-0.2.1/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.2.1/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 20:38:03.647154 psbs-0.2.1/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.1/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.1/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.1/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.1/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/extension.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 20:38:03.653161 psbs-0.2.1/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.1/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/extensions/build.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      433 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/extensions/filters.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/extensions/tiled.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.2.1/psbs/gister.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1764 2023-08-04 20:26:04.000000 psbs-0.2.1/psbs/htmlbuilder.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4469 2023-08-04 19:54:46.000000 psbs-0.2.1/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     3142 2023-08-04 20:08:13.000000 psbs-0.2.1/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     9525 2023-08-04 19:01:45.000000 psbs-0.2.1/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3044 2023-08-04 01:50:46.000000 psbs-0.2.1/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.2.1/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.1/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 20:38:03.650109 psbs-0.2.1/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-04 20:38:03.000000 psbs-0.2.1/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-04 20:38:03.654467 psbs-0.2.1/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-04 20:36:53.000000 psbs-0.2.1/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.699320 psbs-0.2.2/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.2/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-06 15:07:41.699504 psbs-0.2.2/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.2.2/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.693590 psbs-0.2.2/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.2/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.2/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.2/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.2/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.698894 psbs-0.2.2/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.2/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/build.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      451 2023-08-06 12:49:36.000000 psbs-0.2.2/psbs/extensions/filters.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/extensions/tiled.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.2.2/psbs/gister.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1820 2023-08-06 15:04:23.000000 psbs-0.2.2/psbs/htmlbuilder.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4301 2023-08-06 14:09:41.000000 psbs-0.2.2/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-08-06 14:10:04.000000 psbs-0.2.2/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     9382 2023-08-06 15:00:57.000000 psbs-0.2.2/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3044 2023-08-04 01:50:46.000000 psbs-0.2.2/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-08-04 23:04:04.000000 psbs-0.2.2/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.2/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-06 15:07:41.696649 psbs-0.2.2/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-06 15:07:41.000000 psbs-0.2.2/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-06 15:07:41.700371 psbs-0.2.2/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-06 15:04:41.000000 psbs-0.2.2/setup.py
```

### Comparing `psbs-0.2.1/LICENSE` & `psbs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/PKG-INFO` & `psbs-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.1
+Version: 0.2.2
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.1/README.md` & `psbs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/example.txt` & `psbs-0.2.2/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/extension.py` & `psbs-0.2.2/psbs/extension.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/extensions/build.py` & `psbs-0.2.2/psbs/extensions/build.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/extensions/images.py` & `psbs-0.2.2/psbs/extensions/images.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/extensions/tiled.py` & `psbs-0.2.2/psbs/extensions/tiled.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/gister.py` & `psbs-0.2.2/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/htmlbuilder.py` & `psbs-0.2.2/psbs/htmlbuilder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-from requests import get
 from json import dumps
 from os import path
+from requests import get
 
 from .psparser import PSParser
 from .utils import write_file
 
+
 def build_html(engine, source):
-    standalone_url = "/".join(
-        engine.split("/")+["standalone_inlined.txt"]
-    )
-    response = get(standalone_url)
+    standalone_url = "/".join(engine.split("/") + ["standalone_inlined.txt"])
+    response = get(standalone_url, timeout=5)
     if response.status_code != 200:
         print("Error: Can't build html game")
         print(f"  Unable to download {standalone_url}")
         print(f"  Server response: {response.status_code}")
         raise SystemExit(1)
-    standalone_html = response.content.decode('UTF-8')
+    standalone_html = response.content.decode("UTF-8")
     parser = PSParser(source)
     title = parser.prelude_options.get("title", "My Game")
     homepage = parser.prelude_options.get("homepage", engine)
     if "://" in homepage:
-        homepage_stripped_protocol = homepage.split("://",1)[1]
+        homepage_stripped_protocol = homepage.split("://", 1)[1]
     else:
         homepage_stripped_protocol = homepage
-    standalone_html = standalone_html.replace("__GAMETITLE__", parser.prelude_options.get("title", "My Game"))
+    standalone_html = standalone_html.replace(
+        "__GAMETITLE__", parser.prelude_options.get("title", "My Game")
+    )
     standalone_html = standalone_html.replace("__HOMEPAGE__", homepage)
-    standalone_html = standalone_html.replace("__HOMEPAGE_STRIPPED_PROTOCOL__", homepage_stripped_protocol)
-    standalone_html = standalone_html.replace("___BGCOLOR___", parser.prelude_options.get("background_color", "black"))
-    standalone_html = standalone_html.replace("___TEXTCOLOR___", parser.prelude_options.get("text_color", "lightblue"))
-    # for some reason some older forks have extra quotes that need to be removed
-    standalone_html = standalone_html.replace("\"__GAMEDAT__\"", dumps(source))
+    standalone_html = standalone_html.replace(
+        "__HOMEPAGE_STRIPPED_PROTOCOL__", homepage_stripped_protocol
+    )
+    standalone_html = standalone_html.replace(
+        "___BGCOLOR___",
+        parser.prelude_options.get("background_color", "black"),
+    )
+    standalone_html = standalone_html.replace(
+        "___TEXTCOLOR___",
+        parser.prelude_options.get("text_color", "lightblue"),
+    )
+    # for some reason some older forks have extra quotes
+    standalone_html = standalone_html.replace('"__GAMEDAT__"', dumps(source))
     standalone_html = standalone_html.replace("__GAMEDAT__", dumps(source))
 
-    filename = path.join("bin",title+".html")
-    write_file(path.join("bin",title+".html"),standalone_html)
+    filename = path.join("bin", title + ".html")
+    write_file(path.join("bin", title + ".html"), standalone_html)
     return filename
```

### Comparing `psbs-0.2.1/psbs/project.py` & `psbs-0.2.2/psbs/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .template import Template
 from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
 
 
 class PSBSProject:
     def __init__(self, config_filename="config.yaml"):
         self.config = Config(config_filename)
+        self.filename = None
 
     def build(self):
         # Check for target directory
         if not path.exists("bin"):
             print("bin directory does not exist, creating one")
             make_dir("bin")
 
@@ -40,36 +41,28 @@
 
         print(f"Writing file {script_path}")
         write_file(script_path, template.render())
 
     def export(self):
         if not self.config["gist_id"]:
             print("Writing game to html file")
-            return build_html(
+            self.filename = build_html(
                 self.config["engine"],
-                read_file(path.join("bin", "script.txt"))
+                read_file(path.join("bin", "script.txt")),
             )
         else:
-            self.upload()
-            return None
+            print("Updating gist")
+            gist = Gister(gist_id=self.config["gist_id"])
+            gist.write(path.join("bin", "readme.txt"))
+            gist.write(path.join("bin", "script.txt"))
 
-    def upload(self):
-        if not self.config["gist_id"]:
-            print("Error: Unable to upload without a gist_id in config file")
-            raise SystemExit(1)
-
-        print("Updating gist")
-        gist = Gister(gist_id=self.config["gist_id"])
-        gist.write(path.join("bin", "readme.txt"))
-        gist.write(path.join("bin", "script.txt"))
-
-    def run(self, filename, editor=False):
+    def run(self, editor=False):
         print("Opening in browser")
-        if filename:
-            url = PurePath(path.abspath(filename)).as_uri()
+        if self.filename:
+            url = PurePath(path.abspath(self.filename)).as_uri()
         else:
             url = self.config["engine"]
             if editor:
                 url += "editor.html?hack="
             else:
                 url += "play.html?p="
             url += self.config["gist_id"]
```

### Comparing `psbs-0.2.1/psbs/psbs.py` & `psbs-0.2.2/psbs/psbs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from argparse import ArgumentParser, SUPPRESS
-from sys import argv
+from argparse import ArgumentParser
 
 from .project import PSBSProject
 from .token import get_token, set_token
 
 
 def main():
-
-    if len(argv) > 1 and argv[1].lower() == "upload":
-        print("Warning: Upload command deprecated, please use export instead in the future")
-        argv[1] = "export"
-
     parser = ArgumentParser(
         description="PSBS: PuzzleScript Build System", add_help=False
     )
     subparser = parser.add_subparsers(title="Commands", dest="command")
 
     commands_dict = {
         "build": "Build project in current working directory",
         "export": "Build project then export to game",
         "run": "Build project, export, then run in web browser",
         "new": "Create a new project",
         "token": "Check or set GitHub auth token",
-        "help": "Display help dialog"
+        "help": "Display help dialog",
     }
     commands = {}
     for command, help_text in commands_dict.items():
         commands[command] = subparser.add_parser(
             command, help=help_text, description=help_text, add_help=False
         )
 
@@ -84,15 +78,16 @@
     elif args.command == "export":
         project = PSBSProject()
         project.build()
         project.export()
     elif args.command == "run":
         project = PSBSProject()
         project.build()
-        project.run(project.export(),editor=args.editor)
+        project.export()
+        project.run(editor=args.editor)
     elif args.command == "new":
         PSBSProject.create(
             args.name,
             gist_id=args.gist_id,
             file=args.file,
             new_gist=args.new_gist,
         )
```

### Comparing `psbs-0.2.1/psbs/psparser.py` & `psbs-0.2.2/psbs/psparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,37 +91,41 @@
 
     def get_objects(self):
         object_strs = re.split(
             r"(?<=\S)\n+\n+(?=\S)", self.sections["objects"]
         )
         ps_objects = {}
         for object_str in object_strs:
-            object_str_lines = object_str.splitlines()
-            name = object_str_lines.pop(0)
-            if "case_sensitive" not in self.prelude_options:
-                name = name.lower()
-            colors = object_str_lines.pop(0)
-            body = "\n".join(object_str_lines)
-            # ps_objects[object_name] = body
-            # consider using dict:
-            synonyms = []
-            tokens_in_name = name.split()
-            if len(tokens_in_name) > 0:
-                name = tokens_in_name.pop(0)
-                for token in tokens_in_name:
-                    if token.startswith("copy:"):
-                        # handle PuzzleScript+ copy feature
-                        body = ps_objects[token[5:]]["body"]
-                    else:
-                        synonyms.append(token)
-            ps_objects[name] = {
-                "colors": colors,
-                "body": body,
-                "synonyms": synonyms,
-            }
+            try:
+                object_str_lines = object_str.splitlines()
+                name = object_str_lines.pop(0)
+                if "case_sensitive" not in self.prelude_options:
+                    name = name.lower()
+                colors = object_str_lines.pop(0)
+                body = "\n".join(object_str_lines)
+                # ps_objects[object_name] = body
+                # consider using dict:
+                synonyms = []
+                tokens_in_name = name.split()
+                if len(tokens_in_name) > 0:
+                    name = tokens_in_name.pop(0)
+                    for token in tokens_in_name:
+                        if token.startswith("copy:"):
+                            # handle PuzzleScript+ copy feature
+                            body = ps_objects[token[5:]]["body"]
+                        else:
+                            synonyms.append(token)
+                ps_objects[name] = {
+                    "colors": colors,
+                    "body": body,
+                    "synonyms": synonyms,
+                }
+            except IndexError:
+                print("Warning: unable to parse object:")
+                print(object_str)
         return ps_objects
 
     def get_glyphs(self):
         # Code Smell: this method is way too long, consider breaking
         # it up in the future however it's working pretty well for now
         legend = self.sections["legend"]
         ps_objects = self.get_objects()
@@ -157,76 +161,72 @@
                 synonyms[match.group(1)] = match.group(2)
         for ps_object in ps_objects:
             for synonym in ps_objects[ps_object]["synonyms"]:
                 synonyms[synonym] = ps_object
             synonyms[ps_object] = ps_object
         # resolve synonyms
         for synonym in synonyms:
-            if synonyms[synonym] in synonyms:
-                synonyms[synonym] = synonyms[synonyms[synonym]]
+            synonyms[synonym] = synonyms.get(
+                synonyms[synonym], synonyms[synonym]
+            )
 
         def resolve_dict(input_dict):
             must_recurse = True
             output = {}
             while must_recurse:
                 # This can loop forever if there are circular references
-                # consider adding a max number of loops
+                # consider adding a max number of loops maybe?
                 must_recurse = False
                 output = {}
                 for key in input_dict:
                     output[key] = []
                     for object_name in input_dict[key]:
                         if object_name in input_dict:
                             for inner_key in input_dict[object_name]:
-                                if inner_key in synonyms:
-                                    output[key].append(synonyms[inner_key])
-                                else:
-                                    output[key].append(inner_key)
+                                output[key].append(
+                                    synonyms.get(inner_key, inner_key)
+                                )
                         else:
-                            if object_name in synonyms:
-                                output[key].append(synonyms[object_name])
-                            else:
-                                output[key].append(object_name)
+                            output[key].append(
+                                synonyms.get(object_name, object_name)
+                            )
                 for key in output:
                     for object_name in output[key]:
                         if object_name in output:
                             must_recurse = True
                 input_dict = output
             return output
 
         properties = resolve_dict(properties)
         aggregates = resolve_dict(aggregates)
 
         glyphs = {}
         for synonym in synonyms:
             if len(synonym) == 1:
-                if synonyms[synonym] in aggregates:
-                    glyphs[synonym] = aggregates[synonyms[synonym]]
-                else:
-                    glyphs[synonym] = [synonyms[synonym]]
+                glyphs[synonym] = aggregates.get(
+                    synonyms[synonym], [synonyms[synonym]]
+                )
 
         for aggregate in aggregates:
             if len(aggregate) == 1:
                 glyphs[aggregate] = aggregates[aggregate]
 
         collision_order = []
         for collision_object in re.split(
             r",\s*|\s+", collisionlayers, flags=re.MULTILINE
         ):
             if collision_object in properties:
                 for inner_object in properties[collision_object]:
-                    if inner_object in synonyms:
-                        collision_order.append(synonyms[inner_object])
-                    else:
-                        collision_order.append(inner_object)
+                    collision_order.append(
+                        synonyms.get(inner_object, inner_object)
+                    )
             else:
-                if collision_object in synonyms:
-                    collision_order.append(synonyms[collision_object])
-                else:
-                    collision_order.append(collision_object)
+                collision_order.append(
+                    synonyms.get(collision_object, collision_object)
+                )
 
         for glyph in glyphs:
             if background_name not in glyphs[glyph]:
                 glyphs[glyph].append(background_name)
             try:
                 glyphs[glyph] = sorted(
                     glyphs[glyph], key=collision_order.index
```

### Comparing `psbs-0.2.1/psbs/template.py` & `psbs-0.2.2/psbs/template.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/token.py` & `psbs-0.2.2/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs/utils.py` & `psbs-0.2.2/psbs/utils.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/psbs.egg-info/PKG-INFO` & `psbs-0.2.2/psbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.1
+Version: 0.2.2
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.1.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.1/psbs.egg-info/SOURCES.txt` & `psbs-0.2.2/psbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.2.1/setup.py` & `psbs-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.2.1',
+    version='0.2.2',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.1.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.2.tar.gz',
     license='MIT',
     packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
```

