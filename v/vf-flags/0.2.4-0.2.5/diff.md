# Comparing `tmp/vf-flags-0.2.4.tar.gz` & `tmp/vf-flags-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vf-flags-0.2.4.tar", last modified: Fri Jul 21 02:27:39 2023, max compression
+gzip compressed data, was "vf-flags-0.2.5.tar", last modified: Sun Aug  6 13:33:44 2023, max compression
```

## Comparing `vf-flags-0.2.4.tar` & `vf-flags-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.044876 vf-flags-0.2.4/
--rw-rw-rw-   0        0        0    35184 2023-01-13 17:01:05.000000 vf-flags-0.2.4/LICENSE
--rw-rw-rw-   0        0        0    42996 2023-07-21 02:27:39.043876 vf-flags-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-01-13 23:16:44.000000 vf-flags-0.2.4/README.rst
--rw-rw-rw-   0        0        0     1111 2023-07-21 02:26:39.000000 vf-flags-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 02:27:39.044876 vf-flags-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.037871 vf-flags-0.2.4/vf_flags.egg-info/
--rw-rw-rw-   0        0        0    42996 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-21 02:27:39.000000 vf-flags-0.2.4/vf_flags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-21 02:27:38.000000 vf-flags-0.2.4/vf_flags.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 02:27:39.041874 vf-flags-0.2.4/vfflags/
--rw-rw-rw-   0        0        0     4728 2023-07-21 02:26:23.000000 vf-flags-0.2.4/vfflags/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-13 23:16:44.000000 vf-flags-0.2.4/vfflags/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-06 13:33:44.979690 vf-flags-0.2.5/
+-rw-rw-rw-   0        0        0    35184 2023-01-13 17:01:05.000000 vf-flags-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    42996 2023-08-06 13:33:44.978689 vf-flags-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-01-13 23:16:44.000000 vf-flags-0.2.5/README.rst
+-rw-rw-rw-   0        0        0     1111 2023-08-06 13:31:51.000000 vf-flags-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 13:33:44.979690 vf-flags-0.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 13:33:44.974686 vf-flags-0.2.5/vf_flags.egg-info/
+-rw-rw-rw-   0        0        0    42996 2023-08-06 13:33:44.000000 vf-flags-0.2.5/vf_flags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-08-06 13:33:44.000000 vf-flags-0.2.5/vf_flags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 13:33:44.000000 vf-flags-0.2.5/vf_flags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-06 13:33:44.000000 vf-flags-0.2.5/vf_flags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-06 13:33:44.000000 vf-flags-0.2.5/vf_flags.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 13:33:44.976688 vf-flags-0.2.5/vfflags/
+-rw-rw-rw-   0        0        0     4889 2023-08-06 13:30:48.000000 vf-flags-0.2.5/vfflags/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-13 23:16:44.000000 vf-flags-0.2.5/vfflags/py.typed
```

### Comparing `vf-flags-0.2.4/LICENSE` & `vf-flags-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vf-flags-0.2.4/PKG-INFO` & `vf-flags-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-flags
-Version: 0.2.4
+Version: 0.2.5
 Summary: A wrapper for easily making bitwise flags.
 Author-email: Kae Bartlett <kae@voxelfox.co.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `vf-flags-0.2.4/README.rst` & `vf-flags-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `vf-flags-0.2.4/pyproject.toml` & `vf-flags-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [tool.setuptools]
 packages.find.where = ["."]
 package-data.vfflags = ["*.pyi", "py.typed"]
 
 
 [project]
 name = "vf-flags"
-version = "0.2.4"
+version = "0.2.5"
 description = "A wrapper for easily making bitwise flags."
 authors = [
     {name = "Kae Bartlett", email = "kae@voxelfox.co.uk"},
 ]
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `vf-flags-0.2.4/vf_flags.egg-info/PKG-INFO` & `vf-flags-0.2.5/vf_flags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vf-flags
-Version: 0.2.4
+Version: 0.2.5
 Summary: A wrapper for easily making bitwise flags.
 Author-email: Kae Bartlett <kae@voxelfox.co.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `vf-flags-0.2.4/vfflags/__init__.py` & `vf-flags-0.2.5/vfflags/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,16 +117,20 @@
             yield name, val
 
     def update(self, **kwargs: bool) -> Self:
         """
         Set flag values in-place for the given instance.
         """
 
+        for i in kwargs.keys():
+            if i not in self.VALID_FLAGS:
+                raise ValueError("%s is not a valid flag" % i)
         for i, o in kwargs.items():
             setattr(self, i, o)
+        return self
 
     @classmethod
     def all(cls) -> Self:
         """
         Get an instance of this class with all attributes set to ``True``.
         """
```

