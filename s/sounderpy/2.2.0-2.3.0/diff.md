# Comparing `tmp/sounderpy-2.2.0.tar.gz` & `tmp/sounderpy-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-2.2.0.tar", last modified: Sun Aug  6 11:08:54 2023, max compression
+gzip compressed data, was "sounderpy-2.3.0.tar", last modified: Sun Aug  6 12:08:33 2023, max compression
```

## Comparing `sounderpy-2.2.0.tar` & `sounderpy-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 11:08:54.241033 sounderpy-2.2.0/
--rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-2.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-08-06 03:45:32.000000 sounderpy-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4908 2023-08-06 11:08:54.236387 sounderpy-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4072 2023-08-06 11:06:16.000000 sounderpy-2.2.0/README.md
--rw-rw-rw-   0        0        0     1070 2023-08-06 11:06:34.000000 sounderpy-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 11:08:54.241033 sounderpy-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      190 2023-08-06 11:06:49.000000 sounderpy-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-06 11:08:54.104099 sounderpy-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 11:08:54.193470 sounderpy-2.2.0/src/sounderpy/
--rw-rw-rw-   0        0        0   685511 2023-08-06 09:20:13.000000 sounderpy-2.2.0/src/sounderpy/BUFKIT-STATIONS-MASTER.txt
--rw-rw-rw-   0        0        0     8527 2023-08-03 16:26:18.000000 sounderpy-2.2.0/src/sounderpy/BUOY-STATIONS.txt
--rw-rw-rw-   0        0        0   213427 2023-08-03 16:26:18.000000 sounderpy-2.2.0/src/sounderpy/IGRA-STATIONS.txt
--rw-rw-rw-   0        0        0   173630 2023-08-03 16:26:18.000000 sounderpy-2.2.0/src/sounderpy/RAOB-STATIONS.txt
--rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-2.2.0/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0      148 2023-07-27 00:32:21.000000 sounderpy-2.2.0/src/sounderpy/requirements.txt
--rw-rw-rw-   0        0        0    71390 2023-08-06 11:04:16.000000 sounderpy-2.2.0/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2023-08-06 11:08:54.233261 sounderpy-2.2.0/src/sounderpy.egg-info/
--rw-rw-rw-   0        0        0     4908 2023-08-06 11:08:53.000000 sounderpy-2.2.0/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-08-06 11:08:53.000000 sounderpy-2.2.0/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 11:08:53.000000 sounderpy-2.2.0/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-08-06 11:08:53.000000 sounderpy-2.2.0/src/sounderpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 11:08:53.000000 sounderpy-2.2.0/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 12:08:33.936563 sounderpy-2.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-2.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       77 2023-08-06 12:05:41.000000 sounderpy-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4908 2023-08-06 12:08:33.929711 sounderpy-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4072 2023-08-06 11:46:48.000000 sounderpy-2.3.0/README.md
+-rw-rw-rw-   0        0        0     1070 2023-08-06 12:06:54.000000 sounderpy-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 12:08:33.936563 sounderpy-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-08-06 12:05:56.000000 sounderpy-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:08:33.800291 sounderpy-2.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 12:08:33.888380 sounderpy-2.3.0/src/sounderpy/
+-rw-rw-rw-   0        0        0   685511 2023-08-06 09:20:13.000000 sounderpy-2.3.0/src/sounderpy/BUFKIT-STATIONS-MASTER.txt
+-rw-rw-rw-   0        0        0     8527 2023-08-03 16:26:18.000000 sounderpy-2.3.0/src/sounderpy/BUOY-STATIONS.txt
+-rw-rw-rw-   0        0        0   213427 2023-08-03 16:26:18.000000 sounderpy-2.3.0/src/sounderpy/IGRA-STATIONS.txt
+-rw-rw-rw-   0        0        0   173630 2023-08-03 16:26:18.000000 sounderpy-2.3.0/src/sounderpy/RAOB-STATIONS.txt
+-rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-2.3.0/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-07-27 00:32:21.000000 sounderpy-2.3.0/src/sounderpy/requirements.txt
+-rw-rw-rw-   0        0        0    71395 2023-08-06 12:06:20.000000 sounderpy-2.3.0/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:08:33.922455 sounderpy-2.3.0/src/sounderpy.egg-info/
+-rw-rw-rw-   0        0        0     4908 2023-08-06 12:08:33.000000 sounderpy-2.3.0/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-08-06 12:08:33.000000 sounderpy-2.3.0/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 12:08:33.000000 sounderpy-2.3.0/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-08-06 12:08:33.000000 sounderpy-2.3.0/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 12:08:33.000000 sounderpy-2.3.0/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-2.2.0/LICENSE.txt` & `sounderpy-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/PKG-INFO` & `sounderpy-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 2.2.0
+Version: 2.3.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
 Author: Kyle J Gillett
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SOUNDERPY DOCUMENTATION 
-  > LATEST VERSION: v2.2.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+  > LATEST VERSION: v2.3.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
 ### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

