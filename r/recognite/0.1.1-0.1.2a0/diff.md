# Comparing `tmp/recognite-0.1.1.tar.gz` & `tmp/recognite-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognite-0.1.1.tar", last modified: Thu Jul 27 14:57:53 2023, max compression
+gzip compressed data, was "recognite-0.1.2a0.tar", last modified: Sun Aug  6 13:45:37 2023, max compression
```

## Comparing `recognite-0.1.1.tar` & `recognite-0.1.2a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.272090 recognite-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 14:57:42.000000 recognite-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-27 14:57:53.272090 recognite-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-27 14:57:42.000000 recognite-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.268090 recognite-0.1.1/recognite/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.272090 recognite-0.1.1/recognite/data/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/data/data_frame_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/data/gallery_query_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/data/k_fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/data/train_val_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.272090 recognite-0.1.1/recognite/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/hard_pos_neg_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/pr_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/eval/score_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.272090 recognite-0.1.1/recognite/model/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/model/classifier_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/model/recognizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.272090 recognite-0.1.1/recognite/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/utils/avg_ref_embs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/utils/running_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-27 14:57:42.000000 recognite-0.1.1/recognite/utils/three_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:53.268090 recognite-0.1.1/recognite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 14:57:53.000000 recognite-0.1.1/recognite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:57:53.272090 recognite-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-27 14:57:42.000000 recognite-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-06 13:45:27.000000 recognite-0.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-06 13:45:37.965602 recognite-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-08-06 13:45:27.000000 recognite-0.1.2a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/data/data_frame_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/data/gallery_query_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/data/k_fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/data/train_val_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/hard_pos_neg_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/pr_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/eval/score_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/model/classifier_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/model/recognizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/utils/avg_ref_embs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/utils/running_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-08-06 13:45:27.000000 recognite-0.1.2a0/recognite/utils/three_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:45:37.965602 recognite-0.1.2a0/recognite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 13:45:37.000000 recognite-0.1.2a0/recognite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:45:37.969602 recognite-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-06 13:45:27.000000 recognite-0.1.2a0/setup.py
```

### Comparing `recognite-0.1.1/LICENSE` & `recognite-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/PKG-INFO` & `recognite-0.1.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: recognite
-Version: 0.1.1
+Version: 0.1.2a0
 Summary: Recognite is a library to kickstart your next PyTorch-based recognition project.
 Home-page: https://github.com/florisdf/recognite
 Author: Floris De Feyter
 Author-email: floris.defeyter@kuleuven.be
 License: MIT license
 Keywords: recognite
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `recognite-0.1.1/README.md` & `recognite-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/data/data_frame_dataset.py` & `recognite-0.1.2a0/recognite/data/data_frame_dataset.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/data/k_fold.py` & `recognite-0.1.2a0/recognite/data/k_fold.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import numpy as np
 import pandas as pd
 
 
 def k_fold_trainval_split(
     df: pd.DataFrame,
-    num_folds: int,
-    val_fold: int,
-    seed: int,
+    num_folds: int = 5,
+    val_fold: int = 0,
+    seed: int = 0,
     label_key='label'
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Splits the given DataFrame into a train and validation subset.
 
     The subsets are composed by shuffling the labels in the DataFrame, using
     random seed ``seed``. The labels are then split into ``num_folds`` folds,
     where each label can only be in a single fold. We then choose one fold for
```

