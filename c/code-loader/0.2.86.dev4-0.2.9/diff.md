# Comparing `tmp/code_loader-0.2.86.dev4.tar.gz` & `tmp/code-loader-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_loader-0.2.86.dev4.tar", max compression
+gzip compressed data, was "code-loader-0.2.9.tar", max compression
```

## Comparing `code_loader-0.2.86.dev4.tar` & `code-loader-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,17 @@
--rw-r--r--   0        0        0     1067 2021-12-01 12:49:40.221608 code_loader-0.2.86.dev4/LICENSE
--rw-r--r--   0        0        0       63 2021-12-01 12:49:40.221888 code_loader-0.2.86.dev4/README.md
--rw-r--r--   0        0        0      116 2022-05-11 11:47:06.009274 code_loader-0.2.86.dev4/code_loader/__init__.py
--rw-r--r--   0        0        0        0 2021-12-01 12:49:40.222215 code_loader-0.2.86.dev4/code_loader/contract/__init__.py
--rw-r--r--   0        0        0     4614 2023-08-02 10:21:15.931734 code_loader-0.2.86.dev4/code_loader/contract/datasetclasses.py
--rw-r--r--   0        0        0     1481 2023-08-02 12:28:42.743204 code_loader-0.2.86.dev4/code_loader/contract/enums.py
--rw-r--r--   0        0        0       51 2023-01-25 08:28:09.946315 code_loader-0.2.86.dev4/code_loader/contract/exceptions.py
--rw-r--r--   0        0        0     2623 2023-08-02 12:28:42.738582 code_loader-0.2.86.dev4/code_loader/contract/responsedataclasses.py
--rw-r--r--   0        0        0     4761 2022-09-14 12:54:18.363656 code_loader-0.2.86.dev4/code_loader/contract/visualizer_classes.py
--rw-r--r--   0        0        0        0 2023-02-20 09:25:15.316077 code_loader-0.2.86.dev4/code_loader/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 09:25:15.316230 code_loader-0.2.86.dev4/code_loader/helpers/detection/__init__.py
--rw-r--r--   0        0        0     7527 2023-02-20 09:25:15.316380 code_loader-0.2.86.dev4/code_loader/helpers/detection/utils.py
--rw-r--r--   0        0        0        0 2023-02-20 09:25:15.316494 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/__init__.py
--rw-r--r--   0        0        0     7905 2023-07-16 08:27:34.163957 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/decoder.py
--rw-r--r--   0        0        0       81 2023-07-16 08:27:34.164260 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/enums.py
--rw-r--r--   0        0        0     3132 2023-02-20 09:25:15.316760 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/grid.py
--rw-r--r--   0        0        0    18610 2023-08-01 13:17:28.019674 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/loss.py
--rw-r--r--   0        0        0    11349 2023-06-13 11:54:04.302521 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/pytorch_utils.py
--rw-r--r--   0        0        0     8037 2023-07-16 08:27:34.165465 code_loader-0.2.86.dev4/code_loader/helpers/detection/yolo/utils.py
--rw-r--r--   0        0        0        0 2023-06-11 16:22:23.627990 code_loader-0.2.86.dev4/code_loader/helpers/instancesegmentation/__init__.py
--rw-r--r--   0        0        0      930 2023-06-11 16:22:23.628351 code_loader-0.2.86.dev4/code_loader/helpers/instancesegmentation/utils.py
--rw-r--r--   0        0        0       93 2022-05-11 11:47:06.012412 code_loader-0.2.86.dev4/code_loader/leap_binder/__init__.py
--rw-r--r--   0        0        0     6806 2023-08-02 08:52:31.387076 code_loader-0.2.86.dev4/code_loader/leap_binder/leapbinder.py
--rw-r--r--   0        0        0     4758 2023-08-01 13:17:28.020183 code_loader-0.2.86.dev4/code_loader/leap_loader_parallelized_base.py
--rw-r--r--   0        0        0    17900 2023-08-03 13:26:27.432882 code_loader-0.2.86.dev4/code_loader/leaploader.py
--rw-r--r--   0        0        0     2233 2023-08-01 13:17:28.020637 code_loader-0.2.86.dev4/code_loader/metric_calculator_parallelized.py
--rw-r--r--   0        0        0        0 2023-02-20 09:25:15.317766 code_loader-0.2.86.dev4/code_loader/metrics/__init__.py
--rw-r--r--   0        0        0     6727 2023-03-09 14:01:48.440482 code_loader-0.2.86.dev4/code_loader/metrics/default_metrics.py
--rw-r--r--   0        0        0     2376 2023-08-01 13:17:28.021192 code_loader-0.2.86.dev4/code_loader/samples_generator_parallelized.py
--rw-r--r--   0        0        0     1736 2022-05-11 11:47:06.013107 code_loader-0.2.86.dev4/code_loader/utils.py
--rw-r--r--   0        0        0        0 2022-05-19 06:59:13.641605 code_loader-0.2.86.dev4/code_loader/visualizers/__init__.py
--rw-r--r--   0        0        0     2226 2023-06-15 14:22:18.899732 code_loader-0.2.86.dev4/code_loader/visualizers/default_visualizers.py
--rw-r--r--   0        0        0      905 2023-08-03 13:35:58.839491 code_loader-0.2.86.dev4/pyproject.toml
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 code_loader-0.2.86.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-12-01 12:49:40.221608 code-loader-0.2.9/LICENSE
+-rw-r--r--   0        0        0       63 2021-12-01 12:49:40.221888 code-loader-0.2.9/README.md
+-rw-r--r--   0        0        0      131 2021-12-02 13:04:01.154724 code-loader-0.2.9/code_loader/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-01 12:49:40.222215 code-loader-0.2.9/code_loader/contract/__init__.py
+-rw-r--r--   0        0        0     2357 2022-03-28 13:14:06.363969 code-loader-0.2.9/code_loader/contract/datasetclasses.py
+-rw-r--r--   0        0        0     1073 2022-01-30 17:03:35.077863 code-loader-0.2.9/code_loader/contract/decoder_classes.py
+-rw-r--r--   0        0        0      752 2022-01-30 17:03:35.078224 code-loader-0.2.9/code_loader/contract/enums.py
+-rw-r--r--   0        0        0     1409 2022-03-28 13:14:06.364283 code-loader-0.2.9/code_loader/contract/responsedataclasses.py
+-rw-r--r--   0        0        0      108 2021-12-02 13:04:01.155417 code-loader-0.2.9/code_loader/dataset_binder/__init__.py
+-rw-r--r--   0        0        0     3410 2022-03-28 13:14:06.364597 code-loader-0.2.9/code_loader/dataset_binder/datasetbinder.py
+-rw-r--r--   0        0        0     9242 2022-03-28 13:14:06.364931 code-loader-0.2.9/code_loader/datasetloader.py
+-rw-r--r--   0        0        0        0 2022-01-02 09:30:24.026399 code-loader-0.2.9/code_loader/decoders/__init__.py
+-rw-r--r--   0        0        0     2320 2022-01-11 15:15:30.813571 code-loader-0.2.9/code_loader/decoders/default_decoders.py
+-rw-r--r--   0        0        0     1548 2022-01-02 09:30:24.027864 code-loader-0.2.9/code_loader/utils.py
+-rw-r--r--   0        0        0      702 2022-03-28 13:14:39.404244 code-loader-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      797 2022-03-29 08:59:48.662325 code-loader-0.2.9/setup.py
+-rw-r--r--   0        0        0      562 2022-03-29 08:59:48.662571 code-loader-0.2.9/PKG-INFO
```

### Comparing `code_loader-0.2.86.dev4/LICENSE` & `code-loader-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `code_loader-0.2.86.dev4/code_loader/contract/enums.py` & `code-loader-0.2.9/code_loader/contract/enums.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,15 @@
 from enum import Enum, IntEnum
 
 
-class MetricEnum(Enum):
-    MeanSquaredError = 'MeanSquaredError'
-    MeanSquaredLogarithmicError = 'MeanSquaredLogarithmicError'
-    MeanAbsoluteError = 'MeanAbsoluteError'
-    MeanAbsolutePercentageError = 'MeanAbsolutePercentageError'
-    Accuracy = 'Accuracy'
-    BinaryAccuracy = 'BinaryAccuracy'
-    MeanIOU = 'MeanIOU'
-    ConfusionMatrixClassification = 'ConfusionMatrixClassification'
-    ConfusionMatrixBinaryClassification = 'ConfusionMatrixBinaryClassification'
-
-
-# backwards compatability: keeping it to not break old imports of Metric enum
-# should not be copied to engine contracts
-Metric = MetricEnum
-
-
 class LeapDataType(Enum):
     Image = 'Image'
     Text = 'Text'
     Graph = 'Graph'
+    Numeric = 'Numeric'
     HorizontalBar = 'HorizontalBar'
     ImageMask = 'ImageMask'
     TextMask = 'TextMask'
     ImageWithBBox = 'ImageWithBBox'
 
 
 class DatasetMetadataType(Enum):
@@ -35,26 +19,19 @@
     boolean = "boolean"
 
 
 class DataStateType(Enum):
     training = "training"
     validation = "validation"
     test = "test"
-    unlabeled = "unlabeled"
 
 
 class DataStateEnum(IntEnum):
     training = 0
     validation = 1
     test = 2
-    unlabeled = 3
-
-
-class ConfusionMatrixValue(Enum):
-    Positive = "Positive"
-    Negative = "Negative"
 
 
 # todo: handle test not run due to error in pre process and Add to TestingSectionEnum Enum didn't run
 class TestingSectionEnum(Enum):
     Warnings = "Warnings"
     Errors = "Errors"
```