### Comparing `sounderpy-2.2.0/README.md` & `sounderpy-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SOUNDERPY DOCUMENTATION 
-  > LATEST VERSION: v2.2.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+  > LATEST VERSION: v2.3.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
 ### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

### Comparing `sounderpy-2.2.0/pyproject.toml` & `sounderpy-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "2.2.0"
+version = "2.3.0"
 authors = [
   { name="Kyle J Gillett", email="gille3kj@cmich.edu" },
 ]
 description = "VERTICAL PROFILE DATA RETRIEVAL TOOL"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `sounderpy-2.2.0/src/sounderpy/BUFKIT-STATIONS-MASTER.txt` & `sounderpy-2.3.0/src/sounderpy/BUFKIT-STATIONS-MASTER.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/src/sounderpy/BUOY-STATIONS.txt` & `sounderpy-2.3.0/src/sounderpy/BUOY-STATIONS.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/src/sounderpy/IGRA-STATIONS.txt` & `sounderpy-2.3.0/src/sounderpy/IGRA-STATIONS.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/src/sounderpy/RAOB-STATIONS.txt` & `sounderpy-2.3.0/src/sounderpy/RAOB-STATIONS.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/src/sounderpy/__init__.py` & `sounderpy-2.3.0/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-2.2.0/src/sounderpy/sounderpy.py` & `sounderpy-2.3.0/src/sounderpy/sounderpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 # SIPHON 
 from siphon.catalog import TDSCatalog
 from siphon.ncss import NCSS
 from siphon.simplewebservice.wyoming import WyomingUpperAir
 from siphon.simplewebservice.iastate import IAStateUpperAir
 from siphon.simplewebservice.igra2 import IGRAUpperAir
 
-version = 'v2.2.0'
+version = 'v2.3.0'
 version_date = 'August 6th, 2023'
 
 
 '''
         VERTICAL PROFILE DATA RETRIEVAL TOOL
         ------------------------------------
         This script it used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
         
         RELEASE
         -------
-        Version: 2.2.0 | August 6th, 2023
+        Version: 2.3.0 | August 6th, 2023
         
         DOCUMENTATION
         -------
         GiHub Wiki: https://github.com/kylejgillett/sounderpy/wiki
 
         COPYRIGHT
         ---------
@@ -1344,14 +1344,15 @@
 def bufkit_latlon(bufkit_site):
     
     '''
         takes a BUFKIT site id such as 'KMOP', searches over 1200 station IDs and returns
         a list including the lat/lon for the BUFKIT site
 
     '''
+    
     BUFKIT_STATIONS = pd.read_csv(f'BUFKIT-STATIONS-MASTER.txt', skiprows=7, skipinitialspace = True)
     try:
         station = BUFKIT_STATIONS['ID'][np.where(BUFKIT_STATIONS['ID'].str.contains(bufkit_site, na=False, case=True))[0]].values[0]
 
         lat = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LAT'].values[0])
         lon = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LON'].values[0])
         return [lat, lon]
```

### Comparing `sounderpy-2.2.0/src/sounderpy.egg-info/PKG-INFO` & `sounderpy-2.3.0/src/sounderpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 2.2.0
+Version: 2.3.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
 Author: Kyle J Gillett
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SOUNDERPY DOCUMENTATION 
-  > LATEST VERSION: v2.2.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+  > LATEST VERSION: v2.3.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
 ### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

