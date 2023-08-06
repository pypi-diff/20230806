# Comparing `tmp/typerconf-2.2.tar.gz` & `tmp/typerconf-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-2.2.tar", max compression
+gzip compressed data, was "typerconf-2.3.tar", max compression
```

## Comparing `typerconf-2.2.tar` & `typerconf-2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.2/LICENSE
--rw-r--r--   0        0        0     2907 2023-06-30 12:44:28.813745 typerconf-2.2/README.md
--rw-r--r--   0        0        0      934 2023-06-30 12:46:55.754292 typerconf-2.2/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.2/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.2/src/typerconf/Makefile
--rw-r--r--   0        0        0    11041 2023-06-30 11:46:09.116428 typerconf-2.2/src/typerconf/__init__.py
--rw-r--r--   0        0        0    31977 2023-06-30 11:44:31.096060 typerconf-2.2/src/typerconf/init.nw
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 typerconf-2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-2.3/LICENSE
+-rw-r--r--   0        0        0     2907 2023-06-30 12:44:28.813745 typerconf-2.3/README.md
+-rw-r--r--   0        0        0      934 2023-08-06 06:05:45.566209 typerconf-2.3/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-2.3/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-2.3/src/typerconf/Makefile
+-rw-r--r--   0        0        0    11100 2023-08-06 06:05:50.260873 typerconf-2.3/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    33580 2023-08-06 06:04:55.620408 typerconf-2.3/src/typerconf/init.nw
+-rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 typerconf-2.3/PKG-INFO
```

### Comparing `typerconf-2.2/LICENSE` & `typerconf-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-2.2/README.md` & `typerconf-2.3/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-2.2/pyproject.toml` & `typerconf-2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "2.2"
+version = "2.3"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-2.2/src/typerconf/__init__.py` & `typerconf-2.3/src/typerconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 normalized_path = os.path.normpath(sys.argv[0])
 basename = os.path.basename(normalized_path)
 dirs = appdirs.AppDirs(basename)
 
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data={},
+  def __init__(self, json_data=None,
                      conf_file=None):
     """
     Constructs a config object to navigate from JSON data `json_data`.
 
     `conf_file` takes a path to a file which will be used as a config file. If this 
     argument is supplied, the data will be read from the file.
 
     Also, if `conf_file` is not None, we will enable automatic write back. So 
     that any changes (invokations of the `.set` method) will be written to the 
     config file immediately.
 
     To not enable write back, load file contents with the `.read_config` method.
     """
-    self.__data = json_data
+    if not json_data:
+      self.__data = {}
+    else:
+      self.__data = json_data
     if isinstance(conf_file, io.IOBase):
       try:
         self.__conf_file = conf_file.name
       except AttributeError:
         raise ValueError(f"can't enable writeback when `conf_file` is "
                          f"a file-like object without a name: {conf_file}")
     else:
```

### Comparing `typerconf-2.2/src/typerconf/init.nw` & `typerconf-2.3/src/typerconf/init.nw`

 * *Files 1% similar despite different names*

```diff
@@ -119,30 +119,53 @@
 This class has two methods that are central:
 The first gets a value out, the other sets a value in.
 Both work with these dot-separated addresses.
 <<classes>>=
 class Config:
   """Navigates nested JSON structures by dot-separated addressing."""
 
