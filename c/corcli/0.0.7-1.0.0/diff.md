# Comparing `tmp/corcli-0.0.7.tar.gz` & `tmp/corcli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corcli-0.0.7.tar", last modified: Thu Jul 20 15:04:05 2023, max compression
+gzip compressed data, was "corcli-1.0.0.tar", last modified: Sun Jul 30 21:04:53 2023, max compression
```

## Comparing `corcli-0.0.7.tar` & `corcli-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:04:05.499652 corcli-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 15:03:58.000000 corcli-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 15:04:05.499652 corcli-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 15:03:58.000000 corcli-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 15:04:05.499652 corcli-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:03:58.000000 corcli-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:04:05.495651 corcli-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:04:05.499652 corcli-0.0.7/src/ccli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:03:58.000000 corcli-0.0.7/src/ccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-20 15:03:58.000000 corcli-0.0.7/src/ccli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-20 15:03:58.000000 corcli-0.0.7/src/ccli/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-20 15:03:58.000000 corcli-0.0.7/src/ccli/cortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:04:05.499652 corcli-0.0.7/src/corcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 15:04:05.000000 corcli-0.0.7/src/corcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:04:53.833898 corcli-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-30 21:04:45.000000 corcli-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 21:04:53.833898 corcli-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-30 21:04:45.000000 corcli-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-30 21:04:53.837898 corcli-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-30 21:04:45.000000 corcli-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:04:53.833898 corcli-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:04:53.833898 corcli-1.0.0/src/corcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:04:45.000000 corcli-1.0.0/src/corcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-30 21:04:45.000000 corcli-1.0.0/src/corcli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-30 21:04:45.000000 corcli-1.0.0/src/corcli/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-07-30 21:04:45.000000 corcli-1.0.0/src/corcli/cortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:04:53.833898 corcli-1.0.0/src/corcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-30 21:04:53.000000 corcli-1.0.0/src/corcli.egg-info/top_level.txt
```

### Comparing `corcli-0.0.7/LICENSE` & `corcli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corcli-0.0.7/setup.cfg` & `corcli-1.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [metadata]
 name = corcli
-version = 0.0.7
+version = 1.0.0
 author = 0xFustang
 author_email = 0xFustang@proton.me
 description = A simple CLI client for Cortex
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0xFustang/corcli
 
 [options]
 packages = find:
 package_dir = 
 	= src
 python_requires = >=3.9
 install_requires = 
-	cortex4py
-	inquirer
-	requests
+	inquirer==3.1.3
+	cortex4py==2.1.0
+	colorama==0.4.6
+	toml==0.10.2
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
-	ccli = ccli.__main__:main
+	corcli = corcli.__main__:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `corcli-0.0.7/src/ccli/__main__.py` & `corcli-1.0.0/src/corcli/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """
 Main class
 """
 import argparse
-import tomllib
 
 from getpass import getpass
 from os import environ
 from os import path
+from sys import version_info
+
+if version_info >= (3, 11): # Python 3.11 or higher
+    import tomllib
+else:
+    import toml
 
 try:
-    from ccli.analyzer import run_analyzers
+    from corcli.analyzer import run_analyzers
+    from corcli.analyzer import run_analyzers_bulk
 except ModuleNotFoundError:
     from analyzer import run_analyzers
+    from analyzer import run_analyzers_bulk
 
 def init_argparse() -> argparse.ArgumentParser:
     """Initialise the argument parsers
 
     This function creates an instance of `argparse.ArgumentParser` and configures it
     with the following command line arguments:
 
@@ -43,16 +50,18 @@
     parser.add_argument("-ha", "--hash", help="Specify the observable type as hash")
     parser.add_argument("-f", "--file", help="Specify the observable type as file")
     parser.add_argument("-m", "--mail", help="Specify the observable type as mail")
     parser.add_argument("-i", "--ip", help="Specify the observable type as ip")
     parser.add_argument("-ci", "--cortex-instance", help="Specify the Cortex instance number")
     parser.add_argument("-e", "--extract-only", help="Display only the extracted artifacts", action="store_true")
     parser.add_argument("-fr", "--full-report", help="Display the full report", action="store_true")
-    parser.add_argument("-nc", "--no_cache", help="Force no caching", action="store_true")
+    parser.add_argument("-nc", "--no-cache", help="Force no caching", action="store_true")
     parser.add_argument("-cf", "--config-file", help="Set the configuration file path")
+    parser.add_argument("-b", "--bulk", help="Submit multiple observable, read file line by line",action="store_true")
+    parser.add_argument("-df", "--download-files", help="Download all file artifacts",action="store_true")
     return parser
 
 def main() -> None:
     """Main function
 
     This function simply read the config file and build the parameters for run_analyzer
     """
@@ -82,38 +91,47 @@
         args.observable_type = 'file'
         args.observable_data = args.file
         if not path.isfile(args.file):
             print(f'File {args.file} not found')
             exit(1)
     elif args.mail:
         args.observable_type = 'mail'
+    elif args.bulk:
+        if not path.isfile(args.bulk):
+            print(f'File {args.bulk} not found.')
+            exit(1)
+
+    if args.download_files:
+        args.extract_only = True
+
+    if not path.isfile(args.config_file):
+        print(f'Error: configuration file {args.config_file} not found.')
+        exit(1)
 
     if args.config_file:
         try: # Try to open the configuration file ccli_config.toml
             with open(args.config_file) as file_obj:
                 content = file_obj.read()
-                config_data = tomllib.loads(content)
-        except FileNotFoundError:
-            """Pass except if the config file is not found
-            If the configuration file is not found, pass take the arguments passed in the command
-            """
-            pass
+                try:
+                    config_data = tomllib.loads(content)
+                except NameError: # When using toml instead of tomllib
+                    config_data = toml.loads(content)
         except Exception:
             raise Exception("Something unexepected happened...")
 
         if not args.cortex_instance:
             cortex_instance = "default"
         else:
             cortex_instance = args.cortex_instance
 
         try:
             config_cortex_info = config_data["cortex-instance"][cortex_instance]
         except KeyError:
             raise KeyError(f"cortex-instance '{cortex_instance}' not found in the config")
-        except Exception:
+        except Exception as e:
             raise Exception("Something unexepected happened...")
 
     else:
         if not args.cortex_url:
             print("Error: please provide the Cortex instance URL using -c/--cortex-url or a configuration file using -cf/--config-file option.")
             exit(1)
 
@@ -157,11 +175,28 @@
         args.api_key = environ.get('CORTEX_CLI_API')
     else:
         args.api_key = getpass("Please provide your Cortex API key:")
         print("------\n")
 
     parameters = args
 
-    run_analyzers(parameters)
+    if args.bulk:
+        args.observables_bulk = []
+        try:
+            with open(args.observable_data) as file_obj:
+                try:
+                    while line := file_obj.readline():
+                        observable = line.rstrip()
+                        args.observables_bulk.append(observable)
+                    parameters = args
+                    run_analyzers_bulk(parameters)
+                except Exception:
+                    raise Exception("Something unexepected happened...")
+        except FileNotFoundError:
+            print("When using -b/--bulk option, provide a text file using the selected observable type. For instance: -b -d domains.txt")
+        except Exception:
+            raise Exception("Something unexepected happened...")
+    else:
+        run_analyzers(parameters)
 
 if __name__ == "__main__":
     main()
```

