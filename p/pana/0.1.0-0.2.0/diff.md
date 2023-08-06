# Comparing `tmp/pana-0.1.0.tar.gz` & `tmp/pana-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pana-0.1.0.tar", last modified: Wed Jul 12 08:24:11 2023, max compression
+gzip compressed data, was "pana-0.2.0.tar", last modified: Sun Aug  6 21:37:23 2023, max compression
```

## Comparing `pana-0.1.0.tar` & `pana-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-07-12 08:24:11.821014 pana-0.1.0/
--rw-r--r--   0 azazel     (501) staff       (20)     1301 2023-07-11 00:01:43.000000 pana-0.1.0/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)     1963 2023-07-12 08:24:11.820858 pana-0.1.0/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)     1492 2023-07-12 08:14:17.000000 pana-0.1.0/README.md
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-07-12 08:24:11.820665 pana-0.1.0/pana.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     1963 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      204 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       40 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)       18 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)        5 2023-07-12 08:24:11.000000 pana-0.1.0/pana.egg-info/top_level.txt
--rw-r--r--   0 azazel     (501) staff       (20)     2859 2023-07-12 08:14:41.000000 pana-0.1.0/pana.py
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-07-12 08:24:11.821055 pana-0.1.0/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     1024 2023-07-12 08:22:58.000000 pana-0.1.0/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-08-06 21:37:23.459187 pana-0.2.0/
+-rw-r--r--   0 azazel     (501) staff       (20)     1301 2023-07-11 00:01:43.000000 pana-0.2.0/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1659 2023-08-06 21:37:23.459026 pana-0.2.0/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     1188 2023-08-06 21:34:13.000000 pana-0.2.0/README.md
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-08-06 21:37:23.458840 pana-0.2.0/pana.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1659 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      204 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       40 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       18 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        5 2023-08-06 21:37:23.000000 pana-0.2.0/pana.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     2944 2023-08-06 21:13:52.000000 pana-0.2.0/pana.py
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2023-08-06 21:37:23.459229 pana-0.2.0/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1024 2023-08-06 21:18:01.000000 pana-0.2.0/setup.py
```

### Comparing `pana-0.1.0/LICENSE` & `pana-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pana-0.1.0/PKG-INFO` & `pana-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pana
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pana is a CLI and module built to check if a package name or username is available from common package managers.
 Home-page: https://github.com/azazelm3dj3d/pana
 Author: azazelm3dj3d
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -24,48 +24,40 @@
 
 ```bash
 pip install pana
 ```
 
 ## Package Managers
 
