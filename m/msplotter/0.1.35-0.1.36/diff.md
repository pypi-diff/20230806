# Comparing `tmp/msplotter-0.1.35.tar.gz` & `tmp/msplotter-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.35.tar", last modified: Fri Aug  4 22:21:07 2023, max compression
+gzip compressed data, was "msplotter-0.1.36.tar", last modified: Sun Aug  6 02:44:17 2023, max compression
```

## Comparing `msplotter-0.1.35.tar` & `msplotter-0.1.36.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 22:21:07.440729 msplotter-0.1.35/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.35/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-04 22:21:07.440097 msplotter-0.1.35/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.35/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-08-04 21:46:47.000000 msplotter-0.1.35/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-08-04 22:21:07.441402 msplotter-0.1.35/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 22:21:07.401501 msplotter-0.1.35/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 22:21:07.413981 msplotter-0.1.35/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.35/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.35/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.35/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5110 2023-07-30 03:41:21.000000 msplotter-0.1.35/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    21163 2023-08-04 22:17:54.000000 msplotter-0.1.35/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 22:21:07.434878 msplotter-0.1.35/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.35/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/Greys.png
--rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.35/src/msp/images/MSPlotter_gui.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.35/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    37472 2023-08-04 20:39:52.000000 msplotter-0.1.35/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.35/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.35/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.35/src/msp/spinbox.py
--rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.35/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-04 22:21:07.439223 msplotter-0.1.35/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      966 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-08-04 22:21:07.000000 msplotter-0.1.35/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.670691 msplotter-0.1.36/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.36/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-06 02:44:17.670177 msplotter-0.1.36/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.36/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-08-06 02:36:21.000000 msplotter-0.1.36/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-08-06 02:44:17.670828 msplotter-0.1.36/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.625776 msplotter-0.1.36/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.633957 msplotter-0.1.36/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.36/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.36/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.36/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5110 2023-07-30 03:41:21.000000 msplotter-0.1.36/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    21163 2023-08-06 02:37:01.000000 msplotter-0.1.36/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.664522 msplotter-0.1.36/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.36/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/Greys.png
+-rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.36/src/msp/images/MSPlotter_gui.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/YlOrRd.png
+-rw-r--r--   0 msp        (501) staff       (20)       35 2023-08-06 02:35:31.000000 msplotter-0.1.36/src/msp/images/__init__.py
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.36/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    37472 2023-08-06 02:38:58.000000 msplotter-0.1.36/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.36/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.36/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.36/src/msp/spinbox.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.666146 msplotter-0.1.36/src/msp/tmp_files/
+-rw-r--r--   0 msp        (501) staff       (20)       69 2023-08-06 02:34:48.000000 msplotter-0.1.36/src/msp/tmp_files/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.36/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-08-06 02:44:17.669491 msplotter-0.1.36/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     1023 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-08-06 02:44:17.000000 msplotter-0.1.36/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.35/LICENSE` & `msplotter-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/PKG-INFO` & `msplotter-0.1.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.35
+Version: 0.1.36
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.35/README.md` & `msplotter-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/pyproject.toml` & `msplotter-0.1.36/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.35"
+version = "0.1.36"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.35/src/msp/arrows.py` & `msplotter-0.1.36/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/colormap_picker.py` & `msplotter-0.1.36/src/msp/colormap_picker.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/gui.py` & `msplotter-0.1.36/src/msp/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,16 +463,16 @@
         self.height_entry.configure(state='normal')
         self.height_entry.delete(0, 'end')
         self.height_entry.configure(state='disabled')
 
     def plot_figure(self):
         """Plot alignments using msplotter."""
         # Make output path for temporary files.
-        # module_path = resources.files(current_module)
-        module_path = Path(current_module.__file__).resolve().parent
+        module_path = resources.files(current_module)
+        # module_path = Path(current_module.__file__).resolve().parent
         path_tmp_files = module_path / "tmp_files"
         # Create fasta files for BLASTing.
         faa_files = msp.make_fasta_files(self.gb_files, path_tmp_files)
         # Run blastn locally.
         xml_results = msp.run_blastn(faa_files, path_tmp_files)
         # Delete fasta files used for BLASTing.
         msp.delete_files(faa_files)
```

### Comparing `msplotter-0.1.35/src/msp/images/Blues.png` & `msplotter-0.1.36/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/BuGn.png` & `msplotter-0.1.36/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/BuPu.png` & `msplotter-0.1.36/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/GnBu.png` & `msplotter-0.1.36/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/Greens.png` & `msplotter-0.1.36/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/MSPlotter_gui.png` & `msplotter-0.1.36/src/msp/images/MSPlotter_gui.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/OrRd.png` & `msplotter-0.1.36/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/Oranges.png` & `msplotter-0.1.36/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/PuBu.png` & `msplotter-0.1.36/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/PuBuGn.png` & `msplotter-0.1.36/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/PuRd.png` & `msplotter-0.1.36/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/Purples.png` & `msplotter-0.1.36/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/RdPu.png` & `msplotter-0.1.36/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/Reds.png` & `msplotter-0.1.36/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/YlGn.png` & `msplotter-0.1.36/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/YlGnBu.png` & `msplotter-0.1.36/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/YlOrBr.png` & `msplotter-0.1.36/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/YlOrRd.png` & `msplotter-0.1.36/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/images/logo.png` & `msplotter-0.1.36/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/msplotter.py` & `msplotter-0.1.36/src/msp/msplotter.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/plot.py` & `msplotter-0.1.36/src/msp/plot.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/slider_widget.py` & `msplotter-0.1.36/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/spinbox.py` & `msplotter-0.1.36/src/msp/spinbox.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msp/user_input.py` & `msplotter-0.1.36/src/msp/user_input.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.35/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.36/src/msplotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.35
+Version: 0.1.36
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.35/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.36/src/msplotter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 src/msp/images/Purples.png
 src/msp/images/RdPu.png
 src/msp/images/Reds.png
 src/msp/images/YlGn.png
 src/msp/images/YlGnBu.png
 src/msp/images/YlOrBr.png
 src/msp/images/YlOrRd.png
+src/msp/images/__init__.py
 src/msp/images/logo.png
+src/msp/tmp_files/__init__.py
 src/msplotter.egg-info/PKG-INFO
 src/msplotter.egg-info/SOURCES.txt
 src/msplotter.egg-info/dependency_links.txt
 src/msplotter.egg-info/entry_points.txt
 src/msplotter.egg-info/requires.txt
 src/msplotter.egg-info/top_level.txt
```

