# Comparing `tmp/shellserver-0.0.8.tar.gz` & `tmp/shellserver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellserver-0.0.8.tar", last modified: Fri Jan  6 08:10:42 2023, max compression
+gzip compressed data, was "shellserver-0.0.9.tar", last modified: Tue Jan 24 06:32:00 2023, max compression
```

## Comparing `shellserver-0.0.8.tar` & `shellserver-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 08:10:42.221955 shellserver-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-03-20 04:28:04.000000 shellserver-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4057 2023-01-06 08:10:42.206332 shellserver-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3745 2023-01-06 07:47:54.000000 shellserver-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-01-06 08:10:42.221955 shellserver-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      778 2023-01-06 07:48:27.000000 shellserver-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-06 08:10:42.175087 shellserver-0.0.8/shellserver/
--rw-rw-rw-   0        0        0      156 2022-11-15 11:49:39.000000 shellserver-0.0.8/shellserver/__init__.py
--rw-rw-rw-   0        0        0      234 2022-12-29 02:32:56.000000 shellserver-0.0.8/shellserver/__main__.py
--rw-rw-rw-   0        0        0     3762 2022-12-30 00:09:12.000000 shellserver-0.0.8/shellserver/classes.py
--rw-rw-rw-   0        0        0      710 2022-12-21 04:22:17.000000 shellserver-0.0.8/shellserver/cli.py
-drwxrwxrwx   0        0        0        0 2023-01-06 08:10:42.206332 shellserver-0.0.8/shellserver/gitstatus/
--rw-rw-rw-   0        0        0      980 2023-01-05 06:10:10.000000 shellserver-0.0.8/shellserver/gitstatus/__init__.py
--rw-rw-rw-   0        0        0     9233 2023-01-06 07:21:46.000000 shellserver-0.0.8/shellserver/gitstatus/high.py
--rw-rw-rw-   0        0        0     8450 2023-01-06 06:34:39.000000 shellserver-0.0.8/shellserver/gitstatus/low.py
--rw-rw-rw-   0        0        0     5221 2023-01-06 06:44:52.000000 shellserver-0.0.8/shellserver/gitstatus/medium.py
--rw-rw-rw-   0        0        0     2957 2023-01-02 09:52:49.000000 shellserver-0.0.8/shellserver/gitstatus/packs.py
--rw-rw-rw-   0        0        0    23557 2023-01-06 07:42:23.000000 shellserver-0.0.8/shellserver/gitstatus/tests.py
--rw-rw-rw-   0        0        0     1359 2022-12-13 03:27:36.000000 shellserver-0.0.8/shellserver/histdb.py
--rw-rw-rw-   0        0        0     6996 2023-01-04 10:14:48.000000 shellserver-0.0.8/shellserver/server.py
--rw-rw-rw-   0        0        0     5678 2022-12-24 04:25:42.000000 shellserver-0.0.8/shellserver/style.py
--rw-rw-rw-   0        0        0     4103 2022-12-13 18:34:56.000000 shellserver-0.0.8/shellserver/theme.py
-drwxrwxrwx   0        0        0        0 2023-01-06 08:10:42.190798 shellserver-0.0.8/shellserver.egg-info/
--rw-rw-rw-   0        0        0     4057 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-01-06 08:10:42.000000 shellserver-0.0.8/shellserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-24 06:32:00.127877 shellserver-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-03-20 04:28:04.000000 shellserver-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4096 2023-01-24 06:32:00.127877 shellserver-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3783 2023-01-24 06:24:56.000000 shellserver-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-24 06:32:00.127877 shellserver-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-01-24 06:31:36.000000 shellserver-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-24 06:32:00.096200 shellserver-0.0.9/shellserver/
+-rw-rw-rw-   0        0        0      156 2022-11-15 11:49:39.000000 shellserver-0.0.9/shellserver/__init__.py
+-rw-rw-rw-   0        0        0      234 2022-12-29 02:32:56.000000 shellserver-0.0.9/shellserver/__main__.py
+-rw-rw-rw-   0        0        0     3762 2022-12-30 00:09:12.000000 shellserver-0.0.9/shellserver/classes.py
+-rw-rw-rw-   0        0        0      710 2022-12-21 04:22:17.000000 shellserver-0.0.9/shellserver/cli.py
+drwxrwxrwx   0        0        0        0 2023-01-24 06:32:00.127877 shellserver-0.0.9/shellserver/gitstatus/
+-rw-rw-rw-   0        0        0      988 2023-01-07 06:37:08.000000 shellserver-0.0.9/shellserver/gitstatus/__init__.py
+-rw-rw-rw-   0        0        0     9147 2023-01-24 05:17:44.000000 shellserver-0.0.9/shellserver/gitstatus/high.py
+-rw-rw-rw-   0        0        0     8963 2023-01-24 05:17:23.000000 shellserver-0.0.9/shellserver/gitstatus/low.py
+-rw-rw-rw-   0        0        0     5380 2023-01-23 02:17:15.000000 shellserver-0.0.9/shellserver/gitstatus/medium.py
+-rw-rw-rw-   0        0        0     3409 2023-01-24 04:56:36.000000 shellserver-0.0.9/shellserver/gitstatus/packs.py
+-rw-rw-rw-   0        0        0    25600 2023-01-14 23:30:32.000000 shellserver-0.0.9/shellserver/gitstatus/tests.py
+-rw-rw-rw-   0        0        0     1359 2022-12-13 03:27:36.000000 shellserver-0.0.9/shellserver/histdb.py
+-rw-rw-rw-   0        0        0     6741 2023-01-22 08:40:47.000000 shellserver-0.0.9/shellserver/server.py
+-rw-rw-rw-   0        0        0     5678 2022-12-24 04:25:42.000000 shellserver-0.0.9/shellserver/style.py
+-rw-rw-rw-   0        0        0     4103 2022-12-13 18:34:56.000000 shellserver-0.0.9/shellserver/theme.py
+drwxrwxrwx   0        0        0        0 2023-01-24 06:32:00.111831 shellserver-0.0.9/shellserver.egg-info/
+-rw-rw-rw-   0        0        0     4096 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-01-24 06:32:00.000000 shellserver-0.0.9/shellserver.egg-info/top_level.txt
```

### Comparing `shellserver-0.0.8/LICENSE` & `shellserver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/PKG-INFO` & `shellserver-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: shellserver
-Version: 0.0.8
-Summary: Server to aid shell navigation
+Version: 0.0.9
+Summary: Server to aid shell navigation.
 Home-page: https://github.com/HenriquedoVal/shellserver
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellServer
 
 It's a mix of [Starship](https://github.com/starship/starship) and [Zoxide](https://github.com/ajeetdsouza/zoxide) but faster.  
   
 On Starship, every 'Enter' keystroke spawns a new process, which may cause a lag between prompts.  
 Zoxide will raise a new process every time you call it.  
 ShellServer raises the server only in the first shell creation and will _communicate_ with your shell on every 'Enter' keystroke.  
+Fastness comes from not having spawning time, which seems to be way higher in Windows.  
   
 But if your hardware gives you a fluid shell experience using Starship, I recommend that you keep with it because it's way more customizable.  
 
 ## Features
   
 ### Prompt with a fast glance at what is in directory  
 
@@ -33,14 +34,15 @@
 ![Fast](./images/even_bloated.gif)  
   
 ### Better 'cd'  
 
 ![p, pz](./images/p_pz.gif)
 - Tab completions works just fine.
 - With no arguments will behave just like 'cd'.
+- `p -o path` for writing to output. Tool for things like `move somefile (p -o somepath)`
 Note: [fzf](https://github.com/junegunn/fzf) is a dependency to use 'pz'  
   
 ### Switching Theme
   
 ![Switch-Theme](./images/switch_theme.gif)
 Can take four arguments: all, system, terminal, and blue.  
 - terminal: Toggles Windows Terminal default theme between 'Tango Dark' and 'Solarized Light'.  
@@ -96,20 +98,18 @@
 Import-Module ShellServer
 ~~~
 
 ### Keep updated
 As many things might change in versions below 0.1.0, `pip install --upgrade shellserver` and `Upgrade-Module ShellServer` must be run both when one changes.  
 The last v0.0.8 will work with the PowerShell ShellServer module 0.0.6.
 
-## Known Issues
-
-- Git status info: Now we can parse git packfiles, but still can't resolve deltas. So it will fall back to use git when it's needed (faster but still experimental). Do `pythonw -m shellserver --use-git` in your profile to always use git.
-
 ## Debugging
 
+The git status info still experimental, do `pythonw -m shellserver --use-git` in your profile to always use git. 
+
 Any errors that occur will be saved in `$env:localappdata\shellserver\traceback`.  
   
 Attach a _stdout_ to the server, pass `--verbose` to it and it will give lot of info when it sees a git repo.
 ~~~
 shellserver kill
 # A message that the server is not responding and your prompt will be like before.
 python -m shellserver --verbose  # no w, blocking
```

### Comparing `shellserver-0.0.8/README.md` & `shellserver-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ShellServer
 
 It's a mix of [Starship](https://github.com/starship/starship) and [Zoxide](https://github.com/ajeetdsouza/zoxide) but faster.  
   
 On Starship, every 'Enter' keystroke spawns a new process, which may cause a lag between prompts.  
 Zoxide will raise a new process every time you call it.  
 ShellServer raises the server only in the first shell creation and will _communicate_ with your shell on every 'Enter' keystroke.  
+Fastness comes from not having spawning time, which seems to be way higher in Windows.  
   
 But if your hardware gives you a fluid shell experience using Starship, I recommend that you keep with it because it's way more customizable.  
 
 ## Features
   
 ### Prompt with a fast glance at what is in directory  
 
@@ -22,14 +23,15 @@
 ![Fast](./images/even_bloated.gif)  
   
 ### Better 'cd'  
 
 ![p, pz](./images/p_pz.gif)
 - Tab completions works just fine.
 - With no arguments will behave just like 'cd'.
+- `p -o path` for writing to output. Tool for things like `move somefile (p -o somepath)`
 Note: [fzf](https://github.com/junegunn/fzf) is a dependency to use 'pz'  
   
 ### Switching Theme
   
 ![Switch-Theme](./images/switch_theme.gif)
 Can take four arguments: all, system, terminal, and blue.  
 - terminal: Toggles Windows Terminal default theme between 'Tango Dark' and 'Solarized Light'.  
@@ -85,20 +87,18 @@
 Import-Module ShellServer
 ~~~
 
 ### Keep updated
 As many things might change in versions below 0.1.0, `pip install --upgrade shellserver` and `Upgrade-Module ShellServer` must be run both when one changes.  
 The last v0.0.8 will work with the PowerShell ShellServer module 0.0.6.
 
-## Known Issues
-
-- Git status info: Now we can parse git packfiles, but still can't resolve deltas. So it will fall back to use git when it's needed (faster but still experimental). Do `pythonw -m shellserver --use-git` in your profile to always use git.
-
 ## Debugging
 
+The git status info still experimental, do `pythonw -m shellserver --use-git` in your profile to always use git. 
+
 Any errors that occur will be saved in `$env:localappdata\shellserver\traceback`.  
   
 Attach a _stdout_ to the server, pass `--verbose` to it and it will give lot of info when it sees a git repo.
 ~~~
 shellserver kill
 # A message that the server is not responding and your prompt will be like before.
 python -m shellserver --verbose  # no w, blocking
```

### Comparing `shellserver-0.0.8/setup.py` & `shellserver-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
-with open('README.md') as f:
+with open('README.md', 'r') as f:
     page_description = f.read()
 
 # Must be full path for build to find
-with open('C:\\Users\\henri\\github\\shellserver\\requirements.txt') as f:
+with open('C:\\Users\\henri\\Github\\shellserver\\requirements.txt') as f:
     requirements = f.read()
 
 setup(
     name='shellserver',
-    version='0.0.8',
+    version='0.0.9',
     author='Henrique do Val',
     author_email='henrique.val@hotmail.com',
-    description='Server to aid shell navigation',
+    description='Server to aid shell navigation.',
     long_description=page_description,
     long_description_content_type='text/markdown',
     url='https://github.com/HenriquedoVal/shellserver',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'shellserver = shellserver.cli:main',
+            'shellserver = shellserver.cli:main'
         ]},
     install_requires=requirements,
     python_requires='>=3.10'
 )
