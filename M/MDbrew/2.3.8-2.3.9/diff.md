# Comparing `tmp/MDbrew-2.3.8.tar.gz` & `tmp/MDbrew-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.8.tar", last modified: Wed Jul 26 14:46:40 2023, max compression
+gzip compressed data, was "MDbrew-2.3.9.tar", last modified: Sat Jul 29 07:02:12 2023, max compression
```

## Comparing `MDbrew-2.3.8.tar` & `MDbrew-2.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799761 MDbrew-2.3.8/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.8/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.796117 MDbrew-2.3.8/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      182 2023-07-26 14:46:38.000000 MDbrew-2.3.8/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.797358 MDbrew-2.3.8/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     5594 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.797679 MDbrew-2.3.8/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)       20 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10136 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/application/cp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.798230 MDbrew-2.3.8/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5772 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799073 MDbrew-2.3.8/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      940 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      974 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)     1304 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4427 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     2959 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)     1226 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1695 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/opener.py
--rw-r--r--   0 minu       (501) staff       (20)     1353 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/main/writer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.799643 MDbrew-2.3.8/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1579 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      765 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      695 2023-07-26 14:45:56.000000 MDbrew-2.3.8/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-26 14:46:40.796925 MDbrew-2.3.8/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      758 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-26 14:46:29.000000 MDbrew-2.3.8/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-07-26 14:46:40.000000 MDbrew-2.3.8/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-26 14:46:40.799815 MDbrew-2.3.8/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.8/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-07-26 14:46:40.800009 MDbrew-2.3.8/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      665 2023-07-26 14:46:11.000000 MDbrew-2.3.8/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.197527 MDbrew-2.3.9/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.9/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.193940 MDbrew-2.3.9/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      182 2023-07-29 07:01:34.000000 MDbrew-2.3.9/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.195011 MDbrew-2.3.9/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     6160 2023-07-29 07:01:19.000000 MDbrew-2.3.9/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.195297 MDbrew-2.3.9/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       20 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10136 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/application/cp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.195782 MDbrew-2.3.9/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5772 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.196627 MDbrew-2.3.9/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      974 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)     1304 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4427 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     2959 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)     1226 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1695 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/opener.py
+-rw-r--r--   0 minu       (501) staff       (20)     1353 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/main/writer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.197317 MDbrew-2.3.9/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1579 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      765 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      695 2023-07-26 14:45:56.000000 MDbrew-2.3.9/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-07-29 07:02:12.194629 MDbrew-2.3.9/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-29 07:02:12.000000 MDbrew-2.3.9/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      758 2023-07-29 07:02:12.000000 MDbrew-2.3.9/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-29 07:02:12.000000 MDbrew-2.3.9/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-07-26 14:46:29.000000 MDbrew-2.3.9/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-07-29 07:02:12.000000 MDbrew-2.3.9/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-07-29 07:02:12.197599 MDbrew-2.3.9/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.9/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-07-29 07:02:12.197823 MDbrew-2.3.9/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      665 2023-07-29 07:02:09.000000 MDbrew-2.3.9/setup.py
```

### Comparing `MDbrew-2.3.8/MDbrew/analysis/msd.py` & `MDbrew-2.3.9/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/analysis/rdf.py` & `MDbrew-2.3.9/MDbrew/analysis/rdf.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 from ..main.brewery import Brewery
 from ..tool.spacer import *
 from ..tool.colorfont import color
 
 
 # Calculate and Plot the RDF
 class RDF(object):
-    def __init__(self, a, b, box=None, r_max: float = None, resolution: int = 1000, dtype: str = "float64"):
+    def __init__(
+        self,
+        a,
+        b,
+        box=None,
+        r_max: float = None,
+        resolution: int = 1000,
+        dtype: str = "float64",
+    ):
         if type(a) == Brewery:
             self.instance_rdf = BreweryRDF(a=a, b=b, box=box, r_max=r_max, resolution=resolution, dtype=dtype)
         else:
             self.instance_rdf = NormalRDF(a=a, b=b, box=box, r_max=r_max, resolution=resolution, dtype=dtype)
 
     def run(self, start=0, end=None, step=1):
         self.instance_rdf._main_run(start=start, end=end, step=step)
@@ -41,15 +49,23 @@
         "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}RDF{color.reset} ",
         "ncols": 60,
         "ascii": True,
     }
     hist_data = None
     radii = None
 
