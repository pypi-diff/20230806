# Comparing `tmp/ycv-0.0.dev6.tar.gz` & `tmp/ycv-0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycv-0.0.dev6.tar", last modified: Mon Jun 19 14:26:45 2023, max compression
+gzip compressed data, was "ycv-0.0.dev7.tar", last modified: Sun Aug  6 07:24:00 2023, max compression
```

## Comparing `ycv-0.0.dev6.tar` & `ycv-0.0.dev7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:26:45.362008 ycv-0.0.dev6/
--rw-r--r--   0 arif      (1000) arif      (1000)     1071 2023-06-19 13:59:34.000000 ycv-0.0.dev6/LICENSE
--rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-06-19 14:26:45.362008 ycv-0.0.dev6/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)     2697 2023-06-19 13:59:34.000000 ycv-0.0.dev6/README.md
--rw-r--r--   0 arif      (1000) arif      (1000)       84 2023-06-19 13:59:34.000000 ycv-0.0.dev6/pyproject.toml
--rw-r--r--   0 arif      (1000) arif      (1000)      697 2023-06-19 14:26:45.362008 ycv-0.0.dev6/setup.cfg
--rw-r--r--   0 arif      (1000) arif      (1000)      420 2023-06-19 14:25:22.000000 ycv-0.0.dev6/setup.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:26:45.360008 ycv-0.0.dev6/test/
--rw-r--r--   0 arif      (1000) arif      (1000)      204 2023-06-19 13:59:34.000000 ycv-0.0.dev6/test/test_interface.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:26:45.360008 ycv-0.0.dev6/ycv/
--rw-r--r--   0 arif      (1000) arif      (1000)       88 2023-06-19 13:59:34.000000 ycv-0.0.dev6/ycv/__init__.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2311 2023-06-19 13:59:34.000000 ycv-0.0.dev6/ycv/publications.py
--rw-r--r--   0 arif      (1000) arif      (1000)    25186 2023-06-19 14:24:53.000000 ycv-0.0.dev6/ycv/yamlToTex.py
--rw-r--r--   0 arif      (1000) arif      (1000)     1503 2023-06-19 13:59:34.000000 ycv-0.0.dev6/ycv/ycv.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 14:26:45.362008 ycv-0.0.dev6/ycv.egg-info/
--rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)      302 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/SOURCES.txt
--rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/dependency_links.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       48 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/entry_points.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       20 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/requires.txt
--rw-r--r--   0 arif      (1000) arif      (1000)        4 2023-06-19 14:26:45.000000 ycv-0.0.dev6/ycv.egg-info/top_level.txt
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-06 07:24:00.701502 ycv-0.0.dev7/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1071 2023-06-19 13:59:34.000000 ycv-0.0.dev7/LICENSE
+-rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-08-06 07:24:00.701502 ycv-0.0.dev7/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)     2697 2023-06-19 13:59:34.000000 ycv-0.0.dev7/README.md
+-rw-r--r--   0 arif      (1000) arif      (1000)       84 2023-06-19 13:59:34.000000 ycv-0.0.dev7/pyproject.toml
+-rw-r--r--   0 arif      (1000) arif      (1000)      697 2023-08-06 07:24:00.701502 ycv-0.0.dev7/setup.cfg
+-rw-r--r--   0 arif      (1000) arif      (1000)      420 2023-08-06 07:23:46.000000 ycv-0.0.dev7/setup.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-06 07:24:00.699502 ycv-0.0.dev7/test/
+-rw-r--r--   0 arif      (1000) arif      (1000)      204 2023-06-19 13:59:34.000000 ycv-0.0.dev7/test/test_interface.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-06 07:24:00.700502 ycv-0.0.dev7/ycv/
+-rw-r--r--   0 arif      (1000) arif      (1000)       88 2023-06-19 13:59:34.000000 ycv-0.0.dev7/ycv/__init__.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2311 2023-06-19 13:59:34.000000 ycv-0.0.dev7/ycv/publications.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    25447 2023-08-05 11:09:54.000000 ycv-0.0.dev7/ycv/yamlToTex.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1503 2023-06-19 13:59:34.000000 ycv-0.0.dev7/ycv/ycv.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-06 07:24:00.701502 ycv-0.0.dev7/ycv.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)      302 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/SOURCES.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/dependency_links.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       48 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/entry_points.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       20 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/requires.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        4 2023-08-06 07:24:00.000000 ycv-0.0.dev7/ycv.egg-info/top_level.txt
```

### Comparing `ycv-0.0.dev6/LICENSE` & `ycv-0.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev6/PKG-INFO` & `ycv-0.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev6
+Version: 0.0.dev7
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ycv-0.0.dev6/README.md` & `ycv-0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev6/setup.cfg` & `ycv-0.0.dev7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ycv
-version = 0.0.dev6
+version = 0.0.dev7
 author = Md Arif Shaikh
 author_email = arifshaikh.astro@gmail.com
 description = Build CV and job application materials from yaml files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/md-arif-shaikh/ycv
 project_urls =
```

### Comparing `ycv-0.0.dev6/ycv/publications.py` & `ycv-0.0.dev7/ycv/publications.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev6/ycv/yamlToTex.py` & `ycv-0.0.dev7/ycv/yamlToTex.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,25 +269,32 @@
         pos_text = "\\" + self.cv_section + self.cv_section_number + "{Positions}\n"
         pos_text += "\\begin{itemize}\n"
         for idx, pos in enumerate(positions):
             p = positions[pos]
             if p['to-year'] is None:
                 p['to-year'] = r"{\itshape current}"
             pos_text += fr"\item {{\bfseries {p['position']}}} \hfill {p['from-year']}--{p['to-year']}\\" + "\n"
-            pos_text += self.create_link(p['department-website'], p['department'])
+            if p["department"] is not None:
+                pos_text += self.create_link(p['department-website'], p['department'])
             pos_text += self.create_link(p['institute-website'], p['institute'], False) + r"\\" + "\n"
-            pos_text += fr"{p['institute-address']}\\" + "\n"
-            if p["mentors"] is not None:
-                pos_text += r"{\itshape Mentors}: "
-                for idx, mentor in enumerate(p["mentors"]):
-                    m = p["mentors"][mentor]
-                    if idx < len(p['mentors']) - 1:
-                        pos_text += self.create_link(m['website'], m['name'])
-                    else:
-                        pos_text += self.create_link(m['website'], m['name'], False) + "\n\n"
+            pos_text += fr"{p['institute-address']}"
+            if "mentors" in p:
+                if p["mentors"] is not None:
+                    pos_text += r"\\" + "\n"
+                    pos_text += r"{\itshape Mentors}: "
+                    for idx, mentor in enumerate(p["mentors"]):
+                        m = p["mentors"][mentor]
+                        if idx < len(p['mentors']) - 1:
+                            pos_text += self.create_link(m['website'], m['name'])
+                        else:
+                            pos_text += self.create_link(m['website'], m['name'], False) + "\n\n"
+                else:
+                    pos_text += "\n\n"
+            else:
+                pos_text += "\n\n"
         pos_text += "\\end{itemize}\n"
         return pos_text
 
     def create_environment(self, environment, text):
         tex = f"\\begin{{{environment}}}\n"
         tex += text + "\n"
         tex = f"\\end{{{environment}}}\n"
```

### Comparing `ycv-0.0.dev6/ycv/ycv.py` & `ycv-0.0.dev7/ycv/ycv.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev6/ycv.egg-info/PKG-INFO` & `ycv-0.0.dev7/ycv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev6
+Version: 0.0.dev7
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

