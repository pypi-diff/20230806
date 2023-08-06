# Comparing `tmp/networkx-gdf-1.0.tar.gz` & `tmp/networkx-gdf-1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkx-gdf-1.0.tar", last modified: Sun Aug  6 18:23:58 2023, max compression
+gzip compressed data, was "networkx-gdf-1.0.post1.tar", last modified: Sun Aug  6 18:39:22 2023, max compression
```

## Comparing `networkx-gdf-1.0.tar` & `networkx-gdf-1.0.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-08-06 18:23:58.239263 networkx-gdf-1.0/
--rw-r--r--   0 neo       (1000) neo       (1000)     1101 2023-08-05 12:26:45.000000 networkx-gdf-1.0/LICENSE.md
--rw-r--r--   0 neo       (1000) neo       (1000)     3533 2023-08-06 18:23:58.239263 networkx-gdf-1.0/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)     2622 2023-08-06 17:44:28.000000 networkx-gdf-1.0/README.md
-drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-08-06 18:23:58.239263 networkx-gdf-1.0/networkx_gdf.egg-info/
--rw-r--r--   0 neo       (1000) neo       (1000)     3533 2023-08-06 18:23:58.000000 networkx-gdf-1.0/networkx_gdf.egg-info/PKG-INFO
--rw-r--r--   0 neo       (1000) neo       (1000)      224 2023-08-06 18:23:58.000000 networkx-gdf-1.0/networkx_gdf.egg-info/SOURCES.txt
--rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-08-06 18:23:58.000000 networkx-gdf-1.0/networkx_gdf.egg-info/dependency_links.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       28 2023-08-06 18:23:58.000000 networkx-gdf-1.0/networkx_gdf.egg-info/requires.txt
--rw-r--r--   0 neo       (1000) neo       (1000)       13 2023-08-06 18:23:58.000000 networkx-gdf-1.0/networkx_gdf.egg-info/top_level.txt
--rw-r--r--   0 neo       (1000) neo       (1000)     5178 2023-08-06 17:43:41.000000 networkx-gdf-1.0/networkx_gdf.py
--rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-08-06 18:23:58.240263 networkx-gdf-1.0/setup.cfg
--rw-r--r--   0 neo       (1000) neo       (1000)     1311 2023-08-06 17:46:52.000000 networkx-gdf-1.0/setup.py
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-08-06 18:39:22.454875 networkx-gdf-1.0.post1/
+-rw-r--r--   0 neo       (1000) neo       (1000)     1101 2023-08-05 12:26:45.000000 networkx-gdf-1.0.post1/LICENSE.md
+-rw-r--r--   0 neo       (1000) neo       (1000)     3533 2023-08-06 18:39:22.454875 networkx-gdf-1.0.post1/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)     2616 2023-08-06 18:37:52.000000 networkx-gdf-1.0.post1/README.md
+drwxr-xr-x   0 neo       (1000) neo       (1000)        0 2023-08-06 18:39:22.454875 networkx-gdf-1.0.post1/networkx_gdf.egg-info/
+-rw-r--r--   0 neo       (1000) neo       (1000)     3533 2023-08-06 18:39:22.000000 networkx-gdf-1.0.post1/networkx_gdf.egg-info/PKG-INFO
+-rw-r--r--   0 neo       (1000) neo       (1000)      224 2023-08-06 18:39:22.000000 networkx-gdf-1.0.post1/networkx_gdf.egg-info/SOURCES.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)        1 2023-08-06 18:39:22.000000 networkx-gdf-1.0.post1/networkx_gdf.egg-info/dependency_links.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       28 2023-08-06 18:39:22.000000 networkx-gdf-1.0.post1/networkx_gdf.egg-info/requires.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)       13 2023-08-06 18:39:22.000000 networkx-gdf-1.0.post1/networkx_gdf.egg-info/top_level.txt
+-rw-r--r--   0 neo       (1000) neo       (1000)     5178 2023-08-06 17:43:41.000000 networkx-gdf-1.0.post1/networkx_gdf.py
+-rw-r--r--   0 neo       (1000) neo       (1000)       38 2023-08-06 18:39:22.455875 networkx-gdf-1.0.post1/setup.cfg
+-rw-r--r--   0 neo       (1000) neo       (1000)     1317 2023-08-06 18:34:14.000000 networkx-gdf-1.0.post1/setup.py
```

### Comparing `networkx-gdf-1.0/LICENSE.md` & `networkx-gdf-1.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networkx-gdf-1.0/PKG-INFO` & `networkx-gdf-1.0.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx-gdf
-Version: 1.0
+Version: 1.0.post1
 Summary: Python package to read and write NetworkX graphs as GDF (Graph Data Format).
 Home-page: https://github.com/nelsonaloysio/networkx-gdf
 Author: Nelson Aloysio Reis de Almeida Passos
 License: MIT
 Project-URL: Source, https://github.com/nelsonaloysio/networkx-gdf
 Project-URL: Tracker, https://github.com/nelsonaloysio/networkx-gdf/issues
 Keywords: Network,Graph,GDF
