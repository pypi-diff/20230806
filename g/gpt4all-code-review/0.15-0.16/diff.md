# Comparing `tmp/gpt4all-code-review-0.15.tar.gz` & `tmp/gpt4all-code-review-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.15.tar", last modified: Sat Aug  5 16:19:03 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.16.tar", last modified: Sat Aug  5 20:52:28 2023, max compression
```

## Comparing `gpt4all-code-review-0.15.tar` & `gpt4all-code-review-0.16.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.302572 gpt4all-code-review-0.15/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2734 2023-08-05 16:19:03.302427 gpt4all-code-review-0.15/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2458 2023-08-05 16:00:14.000000 gpt4all-code-review-0.15/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.301264 gpt4all-code-review-0.15/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.15/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6235 2023-08-05 16:06:49.000000 gpt4all-code-review-0.15/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 16:19:03.302234 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2734 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 16:19:03.000000 gpt4all-code-review-0.15/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 16:19:03.302609 gpt4all-code-review-0.15/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      720 2023-08-05 16:12:30.000000 gpt4all-code-review-0.15/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.944386 gpt4all-code-review-0.16/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2744 2023-08-05 20:52:28.944252 gpt4all-code-review-0.16/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2458 2023-08-05 16:00:14.000000 gpt4all-code-review-0.16/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.943353 gpt4all-code-review-0.16/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.16/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     5977 2023-08-05 20:46:16.000000 gpt4all-code-review-0.16/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 20:52:28.944078 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     2744 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-05 20:52:28.000000 gpt4all-code-review-0.16/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-05 20:52:28.944420 gpt4all-code-review-0.16/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-05 20:47:50.000000 gpt4all-code-review-0.16/setup.py
```

### Comparing `gpt4all-code-review-0.15/PKG-INFO` & `gpt4all-code-review-0.16/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.15
-Summary: A standalone code review tool based on GPT4ALL.
+Version: 0.16
+Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 # Code Review Automation Tool
```

### Comparing `gpt4all-code-review-0.15/README.md` & `gpt4all-code-review-0.16/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-code-review-0.15/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.16/gpt4all_code_review/gpt4all_code_review.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,170 +2,144 @@
 import json
 import argparse
 from gpt4all import GPT4All
 from prettytable import PrettyTable
 from datetime import datetime
 from console_progressbar import ProgressBar
 
+DEFAULT_MODEL_NAME = "orca-mini-3b.ggmlv3.q4_0.bin"
+SYSTEM_TEMPLATE = 'Imagine that you are a developer, and you are reviewing the code of a junior. You should give short suggestions for improving the code.'
 
-def main():
-    parser = argparse.ArgumentParser(description="check.py")
-    parser.add_argument(
-        "--model",
-        help="Model name",
-        default="orca-mini-3b.ggmlv3.q4_0.bin"
-    )
-    parser.add_argument(
-        "--file",
-        help="File path to analyze"
-    )
-    parser.add_argument(
-        "--all",
-        help="Include all files and folders",
-        action='store_true'
-    )
-    parser.add_argument(
-        "--output",
-        help="Output type",
-        default="text"
-    )
-    parser.add_argument(
-        "--export",
-        help="Export to file"
-    )
-    parser.add_argument(
-        "--export-folder",
-        help="Export to folder"
-    )
-
-    args = parser.parse_args()
-    model_name = args.model
-    scan_all = args.all
-    output_type = args.output
-    export = args.export
-    export_folder = args.export_folder
-    if export_folder is None and export is not None:
-        export_folder = "code_review_results"
-    else:
-        export_folder = None
-    model = GPT4All(model_name)
 
+class CodeAnalyzer:
+    def __init__(self, model_name, scan_all, output_type, export, export_folder):
+        self.model_name = model_name
+        self.scan_all = scan_all
+        self.output_type = output_type
+        self.export = export
+        self.export_folder = export_folder or "code_review_results" if export else None
+        self.model = GPT4All(model_name)
 
-    all_files = gather_files(args.file, scan_all)
-    print("Number of scanning files:", len(all_files))
+    def gather_files(self, scan_file):
+        all_files = []
 
-    results = process_files(all_files, model)
-    export_results(results, export_folder, output_type)
+        if self.scan_all:
+            for path, _, files in os.walk(os.getcwd()):
+                all_files.extend(
+                    os.path.join(path, name) for name in files
+                )
 
+        if scan_file:
+            all_files.append(os.path.join(os.getcwd(), scan_file))
 
