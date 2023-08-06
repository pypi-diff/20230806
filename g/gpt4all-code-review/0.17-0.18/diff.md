# Comparing `tmp/gpt4all-code-review-0.17.tar.gz` & `tmp/gpt4all-code-review-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.17.tar", last modified: Sun Aug  6 10:52:43 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.18.tar", last modified: Sun Aug  6 11:18:19 2023, max compression
```

## Comparing `gpt4all-code-review-0.17.tar` & `gpt4all-code-review-0.18.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.087830 gpt4all-code-review-0.17/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3323 2023-08-06 10:52:43.087537 gpt4all-code-review-0.17/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3037 2023-08-06 10:52:31.000000 gpt4all-code-review-0.17/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.086069 gpt4all-code-review-0.17/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.17/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     5977 2023-08-05 20:46:16.000000 gpt4all-code-review-0.17/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 10:52:43.087119 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3323 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-06 10:52:43.000000 gpt4all-code-review-0.17/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-06 10:52:43.087878 gpt4all-code-review-0.17/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-06 10:52:31.000000 gpt4all-code-review-0.17/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:18:19.755307 gpt4all-code-review-0.18/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3407 2023-08-06 11:18:19.755160 gpt4all-code-review-0.18/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3121 2023-08-06 11:09:04.000000 gpt4all-code-review-0.18/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:18:19.754201 gpt4all-code-review-0.18/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.18/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6316 2023-08-06 11:14:51.000000 gpt4all-code-review-0.18/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:18:19.754981 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3407 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-06 11:18:19.000000 gpt4all-code-review-0.18/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-06 11:18:19.755344 gpt4all-code-review-0.18/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-06 11:09:04.000000 gpt4all-code-review-0.18/setup.py
```

### Comparing `gpt4all-code-review-0.17/PKG-INFO` & `gpt4all-code-review-0.18/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.17
+Version: 0.18
 Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
@@ -42,15 +42,15 @@
 
 ### Options
 
 - `h`, `--help`: Show this help message and exit
 - `--model`: Specifies the model name. Default is `"orca-mini-3b.ggmlv3.q4_0.bin"`.
 - `--file`: Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed.
 - `--all`: Includes all files and folders in the current directory for scanning.
-- `--output`: Output type (default: `txt`). Options: `txt`, `json`, `xml`.
+- `--output`: Output type (default: `plain`). Options: `plain`, `txt` (prettytable), `json`, `xml`.
 - `--export`: Export to file (default: `False`).
 - `--export-folder`: Export to folder (default: `./code_review_results`).
 ### Example
 
 To analyze a single file:
 
 ```bash
@@ -61,15 +61,16 @@
 
 ```bash
 gpt4all_code_review --all
 ```
 
 ## Output Formats
 
-- **Text:** A human-readable table with file paths and suggestions.
+- **PLAIN:** A human-readable plain txt file.
+- **TXT:** A human-readable table (prettytable) with file paths and suggestions.
 - **JSON:** A machine-readable format that can be parsed programmatically.
 - **XML:** An alternative machine-readable format.
 
 ## Dependencies
 
 -   `os`: Standard Python library for interacting with the operating system.
 -   `json`: Standard Python library for working with JSON data.
```

### Comparing `gpt4all-code-review-0.17/README.md` & `gpt4all-code-review-0.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ### Options
 
 - `h`, `--help`: Show this help message and exit
 - `--model`: Specifies the model name. Default is `"orca-mini-3b.ggmlv3.q4_0.bin"`.
 - `--file`: Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed.
 - `--all`: Includes all files and folders in the current directory for scanning.
-- `--output`: Output type (default: `txt`). Options: `txt`, `json`, `xml`.
+- `--output`: Output type (default: `plain`). Options: `plain`, `txt` (prettytable), `json`, `xml`.
 - `--export`: Export to file (default: `False`).
 - `--export-folder`: Export to folder (default: `./code_review_results`).
 ### Example
 
 To analyze a single file:
 
 ```bash
@@ -52,15 +52,16 @@
 
 ```bash
 gpt4all_code_review --all
 ```
 
 ## Output Formats
 
-- **Text:** A human-readable table with file paths and suggestions.
+- **PLAIN:** A human-readable plain txt file.
+- **TXT:** A human-readable table (prettytable) with file paths and suggestions.
 - **JSON:** A machine-readable format that can be parsed programmatically.
 - **XML:** An alternative machine-readable format.
 
 ## Dependencies
 
 -   `os`: Standard Python library for interacting with the operating system.
 -   `json`: Standard Python library for working with JSON data.
```

