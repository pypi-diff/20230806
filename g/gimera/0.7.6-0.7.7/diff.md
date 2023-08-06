# Comparing `tmp/gimera-0.7.6.tar.gz` & `tmp/gimera-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.7.6.tar", last modified: Sun Aug  6 13:46:09 2023, max compression
+gzip compressed data, was "gimera-0.7.7.tar", last modified: Sun Aug  6 17:04:11 2023, max compression
```

## Comparing `gimera-0.7.6.tar` & `gimera-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 13:45:20.000000 gimera-0.7.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:46:09.415567 gimera-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-06 13:45:20.000000 gimera-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28893 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-06 13:45:20.000000 gimera-0.7.6/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:46:09.415567 gimera-0.7.6/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 13:46:09.000000 gimera-0.7.6/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-06 13:46:09.415567 gimera-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 13:45:20.000000 gimera-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:11.733677 gimera-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-06 17:03:20.000000 gimera-0.7.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 17:04:11.733677 gimera-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-06 17:03:20.000000 gimera-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:11.729677 gimera-0.7.7/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29384 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-08-06 17:03:20.000000 gimera-0.7.7/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:04:11.733677 gimera-0.7.7/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 17:04:11.000000 gimera-0.7.7/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-06 17:04:11.733677 gimera-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-06 17:03:20.000000 gimera-0.7.7/setup.py
```

### Comparing `gimera-0.7.6/LICENSE.txt` & `gimera-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/PKG-INFO` & `gimera-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.6
+Version: 0.7.7
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.6/README.md` & `gimera-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/gimera/config.py` & `gimera-0.7.7/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/gimera/gimera.py` & `gimera-0.7.7/gimera/gimera.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,33 @@
 )
 @click.option(
     "-I",
     "--non-interactive",
     is_flag=True,
     help="",
 )
+@click.option(
+    "-C",
+    "--no-auto-commit",
+    is_flag=True,
+    help="",
+)
 def apply(
     repos,
     update,
     all_integrated,
     all_submodule,
     parallel_safe,
     strict,
     recursive,
     no_patches,
     missing,
     remove_invalid_branches,
     non_interactive,
+    no_auto_commit,
 ):
     if non_interactive:
         os.environ["GIMERA_NON_INTERACTIVE"] = "1"
     if all_integrated and all_submodule:
         _raise_error("Please set either -I or -S")
     ttype = None
     ttype = REPO_TYPE_INT if all_integrated else ttype
@@ -214,26 +221,28 @@
         update,
         force_type=ttype,
         parallel_safe=parallel_safe,
         strict=strict,
         recursive=recursive,
         no_patches=no_patches,
         remove_invalid_branches=remove_invalid_branches,
+        auto_commit=no_auto_commit,
     )
 
 
 def _apply(
     repos,
     update,
     force_type=False,
     parallel_safe=False,
     strict=False,
     recursive=False,
     no_patches=False,
     remove_invalid_branches=False,
+    auto_commit=True,
 ):
     """
     :param repos: user input parameter from commandline
     :param update: bool - flag from command line
     """
     config = Config(force_type=force_type, recursive=recursive)
 
@@ -249,82 +258,85 @@
         update,
         force_type,
         parallel_safe=parallel_safe,
         strict=strict,
         recursive=recursive,
         no_patches=no_patches,
         remove_invalid_branches=remove_invalid_branches,
+        auto_commit=auto_commit,
     )
 
 
 def _internal_apply(
     repos,
     update,
     force_type,
     parallel_safe=False,
     strict=False,
     recursive=False,
     no_patches=False,
     common_vars=None,
     parent_config=None,
+    auto_commit=True,
     **options,
 ):
     common_vars = common_vars or {}
     main_repo = Repo(os.getcwd())
     config = Config(
         force_type=force_type,
         recursive=recursive,
         common_vars=common_vars,
         parent_config=parent_config,
     )
+    with main_repo.stay_at_commit(not auto_commit):
+        for repo in config.repos:
+            if not repo.enabled:
+                continue
+            if repos and str(repo.path) not in repos:
+                continue
+            _turn_into_correct_repotype(main_repo, repo, config)
+            if repo.type == REPO_TYPE_SUB:
+                _make_sure_subrepo_is_checked_out(main_repo, repo)
+                _fetch_latest_commit_in_submodule(main_repo, repo, update=update)
+            elif repo.type == REPO_TYPE_INT:
+                if not no_patches:
+                    try:
+                        make_patches(main_repo, repo)
+                    except Exception as ex:
+                        msg = f"Error making patches for: {repo.path}\n\n{ex}"
+                        _raise_error(msg)
 
