# Comparing `tmp/mereja-0.0.7.tar.gz` & `tmp/mereja-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mereja-0.0.7.tar", last modified: Sat Aug  5 07:09:18 2023, max compression
+gzip compressed data, was "mereja-0.0.8.tar", last modified: Sun Aug  6 16:51:07 2023, max compression
```

## Comparing `mereja-0.0.7.tar` & `mereja-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-05 07:09:18.265019 mereja-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-05 07:09:09.000000 mereja-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.261019 mereja-0.0.7/mereja/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/telebirr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/forex_table_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/job_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/marketpalce_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/news_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/transaction_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.261019 mereja-0.0.7/mereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-05 07:09:18.265019 mereja-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-05 07:09:09.000000 mereja-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.820364 mereja-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-08-06 16:51:07.820364 mereja-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-08-06 16:50:55.000000 mereja-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.816363 mereja-0.0.8/mereja/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.820364 mereja-0.0.8/mereja/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/functions/telebirr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.820364 mereja-0.0.8/mereja/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/forex_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/job_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/marketpalce_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/news_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/transaction_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.820364 mereja-0.0.8/mereja/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/ui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-08-06 16:50:55.000000 mereja-0.0.8/mereja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:51:07.816363 mereja-0.0.8/mereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 16:51:07.000000 mereja-0.0.8/mereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-06 16:51:07.820364 mereja-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-06 16:50:55.000000 mereja-0.0.8/setup.py
```

### Comparing `mereja-0.0.7/PKG-INFO` & `mereja-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
@@ -31,15 +31,15 @@
 
 ## Installation
 
 1. Clone this repository:
 
 ```bash
 # for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
+pip install git+https://github.com/wizkiye/mereja.git
 # or 
 pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
@@ -195,10 +195,19 @@
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
 
+# Dependencies
+* rich
+* textual
+* questionary
+* pyEthioJobs
+* pyEthioNews
+* jiji
+* telebirrTxChecker 
+
```

### Comparing `mereja-0.0.7/README.md` & `mereja-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
@@ -18,15 +18,15 @@
 
 ## Installation
 
 1. Clone this repository:
 
 ```bash
 # for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
+pip install git+https://github.com/wizkiye/mereja.git
 # or 
 pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
@@ -182,10 +182,19 @@
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
 
+# Dependencies
+* rich
+* textual
+* questionary
+* pyEthioJobs
+* pyEthioNews
+* jiji
+* telebirrTxChecker 
+
```

### Comparing `mereja-0.0.7/mereja/constants.py` & `mereja-0.0.8/mereja/constants.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/functions/forex.py` & `mereja-0.0.8/mereja/functions/forex.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/functions/jobs.py` & `mereja-0.0.8/mereja/functions/jobs.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/functions/market.py` & `mereja-0.0.8/mereja/functions/market.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/functions/news.py` & `mereja-0.0.8/mereja/functions/news.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/functions/telebirr.py` & `mereja-0.0.8/mereja/functions/telebirr.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/main.py` & `mereja-0.0.8/mereja/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import asyncio
 import sys
 
 import questionary
 
 from mereja import constants
-from mereja.functions import forex, telebirr, market, news, jobs
+from mereja.functions import news, forex, market, telebirr, jobs
 from mereja.utils import awaitable
 
 
 @awaitable
 def show_menu():
     ans = questionary.prompt(
         constants.QUESTIONS,
@@ -45,15 +45,15 @@
             return
 
     elif answers.get("answer") == "💼 Jobs":
         if answers.get("choice") == "Get latest jobs":
             await jobs.get_latest_jobs()
 
         elif answers.get("choice") == "🔍 Search for jobs":
-            await jobs.search_for_job()
+            await jobs.search_for_job(query=answers.get("search"))
 
         elif answers.get("choice") == "🔙 Back":
             return
     elif answers.get("answer") == "🛍 Marketplace":
         if answers.get("choice") == "📈 Get trending products":
             await market.get_trending_products()
 
@@ -216,13 +216,12 @@
     parser.add_argument("--page", "-p", type=int, default=0, help="Page number")
     parser.add_argument("--limit", "-l", type=int, default=10, help="Limit number")
     parser.add_argument("--search", "-s", help="Search for a job/product/news")
     parser.add_argument("--export", "-e", action="store_true", help="Export to file")
     parser.add_argument("--path", "-pa", help="Path to export file")
 
     args = parser.parse_args()
-
     runner(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mereja-0.0.7/mereja/ui/forex_table_ui.py` & `mereja-0.0.8/mereja/ui/forex_table_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/ui/job_view_ui.py` & `mereja-0.0.8/mereja/ui/job_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/ui/marketpalce_ui.py` & `mereja-0.0.8/mereja/ui/marketpalce_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/ui/news_view_ui.py` & `mereja-0.0.8/mereja/ui/news_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/ui/transaction_table.py` & `mereja-0.0.8/mereja/ui/transaction_table.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/ui/widgets/header.py` & `mereja-0.0.8/mereja/ui/widgets/header.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja/utils.py` & `mereja-0.0.8/mereja/utils.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/mereja.egg-info/PKG-INFO` & `mereja-0.0.8/mereja.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
@@ -31,15 +31,15 @@
 
 ## Installation
 
 1. Clone this repository:
 
 ```bash
 # for latest version
-pip install git+https://github.com/your-username/your-repo-name.git
+pip install git+https://github.com/wizkiye/mereja.git
 # or 
 pip install mereja -U
 ```
 
 ## Usage
 
 ```bash
@@ -195,10 +195,19 @@
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
 
+# Dependencies
+* rich
+* textual
+* questionary
+* pyEthioJobs
+* pyEthioNews
+* jiji
+* telebirrTxChecker 
+
```

### Comparing `mereja-0.0.7/mereja.egg-info/SOURCES.txt` & `mereja-0.0.8/mereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mereja-0.0.7/setup.py` & `mereja-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str):
     with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="mereja",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     url="https://github.com/wizkiye/mereja",
     license="MIT",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     description="",
     install_requires=[
@@ -21,14 +21,15 @@
         "markdownify",
         "qrcode",
         "questionary",
         "pyEthioJobs",
         "pyEthioNews",
         "jiji",
         "telebirrTxChecker",
+        "linkify-it-py",
     ],
     entry_points={
         "console_scripts": [
             "mereja = mereja.main:main",
         ],
     },
     long_description=read_file("README.md"),
```