```

### Comparing `shellserver-0.0.8/shellserver/classes.py` & `shellserver-0.0.9/shellserver/classes.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/shellserver/cli.py` & `shellserver-0.0.9/shellserver/cli.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/shellserver/gitstatus/__init__.py` & `shellserver-0.0.9/shellserver/gitstatus/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,22 @@
     git_dir = low.get_dot_git(target_path)
 
     if git_dir is not None and low.exists_head(git_dir):
         branch = low.get_branch_on_head(git_dir)
     else:
         return None, None
 
+    obj = high.High(git_dir, branch)
     try:
         if '--use-git' in sys.argv:
             raise high.FallbackError
-        status = high.status(git_dir, branch)
+        status = obj.status()
 
     except high.FallbackError:
-        status = low.parse_git_status(git_dir)
+        status = obj.parse_git_status()
 
     except Exception:
         if '--let-crash' in sys.argv:
             raise
-        status = low.parse_git_status(git_dir)
+        status = obj.parse_git_status()
 
     return branch, status
```

### Comparing `shellserver-0.0.8/shellserver/gitstatus/high.py` & `shellserver-0.0.9/shellserver/gitstatus/high.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,274 +12,255 @@
 os = low.os  # os module
 
 n = '\n\n'
 if '--verbose' not in sys.argv:
     sys.stdout = None
 
 
-# instead of raising fallback, it should build the deltas
 class FallbackError(Exception):
     pass
 
 
