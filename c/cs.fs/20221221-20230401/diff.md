# Comparing `tmp/cs.fs-20221221.tar.gz` & `tmp/cs.fs-20230401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fs-20221221.tar", last modified: Tue Dec 20 21:09:09 2022, max compression
+gzip compressed data, was "cs.fs-20230401.tar", last modified: Sat Apr  1 05:02:36 2023, max compression
```

## Comparing `cs.fs-20221221.tar` & `cs.fs-20230401.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-20 21:09:09.542841 cs.fs-20221221/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2022-12-20 21:08:55.000000 cs.fs-20221221/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     5053 2022-12-20 21:09:09.542957 cs.fs-20221221/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     4419 2022-12-20 21:08:56.000000 cs.fs-20221221/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-20 21:09:09.538993 cs.fs-20221221/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-20 21:09:09.539296 cs.fs-20221221/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-20 21:09:09.540952 cs.fs-20221221/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)     9981 2022-12-20 21:08:41.000000 cs.fs-20221221/lib/python/cs/fs.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-12-20 21:09:09.542529 cs.fs-20221221/lib/python/cs.fs.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     5053 2022-12-20 21:09:09.000000 cs.fs-20221221/lib/python/cs.fs.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      274 2022-12-20 21:09:09.000000 cs.fs-20221221/lib/python/cs.fs.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2022-12-20 21:09:09.000000 cs.fs-20221221/lib/python/cs.fs.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       72 2022-12-20 21:09:09.000000 cs.fs-20221221/lib/python/cs.fs.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2022-12-20 21:09:09.000000 cs.fs-20221221/lib/python/cs.fs.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     5301 2022-12-20 21:09:01.000000 cs.fs-20221221/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      981 2022-12-20 21:09:09.543588 cs.fs-20221221/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2022-12-20 21:08:56.000000 cs.fs-20221221/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:02:36.368547 cs.fs-20230401/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-01 05:02:20.000000 cs.fs-20230401/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5088 2023-04-01 05:02:36.368659 cs.fs-20230401/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4454 2023-04-01 05:02:21.000000 cs.fs-20230401/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:02:36.363669 cs.fs-20230401/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:02:36.363985 cs.fs-20230401/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:02:36.365749 cs.fs-20230401/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    10106 2023-04-01 05:02:11.000000 cs.fs-20230401/lib/python/cs/fs.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:02:36.368279 cs.fs-20230401/lib/python/cs.fs.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5088 2023-04-01 05:02:36.000000 cs.fs-20230401/lib/python/cs.fs.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      274 2023-04-01 05:02:36.000000 cs.fs-20230401/lib/python/cs.fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-01 05:02:36.000000 cs.fs-20230401/lib/python/cs.fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       72 2023-04-01 05:02:36.000000 cs.fs-20230401/lib/python/cs.fs.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-01 05:02:36.000000 cs.fs-20230401/lib/python/cs.fs.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5336 2023-04-01 05:02:27.000000 cs.fs-20230401/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      981 2023-04-01 05:02:36.369219 cs.fs-20230401/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-01 05:02:21.000000 cs.fs-20230401/setup.py
```

### Comparing `cs.fs-20221221/PKG-INFO` & `cs.fs-20230401/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20221221
+Version: 20230401
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,16 +17,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20221221*:
-Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
+*Latest release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -112,14 +112,17 @@
   substitution before consideration
   The default considers "$HOME/" for replacement by "~/".
 
 # Release Log
 
 
 
+*Release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
+
 *Release 20221221*:
 Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
 
 *Release 20220918*:
 * FSPathBasedSingleton.__init__: return True on the first call, False on subsequent calls.
 * FSPathBasedSingleton.__init__: probe __dict__ for '_lock' instead of using hasattr (which plays poorly this early on with classes with their own __getattr__).
 * needdir: accept optional `log` parameter to log mkdir or makedirs.
```

### Comparing `cs.fs-20221221/README.md` & `cs.fs-20230401/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20221221*:
-Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
+*Latest release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -101,14 +101,17 @@
   substitution before consideration
   The default considers "$HOME/" for replacement by "~/".
 
 # Release Log
 
 
 
