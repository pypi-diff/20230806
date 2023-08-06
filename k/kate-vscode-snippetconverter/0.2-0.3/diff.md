# Comparing `tmp/kate-vscode-snippetconverter-0.2.tar.gz` & `tmp/kate-vscode-snippetconverter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kate-vscode-snippetconverter-0.2.tar", last modified: Fri Jun  3 07:53:15 2022, max compression
+gzip compressed data, was "kate-vscode-snippetconverter-0.3.tar", last modified: Sun Aug  6 13:05:02 2023, max compression
```

## Comparing `kate-vscode-snippetconverter-0.2.tar` & `kate-vscode-snippetconverter-0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-06-03 07:53:15.725442 kate-vscode-snippetconverter-0.2/
--rw-rw-r--   0 max       (1000) max       (1000)     1070 2022-06-03 06:49:08.000000 kate-vscode-snippetconverter-0.2/LICENSE.txt
--rw-rw-r--   0 max       (1000) max       (1000)      383 2022-06-03 07:53:15.725442 kate-vscode-snippetconverter-0.2/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      254 2022-06-03 07:14:30.000000 kate-vscode-snippetconverter-0.2/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-06-03 07:53:15.725442 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      383 2022-06-03 07:53:15.000000 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      399 2022-06-03 07:53:15.000000 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2022-06-03 07:53:15.000000 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       76 2022-06-03 07:53:15.000000 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/entry_points.txt
--rw-rw-r--   0 max       (1000) max       (1000)       17 2022-06-03 07:53:15.000000 kate-vscode-snippetconverter-0.2/kate_vscode_snippetconverter.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)       79 2022-06-03 07:53:15.725442 kate-vscode-snippetconverter-0.2/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      689 2022-06-03 07:52:26.000000 kate-vscode-snippetconverter-0.2/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2022-06-03 07:53:15.725442 kate-vscode-snippetconverter-0.2/snippetconverter/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2022-06-03 07:23:53.000000 kate-vscode-snippetconverter-0.2/snippetconverter/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     4822 2022-06-03 06:54:51.000000 kate-vscode-snippetconverter-0.2/snippetconverter/languages.py
--rwxr-xr-x   0 max       (1000) max       (1000)     6577 2022-06-03 07:52:06.000000 kate-vscode-snippetconverter-0.2/snippetconverter/snippetconverter.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-08-06 13:05:02.771878 kate-vscode-snippetconverter-0.3/
+-rw-rw-r--   0 max       (1000) max       (1000)     1070 2022-06-03 08:00:00.000000 kate-vscode-snippetconverter-0.3/LICENSE.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      420 2023-08-06 13:05:02.771878 kate-vscode-snippetconverter-0.3/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      513 2023-08-06 13:04:52.000000 kate-vscode-snippetconverter-0.3/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-08-06 13:05:02.771878 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/
+-rw-rw-r--   0 max       (1000) max       (1000)      420 2023-08-06 13:05:02.000000 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)      414 2023-08-06 13:05:02.000000 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2023-08-06 13:05:02.000000 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       77 2023-08-06 13:05:02.000000 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/entry_points.txt
+-rw-rw-r--   0 max       (1000) max       (1000)       17 2023-08-06 13:05:02.000000 kate-vscode-snippetconverter-0.3/kate_vscode_snippetconverter.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-08-06 13:04:52.000000 kate-vscode-snippetconverter-0.3/pyproject.toml
+-rw-rw-r--   0 max       (1000) max       (1000)       79 2023-08-06 13:05:02.771878 kate-vscode-snippetconverter-0.3/setup.cfg
+-rw-rw-r--   0 max       (1000) max       (1000)      689 2023-08-06 13:04:52.000000 kate-vscode-snippetconverter-0.3/setup.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-08-06 13:05:02.771878 kate-vscode-snippetconverter-0.3/snippetconverter/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2022-06-03 08:00:00.000000 kate-vscode-snippetconverter-0.3/snippetconverter/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4691 2023-08-06 13:04:52.000000 kate-vscode-snippetconverter-0.3/snippetconverter/languages.py
+-rwxrwxr-x   0 max       (1000) max       (1000)     5931 2023-08-06 13:04:52.000000 kate-vscode-snippetconverter-0.3/snippetconverter/snippetconverter.py
```

### Comparing `kate-vscode-snippetconverter-0.2/LICENSE.txt` & `kate-vscode-snippetconverter-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kate-vscode-snippetconverter-0.2/setup.py` & `kate-vscode-snippetconverter-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 LONG_DESCRIPTION = """\
 snippetconverter.py can convert the snippet used in Kate or KDevelop IDE to the VSCode IDE
 """
 
 setup(
     name="kate-vscode-snippetconverter",
-    version="0.2",
+    version="0.3",
     description="A tool to convert snippet from Kate/KDevelop to VSCode",
     long_description=LONG_DESCRIPTION,
     author="Maxime Haselbauer",
     author_email="maxime.haselbauer@googlemail.com",
     url="https://github.com/renn0xtek9/snippetconverter",
     packages=["snippetconverter"],
     install_requires=[""],
```

### Comparing `kate-vscode-snippetconverter-0.2/snippetconverter/languages.py` & `kate-vscode-snippetconverter-0.3/snippetconverter/languages.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             "YAML",
         ],
         count(),
     ),
 )
 
 
