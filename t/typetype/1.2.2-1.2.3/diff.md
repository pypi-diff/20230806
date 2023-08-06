# Comparing `tmp/typetype-1.2.2.tar.gz` & `tmp/typetype-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetype-1.2.2.tar", last modified: Wed Jul 26 14:06:24 2023, max compression
+gzip compressed data, was "typetype-1.2.3.tar", last modified: Sun Aug  6 15:49:10 2023, max compression
```

## Comparing `typetype-1.2.2.tar` & `typetype-1.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.066961 typetype-1.2.2/
--rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-07-10 22:56:41.000000 typetype-1.2.2/MANIFEST.in
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-26 14:06:24.066771 typetype-1.2.2/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1541 2023-07-12 23:08:54.000000 typetype-1.2.2/README.md
--rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-07-26 14:06:24.067020 typetype-1.2.2/setup.cfg
--rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-07-26 14:05:14.000000 typetype-1.2.2/setup.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.060399 typetype-1.2.2/typetype/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 22:56:30.000000 typetype-1.2.2/typetype/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-07-17 02:43:05.000000 typetype-1.2.2/typetype/ahmetsgame.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.061913 typetype-1.2.2/typetype/functions/
--rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-07-10 05:56:46.000000 typetype-1.2.2/typetype/functions/__init__.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-07-26 14:03:50.000000 typetype-1.2.2/typetype/functions/game_selection.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     8855 2023-07-26 14:04:28.000000 typetype-1.2.2/typetype/functions/refresh_update.py
--rw-r--r--   0 gulcinozer   (501) staff       (20)     7960 2023-07-12 00:29:14.000000 typetype-1.2.2/typetype/functions/setup_results.py
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.064229 typetype-1.2.2/typetype/words/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/200words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/25000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/5000words.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-07-17 02:42:52.000000 typetype-1.2.2/typetype/words/highscores.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-07-10 04:56:06.000000 typetype-1.2.2/typetype/words/text.txt
-drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-07-26 14:06:24.061194 typetype-1.2.2/typetype.egg-info/
--rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/PKG-INFO
--rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/SOURCES.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/dependency_links.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/entry_points.txt
--rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-07-26 14:06:24.000000 typetype-1.2.2/typetype.egg-info/top_level.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:49:10.493491 typetype-1.2.3/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       48 2023-08-06 15:43:12.000000 typetype-1.2.3/MANIFEST.in
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-08-06 15:49:10.493360 typetype-1.2.3/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1541 2023-08-06 15:43:12.000000 typetype-1.2.3/README.md
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       38 2023-08-06 15:49:10.493538 typetype-1.2.3/setup.cfg
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      662 2023-08-06 15:47:37.000000 typetype-1.2.3/setup.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:49:10.488335 typetype-1.2.3/typetype/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10198 2023-08-06 15:47:53.000000 typetype-1.2.3/typetype/ahmetsgame.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:49:10.489821 typetype-1.2.3/typetype/functions/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/functions/__init__.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    10371 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/functions/game_selection.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     8855 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/functions/refresh_update.py
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     7977 2023-08-06 15:45:21.000000 typetype-1.2.3/typetype/functions/setup_results.py
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:49:10.491057 typetype-1.2.3/typetype/words/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1047 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/words/200words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)   213194 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/words/25000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)    38997 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/words/5000words.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       42 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/words/highscores.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)  1605906 2023-08-06 15:43:12.000000 typetype-1.2.3/typetype/words/text.txt
+drwxr-xr-x   0 gulcinozer   (501) staff       (20)        0 2023-08-06 15:49:10.489010 typetype-1.2.3/typetype.egg-info/
+-rw-r--r--   0 gulcinozer   (501) staff       (20)     1738 2023-08-06 15:49:10.000000 typetype-1.2.3/typetype.egg-info/PKG-INFO
+-rw-r--r--   0 gulcinozer   (501) staff       (20)      519 2023-08-06 15:49:10.000000 typetype-1.2.3/typetype.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        1 2023-08-06 15:49:10.000000 typetype-1.2.3/typetype.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)       58 2023-08-06 15:49:10.000000 typetype-1.2.3/typetype.egg-info/entry_points.txt
+-rw-r--r--   0 gulcinozer   (501) staff       (20)        9 2023-08-06 15:49:10.000000 typetype-1.2.3/typetype.egg-info/top_level.txt
```

### Comparing `typetype-1.2.2/PKG-INFO` & `typetype-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.2
+Version: 1.2.3
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.2.2/README.md` & `typetype-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/setup.py` & `typetype-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='typetype',
-    version='1.2.2',
+    version='1.2.3',
     author='Ahmet Ozer',
     url="https://github.com/ahmet8zer/typetype",
     description='A command line typing game',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `typetype-1.2.2/typetype/ahmetsgame.py` & `typetype-1.2.3/typetype/ahmetsgame.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/functions/game_selection.py` & `typetype-1.2.3/typetype/functions/game_selection.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/functions/refresh_update.py` & `typetype-1.2.3/typetype/functions/refresh_update.py`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/functions/setup_results.py` & `typetype-1.2.3/typetype/functions/setup_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         while len(chosen)>300 or len(chosen)<=160:
             chosen = random.choice(lines)[:-1]
     elif choices[0] == 'x' and choices[1] == 'l':
         chosen = random.choice(lines)[:-1]
         while len(chosen)<=300:
             chosen = random.choice(lines)[:-1]
     if choices[0] == 'x':
-        return chosen
+        return chosen.replace("\\","")
     
     #timed or words
     last10 = []
     sentence = ""
     needed = 200
     
     if choices[0] == 't' and choices[2] == '1':
```

### Comparing `typetype-1.2.2/typetype/words/200words.txt` & `typetype-1.2.3/typetype/words/200words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/words/25000words.txt` & `typetype-1.2.3/typetype/words/25000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/words/5000words.txt` & `typetype-1.2.3/typetype/words/5000words.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype/words/text.txt` & `typetype-1.2.3/typetype/words/text.txt`

 * *Files identical despite different names*

### Comparing `typetype-1.2.2/typetype.egg-info/PKG-INFO` & `typetype-1.2.3/typetype.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetype
-Version: 1.2.2
+Version: 1.2.3
 Summary: A command line typing game
 Home-page: https://github.com/ahmet8zer/typetype
 Author: Ahmet Ozer
 Description-Content-Type: text/markdown
 
 # typetype
 A Command Line Typing Game by Ahmet Ozer
```

### Comparing `typetype-1.2.2/typetype.egg-info/SOURCES.txt` & `typetype-1.2.3/typetype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

