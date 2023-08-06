# Comparing `tmp/Artec-0.2.1.tar.gz` & `tmp/Artec-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Artec-0.2.1.tar", last modified: Sun Jul 16 20:31:22 2023, max compression
+gzip compressed data, was "Artec-0.3.0.tar", last modified: Sun Aug  6 10:42:43 2023, max compression
```

## Comparing `Artec-0.2.1.tar` & `Artec-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/Artec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 20:31:22.000000 Artec-0.2.1/Artec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-16 20:31:11.000000 Artec-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-16 20:31:22.537473 Artec-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-16 20:31:11.000000 Artec-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/artec/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-16 20:31:11.000000 Artec-0.2.1/artec/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-16 20:31:11.000000 Artec-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:31:22.537473 Artec-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 20:31:11.000000 Artec-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:31:22.537473 Artec-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-16 20:31:11.000000 Artec-0.2.1/test/test_boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-16 20:31:11.000000 Artec-0.2.1/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.295436 Artec-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/Artec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-06 10:42:33.000000 Artec-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-08-06 10:42:43.291436 Artec-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-08-06 10:42:33.000000 Artec-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/artec/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-06 10:42:33.000000 Artec-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:42:43.295436 Artec-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:42:33.000000 Artec-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_parser.py
```

### Comparing `Artec-0.2.1/LICENSE` & `Artec-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Artec-0.2.1/artec/argparser.py` & `Artec-0.3.0/artec/argparser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 """
-	Parser class is a wrapper for easy access of argparse module
+	Parser class is a wrapper for easy access of argparse module v2.1.0
 """
-from argparse import ArgumentParser, Namespace, RawTextHelpFormatter, _VersionAction
+from argparse import (
+    ArgumentParser,
+    Namespace,
+    RawTextHelpFormatter,
+    _VersionAction,
+)
 from .templates import templates
 import sys
 
 
 class list_templates(_VersionAction):
     def __call__(self, parser: ArgumentParser, *args, **kwargs) -> None:
         formatter = parser._get_formatter()
         formatter.add_text(
-            "Available templates\n\n"
-            + "\n".join([f"> {key.title()}\t" for key in templates.keys()])
+            "".join(
+                "Available templates\n\n",
+                "\n".join([f"> {key.title()}\t" for key in templates.keys()]),
+            )
         )
         parser._print_message(formatter.format_help(), sys.stdout)
         parser.exit()
 
 
 class Parser(ArgumentParser):
     def __init__(self, appVersion):
         self.appVersion = appVersion
         prog = "Artec"
         usage = "artec [OPTIONS] -o [DEST] "
-        description = "Artec is a simple python 3 script to create a project template in a given directory."
+        description = "Artec is a python application that creates a configurable python project template in a given directory."
         epilog = "Examples:\n\tartec -h\n\tartec -o dest\
-            \n\tartec -o dest -t python \n\tartec -o dest -s structure.json \n\tartec -o dest -s structure.json -v"
+            \n\tartec -o dest -t python \n\tartec -o dest -s structure.json\
+             \n\tartec -o dest -s structure.json -v"
         super().__init__(
-            prog, usage, description, epilog, formatter_class=RawTextHelpFormatter
+            prog,
+            usage,
+            description,
+            epilog,
+            formatter_class=RawTextHelpFormatter,
         )
 
     def setup(self):
         group = self.add_mutually_exclusive_group()
