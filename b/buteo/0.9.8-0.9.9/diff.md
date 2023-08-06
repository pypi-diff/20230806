# Comparing `tmp/buteo-0.9.8.tar.gz` & `tmp/buteo-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buteo-0.9.8.tar", last modified: Fri May 12 13:35:34 2023, max compression
+gzip compressed data, was "buteo-0.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `buteo-0.9.8.tar` & `buteo-0.9.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.8/LICENSE
--rw-r--r--   0        0        0     4779 2023-05-09 11:35:41.351219 buteo-0.9.8/buteo/__init__.py
--rw-r--r--   0        0        0      222 2023-05-09 11:50:06.491154 buteo-0.9.8/buteo/ai/__init__.py
--rw-r--r--   0        0        0     9723 2023-05-12 11:16:29.988305 buteo-0.9.8/buteo/ai/augmentation.py
--rw-r--r--   0        0        0    28002 2023-05-09 12:27:55.018873 buteo-0.9.8/buteo/ai/augmentation_funcs.py
--rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.8/buteo/ai/augmentation_utils.py
--rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.8/buteo/ai/encoding.py
--rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.8/buteo/ai/scalers.py
--rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.8/buteo/ai/selection.py
--rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.8/buteo/array/__init__.py
--rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.8/buteo/array/color.py
--rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.8/buteo/array/convolution.py
--rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.8/buteo/array/convolution_distance.py
--rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.8/buteo/array/convolution_funcs.py
--rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.8/buteo/array/convolution_kernels.py
--rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.8/buteo/array/edge_detection.py
--rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.8/buteo/array/fill.py
--rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.8/buteo/array/filters.py
--rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.8/buteo/array/morphology.py
--rw-r--r--   0        0        0    31384 2023-05-12 13:33:23.446975 buteo-0.9.8/buteo/array/patches.py
--rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.8/buteo/array/timeseries.py
--rw-r--r--   0        0        0     2819 2023-05-09 11:52:21.206628 buteo-0.9.8/buteo/array/utils_array.py
--rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.8/buteo/eo/__init__.py
--rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/L2A_GIPP.xml
--rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_01_backstatter.xml
--rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_01_coherence.xml
--rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_backscatter.xml
--rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_backscatter_speckle.xml
--rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_coherence.xml
--rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.8/buteo/eo/s1_preprocess.py
--rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.8/buteo/eo/s1_utils.py
--rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.8/buteo/eo/s2_indices.py
--rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.8/buteo/eo/s2_utils.py
--rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.8/buteo/raster/__init__.py
--rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.8/buteo/raster/align.py
--rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.8/buteo/raster/borders.py
--rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.8/buteo/raster/clip.py
--rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.8/buteo/raster/coordinates.py
--rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.8/buteo/raster/core_offsets.py
--rw-r--r--   0        0        0    18432 2023-05-10 07:50:31.889375 buteo-0.9.8/buteo/raster/core_raster.py
--rw-r--r--   0        0        0    37055 2023-05-12 11:11:07.920206 buteo-0.9.8/buteo/raster/core_raster_io.py
--rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.8/buteo/raster/core_stack.py
--rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.8/buteo/raster/datatype.py
--rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.8/buteo/raster/dem.py
--rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.8/buteo/raster/grid.py
--rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.8/buteo/raster/metadata.py
--rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.8/buteo/raster/nodata.py
--rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.8/buteo/raster/proximity.py
--rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.8/buteo/raster/reproject.py
--rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.8/buteo/raster/resample.py
--rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.8/buteo/raster/shift.py
--rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.8/buteo/raster/vectorize.py
--rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.8/buteo/utils/__init__.py
--rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.8/buteo/utils/utils_aux.py
--rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.8/buteo/utils/utils_base.py
--rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.8/buteo/utils/utils_bbox.py
--rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.8/buteo/utils/utils_gdal.py
--rw-r--r--   0        0        0     8848 2023-05-12 08:52:50.076953 buteo-0.9.8/buteo/utils/utils_io.py
--rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.8/buteo/utils/utils_path.py
--rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.8/buteo/utils/utils_projection.py
--rw-r--r--   0        0        0    16744 2023-05-09 10:16:56.513576 buteo-0.9.8/buteo/utils/utils_translate.py
--rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.8/buteo/vector/__init__.py
--rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.8/buteo/vector/buffer.py
--rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.8/buteo/vector/clip.py
--rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/convert_parts.py
--rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.8/buteo/vector/core_vector.py
--rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/dissolve.py
--rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.8/buteo/vector/grid.py
--rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/intersect.py
--rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/merge.py
--rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/metadata.py
--rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.8/buteo/vector/rasterize.py
--rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.8/buteo/vector/reproject.py
--rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/shapes.py
--rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.8/buteo/vector/split.py
--rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.8/buteo/vector/zonal_statistics.py
--rw-r--r--   0        0        0      785 2023-05-12 13:33:46.713793 buteo-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.8/readme.md
--rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.9/LICENSE
+-rw-r--r--   0        0        0     4779 2023-05-09 11:35:41.351219 buteo-0.9.9/buteo/__init__.py
+-rw-r--r--   0        0        0      222 2023-05-09 11:50:06.491154 buteo-0.9.9/buteo/ai/__init__.py
+-rw-r--r--   0        0        0    10120 2023-05-30 11:44:10.691097 buteo-0.9.9/buteo/ai/augmentation.py
+-rw-r--r--   0        0        0    28002 2023-05-09 12:27:55.018873 buteo-0.9.9/buteo/ai/augmentation_funcs.py
+-rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.9/buteo/ai/augmentation_utils.py
+-rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.9/buteo/ai/encoding.py
+-rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.9/buteo/ai/scalers.py
+-rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.9/buteo/ai/selection.py
+-rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.9/buteo/array/__init__.py
+-rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.9/buteo/array/color.py
+-rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.9/buteo/array/convolution.py
+-rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.9/buteo/array/convolution_distance.py
+-rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.9/buteo/array/convolution_funcs.py
+-rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.9/buteo/array/convolution_kernels.py
+-rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.9/buteo/array/edge_detection.py
+-rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.9/buteo/array/fill.py
+-rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.9/buteo/array/filters.py
+-rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.9/buteo/array/morphology.py
+-rw-r--r--   0        0        0    31384 2023-05-12 13:33:23.446975 buteo-0.9.9/buteo/array/patches.py
+-rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.9/buteo/array/timeseries.py
+-rw-r--r--   0        0        0     2819 2023-05-09 11:52:21.206628 buteo-0.9.9/buteo/array/utils_array.py
+-rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.9/buteo/eo/__init__.py
+-rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/L2A_GIPP.xml
+-rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/step_01_backstatter.xml
+-rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/step_01_coherence.xml
+-rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/step_02_backscatter.xml
+-rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/step_02_backscatter_speckle.xml
+-rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.9/buteo/eo/graphs/step_02_coherence.xml
+-rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.9/buteo/eo/s1_preprocess.py
+-rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.9/buteo/eo/s1_utils.py
+-rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.9/buteo/eo/s2_indices.py
+-rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.9/buteo/eo/s2_utils.py
+-rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.9/buteo/raster/__init__.py
+-rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.9/buteo/raster/align.py
+-rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.9/buteo/raster/borders.py
+-rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.9/buteo/raster/clip.py
+-rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.9/buteo/raster/coordinates.py
+-rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.9/buteo/raster/core_offsets.py
+-rw-r--r--   0        0        0    18432 2023-05-10 07:50:31.889375 buteo-0.9.9/buteo/raster/core_raster.py
+-rw-r--r--   0        0        0    37055 2023-05-12 11:11:07.920206 buteo-0.9.9/buteo/raster/core_raster_io.py
+-rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.9/buteo/raster/core_stack.py
+-rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.9/buteo/raster/datatype.py
+-rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.9/buteo/raster/dem.py
+-rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.9/buteo/raster/grid.py
+-rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.9/buteo/raster/metadata.py
+-rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.9/buteo/raster/nodata.py
+-rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.9/buteo/raster/proximity.py
+-rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.9/buteo/raster/reproject.py
+-rw-r--r--   0        0        0    10614 2023-05-30 11:35:51.623814 buteo-0.9.9/buteo/raster/resample.py
+-rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.9/buteo/raster/shift.py
+-rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.9/buteo/raster/vectorize.py
+-rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.9/buteo/utils/__init__.py
+-rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.9/buteo/utils/utils_aux.py
+-rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.9/buteo/utils/utils_base.py
+-rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.9/buteo/utils/utils_bbox.py
+-rw-r--r--   0        0        0    28752 2023-05-30 11:35:50.361021 buteo-0.9.9/buteo/utils/utils_gdal.py
+-rw-r--r--   0        0        0     8848 2023-05-12 08:52:50.076953 buteo-0.9.9/buteo/utils/utils_io.py
+-rw-r--r--   0        0        0    28603 2023-05-30 11:39:15.787232 buteo-0.9.9/buteo/utils/utils_path.py
+-rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.9/buteo/utils/utils_projection.py
+-rw-r--r--   0        0        0    16744 2023-05-09 10:16:56.513576 buteo-0.9.9/buteo/utils/utils_translate.py
+-rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.9/buteo/vector/__init__.py
+-rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.9/buteo/vector/buffer.py
+-rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.9/buteo/vector/clip.py
+-rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/convert_parts.py
+-rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.9/buteo/vector/core_vector.py
+-rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/dissolve.py
+-rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.9/buteo/vector/grid.py
+-rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/intersect.py
+-rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/merge.py
+-rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/metadata.py
+-rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.9/buteo/vector/rasterize.py
+-rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.9/buteo/vector/reproject.py
+-rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.9/buteo/vector/shapes.py
+-rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.9/buteo/vector/split.py
+-rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.9/buteo/vector/zonal_statistics.py
+-rw-r--r--   0        0        0      785 2023-05-30 11:39:32.583574 buteo-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4956 2023-05-15 12:41:46.634378 buteo-0.9.9/readme.md
+-rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 buteo-0.9.9/PKG-INFO
```

### Comparing `buteo-0.9.8/LICENSE` & `buteo-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/__init__.py` & `buteo-0.9.9/buteo/__init__.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/ai/augmentation.py` & `buteo-0.9.9/buteo/ai/augmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,16 +131,27 @@
         # Set augmentations and callback
         self.augmentations = augmentations or []
         self.callback = callback
         self.channel_last = False
         self.output_is_channel_last = output_is_channel_last
 
         for aug in self.augmentations:
+
+            # Check if augmentation is valid
+            if "name" not in aug:
+                raise ValueError("Augmentation name not specified.")
+
+            if "p" not in aug and "chance" not in aug:
+                raise ValueError("Augmentation chance not specified.")
+
             aug_name = aug["name"]
-            aug_change = aug["chance"] if aug["chance"] is not None else aug["p"]
+            if "chance" in aug:
+                aug_change = aug["chance"]
+            elif "p" in aug:
+                aug_change = aug["p"]
 
             assert aug_change is not None, "Augmentation chance cannot be None."
             assert 0 <= aug_change <= 1, "Augmentation chance must be between 0 and 1."
             assert aug_name is not None, "Augmentation name cannot be None."
 
     def __len__(self):
         return len(self.x_train)
@@ -148,15 +159,18 @@
     def __getitem__(self, index):
         x = self.x_train[index].copy()
         y = self.y_train[index].copy()
 
         # Apply augmentations
         for aug in self.augmentations:
             aug_name = aug["name"]
-            aug_change = aug["chance"] if aug["chance"] is not None else aug["p"]
+            if "chance" in aug:
+                aug_change = aug["chance"]
+            elif "p" in aug:
+                aug_change = aug["p"]
             func = None
 
             # Check if augmentation should be applied
             if np.random.rand() > aug_change:
                 break
 
             # Mapping augmentation names to their respective functions