+*Release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
+
 *Release 20221221*:
 Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
 
 *Release 20220918*:
 * FSPathBasedSingleton.__init__: return True on the first call, False on subsequent calls.
 * FSPathBasedSingleton.__init__: probe __dict__ for '_lock' instead of using hasattr (which plays poorly this early on with classes with their own __getattr__).
 * needdir: accept optional `log` parameter to log mkdir or makedirs.
```

### Comparing `cs.fs-20221221/lib/python/cs/fs.py` & `cs.fs-20230401/lib/python/cs/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from icontract import require
 from typeguard import typechecked
 
 from cs.deco import decorator
 from cs.obj import SingletonMixin
 from cs.pfx import pfx_call
 
-__version__ = '20221221'
+__version__ = '20230401'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -172,15 +172,18 @@
   def __str__(self):
     return f'{self.__class__.__name__}(fspath={self.shortpath})'
 
   @property
   def shortpath(self):
     ''' The short version of `self.fspath`.
     '''
-    return shortpath(self.fspath)
+    try:
+      return shortpath(self.fspath)
+    except AttributeError:
+      return "<no-fspath>"
 
   @require(lambda subpath: not isabspath(subpath))
   def pathto(self, subpath):
     ''' The full path to `subpath`, a relative path below `self.fspath`.
     '''
     return joinpath(self.fspath, subpath)
 
@@ -190,15 +193,20 @@
     return fnmatchdir(self.fspath, fnglob)
 
 class FSPathBasedSingleton(SingletonMixin, HasFSPath):
   ''' The basis for a `SingletonMixin` based on `realpath(self.fspath)`.
   '''
 
   @classmethod
-  def _resolve_fspath(cls, fspath, envvar=None, default_attr=None):
+  def _resolve_fspath(
+      cls,
+      fspath: Optional[str],
+      envvar: Optional[str] = None,
+      default_attr=None
+  ):
     ''' Resolve the filesystem path `fspath` using `os.path.realpath`.
 
         Parameters:
         * `fspath`: the filesystem path to resolve;
           this may be `None` to use the class defaults
         * `envvar`: the environment variable to consult for a default `fspath`;
           the default for this comes from `cls.FSPATH_ENVVAR` if defined
```

### Comparing `cs.fs-20221221/lib/python/cs.fs.egg-info/PKG-INFO` & `cs.fs-20230401/lib/python/cs.fs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20221221
+Version: 20230401
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -17,16 +17,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20221221*:
-Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
+*Latest release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -112,14 +112,17 @@
   substitution before consideration
   The default considers "$HOME/" for replacement by "~/".
 
 # Release Log
 
 
 
+*Release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
+
 *Release 20221221*:
 Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
 
 *Release 20220918*:
 * FSPathBasedSingleton.__init__: return True on the first call, False on subsequent calls.
 * FSPathBasedSingleton.__init__: probe __dict__ for '_lock' instead of using hasattr (which plays poorly this early on with classes with their own __getattr__).
 * needdir: accept optional `log` parameter to log mkdir or makedirs.
```

### Comparing `cs.fs-20221221/pyproject.toml` & `cs.fs-20230401/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,45 +5,45 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20221214",
+    "cs.deco>=20230331",
     "cs.obj>=20220918",
-    "cs.pfx>=20221118",
+    "cs.pfx>=20230331",
     "icontract",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20221221"
+version = "20230401"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20221221*:
-Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
+*Latest release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -129,14 +129,17 @@
   substitution before consideration
   The default considers \"$HOME/\" for replacement by \"~/\".
 
 # Release Log
 
 
 
+*Release 20230401*:
+HasFSPath.shortpath: hand call before .fspath set.
+
 *Release 20221221*:
 Replace use of cs.env.envsub with os.path.expandvars and drop unused environ parameter.
 
 *Release 20220918*:
 * FSPathBasedSingleton.__init__: return True on the first call, False on subsequent calls.
 * FSPathBasedSingleton.__init__: probe __dict__ for '_lock' instead of using hasattr (which plays poorly this early on with classes with their own __getattr__).
 * needdir: accept optional `log` parameter to log mkdir or makedirs.
```

### Comparing `cs.fs-20221221/setup.cfg` & `cs.fs-20230401/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.fs
-version = 20221221
+version = 20230401
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -19,17 +19,17 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.deco>=20221214
+	cs.deco>=20230331
 	cs.obj>=20220918
-	cs.pfx>=20221118
+	cs.pfx>=20230331
 	icontract
 	typeguard
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