-        
         group.add_argument(
             "-s",
             "--source-file",
             dest="source",
             help="Source JSON file containing structure to be created",
             type=str,
             required=False,
@@ -61,32 +72,42 @@
         self.add_argument(
             "-ls",
             "--list-template",
             help="lists all ready-made templates.",
             action=list_templates,
         )
 
-
         self.add_argument(
             "-v",
             "--verbose",
             dest="verbose",
             help="Runs Artec in verbose mode.",
+            action="count",
+            default=0,
+            required=False,
+        )
+
+        self.add_argument(
+            "-g",
+            "--git-init",
+            dest="git",
+            help="Creates a git Repo for the project.",
             action="store_true",
             required=False,
         )
 
         self.add_argument(
             "-V",
             "--version",
             help="Display current version of Artec",
             action="version",
             version=f"{self.prog} {self.appVersion}",
         )
 
+
 def main_args(appVersion) -> Namespace:
     parser = Parser(appVersion)
     parser.setup()
     return parser.parse_args()
 
 
 if __name__ == "__main__":
```

### Comparing `Artec-0.2.1/artec/boiler.py` & `Artec-0.3.0/artec/boiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 """
 	Main module core.
 	#3 Step
 """
 import json
 import os
 from pathlib import Path
-from .exceptions import NotJsonFile, NotValidJson, NoSource, InValidTemplate
-from .templates import templates, static_list
-
+from . import exceptions as ex
+from . import templates as temps
+from . import repo 
+from . import logger 
 
 class boiler_builder:
-    def __init__(self, source=None, target=None, verbose=False, template=None) -> None:
-        self.verbose = verbose
+    def __init__(
+        self,
+        source: str = None,
+        target: str = None,
+        template: str = None,
+        git=False,
+    ) -> None:
         self.target = target
+        self.git = git
+        self.home_dir = os.path.abspath(os.path.curdir)
+
         if template is None:
             self.structure = self._source(source)
         else:
             self.structure = self._source_temp(template.lower())
 
     def _source_temp(self, template) -> list[dict[str, str]]:
         try:
-            if template in templates:
-                structure = templates[template].format(self.target)
+            if template in temps.templates:
+                structure = temps.templates[template].format(self.target)
             else:
-                raise InValidTemplate(self.verbose)
+                raise ex.InValidTemplate()
 
-        except InValidTemplate:
-            structure = templates["python"].format(self.target)
+        except ex.InValidTemplate:
+            structure = temps.templates["python"].format(self.target)
         return structure
 
     def _source(self, source) -> list[dict[str, str]]:
         try:
-            if source is None : 
-                raise NoSource(self.verbose)
+            if source is None:
+                raise ex.NoSource()
             if os.path.isfile(source) and source.endswith(".json"):
                 with open(source, "rt", encoding="utf-8") as file_data:
-                    structure = static_list(json.load(file_data)).format(self.target)
+                    structure = temps.static_list(json.load(file_data)).format(
+                        self.target
+                    )
             else:
-                raise NotJsonFile(self.verbose)
+                raise ex.NotJsonFile()
 
-        except Exception as e:
+        except Exception:
+            structure = temps.templates["python"].format(self.target)
 
-            structure = templates["python"].format(self.target)
         return structure
 
     def build(self):
         print("> Creating folder structure: {}\n".format(self.target))
 
         for entry in self.structure:
             for _type, name in entry.items():
                 try:
                     joined = Path(os.path.join(self.target, name))
-                    if "folder" in _type :
+                    if "folder" in _type:
                         self._make_folder(joined)
-                    elif "file" in _type :
+                    elif "file" in _type:
                         self._make_file(joined)
                     else:
-                        raise NotValidJson(self.verbose)
+                        raise ex.NotValidJson()
                     print("Created: %s" % joined)
                 except Exception:
-                    exit("> Fatal error - exiting...")
+                    pass
+        print()
+
+        if self.git:
+            try:
+                Repo = repo.repository(os.path.join(self.home_dir, self.target), self.target)
+                Repo.add()
+                    
+            except Exception as e :
+                ex.GitError(e)
 
     def _make_file(self, path):
         """Create an empty file in a given directory"""
         path.parent.mkdir(parents=True, exist_ok=True)
         open(path, "a").close()
 
     def _make_folder(self, path):
```

### Comparing `Artec-0.2.1/artec/templates.py` & `Artec-0.3.0/artec/templates.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,65 @@
+from . import exceptions as ex
+
+
 class static_list(list):
     def format(self, name):
-        for _ in self:
-            for i, j in _.items():
-                _[i] = j.format(name)
-        return self
+        try:
+            for _ in self:
+                for i, j in _.items():
+                    _[i] = j.format(name)
+            return self
+        except AttributeError:
+            raise ex.NotValidJson()
 
 
 PYTHON = static_list(
     [
         {"folder": "{}"},
         {"file": "{}/__init__.py"},
         {"folder": "test"},
         {"file": "test/__init__.py"},
         {"file": "README.md"},
         {"file": "LICENSE"},
         {"file": "setup.py"},
         {"file": "setup.cfg"},
-        {"file": "pyproject.toml"}
+        {"file": "pyproject.toml"},
+    ]
+)
+
+FLASK = static_list(
+    [
+        {"folder": "{}"},
+        {"file": "{}/__init__.py"},
+        {"file": "{}/db.py"},
+        {"file": "{}/schema.py"},
+        {"file": "{}/auth.py"},
+        {"file": "{}/blog.py"},
+        {"folder": "{}/templates"},
+        {"file": "{}/templates/base.html"},
+        {"folder": "{}/templates/auth/"},
+        {"file": "{}/templates/auth/login.html"},
+        {"file": "{}/templates/auth/register.html"},
+        {"folder": "{}/blog"},
+        {"file": "{}/blog/create.html"},
+        {"file": "{}/blog/index.html"},
+        {"file": "{}/blog/update.html"},
+        {"folder": "{}/static"},
+        {"file": "{}/static/style.css"},
+        {"folder": "test"},
+        {"file": "test/__init__.py"},
+        {"file": "test/conftest.py"},
+        {"file": "test/data.sql"},
+        {"file": "test/test_db.py"},
+        {"file": "test/test_auth.py"},
+        {"file": "test/test_blog.py"},
+        {"file": "README.md"},
+        {"file": "LICENSE"},
+        {"file": "setup.py"},
+        {"file": "pyproject.toml"},
     ]
 )
 
 NODE_JS = static_list(
     [
         {"folder": "src"},
         {"folder": "src/api"},
@@ -83,11 +122,13 @@
         {"file": ".env.sample"},
         {"file": "README.md"},
         {"file": "LICENSE"},
         {"file": "package.json"},
         {"file": "package-lock.json"},
     ]
 )
+
 templates = {
     "python": PYTHON,
     "node.js": NODE_JS,
+    "flask": FLASK,
 }
```

