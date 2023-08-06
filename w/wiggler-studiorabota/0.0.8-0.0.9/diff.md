# Comparing `tmp/wiggler_studiorabota-0.0.8.tar.gz` & `tmp/wiggler_studiorabota-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.8.tar", last modified: Sat Jul 15 16:24:14 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.9.tar", last modified: Sat Jul 15 16:30:10 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.8.tar` & `wiggler_studiorabota-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.189909 wiggler_studiorabota-0.0.8/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:24:14.189749 wiggler_studiorabota-0.0.8/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.8/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      544 2023-07-15 16:23:44.000000 wiggler_studiorabota-0.0.8/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 16:24:14.189947 wiggler_studiorabota-0.0.8/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.188295 wiggler_studiorabota-0.0.8/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.8/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      611 2023-07-15 16:24:09.000000 wiggler_studiorabota-0.0.8/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)     1234 2023-07-15 11:06:24.000000 wiggler_studiorabota-0.0.8/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:24:14.189516 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)       58 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 16:24:14.000000 wiggler_studiorabota-0.0.8/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:30:10.202367 wiggler_studiorabota-0.0.9/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:30:10.202209 wiggler_studiorabota-0.0.9/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.9/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      544 2023-07-15 16:30:04.000000 wiggler_studiorabota-0.0.9/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 16:30:10.202407 wiggler_studiorabota-0.0.9/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:30:10.200601 wiggler_studiorabota-0.0.9/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.9/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      627 2023-07-15 16:29:56.000000 wiggler_studiorabota-0.0.9/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1234 2023-07-15 11:06:24.000000 wiggler_studiorabota-0.0.9/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 16:30:10.202015 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      341 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       58 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 16:30:10.000000 wiggler_studiorabota-0.0.9/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.8/pyproject.toml` & `wiggler_studiorabota-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wiggler_studiorabota"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Vincent Kranendonk" },
 ]
 description = "WiggleR - Desktop research unit for making controlled experiments"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `wiggler_studiorabota-0.0.8/wiggler/cli.py` & `wiggler_studiorabota-0.0.9/wiggler/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,10 +10,10 @@
     
     args = parser.parse_args()
   
     if args.server:
         os.system(f"uvicorn wiggler.main:app --reload --host 0.0.0.0")
 
     if args.boot:
-         os.system('cp ./start_wiggler.sh /usr/bin/start_wiggler.sh')
-         os.system('cp ./start_wiggler.service /etc/systemd/system/start_wiggler.service')
+         os.system('cp ./wiggler/start_wiggler.sh /usr/bin/start_wiggler.sh')
+         os.system('cp ./wiggler/start_wiggler.service /etc/systemd/system/start_wiggler.service')
          os.system('systemctl enable start_wiggler')
```

### Comparing `wiggler_studiorabota-0.0.8/wiggler/main.py` & `wiggler_studiorabota-0.0.9/wiggler/main.py`

 * *Files identical despite different names*