-def export_as_text(results, export_folder):
-    t = PrettyTable(['File path', 'Suggestions'])
-    for result in results:
-        t.add_row(result)
-    t.align = "l"
-    t._max_width = {"File path": 50, "Suggestions": 100}
-    print(t)
-    if export_folder:
-        filename = f"review-{datetime.now().strftime('%Y%m%d-%H%M%S')}.txt"
-        with open(os.path.join(export_folder, filename), "w") as f:
-            f.write(t.get_string())
-
-def export_as_json(results, export_folder):
-    print(json.dumps(results))
-    if export_folder:
-        filename = f"review-{datetime.now().strftime('%Y%m%d-%H%M%S')}.json"
-        with open(os.path.join(export_folder, filename), "w") as f:
-            json.dump(results, f)
-
-def export_as_xml(results, export_folder):
-    xml_content = "<results>" + "".join(f"<result><file_path>{result[0]}</file_path><suggestions>{result[1]}</suggestions></result>" for result in results) + "</results>"
-    print(xml_content)
-    if export_folder:
-        filename = f"review-{datetime.now().strftime('%Y%m%d-%H%M%S')}.xml"
-        with open(os.path.join(export_folder, filename), "w") as f:
-            f.write(xml_content)
-
-def export_results(results, export_folder, output_type):
-    if export_folder and not os.path.exists(export_folder):
-        os.makedirs(export_folder)
-
-    if output_type == "text":
-        export_as_text(results, export_folder)
-    elif output_type == "json":
-        export_as_json(results, export_folder)
-    elif output_type == "xml":
-        export_as_xml(results, export_folder)
-    else:
-        print("Unknown output type")
-
-def process_files(all_files, model):
-    results = []
-    system_template = 'Imagine that you are a developer, and you are reviewing the code of a junior. You should give short suggestions for improving the code.'
-
-
-    total_files = len(all_files)
-    current_file = 0
-    pb_files = ProgressBar(total=100, prefix='Files', suffix='', decimals=3, length=100, fill='X',
-                     zfill='-')
+        return all_files
 
-    for file_path in all_files:
-        try:
-            current_file += 1
-            print("Processing file: " + file_path + " (" + str(current_file) +"/"+ str(total_files) + ")")
-            if current_file == 1:
-                current_progress_files = 0
-            pb_files.print_progress_bar(current_progress_files)
+    def process_files(self, all_files):
+        results = []
+        total_files = len(all_files)
+        pb_files = ProgressBar(total=100, prefix='Files', suffix='', decimals=3, length=100, fill='X', zfill='-')
 
+        for idx, file_path in enumerate(all_files, 1):
+            print(f"Processing file: {file_path} ({idx}/{total_files})")
+            results.append(self.process_file(file_path, idx, total_files, pb_files))
+
+        return results
+
+    def process_file(self, file_path, file_index, total_files, pb_files):
+        try:
             with open(file_path, "r", encoding='utf-8', errors='replace') as f:
                 file_content = f.read()
-                file_name = os.path.basename(file_path)
-                content_chunks = [file_content[i:i+1900] for i in range(0, len(file_content), 1900)]
-                print(" number of chunks:", len(content_chunks))
-                suggestions = []
-                chunk_number = 0
-                total_chunks = len(content_chunks)
-                pb_chunks = ProgressBar(total=100, prefix='Chunks', suffix='', decimals=3,
-                                       length=100, fill='X',
-                                       zfill='-')
-                for chunk in content_chunks:
-                    chunk_number += 1
-                    if chunk_number == 1:
-                        current_progress_chunks = 0
-
-                    pb_chunks.print_progress_bar(current_progress_chunks)
-                    print("     chunk number:", chunk_number)
-                    prompt = f"The file '{file_name}' (chunk '{str(chunk_number)}') contains: {chunk}. Could you give some recommendations for improving the code? and sorting suggestions list by priority from hight to low"
-
-                    with model.chat_session(system_template):
-                        response = model.generate(prompt=prompt, temp=0, max_tokens=1000)
-                        current_progress_chunks = chunk_number / total_chunks * 100
-                        suggestion = response.lstrip().replace("Sure", "").replace("Sure, ", "").replace("!", "")
-                        suggestions.append(suggestion)
-                pb_chunks.print_progress_bar(100)
-                combined_suggestion = ""
-                for i in range(len(suggestions)):
-                    combined_suggestion += str(i+1) + ". " + suggestions[i] + "\n"
-                current_progress_files = current_file / total_files * 100
-                pb_files.print_progress_bar(current_progress_files)
-                results.append([file_path.replace(os.getcwd(), ""), combined_suggestion])
+            file_name = os.path.basename(file_path)
+            content_chunks = self.get_chunks(file_content)
+            suggestions = self.get_suggestions(file_name, content_chunks)
 
+            pb_files.print_progress_bar((file_index / total_files) * 100)
+            return [file_path.replace(os.getcwd(), ""), "\n".join(suggestions)]
         except Exception as e:
             print(e)
 