-def status(git_dir: str, branch: str) -> str | None:
-    """
-    Do a inline version of 'git status' without any use of git.
-    param `git_dir`: The directory where .git resides.
-    param `branch`: The name of the branch to get status.
-    return: str | None: String with the status, None if there's
-                        nothing to report.
-    """
-
-    print('GIT_DIR:', git_dir)
-    print('Branch', branch, end=n)
-
-    fixed, ignored = medium.get_split_ignored(git_dir)
-
-    index_tracked = medium.get_index_tracked(git_dir)
-
-    packs_list = medium.get_packs(git_dir)
-    print('List of packfiles:', *packs_list, sep='\n', end=n)
-
-    untracked, staged, modified, deleted = get_full_status(
-        git_dir, branch, fixed, ignored, index_tracked, packs_list
-    )
-
-    return low.get_status_string((untracked, staged, modified, deleted))
-
-
-def get_full_status(
-    git_dir: str,
-    branch: str,
-    fixed: list,
-    ignored: list,
-    index_tracked: list,
-    packs_list: list,
-    recurse_path=None,
-    tree_hash=None
-) -> tuple[int, int, int, int]:
-    """
-    Carries all the workload of getting a status.
-    param `git_dir`: The directory where .git resides.
-    param `branch`: The actual branch of git.
-    param `fixed`: list of full paths in both '.gitignore' and 'exclude'.
-    param `ignored`: list of relative paths in both '.gitignore' and 'exclude'.
-    param `index_tracked`: list of files tracked in git index.
-    param `packs_list`: list of full paths of packfiles.
-    param `recurse_path`: For recursive use.
-    param `tree_hash`: For recursive use.
-    return: tuple: tuple of four integer numbers representing the number of
-                    untracked, staged, modified and deleted files.
-    """
-
-    untracked = staged = modified = deleted = 0
-
-    if recurse_path is None:
-        recurse_path = git_dir
-
-    tree_items_list = []
-    # will happen only in very first call
-    if tree_hash is None:
-        last_cmmt = medium.get_last_commit_hash(git_dir, branch)
-        if last_cmmt is not None:
-            res = get_tree_items(git_dir, last_cmmt, packs_list)
-            if res is not None:
-                tree_items_list = res
-    # all recursive calls must fall here
-    else:
-        tree_items_list = get_tree_items_from_hash(
-            git_dir, tree_hash, packs_list
+class High(medium.Medium):
+
+    __slots__ = 'git_dir', 'branch', 'fixed', 'ignored', 'packs_list'
+
+    def __init__(self, git_dir: str, branch: str) -> None:
+        self.git_dir = git_dir
+        self.branch = branch
+
+        print('GIT_DIR:', git_dir)
+        print('Branch', branch, end=n)
+
+        self.set_split_ignored()
+        self.set_index_tracked()
+        self.set_packs()
+        print('List of packfiles:', self.packs_list, sep='\n', end=n)
+
+    def status(self):
+        """
+        Do a inline version of 'git status' without any use of git.
+        return: str | None: String with the status, None if there's
+                            nothing to report.
+        """
+        untracked, staged, modified, deleted = self.get_full_status(
+            recurse_path=self.git_dir
         )
 
-    try:
-        directory = os.scandir(recurse_path)
-    except PermissionError:
-        return untracked, staged, modified, deleted
+        return self.get_status_string((untracked, staged, modified, deleted))
 
-    # index will have only the full path of blobs
-    # trees have everything
-    found_in_tree = 0
-    for file in directory:
-
-        relpath = os.path.relpath(
-            file.path, git_dir
-        ).replace('\\', '/', -1)
-
-        if file.is_file() and relpath in index_tracked:
-            if file.name not in (i[2] for i in tree_items_list):
-                print('Staged:', file.name, "isn't under a commit.")
-                staged += 1
-                continue
+    def get_full_status(
+        self,
+        recurse_path,
+        tree_hash=None
+    ) -> tuple[int, int, int, int]:
+        """
+        Carries all the workload of getting a status.
+        param `recurse_path`: For recursive use.
+        param `tree_hash`: For recursive use.
+        return: tuple: tuple of four integer numbers representing the number of
+                        untracked, staged, modified and deleted files.
+        """
+
+        untracked = staged = modified = deleted = 0
+
+        tree_items_list = []
+        # will happen only in very first call
+        if tree_hash is None:
+            last_cmmt = self.get_last_commit_hash()
+            if last_cmmt is not None:
+                res = self.get_tree_items(last_cmmt)
+                if res is not None:
+                    tree_items_list = res
+                    print('Found:', *tree_items_list, sep='\n', end=n)
+        # all recursive calls will fall here
+        else:
+            tree_items_list = self.get_tree_items_from_hash(tree_hash)
 
-            found_in_tree += 1
-            if ('100644', low.get_hash_of_file(file.path), file.name) in tree_items_list:  # noqa
-                continue
-            elif ('100644', low.get_hash_of_file(file.path, use_cr=True), file.name) in tree_items_list:  # noqa
+        try:
+            directory = os.scandir(recurse_path)
+        except PermissionError:
+            return untracked, staged, modified, deleted
+
+        # index will have only the full path of blobs
+        # trees have everything
+        found_in_tree = 0
+        for file in directory:
+
+            if file.is_symlink():
+                # it would raise PermissionError when calling .is_file()
                 continue
-            print('Modified:', file.name, "has different sha1.")
-            modified += 1
 
-        elif file.name == '.git':
-            pass
+            relpath = os.path.relpath(
+                file.path, self.git_dir
+            ).replace('\\', '/', -1)
+
+            # 100755(exe) is file
+            if file.is_file() and relpath in self.index_tracked:
+                # if file not in tree
+                if file.name not in (i[2] for i in tree_items_list):
+                    print('Staged:', file.name, "isn't under a commit.")
+                    staged += 1
+                    continue
+
+                # the check if file.name is file is done above
+                for item in tree_items_list:
+                    if item[2] == file.name:
+                        break
+                else:
+                    continue
+
+                found_in_tree += 1
+                file_hash = self.get_hash_of_file(file.path)
+                file_hash_in_tree = item[1]
+
+                if file_hash_in_tree == file_hash:
+                    continue
+                elif file_hash_in_tree == self.get_hash_of_file(file.path,
+                                                                use_cr=True):
+                    continue
+                modified += 1
+
+                print('Modified:', file.name,
+                      f"has different sha1: {file_hash}")
+
+            elif file.name == '.git':
+                pass
+
+            elif any(fnmatch(file.name, pattern) for pattern in self.ignored):
+                pass
+            elif any(fnmatch(relpath, pattern) for pattern in self.fixed):
+                pass
 
-        elif any(fnmatch(file.name, pat) for pat in ignored):
-            pass
-        elif any(fnmatch(relpath, pat) for pat in fixed):
-            pass
-
-        elif file.is_file():  # and relpath not in index
-            print('Untracked:', relpath)
-            untracked += 1
-
-        # if dir is not in tree_items_list
-        elif file.name not in (
-                i[2] for i in
-                filter(lambda x: x[0] == '40000', tree_items_list)
-        ):
-            # untrack must be setted only if any children is not ignored
-            result = handle_untracked_dir(
-                git_dir, file.path, fixed, ignored
-            )
-            if result:
-                untracked += result
+            elif file.is_file():  # and relpath not in index
                 print('Untracked:', relpath)
+                untracked += 1
 
-        else:
-            found_in_tree += 1
+            # if dir isn't in tree_items_list
+            elif file.name not in (
+                    i[2] for i in
+                    filter(lambda x: x[0] == '40000', tree_items_list)
+            ):
+                # untrack must be setted only if any children is not ignored
+                result = self.handle_untracked_dir(file.path)
+                if result:
+                    untracked += result
+                    print('Untracked:', relpath)
+
+            # is_dir and is in tree
+            else:
+                found_in_tree += 1
+
+                # filter entries with type == 40000
+                trees = filter(lambda x: x[0] == '40000', tree_items_list)
+                file_name_tuple = filter(lambda x: x[2] == file.name, trees)
+                item_tuple = tuple(file_name_tuple)
+                tree_hash = item_tuple[0][1]
+
+                unt, sta, mod, del_ = self.get_full_status(
+                    file.path,
+                    tree_hash
+                )
+                untracked += unt
+                staged += sta
+                modified += mod
+                deleted += del_
 
-            trees = filter(lambda x: x[0] == '40000', tree_items_list)
-            file_name_tuple = filter(lambda x: x[2] == file.name, trees)
-            item_tuple = tuple(file_name_tuple)
-            tree_hash = item_tuple[0][1]
-
-            unt, sta, mod, del_ = get_full_status(
-                git_dir,
-                branch,
-                fixed,
-                ignored,
-                index_tracked,
-                packs_list,
-                file.path,
-                tree_hash
-            )
-            untracked += unt
-            staged += sta
-            modified += mod
-            deleted += del_
-
-    # endfor
-    deleted += len(tree_items_list) - found_in_tree
-
-    return untracked, staged, modified, deleted
-
-
-def handle_untracked_dir(
-        git_dir: str, dir_name: str, fixed: list, ignored: list
-) -> int:
-    """
-    Handles when `get_full_status` finds untracked directory.
-    param `git_dir`: The directory where .git resides.
-    param `dir_name`: The path of the untracked directory.
-    param `fixed`: list of full paths in both '.gitignore' and 'exclude'.
-    param `ignored`: list of relative paths in both '.gitignore' and 'exclude'.
-    return: int: 1 if there was at least one not ignored file in directory.
-                 0 if there was none.
-    """
-    try:
-        with os.scandir(dir_name) as sub_dir:
-
-            untracked = 0
-            for sub_file in sub_dir:
-                if sub_file.is_dir():
-                    untracked += handle_untracked_dir(
-                        git_dir, sub_file.path, fixed, ignored
-                    )
-
-                if untracked:
-                    return 1
-
-                if sub_file.is_file():
-                    if any(fnmatch(sub_file.name, pat)
-                           for pat in ignored):
-                        continue
-
-                    sub_relpath = os.path.relpath(
-                        sub_file.path, git_dir
-                    ).replace('\\', '/', -1)
-
-                    if any(fnmatch(sub_relpath, pat)
-                           for pat in fixed):
-                        continue
-                    return 1
+        # endfor
+        deleted += len(tree_items_list) - found_in_tree
 
-            return 0
-    except PermissionError:
-        return 0
+        return untracked, staged, modified, deleted
 
+    def handle_untracked_dir(self, dir_path: str) -> int:
+        """
+        Handles when `get_full_status` finds untracked directory.
+        param `dir_name`: The path of the untracked directory.
+        return: int: 1 if there was at least one not ignored file in directory.
+                     0 if there was none.
+        """
+        try:
+            with os.scandir(dir_path) as sub_dir:
+
+                untracked = 0
+                for sub_file in sub_dir:
+                    if sub_file.is_dir():
+                        untracked += self.handle_untracked_dir(sub_file.path)
+
+                    if untracked:
+                        return 1
+
+                    if sub_file.is_file():
+                        if any(fnmatch(sub_file.name, pattern)
+                               for pattern in self.ignored):
+                            continue
+
+                        sub_relpath = os.path.relpath(
+                            sub_file.path, self.git_dir
+                        ).replace('\\', '/', -1)
+
+                        if any(fnmatch(sub_relpath, pattern)
+                               for pattern in self.fixed):
+                            continue
+                        return 1
 
-def get_tree_items(
-        git_dir: str, last_cmmt: str, packs_list: list
-) -> list | None:
-    """
-    Gets the last commit tree itens (type, hash and filename).
-    param `git_dir`: The directory where .git resides.
-    param `last_cmmt`: The hash of the last commit.
-    param `packs_list`: list of full paths of packfiles.
-    return: list | None: list of tuples with the type, hash and filenames,
-                None if tree is empty.
-    """
-
-    last_cmmt_obj = low.get_content_by_hash_loose(git_dir, last_cmmt)
-    if last_cmmt_obj is None:
-        last_cmmt_obj = medium.get_content_by_hash_packed(
-            last_cmmt, packs_list
-        )
+                return 0
+        except PermissionError:
+            return 0
 
-    if last_cmmt_obj is None:
-        print("Couldn't get last commit object. Fallback.")
-        raise FallbackError
-
-    tree_hash = low.get_tree_hash_from_commit(last_cmmt_obj)
-    print('Last commit tree hash:', tree_hash)
-
-    tree_obj = low.get_content_by_hash_loose(git_dir, tree_hash)
-    if tree_obj is None:
-        tree_obj = medium.get_content_by_hash_packed(tree_hash, packs_list)
-
-    if tree_obj is None:
-        print("Couldn't get last commit tree. Fallback.")
-        raise FallbackError
-
-    # there is a tree object but the git worktree is empty.
-    if not tree_obj:
-        return
-
-    return low.parse_tree_object(tree_obj)
-
-
-def get_tree_items_from_hash(
-        git_dir: str, tree_hash: str, packs_list: list
-) -> list:
-    """
-    Gets the tree itens searching for its hash.
-    param `git_dir`: The directory where .git resides.
-    param `tree_hash`: The hash of tree.
-    param `packs_list`: list of full paths of packfiles.
-    return: list: list of tuples with the type, hash and filenames.
-    """
-    from_pack = False
-    tree_obj = low.get_content_by_hash_loose(git_dir, tree_hash)
-    print('Searching loose', tree_hash)
-
-    if tree_obj is None:
-        from_pack = True
-        tree_obj = medium.get_content_by_hash_packed(tree_hash, packs_list)
-        print('Searching packed', tree_hash)
-
-    if tree_obj is None:
-        print('Not found. Fallback.')
-        raise FallbackError
+    def get_tree_items(self, last_cmmt: str) -> list | None:
+        """
+        Gets the last commit tree itens (type, hash and filename).
+        param `last_cmmt`: The hash of the last commit.
+        return: list | None: list of tuples with the type, hash and filenames,
+                    None if tree is empty.
+        """
+
+        last_cmmt_obj = self.get_content_by_hash_loose(last_cmmt)
+        if last_cmmt_obj is None:
+            last_cmmt_obj = self.get_content_by_hash_packed(last_cmmt)
+
+        if last_cmmt_obj is None:
+            print("Couldn't get last commit object. Fallback.")
+            raise FallbackError
+
+        tree_hash = self.get_tree_hash_from_commit(last_cmmt_obj)
+        print('Last commit tree hash:', tree_hash)
+
+        from_pack = False
+        tree_obj = self.get_content_by_hash_loose(tree_hash)
+        if tree_obj is None:
+            from_pack = True
+            tree_obj = self.get_content_by_hash_packed(tree_hash)
+
+        if tree_obj is None:
+            print("Couldn't get last commit tree. Fallback.")
+            raise FallbackError
+
+        # there is a tree object but the git worktree is empty.
+        if not tree_obj:
+            return
+
+        return self.parse_tree_object(tree_obj, from_pack)
+
+    def get_tree_items_from_hash(self, tree_hash: str) -> list:
+        """
+        Gets the tree itens searching for its hash.
+        param `tree_hash`: The hash of tree.
+        return: list: list of tuples with the type, hash and filenames.
+        """
+        from_pack = False
+        tree_obj = self.get_content_by_hash_loose(tree_hash)
+        print('Searching loose', tree_hash)
+
+        if tree_obj is None:
+            from_pack = True
+            tree_obj = self.get_content_by_hash_packed(tree_hash)
+            print('Searching packed', tree_hash)
+
+        if tree_obj is None:
+            print('Not found. Fallback.')
+            raise FallbackError
 
-    tree_items_list = low.parse_tree_object(tree_obj, from_pack)
-    print('Found:', *tree_items_list, sep='\n', end=n)
+        tree_items_list = self.parse_tree_object(tree_obj, from_pack)
+        print('Found:', *tree_items_list, sep='\n', end=n)
 
-    return tree_items_list
+        return tree_items_list
```

### Comparing `shellserver-0.0.8/shellserver/gitstatus/low.py` & `shellserver-0.0.9/shellserver/gitstatus/low.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module with functions considered to be of low level,
 that is, functions that doesn't call its siblings.
+Same idea for the methods of Low class.
 """
 
 import hashlib
 import os
 import subprocess
 import zlib
 
@@ -23,294 +24,282 @@
     parent = os.path.dirname(target_path)
     if parent == target_path:
         return
 
     return get_dot_git(parent)
 
 
-def get_branch_on_head(git_dir: str) -> str:
-    """
-    Parses 'HEAD' file to get the head branch.
-    param `git_dir`: The path of .git.
-    return: str: The name of the git branch.
-    """
-
-    head_path = os.path.join(git_dir, '.git/HEAD')
-
-    with open(head_path) as head:
-        content = head.read()
-
-    return content[content.rindex('/') + 1:].strip()
-
-
-def get_info_packs_content(git_dir: str) -> list[str]:
-    """
-    Checks the existence of a 'packs' file in git/objects
-    and return its content.
-    param `git_dir`: The path of .git.
-    return: list: Content of packs by line.
-    """
-
-    packs = os.path.join(git_dir, '.git/objects/info/packs')
-    if not os.path.exists(packs):
-        return []
-
-    with open(packs) as in_file:
-        content = in_file.readlines()[::-1]
-
-    counter = 0
-    while counter < len(content):
-        test = content[counter][2:].strip()
-        if not test:
-            del content[counter]
-            continue
-
-        content[counter] = test
-        counter += 1
-
-    return content
-
-
-def get_gitignore_content(git_dir: str) -> list[str]:
-    """
-    Checks the existence of a .gitignore in same level of .git
-    and return its content
-    param `git_dir`: The path of .git.
-    return: list: Content of .gitignore by line.
-    """
-
-    gitignore = os.path.join(git_dir, '.gitignore')
-    if not os.path.exists(gitignore):
-        return []
-
-    with open(gitignore) as in_file:
-        content = in_file.readlines()
-
-    counter = 0
-    while counter < len(content):
-        test = content[counter].strip()
-        if not test:
-            del content[counter]
-            continue
-
-        content[counter] = test
-        counter += 1
-
-    return content
-
-
-def get_last_commit_loose(git_dir: str, branch: str) -> str | None:
-    """
-    Gets the last commit's hash of a git repo.
-    param `git_dir`: The path of .git.
-    return: str | None: String of the last commit hash, None if there's no
-                        last commit.
-    """
-
-    head_path = os.path.join(git_dir, f'.git/refs/heads/{branch}')
-
-    if not os.path.exists(head_path):
-        return
-
-    with open(head_path) as file:
-        return file.read().strip()
-
-
-def get_info_refs_content(git_dir) -> list[str]:
-    """
-    Checks the existence of a 'refs' file in .git/info
-    and return its content
-    param `git_dir`: The path of .git.
-    return: list: Content of 'refs' by line.
-    """
-
-    refs = os.path.join(git_dir, '.git/info/refs')
-    if not os.path.exists(refs):
-        return []
-
-    with open(refs) as in_file:
-        content = in_file.readlines()
-
-    for ind in range(len(content)):
-        content[ind] = content[ind].strip()
-
-    return content
-
-
-def get_exclude_content(git_dir: str) -> list[str]:
-    """
-    Checks the existence of a 'exclude' file inside .git/info
-    and return its content.
-    param `git_dir`: The path of .git.
-    return: list: Content of exclude by line.
-    """
-    exclude = os.path.join(git_dir, '.git/info/exclude')
-    if not os.path.exists(exclude):
-        return []
-
-    with open(exclude) as in_file:
-        content = in_file.readlines()
-
-    counter = 0
-    while counter < len(content):
-        test = content[counter].strip()
-        if not test:
-            del content[counter]
-            continue
-
-        content[counter] = test
-        counter += 1
-
-    return content
-
-
-def get_hash_of_file(file_path: bytes | str, use_cr=False) -> str:
-    """
-    Get the SHA1 hash in the same way Git would do.
-    param `file_path`: str | bytes: The path to file.
-    param `use_cr`: bool: Use CRLF for new line?
-    """
-    with open(file_path, 'rb') as in_file:
-        content = in_file.read()
-
-    if not use_cr:
-        content = content.replace(b'\r\n', b'\n', -1)
-
-    size = len(content)
-    string = f"blob {size}\x00"
-    hash_ = hashlib.sha1(string.encode() + content).hexdigest()
-
-    return hash_
-
-
-def get_content_by_hash_loose(git_dir: str, hash_: str) -> bytes | None:
-    """
-    Get the content of a loose file by its hash.
-    param `git_dir`: The path of .git.
-    param `hash`: The hash gotten from `get_hash_of_file` for files in repo
-                  or in git files.
-    return: bytes | None: The content of file, None if it was not found.
-    """
-
-    path = os.path.join(git_dir, f'.git/objects/{hash_[:2]}/{hash_[2:]}')
-    if not os.path.exists(path):
-        return
-
-    with open(path, 'rb') as in_file:
-        content = in_file.read()
-
-    # cannot decode here
-    # in blob we can take bytes or str
-    # in tree, only bytes
-    return zlib.decompress(content)
-
-
-def get_tree_hash_from_commit(cmmt_obj: bytes) -> str:
-    """
-    Get the tree hash from an commit object.
-    param `cmmt_obj`: bytes: A git commit object.
-    return: str: The tree hash.
-    """
-
-    first_line = cmmt_obj.splitlines()[0].decode()
-    tree_hash = first_line[first_line.index('tree') + 5:].strip()
-
-    return tree_hash
-
-
-def get_status_string(status: tuple[int, int, int, int]) -> str | None:
-    """
-    Get the string version of given Git status
-    param `status`: tuple: untracked, staged, modified and deleted sums.
-    return: str | None: String of status, None if not any value is above 0.
-    """
-    if not any(status):
-        return
-
-    symbols = ('?', '+', 'm', 'x')
-
-    return ' '.join(
-        symb + str(stat)
-        for symb, stat in zip(symbols, status)
-        if stat
-    )
-
-
 def exists_head(git_dir: str) -> bool:
     """
     Checks if there are a 'HEAD' in git files.
-    param `git_dir`: The path of .git.
     return: bool: Is there a 'HEAD' in .git?
     """
 
     head = os.path.join(git_dir, '.git/HEAD')
     return os.path.exists(head)
 
 
-def parse_git_status(git_dir: str) -> str:
+def get_branch_on_head(git_dir: str) -> str:
     """
-    Parses `git status -s` returning tuple of untracked, staged,
-    modified and deleted sums.
-    param `git_dir`: The path of .git.
-    return: str: String of status.
+    Parses 'HEAD' file to get the head branch.
+    return: str: The name of the git branch.
     """
-    data, err = subprocess.Popen(
-        f'git -C {git_dir} status -s --porcelain',
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        creationflags=subprocess.CREATE_NO_WINDOW
-    ).communicate()
-
-    data = data.decode().splitlines()
-    data = [line[:2].strip() for line in data]
 
-    possibles = list(set(data))
+    head_path = os.path.join(git_dir, '.git/HEAD')
 
-    res = [mark + str(data.count(mark)) for mark in possibles]
+    with open(head_path) as head:
+        content = head.read()
 
-    return ' '.join(res)
+    return content[content.rindex('/') + 1:].strip()
 
 
-def parse_tree_object(
-        data: bytes, from_pack: bool = False
-) -> list[tuple[str, str, str]] | None:
-    """
-    Parses the content of a git tree object and returns a list
-    of its values
-    param `data`: The content decompressed of tree object
-    return: list | None: list of tuples containing the type, hash and
-            the filename in tree, None if tree is empty.
-    """
+class Low:
+    def get_info_packs_content(self) -> list:  # [str]:
+        """
+        Checks the existence of a 'packs' file in git/objects
+        and return its content.
+        return: list: Content of packs by line.
+        """
+
+        packs = os.path.join(self.git_dir, '.git/objects/info/packs')
+        if not os.path.exists(packs):
+            return []
+
+        with open(packs) as in_file:
+            content = in_file.readlines()[::-1]
+
+        counter = 0
+        while counter < len(content):
+            test = content[counter][2:].strip()
+            if not test:
+                del content[counter]
+                continue
+
+            content[counter] = test
+            counter += 1
+
+        return content
+
+    def get_gitignore_content(self) -> list:  # [str]:
+        """
+        Checks the existence of a .gitignore in same level of .git
+        and return its content
+        return: list: Content of .gitignore by line.
+        """
+
+        gitignore = os.path.join(self.git_dir, '.gitignore')
+        if not os.path.exists(gitignore):
+            return []
+
+        with open(gitignore) as in_file:
+            content = in_file.readlines()
+
+        counter = 0
+        while counter < len(content):
+            test = content[counter].strip()
+            if not test:
+                del content[counter]
+                continue
+
+            content[counter] = test
+            counter += 1
+
+        return content
+
+    def get_last_commit_loose(self) -> str | None:
+        """
+        Gets the last commit's hash of a git repo.
+        return: str | None: String of the last commit hash, None if there's no
+                            last commit.
+        """
+
+        head_path = os.path.join(
+            self.git_dir, f'.git/refs/heads/{self.branch}'
+        )
 
-    if not from_pack:
-        if not data[data.index(b'\x00') + 1:]:
+        if not os.path.exists(head_path):
             return
 
-        # first remove everything before first null byte
-        start = data.index(b'\x00') + 1
-    else:
-        start = 0
+        with open(head_path) as file:
+            return file.read().strip()
 
-    res = []
-
-    while True:
-        # cant split(b'\x00), hash might have it
-        # cant split(' '), filename might have it
-        stop = data.index(b'\x00', start)
+    def get_info_refs_content(self) -> list[str]:
+        """
+        Checks the existence of a 'refs' file in .git/info
+        and return its content
+        return: list: Content of 'refs' by line.
+        """
+
+        refs = os.path.join(self.git_dir, '.git/info/refs')
+        if not os.path.exists(refs):
+            return []
+
+        with open(refs) as in_file:
+            content = in_file.readlines()
+
+        for ind in range(len(content)):
+            content[ind] = content[ind].strip()
+
+        return content
+
+    def get_exclude_content(self) -> list:  # [str]:
+        """
+        Checks the existence of a 'exclude' file inside .git/info
+        and return its content.
+        return: list: Content of exclude by line.
+        """
+        exclude = os.path.join(self.git_dir, '.git/info/exclude')
+        if not os.path.exists(exclude):
+            return []
+
+        with open(exclude) as in_file:
+            content = in_file.readlines()
+
+        counter = 0
+        while counter < len(content):
+            test = content[counter].strip()
+            if not test:
+                del content[counter]
+                continue
+
+            content[counter] = test
+            counter += 1
+
+        return content
+
+    def get_hash_of_file(self, file_path: bytes | str, use_cr=False) -> str:
+        """
+        Get the SHA1 hash in the same way Git would do.
+        param `file_path`: str | bytes: The path to file.
+        param `use_cr`: bool: Use CRLF for new line?
+        """
+        with open(file_path, 'rb') as in_file:
+            content = in_file.read()
+
+        if not use_cr:
+            content = content.replace(b'\r\n', b'\n', -1)
+
+        size = len(content)
+        string = f"blob {size}\x00"
+        hash_ = hashlib.sha1(string.encode() + content).hexdigest()
+
+        return hash_
+
+    def get_content_by_hash_loose(self, hash_: str) -> bytes | None:
+        """
+        Get the content of a loose file by its hash.
+        param `hash`: The hash gotten from `get_hash_of_file` for files in repo
+                      or in git files.
+        return: bytes | None: The content of file, None if it was not found.
+        """
+
+        path = os.path.join(
+            self.git_dir, f'.git/objects/{hash_[:2]}/{hash_[2:]}'
+        )
+        if not os.path.exists(path):
+            return
 
-        piece = data[start: stop]
-        sep = piece.index(b' ')
+        with open(path, 'rb') as in_file:
+            content = in_file.read()
 
-        type_ = piece[:sep]
-        filename = piece[sep + 1:]
+        # cannot decode here
+        # in blob we can take bytes or str
+        # in tree, only bytes
+        return zlib.decompress(content)
+
+    def get_tree_hash_from_commit(self, cmmt_obj: bytes) -> str:
+        """
+        Get the tree hash from an commit object.
+        param `cmmt_obj`: bytes: A git commit object.
+        return: str: The tree hash.
+        """
+
+        first_line = cmmt_obj.splitlines()[0].decode()
+        tree_hash = first_line[first_line.index('tree') + 5:].strip()
+
+        return tree_hash
+
+    def get_status_string(
+            self, status: tuple[int, int, int, int]
+    ) -> str | None:
+        """
+        Get the string version of given Git status
+        param `status`: tuple: untracked, staged, modified and deleted sums.
+        return: str | None: String of status, None if not any value is above 0.
+        """
+        if not any(status):
+            return
 
-        start = stop + 21  # next start
+        symbols = ('?', '+', 'm', 'x')
 
-        hexa = data[stop + 1:start]
-        hexa = f'{int.from_bytes(hexa):x}'.zfill(40)
+        return ' '.join(
+            symb + str(stat)
+            for symb, stat in zip(symbols, status)
+            if stat
+        )
+
+    def parse_git_status(self) -> str:
+        """
+        Parses `git status -s` returning tuple of untracked, staged,
+        modified and deleted sums.
+        return: str: String of status.
+        """
+        data, err = subprocess.Popen(
+            f'git -C {self.git_dir} status -s --porcelain',
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            creationflags=subprocess.CREATE_NO_WINDOW
+        ).communicate()
+
+        data = data.decode().splitlines()
+        data = [line[:2].strip() for line in data]
+
+        possibles = list(set(data))
+
+        res = [mark + str(data.count(mark)) for mark in possibles]
+
+        return ' '.join(res)
+
+    def parse_tree_object(
+            self, data: bytes, from_pack: bool = False
+    ) -> list:  # [tuple[str, str, str]] | None:
+        """
+        Parses the content of a git tree object and returns a list
+        of its values
+        param `data`: The content decompressed of tree object
+        return: list | None: list of tuples containing the type, hash and
+                the filename in tree, None if tree is empty.
+        """
+
+        if not from_pack:
+            if not data[data.index(b'\x00') + 1:]:
+                return
+
+            # first remove everything before first null byte
+            start = data.index(b'\x00') + 1
+        else:
+            start = 0
+
+        res = []
+
+        while True:
+            # cant split(b'\x00), hash might have it
+            # cant split(' '), filename might have it
+            stop = data.index(b'\x00', start)
+
+            piece = data[start: stop]
+            sep = piece.index(b' ')
+
+            type_ = piece[:sep]
+            filename = piece[sep + 1:]
+
+            start = stop + 21  # next start
+
+            hexa = data[stop + 1:start]
+            hexa = f'{int.from_bytes(hexa):x}'.zfill(40)
 
-        res.append((type_.decode(), hexa, filename.decode()))
+            res.append((type_.decode(), hexa, filename.decode()))
 
-        if not data[start + 1:]:
-            break
+            if not data[start + 1:]:
+                break
 
-    return res
+        return res
```

### Comparing `shellserver-0.0.8/shellserver/gitstatus/medium.py` & `shellserver-0.0.9/shellserver/gitstatus/medium.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,173 +5,168 @@
 
 from . import low
 from . import packs
 
 os = low.os
 
 
-def get_packs(git_dir) -> list[str]:
-    """
-    Get the path of packfiles.
-    param `git_dir`: The directory in which .git resides.
-    return: list: The paths of packfiles.
-    """
-    # info/packs is not needed
-    pack_def_path = '.git/objects/pack'
-
-    packs_list = low.get_info_packs_content(git_dir)
-    if not packs_list:
-        packs = os.path.join(git_dir, pack_def_path)
-        if not os.path.exists(packs):
-            return []
-        packs_list = os.scandir(packs)
-        return [i.path for i in packs_list if i.name.endswith('.pack')]
+class Medium(low.Low, packs.Packs):
+    def set_packs(self) -> None:
+        """
+        Sets the `packs_list` attribute.
+        return: None.
+        """
+        # info/packs is not needed
+        pack_def_path = '.git/objects/pack'
+
+        packs_list = self.get_info_packs_content()
+        if packs_list:
+            self.packs_list = [
+                os.path.join(
+                    self.git_dir, pack_def_path, i
+                ) for i in packs_list
+            ]
+            return
 
-    packs_list = [
-        os.path.join(
-            git_dir, pack_def_path, i
-        ) for i in packs_list
-    ]
-
-    return packs_list
-
-
-def get_content_by_hash_packed(hash_: str, packs_list: list) -> bytes | None:
-    """
-    Get the content of an object by its hash in any packfiles present.
-    param `hash_`: The hash to be searched in packfiles.
-    return: bytes | None: The content of object, None if it was not Found.
-    """
-    content = None
-
-    for pack in packs_list:
-        idx = packs.get_idx_of_pack(pack)
-        offset = packs.search_idx(idx, hash_, rt_offset=True)
-        if offset is None:
-            continue
-        content = packs.get_content_by_offset(pack, offset)
-        if content:
-            break
-
-    return content
-
-
-def get_last_commit_packed(git_dir: str, branch: str) -> str | None:
-    """
-    Gets the last commit's hash of a git repo by a packed perspective.
-    param `git_dir`: The path of .git.
-    return: str | None: String of the last commit hash, None if there's no
-                        last commit packed.
-    """
-    info_refs = low.get_info_refs_content(git_dir)
-    last_commt_hash = None
-
-    for line in info_refs:
-        a, b = line.strip().split()
-        if b == f'refs/heads/{branch}':
-            last_commt_hash = a
-            break
-
-    return last_commt_hash
-
-
-def get_last_commit_hash(git_dir: str, branch: str) -> str | None:
-    """
-    Gets the last commit's hash of a git repo.
-    param `git_dir`: The path of .git.
-    return: str | None: String of the last commit hash, None if there's no
-                        last commit.
-    """
-    last_cmmt = low.get_last_commit_loose(git_dir, branch)
-
-    if last_cmmt is None:
-        last_cmmt = get_last_commit_packed(git_dir, branch)
-
-    return last_cmmt
-
-
-def get_index_tracked(git_dir: str) -> list[str] | None:
-    """
-    Modified and simpler version of gin.
-    https://github.com/sbp/gin
-    param `git_dir`: The path of .git.
-    return: list[str] | None: List containing the paths of tracked files,
-                              None if index file is unsuported.
-    """
-    index_path = os.path.join(git_dir, '.git/index')
-    if not os.path.exists(index_path):
-        return []
-
-    with open(index_path, 'rb') as f:
-
-        def readStrUntil(delim):
-            ret = []
-            while True:
-                b = f.read(1)
-                if b == '' or b == delim:
-                    return b"".join(ret).decode("utf-8", "replace")
-
-                ret.append(b)
-
-        constant = f.read(4)
-        version = int.from_bytes(f.read(4))
-        if constant != b'DIRC' or version not in (2, 3):
+        packs = os.path.join(self.git_dir, pack_def_path)
+        if not os.path.exists(packs):
+            self.packs_list = []
             return
 
-        entries = int.from_bytes(f.read(4))
-        res = []
+        packs_list = os.scandir(packs)
+        self.packs_list = [
+            i.path for i in packs_list if i.name.endswith('.pack')
+        ]
+
+    def set_index_tracked(self) -> None:
+        """
+        Sets `index_tracked` attribute.
+        Modified and simpler version of gin.
+        https://github.com/sbp/gin
+        return: None.
+        """
+        index_path = os.path.join(self.git_dir, '.git/index')
+        if not os.path.exists(index_path):
+            self.index_tracked = []
+            return
 
-        for entry in range(entries):
-            f.read(60)
+        with open(index_path, 'rb') as f:
 
-            flags = int.from_bytes(f.read(2))
-            namelen = flags & 0xfff
-            extended = flags & (0b0100_0000 << 8)
-
-            entrylen = 62
-
-            if extended:
-                f.read(2)
-                entrylen += 2
-
-            if namelen < 0xfff:
-                name = f.read(namelen).decode("utf-8", "replace")
-                entrylen += namelen
-            else:
-                name = readStrUntil('\x00')
-                entrylen += 1
-
-            res.append(name)
-
-            padlen = (8 - (entrylen % 8)) or 8
-            f.read(padlen)
-
-    return res
-
-
-def get_split_ignored(git_dir: str) -> tuple[list[str], list[str]]:
-    """
-    Gets the content of both 'exclude' and '.gitignore' files,
-    splits the content by patterns of full paths and relative paths.
-    param `git_dir`: The path of .git.
-    return: tuple[list[str], list[str]]: tuple of full path patterns and
-                relative path patterns.
-    """
-    raw_ignored = low.get_exclude_content(git_dir)
-    raw_ignored += low.get_gitignore_content(git_dir)
-
-    # raw_ignored will become the the 'fixed', return[0]
-    every_time = []
-    counter = 0
-    while counter < len(raw_ignored):
-        if raw_ignored[counter].strip().startswith('#'):
-            del raw_ignored[counter]
-            continue
-
-        if '/' not in raw_ignored[counter]:
-            every_time.append(raw_ignored[counter])
-            del raw_ignored[counter]
-            continue
+            def readStrUntil(delim):
+                ret = []
+                while True:
+                    b = f.read(1)
+                    if b == '' or b == delim:
+                        return b"".join(ret).decode("utf-8", "replace")
+
+                    ret.append(b)
+
+            constant = f.read(4)
+            version = int.from_bytes(f.read(4))
+            if constant != b'DIRC' or version not in (2, 3):
+                self.index_tracked = None
+
+            entries = int.from_bytes(f.read(4))
+            res = []
+
+            for entry in range(entries):
+                f.read(60)
+
+                flags = int.from_bytes(f.read(2))
+                namelen = flags & 0xfff
+                extended = flags & (0b0100_0000 << 8)
+
+                entrylen = 62
+
+                if extended:
+                    f.read(2)
+                    entrylen += 2
+
+                if namelen < 0xfff:
+                    name = f.read(namelen).decode("utf-8", "replace")
+                    entrylen += namelen
+                else:
+                    name = readStrUntil('\x00')
+                    entrylen += 1
+
+                res.append(name)
+
+                padlen = (8 - (entrylen % 8)) or 8
+                f.read(padlen)
+
+        self.index_tracked = res
+
+    def set_split_ignored(self) -> None:
+        """
+        Sets `fixed` and `ignored` attributes.
+        `fixed` represents the patterns to ignore as full paths.
+        `ignored` represents the patterns to ignore as relative paths.
+        return: None.
+        """
+        raw_ignored = self.get_exclude_content()
+        raw_ignored += self.get_gitignore_content()
+
+        # raw_ignored will become the the 'fixed', return[0]
+        every_time = []
+        counter = 0
+        while counter < len(raw_ignored):
+            if raw_ignored[counter].strip().startswith('#'):
+                del raw_ignored[counter]
+                continue
+
+            if '/' not in raw_ignored[counter]:
+                every_time.append(raw_ignored[counter])
+                del raw_ignored[counter]
+                continue
+
+            counter += 1
+
+        self.fixed, self.ignored = raw_ignored, every_time
+
+    def get_content_by_hash_packed(self, hash_: str) -> bytes | None:
+        """
+        Gets the content of an object by its hash in any packfiles present.
+        param `hash_`: The hash to be searched in packfiles.
+        return: bytes | None: The content of object, None if it was not Found.
+        """
+        content = None
+
+        for pack in self.packs_list:
+            idx = self.get_idx_of_pack(pack)
+            offset = self.search_idx(idx, hash_, rt_offset=True)
+            if offset is None:
+                continue
+            content = self.get_content_by_offset(pack, offset)
+            if content:
+                break
+
+        return content
+
+    def get_last_commit_packed(self) -> str | None:
+        """
+        Gets the last commit's hash of a git repo by a packed perspective.
+        return: str | None: String of the last commit hash, None if there's no
+                            last commit packed.
+        """
+        info_refs = self.get_info_refs_content()
+        last_commt_hash = None
+
+        for line in info_refs:
+            a, b = line.strip().split()
+            if b == f'refs/heads/{self.branch}':
+                last_commt_hash = a
+                break
+
+        return last_commt_hash
+
+    def get_last_commit_hash(self) -> str | None:
+        """
+        Gets the last commit's hash of a git repo.
+        return: str | None: String of the last commit hash, None if there's no
+                            last commit.
+        """
+        last_cmmt = self.get_last_commit_loose()
 
-        counter += 1
+        if last_cmmt is None:
+            last_cmmt = self.get_last_commit_packed()
 
-    return raw_ignored, every_time
+        return last_cmmt
```

### Comparing `shellserver-0.0.8/shellserver/gitstatus/packs.py` & `shellserver-0.0.9/shellserver/gitstatus/packs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,107 @@
 """
 Low level operations on packfiles.
 """
 
 import zlib
 
 
-def search_idx(
-        idx_path: str,
-        hash_: str,
-        rt_offset=False
-) -> bool | int | None:
-    """
-    Searches given `idx_path` for `hash_`.
-    param `idx_path`: The path of the pack index file.
-    param `rt_offset`: Should this function return the offset of given file
-                       if it's found?
-    return: bool | int | None:
-        If `rt_offset` is set to False, returns boolean value
-        representing the presence of hash in the index.
-        If `rt_offset` is set to True, returns the integer
-        representing the offset of hash in the pack file.
-        If `rt_offset` is set to True, but hash wasn't found in
-        the index file, returns None.
-    """
-
-    layer1_idx = int(hash_[:2], 16)
-    found = False
-
-    with open(idx_path, 'rb') as file:
-        file.seek(8 + 4 * layer1_idx)
-        files_before = int.from_bytes(file.read(4))
-        file.seek(1028)
-        total_files = int.from_bytes(file.read(4))
-
-        file.seek(
-            1032  # end of fanout_layer1
-            + 20 * (files_before - 1)  # each will have 20 bytes
-        )
-
-        while not found:
-            file_hash_bytes = file.read(20)
-            file_hash = hex(int.from_bytes(file_hash_bytes))[2:].zfill(40)
-
-            if hash_ == file_hash:
-                found = True
-
-            elif int(file_hash[:2], 16) > layer1_idx:
-                break
+class Packs:
+    def search_idx(
+            self,
+            idx_path: str,
+            hash_: str,
+            rt_offset=False
+    ) -> bool | int | None:
+        """
+        Searches given `idx_path` for `hash_`.
+        param `idx_path`: The path of the pack index file.
+        param `rt_offset`: Should this function return the offset of given file
+                           if it's found?
+        return: bool | int | None:
+            If `rt_offset` is set to False, returns boolean value
+            representing the presence of hash in the index.
+            If `rt_offset` is set to True, returns the integer
+            representing the offset of hash in the pack file.
+            If `rt_offset` is set to True, but hash wasn't found in
+            the index file, returns None.
+        """
+
+        layer1_idx = int(hash_[:2], 16) - 1
+        found = False
+
+        with open(idx_path, 'rb') as file:
+            file.seek(8 + 4 * layer1_idx)
+            files_before = int.from_bytes(file.read(4))
+            file.seek(1028)
+            total_files = int.from_bytes(file.read(4))
 
-            elif file.tell() >= 1032 + 20 * total_files:
-                break
-
-        if not rt_offset:
-            return found
-
-        if found:
             file.seek(
-                1032
-                + 20 * total_files  # jump layer2
-                + 4 * total_files  # jump layer3
-                + 4 * (files_before - 1)
+                1032  # end of fanout_layer1
+                + 20 * files_before  # each will have 20 bytes
             )
-            return int.from_bytes(file.read(4))
-
-
-def get_content_by_offset(pack_path: str, offset: int) -> bytes | None:
-    """
-    Gets the content of object in given `pack_path` by its `offset`.
-    param `pack_path`: The path to the pack file.
-    param `offset`: The offset of the object.
-    return: bytes | None: The content of the object, None it is a delta object
-    """
 
-    with open(pack_path, 'rb') as file:
-        file.seek(offset)
+            while not found:
+                file_hash_bytes = file.read(20)
+                file_hash = hex(int.from_bytes(file_hash_bytes))[2:].zfill(40)
+
+                if hash_ == file_hash:
+                    found = True
+                    break
+
+                elif int(file_hash[:2], 16) > layer1_idx + 1:
+                    break
+
+                elif file.tell() >= 1032 + 20 * total_files:
+                    break
+
+                files_before += 1
+
+            if not rt_offset:
+                return found
+
+            if found:
+                file.seek(
+                    1032
+                    + 20 * total_files  # jump layer2
+                    + 4 * total_files  # jump layer3
+                    + 4 * files_before
+                )
+                return int.from_bytes(file.read(4))
+
+    def get_content_by_offset(
+            self, pack_path: str, offset: int
+    ) -> bytes | None:
+        """
+        Gets the content of object in given `pack_path` by its `offset`.
+        param `pack_path`: The path to the pack file.
+        param `offset`: The offset of the object.
+        return: bytes | None: The content of the object,
+                              None it is a delta object
+        """
 
-        int_ = int.from_bytes(file.read(1))
-        binary = f'{int_:b}'.zfill(8)
-        type_ = binary[1:4]
+        with open(pack_path, 'rb') as file:
+            file.seek(offset)
 
-        if type_ == '110':  # delta type
-            return
-
-        msb = binary.startswith('1')
-        # size = binary[4:]
-
-        while msb:
             int_ = int.from_bytes(file.read(1))
             binary = f'{int_:b}'.zfill(8)
-            # size += binary[1:]
-            msb = binary.startswith('1')
+            type_ = binary[1:4]
 
-        return zlib.decompress(file.read())
+            if type_ == '110':  # delta type
+                return
 
+            msb = binary.startswith('1')
+            # size = binary[4:]
 
-def get_idx_of_pack(pack: str) -> str:
-    """
-    return pack.removesuffix('pack') + 'idx'
-    """
-    return pack.removesuffix('pack') + 'idx'
+            while msb:
+                int_ = int.from_bytes(file.read(1))
+                binary = f'{int_:b}'.zfill(8)
+                # size += binary[1:]
+                msb = binary.startswith('1')
+
+            return zlib.decompress(file.read())
+
+    def get_idx_of_pack(self, pack: str) -> str:
+        """
+        return pack.removesuffix('pack') + 'idx'
+        """
+        return pack.removesuffix('pack') + 'idx'
```

### Comparing `shellserver-0.0.8/shellserver/gitstatus/tests.py` & `shellserver-0.0.9/shellserver/gitstatus/tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import subprocess
 import tempfile
 import unittest
 
 from .__init__ import gitstatus
 from . import low
 from . import medium
-from . import packs
 from . import high
 
 
 def popen(cmd: str) -> bytes:
     out, err = subprocess.Popen(
         cmd,
         stdout=subprocess.PIPE,
@@ -37,15 +36,15 @@
 class TestGitstatusLowEmpty(unittest.TestCase):
     """
     Tests for low module with just initialized git repo.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_empty_get_dot_git(self):
@@ -58,115 +57,141 @@
         self.assertEqual(branch, 'master')
 
         popen(f'git -C {self.temp} branch -M main')
         branch = low.get_branch_on_head(self.temp)
         self.assertEqual(branch, 'main')
 
     def test_empty_get_info_packs_content(self):
-        tested = low.get_info_packs_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_info_packs_content()
         self.assertEqual(tested, [])
 
     def test_empty_get_gitignore_content(self):
-        tested = low.get_gitignore_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_gitignore_content()
         self.assertEqual(tested, [])
 
         text = 'some text'
         with open(self.temp + '/.gitignore', 'w') as f:
             print(text, file=f)
-        tested = low.get_gitignore_content(self.temp)
+        tested = obj.get_gitignore_content()
         self.assertEqual(tested, [text])
 
     def test_empty_get_last_commit_loose(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = low.get_last_commit_loose(self.temp, branch)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_last_commit_loose()
         self.assertIsNone(tested)
 
     def test_empty_get_info_refs_content(self):
-        tested = low.get_info_refs_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_info_refs_content()
         self.assertEqual(tested, [])
 
     def test_empty_get_exclude_content(self):
-        tested = low.get_exclude_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_exclude_content()
         exc = os.path.join(self.temp, '.git/info/exclude')
         with open(exc) as f:
             local = f.readlines()
         local = [i.strip() for i in local if i.strip()]
         self.assertEqual(tested, local)
 
     # commet the ones not really testing
     # so we don't fake the number of ran tests
     '''
     def test_empty_get_hash_of_file(self):
         # can't test for empty repo
     '''
 
     def test_empty_get_content_by_hash_loose(self):
-        tested = low.get_content_by_hash_loose(self.temp, 'any')
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.get_content_by_hash_loose('any')
         self.assertIsNone(tested)
 
     def test_empty_get_tree_hash_from_commit(self):
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
         # supose and cmmt obj
         tree_hash = b'0123456789abcdf'
         cmmt_obj = b'may be more things tree ' + tree_hash + b'\n'
-        tested = low.get_tree_hash_from_commit(cmmt_obj)
+        tested = obj.get_tree_hash_from_commit(cmmt_obj)
         self.assertEqual(tested, tree_hash.decode())
 
     def test_empty_get_status_string(self):
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
         sts = (0, 0, 0, 0)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertIsNone(tested)
 
         sts = (1, 0, 0, 0)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, '?1')
 
         sts = (0, 1, 0, 0)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, '+1')
 
         sts = (0, 0, 1, 0)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, 'm1')
 
         sts = (0, 0, 0, 1)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, 'x1')
 
         sts = (1, 1, 1, 1)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, '?1 +1 m1 x1')
 
         sts = (1, 0, 1, 0)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, '?1 m1')
 
         sts = (0, 1, 0, 1)
