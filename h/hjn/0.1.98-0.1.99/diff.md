# Comparing `tmp/hjn-0.1.98.tar.gz` & `tmp/hjn-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hjn-0.1.98.tar", last modified: Wed Apr 21 07:32:22 2021, max compression
+gzip compressed data, was "dist/hjn-0.1.99.tar", last modified: Thu Apr 22 05:27:17 2021, max compression
```

## Comparing `hjn-0.1.98.tar` & `hjn-0.1.99.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 07:32:22.000000 hjn-0.1.98/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 07:32:22.000000 hjn-0.1.98/hjn/
--rw-r--r--   0 root         (0) root         (0)    17475 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn/H8mess.py
--rw-r--r--   0 root         (0) root         (0)      171 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6949 2021-04-21 01:37:33.000000 hjn-0.1.98/hjn/examMeso.py
--rw-r--r--   0 root         (0) root         (0)      840 2020-08-27 02:28:00.000000 hjn-0.1.98/hjn/hjnDAA.py
--rw-r--r--   0 root         (0) root         (0)     2916 2020-10-10 07:01:16.000000 hjn-0.1.98/hjn/hjnFTP.py
--rw-r--r--   0 root         (0) root         (0)     8307 2020-12-17 09:10:26.000000 hjn-0.1.98/hjn/hjnGIS.py
--rw-r--r--   0 root         (0) root         (0)     2362 2021-03-30 01:24:36.000000 hjn-0.1.98/hjn/hjnIDW.py
--rw-r--r--   0 root         (0) root         (0)     2395 2020-09-23 07:59:45.000000 hjn-0.1.98/hjn/hjnKDTree.py
--rw-r--r--   0 root         (0) root         (0)     1923 2021-04-15 02:18:27.000000 hjn-0.1.98/hjn/hjnLAPSTransform.py
--rw-r--r--   0 root         (0) root         (0)     3279 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn/hjnProj.py
--rw-r--r--   0 root         (0) root         (0)     1290 2020-11-09 05:27:26.000000 hjn-0.1.98/hjn/inotify.py
--rw-r--r--   0 root         (0) root         (0)     3343 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn/matplotlibMess.py
--rw-r--r--   0 root         (0) root         (0)    17016 2021-04-21 07:32:03.000000 hjn-0.1.98/hjn/mkNCHJN.py
--rw-r--r--   0 root         (0) root         (0)    23449 2020-09-14 01:12:02.000000 hjn-0.1.98/hjn/newTypeRadar.py
--rw-r--r--   0 root         (0) root         (0)       72 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-21 07:32:22.000000 hjn-0.1.98/hjn.egg-info/
--rw-r--r--   0 root         (0) root         (0)      177 2021-04-21 07:32:21.000000 hjn-0.1.98/hjn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      404 2021-04-21 07:32:21.000000 hjn-0.1.98/hjn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-21 07:32:21.000000 hjn-0.1.98/hjn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-07-22 06:07:59.000000 hjn-0.1.98/hjn.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2021-04-21 07:32:21.000000 hjn-0.1.98/hjn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       16 2020-07-22 06:08:00.000000 hjn-0.1.98/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-21 07:32:22.000000 hjn-0.1.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      245 2021-04-21 07:32:16.000000 hjn-0.1.98/setup.py
--rw-r--r--   0 root         (0) root         (0)      177 2021-04-21 07:32:22.000000 hjn-0.1.98/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:27:17.000000 hjn-0.1.99/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn/
+-rw-r--r--   0 root         (0) root         (0)    17475 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn/H8mess.py
+-rw-r--r--   0 root         (0) root         (0)      171 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2021-04-21 01:37:33.000000 hjn-0.1.99/hjn/examMeso.py
+-rw-r--r--   0 root         (0) root         (0)      840 2020-08-27 02:28:00.000000 hjn-0.1.99/hjn/hjnDAA.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2020-10-10 07:01:16.000000 hjn-0.1.99/hjn/hjnFTP.py
+-rw-r--r--   0 root         (0) root         (0)     8307 2020-12-17 09:10:26.000000 hjn-0.1.99/hjn/hjnGIS.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2021-03-30 01:24:36.000000 hjn-0.1.99/hjn/hjnIDW.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2020-09-23 07:59:45.000000 hjn-0.1.99/hjn/hjnKDTree.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2021-04-15 02:18:27.000000 hjn-0.1.99/hjn/hjnLAPSTransform.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn/hjnProj.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2020-11-09 05:27:26.000000 hjn-0.1.99/hjn/inotify.py
+-rw-r--r--   0 root         (0) root         (0)     3343 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn/matplotlibMess.py
+-rw-r--r--   0 root         (0) root         (0)    17131 2021-04-22 05:26:48.000000 hjn-0.1.99/hjn/mkNCHJN.py
+-rw-r--r--   0 root         (0) root         (0)    23449 2020-09-14 01:12:02.000000 hjn-0.1.99/hjn/newTypeRadar.py
+-rw-r--r--   0 root         (0) root         (0)       72 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      177 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      404 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-07-22 06:07:59.000000 hjn-0.1.99/hjn.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2021-04-22 05:27:17.000000 hjn-0.1.99/hjn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2020-07-22 06:08:00.000000 hjn-0.1.99/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-22 05:27:17.000000 hjn-0.1.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      245 2021-04-22 05:27:10.000000 hjn-0.1.99/setup.py
+-rw-r--r--   0 root         (0) root         (0)      177 2021-04-22 05:27:17.000000 hjn-0.1.99/PKG-INFO
```

### Comparing `hjn-0.1.98/hjn/H8mess.py` & `hjn-0.1.99/hjn/H8mess.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/examMeso.py` & `hjn-0.1.99/hjn/examMeso.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnDAA.py` & `hjn-0.1.99/hjn/hjnDAA.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnFTP.py` & `hjn-0.1.99/hjn/hjnFTP.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnGIS.py` & `hjn-0.1.99/hjn/hjnGIS.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnIDW.py` & `hjn-0.1.99/hjn/hjnIDW.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnKDTree.py` & `hjn-0.1.99/hjn/hjnKDTree.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnLAPSTransform.py` & `hjn-0.1.99/hjn/hjnLAPSTransform.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/hjnProj.py` & `hjn-0.1.99/hjn/hjnProj.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/inotify.py` & `hjn-0.1.99/hjn/inotify.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/matplotlibMess.py` & `hjn-0.1.99/hjn/matplotlibMess.py`

 * *Files identical despite different names*

### Comparing `hjn-0.1.98/hjn/mkNCHJN.py` & `hjn-0.1.99/hjn/mkNCHJN.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,32 +109,32 @@
 
 	def __init__(self,data, name, type_,coordinate, unit,missing_value=np.NAN, scale_factor=np.float32(1.0), add_offset=np.float32(0.0),valid_range=[-999,999]):
 		self.data_, self.name_, self.type_, self.coordinate_, self.unit_ ,self.missing_value_ ,self.scale_factor_,self.add_offset_,self.valid_range_= data, name,type_, coordinate, unit,missing_value, scale_factor, add_offset, valid_range
 
 	def print(self):
 		print(self.data_, self.name_, self.type_, self.coordinate_, self.unit_,self.missing_value_,self.scale_factor_,self.add_offset_,self.valid_range_)
 		
