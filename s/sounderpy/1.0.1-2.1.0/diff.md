# Comparing `tmp/sounderpy-1.0.1.tar.gz` & `tmp/sounderpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-1.0.1.tar", last modified: Fri Aug  4 20:37:45 2023, max compression
+gzip compressed data, was "sounderpy-2.1.0.tar", last modified: Sun Aug  6 03:47:04 2023, max compression
```

## Comparing `sounderpy-1.0.1.tar` & `sounderpy-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.830464 sounderpy-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4884 2023-08-04 20:37:45.822953 sounderpy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4072 2023-08-03 23:53:29.000000 sounderpy-1.0.1/README.md
--rw-rw-rw-   0        0        0     1070 2023-08-03 23:48:20.000000 sounderpy-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 20:37:45.830464 sounderpy-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.678139 sounderpy-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.735021 sounderpy-1.0.1/src/sounderpy/
--rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-1.0.1/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0    71924 2023-08-04 00:41:38.000000 sounderpy-1.0.1/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.771072 sounderpy-1.0.1/src/sounderpy.egg-info/
-drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.819707 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     3604 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-rw-rw-   0        0        0      273 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-rw-rw-   0        0        0      137 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-rw-   0        0        0     4884 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 03:47:04.718769 sounderpy-2.1.0/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-08-06 03:45:32.000000 sounderpy-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4904 2023-08-06 03:47:04.714753 sounderpy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4068 2023-08-06 03:26:24.000000 sounderpy-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1070 2023-08-06 03:45:49.000000 sounderpy-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 03:47:04.718769 sounderpy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      190 2023-08-06 03:46:00.000000 sounderpy-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:47:04.614645 sounderpy-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 03:47:04.687145 sounderpy-2.1.0/src/sounderpy/
+-rw-rw-rw-   0        0        0   685511 2023-08-06 03:39:09.000000 sounderpy-2.1.0/src/sounderpy/BUFKIT-STATIONS-MASTER.txt
+-rw-rw-rw-   0        0        0     8527 2023-08-03 16:26:18.000000 sounderpy-2.1.0/src/sounderpy/BUOY-STATIONS.txt
+-rw-rw-rw-   0        0        0   213427 2023-08-03 16:26:18.000000 sounderpy-2.1.0/src/sounderpy/IGRA-STATIONS.txt
+-rw-rw-rw-   0        0        0   173630 2023-08-03 16:26:18.000000 sounderpy-2.1.0/src/sounderpy/RAOB-STATIONS.txt
+-rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-2.1.0/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-07-27 00:32:21.000000 sounderpy-2.1.0/src/sounderpy/requirements.txt
+-rw-rw-rw-   0        0        0    71390 2023-08-06 03:45:14.000000 sounderpy-2.1.0/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2023-08-06 03:47:04.711725 sounderpy-2.1.0/src/sounderpy.egg-info/
+-rw-rw-rw-   0        0        0     4904 2023-08-06 03:47:04.000000 sounderpy-2.1.0/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-08-06 03:47:04.000000 sounderpy-2.1.0/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 03:47:04.000000 sounderpy-2.1.0/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-08-06 03:47:04.000000 sounderpy-2.1.0/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 03:47:04.000000 sounderpy-2.1.0/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-1.0.1/LICENSE.txt` & `sounderpy-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/PKG-INFO` & `sounderpy-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 1.0.1
+Version: 2.1.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
+Author: Kyle J Gillett
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
@@ -14,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SOUNDERPY DOCUMENTATION 
-  > LATEST VERSION: v2.0.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+  > LATEST VERSION: v2 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
 ### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

### Comparing `sounderpy-1.0.1/README.md` & `sounderpy-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SOUNDERPY DOCUMENTATION 
-  > LATEST VERSION: v2.0.0 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+  > LATEST VERSION: v2 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
 
 <div align="center">
 <img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
 ### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