@@ -19,39 +19,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # networkx-gdf
 
 Python package to read and write NetworkX graphs as GDF (Graph Data Format).
 
-### Requirements
+## Requirements
 
 * **Python>=3.7**
 * networkx>=2.1
 * pandas>=1.1.0
 
-### Usage
+## Usage
 
 Just two functions are implemented, for reading from and writing data to file.
 
 ```
 from networkx_gdf import read_gdf, write_gdf
 
 # Builds NetworkX graph object from file.
 G = read_gdf("input_file.gdf")
 
 # Writes NetworkX graph object to file.
 write_gdf(G, "output_file.gdf)
 ```
 
-#### Detailed usage
+### Detailed usage
 
 A few additional arguments are available both for reading and writing files:
 
-##### Building NetworkX graph object from file
+#### Building NetworkX graph object from file
 
 ```
 G = read_gdf(
     "input_file.gdf",
     # Required; file path to read data from.
 
     directed=None,
@@ -74,23 +74,23 @@
     edge_attr=True,
     # Optional; edge attributes to import data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all edge attributes.
 )
 ```
 
-##### Writing NetworkX graph object to file
+#### Writing NetworkX graph object to file
 
 ```
 write_gdf(
     G,
     # Required; graph object from NetworkX.
 
     "output_file.gdf",
-    # Required; file path to read data from.
+    # Required; file path to write data to.
 
     node_attr=True,
     # Optional; node attributes to export data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all node attributes.
 
     edge_attr=True,
@@ -109,11 +109,12 @@
 
 class MyClass(GDF):
     ...
 ```
 
 ___
 
