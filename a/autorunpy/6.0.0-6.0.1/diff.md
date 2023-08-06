# Comparing `tmp/autorunpy-6.0.0.tar.gz` & `tmp/autorunpy-6.0.1.tar.gz`

## Comparing `autorunpy-6.0.0.tar` & `autorunpy-6.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.gitattributes
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/auto.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/dl_and_ret_dirpath.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/github_release.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/ret_module_2_run_name.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 autorunpy-6.0.0/src/autorunpy/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-6.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-6.0.0/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-6.0.0/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 autorunpy-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 autorunpy-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autorunpy-6.0.1/.gitattributes
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-6.0.1/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/auto.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/dl_and_ret_dirpath.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/github_release.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/ret_module_2_run_name.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 autorunpy-6.0.1/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-6.0.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-6.0.1/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-6.0.1/README.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 autorunpy-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 autorunpy-6.0.1/PKG-INFO
```

### Comparing `autorunpy-6.0.0/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-6.0.1/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.0/src/autorunpy/auto.py` & `autorunpy-6.0.1/src/autorunpy/auto.py`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.0/src/autorunpy/github_release.py` & `autorunpy-6.0.1/src/autorunpy/github_release.py`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.0/src/autorunpy/util.py` & `autorunpy-6.0.1/src/autorunpy/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     return UserRepo(user_name , repo_name , user_slash_repo , user_und_repo)
 
 def read_json(fp) :
     # if fp is not entered with .json extension, add it
     fp = Path(fp).with_suffix('.json')
 
     # assume cd is the GitHub dir
-    fp = Path.cwd() / fp
+    fp = Path.cwd() / 'auto-run-configs' / fp
 
     with open(fp , 'r') as f :
         return json.load(f)
```

### Comparing `autorunpy-6.0.0/.gitignore` & `autorunpy-6.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.0/LICENSE` & `autorunpy-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.0/PKG-INFO` & `autorunpy-6.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autorunpy
-Version: 6.0.0
+Version: 6.0.1
 Summary: Tools for auto running python scripts
 Project-URL: Homepage, https://github.com/imahdimir/pyautorun
 Project-URL: Bug Tracker, https://github.com/imahdimir/pyautorun/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
```

