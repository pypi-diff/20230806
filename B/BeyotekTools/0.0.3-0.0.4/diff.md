# Comparing `tmp/BeyotekTools-0.0.3.tar.gz` & `tmp/BeyotekTools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyotekTools-0.0.3.tar", last modified: Sat Aug  5 23:13:24 2023, max compression
+gzip compressed data, was "BeyotekTools-0.0.4.tar", last modified: Sat Aug  5 23:50:32 2023, max compression
```

## Comparing `BeyotekTools-0.0.3.tar` & `BeyotekTools-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 23:13:23.998859 BeyotekTools-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      363 2023-08-05 23:13:23.998859 BeyotekTools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.3/README.md
--rw-rw-rw-   0        0        0      581 2023-08-05 23:13:08.000000 BeyotekTools-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 23:13:23.999859 BeyotekTools-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 23:13:23.984860 BeyotekTools-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 23:13:23.989860 BeyotekTools-0.0.3/src/BeyotekTools/
--rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.3/src/BeyotekTools/__init__.py
--rw-rw-rw-   0        0        0      745 2023-08-05 22:46:29.000000 BeyotekTools-0.0.3/src/BeyotekTools/speedlimit.py
--rw-rw-rw-   0        0        0     2157 2023-08-05 23:11:23.000000 BeyotekTools-0.0.3/src/BeyotekTools/stringutil.py
-drwxrwxrwx   0        0        0        0 2023-08-05 23:13:23.998859 BeyotekTools-0.0.3/src/BeyotekTools.egg-info/
--rw-rw-rw-   0        0        0      363 2023-08-05 23:13:23.000000 BeyotekTools-0.0.3/src/BeyotekTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-08-05 23:13:23.000000 BeyotekTools-0.0.3/src/BeyotekTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 23:13:23.000000 BeyotekTools-0.0.3/src/BeyotekTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 23:13:23.000000 BeyotekTools-0.0.3/src/BeyotekTools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.146136 BeyotekTools-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-08-05 21:37:12.000000 BeyotekTools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      363 2023-08-05 23:50:32.146136 BeyotekTools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:24:31.000000 BeyotekTools-0.0.4/README.md
+-rw-rw-rw-   0        0        0      581 2023-08-05 23:50:16.000000 BeyotekTools-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 23:50:32.147140 BeyotekTools-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.130627 BeyotekTools-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.137633 BeyotekTools-0.0.4/src/BeyotekTools/
+-rw-rw-rw-   0        0        0        0 2023-08-05 21:33:00.000000 BeyotekTools-0.0.4/src/BeyotekTools/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-05 23:49:22.000000 BeyotekTools-0.0.4/src/BeyotekTools/mongodbutil.py
+-rw-rw-rw-   0        0        0     7853 2023-08-05 23:49:59.000000 BeyotekTools-0.0.4/src/BeyotekTools/scraperutil.py
+-rw-rw-rw-   0        0        0      745 2023-08-05 22:46:29.000000 BeyotekTools-0.0.4/src/BeyotekTools/speedlimit.py
+-rw-rw-rw-   0        0        0     1775 2023-08-05 23:26:53.000000 BeyotekTools-0.0.4/src/BeyotekTools/stringutil.py
+drwxrwxrwx   0        0        0        0 2023-08-05 23:50:32.144632 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/
+-rw-rw-rw-   0        0        0      363 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 23:50:32.000000 BeyotekTools-0.0.4/src/BeyotekTools.egg-info/top_level.txt
```

### Comparing `BeyotekTools-0.0.3/LICENSE` & `BeyotekTools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.3/pyproject.toml` & `BeyotekTools-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BeyotekTools"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Beyotek", email="chuck@beyotek.com" },
 ]
 description = "Beyotek Tools"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `BeyotekTools-0.0.3/src/BeyotekTools/speedlimit.py` & `BeyotekTools-0.0.4/src/BeyotekTools/speedlimit.py`

 * *Files identical despite different names*

### Comparing `BeyotekTools-0.0.3/src/BeyotekTools/stringutil.py` & `BeyotekTools-0.0.4/src/BeyotekTools/stringutil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-import logging
-logger = logging.getLogger()
-
-
 def get_string_between_2_substrings(input_string, start_substring, end_substring, remove_space):
     input_string = str(input_string)
     start_index = input_string.find(start_substring)
 
     if not start_index or start_index == -1:
-        return f"Get String Between 2 Substrings: Could not locate start substring '{start_substring}'"
+        return None
 
     start_index += len(start_substring)
     end_index = input_string.find(end_substring, start_index)
 
     if not end_index or end_index == -1:
-        return f"Get String Between 2 Substrings: Could not locate end substring '{end_substring}'"
+        return None
 
     if remove_space:
         string = input_string[start_index:end_index]
         string.replace(" ", "")
         return string
 
     else:
@@ -25,15 +21,15 @@
 
 
 def get_string_between_substring_and_end(input_string, start_substring, remove_space):
     input_string = str(input_string)
     start_index = input_string.find(start_substring)
 
     if not start_index or start_index == -1:
-        return f"Get String Between 2 Substrings: Could not locate start substring '{start_substring}'"
+        return None
     else:
 
         start_index += len(start_substring)
         end_index = len(input_string)
 
         if remove_space:
             string = input_string[start_index:end_index]
@@ -44,15 +40,15 @@
 
 
 def get_string_between_last_substring_and_end(input_string, start_substring, remove_space):
     input_string = str(input_string)
     start_index = input_string.rfind(start_substring)
 
     if not start_index or start_index == -1:
-        return f"Get String Between 2 Substrings: Could not locate start substring '{start_substring}'"
+        return None
     else:
 
         start_index += len(start_substring)
         end_index = len(input_string)
 
         if remove_space:
             string = input_string[start_index:end_index]
```