-    for repo in config.repos:
-        if not repo.enabled:
-            continue
-        if repos and str(repo.path) not in repos:
-            continue
-        _turn_into_correct_repotype(main_repo, repo, config)
-        if repo.type == REPO_TYPE_SUB:
-            _make_sure_subrepo_is_checked_out(main_repo, repo)
-            _fetch_latest_commit_in_submodule(main_repo, repo, update=update)
-        elif repo.type == REPO_TYPE_INT:
-            if not no_patches:
                 try:
-                    make_patches(main_repo, repo)
+                    _update_integrated_module(
+                        main_repo, repo, update, parallel_safe, **options
+                    )
                 except Exception as ex:
-                    msg = f"Error making patches for: {repo.path}"
+                    msg = f"Error updating integrated submodules for: {repo.path}\n\n{ex}"
                     _raise_error(msg)
 
-            try:
-                _update_integrated_module(
-                    main_repo, repo, update, parallel_safe, **options
+                if not strict:
+                    # fatal: refusing to create/use '.git/modules/addons_connector/modules/addons_robot/aaa' in another submodule's git dir
+                    # not submodules inside integrated modules
+                    force_type = REPO_TYPE_INT
+
+            if recursive:
+                common_vars.update(config.yaml_config.get("common", {}).get("vars", {}))
+                _apply_subgimera(
+                    main_repo,
+                    repo,
+                    update,
+                    force_type,
+                    parallel_safe=parallel_safe,
+                    strict=strict,
+                    no_patches=no_patches,
+                    common_vars=common_vars,
+                    parent_config=config,
+                    auto_commit=auto_commit,
+                    **options,
                 )
-            except Exception as ex:
-                msg = f"Error updating integrated submodules for: {repo.path}"
-                _raise_error(msg)
-
-            if not strict:
-                # fatal: refusing to create/use '.git/modules/addons_connector/modules/addons_robot/aaa' in another submodule's git dir
-                # not submodules inside integrated modules
-                force_type = REPO_TYPE_INT
-
-        if recursive:
-            common_vars.update(config.yaml_config.get("common", {}).get("vars", {}))
-            _apply_subgimera(
-                main_repo,
-                repo,
-                update,
-                force_type,
-                parallel_safe=parallel_safe,
-                strict=strict,
-                no_patches=no_patches,
-                common_vars=common_vars,
-                parent_config=config,
-                **options,
-            )
 
 
 def _apply_subgimera(
     main_repo,
     repo,
     update,
     force_type,
```

### Comparing `gimera-0.7.6/gimera/gitcommands.py` & `gimera-0.7.7/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/gimera/patches.py` & `gimera-0.7.7/gimera/patches.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/gimera/repo.py` & `gimera-0.7.7/gimera/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import subprocess
 import click
 import shutil
 from .gitcommands import GitCommands
 from pathlib import Path
 from .tools import yieldlist, X, safe_relative_to, _raise_error, rmtree
 from .consts import gitcmd as git
+from contextlib import contextmanager
 
 
 class Repo(GitCommands):
     def __init__(self, path):
         self.path = Path(path)
 
     def __repr__(self):
@@ -352,14 +353,23 @@
             else:
                 next_path = root / part / "modules"
                 if next_path.exists():
                     root = next_path
                 else:
                     _raise_error(f"Could not find submodule in .git for {part}")
 
+    @contextmanager
+    def stay_at_commit(self, enabled):
+        commit = self.hex
+        try:
+            yield
+        finally:
+            if enabled:
+                self.X("git", "reset", "--soft", commit)
+
 
 class Remote(object):
     def __init__(self, repo, name, url):
         self.repo = repo
         self.name = name
         self.url = url
```

### Comparing `gimera-0.7.6/gimera/tools.py` & `gimera-0.7.7/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.7.6/gimera.egg-info/PKG-INFO` & `gimera-0.7.7/gimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.7.6
+Version: 0.7.7
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.7.6/setup.py` & `gimera-0.7.7/setup.py`

 * *Files identical despite different names*