-def mkNCCommonUni(output,dateTimeStart,dateTimeArr,isoArr,latArr,lonArr,dataClass4D=[],dataClass3D=[],dataClass2D=[],formate='NETCDF4'):
-    dataset = nc.Dataset(output,'w',format=formate) #'NETCDF4_CLASSIC')
+def mkNCCommonUni(output,dateTimeStart,dateTimeArr,isoArr,latArr,lonArr,dataClass4D=[],dataClass3D=[],dataClass2D=[],format='NETCDF4'):
+    dataset = nc.Dataset(output,'w',format=format) #'NETCDF4_CLASSIC')
     
     try:
         if not dateTimeArr is None and not dateTimeStart is None: 
             dataset.createDimension("time", len(dateTimeArr))
         if not isoArr is None:
             dataset.createDimension("isobaric", len(isoArr))
         
         dataset.createDimension("lat", len(latArr))
         dataset.createDimension("lon", len(lonArr))
     
         if not dateTimeArr is None and not dateTimeStart is None:
             dataset.createVariable("time", np.float32, ("time"), zlib=True)
         if not isoArr is None:
             dataset.createVariable("isobaric", np.float32, ("isobaric"), zlib=True)
-        dataset.createVariable("lat", np.float32, ("lat"), zlib=True)
-        dataset.createVariable("lon", np.float32, ("lon"), zlib=True)
+        dataset.createVariable("lat", np.float64, ("lat"), zlib=True)
+        dataset.createVariable("lon", np.float64, ("lon"), zlib=True)
 
         for e in dataClass2D:
             dataset.createVariable(e.name_, e.type_, tuple(["lat","lon"]), zlib=True)    
 
         for e in dataClass3D:
             dataset.createVariable(e.name_, e.type_, tuple(["time","lat","lon"]), zlib=True)
 
@@ -156,33 +156,36 @@
         dataset.variables["lon"][:] = lonArr
         dataset.variables['lon'].units = 'degrees_east'
         
         for e in dataClass2D:
             dataset.variables[e.name_][:] = e.data_
             dataset.variables[e.name_].units = e.unit_
             dataset.variables[e.name_].valid_range = e.valid_range_
-            dataset.variables[e.name_].coordinate = e.coordinate_
+            if not "3" in format:
+                dataset.variables[e.name_].coordinate = e.coordinate_
             dataset.variables[e.name_].missing_value = e.missing_value_
             dataset.variables[e.name_].scale_factor = e.scale_factor_
             dataset.variables[e.name_].add_offset = e.add_offset_
     
         for e in dataClass3D:
             dataset.variables[e.name_][:] = e.data_
             dataset.variables[e.name_].units = e.unit_
             dataset.variables[e.name_].valid_range = e.valid_range_
-            dataset.variables[e.name_].coordinate = e.coordinate_
+            if not "3" in format:
+                dataset.variables[e.name_].coordinate = e.coordinate_
             dataset.variables[e.name_].missing_value = e.missing_value_
             dataset.variables[e.name_].scale_factor = e.scale_factor_
             dataset.variables[e.name_].add_offset = e.add_offset_
 
         for e in dataClass4D:
             dataset.variables[e.name_][:] = e.data_
             dataset.variables[e.name_].units = e.unit_
             dataset.variables[e.name_].valid_range = e.valid_range_
-            dataset.variables[e.name_].coordinate = e.coordinate_
+            if not "3" in format:
+                dataset.variables[e.name_].coordinate = e.coordinate_
             dataset.variables[e.name_].missing_value = e.missing_value_
             dataset.variables[e.name_].scale_factor = e.scale_factor_
             dataset.variables[e.name_].add_offset = e.add_offset_
 
         #dataset.close()
     except Exception as ex:
         print(ex)
```

### Comparing `hjn-0.1.98/hjn/newTypeRadar.py` & `hjn-0.1.99/hjn/newTypeRadar.py`

 * *Files identical despite different names*

