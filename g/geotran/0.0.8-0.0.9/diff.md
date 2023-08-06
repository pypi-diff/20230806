# Comparing `tmp/geotran-0.0.8-py3-none-any.whl.zip` & `tmp/geotran-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,9 @@
-Zip file size: 4347 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx        0 b- defN 23-Apr-14 04:19 geotran/__init__.py
--rwxrwxrwx  2.0 unx      628 b- defN 23-Apr-17 02:43 geotran/geofuncs.py
--rwxrwxrwx  2.0 unx     3163 b- defN 23-Apr-28 04:33 geotran/raster.py
--rwxrwxrwx  2.0 unx     1066 b- defN 23-Apr-28 04:34 geotran-0.0.8.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx     1617 b- defN 23-Apr-28 04:34 geotran-0.0.8.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-28 04:34 geotran-0.0.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Apr-28 04:34 geotran-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      611 b- defN 23-Apr-28 04:34 geotran-0.0.8.dist-info/RECORD
-8 files, 7185 bytes uncompressed, 3281 bytes compressed:  54.3%
+Zip file size: 4220 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 00:48 geotran/__init__.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Aug-06 02:34 geotran/raster.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Aug-06 02:41 geotran-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1819 b- defN 23-Aug-06 02:41 geotran-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 02:41 geotran-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-06 02:41 geotran-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      536 b- defN 23-Aug-06 02:41 geotran-0.0.9.dist-info/RECORD
+7 files, 7607 bytes uncompressed, 3268 bytes compressed:  57.0%
```

## zipnote {}

```diff
@@ -1,25 +1,22 @@
 Filename: geotran/__init__.py
 Comment: 
 
-Filename: geotran/geofuncs.py
-Comment: 
-
 Filename: geotran/raster.py
 Comment: 
 
-Filename: geotran-0.0.8.dist-info/LICENSE.txt
+Filename: geotran-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: geotran-0.0.8.dist-info/METADATA
+Filename: geotran-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: geotran-0.0.8.dist-info/WHEEL
+Filename: geotran-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: geotran-0.0.8.dist-info/top_level.txt
+Filename: geotran-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: geotran-0.0.8.dist-info/RECORD
+Filename: geotran-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geotran/raster.py

```diff
@@ -5,30 +5,61 @@
 from rasterio.plot import show_hist
 from rasterio.mask import mask
 from shapely.geometry import Point
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 
-def plot(file):
+from math import radians, cos, sin, asin, sqrt
+import rasterio
+from matplotlib import pyplot
+from rasterio.plot import show
+from rasterio.plot import show_hist
+from rasterio.mask import mask
+from shapely.geometry import Point
+import geopandas as gpd
+import numpy as np
+import pandas as pd
+
+
+def normalise(array):
+    min = np.percentile(array, 0.5)  
+    max = np.percentile(array, 99.5)    
+    norm = (array - min) / (max-min)
+    norm[norm<0.0] = 0.0
+    norm[norm>1.0] = 1.0
+    return norm
+
+def plot(file, bands=(3, 2, 1),cmap='viridis', title='Raster photo',ax=ax):
     src = rasterio.open(file)
-    show(src)
+    if len(bands) == 3:
+        image_data = src.read(bands)
+    elif len(bands) == 1:
+        image_data = src.read(bands)
+    else:
+        raise ValueError("You must provide 1 or 3 bands to display.")
+    image_data[image_data == 65536] = 0.0
+    normalized_data = np.stack([normalise(band) for band in image_data])
+
+    show(normalized_data,cmap=cmap, title=title, ax=ax)
 
 def plot_contour(file):
     src = rasterio.open(file)
     fig, ax = pyplot.subplots(1, figsize=(12, 12))
     show((src, 1), cmap='Greys_r', interpolation='none', ax=ax)
     show((src, 1), contour=True, ax=ax)
     pyplot.show()
 
 def plot_hist(file, bin=50, title="Histogram"):
     src = rasterio.open(file)
     show_hist(
     src, bins=bin, lw=0.0, stacked=False, alpha=0.3,
     histtype='stepfilled', title=title)
+   
+
 
     
 def haversine(lon1: float, lat1: float, lon2: float, lat2: float) -> float:
 
     # Convert decimal degrees to radians
     lon1, lat1, lon2, lat2 = map(radians, [lon1, lat1, lon2, lat2])
```

## Comparing `geotran-0.0.8.dist-info/LICENSE.txt` & `geotran-0.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `geotran-0.0.8.dist-info/METADATA` & `geotran-0.0.9.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotran
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Geospatial Library
 Home-page: https://github.com/tnmthai/geotran
 Author: Thai Tran
 Author-email: tnmthai@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/tnmthai/geotran/issues
 Project-URL: repository, https://github.com/tnmthai/geotran
@@ -21,13 +21,16 @@
 
 Geotran is widely used in the geospatial industry, research, and open-source communities for developing geospatial applications, performing spatial analysis, and modeling complex geospatial phenomena.        
 
 Example:     
 
 ```
 from geotran import raster
+from matplotlib import pyplot
 
-raster.plot('RGB.byte.tif') 
 
-raster.plot_contour('RGB.byte.tif')
+fig, (axr, axg, axb) = pyplot.subplots(1,3, figsize=(21,7))
+
+raster.plot('T60GVV.tif',bands=[3],ax=axr, title="Red", cmap='Reds')
+raster.plot('T60GVV.tif',bands=[2],ax=axg, title="Green", cmap="Greens")
+raster.plot('T60GVV.tif',bands=[1],ax=axb, title="Blue", cmap="Blues")
 
-raster.plot_hist('RGB.byte.tif',100)
```