-    return results
+    @staticmethod
+    def get_chunks(file_content, chunk_size=1900):
+        return [file_content[i:i + chunk_size] for i in range(0, len(file_content), chunk_size)]
+
+    def get_suggestions(self, file_name, content_chunks):
+        total_chunks = len(content_chunks)
+        pb_chunks = ProgressBar(total=100, prefix='Chunks', suffix='', decimals=3, length=100, fill='X', zfill='-')
+        suggestions = []
+
+        for idx, chunk in enumerate(content_chunks, 1):
+            pb_chunks.print_progress_bar((idx / total_chunks) * 100)
+            prompt = f"The file '{file_name}' (chunk '{str(idx)}') contains: {chunk}. Could you give some recommendations for improving the code? and sorting suggestions list by priority from hight to low"
+
+            with self.model.chat_session(SYSTEM_TEMPLATE):
+                response = self.model.generate(prompt=prompt, temp=0, max_tokens=1000)
+                suggestion = response.lstrip().replace("Sure", "").replace("Sure, ", "").replace("!", "")
+                suggestions.append(suggestion)
+
+        return suggestions
+
+    def export_results(self, results):
+        if self.export_folder and not os.path.exists(self.export_folder):
+            os.makedirs(self.export_folder)
+
+        exporters = {
+            'text': self.export_as_text,
+            'json': self.export_as_json,
+            'xml': self.export_as_xml,
+        }
+        export_func = exporters.get(self.output_type, lambda *args: print("Unknown output type"))
+        export_func(results)
+
+    def export_as_text(self, results):
+        t = PrettyTable(['File path', 'Suggestions'])
+        for result in results:
+            t.add_row(result)
+        t.align = "l"
+        t._max_width = {"File path": 50, "Suggestions": 100}
+        print(t)
+        if self.export_folder:
+            self.write_to_file(t.get_string(), ".txt")
+
+    def export_as_json(self, results):
+        print(json.dumps(results))
+        if self.export_folder:
+            self.write_to_file(json.dumps(results), ".json")
+
+    def export_as_xml(self, results):
+        xml_content = "<results>" + "".join(
+            f"<result><file_path>{result[0]}</file_path><suggestions>{result[1]}</suggestions></result>" for result in
+            results) + "</results>"
+        print(xml_content)
+        if self.export_folder:
+            self.write_to_file(xml_content, ".xml")
+
+    def write_to_file(self, content, extension):
+        filename = f"review-{datetime.now().strftime('%Y%m%d-%H%M%S')}{extension}"
+        with open(os.path.join(self.export_folder, filename), "w") as f:
+            f.write(content)
 
-def gather_files(scan_file, scan_all):
-    all_files = []
 
-    if scan_all:
-        for path, _, files in os.walk(os.getcwd()):
-            all_files.extend(
-                os.path.join(path, name) for name in files
-            )
+def parse_arguments():
+    parser = argparse.ArgumentParser(description="check.py")
+    parser.add_argument("--model", help="Specifies the model name. Default is orca-mini-3b.ggmlv3.q4_0.bin", default=DEFAULT_MODEL_NAME)
+    parser.add_argument("--file", help="Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed")
+    parser.add_argument("--all", help="Includes all files and folders in the current directory for scanning", action='store_true')
+    parser.add_argument("--output", help="Output type (default: txt). Options: txt, json, xml", default="text")
+    parser.add_argument("--export", help="Export to file (default: False)")
+    parser.add_argument("--export-folder", help="Export to folder (default: ./code_review_results)")
+
+    return parser.parse_args()
+
+
+def main():
+    args = parse_arguments()
+    analyzer = CodeAnalyzer(args.model, args.all, args.output, args.export, args.export_folder)
+
+    all_files = analyzer.gather_files(args.file)
+    print("Number of scanning files:", len(all_files))
 
-    if scan_file:
-        all_files.append(os.path.join(os.getcwd(), scan_file))
+    results = analyzer.process_files(all_files)
+    analyzer.export_results(results)
 
-    return all_files
 
 if __name__ == "__main__":
     main()
```

### Comparing `gpt4all-code-review-0.15/gpt4all_code_review.egg-info/PKG-INFO` & `gpt4all-code-review-0.16/gpt4all_code_review.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.15
-Summary: A standalone code review tool based on GPT4ALL.
+Version: 0.16
+Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 # Code Review Automation Tool
```

### Comparing `gpt4all-code-review-0.15/setup.py` & `gpt4all-code-review-0.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.15',
+    version='0.16',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
     ],
     author='Evgenii Evstafev',
     author_email='chigwel@gmail.com',
-    description='A standalone code review tool based on GPT4ALL.',
+    description='A self-contained tool for code review powered by GPT4ALL.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/gpt4all-code-review',
     entry_points={
         'console_scripts': [
             'gpt4all_code_review = gpt4all_code_review.gpt4all_code_review:main',
         ],
```

