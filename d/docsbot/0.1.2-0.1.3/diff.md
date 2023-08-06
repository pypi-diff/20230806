# Comparing `tmp/docsbot-0.1.2.tar.gz` & `tmp/docsbot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsbot-0.1.2.tar", last modified: Thu Aug  3 15:58:49 2023, max compression
+gzip compressed data, was "docsbot-0.1.3.tar", last modified: Sun Aug  6 04:18:33 2023, max compression
```

## Comparing `docsbot-0.1.2.tar` & `docsbot-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-03 15:58:49.653809 docsbot-0.1.2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1807 2023-08-03 15:58:49.653709 docsbot-0.1.2/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     1618 2023-08-03 14:33:32.000000 docsbot-0.1.2/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-03 15:58:49.653580 docsbot-0.1.2/docsbot.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1807 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-03 15:58:49.000000 docsbot-0.1.2/docsbot.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-03 15:58:49.653841 docsbot-0.1.2/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-03 15:58:46.000000 docsbot-0.1.2/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-06 04:18:33.289890 docsbot-0.1.3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-06 04:18:33.289774 docsbot-0.1.3/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4629 2023-08-04 13:20:17.000000 docsbot-0.1.3/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-08-06 04:18:33.289628 docsbot-0.1.3/docsbot.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4818 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      206 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       37 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       80 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-08-06 04:18:33.000000 docsbot-0.1.3/docsbot.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-08-06 04:18:33.289919 docsbot-0.1.3/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      667 2023-08-06 04:18:32.000000 docsbot-0.1.3/setup.py
```

### Comparing `docsbot-0.1.2/setup.py` & `docsbot-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name='docsbot',
-    version='0.1.2',
+    version='0.1.3',
     description='A simple chat bot for querying information from your local private documents.',
     author='J',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
```

