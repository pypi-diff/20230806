# Comparing `tmp/win-basic-tools-0.3.4.tar.gz` & `tmp/win-basic-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win-basic-tools-0.3.4.tar", last modified: Thu Apr 20 12:10:31 2023, max compression
+gzip compressed data, was "win-basic-tools-0.4.0.tar", last modified: Sun Aug  6 09:13:51 2023, max compression
```

## Comparing `win-basic-tools-0.3.4.tar` & `win-basic-tools-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/
--rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.3.4/LICENSE
--rw-rw-rw-   0        0        0     1265 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-04-20 12:08:57.000000 win-basic-tools-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.649725 win-basic-tools-0.3.4/win_basic_tools/
--rw-rw-rw-   0        0        0     8159 2023-04-20 12:05:40.000000 win-basic-tools-0.3.4/win_basic_tools/__init__.py
--rw-rw-rw-   0        0        0      304 2023-02-22 04:20:54.000000 win-basic-tools-0.3.4/win_basic_tools/__main__.py
--rw-rw-rw-   0        0        0     2132 2023-02-17 06:01:06.000000 win-basic-tools-0.3.4/win_basic_tools/setup_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:10:31.665343 win-basic-tools-0.3.4/win_basic_tools.egg-info/
--rw-rw-rw-   0        0        0     1265 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-20 12:10:31.000000 win-basic-tools-0.3.4/win_basic_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/
+-rw-rw-rw-   0        0        0     1093 2023-02-21 08:29:35.000000 win-basic-tools-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1785 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-02-04 05:43:45.000000 win-basic-tools-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1075 2023-07-18 06:25:40.000000 win-basic-tools-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:13:51.011726 win-basic-tools-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 09:13:50.996150 win-basic-tools-0.4.0/win_basic_tools/
+-rw-rw-rw-   0        0        0     9936 2023-07-18 06:09:09.000000 win-basic-tools-0.4.0/win_basic_tools/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-07-18 03:23:45.000000 win-basic-tools-0.4.0/win_basic_tools/__main__.py
+-rw-rw-rw-   0        0        0     2137 2023-08-06 09:12:17.000000 win-basic-tools-0.4.0/win_basic_tools/setup_cmd.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:13:50.996150 win-basic-tools-0.4.0/win_basic_tools.egg-info/
+-rw-rw-rw-   0        0        0     1785 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:13:50.000000 win-basic-tools-0.4.0/win_basic_tools.egg-info/top_level.txt
```

### Comparing `win-basic-tools-0.3.4/LICENSE` & `win-basic-tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.3.4/PKG-INFO` & `win-basic-tools-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.3.4
-Summary: Gives some small tools for shells on Windows
-Home-page: https://github.com/HenriquedoVal/win-basic-tools
+Version: 0.4.0
+Summary: Cli tool for listing the directory.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
+License: MIT
+Project-URL: Home-page, https://github.com/HenriquedoVal/win-basic-tools
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # win-basic-tools
 
 Description:
```

### Comparing `win-basic-tools-0.3.4/README.md` & `win-basic-tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `win-basic-tools-0.3.4/win_basic_tools/__init__.py` & `win-basic-tools-0.4.0/win_basic_tools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 import os
 import stat
 import sys
 import time
 
 from colorama import Fore, Style, deinit, init
 
+try:
+    import locale
+    locale.setlocale(locale.LC_ALL, '')
+except locale.Error:
+    pass
+
 check_0 = (
     ('d', stat.FILE_ATTRIBUTE_DIRECTORY),
     ('l', stat.FILE_ATTRIBUTE_REPARSE_POINT),
 )
 
 check_1 = (
     ('a', stat.FILE_ATTRIBUTE_ARCHIVE),
@@ -54,14 +60,27 @@
         except PermissionError:
             return self.entry.is_dir(follow_symlinks=False)
 
     def is_symlink(self):
         return self.entry.is_symlink()
 
 
+class Options:
+    def __init__(self, opt: str) -> None:
+        self.all = 'a' in opt
+        self.colors = 'c' in opt
+        self.icons = 'i' in opt
+        self.list = 'l' in opt
+        self.mtime = 'm' in opt
+        self.ctime = 'C' in opt
+        self.atime = 'A' in opt
+        self.hour = 'H' in opt
+        self.headers = 'h' in opt
+
+
 class Ls:
     '''
     Lists the content of a directory.
     '''
 
     __slots__ = 'opt', 'path', 'out', 'files', 'dirs', 'size'
 
@@ -70,14 +89,15 @@
         init()
 
         if not opt or opt.startswith('-'):
             self.opt, self.path = opt, path
         else:
             self.opt, self.path = '', opt
 
+        self.opt = Options(opt)
         self.out = StringIO() if to_cache else sys.stdout
         self.files = 0
         self.dirs = 0
         self.size = 0
 
     def __del__(self):
         deinit()
@@ -108,73 +128,123 @@
             print(f'{self.path} is not a valid path.', file=self.out)
             return
 
         scandir = [DirEntryWrapper(i) for i in scandir]
 
         # just add to the list if it will be ever displayed
         # first we remove hidden ones if user hasn't asked for it
-        dir = [
-            i for i in scandir
-            if ('a' in self.opt or not (
+        _dir = [
+            (i, i.stat()) for i in scandir
+            if (self.opt.all or not (
                 i.name.startswith('.') or
                 i.stat().st_file_attributes &
                 stat.FILE_ATTRIBUTE_HIDDEN)
                 )
         ]
 
-        if 'l' not in self.opt:
-            # if in, i would want the oposite order
-            dir.sort(key=lambda x: (x.stat().st_mode, x.name), reverse=True)
+        pad = '   '
+
+        if not self.opt.list:
+            # if True, i would want the oposite order
+            _dir.sort(key=lambda x: (x[1].st_mode, x[0].name), reverse=True)
 
             print(
-                *[self._type_color(i) for i in dir],
-                sep='   ', file=self.out
+                *[self._type_color(i[0]) for i in _dir],
+                sep=pad, file=self.out
             )
             return
 
-        dir.sort(key=lambda x: (x.stat().st_mode, x.name))
+        _dir.sort(key=lambda x: (x[1].st_mode, x[0].name))
+
+        if self.opt.headers and _dir:
+            self._print_headers(pad)
 
-        for i in dir:
+        time_mask = '%x'
+        if self.opt.hour:
+            time_mask += ' %X'
+
+        time_str = ''
+
+        for file, file_stat in _dir:
             filemode_str = self._windows_filemode(
-                i.stat().st_file_attributes
+                file_stat.st_file_attributes
             )
 
-            # print() by 'column item' for better performance
+            # print() by 'column item' for better "performance feel"
+            # when output is stdout
             print(end=' ', file=self.out)
-            print(filemode_str, end='   ', file=self.out)
-            print(time.strftime(
-                '%d %b %y %H:%M', time.localtime(
-                    i.stat().st_ctime)), end='   ', file=self.out)
+            print(filemode_str, end=pad, file=self.out)
+
+            for _opt in ('ctime', 'mtime', 'atime'):
+                if getattr(self.opt, _opt):
+                    time_str = time.strftime(
+                        time_mask, time.localtime(
+                            getattr(file_stat, 'st_' + _opt))
+                    )
+
+                    print(time_str, end=pad, file=self.out)
+
             print(
-                self._humanize_size(i).rjust(7),
-                end='   ', file=self.out
+                self._humanize_size(file).rjust(7),
+                end=pad, file=self.out
             )
-            print(self._type_color(i), file=self.out)
+
+            print(self._type_color(file), file=self.out)
 
         if not any((self.files, self.dirs)):
             return
 
-        total_size = self._humanize_size2(self.size).rjust(7)
+        total_size = (
+            self._humanize_size2(self.size) if self.size else '-'
+        ).rjust(7)
+
+        left_pad = (
+            sum((self.opt.mtime, self.opt.ctime, self.opt.atime))
+            * (len(time_str) + len(pad))
+            + len(pad) + 8  # inital space + filemode
+        )
+
+        f = 'File'
+        if self.files != 1:
+            f += 's'
+
+        d = 'Directory'
+        if self.dirs != 1:
+            d = d[:-1] + 'ies'
+
         print(
-            str(self.files).rjust(3) + ' Files',
-            str(self.dirs).rjust(2) + ' Dirs',
-            'Total: ', total_size,
-            sep='  ', file=self.out
+            ' ' * left_pad
+            + total_size
+            + pad
+            + f'{self.files} {f}, {self.dirs} {d}',
+            end='', file=self.out
         )
 
+    def _print_headers(self, pad):
+        res = Fore.GREEN + ' ' * 3 + 'Mode ' + pad
+
+        for _opt in ('ctime', 'mtime', 'atime'):
+            if getattr(self.opt, _opt):
+                res += _opt.capitalize().center(
+                    10 + 9 * int(self.opt.hour)) + pad
+
+        res += '   Size' + pad + 'Name' + Style.RESET_ALL
+
+        print(res, end='\n\n', file=self.out)
+
     def _type_color(self, i: DirEntryWrapper) -> str:
         is_syml = i.is_symlink()
         is_dir = i.is_dir()
 
         if is_dir:
             self.dirs += 1
         if is_syml:
             self.files += 1
 
-        if 'c' not in self.opt:
+        if not self.opt.colors:
             return i.name
 
         if is_dir or is_syml:
             joined = os.path.join(os.path.realpath(self.path), i.name)
             if os.path.realpath(i.path) != joined:
                 return (Fore.CYAN
                         + i.name
@@ -208,15 +278,15 @@
             final = unit
 
         if final:
             data = f'{entry:.1f}{final}'
         else:
             data = str(entry)
 
-        if 'c' in self.opt:
+        if self.opt.colors:
             if 'G' in data:
                 data = Fore.RED + data + Style.RESET_ALL
                 data = data.rjust(16)
             elif 'M' in data:
                 data = Fore.LIGHTRED_EX + data + Style.RESET_ALL
                 data = data.rjust(16)
             elif 'k' in data:
@@ -245,24 +315,24 @@
                     res[0] = check[0]
 
             for ind, check in zip(range(1, 5), check_1):
                 if data & check[1]:
                     res[ind] = check[0]
 
         icon = ''
-        if 'i' in self.opt:
+        if self.opt.icons:
             for ind in range(5):
                 if res[ind] in icons_map:
                     icon = icons_map[res[ind]]
                     break
             else:
                 icon = icons_map['else']
 
         done = False  # flags coloring icon
-        if 'c' in self.opt:
+        if self.opt.colors:
             for ind in range(5):
                 if res[ind] == '-':
                     continue
                 if icon and res[ind] in icons_map and not done:
                     icon = colors_map[res[ind]] + icon + Style.RESET_ALL
                     done = True
                 res[ind] = (Fore.BLUE + res[ind] + Style.RESET_ALL)
```