-  def __init__(self, json_data={},
+  def __init__(self, json_data=None,
                      <<Config constructor args>>):
     """
     Constructs a config object to navigate from JSON data `json_data`.
 
     <<Config constructor args doc>>
     """
-    self.__data = json_data
+    if not json_data:
+      self.__data = {}
+    else:
+      self.__data = json_data
     <<Config attributes>>
 
   <<Config methods for get and set>>
   <<Config methods for available paths>>
   <<Config methods for reading from and writing to file>>
 @
 
-We will use the following test data for the test functions.
+We want to test the constructor.
+<<test functions>>=
+def test_constructor():
+  test_key = "courses"
+  test_value = "test"
+
+  conf = Config(json_data={test_key: test_value})
+  assert test_key in conf.get()
+
+  assert test_key not in Config(json_data={}).get()
+  assert test_key not in Config().get()
+
+  conf = Config()
+  conf.set(test_key, test_value)
+  assert conf.get(test_key) == test_value
+
+  assert test_key not in Config().get()
+@
+
+We will use the following test data for the test functions in the remainder of 
+the text.
 <<test functions>>=
 test_data = {
   "courses": {
     "datintro22": {
       "url": "https://...",
       "TAs": ["Asse", "Assa"]
     }
@@ -274,14 +297,24 @@
   path = "courses.prgx22.TAs"
   conf.set(path, value)
   gotten_value = conf.get(path)
   assert isinstance(gotten_value, list)
   assert gotten_value == value
 @
 
+We also want to test short paths.
+<<test functions>>=
+def test_set_short_path():
+  value = "Test Tester"
+  path = "contact"
+  conf.set(path, value)
+
+  assert conf.get(path) == value
+@
+
 When we want to remove a node, the pythonic way is to simply try to remove it.
 If it doesn't exist, we silently fail.
 The reasoning is as follows: the goal is to remove something; if it doesn't 
 exist, we have already achieved our goal.
 (However, giving an error, as the rm(1) command does, helps in debugging.
 But we consider this silently failing most beneficial at the moment.)
 <<remove part from the config>>=
@@ -302,14 +335,27 @@
     conf.get("test")
   except KeyError:
     assert True
   else:
     assert False
 @
 
+We also want to remove from a longer path.
+<<test functions>>=
+def test_set_path_list():
+  path = "courses.prgx22.TAs"
+  conf.set(path, None)
+  try:
+    conf.get(path)
+  except KeyError:
+    assert True
+  else:
+    assert False
+@
+
 We want to traverse the tree, we want to go to the immediate parent of the leaf 
 that we want to set a value for (or delete).
 We iterate through the path.
 <<update structure to parent node, create parents if they don't exist>>=
 for part in parts[:-1]:
   <<check if part is an integer, if so, convert it>>
   try:
@@ -750,28 +796,32 @@
 (Otherwise, JSON can't decode an empty file.)
 Then we try to get the original value and then change it.
 Finally, we try to read the config to see if the changed value was actually 
 written to the file.
 <<test functions>>=
 def test_writeback_constructor():
   with tempfile.NamedTemporaryFile("w") as tmp_conf_file:
-    tmp_conf_file_name = "/tmp/writeback" #tmp_conf_file.name
+    tmp_conf_file_name = tmp_conf_file.name
     path = "the.path"
     first_value = "1st"
     second_value = "2nd"
 
     initial_conf = Config()
+    assert initial_conf.get() == {}
+
     initial_conf.set(path, first_value)
     initial_conf.write_config(tmp_conf_file_name)
 
     conf = Config(conf_file=tmp_conf_file_name)
     assert conf.get(path) == first_value
     conf.set(path, second_value)
 
     last_conf = Config()
+    assert last_conf.get() == {}
+
     last_conf.read_config(tmp_conf_file_name)
     assert last_conf.get(path) == second_value
 <<test imports>>=
 import tempfile
 @
 
 We would like to be able to enable write back when we call [[.read_config]] 
@@ -917,14 +967,16 @@
 Additionally, if that one element is an empty string, we replace it with 
 [[None]] to trigger a delete.
 <<if [[values]] is empty string, replace it with [[None]]>>=
 if values == "":
   values = None
 @
 
+\subsection{Testing the config command}
+
 Let's test this command.
 We'll set up the testing.
 <<test functions>>=
 runner = CliRunner()
 
 def test_cli():
   <<run tests on [[cli]]>>
@@ -932,28 +984,28 @@
 from typer.testing import CliRunner
 @
 
 Let's look at the actual tests.
 <<run tests on [[cli]]>>=
 # set example data
 result = runner.invoke(cli,
-                        ["courses.datintro22.url", "--set", "https://..."])
+                       ["courses.datintro22.url", "--set", "https://..."])
 assert result.exit_code == 0
 
 # try access nonexisting
 result = runner.invoke(cli, ["courses.datintro.url"])
 assert result.exit_code == 1
 
 # access existing
 result = runner.invoke(cli, ["courses.datintro22.url"])
 assert "courses.datintro22.url = https://..." in result.stdout
 
 # clear config
 result = runner.invoke(cli,
-                        ["courses", "--set", None])
+                       ["courses", "--set", ""])
 assert result.exit_code == 0
 
 # check that it's cleared
 result = runner.invoke(cli, ["courses"])
 assert "courses" not in result.stdout
 @
 
@@ -968,14 +1020,34 @@
 
   cli = typer.Typer()
   add_config_cmd(cli, tmp_conf.name)
 
   <<run tests on [[cli]]>>
 @
 
+We'll do another round of tests, but this time for shorter paths.
+<<test functions>>=
+def test_short_paths():
+  result = runner.invoke(cli, ["contact"])
+  assert result.exit_code != 0
+
+  result = runner.invoke(cli,
+                        ["contact", "--set", "me"])
+  assert result.exit_code == 0
+
+  result = runner.invoke(cli, ["contact"])
+  assert "contact = me" in result.stdout
+
+  result = runner.invoke(cli,
+                        ["contact", "--set", ""])
+  assert result.exit_code == 0
+
+  result = runner.invoke(cli, ["contact"])
+  assert result.exit_code != 0
+@
 
 \subsection{Autocompleting the path}
 
 The [[complete_path]] function returns the possible completions for an 
 incomplete path from the command line.
 <<helper functions>>=
 def complete_path(initial_path: str, conf: Config = None):
```

### Comparing `typerconf-2.2/PKG-INFO` & `typerconf-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 2.2
+Version: 2.3
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```