### Comparing `sounderpy-1.0.1/pyproject.toml` & `sounderpy-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "1.0.1"
+version = "2.1.0"
 authors = [
   { name="Kyle J Gillett", email="gille3kj@cmich.edu" },
 ]
 description = "VERTICAL PROFILE DATA RETRIEVAL TOOL"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `sounderpy-1.0.1/src/sounderpy/__init__.py` & `sounderpy-2.1.0/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/src/sounderpy/sounderpy.py` & `sounderpy-2.1.0/src/sounderpy/sounderpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 # SIPHON 
 from siphon.catalog import TDSCatalog
 from siphon.ncss import NCSS
 from siphon.simplewebservice.wyoming import WyomingUpperAir
 from siphon.simplewebservice.iastate import IAStateUpperAir
 from siphon.simplewebservice.igra2 import IGRAUpperAir
 
-version = 'v2.0.0'
+version = 'v2.1.0'
 version_date = 'August 6th, 2023'
 
 
 '''
         VERTICAL PROFILE DATA RETRIEVAL TOOL
         ------------------------------------
         This script it used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
         
         RELEASE
         -------
-        Version: 2.0.0 | August 6th, 2023
+        Version: 2.1.0 | August 6th, 2023
         
         DOCUMENTATION
         -------
         GiHub Wiki: https://github.com/kylejgillett/sounderpy/wiki
 
         COPYRIGHT
         ---------
@@ -91,14 +91,15 @@
     
     global latlon1, source, year1, month1, day1, hour1
     latlon1 = latlon
     year1  = year
     month1 = month
     day1   = day
     hour1  = hour
+    
                  #lat            #lat           #lon               #lon
     latlons = [latlon[0] + .5, latlon[0] - .5, latlon[1] - .5, latlon[1] + .5]
 
     
     
     
     
@@ -356,16 +357,16 @@
     global station1, source, year1, month1, day1, hour1
     source = 'obs'
     station1 = station
     year1  = year
     month1 = month
     day1   = day
     hour1  = hour
-    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
-    IGRA_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    RAOB_STATIONS = pd.read_csv(f'RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    IGRA_STATIONS = pd.read_csv(f'IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
     
     dt = datetime(int(year), int(month), int(day), int(hour)) 
     got_data = False
     
     if RAOB_STATIONS['ICAO'].str.contains(station, na=False, case=True).sum() >= 1:
         for i in range(1, 11):
             try: 
@@ -531,15 +532,15 @@
 
         
     # GET BUFKIT FILE 
     # CONVERT LINES OF BYTES TO STRINGS 
     buf_file = urlopen(data_conn)
     buf_file = [str(line).replace("b'", "").replace("\\r\\n'", "") for line in buf_file]
     
-    BUFKIT_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
+    BUFKIT_STATIONS = pd.read_csv(f'BUFKIT-STATIONS-MASTER.txt', skiprows=7, skipinitialspace = True)
     
     station = BUFKIT_STATIONS['ID'][np.where(BUFKIT_STATIONS['ID'].str.contains(station, na=False, case=True))[0]].values[0]
     
     # Create temp data list and record trigger
     tmp_data, sounding_headers, derived_headers = [], '', ''
     recordSounding = False
     
@@ -1343,15 +1344,15 @@
 def bufkit_latlon(bufkit_site):
     
     '''
         takes a BUFKIT site id such as 'KMOP', searches over 1200 station IDs and returns
         a list including the lat/lon for the BUFKIT site
 
     '''
-    BUFKIT_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
+    BUFKIT_STATIONS = pd.read_csv(f'BUFKIT-STATIONS-MASTER.txt', skiprows=7, skipinitialspace = True)
     try:
         station = BUFKIT_STATIONS['ID'][np.where(BUFKIT_STATIONS['ID'].str.contains(bufkit_site, na=False, case=True))[0]].values[0]
 
         lat = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LAT'].values[0])
         lon = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LON'].values[0])
         return [lat, lon]
     
@@ -1371,15 +1372,15 @@
     '''
     
     def dms2dd(degrees, direction):
         dd = float(degrees)
         if direction == "S" or direction == "W":
             dd *= -1
         return dd
-    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    RAOB_STATIONS = pd.read_csv(f'RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
     try:
         station = RAOB_STATIONS['ICAO'][np.where(RAOB_STATIONS['ICAO'].str.contains(raob_site, na=False, case=True))[0]].values[0]
 
         lat = dms2dd(RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LAT'].values[0], RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['A'].values[0])
         lon = dms2dd(RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LON'].values[0], RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['B'].values[0])
         return [lat, lon]
     
@@ -1398,15 +1399,15 @@
     
     '''
         takes a IGRA2 site id such as 'GMM00010393', searches nearly 3000 station IDs  and returns
         a list including the lat/lon for the IGRA2 site
     '''
     
     
-    IGRA_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    IGRA_STATIONS = pd.read_csv(f'IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
     try:
         station = IGRA_STATIONS['ID'][np.where(IGRA_STATIONS['ID'].str.contains(igra_site, na=False, case=True))[0]].values[0]
 
         lat = np.round(IGRA_STATIONS[IGRA_STATIONS['ID']==station]['LAT'].values[0], 2)
         lon = np.round(IGRA_STATIONS[IGRA_STATIONS['ID']==station]['LON'].values[0], 2)
         return [lat, lon]
     
@@ -1429,15 +1430,15 @@
     '''
 
     def dms2dd(degrees, direction):
         dd = float(degrees)
         if direction == "S" or direction == "W":
             dd *= -1
         return dd
-    BUOY_STATIONS = pd.read_csv('https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUOY-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    BUOY_STATIONS = pd.read_csv('BUOY-STATIONS.txt', skiprows=7, skipinitialspace = True)
     try:
         station = BUOY_STATIONS['ID'][np.where(BUOY_STATIONS['ID'].str.contains(buoy_site, na=False, case=True))[0]].values[0]
 
         lat = dms2dd(BUOY_STATIONS[BUOY_STATIONS['ID']==station]['LAT'].values[0], BUOY_STATIONS[BUOY_STATIONS['ID']==station]['A'].values[0])
         lon = dms2dd(BUOY_STATIONS[BUOY_STATIONS['ID']==station]['LON'].values[0], BUOY_STATIONS[BUOY_STATIONS['ID']==station]['B'].values[0])
         return [lat, lon]
     
@@ -1518,16 +1519,9 @@
     
     
     
     
     
     
     
-    
-    
-    
-    
-    
-    
-
```