### Comparing `recognite-0.1.1/recognite/data/train_val_datasets.py` & `recognite-0.1.2a0/recognite/data/train_val_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Callable, Tuple
+from typing import Callable, Optional, Tuple
 
 import pandas as pd
 
 from .gallery_query_split import split_gallery_query
 from .k_fold import k_fold_trainval_split
 from .data_frame_dataset import DataFrameDataset
 
 
 def train_val_datasets(
     data_csv_file: str,
-    label_key: str,
-    image_key: str,
-    num_folds: int,
-    val_fold: int,
-    fold_seed: int,
-    num_refs: int,
-    ref_seed: int,
-    tfm_train: Callable = None,
-    tfm_val: Callable = None,
+    image_key: str = 'image',
+    label_key: str = 'label',
+    num_folds: int = 5,
+    val_fold: int = 0,
+    fold_seed: int = 0,
+    num_refs: int = 1,
+    ref_seed: int = 0,
+    tfm_train: Optional[Callable] = None,
+    tfm_val: Optional[Callable] = None,
 ) -> Tuple[DataFrameDataset, DataFrameDataset, DataFrameDataset]:
     """Creates training and validation datasets for recognition training.
 
     The datasets are created based on a CSV file that contains all image paths
     with a corresponding label. The images are split up into a training and a
     validation subset. The data split is based on labels, so no label will
     occur both in the training and in the validation subset. We do this to
@@ -48,18 +48,18 @@
     The query-gallery split is determined by ``num_refs`` (the number of
     references per label) and ``ref_seed`` (the seed for the random
     generator that shuffles the data before splitting).
 
     Args:
         data_csv_file: The path of the CSV file containing the images and
             corresponding labels.
-        label_key: The column in the CSV file that contains the label of each
-            image.
         image_key: The column in the CSV file that contains th image path of
             each image.
+        label_key: The column in the CSV file that contains the label of each
+            image.
         num_folds: The number of folds to use for splitting the dataset into
             training and validation. Note that the folds are label-based, not
             sample-based.
         val_fold: The index of the fold to use for validation. The others will
             be used for training.
         fold_seed: The random seed to use for k-fold splitting.
         num_refs: The number of references per class in the gallery.
```

### Comparing `recognite-0.1.1/recognite/eval/accuracy.py` & `recognite-0.1.2a0/recognite/eval/accuracy.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/eval/hard_pos_neg_scores.py` & `recognite-0.1.2a0/recognite/eval/hard_pos_neg_scores.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/eval/knn.py` & `recognite-0.1.2a0/recognite/eval/knn.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/eval/pr_metrics.py` & `recognite-0.1.2a0/recognite/eval/pr_metrics.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/model/classifier_ops.py` & `recognite-0.1.2a0/recognite/model/classifier_ops.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/model/recognizer.py` & `recognite-0.1.2a0/recognite/model/recognizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,46 +63,58 @@
         backbone: The backbone model.
         classifier: The fully-connected layer that acts as the classifier
             during training.
     """
     def __init__(
         self,
         model_name: str,
-        num_classes: int,
+        num_classes: Optional[int] = None,
         weights: Optional[Union[Weights, str]] = None,
         clf_bias: bool = False,
+        normalize: bool = True,
     ):
         """
         Args:
             model_name: The name of the model to use. The classification layer
                 of this model will be extracted and replaced by a
                 fully-connected layer that outputs the desired number of
                 classes (see ``num_classes``). Note that we normalize the
                 weights of the fully connected layer so that the columns have
                 norm 1.
-            num_classes: The number of classes outputted by the classifier.
+            num_classes: The number of classes outputted by the classifier. If
+                ``None``, don't use classifier and instead also return the
+                backbone's embedding during training.
             weights: The pretrained weights to initialize the model with. If
                 ``None``, the weights are randomly initialized. See also
                 <https://pytorch.org/vision/stable/models.html>.
             clf_bias: If ``True``, use a bias in the classification layer.
                 Using bias in the fully connected layer together with weight
                 normalization can worsen the results (see
                 <https://dl.acm.org/doi/10.1145/3123266.3123359>), so we
                 suggest to keep it turned off.
+            normalize: If ``True``, normalize the embedding returned by the
+                backbone, as well as the weights of the classifier (if
+                applicable).
         """
         super().__init__()
 
         if model_name not in SUPPORTED_MODELS:
             raise ValueError(f'Unsupported model "{model_name}"')
 
+        self.normalize = normalize
+
         model = models.get_model(model_name, weights=weights)
-        update_classifier(model, num_classes, bias=clf_bias)
 
-        self.backbone, self.classifier = split_backbone_classifier(model)
-        self._ult_clf = get_ultimate_classifier(self.classifier)
+        if num_classes is not None:
+            update_classifier(model, num_classes, bias=clf_bias)
+            self.backbone, self.classifier = split_backbone_classifier(model)
+            self._ult_clf = get_ultimate_classifier(self.classifier)
+        else:
+            self.backbone, self.classifier = split_backbone_classifier(model)
+            self.classifier = None
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Passes a batch of input images through the model.
 
         During training, the input is passed through the backbone and the
         classifier, and the classification logits are returned. During
         inference, only the backbone is used and the extracted embeddings are
@@ -111,26 +123,27 @@
         Args:
             x: The batch of input images.
 
         Returns:
             The classification logits during training, and the embeddings
             during inference (evaluation).
         """
-        if self.training:
+        if self.training and self.normalize and self.classifier is not None:
             self._normalize_clf_layer()
 
         x = self.backbone(x)
 
         if hasattr(x, 'logits'):
             # Support GoogLeNet and Inception v3
             x = x.logits
 
-        x = x / torch.norm(x, dim=1, keepdim=True)
+        if self.normalize:
+            x = x / torch.norm(x, dim=1, keepdim=True)
 
-        if self.training:
+        if self.training and self.classifier is not None:
             x = self.classifier(x)
 
         return x
 
     def _normalize_clf_layer(self):
         """Normalizes the weights of the classifier."""
         self._ult_clf.weight.data = (
```

### Comparing `recognite-0.1.1/recognite/utils/avg_ref_embs.py` & `recognite-0.1.2a0/recognite/utils/avg_ref_embs.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/utils/running_extrema.py` & `recognite-0.1.2a0/recognite/utils/running_extrema.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite/utils/three_crop.py` & `recognite-0.1.2a0/recognite/utils/three_crop.py`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/recognite.egg-info/PKG-INFO` & `recognite-0.1.2a0/recognite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: recognite
-Version: 0.1.1
+Version: 0.1.2a0
 Summary: Recognite is a library to kickstart your next PyTorch-based recognition project.
 Home-page: https://github.com/florisdf/recognite
 Author: Floris De Feyter
 Author-email: floris.defeyter@kuleuven.be
 License: MIT license
 Keywords: recognite
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `recognite-0.1.1/recognite.egg-info/SOURCES.txt` & `recognite-0.1.2a0/recognite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recognite-0.1.1/setup.py` & `recognite-0.1.2a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Floris De Feyter",
     author_email='floris.defeyter@kuleuven.be',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
@@ -39,10 +39,10 @@
     include_package_data=True,
     keywords='recognite',
     name='recognite',
     packages=find_packages(include=['recognite', 'recognite.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/florisdf/recognite',
-    version='0.1.1',
+    version='0.1.2-alpha',
     zip_safe=False,
 )
```