### Comparing `gpt4all-code-review-0.17/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.18/gpt4all_code_review/gpt4all_code_review.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,22 +78,28 @@
         return suggestions
 
     def export_results(self, results):
         if self.export_folder and not os.path.exists(self.export_folder):
             os.makedirs(self.export_folder)
 
         exporters = {
-            'text': self.export_as_text,
+            'plain': self.export_as_plain_text,
+            'text': self.export_as_text_table,
             'json': self.export_as_json,
             'xml': self.export_as_xml,
         }
         export_func = exporters.get(self.output_type, lambda *args: print("Unknown output type"))
         export_func(results)
 
-    def export_as_text(self, results):
+    def export_as_plain_text(self, results):
+        print("\n".join(f"{result[0]}: {result[1]}" for result in results))
+        if self.export_folder:
+            self.write_to_file("\n".join(f"{result[0]}: {result[1]}" for result in results), ".txt")
+
+    def export_as_text_table(self, results):
         t = PrettyTable(['File path', 'Suggestions'])
         for result in results:
             t.add_row(result)
         t.align = "l"
         t._max_width = {"File path": 50, "Suggestions": 100}
         print(t)
         if self.export_folder:
@@ -119,15 +125,15 @@
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description="check.py")
     parser.add_argument("--model", help="Specifies the model name. Default is orca-mini-3b.ggmlv3.q4_0.bin", default=DEFAULT_MODEL_NAME)
     parser.add_argument("--file", help="Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed")
     parser.add_argument("--all", help="Includes all files and folders in the current directory for scanning", action='store_true')
-    parser.add_argument("--output", help="Output type (default: txt). Options: txt, json, xml", default="text")
+    parser.add_argument("--output", help="Output type (default: plain). Options: plaint, txt (prettytable), json, xml", default="plain")
     parser.add_argument("--export", help="Export to file (default: False)")
     parser.add_argument("--export-folder", help="Export to folder (default: ./code_review_results)")
 
     return parser.parse_args()
 
 
 def main():
```

### Comparing `gpt4all-code-review-0.17/gpt4all_code_review.egg-info/PKG-INFO` & `gpt4all-code-review-0.18/gpt4all_code_review.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.17
+Version: 0.18
 Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
@@ -42,15 +42,15 @@
 
 ### Options
 
 - `h`, `--help`: Show this help message and exit
 - `--model`: Specifies the model name. Default is `"orca-mini-3b.ggmlv3.q4_0.bin"`.
 - `--file`: Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed.
 - `--all`: Includes all files and folders in the current directory for scanning.
-- `--output`: Output type (default: `txt`). Options: `txt`, `json`, `xml`.
+- `--output`: Output type (default: `plain`). Options: `plain`, `txt` (prettytable), `json`, `xml`.
 - `--export`: Export to file (default: `False`).
 - `--export-folder`: Export to folder (default: `./code_review_results`).
 ### Example
 
 To analyze a single file:
 
 ```bash
@@ -61,15 +61,16 @@
 
 ```bash
 gpt4all_code_review --all
 ```
 
 ## Output Formats
 
-- **Text:** A human-readable table with file paths and suggestions.
+- **PLAIN:** A human-readable plain txt file.
+- **TXT:** A human-readable table (prettytable) with file paths and suggestions.
 - **JSON:** A machine-readable format that can be parsed programmatically.
 - **XML:** An alternative machine-readable format.
 
 ## Dependencies
 
 -   `os`: Standard Python library for interacting with the operating system.
 -   `json`: Standard Python library for working with JSON data.
```

### Comparing `gpt4all-code-review-0.17/setup.py` & `gpt4all-code-review-0.18/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.17',
+    version='0.18',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
```

