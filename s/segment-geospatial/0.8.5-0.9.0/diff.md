# Comparing `tmp/segment-geospatial-0.8.5.tar.gz` & `tmp/segment-geospatial-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.8.5.tar", last modified: Wed Jul 19 18:19:36 2023, max compression
+gzip compressed data, was "segment-geospatial-0.9.0.tar", last modified: Sun Aug  6 19:29:17 2023, max compression
```

## Comparing `segment-geospatial-0.8.5.tar` & `segment-geospatial-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:19:36.259652 segment-geospatial-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-19 18:19:36.259652 segment-geospatial-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:19:36.259652 segment-geospatial-0.8.5/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92951 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30749 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/samgeo/samgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    19497 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/samgeo/text_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 18:19:36.259652 segment-geospatial-0.8.5/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 18:19:36.000000 segment-geospatial-0.8.5/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-19 18:19:36.259652 segment-geospatial-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-19 18:19:23.000000 segment-geospatial-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.059663 segment-geospatial-0.9.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96991 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 19:29:17.000000 segment-geospatial-0.9.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 19:29:17.067663 segment-geospatial-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-06 19:29:08.000000 segment-geospatial-0.9.0/setup.py
```

### Comparing `segment-geospatial-0.8.5/LICENSE` & `segment-geospatial-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.8.5/PKG-INFO` & `segment-geospatial-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.5
+Version: 0.9.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -54,18 +54,19 @@
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
--   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting remote sensing imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
--   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Segmenting remote sensing imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting remote sensing imagery with box prompts](https://samgeo.gishub.org/examples/box_prompts)
+-   [Segmenting remote sensing imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
 -   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 -   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
@@ -111,14 +112,16 @@
 
 ## Legal Notice
 
 This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
 
 ## Acknowledgements
 
-This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is based upon work partially supported by the National Aeronautics and Space Administration (NASA) under Grant No. 80NSSC22K1742 issued through the [Open Source Tools, Frameworks, and Libraries 2020 Program](https://bit.ly/3RVBRcQ).
+
+This project is also supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.5/README.md` & `segment-geospatial-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
--   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting remote sensing imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
--   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Segmenting remote sensing imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting remote sensing imagery with box prompts](https://samgeo.gishub.org/examples/box_prompts)
+-   [Segmenting remote sensing imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
 -   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 -   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
@@ -89,14 +90,16 @@
 
 ## Legal Notice
 
 This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
 
 ## Acknowledgements
 
-This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is based upon work partially supported by the National Aeronautics and Space Administration (NASA) under Grant No. 80NSSC22K1742 issued through the [Open Source Tools, Frameworks, and Libraries 2020 Program](https://bit.ly/3RVBRcQ).
+
+This project is also supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.5/samgeo/common.py` & `segment-geospatial-0.9.0/samgeo/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -747,26 +747,117 @@
         print("No valid pixel coordinates found.")
     elif len(result) < len(coords):
         print("Some coordinates are out of the image boundary.")
 
     return result
 
 
+def boxes_to_vector(coords, src_crs, dst_crs="EPSG:4326", output=None, **kwargs):
+    """
+    Convert a list of bounding box coordinates to vector data.
+
+    Args:
+        coords (list): A list of bounding box coordinates in the format [[left, top, right, bottom], [left, top, right, bottom], ...].
+        src_crs (int or str): The EPSG code or proj4 string representing the source coordinate reference system (CRS) of the input coordinates.
+        dst_crs (int or str, optional): The EPSG code or proj4 string representing the destination CRS to reproject the data (default is "EPSG:4326").
+        output (str or None, optional): The full file path (including the directory and filename without the extension) where the vector data should be saved.
+                                       If None (default), the function returns the GeoDataFrame without saving it to a file.
+        **kwargs: Additional keyword arguments to pass to geopandas.GeoDataFrame.to_file() when saving the vector data.
+
+    Returns:
+        geopandas.GeoDataFrame or None: The GeoDataFrame with the converted vector data if output is None, otherwise None if the data is saved to a file.
+    """
+
+    from shapely.geometry import box
+
+    # Create a list of Shapely Polygon objects based on the provided coordinates
+    polygons = [box(*coord) for coord in coords]
+
+    # Create a GeoDataFrame with the Shapely Polygon objects
+    gdf = gpd.GeoDataFrame({"geometry": polygons}, crs=src_crs)
+
+    # Reproject the GeoDataFrame to the specified EPSG code
+    gdf_reprojected = gdf.to_crs(dst_crs)
+
+    if output is not None:
+        gdf_reprojected.to_file(output, **kwargs)
+    else:
+        return gdf_reprojected
+
+
+def rowcol_to_xy(
+    src_fp,
+    rows=None,
+    cols=None,
+    boxes=None,
+    zs=None,
+    offset="center",
+    output=None,
+    dst_crs="EPSG:4326",
+    **kwargs,
+):
+    """Converts a list of (row, col) coordinates to (x, y) coordinates.
+
+    Args:
+        src_fp (str): The source raster file path.
+        rows (list, optional): A list of row coordinates. Defaults to None.
+        cols (list, optional): A list of col coordinates. Defaults to None.
+        boxes (list, optional): A list of (row, col) coordinates in the format of [[left, top, right, bottom], [left, top, right, bottom], ...]
+        zs: zs (list or float, optional): Height associated with coordinates. Primarily used for RPC based coordinate transformations.
+        offset (str, optional): Determines if the returned coordinates are for the center of the pixel or for a corner.
+        output (str, optional): The output vector file path. Defaults to None.
+        dst_crs (str, optional): The destination CRS. Defaults to "EPSG:4326".
+        **kwargs: Additional keyword arguments to pass to rasterio.transform.xy.
+
+    Returns:
+        A list of (x, y) coordinates.
+    """
+
+    if boxes is not None:
+        rows = []
+        cols = []
+
+        for box in boxes:
+            rows.append(box[1])
+            rows.append(box[3])
+            cols.append(box[0])
+            cols.append(box[2])
+
+    if rows is None or cols is None:
+        raise ValueError("rows and cols must be provided.")
+
+    with rasterio.open(src_fp) as src:
+        xs, ys = rasterio.transform.xy(src.transform, rows, cols, zs, offset, **kwargs)
+        src_crs = src.crs
+
+    if boxes is None:
+        return [[x, y] for x, y in zip(xs, ys)]
+    else:
+        result = [[xs[i], ys[i + 1], xs[i + 1], ys[i]] for i in range(0, len(xs), 2)]
+
+        if output is not None:
+            boxes_to_vector(result, src_crs, dst_crs, output)
+        else:
+            return result
+
+
 def bbox_to_xy(
     src_fp: str, coords: list, coord_crs: str = "epsg:4326", **kwargs
 ) -> list:
     """Converts a list of coordinates to pixel coordinates, i.e., (col, row) coordinates.
+        Note that map bbox coords is [minx, miny, maxx, maxy] from bottomleft to topright
+        While rasterio bbox coords is [minx, max, maxx, min] from topleft to bottomright
 
     Args:
         src_fp (str): The source raster file path.
         coords (list): A list of coordinates in the format of [[minx, miny, maxx, maxy], [minx, miny, maxx, maxy], ...]
         coord_crs (str, optional): The coordinate CRS of the input coordinates. Defaults to "epsg:4326".
 
     Returns:
-        list: A list of pixel coordinates in the format of [[minx, miny, maxx, maxy], ...]
+        list: A list of pixel coordinates in the format of [[minx, maxy, maxx, miny], ...] from top left to bottom right.
     """
 
     if isinstance(coords, str):
         gdf = gpd.read_file(coords)
         coords = gdf.geometry.bounds.values.tolist()
         if gdf.crs is not None:
             coord_crs = f"epsg:{gdf.crs.to_epsg()}"
@@ -821,15 +912,17 @@
             and maxx >= 0
             and maxy >= 0
             and minx < width
             and miny < height
             and maxx < width
             and maxy < height
         ):
-            result.append(coord)
+            # Note that map bbox coords is [minx, miny, maxx, maxy] from bottomleft to topright
+            # While rasterio bbox coords is [minx, max, maxx, min] from topleft to bottomright
+            result.append([minx, maxy, maxx, miny])
 
     if len(result) == 0:
         print("No valid pixel coordinates found.")
         return None
     elif len(result) == 1:
         return result[0]
     elif len(result) < len(coords):
@@ -1241,14 +1334,15 @@
         with rasterio.open(source) as src:
             crs = src.crs
             transform = src.transform
             if compress is None:
                 compress = src.compression
 
         # Determine the minimum and maximum values in the array
+
         min_value = np.min(array)
         max_value = np.max(array)
 
         if dtype is None:
             # Determine the best dtype for the array
             if min_value >= 0 and max_value <= 1:
                 dtype = np.float32
```

### Comparing `segment-geospatial-0.8.5/samgeo/samgeo.py` & `segment-geospatial-0.9.0/samgeo/samgeo.py`

 * *Files 22% similar despite different names*

```diff
@@ -482,36 +482,36 @@
         if vector is not None:
             raster_to_vector(output, vector, simplify_tolerance=simplify_tolerance)
 
     def predict(
         self,
         point_coords=None,
         point_labels=None,
-        box=None,
+        boxes=None,
         point_crs=None,
         mask_input=None,
         multimask_output=True,
         return_logits=False,
         output=None,
         index=None,
         mask_multiplier=255,
-        dtype=np.float32,
+        dtype="float32",
         return_results=False,
         **kwargs,
     ):
         """Predict masks for the given input prompts, using the currently set image.
 
         Args:
             point_coords (str | dict | list | np.ndarray, optional): A Nx2 array of point prompts to the
                 model. Each point is in (X,Y) in pixels. It can be a path to a vector file, a GeoJSON
                 dictionary, a list of coordinates [lon, lat], or a numpy array. Defaults to None.
             point_labels (list | int | np.ndarray, optional): A length N array of labels for the
                 point prompts. 1 indicates a foreground point and 0 indicates a background point.
             point_crs (str, optional): The coordinate reference system (CRS) of the point prompts.
-            box (list | np.ndarray, optional): A length 4 array given a box prompt to the
+            boxes (list | np.ndarray, optional): A length 4 array given a box prompt to the
                 model, in XYXY format.
             mask_input (np.ndarray, optional): A low resolution mask input to the model, typically
                 coming from a previous prediction iteration. Has form 1xHxW, where for SAM, H=W=256.
                 multimask_output (bool, optional): If true, the model will return three masks.
                 For ambiguous input prompts (such as a single click), this will often
                 produce better masks than a single prediction. If only a single
                 mask is needed, the model's predicted quality score can be used
@@ -524,64 +524,170 @@
                 which will save the mask with the highest score.
             mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
             dtype (np.dtype, optional): The data type of the output image. Defaults to np.float32.
             return_results (bool, optional): Whether to return the predicted masks, scores, and logits. Defaults to False.
 
         """
 
+        if isinstance(boxes, str):
+            gdf = gpd.read_file(boxes)
+            if gdf.crs is not None:
+                gdf = gdf.to_crs("epsg:4326")
+            boxes = gdf.geometry.bounds.values.tolist()
+        elif isinstance(boxes, dict):
+            import json
+
+            geojson = json.dumps(boxes)
+            gdf = gpd.read_file(geojson, driver="GeoJSON")
+            boxes = gdf.geometry.bounds.values.tolist()
+
         if isinstance(point_coords, str):
             point_coords = vector_to_geojson(point_coords)
 
         if isinstance(point_coords, dict):
             point_coords = geojson_to_coords(point_coords)
 
         if hasattr(self, "point_coords"):
             point_coords = self.point_coords
 
         if hasattr(self, "point_labels"):
             point_labels = self.point_labels
 
-        if point_crs is not None:
+        if (point_crs is not None) and (point_coords is not None):
             point_coords = coords_to_xy(self.source, point_coords, point_crs)
 
         if isinstance(point_coords, list):
             point_coords = np.array(point_coords)
 
-        if point_labels is None:
-            point_labels = [1] * len(point_coords)
-        elif isinstance(point_labels, int):
-            point_labels = [point_labels] * len(point_coords)
+        if point_coords is not None:
+            if point_labels is None:
+                point_labels = [1] * len(point_coords)
+            elif isinstance(point_labels, int):
+                point_labels = [point_labels] * len(point_coords)
 
         if isinstance(point_labels, list):
             if len(point_labels) != len(point_coords):
                 if len(point_labels) == 1:
                     point_labels = point_labels * len(point_coords)
                 else:
                     raise ValueError(
                         "The length of point_labels must be equal to the length of point_coords."
                     )
             point_labels = np.array(point_labels)
 
-        if isinstance(box, list) and point_crs is not None:
-            box = np.array(bbox_to_xy(self.source, box, point_crs))
-
         predictor = self.predictor
-        masks, scores, logits = predictor.predict(
-            point_coords, point_labels, box, mask_input, multimask_output, return_logits
-        )
+
+        input_boxes = None
+        if isinstance(boxes, list) and (point_crs is not None):
+            coords = bbox_to_xy(self.source, boxes, point_crs)
+            input_boxes = np.array(coords)
+            if isinstance(coords[0], int):
+                input_boxes = input_boxes[None, :]
+            else:
+                input_boxes = torch.tensor(input_boxes, device=self.device)
+                input_boxes = predictor.transform.apply_boxes_torch(
+                    input_boxes, self.image.shape[:2]
+                )
+        elif isinstance(boxes, list) and (point_crs is None):
+            input_boxes = np.array(boxes)
+            if isinstance(boxes[0], int):
+                input_boxes = input_boxes[None, :]
+
+        self.boxes = input_boxes
+
+        if boxes is None or (not isinstance(boxes[0], list)):
+            masks, scores, logits = predictor.predict(
+                point_coords,
+                point_labels,
+                input_boxes,
+                mask_input,
+                multimask_output,
+                return_logits,
+            )
+        else:
+            masks, scores, logits = predictor.predict_torch(
+                point_coords=point_coords,
+                point_labels=point_coords,
+                boxes=input_boxes,
+                multimask_output=True,
+            )
+
         self.masks = masks
         self.scores = scores
         self.logits = logits
 
         if output is not None:
-            self.save_prediction(output, index, mask_multiplier, dtype, **kwargs)
+            if boxes is None or (not isinstance(boxes[0], list)):
+                self.save_prediction(output, index, mask_multiplier, dtype, **kwargs)
+            else:
+                self.tensor_to_numpy(
+                    index, output, mask_multiplier, dtype, save_args=kwargs
+                )
 
         if return_results:
             return masks, scores, logits
 
+    def tensor_to_numpy(
+        self, index=None, output=None, mask_multiplier=255, dtype="uint8", save_args={}
+    ):
+        """Convert the predicted masks from tensors to numpy arrays.
+
+        Args:
+            index (index, optional): The index of the mask to save. Defaults to None,
+                which will save the mask with the highest score.
+            output (str, optional): The path to the output image. Defaults to None.
+            mask_multiplier (int, optional): The mask multiplier for the output mask, which is usually a binary mask [0, 1].
+            dtype (np.dtype, optional): The data type of the output image. Defaults to np.uint8.
+            save_args (dict, optional): Optional arguments for saving the output image. Defaults to {}.
+
+        Returns:
+            np.ndarray: The predicted mask as a numpy array.
+        """
+
+        boxes = self.boxes
+        masks = self.masks
+
+        image_pil = self.image
+        image_np = np.array(image_pil)
+
+        if index is None:
+            index = 1
+
+        masks = masks[:, index, :, :]
+        masks = masks.squeeze(1)
+
+        if boxes is None or (len(boxes) == 0):  # No "object" instances found
+            print("No objects found in the image.")
+            return
+        else:
+            # Create an empty image to store the mask overlays
+            mask_overlay = np.zeros_like(
+                image_np[..., 0], dtype=dtype
+            )  # Adjusted for single channel
+
+            for i, (box, mask) in enumerate(zip(boxes, masks)):
+                # Convert tensor to numpy array if necessary and ensure it contains integers
+                if isinstance(mask, torch.Tensor):
+                    mask = (
+                        mask.cpu().numpy().astype(dtype)
+                    )  # If mask is on GPU, use .cpu() before .numpy()
+                mask_overlay += ((mask > 0) * (i + 1)).astype(
+                    dtype
+                )  # Assign a unique value for each mask
+
+            # Normalize mask_overlay to be in [0, 255]
+            mask_overlay = (
+                mask_overlay > 0
+            ) * mask_multiplier  # Binary mask in [0, 255]
+
+        if output is not None:
+            array_to_image(mask_overlay, output, self.source, dtype=dtype, **save_args)
+        else:
+            return mask_overlay
+
     def show_map(self, basemap="SATELLITE", repeat_mode=True, out_dir=None, **kwargs):
         """Show the interactive map.
 
         Args:
             basemap (str, optional): The basemap. It can be one of the following: SATELLITE, ROADMAP, TERRAIN, HYBRID.
             repeat_mode (bool, optional): Whether to use the repeat mode for draw control. Defaults to True.
             out_dir (str, optional): The path to the output directory. Defaults to None.
```

### Comparing `segment-geospatial-0.8.5/samgeo/text_sam.py` & `segment-geospatial-0.9.0/samgeo/text_sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,16 +264,16 @@
             self.source = image
 
             # Load the georeferenced image
             with rasterio.open(image) as src:
                 image_np = src.read().transpose(
                     (1, 2, 0)
                 )  # Convert rasterio image to numpy array
-                transform = src.transform  # Save georeferencing information
-                crs = src.crs  # Save the Coordinate Reference System
+                self.transform = src.transform  # Save georeferencing information
+                self.crs = src.crs  # Save the Coordinate Reference System
                 image_pil = Image.fromarray(
                     image_np[:, :, :3]
                 )  # Convert numpy array to PIL image, excluding the alpha channel
         else:
             image_pil = image
             image_np = np.array(image_pil)
 
@@ -392,14 +392,34 @@
 
         if merge:
             output = os.path.join(out_dir, "merged.tif")
             merge_rasters(out_dir, output)
             if verbose:
                 print(f"Saved the merged prediction to {output}.")
 
+    def save_boxes(self, output=None, dst_crs="EPSG:4326", **kwargs):
+        """Save the bounding boxes to a vector file.
+
+        Args:
+            output (str): The path to the output vector file.
+            dst_crs (str, optional): The destination CRS. Defaults to "EPSG:4326".
+            **kwargs: Additional arguments for boxes_to_vector().
+        """
+
+        if self.boxes is None:
+            print("Please run predict() first.")
+            return
+        else:
+            boxes = self.boxes.tolist()
+            coords = rowcol_to_xy(self.source, boxes=boxes, dst_crs=dst_crs, **kwargs)
+            if output is None:
+                return boxes_to_vector(coords, self.crs, dst_crs, output)
+            else:
+                boxes_to_vector(coords, self.crs, dst_crs, output)
+
     def show_anns(
         self,
         figsize=(12, 10),
         axis="off",
         cmap="viridis",
         alpha=0.4,
         add_boxes=True,
```

### Comparing `segment-geospatial-0.8.5/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.9.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.8.5
+Version: 0.9.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -54,18 +54,19 @@
 -   Load existing markers from vector datasets
 -   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON)
 -   Save input prompts as GeoJSON files
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
--   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
+-   [Segmenting remote sensing imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
--   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
--   [Segmenting imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
+-   [Segmenting remote sensing imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Segmenting remote sensing imagery with box prompts](https://samgeo.gishub.org/examples/box_prompts)
+-   [Segmenting remote sensing imagery with text prompts](https://samgeo.gishub.org/examples/text_prompts)
 -   [Batch segmentation with text prompts](https://samgeo.gishub.org/examples/text_prompts_batch)
 -   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/arcgis)
 -   [Segmenting swimming pools with text prompts](https://samgeo.gishub.org/examples/swimming_pools)
 
 ## Demos
 
 -   Automatic mask generator
@@ -111,14 +112,16 @@
 
 ## Legal Notice
 
 This repository and its content are provided for educational purposes only. By using the information and code provided, users acknowledge that they are using the APIs and models at their own risk and agree to comply with any applicable laws and regulations. Users who intend to download a large number of image tiles from any basemap are advised to contact the basemap provider to obtain permission before doing so. Unauthorized use of the basemap or any of its components may be a violation of copyright laws or other applicable laws and regulations.
 
 ## Acknowledgements
 
-This project is supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
+This project is based upon work partially supported by the National Aeronautics and Space Administration (NASA) under Grant No. 80NSSC22K1742 issued through the [Open Source Tools, Frameworks, and Libraries 2020 Program](https://bit.ly/3RVBRcQ).
+
+This project is also supported by Amazon Web Services ([AWS](https://aws.amazon.com/)). In addition, this package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
 -   [tms2geotiff](https://github.com/gumblex/tms2geotiff)
 -   [GroundingDINO](https://github.com/IDEA-Research/GroundingDINO)
 -   [lang-segment-anything](https://github.com/luca-medeiros/lang-segment-anything)
```

### Comparing `segment-geospatial-0.8.5/setup.py` & `segment-geospatial-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
 
 install_requires = [x.strip() for x in all_reqs if "git+" not in x]
 dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
 
 extras_requires = {
-    "all": ["leafmap", "localtileserver"],
+    "all": ["groundingdino-py"],
 }
 
 requirements = []
 
 setup_requirements = []
 
 test_requirements = []
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.8.5',
+    version='0.9.0',
     zip_safe=False,
 )
```