-    def __init__(self, a, b, box=None, r_max: float = None, resolution: int = 1000, dtype: str = "float64"):
+    def __init__(
+        self,
+        a,
+        b,
+        box=None,
+        r_max: float = None,
+        resolution: int = 1000,
+        dtype: str = "float64",
+    ):
         self.r_max = np.max(self.box) * 0.5 if r_max is None else r_max
         self.resolution = resolution
         self._dtype = dtype
 
     def _main_run(self, start=0, end=None, step=1):
         pass
 
@@ -76,44 +92,68 @@
     # Function for get coordinate number
     def _cal_cn(self):
         self.n = self.hist_data / (self.frame_num * self.a_number)
         return np.cumsum(self.n)
 
 
 class BreweryRDF(InterfaceRDF):
-    def __init__(self, a, b, box=None, r_max: float = None, resolution: int = 1000, dtype: str = "float64"):
+    def __init__(
+        self,
+        a,
+        b,
+        box=None,
+        r_max: float = None,
+        resolution: int = 1000,
+        dtype: str = "float64",
+    ):
         self.a: Brewery = a.reorder()
         self.b: Brewery = b.reorder()
         self.a_number = a.atom_num
         self.b_number = b.atom_num
+        self._is_external_box = box is None
         self.box = a.box_size if box is None else box
         assert len(self.box), "plz set box"
         super().__init__(self.a, self.b, self.box, r_max, resolution, dtype)
 
     def _main_run(self, start=0, end=None, step=1):
         self.frame_num = 0
         self.gr = np.zeros(self.resolution)
         self.hist_data = np.zeros(self.resolution)
         frange = self._make_frange(start=start, end=end, step=step)
-        for _ in tqdm(frange, **self.kwrgs_trange):
+        for idx in tqdm(frange, **self.kwrgs_trange):
             a_unit = self.a.coords
             b_unit = self.b.coords
-            box_unit = np.array(self.a.box_size)
+            box_unit = self._make_box(self.box, idx)
             self._unit_run(a_unit=a_unit, b_unit=b_unit, box_unit=box_unit)
 
     def _make_frange(self, start=0, end=None, step=1):
         kwrgs = {"start": start, "end": end, "step": step}
         if self.a is self.b:
             return self.a.frange(**kwrgs)
         else:
             return zip(self.a.frange(**kwrgs), self.b.frange(**kwrgs))
 
+    def _make_box(self, box, idx):
+        if self._is_external_box:
+            return np.array(self.a.box_size)
+        else:
+            box = np.array([box])
+            return box if box.shape[0] == 1 else box[0][idx]
+
 
 class NormalRDF(InterfaceRDF):
-    def __init__(self, a, b, box=None, r_max: float = None, resolution: int = 1000, dtype: str = "float64"):
+    def __init__(
+        self,
+        a,
+        b,
+        box=None,
+        r_max: float = None,
+        resolution: int = 1000,
+        dtype: str = "float64",
+    ):
         self.a = check_dimension(a, dim=3, dtype=dtype)
         self.b = check_dimension(b, dim=3, dtype=dtype)
         self.a_number = self.a.shape[1]
         self.b_number = self.b.shape[1]
         self.box = self._make_box(box=box)
         super().__init__(a, b, box, r_max, resolution, dtype)
```

### Comparing `MDbrew-2.3.8/MDbrew/application/cp2k.py` & `MDbrew-2.3.9/MDbrew/application/cp2k.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/brewery.py` & `MDbrew-2.3.9/MDbrew/main/brewery.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/gro.py` & `MDbrew-2.3.9/MDbrew/main/filetype/gro.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.9/MDbrew/main/filetype/lmps.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.9/MDbrew/main/filetype/pdb.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/trr.py` & `MDbrew-2.3.9/MDbrew/main/filetype/trr.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.9/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/filetype/xyz.py` & `MDbrew-2.3.9/MDbrew/main/filetype/xyz.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/opener.py` & `MDbrew-2.3.9/MDbrew/main/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/main/writer.py` & `MDbrew-2.3.9/MDbrew/main/writer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/tool/colorfont.py` & `MDbrew-2.3.9/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/tool/decorator.py` & `MDbrew-2.3.9/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/tool/doctor.py` & `MDbrew-2.3.9/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew/tool/spacer.py` & `MDbrew-2.3.9/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.9/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.8/setup.py` & `MDbrew-2.3.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.8",
+    version="2.3.9",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.8.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.9.tar.gz",
     install_requies=[
         "numpy>=1.19.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
```

