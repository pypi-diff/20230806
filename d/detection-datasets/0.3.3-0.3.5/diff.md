# Comparing `tmp/detection_datasets-0.3.3.tar.gz` & `tmp/detection_datasets-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detection_datasets-0.3.3.tar", max compression
+gzip compressed data, was "detection_datasets-0.3.5.tar", max compression
```

## Comparing `detection_datasets-0.3.3.tar` & `detection_datasets-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     7828 2022-10-12 19:11:22.045618 detection_datasets-0.3.3/README.md
--rw-r--r--   0        0        0     1356 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      188 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/__init__.py
--rw-r--r--   0        0        0     2914 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/bbox.py
--rw-r--r--   0        0        0    21378 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/detection_dataset.py
--rw-r--r--   0        0        0      110 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/readers/__init__.py
--rw-r--r--   0        0        0      589 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/readers/base.py
--rw-r--r--   0        0        0     3874 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/readers/coco.py
--rw-r--r--   0        0        0        0 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/__init__.py
--rw-r--r--   0        0        0      838 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/cache.py
--rw-r--r--   0        0        0       91 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/constants.py
--rw-r--r--   0        0        0      906 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/factories.py
--rw-r--r--   0        0        0      653 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/hub.py
--rw-r--r--   0        0        0      626 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/utils/visualization.py
--rw-r--r--   0        0        0      222 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/writers/__init__.py
--rw-r--r--   0        0        0     1813 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/writers/base.py
--rw-r--r--   0        0        0     3370 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/writers/coco.py
--rw-r--r--   0        0        0     2587 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/writers/mmdet.py
--rw-r--r--   0        0        0     3843 2022-10-12 19:11:22.081618 detection_datasets-0.3.3/src/detection_datasets/writers/yolo.py
--rw-r--r--   0        0        0     9003 1970-01-01 00:00:00.000000 detection_datasets-0.3.3/setup.py
--rw-r--r--   0        0        0     8769 1970-01-01 00:00:00.000000 detection_datasets-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     7828 2023-01-03 09:53:21.212107 detection_datasets-0.3.5/README.md
+-rw-r--r--   0        0        0     2042 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      242 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/__init__.py
+-rw-r--r--   0        0        0     2914 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/bbox.py
+-rw-r--r--   0        0        0    21378 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/detection_dataset.py
+-rw-r--r--   0        0        0      110 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/readers/__init__.py
+-rw-r--r--   0        0        0      589 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/readers/base.py
+-rw-r--r--   0        0        0     3874 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/readers/coco.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:53:21.236108 detection_datasets-0.3.5/src/detection_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      838 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/utils/cache.py
+-rw-r--r--   0        0        0       91 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/utils/constants.py
+-rw-r--r--   0        0        0      906 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/utils/factories.py
+-rw-r--r--   0        0        0      653 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/utils/hub.py
+-rw-r--r--   0        0        0      626 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/utils/visualization.py
+-rw-r--r--   0        0        0      222 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/writers/__init__.py
+-rw-r--r--   0        0        0     1813 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/writers/base.py
+-rw-r--r--   0        0        0     3370 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/writers/coco.py
+-rw-r--r--   0        0        0     2587 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/writers/mmdet.py
+-rw-r--r--   0        0        0     3843 2023-01-03 09:53:21.240108 detection_datasets-0.3.5/src/detection_datasets/writers/yolo.py
+-rw-r--r--   0        0        0     9003 1970-01-01 00:00:00.000000 detection_datasets-0.3.5/setup.py
+-rw-r--r--   0        0        0     8769 1970-01-01 00:00:00.000000 detection_datasets-0.3.5/PKG-INFO
```

### Comparing `detection_datasets-0.3.3/README.md` & `detection_datasets-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/bbox.py` & `detection_datasets-0.3.5/src/detection_datasets/bbox.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/detection_dataset.py` & `detection_datasets-0.3.5/src/detection_datasets/detection_dataset.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/readers/base.py` & `detection_datasets-0.3.5/src/detection_datasets/readers/base.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/readers/coco.py` & `detection_datasets-0.3.5/src/detection_datasets/readers/coco.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/utils/factories.py` & `detection_datasets-0.3.5/src/detection_datasets/utils/factories.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/utils/hub.py` & `detection_datasets-0.3.5/src/detection_datasets/utils/hub.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/utils/visualization.py` & `detection_datasets-0.3.5/src/detection_datasets/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/writers/base.py` & `detection_datasets-0.3.5/src/detection_datasets/writers/base.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/writers/coco.py` & `detection_datasets-0.3.5/src/detection_datasets/writers/coco.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/writers/mmdet.py` & `detection_datasets-0.3.5/src/detection_datasets/writers/mmdet.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/src/detection_datasets/writers/yolo.py` & `detection_datasets-0.3.5/src/detection_datasets/writers/yolo.py`

 * *Files identical despite different names*

### Comparing `detection_datasets-0.3.3/setup.py` & `detection_datasets-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'': ['*']}
 
 install_requires = \
 ['datasets[vision]>=2.4.0,<3.0.0', 'pandas>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'detection-datasets',
-    'version': '0.3.3',
+    'version': '0.3.5',
     'description': 'Easily load and transform datasets for object detection',
     'long_description': '<div align="center">\n\n<img src="https://raw.githubusercontent.com/blinjrm/detection-datasets/main/images/dd_logo.png" alt="logo" width="100"/>\n\n<br>\n\n# Detection datasets\n\n<a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.7-blue?style=flat-square&logo=python&logoColor=white"></a>\n<a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=flat-square&labelColor=gray"></a>\n<a href="https://github.com/blinjrm/detection-datasets/actions/workflows/ci.yaml"><img src="https://img.shields.io/github/workflow/status/blinjrm/detection-datasets/CI?label=CI&style=flat-square"/></a>\n<a href="https://github.com/blinjrm/detection-datasets/actions/workflows/pypi.yaml"><img src="https://img.shields.io/github/workflow/status/blinjrm/detection-datasets/Python%20package?label=Build&style=flat-square"/></a>\n<a href="https://pypi.org/project/detection-datasets/"><img src="https://img.shields.io/pypi/status/detection-datasets?style=flat-square"/></a>\n\n<br>\n\n*Easily load and transform datasets for object detection.*\n\n</div>\n<br>\n\n---\n\n**Documentation**: https://blinjrm.github.io/detection-datasets/\n\n**Source Code**: https://github.com/blinjrm/detection-datasets\n\n**Datasets on Hugging Face Hub**: https://huggingface.co/detection-datasets\n\n---\n\n<br>\n\n`detection_datasets` aims to make it easier to work with detection datasets.  \n\nThis library works alongside the [Detection dataset](https://huggingface.co/detection-datasets) organisation on the 🤗 Hub, where some detection datasets have been uploaded in the format expected by the library, and are ready to use.  \n\nThe main features are:\n* **Read** the dataset :\n    * From disk if it has already been downloaded.\n    * Directly from the Hugging Face Hub if it [already exist](https://huggingface.co/detection-datasets).\n* **Transform** the dataset:\n    * Select a subset of data.\n    * Remap categories.\n    * Create new train-val-test splits.\n* **Visualize** the annotations and images.\n* **Write** the dataset:\n    * To disk, selecting the target detection format: `COCO`, `YOLO` and more to come.\n    * To the Hugging Face Hub for easy reuse in a different environment and share with the community.\n\n<br>\n\n<div align="center">\n\n---\n\n*Read the quick start bellow, or directly jump to the tutorials:*\n\n| Goal                                 | Tutorial | Colab |\n|--------------------------------------|:--------:|:-----:|\n| Load from disk and upload to the Hub | [Open in the docs](https://blinjrm.github.io/detection-datasets/tutorials/1_Read/)     | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blinjrm/detection-datasets/blob/main/docs/tutorials/1_Read.ipynb)      |\n| Load from the Hub and transform          | [Open in the docs](https://blinjrm.github.io/detection-datasets/tutorials/2_Transform/)     | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blinjrm/detection-datasets/blob/main/docs/tutorials/2_Transform.ipynb)      |\n\n---\n\n</div>\n\n<br>\n\n# Getting started\n\n## 0. Setup\n\n### Requirements\n\nPython 3.7+\n\n`detection_datasets` is upon the great work of:\n\n- [Pandas](https://pandas.pydata.org) for manipulating data.  \n- [Hugging Face Datasets](https://huggingface.co/docs/datasets/index) to store and load datasets from the Hub.\n\n### Installation\n\n```console\n$ pip install detection_datasets\n```\n\n### Import\n\n```Python\nfrom detection_datasets import DetectionDataset\n```\n\n## 1. Read\n\n### From local filesystem\n\n```Python\nconfig = {\n    \'dataset_format\': \'coco\',                   # the format of the dataset on disk\n    \'path\': \'path/do/data/on/disk\',             # where the dataset is located\n    \'splits\': {                                 # how to read the files\n        \'train\': (\'train.json\', \'train\'),       # name of the split (annotation file, images directory)\n        \'test\': (\'test.json\', \'test\'),\n    },\n}\n\ndd = DetectionDataset()\ndd.from_disk(**config)\n\n# note that you can use method cascading as well:\n# dd = DetectionDataset().from_disk(**config)\n```\n\n### From the Hugging Face Hub\n\nThe `detection_dataset` library works alongside the [Detection dataset](https://huggingface.co/detection-datasets) organisation on the Hugging Face Hub, where some detection datasets have been uploaded in the format expected by the library, and are ready to use.\n\n```Python\ndd = DetectionDataset().from_hub(name=\'fashionpedia\')\n```\nCurrently supported format for reading datasets are:  \n- COCO  \n- *more to come*  \n\nThe list of datasets available from the Hub is given by:\n\n```Python\n# Search in the "detection-datasets" repository on the Hub.\nDetectionDataset().available_in_hub()  \n\n# Search in another repository on the Hub.\nDetectionDataset().available_in_hub(repo_name=MY_REPO_OR_ORGANISATION)\n```\n\n## 2. Transform\n\nThe supported transformations are:\n\n```Python\n# Select a subset of images, perserving the splits and their proportions\ndd.select(n_images=1000)\n\n# Shuffle the dataset, perserving the splits and their proportions\ndd.shuffle(seed=42)\n\n# Create new train-val-test splits, overwritting the splits from the original dataset\ndd.split(splits=[0.8, 0.1, 0.1])\n\n# Map existing categories to new categories.\n# The annotations with a category absent from the mapping are dropped.\ndd.map_categories(mapping={\'existing_category\': \'new_category\'})\n```\n\nThese transformations can be chained; for example here we select a subset of 10.000 images and create new train-val-test splits:\n\n```Python\ndd = DetectionDataset()\\\n    .from_hub(name=\'fashionpedia\')\\\n    .select(n_images=10000)\\\n    .split(splits=[0.8, 0.1, 0.1])\n```\n\n## 3. Visualize\n\nThe `DetectionDataset` objects contains several properties to analyze your data:\n\n\n```Python\ndd.data                     # This is equivlent to calling `dd.get_data(\'image\')`,\n                            # and returns a DataFrame with 1 row per image\n\ndd.get_data(\'bbox\')         # Returns a DataFrame with 1 row per annotation\n\ndd.n_images                 # Number of images\n\ndd.n_bbox                   # Number of annotations\n\ndd.splits                   # List of split names\n\ndd.split_proportions        # DataFrame with the % of iamges in each split\n\ndd.categories               # DataFrame with the categories and thei ids\n\ndd.category_names           # List of categories\n\ndd.n_categories             # Number of categories\n\n```\n\nYou can also visualize a image with its annotations in a notebook:\n\n```Python\ndd.show()                   # Shows a random image from the dataset\ndd.show(image_id=42)        # Shows the select image based on image_id\n```\n\n<div align="center">\n<img src="https://raw.githubusercontent.com/blinjrm/detection-datasets/main/images/show.png" alt="image with annotations" width="500"/>\n</div>\n\n## 4. Write\n\n### To local filesystem\n\nOnce the dataset is ready, you can write it to the local filesystem in a given format:\n\n```Python\ndd.to_disk(\n    dataset_format=\'yolo\',\n    name=\'MY_DATASET_NAME\',\n    path=\'DIRECTORY_TO_WRITE_TO\',\n)\n```\n\nCurrently supported format for writing datasets are:  \n- YOLO  \n- COCO\n- MMDET  \n- *more to come*  \n\n### To the Hugging Face Hub\n\nThe dataset can also be easily uploaded to the Hugging Face Hub, for reuse later on or in a different environment:\n\n```Python\ndd.to_hub(\n    dataset_name=\'MY_DATASET_NAME\',\n    repo_name=\'MY_REPO_OR_ORGANISATION\'\n)\n```\nThe dataset viewer on the Hub will work out of the box, and we encourage you to update the README in your new repo to make it easier for the comminuty to use the dataset.\n\n<div align="center">\n<img src="https://raw.githubusercontent.com/blinjrm/detection-datasets/main/images/hub.png" alt="hub viewer" width="800"/>\n</div>\n',
     'author': 'Jerome Blin',
     'author_email': 'blinjrm@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/blinjrm/detection-dataset',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['detection_datasets', 'detection_datasets.readers',
 'detection_datasets.utils', 'detection_datasets.writers'] package_data = \ {'':
 ['*']} install_requires = \ ['datasets[vision]>=2.4.0,<3.0.0',
 'pandas>=1.3.0,<2.0.0'] setup_kwargs = { 'name': 'detection-datasets',
-'version': '0.3.3', 'description': 'Easily load and transform datasets for
+'version': '0.3.5', 'description': 'Easily load and transform datasets for
 object detection', 'long_description': '
                                 \n\n[logo]\n\n
      \n\n# Detection datasets\n\n[Python]\n[Code_style:_black]\n[https://
        img.shields.io/github/workflow/status/blinjrm/detection-datasets/
 CI?label=CI&style=flat-square]\n[https://img.shields.io/github/workflow/status/
  blinjrm/detection-datasets/Python%20package?label=Build&style=flat-square]\n
  [https://img.shields.io/pypi/status/detection-datasets?style=flat-square]\n\n
```

### Comparing `detection_datasets-0.3.3/PKG-INFO` & `detection_datasets-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detection-datasets
-Version: 0.3.3
+Version: 0.3.5
 Summary: Easily load and transform datasets for object detection
 Home-page: https://github.com/blinjrm/detection-dataset
 License: MIT
 Author: Jerome Blin
 Author-email: blinjrm@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: detection-datasets Version: 0.3.3 Summary: Easily
+Metadata-Version: 2.1 Name: detection-datasets Version: 0.3.5 Summary: Easily
 load and transform datasets for object detection Home-page: https://github.com/
 blinjrm/detection-dataset License: MIT Author: Jerome Blin Author-email:
 blinjrm@gmail.com Requires-Python: >=3.7.1,<4.0.0 Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