-:white_check_mark: - Actively supported & tested
-
-:warning: - In development
-
-:question: - Not started, but I'd like to eventually get them added
-
 | Package Manager                                              | Status               |
 |--------------------------------------------------------------|----------------------|
 | [PyPI](https://pypi.org/)                                    |  :white_check_mark:  |
 | [npm](https://www.npmjs.com/)                                |  :white_check_mark:  |
 | [NuGet](https://www.nuget.org/)                              |  :white_check_mark:  |
-| [crates](https://crates.io/)                                 |  :question:           |
-| [packagist](https://packagist.org/)                          |  :question:          |
-| [VSCode Marketplace](https://marketplace.visualstudio.com/)  |  :question:          |
+| [crates](https://crates.io/)                                 |  :white_check_mark:  |
 
 ## Examplea
 
 ### Module
 ```python
 from pana import Pana
 
 # Print both lists to stdout
 print(Pana.check_pkg("pana"))
 print(Pana.check_user("azazelm3dj3d"))
 
 # Example output
 """
 [
-    ['pypi', True],
-    ['npm', True],
-    ['nuget', False]
+  ['pypi', False],
+  ['npm', False],
+  ['nuget', True],
+  ['crates/docs', False]
 ]
 """
-
 ```
 
 ### CLI
 
 Search for a specific package
 
 ```bash
```

### Comparing `pana-0.1.0/README.md` & `pana-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,48 +11,40 @@
 
 ```bash
 pip install pana
 ```
 
 ## Package Managers
 
-:white_check_mark: - Actively supported & tested
-
-:warning: - In development
-
-:question: - Not started, but I'd like to eventually get them added
-
 | Package Manager                                              | Status               |
 |--------------------------------------------------------------|----------------------|
 | [PyPI](https://pypi.org/)                                    |  :white_check_mark:  |
 | [npm](https://www.npmjs.com/)                                |  :white_check_mark:  |
 | [NuGet](https://www.nuget.org/)                              |  :white_check_mark:  |
-| [crates](https://crates.io/)                                 |  :question:           |
-| [packagist](https://packagist.org/)                          |  :question:          |
-| [VSCode Marketplace](https://marketplace.visualstudio.com/)  |  :question:          |
+| [crates](https://crates.io/)                                 |  :white_check_mark:  |
 
 ## Examplea
 
 ### Module
 ```python
 from pana import Pana
 
 # Print both lists to stdout
 print(Pana.check_pkg("pana"))
 print(Pana.check_user("azazelm3dj3d"))
 
 # Example output
 """
 [
-    ['pypi', True],
-    ['npm', True],
-    ['nuget', False]
+  ['pypi', False],
+  ['npm', False],
+  ['nuget', True],
+  ['crates/docs', False]
 ]
 """
-
 ```
 
 ### CLI
 
 Search for a specific package
 
 ```bash
```

### Comparing `pana-0.1.0/pana.egg-info/PKG-INFO` & `pana-0.2.0/pana.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pana
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pana is a CLI and module built to check if a package name or username is available from common package managers.
 Home-page: https://github.com/azazelm3dj3d/pana
 Author: azazelm3dj3d
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -24,48 +24,40 @@
 
 ```bash
 pip install pana
 ```
 
 ## Package Managers
 
-:white_check_mark: - Actively supported & tested
-
-:warning: - In development
-
-:question: - Not started, but I'd like to eventually get them added
-
 | Package Manager                                              | Status               |
 |--------------------------------------------------------------|----------------------|
 | [PyPI](https://pypi.org/)                                    |  :white_check_mark:  |
 | [npm](https://www.npmjs.com/)                                |  :white_check_mark:  |
 | [NuGet](https://www.nuget.org/)                              |  :white_check_mark:  |
-| [crates](https://crates.io/)                                 |  :question:           |
-| [packagist](https://packagist.org/)                          |  :question:          |
-| [VSCode Marketplace](https://marketplace.visualstudio.com/)  |  :question:          |
+| [crates](https://crates.io/)                                 |  :white_check_mark:  |
 
 ## Examplea
 
 ### Module
 ```python
 from pana import Pana
 
 # Print both lists to stdout
 print(Pana.check_pkg("pana"))
 print(Pana.check_user("azazelm3dj3d"))
 
 # Example output
 """
 [
-    ['pypi', True],
-    ['npm', True],
-    ['nuget', False]
+  ['pypi', False],
+  ['npm', False],
+  ['nuget', True],
+  ['crates/docs', False]
 ]
 """
-
 ```
 
 ### CLI
 
 Search for a specific package
 
 ```bash
```

### Comparing `pana-0.1.0/pana.py` & `pana-0.2.0/pana.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from colorama import Fore, Style
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-p', '--pkg', help="Name of the package", default=None, required=False)
 parser.add_argument('-u', '--user', help="Name of the username", default=None, required=False)
 args = parser.parse_args()
 
-version = "0.1.0"
+version = "0.2.0"
 
 banner = \
 f"""
  ____  _____ ____  _____ 
 |  _ \(____ |  _ \(____ |
 | |_| / ___ | | | / ___ |
 |  __/\_____|_| |_\_____|
@@ -29,64 +29,66 @@
 class Pana:
 
     def check_pkg(pkg_name: str) -> list:
 
         pkg_config = {
             "pypi": f"https://pypi.org/project/{pkg_name}",
             "npm": f"https://www.npmjs.com/package/{pkg_name}",
-            "nuget": f"https://www.nuget.org/packages/{pkg_name}"
+            "nuget": f"https://www.nuget.org/packages/{pkg_name}",
+            "crates/docs": f"https://docs.rs/crate/{pkg_name}",
         }
 
         pkg_arr = []
 
+        if args.pkg is not None:
+            print(f"\n{Fore.BLUE}Checking package:{Style.RESET_ALL} {args.pkg}")
+
         for p in pkg_config:
-            if args.pkg is not None:
-                print(f"\n{Fore.BLUE}Checking...{Style.RESET_ALL} {pkg_config[p]}")
-            
             response = requests.get(pkg_config[p])
 
             if response.status_code == 200:
                 if args.pkg is not None:
-                    print(f"{Fore.RED}[{p}]{Style.RESET_ALL} Package name taken")
+                    print(f"[{Fore.RED}{p}{Style.RESET_ALL}] Package name taken")
                 
                 pkg_arr.append([p, False])
 
             if response.status_code == 404:
                 if args.pkg is not None:
-                    print(f"{Fore.GREEN}[{p}]{Style.RESET_ALL} Package name available")
+                    print(f"[{Fore.GREEN}{p}{Style.RESET_ALL}] Package name available")
                 
                 pkg_arr.append([p, True])
         
         return pkg_arr
 
     def check_user(user: str) -> list:
 
         user_config = {
             "pypi": f"https://pypi.org/user/{user}",
             "npm": f"https://www.npmjs.com/~{user}",
-            "nuget": f"https://www.nuget.org/profiles/{user}"
+            "nuget": f"https://www.nuget.org/profiles/{user}",
+            "crates/docs": f"https://github.com/{user}"
         }
 
         pkg_arr = []
 
+        if args.user is not None:
+            print(f"\n{Fore.BLUE}Checking username:{Style.RESET_ALL} {args.user}")
+
         for p in user_config:
-            if args.user is not None:
-                print(f"\n{Fore.BLUE}Checking...{Style.RESET_ALL} {user_config[p]}")
-            
             response = requests.get(user_config[p])
 
             if response.status_code == 200:
                 if args.user is not None:
-                    print(f"{Fore.RED}[{p}]{Style.RESET_ALL} Username taken")
+                    print(f"[{Fore.RED}{p}{Style.RESET_ALL}] Username taken")
                 
                 pkg_arr.append([p, False])
 
             if response.status_code == 404:
                 if args.user is not None:
-                    print(f"{Fore.GREEN}[{p}]{Style.RESET_ALL} Username available")
+                    print(f"[{Fore.GREEN}{p}{Style.RESET_ALL}] Username available")
                 
                 pkg_arr.append([p, True])
             
         return pkg_arr
 
     def main():
         print(banner)
```

### Comparing `pana-0.1.0/setup.py` & `pana-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "pana",
-    version = "0.1.0",
+    version = "0.2.0",
     author = "azazelm3dj3d",
     description = "Pana is a CLI and module built to check if a package name or username is available from common package managers.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/azazelm3dj3d/pana",
     classifiers = [
         "Programming Language :: Python :: 3",
```