### Comparing `win-basic-tools-0.3.4/win_basic_tools/setup_cmd.py` & `win-basic-tools-0.4.0/win_basic_tools/setup_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 
 def setup():
 
     with open(f'{HOME_PATH}\\.macros.doskey', 'w') as f:
         print(
             'ls=python -m win_basic_tools $*',
-            'll=python -m win_basic_tools -cil $*',
-            'la=python -m win_basic_tools -acil $*',
+            'll=python -m win_basic_tools -cilm $*',
+            'la=python -m win_basic_tools -acilmhAH $*',
             'touch=echo off $T for %x in ($*) do type nul > %x $T echo on',
             'cat=type $1',
             'pwd=cd',
             'mv=move $1 $2',
             'rm=del $*',
             sep='\n',
             file=f
```

### Comparing `win-basic-tools-0.3.4/win_basic_tools.egg-info/PKG-INFO` & `win-basic-tools-0.4.0/win_basic_tools.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 Metadata-Version: 2.1
 Name: win-basic-tools
-Version: 0.3.4
-Summary: Gives some small tools for shells on Windows
-Home-page: https://github.com/HenriquedoVal/win-basic-tools
+Version: 0.4.0
+Summary: Cli tool for listing the directory.
 Author: Henrique do Val
 Author-email: henrique.val@hotmail.com
+License: MIT
+Project-URL: Home-page, https://github.com/HenriquedoVal/win-basic-tools
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: Terminals
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # win-basic-tools
 
 Description:
```

