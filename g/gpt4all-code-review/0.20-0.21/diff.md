# Comparing `tmp/gpt4all-code-review-0.20.tar.gz` & `tmp/gpt4all-code-review-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-code-review-0.20.tar", last modified: Sun Aug  6 11:30:30 2023, max compression
+gzip compressed data, was "gpt4all-code-review-0.21.tar", last modified: Sun Aug  6 11:32:37 2023, max compression
```

## Comparing `gpt4all-code-review-0.20.tar` & `gpt4all-code-review-0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:30:30.982761 gpt4all-code-review-0.20/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3401 2023-08-06 11:30:30.982619 gpt4all-code-review-0.20/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3115 2023-08-06 11:23:56.000000 gpt4all-code-review-0.20/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:30:30.981363 gpt4all-code-review-0.20/gpt4all_code_review/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.20/gpt4all_code_review/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6304 2023-08-06 11:30:05.000000 gpt4all-code-review-0.20/gpt4all_code_review/gpt4all_code_review.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:30:30.982410 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3401 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-06 11:30:30.000000 gpt4all-code-review-0.20/gpt4all_code_review.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-06 11:30:30.982801 gpt4all-code-review-0.20/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-06 11:30:27.000000 gpt4all-code-review-0.20/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:32:37.634757 gpt4all-code-review-0.21/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3401 2023-08-06 11:32:37.634632 gpt4all-code-review-0.21/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3115 2023-08-06 11:23:56.000000 gpt4all-code-review-0.21/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:32:37.633690 gpt4all-code-review-0.21/gpt4all_code_review/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2023-08-05 15:31:18.000000 gpt4all-code-review-0.21/gpt4all_code_review/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     6315 2023-08-06 11:32:18.000000 gpt4all-code-review-0.21/gpt4all_code_review/gpt4all_code_review.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2023-08-06 11:32:37.634470 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     3401 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      353 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       85 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       58 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       20 2023-08-06 11:32:37.000000 gpt4all-code-review-0.21/gpt4all_code_review.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2023-08-06 11:32:37.634791 gpt4all-code-review-0.21/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      730 2023-08-06 11:32:30.000000 gpt4all-code-review-0.21/setup.py
```

### Comparing `gpt4all-code-review-0.20/PKG-INFO` & `gpt4all-code-review-0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.20
+Version: 0.21
 Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
```

### Comparing `gpt4all-code-review-0.20/README.md` & `gpt4all-code-review-0.21/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-code-review-0.20/gpt4all_code_review/gpt4all_code_review.py` & `gpt4all-code-review-0.21/gpt4all_code_review/gpt4all_code_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     def write_to_file(self, content, extension):
         filename = f"review-{datetime.now().strftime('%Y%m%d-%H%M%S')}{extension}"
         with open(os.path.join(self.export_folder, filename), "w") as f:
             f.write(content)
 
 
 def parse_arguments():
-    parser = argparse.ArgumentParser(description="check.py")
+    parser = argparse.ArgumentParser(description="gpt4all_code_review")
     parser.add_argument("--model", help="Specifies the model name. Default is orca-mini-3b.ggmlv3.q4_0.bin", default=DEFAULT_MODEL_NAME)
     parser.add_argument("--file", help="Specifies the file path to analyze. If not provided, all files in the current directory will be analyzed")
     parser.add_argument("--all", help="Includes all files and folders in the current directory for scanning", action='store_true')
     parser.add_argument("--output", help="Output type (default: plain). Options: plain, txt (prettytable), json, xml", default="plain")
     parser.add_argument("--export", help="Export to file (default: False)")
     parser.add_argument("--export-folder", help="Export to folder (default: ./code_review_results)")
```

### Comparing `gpt4all-code-review-0.20/gpt4all_code_review.egg-info/PKG-INFO` & `gpt4all-code-review-0.21/gpt4all_code_review.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all-code-review
-Version: 0.20
+Version: 0.21
 Summary: A self-contained tool for code review powered by GPT4ALL.
 Home-page: https://github.com/chigwell/gpt4all-code-review
 Author: Evgenii Evstafev
 Author-email: chigwel@gmail.com
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/gpt4all-code-review.svg)](https://badge.fury.io/py/gpt4all-code-review)  [![Downloads](https://static.pepy.tech/personalized-badge/gpt4all-code-review?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/gpt4all-code-review) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
```

### Comparing `gpt4all-code-review-0.20/setup.py` & `gpt4all-code-review-0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gpt4all-code-review',
-    version='0.20',
+    version='0.21',
     packages=find_packages(),
     install_requires=[
         "argparse",
         "gpt4all",
         "prettytable",
         "datetime",
         "console_progressbar",
```

