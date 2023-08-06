# Comparing `tmp/sounderpy-1.0.1.tar.gz` & `tmp/sounderpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-1.0.1.tar", last modified: Fri Aug  4 20:37:45 2023, max compression
+gzip compressed data, was "sounderpy-2.0.0.tar", last modified: Sun Aug  6 01:42:49 2023, max compression
```

## Comparing `sounderpy-1.0.1.tar` & `sounderpy-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
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
+drwxrwxrwx   0        0        0        0 2023-08-06 01:42:49.138566 sounderpy-2.0.0/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4884 2023-08-06 01:42:49.134436 sounderpy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4072 2023-08-03 23:53:29.000000 sounderpy-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1070 2023-08-06 01:41:05.000000 sounderpy-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 01:42:49.138983 sounderpy-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 01:42:49.061144 sounderpy-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 01:42:49.087299 sounderpy-2.0.0/src/sounderpy/
+-rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-2.0.0/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0    71411 2023-08-06 01:39:54.000000 sounderpy-2.0.0/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2023-08-06 01:42:49.108330 sounderpy-2.0.0/src/sounderpy.egg-info/
+drwxrwxrwx   0        0        0        0 2023-08-06 01:42:49.131436 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     3604 2023-07-27 02:15:00.000000 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-rw-   0        0        0      273 2023-07-27 02:15:00.000000 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:15:00.000000 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-rw-   0        0        0      137 2023-07-27 02:15:00.000000 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 02:15:00.000000 sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-rw-   0        0        0     4884 2023-08-06 01:42:49.000000 sounderpy-2.0.0/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-08-06 01:42:49.000000 sounderpy-2.0.0/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 01:42:49.000000 sounderpy-2.0.0/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-08-06 01:42:49.000000 sounderpy-2.0.0/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 01:42:49.000000 sounderpy-2.0.0/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-1.0.1/LICENSE.txt` & `sounderpy-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/PKG-INFO` & `sounderpy-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 1.0.1
+Version: 2.0.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `sounderpy-1.0.1/README.md` & `sounderpy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/pyproject.toml` & `sounderpy-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "1.0.1"
+version = "2.0.0"
 authors = [
   { name="Kyle J Gillett", email="gille3kj@cmich.edu" },
 ]
 description = "VERTICAL PROFILE DATA RETRIEVAL TOOL"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `sounderpy-1.0.1/src/sounderpy/__init__.py` & `sounderpy-2.0.0/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/src/sounderpy/sounderpy.py` & `sounderpy-2.0.0/src/sounderpy/sounderpy.py`

 * *Files 2% similar despite different names*

```diff
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
+    RAOB_STATIONS = pd.read_csv(f'../RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    IGRA_STATIONS = pd.read_csv(f'../IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
     
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
+    BUFKIT_STATIONS = pd.read_csv(f'../BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
     
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
+    BUFKIT_STATIONS = pd.read_csv(f'../BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
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
+    RAOB_STATIONS = pd.read_csv(f'../RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
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
+    IGRA_STATIONS = pd.read_csv(f'../IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
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
+    BUOY_STATIONS = pd.read_csv('../BUOY-STATIONS.txt', skiprows=7, skipinitialspace = True)
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

### Comparing `sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `sounderpy-2.0.0/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.1/src/sounderpy.egg-info/PKG-INFO` & `sounderpy-2.0.0/src/sounderpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 1.0.1
+Version: 2.0.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/wiki
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `sounderpy-1.0.1/src/sounderpy.egg-info/SOURCES.txt` & `sounderpy-2.0.0/src/sounderpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