-        tested = low.get_status_string(sts)
+        tested = obj.get_status_string(sts)
         self.assertEqual(tested, '+1 x1')
 
     def test_empty_exists_head(self):
         tested = low.exists_head(self.temp)
         path = os.path.join(self.temp, '.git/HEAD')
         local = os.path.exists(path)
         self.assertEqual(tested, local)
 
     def test_empty_parse_git_status(self):
-        tested = low.parse_git_status(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'main'
+        tested = obj.parse_git_status()
         # test_get_gitignore_content created .gitignore
         self.assertEqual(tested, '??1')
 
 
 class TestGitstatusLowLoose(unittest.TestCase):
     """
     Tests for low module with git repo with files.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         with open(f'{cls.temp}/file.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\n')
         with open(f'{cls.temp}/file_cr.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\r\n')
         popen(f'git -C {cls.temp} add .')
         popen(f'git -C {cls.temp} commit -m "some"')
@@ -186,52 +211,63 @@
         # no need to retest
 
     def test_loose_get_gitignore_content(self):
         # no need to retest
     '''
 
     def test_loose_get_last_commit_loose(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = low.get_last_commit_loose(self.temp, branch)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_last_commit_loose()
         master = os.path.join(self.temp, '.git/refs/heads/master')
         with open(master) as file:
             local = file.read()
         self.assertEqual(tested, local.strip())
 
     def test_loose_get_info_refs_content(self):
         # should only exists if there are packed files
-        tested = low.get_info_refs_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_info_refs_content()
         self.assertEqual(tested, [])
 
     '''
     def test_loose_get_exclude_content(self):
         # no need to retest
 
     def test_loose_build_filtered_patterns(self):
         # no need to retest
     '''
 
     def test_loose_get_hash_of_file(self):
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
         git_hash = popen(
             f'git -C {self.temp} hash-object file.txt'
         ).strip().decode()
         self.assertEqual(file_hash, git_hash)
 
-        file_hash = low.get_hash_of_file(
+        file_hash = obj.get_hash_of_file(
             self.temp + '/file_cr.txt'
         )
         git_hash = popen(
             f'git -C {self.temp} hash-object file_cr.txt'
         ).strip().decode()
         self.assertEqual(file_hash, git_hash)
 
     def test_loose_get_content_by_hash_loose(self):
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
-        tested = low.get_content_by_hash_loose(self.temp, file_hash)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
+        tested = obj.get_content_by_hash_loose(file_hash)
         local = popen(
             f'git -C {self.temp} cat-file -p {file_hash}'
         ).strip()
         self.assertIn(local, tested)
 
     '''
     def test_loose_get_tree_hash_from_commit(self):
@@ -241,26 +277,29 @@
         # no need to retest
 
     def test_loose_exists_head(self):
         # no need to retest
     '''
 
     def test_loose_parse_git_status(self):
-        tested = low.parse_git_status(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.parse_git_status()
         self.assertEqual(tested, '')
 
 
 class TestGitstatusLowPacked(unittest.TestCase):
     """
     Tests for low module with git repo with packed files.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         with open(f'{cls.temp}/file.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\n')
         with open(f'{cls.temp}/file_cr.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\r\n')
         popen(f'git -C {cls.temp} add .')
         popen(f'git -C {cls.temp} commit -m "some"')
@@ -281,20 +320,25 @@
         # no need to retest
 
     def test_packed_get_gitignore_content(self):
         # no need to retest
     '''
 
     def test_packed_get_last_commit_loose(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = low.get_last_commit_loose(self.temp, branch)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_last_commit_loose()
         self.assertIsNone(tested)
 
     def test_packed_get_info_refs_content(self):
-        tested = low.get_info_refs_content(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_info_refs_content()
         refs = os.path.join(self.temp, '.git/info/refs')
         with open(refs) as file:
             local = file.readlines()
         local = [i.strip() for i in local if i.strip()]
         self.assertEqual(tested, local)
 
     '''
@@ -302,76 +346,92 @@
         # no need to retest
 
     def test_packed_get_hash_of_file(self):
         # no need to retest
     '''
 
     def test_packed_get_content_by_hash_loose(self):
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
-        tested = low.get_content_by_hash_loose(self.temp, file_hash)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
+        tested = obj.get_content_by_hash_loose(file_hash)
         self.assertIsNone(tested)
 
     '''
     def test_packed_get_tree_hash_from_commit(self):
         # no need to retest
 
     def test_packed_get_status_string(self):
         # no need to retest
 
     def test_packed_exists_head(self):
         # no need to retest
     '''
 
     def test_packed_parse_git_status(self):
-        tested = low.parse_git_status(self.temp)
+        obj = low.Low()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.parse_git_status()
         self.assertEqual(tested, '')
 
 
 class TestGitstatusMediumEmpty(unittest.TestCase):
     """
     Tests for medium module with just initialized git repo.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_empty_get_packs(self):
-        tested = medium.get_packs(self.temp)
-        self.assertEqual(tested, [])
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
+        self.assertEqual(obj.packs_list, [])
 
     def test_empty_get_content_by_hash_packed(self):
-        packs_list = medium.get_packs(self.temp)
-        tested = medium.get_content_by_hash_packed('anyabcdf01234', packs_list)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
+        tested = obj.get_content_by_hash_packed('anyabcdf01234')
         self.assertIsNone(tested)
 
     def test_empty_get_last_commit_packed(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = medium.get_last_commit_packed(self.temp, branch)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_last_commit_packed()
         self.assertIsNone(tested)
 
     def test_empty_get_last_commit(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = medium.get_last_commit_hash(self.temp, branch)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_last_commit_hash()
         self.assertIsNone(tested)
 
 
 class TestGitstatusMediumLoose(unittest.TestCase):
     """
     Tests for medium module with git repo with files.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests_')
         popen(f'git init {cls.temp}')
         with open(f'{cls.temp}/file.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\n')
         with open(f'{cls.temp}/file_cr.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\r\n')
         popen(f'git -C {cls.temp} add .')
         popen(f'git -C {cls.temp} commit -m "some"')
@@ -388,31 +448,38 @@
         # no need to retest
 
     def test_loose_get_last_commit_packed(self):
         # no need to retest
     """
 
     def test_loose_get_last_commit(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = medium.get_last_commit_hash(self.temp, branch)
-        low_tested = low.get_last_commit_loose(self.temp, branch)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        tested = obj.get_last_commit_hash()
+        low_tested = obj.get_last_commit_loose()
         self.assertEqual(tested, low_tested)
 
         master = os.path.join(self.temp, '.git/refs/heads/master')
         with open(master) as file:
             local = file.read()
         self.assertEqual(tested, local.strip())
 
     def test_loose_get_index_tracked(self):
         ni(self.temp, 'file')
         ni(self.temp, 'other')
         ni(self.temp, 'some')
         ni(self.temp, 'dir/file')
         popen(f'git -C {self.temp} add .')
-        tested = medium.get_index_tracked(self.temp)
+
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_index_tracked()
+        tested = obj.index_tracked
 
         self.assertGreaterEqual(len(tested), 3)
         self.assertIn('file', tested)
         self.assertIn('other', tested)
         self.assertIn('some', tested)
         self.assertIn('dir/file', tested)
 
@@ -423,107 +490,125 @@
 class TestGitstatusMediumPacked(unittest.TestCase):
     """
     Tests for medium module with git repo with packed files.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         with open(f'{cls.temp}/file.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\n')
         with open(f'{cls.temp}/file_cr.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\r\n')
         popen(f'git -C {cls.temp} add .')
         popen(f'git -C {cls.temp} commit -m "some"')
         popen(f'git -C {cls.temp} gc')
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_packed_get_packs(self):
-        packs = os.path.join(self.temp, '.git/objects/pack')
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
 
+        packs = os.path.join(self.temp, '.git/objects/pack')
         local = [packs + '\\' + i
                  for i in os.listdir(packs)
                  if i.endswith('pack')]
-        tested = medium.get_packs(self.temp)
+        tested = obj.packs_list
         self.assertEqual(tested, local)
 
     def test_packed_get_content_by_hash_packed(self):
-        packs_list = medium.get_packs(self.temp)
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
-        tested = medium.get_content_by_hash_packed(file_hash, packs_list)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
+
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
+        tested = obj.get_content_by_hash_packed(file_hash)
         local = popen(f'git -C {self.temp} cat-file -p {file_hash}')
         self.assertIn(local, tested)
 
     def test_packed_get_last_commit_packed(self):
         # I can't test this with a git background
-        branch = low.get_branch_on_head(self.temp)
-        tested = medium.get_last_commit_packed(self.temp, branch)
-        refs = low.get_info_refs_content(self.temp)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
+
+        tested = obj.get_last_commit_packed()
+        refs = obj.get_info_refs_content()
         self.assertEqual(len(tested), 40)
         self.assertTrue(int(tested, 16))
         self.assertEqual(tested, tested.strip())
         self.assertIn(tested, refs[0])
 
     def test_packed_get_last_commit(self):
-        branch = low.get_branch_on_head(self.temp)
-        tested = medium.get_last_commit_hash(self.temp, branch)
-        other_tested = medium.get_last_commit_packed(self.temp, branch)
+        obj = medium.Medium()
+        obj.git_dir = self.temp
+        obj.branch = 'master'
+        obj.set_packs()
+
+        tested = obj.get_last_commit_hash()
+        other_tested = obj.get_last_commit_packed()
         self.assertEqual(tested, other_tested)
 
 
 class TestGitstatusPacksPacked(unittest.TestCase):
     """
     Tests for packs module with git repo with packed files.
     """
     # makes no sense testing for other cases
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         with open(f'{cls.temp}/file.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\n')
         with open(f'{cls.temp}/file_cr.txt', 'wb') as file:
             file.write(get_random_string().encode() + b'\r\n')
         popen(f'git -C {cls.temp} add .')
         popen(f'git -C {cls.temp} commit -m "some"')
         popen(f'git -C {cls.temp} gc')
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_search_idx(self):
-        idx_path = packs.get_idx_of_pack(
-            medium.get_packs(self.temp)[0]
+        obj = high.High(self.temp, 'master')
+        idx_path = obj.get_idx_of_pack(
+            obj.packs_list[0]
         )
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
-        filecr_hash = low.get_hash_of_file(self.temp + '/file_cr.txt')
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
+        filecr_hash = obj.get_hash_of_file(self.temp + '/file_cr.txt')
 
-        tested = packs.search_idx(idx_path, file_hash)
+        tested = obj.search_idx(idx_path, file_hash)
         self.assertTrue(tested)
-        tested = packs.search_idx(idx_path, filecr_hash)
+        tested = obj.search_idx(idx_path, filecr_hash)
         self.assertTrue(tested)
 
     def test_get_content_by_offset(self):
-        pack = medium.get_packs(self.temp)[0]
-        idx_path = packs.get_idx_of_pack(pack)
+        obj = high.High(self.temp, 'master')
+        pack = obj.packs_list[0]
+        idx_path = obj.get_idx_of_pack(pack)
 
-        file_hash = low.get_hash_of_file(self.temp + '/file.txt')
-        filecr_hash = low.get_hash_of_file(self.temp + '/file_cr.txt')
+        file_hash = obj.get_hash_of_file(self.temp + '/file.txt')
+        filecr_hash = obj.get_hash_of_file(self.temp + '/file_cr.txt')
 
-        file_off = packs.search_idx(idx_path, file_hash, rt_offset=True)
-        filecr_off = packs.search_idx(idx_path, filecr_hash, rt_offset=True)
+        file_off = obj.search_idx(idx_path, file_hash, rt_offset=True)
+        filecr_off = obj.search_idx(idx_path, filecr_hash, rt_offset=True)
 
-        file_obj = packs.get_content_by_offset(pack, file_off)
-        filecr_obj = packs.get_content_by_offset(pack, filecr_off)
+        file_obj = obj.get_content_by_offset(pack, file_off)
+        filecr_obj = obj.get_content_by_offset(pack, filecr_off)
 
         local1 = popen(f'git -C {self.temp} cat-file -p {file_hash}')
         local2 = popen(f'git -C {self.temp} cat-file -p {filecr_hash}')
 
         self.assertEqual(local1, file_obj)
         self.assertEqual(local2, filecr_obj)
 
@@ -531,154 +616,170 @@
 class TestGitstatusHighStatus(unittest.TestCase):
     """
     Tests for high module with just initialized git repo.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         cls.branch = low.get_branch_on_head(cls.temp)
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_status(self):
-        self.assertIsNone(high.status(self.temp, self.branch))
+        obj = high.High(self.temp, 'master')
+        self.assertIsNone(obj.status())
 
         file_path = self.temp + '/file.txt'
         with open(file_path, 'w') as file:
             file.write(get_random_string())
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, '??1')
-        tested = high.status(self.temp, self.branch)
+        tested = obj.status()
         self.assertEqual(tested, '?1')
 
         popen(f'git -C {self.temp} add .')
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, 'A1')
-        tested = high.status(self.temp, self.branch)
+        obj = high.High(self.temp, 'master')
+        tested = obj.status()
         self.assertEqual(tested, '+1')
 
         popen(f'git -C {self.temp} commit -m "some"')
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, '')
-        self.assertIsNone(high.status(self.temp, self.branch))
+        obj = high.High(self.temp, 'master')
+        self.assertIsNone(obj.status())
 
         with open(file_path, 'a') as file:
             file.write(get_random_string())
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, 'M1')
-        tested = high.status(self.temp, self.branch)
+        obj = high.High(self.temp, 'master')
+        tested = obj.status()
         self.assertEqual(tested, 'm1')
 
         os.remove(file_path)
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, 'D1')
-        tested = high.status(self.temp, self.branch)
+        obj = high.High(self.temp, 'master')
+        tested = obj.status()
         self.assertEqual(tested, 'x1')
 
         popen(f'git -C {self.temp} add .')
         popen(f'git -C {self.temp} commit -m "other"')
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, '')
-        self.assertIsNone(high.status(self.temp, self.branch))
+        obj = high.High(self.temp, 'master')
+        self.assertIsNone(obj.status())
 
         popen(f'git -C {self.temp} gc')
-        git = low.parse_git_status(self.temp)
+        git = obj.parse_git_status()
         self.assertEqual(git, '')
-        self.assertIsNone(high.status(self.temp, self.branch))
+        obj = high.High(self.temp, 'master')
+        self.assertIsNone(obj.status())
 
 
 class TestGitstatusHighStatusIgnore(unittest.TestCase):
     """
     Tests for high module with just initialized git repo.
     """
 
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
         popen(f'git init {cls.temp}')
         cls.branch = low.get_branch_on_head(cls.temp)
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_status_ignore(self):
+        obj = high.High(self.temp, 'master')
         gitignore = self.temp + '/.gitignore'
         with open(gitignore, 'w') as ignore:
-            tested = high.status(self.temp, self.branch)
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
             ni(self.temp, 'ignored_dir/some')
             ignore.write('ignored_dir\n')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
             ni(self.temp, 'other/ignored.txt')
             ignore.write('other/ign\n')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?2')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??2')
 
             ignore.write('other/ign*\n')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
             ni(self.temp, 'some/ignored.txt')
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?2')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??2')
 
             ignore.write('some\n')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
             ni(self.temp, 'a/b/c/d')
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?2')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??2')
 
             ignore.write('a/**/d\n')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
             ni(self.temp, 'interrog.txt')
             ignore.write('inter???.txt')
             ignore.flush()
-            tested = high.status(self.temp, self.branch)
+            obj = high.High(self.temp, 'master')
+            tested = obj.status()
             self.assertEqual(tested, '?1')
-            git = low.parse_git_status(self.temp)
+            git = obj.parse_git_status()
             self.assertEqual(git, '??1')
 
 
 class TestGitstatusInit(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.temp = tempfile.mkdtemp(prefix='shellserver_tests-')
+        cls.temp = tempfile.mkdtemp(prefix='shellserver_test_')
 
     @classmethod
     def tearDownClass(cls):
         os.system(f'rmdir /s /q {cls.temp}')
 
     def test_gitstatus(self):
         tested = gitstatus(self.temp)
```

### Comparing `shellserver-0.0.8/shellserver/histdb.py` & `shellserver-0.0.9/shellserver/histdb.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/shellserver/server.py` & `shellserver-0.0.9/shellserver/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 # Quit program as soon as possible
 try:
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.bind(('localhost', PORT))
 except OSError:
     raise SystemExit
 
+import gc
 import os
 import subprocess
 import sys
 import threading
 import time
 
 from win_basic_tools.ls import Ls
 
 from . import histdb, theme
 from .gitstatus import gitstatus
 from .classes import DirCache, Dispatcher
 from .style import style
 
 
+gc.disable()
+
+
 def shell_manager(entry: str, addr) -> None:
     if entry.startswith('Init'):
         shell = entry.removeprefix('Init')
         dispatcher.register(addr, shell)
         clients.append(1)
         completions = ';'.join(item[2] for item in cache.dirs)
         dispatcher.send_through(sock, completions, addr)
@@ -67,15 +71,15 @@
     # Ls class can handle symlink
     ls = Ls(opt, path, to_cache=True)
     ls.echo(0)
 
     dispatcher.send_through(sock, ls.out.data, addr)
 
 
-def theme_manager(entry: str) -> None:
+def theme_manager(entry: str, addr) -> None:
     try:
         if entry in ('all', ''):
             theme.all()
         elif entry == 'terminal':
             theme.windows_terminal_change()
         elif entry == 'blue':
             theme.night_light_change()
@@ -117,36 +121,39 @@
     if branch is not None:
         git_flag = True
         brackets.append(f'Branch;{branch}')
         if status:
             brackets.append(f'Status;{status}')
 
     target_dir = curdir if curdir == link else link
+
     try:
-        with os.scandir(target_dir) as directory:
-            for file in directory:
-                if (py_not not in brackets
-                   and file.name.endswith(('.py', '.pyc', '.pyw', '.pyd'))):
-                    brackets.append(py_not)
-
-                for exe in exes_with_version:
-                    notation = f'{map_lang_name[exe]};{exes_with_version[exe]}'
-                    condition1 = notation not in brackets
-                    if condition1 and file.name.endswith(map_suffix[exe]):
-                        brackets.append(notation)
-
-                for exe in exes_to_search:  # those who don't have version
-                    notation = map_lang_name[exe]
-                    if (notation not in after_brackets
-                       and file.name.endswith(map_suffix[exe])):
-                        after_brackets.append(notation)
+        directory = os.scandir(target_dir)
     except PermissionError:
         brackets.append('Error;Permission')
+        directory = tuple()
     except OSError:
-        pass
+        directory = tuple()
+
+    for file in directory:
+        if (py_not not in brackets
+           and file.name.endswith(('.py', '.pyc', '.pyw', '.pyd'))):
+            brackets.append(py_not)
+
+        for exe in exes_with_version:
+            notation = f'{map_lang_name[exe]};{exes_with_version[exe]}'
+            condition1 = notation not in brackets
+            if condition1 and file.name.endswith(map_suffix[exe]):
+                brackets.append(notation)
+
+        for exe in exes_to_search:  # those who don't have version
+            notation = map_lang_name[exe]
+            if (notation not in after_brackets
+               and file.name.endswith(map_suffix[exe])):
+                after_brackets.append(notation)
 
     if home in curdir:
         curdir = '~' + curdir.removeprefix(home)
     if home in link:
         link = '~' + link.removeprefix(home)
 
     prompt = style(
@@ -158,53 +165,23 @@
 
 
 def mainloop():
     while 1:
         entry, addr = sock.recvfrom(4096)
         init = time.perf_counter()
         entry = entry.decode()
+        prot = entry[0]
 
-        if entry.startswith('1'):
-            scan(entry[1:], addr)
-
-        elif entry.startswith('2'):
-            shell_manager(entry[1:], addr)
-
-        elif entry.startswith('3'):
-            zsearch(entry[1:], addr)
-
-        elif entry.startswith('4'):
-            fzfsearch(entry[1:], addr)
-
-        elif entry.startswith('5'):
-            list_directory(entry[1:], addr)
-
-        elif entry.startswith('6'):
-            theme_manager(entry[1:])
-
-        elif entry.startswith('7'):
-            history_search(entry[1:], addr)
+        functionalities[prot](entry[1:], addr)
 
         if '--verbose' in sys.argv:
             took = round(time.perf_counter() - init, 5)
             print(f'Took: {took}s')
 
-
-os.makedirs(APP_HOME, exist_ok=True)
-
-clients = []
-cache = DirCache()
-dispatcher = Dispatcher()
-home = os.path.expanduser('~')
-
-py_version = sys.version
-py_version = py_version[:py_version.index(' ')]
-py_not = 'Python' + ';' + py_version  # notation
-
-exes_with_version = {}
+        gc.collect()
 
 
 #
 # Updating the executables that will be searched starts here
 #
 
 
@@ -252,9 +229,34 @@
     'pwsh': 'Pwsh'
 }
 
 #
 # Stop here
 #
 
+os.makedirs(APP_HOME, exist_ok=True)
+
+entries = map(str, range(1, 8))
+defined_functions = (
+    scan,
+    shell_manager,
+    zsearch,
+    fzfsearch,
+    list_directory,
+    theme_manager,
+    history_search
+)
+functionalities = dict(zip(entries, defined_functions))
+
+clients = []
+cache = DirCache()
+dispatcher = Dispatcher()
+home = os.path.expanduser('~')
+
+py_version = sys.version
+py_version = py_version[:py_version.index(' ')]
+py_not = 'Python' + ';' + py_version  # notation
+
+exes_with_version = {}
+
 for exe in exes_to_search:
     threading.Thread(target=get_version, args=(exe,)).start()
```

### Comparing `shellserver-0.0.8/shellserver/style.py` & `shellserver-0.0.9/shellserver/style.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/shellserver/theme.py` & `shellserver-0.0.9/shellserver/theme.py`

 * *Files identical despite different names*

### Comparing `shellserver-0.0.8/shellserver.egg-info/PKG-INFO` & `shellserver-0.0.9/shellserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: shellserver
-Version: 0.0.8
-Summary: Server to aid shell navigation
+Version: 0.0.9
+Summary: Server to aid shell navigation.
 Home-page: https://github.com/HenriquedoVal/shellserver
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellServer
 
 It's a mix of [Starship](https://github.com/starship/starship) and [Zoxide](https://github.com/ajeetdsouza/zoxide) but faster.  
   
 On Starship, every 'Enter' keystroke spawns a new process, which may cause a lag between prompts.  
 Zoxide will raise a new process every time you call it.  
 ShellServer raises the server only in the first shell creation and will _communicate_ with your shell on every 'Enter' keystroke.  
+Fastness comes from not having spawning time, which seems to be way higher in Windows.  
   
 But if your hardware gives you a fluid shell experience using Starship, I recommend that you keep with it because it's way more customizable.  
 
 ## Features
   
 ### Prompt with a fast glance at what is in directory  
 
@@ -33,14 +34,15 @@
 ![Fast](./images/even_bloated.gif)  
   
 ### Better 'cd'  
 
 ![p, pz](./images/p_pz.gif)
 - Tab completions works just fine.
 - With no arguments will behave just like 'cd'.
+- `p -o path` for writing to output. Tool for things like `move somefile (p -o somepath)`
 Note: [fzf](https://github.com/junegunn/fzf) is a dependency to use 'pz'  
   
 ### Switching Theme
   
 ![Switch-Theme](./images/switch_theme.gif)
 Can take four arguments: all, system, terminal, and blue.  
 - terminal: Toggles Windows Terminal default theme between 'Tango Dark' and 'Solarized Light'.  
@@ -96,20 +98,18 @@
 Import-Module ShellServer
 ~~~
 
 ### Keep updated
 As many things might change in versions below 0.1.0, `pip install --upgrade shellserver` and `Upgrade-Module ShellServer` must be run both when one changes.  
 The last v0.0.8 will work with the PowerShell ShellServer module 0.0.6.
 
-## Known Issues
-
-- Git status info: Now we can parse git packfiles, but still can't resolve deltas. So it will fall back to use git when it's needed (faster but still experimental). Do `pythonw -m shellserver --use-git` in your profile to always use git.
-
 ## Debugging
 
+The git status info still experimental, do `pythonw -m shellserver --use-git` in your profile to always use git. 
+
 Any errors that occur will be saved in `$env:localappdata\shellserver\traceback`.  
   
 Attach a _stdout_ to the server, pass `--verbose` to it and it will give lot of info when it sees a git repo.
 ~~~
 shellserver kill
 # A message that the server is not responding and your prompt will be like before.
 python -m shellserver --verbose  # no w, blocking
```

### Comparing `shellserver-0.0.8/shellserver.egg-info/SOURCES.txt` & `shellserver-0.0.9/shellserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