-def induce_language_from_file_name(filename):
+def induce_language_from_file_name(filename: str):
     """identify languaged of snippet file based on filename"""
     # pylint: disable=R0911
     # pylint: disable=R0912
     if "C++" in filename or "c++" in filename or "cpp" in filename or "Cpp" in filename:
         return LANGUAGES.CPP
     if "Python" in filename or "python" in filename:
         return LANGUAGES.PYTHON
@@ -99,15 +99,15 @@
     if "Bash" in filename:
         return LANGUAGES.SHELLSCRIPT
     if "SQL" in filename:
         return LANGUAGES.SQL
     raise Exception("Could not induce language from filename {}".format(filename))
 
 
-def get_language_identifier_for_vscode(language):
+def get_language_identifier_for_vscode(language: LANGUAGES):
     """get language identiger for vscode based on language"""
     languageidentifier = dict(
         {
             "ABAP": "abap",
             "BAT": "bat",
             "BIBTEX": "bibtex",
             "CLOJURE": "clojure",
@@ -158,12 +158,8 @@
             "TEX": "tex",
             "VB": "vb",
             "XML": "xml",
             "XSL": "xsl",
             "YAML": "yaml",
         }
     )
-    try:
-        return languageidentifier[language.name]
-    except ValueError:
-        print("No known VSCode language identifier for language {}".format(language))
-        raise ValueError
+    return languageidentifier[language.name]
```

### Comparing `kate-vscode-snippetconverter-0.2/snippetconverter/snippetconverter.py` & `kate-vscode-snippetconverter-0.3/snippetconverter/snippetconverter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/python3
 """Convert snippet from Kate/KDevelop to VSCode and vice versa """
 import sys
-import getopt
+import argparse
 import re
 import xml.etree.ElementTree as ET
 import json
 import os.path
 from enum import Enum
 from typing import TypedDict
+from pathlib import Path
 from snippetconverter.languages import (
     get_language_identifier_for_vscode,
     induce_language_from_file_name,
 )
 
 
 class IDE(Enum):
@@ -29,15 +30,14 @@
     )
 
 
 def induce_ide_from_file(filename):
     """Induce which IDE was used to create the file based on its name"""
     if "ktexteditor" in filename or "kdevelop" in filename:
         return IDE.KATE