```

### Comparing `buteo-0.9.8/buteo/ai/augmentation_funcs.py` & `buteo-0.9.9/buteo/ai/augmentation_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/ai/augmentation_utils.py` & `buteo-0.9.9/buteo/ai/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/ai/encoding.py` & `buteo-0.9.9/buteo/ai/encoding.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/ai/scalers.py` & `buteo-0.9.9/buteo/ai/scalers.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/ai/selection.py` & `buteo-0.9.9/buteo/ai/selection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/color.py` & `buteo-0.9.9/buteo/array/color.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/convolution.py` & `buteo-0.9.9/buteo/array/convolution.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/convolution_distance.py` & `buteo-0.9.9/buteo/array/convolution_distance.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/convolution_funcs.py` & `buteo-0.9.9/buteo/array/convolution_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/convolution_kernels.py` & `buteo-0.9.9/buteo/array/convolution_kernels.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/edge_detection.py` & `buteo-0.9.9/buteo/array/edge_detection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/fill.py` & `buteo-0.9.9/buteo/array/fill.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/filters.py` & `buteo-0.9.9/buteo/array/filters.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/morphology.py` & `buteo-0.9.9/buteo/array/morphology.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/patches.py` & `buteo-0.9.9/buteo/array/patches.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/timeseries.py` & `buteo-0.9.9/buteo/array/timeseries.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/array/utils_array.py` & `buteo-0.9.9/buteo/array/utils_array.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/L2A_GIPP.xml` & `buteo-0.9.9/buteo/eo/graphs/L2A_GIPP.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/step_01_backstatter.xml` & `buteo-0.9.9/buteo/eo/graphs/step_01_backstatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/step_01_coherence.xml` & `buteo-0.9.9/buteo/eo/graphs/step_01_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/step_02_backscatter.xml` & `buteo-0.9.9/buteo/eo/graphs/step_02_backscatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/step_02_backscatter_speckle.xml` & `buteo-0.9.9/buteo/eo/graphs/step_02_backscatter_speckle.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/graphs/step_02_coherence.xml` & `buteo-0.9.9/buteo/eo/graphs/step_02_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/s1_preprocess.py` & `buteo-0.9.9/buteo/eo/s1_preprocess.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/s1_utils.py` & `buteo-0.9.9/buteo/eo/s1_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/s2_indices.py` & `buteo-0.9.9/buteo/eo/s2_indices.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/eo/s2_utils.py` & `buteo-0.9.9/buteo/eo/s2_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/align.py` & `buteo-0.9.9/buteo/raster/align.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/borders.py` & `buteo-0.9.9/buteo/raster/borders.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/clip.py` & `buteo-0.9.9/buteo/raster/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/coordinates.py` & `buteo-0.9.9/buteo/raster/coordinates.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/core_offsets.py` & `buteo-0.9.9/buteo/raster/core_offsets.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/core_raster.py` & `buteo-0.9.9/buteo/raster/core_raster.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/core_raster_io.py` & `buteo-0.9.9/buteo/raster/core_raster_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/core_stack.py` & `buteo-0.9.9/buteo/raster/core_stack.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/datatype.py` & `buteo-0.9.9/buteo/raster/datatype.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/dem.py` & `buteo-0.9.9/buteo/raster/dem.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/grid.py` & `buteo-0.9.9/buteo/raster/grid.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/metadata.py` & `buteo-0.9.9/buteo/raster/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/nodata.py` & `buteo-0.9.9/buteo/raster/nodata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/proximity.py` & `buteo-0.9.9/buteo/raster/proximity.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/reproject.py` & `buteo-0.9.9/buteo/raster/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/resample.py` & `buteo-0.9.9/buteo/raster/resample.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         if not utils_path._check_is_valid_output_filepath(out_path):
             raise ValueError(f"Invalid output path: {out_path}")
 
     ref = core_raster._raster_open(raster)
     metadata = core_raster._get_basic_metadata_raster(ref)
 
     if isinstance(target_size, (gdal.Dataset, str)):
