# Comparing `tmp/BubbleGun-1.1.6.tar.gz` & `tmp/BubbleGun-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BubbleGun-1.1.6.tar", last modified: Tue Feb 28 21:20:34 2023, max compression
+gzip compressed data, was "BubbleGun-1.1.7.tar", last modified: Sun Aug  6 12:42:47 2023, max compression
```

## Comparing `BubbleGun-1.1.6.tar` & `BubbleGun-1.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-02-28 21:20:34.234011 BubbleGun-1.1.6/
-drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-02-28 21:20:34.234011 BubbleGun-1.1.6/BubbleGun/
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2751 2022-04-26 12:40:42.000000 BubbleGun-1.1.6/BubbleGun/Bubble.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     4827 2022-03-10 11:02:38.000000 BubbleGun-1.1.6/BubbleGun/BubbleChain.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11937 2022-06-17 12:54:10.000000 BubbleGun-1.1.6/BubbleGun/Graph.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2199 2021-03-24 19:55:49.000000 BubbleGun-1.1.6/BubbleGun/Node.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)        0 2021-03-24 19:55:49.000000 BubbleGun-1.1.6/BubbleGun/__init__.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     4078 2021-11-25 15:45:33.000000 BubbleGun-1.1.6/BubbleGun/bfs.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      935 2022-05-31 10:07:33.000000 BubbleGun-1.1.6/BubbleGun/bubbles_fasta.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    10382 2022-04-29 09:14:17.000000 BubbleGun-1.1.6/BubbleGun/compact_graph.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1904 2021-03-24 19:58:26.000000 BubbleGun-1.1.6/BubbleGun/connect_bubbles.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1463 2022-03-14 09:34:35.000000 BubbleGun-1.1.6/BubbleGun/connected_components.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2061 2021-03-24 19:58:26.000000 BubbleGun-1.1.6/BubbleGun/fasta_chains.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     7855 2021-03-24 19:58:26.000000 BubbleGun-1.1.6/BubbleGun/find_bubbles.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1616 2021-03-24 19:58:26.000000 BubbleGun-1.1.6/BubbleGun/find_parents.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1831 2023-01-02 10:43:15.000000 BubbleGun-1.1.6/BubbleGun/functions.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    12063 2022-03-10 12:08:22.000000 BubbleGun-1.1.6/BubbleGun/graph_io.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2895 2021-03-24 19:55:49.000000 BubbleGun-1.1.6/BubbleGun/json_out.py
--rwxrwxr-x   0 fawaz     (1000) fawaz     (1000)    14265 2022-06-17 12:59:51.000000 BubbleGun-1.1.6/BubbleGun/main.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      997 2021-03-24 19:55:49.000000 BubbleGun-1.1.6/BubbleGun/output_certain_chains.py
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2801 2021-03-24 19:55:49.000000 BubbleGun-1.1.6/BubbleGun/path_extractor.py
-drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-02-28 21:20:34.234011 BubbleGun-1.1.6/BubbleGun.egg-info/
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11720 2023-02-28 21:20:34.000000 BubbleGun-1.1.6/BubbleGun.egg-info/PKG-INFO
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      658 2023-02-28 21:20:34.000000 BubbleGun-1.1.6/BubbleGun.egg-info/SOURCES.txt
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)        1 2023-02-28 21:20:34.000000 BubbleGun-1.1.6/BubbleGun.egg-info/dependency_links.txt
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       51 2023-02-28 21:20:34.000000 BubbleGun-1.1.6/BubbleGun.egg-info/entry_points.txt
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       10 2023-02-28 21:20:34.000000 BubbleGun-1.1.6/BubbleGun.egg-info/top_level.txt
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1071 2021-01-27 03:32:31.000000 BubbleGun-1.1.6/LICENSE
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11720 2023-02-28 21:20:34.234011 BubbleGun-1.1.6/PKG-INFO
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11364 2022-07-11 15:12:31.000000 BubbleGun-1.1.6/README.md
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       38 2023-02-28 21:20:34.234011 BubbleGun-1.1.6/setup.cfg
--rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1172 2023-02-28 21:20:25.000000 BubbleGun-1.1.6/setup.py
+drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-08-06 12:42:47.185027 BubbleGun-1.1.7/
+drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-08-06 12:42:47.185027 BubbleGun-1.1.7/BubbleGun/
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     4535 2023-08-06 08:15:04.000000 BubbleGun-1.1.7/BubbleGun/Bubble.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     4827 2022-03-10 11:02:38.000000 BubbleGun-1.1.7/BubbleGun/BubbleChain.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11937 2022-06-17 12:54:10.000000 BubbleGun-1.1.7/BubbleGun/Graph.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2199 2021-03-24 19:55:49.000000 BubbleGun-1.1.7/BubbleGun/Node.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)        0 2021-03-24 19:55:49.000000 BubbleGun-1.1.7/BubbleGun/__init__.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     4078 2021-11-25 15:45:33.000000 BubbleGun-1.1.7/BubbleGun/bfs.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      935 2022-05-31 10:07:33.000000 BubbleGun-1.1.7/BubbleGun/bubbles_fasta.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    10382 2022-04-29 09:14:17.000000 BubbleGun-1.1.7/BubbleGun/compact_graph.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1904 2021-03-24 19:58:26.000000 BubbleGun-1.1.7/BubbleGun/connect_bubbles.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1463 2022-03-14 09:34:35.000000 BubbleGun-1.1.7/BubbleGun/connected_components.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2061 2021-03-24 19:58:26.000000 BubbleGun-1.1.7/BubbleGun/fasta_chains.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     8032 2023-08-05 05:14:08.000000 BubbleGun-1.1.7/BubbleGun/find_bubbles.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1616 2021-03-24 19:58:26.000000 BubbleGun-1.1.7/BubbleGun/find_parents.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1831 2023-01-02 10:43:15.000000 BubbleGun-1.1.7/BubbleGun/functions.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    12063 2022-03-10 12:08:22.000000 BubbleGun-1.1.7/BubbleGun/graph_io.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2895 2021-03-24 19:55:49.000000 BubbleGun-1.1.7/BubbleGun/json_out.py
+-rwxrwxr-x   0 fawaz     (1000) fawaz     (1000)    14265 2022-06-17 12:59:51.000000 BubbleGun-1.1.7/BubbleGun/main.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      997 2021-03-24 19:55:49.000000 BubbleGun-1.1.7/BubbleGun/output_certain_chains.py
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     2801 2021-03-24 19:55:49.000000 BubbleGun-1.1.7/BubbleGun/path_extractor.py
+drwxrwxr-x   0 fawaz     (1000) fawaz     (1000)        0 2023-08-06 12:42:47.185027 BubbleGun-1.1.7/BubbleGun.egg-info/
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11720 2023-08-06 12:42:47.000000 BubbleGun-1.1.7/BubbleGun.egg-info/PKG-INFO
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)      658 2023-08-06 12:42:47.000000 BubbleGun-1.1.7/BubbleGun.egg-info/SOURCES.txt
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)        1 2023-08-06 12:42:47.000000 BubbleGun-1.1.7/BubbleGun.egg-info/dependency_links.txt
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       51 2023-08-06 12:42:47.000000 BubbleGun-1.1.7/BubbleGun.egg-info/entry_points.txt
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       10 2023-08-06 12:42:47.000000 BubbleGun-1.1.7/BubbleGun.egg-info/top_level.txt
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1071 2021-01-27 03:32:31.000000 BubbleGun-1.1.7/LICENSE
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11720 2023-08-06 12:42:47.185027 BubbleGun-1.1.7/PKG-INFO
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)    11364 2022-07-11 15:12:31.000000 BubbleGun-1.1.7/README.md
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)       38 2023-08-06 12:42:47.185027 BubbleGun-1.1.7/setup.cfg
+-rw-rw-r--   0 fawaz     (1000) fawaz     (1000)     1172 2023-08-06 08:11:01.000000 BubbleGun-1.1.7/setup.py
```

### Comparing `BubbleGun-1.1.6/BubbleGun/BubbleChain.py` & `BubbleGun-1.1.7/BubbleGun/BubbleChain.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/Graph.py` & `BubbleGun-1.1.7/BubbleGun/Graph.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/Node.py` & `BubbleGun-1.1.7/BubbleGun/Node.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/bfs.py` & `BubbleGun-1.1.7/BubbleGun/bfs.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/bubbles_fasta.py` & `BubbleGun-1.1.7/BubbleGun/bubbles_fasta.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/compact_graph.py` & `BubbleGun-1.1.7/BubbleGun/compact_graph.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/connect_bubbles.py` & `BubbleGun-1.1.7/BubbleGun/connect_bubbles.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/connected_components.py` & `BubbleGun-1.1.7/BubbleGun/connected_components.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/fasta_chains.py` & `BubbleGun-1.1.7/BubbleGun/fasta_chains.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/find_bubbles.py` & `BubbleGun-1.1.7/BubbleGun/find_bubbles.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,19 @@
             nodes_inside.remove(t[0])
             bubble = Bubble(source=s, sink=t[0], inside=nodes_inside)
 
             if only_simple:
                 if bubble.is_simple():
                     return bubble
             elif only_super:
-                if bubble.is_super():
-                    return bubble
+                # If it's a bubble and it's not simple or an insertion
+                # then it's marked as super
+                if not bubble.is_simple():
+                    if not bubble.is_insertion():
+                        return bubble
             else:
                 return bubble
 
             # if we already found the same bubble from another direction
             # I don't think I need to check because I'm finding bubbles sequentially
             # but I will investigate this later
```

### Comparing `BubbleGun-1.1.6/BubbleGun/find_parents.py` & `BubbleGun-1.1.7/BubbleGun/find_parents.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/functions.py` & `BubbleGun-1.1.7/BubbleGun/functions.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/graph_io.py` & `BubbleGun-1.1.7/BubbleGun/graph_io.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/json_out.py` & `BubbleGun-1.1.7/BubbleGun/json_out.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/main.py` & `BubbleGun-1.1.7/BubbleGun/main.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/output_certain_chains.py` & `BubbleGun-1.1.7/BubbleGun/output_certain_chains.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun/path_extractor.py` & `BubbleGun-1.1.7/BubbleGun/path_extractor.py`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/BubbleGun.egg-info/PKG-INFO` & `BubbleGun-1.1.7/BubbleGun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BubbleGun
-Version: 1.1.6
+Version: 1.1.7
 Summary: Detection of Bubble and Superbubble chains in genome graphs
 Home-page: https://github.com/fawaz-dabbaghieh/bubble_gun
 Author: Fawaz Dabbaghie
 Author-email: fawaz.dabbaghie@helmholtz-hips.de
 License: LICENSE.TXT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BubbleGun-1.1.6/BubbleGun.egg-info/SOURCES.txt` & `BubbleGun-1.1.7/BubbleGun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/LICENSE` & `BubbleGun-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/PKG-INFO` & `BubbleGun-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BubbleGun
-Version: 1.1.6
+Version: 1.1.7
 Summary: Detection of Bubble and Superbubble chains in genome graphs
 Home-page: https://github.com/fawaz-dabbaghieh/bubble_gun
 Author: Fawaz Dabbaghie
 Author-email: fawaz.dabbaghie@helmholtz-hips.de
 License: LICENSE.TXT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BubbleGun-1.1.6/README.md` & `BubbleGun-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `BubbleGun-1.1.6/setup.py` & `BubbleGun-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write("BubbleGun requires Python 3.3 or higher and "
                      "you current version is {}".format(CURRENT_PYTHON))
     sys.exit(1)
 
 
 setup(name='BubbleGun',
-      version='1.1.6',
+      version='1.1.7',
       description='Detection of Bubble and Superbubble chains in genome graphs',
       author='Fawaz Dabbaghie',
       author_email='fawaz.dabbaghie@helmholtz-hips.de',
       url='https://github.com/fawaz-dabbaghieh/bubble_gun',
       packages=find_packages(),
       # scripts=['bin/main.py'],
       license="LICENSE.TXT",
```