### Comparing `sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `sounderpy-2.1.0/src/sounderpy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,97 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 1.0.0
+Version: 2.1.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
+Author: Kyle J Gillett
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
-Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/blob/main/DOCUMENTATION.md
+Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# sounderpy
+# SOUNDERPY DOCUMENTATION 
+  > LATEST VERSION: v2 |  RELEASED: August 6, 2023  |  COPYRIGHT Kyle J Gillett, 2023
+
+<div align="center">
+<img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
 
 ## WELCOME! thank you for visiting SounderPy!
+### [VISIT SOUNDERPY DOCUMENTATION HERE](https://github.com/kylejgillett/sounderpy/wiki)
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding). 
 
-Thank you for visiting SounderPy.
+[![PyPI Package](https://img.shields.io/pypi/v/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://github.com/kylejgillett/sounderpy/blob/main/LICENSE.txt)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/sounderpy.svg)](https://pypi.python.org/pypi/sounderpy/)
+[![GitHub commits](https://badgen.net/github/commits/kylejgillett/sounderpy)](https://GitHub.com/kylejgillett/sounderpy/commit/)
+[![Maintainer](https://img.shields.io/badge/maintainer-kylejgillett-blue)](https://github.com/kylejgillett)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
-### Why SounderPy?
-+ Sometimes data is tough to find, and often times is even tougher to get in the format you like. SounderPy gets you this data!
-+ The code needed for loading and parsing vertical data (especially from models) can be large and messy. SounderPy keeps it hidden away in a separate file -- just import and call sounderPy functions to keep your code clean!
-
-## SounderPy is used for:
-- Accessing and loading raw vertical profile data from the sources listed above
-- Parsing these raw data into a clean & simple-to-use format for calculations and plotting
-- SounderPy offers a built-in quick MetPy plotting function, but sounderPy itself is meant as a source for accessing data -- not for plotting (that may be a future package ;) )
--------
+</div>
+
+
+
+-----
+## What is SounderPy:
+
+- SounderPy is a Python package used to access vertical profile data for calculations or plotting of a vertical profile (sounding). SounderPy's main use is for getting the data, but some basic plotting tools are included.
 
 ## SounderPy is currently capable of accessing and processing data from:
+
 - ECMWF CDS ERA5 reanalysis [1940-present] *note: you must set up an account through the CDS to unlock ERA5 data. (see: https://cds.climate.copernicus.eu/api-how-to)
 - UNIDATA THREDDS TDS RAP reanalysis [2005-present]
 - UNIDATA THREDDS TDS RUC reanalysis [2005-2020]
 - The University of Wyoming RAOB archive [1973-present, depending on station]
 - Iowa State University's RAOB archive [1945-present, depending on station]
+- The IGRAv2 Observed profile archive [1905-present, depending on station]
+- Iowa State University's BUFKIT archive [2011-present, depending on station & model]
+- Penn State University's BUFKIT archive [most-recent run, depending on station & model]
+- UNIDATA THREDDS TDS RAP-most-recent-analysis [now, most recent analysis only]
+
+## Why SounderPy?
+- Sometimes data is tough to find, and often times is even tougher to get it in the format you like. SounderPy gets you this data!
+- The code needed for loading and parsing vertical data (especially from models) can be large and messy. SounderPy keeps it hidden away in a PyPi package -- just import and call sounderPy functions to keep your code clean!
+
 -------
+
 ## How to use SounderPy:
 1. Make sure your environment has the required dependencies:
-   -  metpy
-   -  xarray
-   -  urllib
-   -  numpy
-   -  siphon
-   -  cartopy
-   -  datetime
-   -  cdsapi
-   -  pandas
+   - cdsapi>=0.6.1
+   - matplotlib>=3.3.0, <=3.7.1
+   - metpy>=1.5.1
+   - netcdf4>=1.6.4
+   - numpy>=1.20.0
+   - pandas>=1.2.0
+   - siphon>=0.9
+   - scipy>= 1.10.1
+   - xarray>=0.18.0
+
 2. ```
    pip install sounderpy
    ```
+   Find it at https://pypi.org/project/sounderpy/2.0.0/
 3. ```
    import sounderpy as spy
    ```
 4. ```
-   year  = '2014'
-   month = '06'
-   day   = '16'
-   hour  = '20'
-   latlon = [41.9, -97.01]
+   year  = '2011'
+   month = '04'
+   day   = '27'
+   hour  = '22'
+   latlon = [33.19, -87.46]
    method = 'rap'
    ```
 5. ```
    raw_data = spy.get_model_data(method, latlon, year, month, day, hour)
    ```
 6. ```
    clean_data = spy.parse_data(raw_data)
@@ -85,12 +109,7 @@
 9. V-component Wind
 
 You can make a quick plot of the data using built-in MetPy plotting functions!, just call...
 `spy.metpy_sounding(clean_data)`
 <div align="center">
 <img src="https://raw.githubusercontent.com/kylejgillett/sounderpy/main/images/example_RAP_0427201122z.png" width="600">
 </div>
-<br>
-<br>
-<div align="center">
-<img src="https://github.com/kylejgillett/sounderpy/assets/100786530/2e9477c9-e36a-4163-accb-fe46780058dd" width="250">
-</div>
```