-    # TODO implement some better ways .(document what other IDE have for name, to ensure we won't have double match if using only *.json) pylint: disable=W0511
     if "Code/User" in filename:
         return IDE.VSCODE
     return IDE.UNKNOWN
 
 
 class Variable(TypedDict):
     """@brief This describe a variable in a snipppet.
@@ -64,26 +64,21 @@
 
     def to_vs_code(self, language):
         """
         @brief print the snippet into Visual Studio Code format
         @param language the language (c++, python, javascript, brainfuck... )relevant for this snippet
         """
         contentlist = self.content.split("\n")
-        # Now modify the content regarding variables to ensure are correcty formatted !
         # See https://code.visualstudio.com/docs/editor/userdefinedsnippets
         for content in enumerate(contentlist):
             for variable in self.variables:
-                # print(variable)
                 if variable["original_text"] in content[1]:
                     content[1].replace(
                         variable["original_text"], str("{" + variable["name"] + "}")
                     )
-                    # print("REPLACED !!!")
-                    # print(content[1])
-                    # print(contentlist)
 
         return dict(
             {
                 "scope": get_language_identifier_for_vscode(language),
                 "prefix": self.name,
                 "body": contentlist,
                 "description": "",
@@ -103,90 +98,67 @@
             name = re.sub(r" ", "_", name)
             if not name in [var["name"] for var in variables]:
                 variable = Variable({"name": name, "original_text": original_text})
                 variables.append(variable)
     return variables
 
 
-def convert_from_kate_to_vscode(katensippet, vscodesnippet):
+def convert_from_kate_to_vscode(katensippet:Path, vscodesnippet:Path):
     """
     @brief Convert a snippet from a Kate/KDevelop snippet format to a visual studio code
     @param katensippet. URL of the Kate snippet file
     @param vscodesnippet. URL of the Visual Studio Code snippet file
     """
     snippets = list()
 
     # First we parse the Kate xml snippet to get a list of snippet that written in the file
-    tree = ET.parse(katensippet)
+    tree = ET.parse(katensippet.absolute())
     root = tree.getroot()
     for items in root.findall("item"):
         match = items.find("match")
         fillin = items.find("fillin")
         variables = get_variable_lists_from_kate_snippet(fillin.text.split("\n"))
         snippets.append(Snippet(match.text, fillin.text, variables))
     # Second we induce which language it is
-    language = induce_language_from_file_name(katensippet)
+    language = induce_language_from_file_name(str(katensippet.absolute()))
 
     outputsnippets = dict()
     for snippet in snippets:
         outputsnippets[snippet.name] = snippet.to_vs_code(language)
 
-    vscode_snippetfile = open(vscodesnippet, "w")
+    vscode_snippetfile = open(vscodesnippet.absolute(), "w")
     vscode_snippetfile.write(json.dumps(outputsnippets, indent=4, sort_keys=True))
 
 
 def convert_vscode_to_kate(vscodesnippet, katesnippet):
     # pylint: disable=W0613
     """@brief Convert a Visual Studio Code snippet to a Kate Snippet
     @param vscodesnippet URL to the visual studio snippet file
     @param katesnippet URL to the Kate/KDevelop snippet file"""
-    print("Conversion from Visual Studio to Kate is not yet implemented")
-    sys.exit(2)
+    raise NotImplementedError("Conversion from Visual Studio to Kate is not yet implemented")
 
 
-def main():
+def main(argv):
     """module main"""
-    inputfile = ""
-    outputfile = ""
-    try:
-        opts, args = getopt.getopt(
-            sys.argv[1:], "hi:o:", ["errorcode", "input", "ouput"]
-        )
-
-    except getopt.GetoptError:
-        usage()
-        sys.exit(1)
-
-    for opt, arg in opts:
-        if opt == "-h":
-            usage()
-            sys.exit()
-
-        elif opt in ("-i", "--input"):
-            inputfile = arg
-
-        elif opt in ("-o", "--ouput"):
-            outputfile = arg
-    # Write the code below, bare in minde functions must be forwarde declared
-
-    if len(inputfile) == 0 or len(outputfile) == 0:
-        usage()
-        sys.exit(1)
+    ap = argparse.ArgumentParser(description='Kate to VSCode snippet converter')
+    ap.add_argument("-i","--input",help="input snippet file",required=True)
+    ap.add_argument("-o","--output",help="output snippet file",required=True)
+    args = ap.parse_args(argv[1:])
 
-    if not os.path.isfile(inputfile):
-        raise FileNotFoundError(str("File: {} does not exist".format(inputfile)))
+    if not os.path.isfile(args.input):
+        raise FileNotFoundError(str("Input file: {} does not exist".format(args.input)))
 
-    ide_in = induce_ide_from_file(inputfile)
-    ide_out = induce_ide_from_file(outputfile)
+    ide_in = induce_ide_from_file(args.input)
+    ide_out = induce_ide_from_file(args.output)
     if ide_in == IDE.UNKNOWN:
-        raise Exception(
-            str("Could not find which IDE the file {} comes from.".format(inputfile))
+        raise RuntimeError(
+            str("Could not find which IDE the input file {} comes from.".format(args.input))
         )
     if ide_out == IDE.UNKNOWN:
-        raise Exception(
-            str("Could not find which IDE the file {} comes from.".format(outputfile))
+        raise RuntimeError(
+            str("Could not find which IDE the output file {} comes from.".format(args.output))
         )
 
     if ide_in == IDE.KATE and ide_out == IDE.VSCODE:
-        convert_from_kate_to_vscode(inputfile, outputfile)
+        convert_from_kate_to_vscode(args.input, args.output)
     if ide_in == IDE.VSCODE and ide_out == IDE.KATE:
-        convert_vscode_to_kate(inputfile, outputfile)
+        convert_vscode_to_kate(args.input, args.output)
```