-### References
+References
+---
 
 * [NetworkX](https://networkx.github.io)
 * [Pandas](https://pandas.pydata.org/)
```

### Comparing `networkx-gdf-1.0/README.md` & `networkx-gdf-1.0.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # networkx-gdf
 
 Python package to read and write NetworkX graphs as GDF (Graph Data Format).
 
-### Requirements
+## Requirements
 
 * **Python>=3.7**
 * networkx>=2.1
 * pandas>=1.1.0
 
-### Usage
+## Usage
 
 Just two functions are implemented, for reading from and writing data to file.
 
 ```
 from networkx_gdf import read_gdf, write_gdf
 
 # Builds NetworkX graph object from file.
 G = read_gdf("input_file.gdf")
 
 # Writes NetworkX graph object to file.
 write_gdf(G, "output_file.gdf)
 ```
 
-#### Detailed usage
+### Detailed usage
 
 A few additional arguments are available both for reading and writing files:
 
-##### Building NetworkX graph object from file
+#### Building NetworkX graph object from file
 
 ```
 G = read_gdf(
     "input_file.gdf",
     # Required; file path to read data from.
 
     directed=None,
@@ -53,23 +53,23 @@
     edge_attr=True,
     # Optional; edge attributes to import data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all edge attributes.
 )
 ```
 
-##### Writing NetworkX graph object to file
+#### Writing NetworkX graph object to file
 
 ```
 write_gdf(
     G,
     # Required; graph object from NetworkX.
 
     "output_file.gdf",
-    # Required; file path to read data from.
+    # Required; file path to write data to.
 
     node_attr=True,
     # Optional; node attributes to export data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all node attributes.
 
     edge_attr=True,
@@ -88,11 +88,12 @@
 
 class MyClass(GDF):
     ...
 ```
 
 ___
 
-### References
+References
+---
 
 * [NetworkX](https://networkx.github.io)
 * [Pandas](https://pandas.pydata.org/)
```

### Comparing `networkx-gdf-1.0/networkx_gdf.egg-info/PKG-INFO` & `networkx-gdf-1.0.post1/networkx_gdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx-gdf
-Version: 1.0
+Version: 1.0.post1
 Summary: Python package to read and write NetworkX graphs as GDF (Graph Data Format).
 Home-page: https://github.com/nelsonaloysio/networkx-gdf
 Author: Nelson Aloysio Reis de Almeida Passos
 License: MIT
 Project-URL: Source, https://github.com/nelsonaloysio/networkx-gdf
 Project-URL: Tracker, https://github.com/nelsonaloysio/networkx-gdf/issues
 Keywords: Network,Graph,GDF
@@ -19,39 +19,39 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # networkx-gdf
 
 Python package to read and write NetworkX graphs as GDF (Graph Data Format).
 
-### Requirements
+## Requirements
 
 * **Python>=3.7**
 * networkx>=2.1
 * pandas>=1.1.0
 
-### Usage
+## Usage
 
 Just two functions are implemented, for reading from and writing data to file.
 
 ```
 from networkx_gdf import read_gdf, write_gdf
 
 # Builds NetworkX graph object from file.
 G = read_gdf("input_file.gdf")
 
 # Writes NetworkX graph object to file.
 write_gdf(G, "output_file.gdf)
 ```
 
-#### Detailed usage
+### Detailed usage
 
 A few additional arguments are available both for reading and writing files:
 
-##### Building NetworkX graph object from file
+#### Building NetworkX graph object from file
 
 ```
 G = read_gdf(
     "input_file.gdf",
     # Required; file path to read data from.
 
     directed=None,
@@ -74,23 +74,23 @@
     edge_attr=True,
     # Optional; edge attributes to import data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all edge attributes.
 )
 ```
 
-##### Writing NetworkX graph object to file
+#### Writing NetworkX graph object to file
 
 ```
 write_gdf(
     G,
     # Required; graph object from NetworkX.
 
     "output_file.gdf",
-    # Required; file path to read data from.
+    # Required; file path to write data to.
 
     node_attr=True,
     # Optional; node attributes to export data from.
     # Accepts either a [list] containing attribute names or a bool (True, False).
     # Defaults to True, which considers all node attributes.
 
     edge_attr=True,
@@ -109,11 +109,12 @@
 
 class MyClass(GDF):
     ...
 ```
 
 ___
 
-### References
+References
+---
 
 * [NetworkX](https://networkx.github.io)
 * [Pandas](https://pandas.pydata.org/)
```

### Comparing `networkx-gdf-1.0/networkx_gdf.py` & `networkx-gdf-1.0.post1/networkx_gdf.py`

 * *Files identical despite different names*

### Comparing `networkx-gdf-1.0/setup.py` & `networkx-gdf-1.0.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name="networkx-gdf",
-    version="1.0",
+    version="1.0.post1",
     description=description.strip(),
     long_description=long_description,
     install_requires=install_requires,
     url="https://github.com/nelsonaloysio/networkx-gdf",
     author="Nelson Aloysio Reis de Almeida Passos",
     long_description_content_type="text/markdown",
     license="MIT",
```