-        x_res, y_res, x_pixels, y_pixels = utils_gdal._get_raster_size(
-            target_size, target_in_pixels=target_in_pixels
-        )
+        x_res, y_res, x_pixels, y_pixels = utils_gdal._get_raster_size(target_size)
     elif target_in_pixels:
         x_res = None
         y_res = None
 
         if isinstance(target_size, (list, tuple)):
             assert len(target_size) == 2, f"Invalid target_size. {target_size}"
             x_pixels = target_size[0]
```

### Comparing `buteo-0.9.8/buteo/raster/shift.py` & `buteo-0.9.9/buteo/raster/shift.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/raster/vectorize.py` & `buteo-0.9.9/buteo/raster/vectorize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_aux.py` & `buteo-0.9.9/buteo/utils/utils_aux.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_base.py` & `buteo-0.9.9/buteo/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_bbox.py` & `buteo-0.9.9/buteo/utils/utils_bbox.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_gdal.py` & `buteo-0.9.9/buteo/utils/utils_gdal.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,17 +918,14 @@
     Gets the size of a raster (xres, yres).
 
     Parameters
     ----------
     target : Union[gdal.Dataset, str]
         The target to get the size from.
 
-    target_in_pixels : bool, optional
-        If True, the target is in pixels. Default: False.
-
     Returns
     -------
     Tuple[float, float]
     """
     assert _check_is_raster(raster), "The target must be a raster."
 
     try:
```

### Comparing `buteo-0.9.8/buteo/utils/utils_io.py` & `buteo-0.9.9/buteo/utils/utils_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_path.py` & `buteo-0.9.9/buteo/utils/utils_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,14 +694,18 @@
     if not isinstance(output_list, list):
         return False
 
     if len(output_list) == 0:
         return False
 
     for path in output_list:
+        # TODO: This is a hack to avoid checking vsimem paths.
+        if "vsimem" in path:
+            continue
+
         if not _check_is_valid_output_filepath(path, overwrite=overwrite):
             return False
 
     return True
 
 
 def _delete_if_required(
```

### Comparing `buteo-0.9.8/buteo/utils/utils_projection.py` & `buteo-0.9.9/buteo/utils/utils_projection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/utils/utils_translate.py` & `buteo-0.9.9/buteo/utils/utils_translate.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/buffer.py` & `buteo-0.9.9/buteo/vector/buffer.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/clip.py` & `buteo-0.9.9/buteo/vector/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/convert_parts.py` & `buteo-0.9.9/buteo/vector/convert_parts.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/core_vector.py` & `buteo-0.9.9/buteo/vector/core_vector.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/dissolve.py` & `buteo-0.9.9/buteo/vector/dissolve.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/intersect.py` & `buteo-0.9.9/buteo/vector/intersect.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/merge.py` & `buteo-0.9.9/buteo/vector/merge.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/metadata.py` & `buteo-0.9.9/buteo/vector/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/rasterize.py` & `buteo-0.9.9/buteo/vector/rasterize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/reproject.py` & `buteo-0.9.9/buteo/vector/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/shapes.py` & `buteo-0.9.9/buteo/vector/shapes.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/split.py` & `buteo-0.9.9/buteo/vector/split.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/buteo/vector/zonal_statistics.py` & `buteo-0.9.9/buteo/vector/zonal_statistics.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.8/pyproject.toml` & `buteo-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.8.0", "numba>=0.57.0", "psutil>=5.9.5", "PyYAML>=6.0", "tqdm>=4.65.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "buteo"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="Casper Fibaek", email="casperfibaek@gmail.com" },
 ]
 description = "Tools for merging Geospatial Analysis and AI."
 readme = "readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `buteo-0.9.8/readme.md` & `buteo-0.9.9/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 Please note that Buteo is under active development, and its API may not be entirely stable. Feel free to report any bugs or suggest improvements.
 
 When using, please pin the version of Buteo you are using to avoid breaking changes.
 
 For documentation, visit: https://casperfibaek.github.io/buteo/
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7936577.svg)](https://doi.org/10.5281/zenodo.7936577)
+
+Fibaek, Casper. (2023). Buteo: Geospatial Data Analysis Framework for AI/EO. (v0.9.8). Zenodo. https://doi.org/10.5281/zenodo.7936577
+
 **Dependencies** </br>
 `numba` (https://numba.pydata.org/) </br>
 `gdal` (https://gdal.org/) </br>
 
 **Installation** </br>
 Using pip:
 ```
```

### Comparing `buteo-0.9.8/PKG-INFO` & `buteo-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buteo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Tools for merging Geospatial Analysis and AI.
 Author-email: Casper Fibaek <casperfibaek@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,14 +20,18 @@
 
 Please note that Buteo is under active development, and its API may not be entirely stable. Feel free to report any bugs or suggest improvements.
 
 When using, please pin the version of Buteo you are using to avoid breaking changes.
 
 For documentation, visit: https://casperfibaek.github.io/buteo/
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7936577.svg)](https://doi.org/10.5281/zenodo.7936577)
+
+Fibaek, Casper. (2023). Buteo: Geospatial Data Analysis Framework for AI/EO. (v0.9.8). Zenodo. https://doi.org/10.5281/zenodo.7936577
+
 **Dependencies** </br>
 `numba` (https://numba.pydata.org/) </br>
 `gdal` (https://gdal.org/) </br>
 
 **Installation** </br>
 Using pip:
 ```
```