### Comparing `code_loader-0.2.86.dev4/code_loader/utils.py` & `code-loader-0.2.9/code_loader/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import sys
+from typing import List
 from types import TracebackType
-from typing import List, Union
-
-import numpy as np
-import numpy.typing as npt
+import numpy as np  # type: ignore
 
 from code_loader.contract.datasetclasses import SectionCallableInterface, PreprocessResponse
 
 
 def to_numpy_return_wrapper(encoder_function: SectionCallableInterface) -> SectionCallableInterface:
-    def numpy_encoder_function(idx: int, samples: PreprocessResponse) -> npt.NDArray[np.float32]:
+    def numpy_encoder_function(idx: int, samples: PreprocessResponse) -> np.ndarray:
         result = encoder_function(idx, samples)
-        numpy_result: npt.NDArray[np.float32] = np.array(result)
+        numpy_result = np.array(result)
         return numpy_result
 
     return numpy_encoder_function
 
 
 def get_root_traceback(exc_tb: TracebackType) -> TracebackType:
     return_traceback = exc_tb
@@ -29,26 +27,24 @@
     root_exception_line_number = -1
     if exc_tb is not None:
         root_traceback = get_root_traceback(exc_tb)
         root_exception_line_number = root_traceback.tb_lineno
     return root_exception_line_number
 
 
-def get_shape(result: Union[npt.NDArray[np.float32], str, float, int, bool]) -> List[int]:
-    if not isinstance(result, np.ndarray):
-        return [1]
+def get_shape(result: np.ndarray) -> List[int]:
     np_shape = result.shape
     # fix single result shape viewing
-    if np_shape == ():
+    if np_shape is ():
         np_shape = (1,)
     shape = list(np_shape)
     return shape
 
 
-def rescale_min_max(image: npt.NDArray[np.float32]) -> npt.NDArray[np.float32]:
+def rescale_min_max(image: np.ndarray) -> np.ndarray:
     image = image.astype('float32')
     image -= image.min()
     image /= (image.max() - image.min() + 1e-5)
 
     # rescale the values to range between 0 and 255
     image *= 255
     image = image.astype('uint8')
```

