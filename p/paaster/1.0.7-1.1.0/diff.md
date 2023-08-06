# Comparing `tmp/paaster-1.0.7.tar.gz` & `tmp/paaster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paaster-1.0.7.tar", max compression
+gzip compressed data, was "paaster-1.1.0.tar", max compression
```

## Comparing `paaster-1.0.7.tar` & `paaster-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-24 00:56:46.675347 paaster-1.0.7/LICENSE
--rw-r--r--   0        0        0      659 2023-07-24 00:56:46.675347 paaster-1.0.7/README.md
--rw-r--r--   0        0        0     2831 2023-07-24 00:56:46.675347 paaster-1.0.7/paaster_cli/__init__.py
--rw-r--r--   0        0        0      332 2023-07-24 00:56:46.675347 paaster-1.0.7/paaster_cli/misc.py
--rw-r--r--   0        0        0     1409 2023-07-24 00:56:46.675347 paaster-1.0.7/paaster_cli/storage.py
--rw-r--r--   0        0        0      522 2023-07-24 00:56:46.675347 paaster-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1319 1970-01-01 00:00:00.000000 paaster-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-06 13:35:01.955941 paaster-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1044 2023-08-06 13:35:01.955941 paaster-1.1.0/README.md
+-rw-r--r--   0        0        0     4176 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/__init__.py
+-rw-r--r--   0        0        0      332 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/misc.py
+-rw-r--r--   0        0        0     1445 2023-08-06 13:35:01.955941 paaster-1.1.0/paaster_cli/storage.py
+-rw-r--r--   0        0        0      522 2023-08-06 13:35:01.955941 paaster-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 paaster-1.1.0/PKG-INFO
```

### Comparing `paaster-1.0.7/LICENSE` & `paaster-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paaster-1.0.7/paaster_cli/storage.py` & `paaster-1.1.0/paaster_cli/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             pass
 
         self.set("API_URL", "https://api.paaster.io/")
         self.set("FRONTEND_URL", "https://paaster.io/")
         self.set("COPY_URL_TO_CLIPBOARD", True)
         self.set("OPEN_URL_IN_BROWSER", False)
         self.set("NAME", "paaster")
+        self.set("ECHO_URL", False)
 
     @property
     def pathway(self) -> str:
         return path.join(self._pathway, "config.json")
 
     def all(self) -> dict:
         try:
```

### Comparing `paaster-1.0.7/pyproject.toml` & `paaster-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paaster"
-version = "1.0.7"
+version = "1.1.0"
 description = "Upload locally encrypted pastes from your terminal to Paaster"
 authors = ["WardPearce <wardpearce@protonmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "paaster_cli"}]
 
 [tool.poetry.dependencies]
```

### Comparing `paaster-1.0.7/PKG-INFO` & `paaster-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paaster
-Version: 1.0.7
+Version: 1.1.0
 Summary: Upload locally encrypted pastes from your terminal to Paaster
 License: GPL-3.0
 Author: WardPearce
 Author-email: wardpearce@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -12,36 +12,35 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pysodium (>=0.7.12,<0.8.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Paaster CLI
-Upload locally encrypted pastes to paaster.io from your desktop.
+# Paaster CLI: Encrypted Pastes from Your Terminal
 
 ## Support
 - Linux (Tested)
 - Windows (Tested)
-- MacOS (Not test, please submit issue if works or not)
+- MacOS (Not tested, please submit an issue if it works or not)
 
-## Installing
+## Installation
 - `pip3 install paaster`
 
 ## Commands
-- paaster --help
-    - Shows commands
-- paaster upload
-    - Upload locally encrypted clipboard to API.
-- paaster set --name "" --value ""
-    - Sets config parameters
+- `paaster --help`: Shows available commands.
+- `paaster upload`: Upload locally encrypted clipboard to the API.
+
+    Options:
+    - `-m, --mode TEXT`: Specify the mode for the paste, choose from "clipboard", "file", or "inline". (default: clipboard)
+    - `-ctc, --copy_to_clipboard BOOLEAN`: Overwrite COPY_URL_TO_CLIPBOARD setting. (default: True)
+    - `-ob, --open_browser BOOLEAN`: Overwrite OPEN_URL_IN_BROWSER setting. (default: True)
+    - `-eu, --echo_url BOOLEAN`: Overwrite ECHO_URL setting. (default: False)
+
+- `paaster set --name "" --value ""`: Set config parameters.
 
 ## Parameters
-- API_URL
-    - Backend URL, type string
-- FRONTEND_URL
-    - Frontend URL, type string
-- COPY_URL_TO_CLIPBOARD
-    - If to copy URL to clipboard, type "true/false"
-- OPEN_URL_IN_BROWSER
-    - If to open paste in browser, type "true/false"
+- `API_URL`: Backend URL, type: string.
+- `FRONTEND_URL`: Frontend URL, type: string.
+- `COPY_URL_TO_CLIPBOARD`: Copy URL to clipboard, type: "true/false".
+- `OPEN_URL_IN_BROWSER`: Open paste in the browser, type: "true/false".
```

