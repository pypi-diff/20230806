# Comparing `tmp/md2cf-2.2.1.tar.gz` & `tmp/md2cf-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/md2cf-2.2.1.tar", last modified: Mon Jul 17 15:36:05 2023, max compression
+gzip compressed data, was "dist/md2cf-2.3.0.tar", last modified: Sun Aug  6 19:01:52 2023, max compression
```

## Comparing `md2cf-2.2.1.tar` & `md2cf-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 15:36:05.000000 md2cf-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-17 15:35:59.000000 md2cf-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/confluence_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/ignored_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-17 15:35:59.000000 md2cf-2.2.1/md2cf/upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:36:05.000000 md2cf-2.2.1/md2cf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:36:05.000000 md2cf-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-17 15:35:59.000000 md2cf-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:01:52.000000 md2cf-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-08-06 19:01:52.000000 md2cf-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-08-06 19:01:50.000000 md2cf-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27336 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/confluence_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/ignored_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-08-06 19:01:50.000000 md2cf-2.3.0/md2cf/upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 19:01:52.000000 md2cf-2.3.0/md2cf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:01:52.000000 md2cf-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-06 19:01:50.000000 md2cf-2.3.0/setup.py
```

### Comparing `md2cf-2.2.1/PKG-INFO` & `md2cf-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.2.1
+Version: 2.3.0
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
```

### Comparing `md2cf-2.2.1/README.md` & `md2cf-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf/__main__.py` & `md2cf-2.3.0/md2cf/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,22 @@
     )
     parser.add_argument(
         "file_list",
         type=Path,
         help="markdown files or directories to upload to Confluence. Empty for stdin",
         nargs="*",
     )
+    parser.add_argument(
+        "--max-retries",
+        action="store",
+        dest="max_retries",
+        type=int,
+        default=4,
+        help="number of retry attempts if any API call fails",
+    )
 
     return parser
 
 
 def print_missing_parameter(parameter_name: str):
     error_console.log(
         ":x: Missing required parameter: {}\n"
@@ -293,14 +301,15 @@
 
     confluence = api.MinimalConfluence(
         host=args.host,
         username=args.username,
         password=args.password,
         token=args.token,
         verify=not args.insecure,
+        max_retries=args.max_retries,
     )
 
     if (args.title or args.page_id) and (
         len(args.file_list) > 1 or any(map(os.path.isdir, args.file_list))
     ):
         error_console.log(
             ":x: Title and page ID cannot be specified on the command line "
@@ -376,14 +385,15 @@
             validate_relative_links(
                 pages_to_upload, map_document_path_to_confluence_page
             )
 
     something_went_wrong = False
     error = None
     tui = Md2cfTUI(pages_to_upload)
+
     with tui:
         space_info = confluence.get_space(
             args.space, additional_expansions=["homepage"]
         )
 
         for page in pages_to_upload:
             pre_process_page(page, args, postface_markup, preface_markup, space_info)
```

### Comparing `md2cf-2.2.1/md2cf/api.py` & `md2cf-2.3.0/md2cf/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         for key, value in kwargs.items():
             kwargs[key] = bunchify(value)
         super(Bunch, self).__init__(kwargs)
         self.__dict__ = self
 
 
 class MinimalConfluence:
-    def __init__(self, host, username=None, password=None, token=None, verify=True):
+    def __init__(
+        self, host, username=None, password=None, token=None, verify=True, max_retries=4
+    ):
         if token is None:
             if username is None and password is None:
                 raise ValueError(
                     "Either a personal access token, "
                     "or username and password are required"
                 )
 
@@ -43,18 +45,18 @@
         if token is not None:
             self.api.headers.update({"Authorization": f"Bearer {token}"})
         elif username is not None and password is not None:
             self.api.auth = (username, password)
 
         adapter = requests.adapters.HTTPAdapter(
             max_retries=urllib3.Retry(
-                total=4,
+                total=max_retries,
                 backoff_factor=1,
                 respect_retry_after_header=True,
-                status_forcelist=[429],
+                allowed_methods=None,
             )
         )
         self.api.mount("http://", adapter)
         self.api.mount("https://", adapter)
 
         if not verify:
             requests.packages.urllib3.disable_warnings(
```

### Comparing `md2cf-2.2.1/md2cf/confluence_renderer.py` & `md2cf-2.3.0/md2cf/confluence_renderer.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf/document.py` & `md2cf-2.3.0/md2cf/document.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf/ignored_files.py` & `md2cf-2.3.0/md2cf/ignored_files.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf/tui.py` & `md2cf-2.3.0/md2cf/tui.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf/upsert.py` & `md2cf-2.3.0/md2cf/upsert.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.2.1/md2cf.egg-info/PKG-INFO` & `md2cf-2.3.0/md2cf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.2.1
+Version: 2.3.0
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
```

### Comparing `md2cf-2.2.1/setup.py` & `md2cf-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="md2cf",
-    version="2.2.1",
+    version="2.3.0",
     packages=["md2cf"],
     url="https://github.com/iamjackg/md2cf",
     license="MIT",
     author="Jack Gaino",
     author_email="md2cf@jackgaino.com",
     description="Convert Markdown documents to Confluence",
     long_description=long_description,
@@ -22,13 +22,13 @@
     keywords="markdown confluence",
     install_requires=[
         "rich-argparse==1.0.0",
         "rich==13.0.1",
         "mistune==0.8.4",
         "chardet==5.1.0",
         "requests==2.31.0",
-        "PyYAML==6.0",
+        "PyYAML==6.0.1",
         "gitignorefile==1.1.2",
     ],
     python_requires=">=3.7",
     entry_points={"console_scripts": ["md2cf=md2cf.__main__:main"]},
 )
```

