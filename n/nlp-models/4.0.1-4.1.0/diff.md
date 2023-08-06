# Comparing `tmp/nlp-models-4.0.1.tar.gz` & `tmp/nlp-models-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-4.0.1.tar", last modified: Tue Aug  1 07:32:36 2023, max compression
+gzip compressed data, was "nlp-models-4.1.0.tar", last modified: Sun Aug  6 12:51:34 2023, max compression
```

## Comparing `nlp-models-4.0.1.tar` & `nlp-models-4.1.0.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.442026 nlp-models-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 07:32:24.000000 nlp-models-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-01 07:32:36.442026 nlp-models-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-01 07:32:24.000000 nlp-models-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 07:32:24.000000 nlp-models-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-01 07:32:36.442026 nlp-models-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 07:32:24.000000 nlp-models-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.438026 nlp-models-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.438026 nlp-models-4.0.1/src/nlp_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.442026 nlp-models-4.0.1/src/nlp_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.442026 nlp-models-4.0.1/src/nlp_models/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.442026 nlp-models-4.0.1/src/nlp_models/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/llm/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/llm/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/llm/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.442026 nlp-models-4.0.1/src/nlp_models/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-08-01 07:32:24.000000 nlp-models-4.0.1/src/nlp_models/multi_task_model/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 07:32:36.438026 nlp-models-4.0.1/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-08-01 07:32:36.000000 nlp-models-4.0.1/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-01 07:32:36.000000 nlp-models-4.0.1/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 07:32:36.000000 nlp-models-4.0.1/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 07:32:36.000000 nlp-models-4.0.1/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 07:32:36.000000 nlp-models-4.0.1/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.649653 nlp-models-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-06 12:51:21.000000 nlp-models-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-06 12:51:34.653653 nlp-models-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-06 12:51:21.000000 nlp-models-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-06 12:51:21.000000 nlp-models-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-06 12:51:34.653653 nlp-models-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 12:51:21.000000 nlp-models-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.641653 nlp-models-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.641653 nlp-models-4.1.0/src/nlp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.645653 nlp-models-4.1.0/src/nlp_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.645653 nlp-models-4.1.0/src/nlp_models/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.645653 nlp-models-4.1.0/src/nlp_models/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/cmd/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.649653 nlp-models-4.1.0/src/nlp_models/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/llm/vectordbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.649653 nlp-models-4.1.0/src/nlp_models/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-08-06 12:51:21.000000 nlp-models-4.1.0/src/nlp_models/multi_task_model/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:51:34.641653 nlp-models-4.1.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 12:51:34.000000 nlp-models-4.1.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-4.0.1/LICENSE` & `nlp-models-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/PKG-INFO` & `nlp-models-4.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 4.0.1
+Version: 4.1.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -26,20 +26,27 @@
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 
 # NLP Models
 
 A repository for building transformer based nlp models
 
-## Run Llama2 Chat UI on CPU
+## Run Llama2 on consumer CPU
+
+### Run Chat UI on CPU
 ```
 cd pipelines/nlp_models/
 streamlit run app.py
 ```
 
+### Run Chat cmd line on CPU
+```
+llm_app chat -s 'hi there'
+```
+
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
 
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
@@ -47,19 +54,21 @@
    An implementation of multi-tasking model built on encoder models
 
    - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
    - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
-## Other Example Notebooks
-
+3. `GPT-2`
 - [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
-- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+4. `Falcon 7B`
+- [Running Falcon 7b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_7b.ipynb)
+5. Quantized Llama2 models
+- [Run Llama2 chat on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+- [Run Llama2 QA on a custom pdf document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/07_llama2_doc_qa.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 4.0.1 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 4.1.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -14,32 +14,35 @@
 pypi.python.org/pypi/nlp-models/) [![Python package](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/python-package.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
-transformer based nlp models ## Run Llama2 Chat UI on CPU ``` cd pipelines/
-nlp_models/ streamlit run app.py ``` ## Models 1. bert_classifier A wrapper
-package around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
-finetuning/01_a_classification_model_training_example.ipynb) - [Inference
-example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
-classification-finetuning/01_b_classification_inference_example.ipynb) 2.
-multi_task_model An implementation of multi-tasking model built on encoder
-models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
-blob/master/notebooks/02_multi-task-model/
-02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
-training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+transformer based nlp models ## Run Llama2 on consumer CPU ### Run Chat UI on
+CPU ``` cd pipelines/nlp_models/ streamlit run app.py ``` ### Run Chat cmd line
+on CPU ``` llm_app chat -s 'hi there' ``` ## Models 1. bert_classifier A
+wrapper package around BERT-based classification models - [Training example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_a_classification_model_training_example.ipynb) -
+[Inference example](https://github.com/minggnim/nlp-models/blob/master/
+notebooks/01_bert-classification-finetuning/
+01_b_classification_inference_example.ipynb) 2. multi_task_model An
+implementation of multi-tasking model built on encoder models - [Zero-shot
+multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb) - [Training
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-
+task-model/02_b_multitask_model_training_example.ipynb) - [Inference example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-
+model/02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https:
+//github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) 3. `GPT-2` - [Training GPT-2 model](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-
+training/03_gpt2_training.ipynb) 4. `Falcon 7B` - [Running Falcon 7b model]
 (https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
-05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
-## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
-Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
-install -r requirements ```
+05_falcon_7b.ipynb) 5. Quantized Llama2 models - [Run Llama2 chat on CPU]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+06_llama2_langchain_gglm_inference.ipynb) - [Run Llama2 QA on a custom pdf
+document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+04_llms/07_llama2_doc_qa.ipynb) ## Installation ### Install from PyPi ``` pip
+install nlp-models ``` ### Install from source ``` git clone git@github.com:
+minggnim/nlp-models.git pip install -r requirements ```
```

### Comparing `nlp-models-4.0.1/README.md` & `nlp-models-4.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,27 @@
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 
 # NLP Models
 
 A repository for building transformer based nlp models
 
-## Run Llama2 Chat UI on CPU
+## Run Llama2 on consumer CPU
+
+### Run Chat UI on CPU
 ```
 cd pipelines/nlp_models/
 streamlit run app.py
 ```
 
+### Run Chat cmd line on CPU
+```
+llm_app chat -s 'hi there'
+```
+
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
 
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
@@ -25,19 +32,21 @@
    An implementation of multi-tasking model built on encoder models
 
    - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
    - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
-## Other Example Notebooks
-
+3. `GPT-2`
 - [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
-- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+4. `Falcon 7B`
+- [Running Falcon 7b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_7b.ipynb)
+5. Quantized Llama2 models
+- [Run Llama2 chat on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+- [Run Llama2 QA on a custom pdf document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/07_llama2_doc_qa.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -4,32 +4,35 @@
 pypi.python.org/pypi/nlp-models/) [![Python package](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/python-package.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
-transformer based nlp models ## Run Llama2 Chat UI on CPU ``` cd pipelines/
-nlp_models/ streamlit run app.py ``` ## Models 1. bert_classifier A wrapper
-package around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
-finetuning/01_a_classification_model_training_example.ipynb) - [Inference
-example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
-classification-finetuning/01_b_classification_inference_example.ipynb) 2.
-multi_task_model An implementation of multi-tasking model built on encoder
-models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
-blob/master/notebooks/02_multi-task-model/
-02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
-training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+transformer based nlp models ## Run Llama2 on consumer CPU ### Run Chat UI on
+CPU ``` cd pipelines/nlp_models/ streamlit run app.py ``` ### Run Chat cmd line
+on CPU ``` llm_app chat -s 'hi there' ``` ## Models 1. bert_classifier A
+wrapper package around BERT-based classification models - [Training example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_a_classification_model_training_example.ipynb) -
+[Inference example](https://github.com/minggnim/nlp-models/blob/master/
+notebooks/01_bert-classification-finetuning/
+01_b_classification_inference_example.ipynb) 2. multi_task_model An
+implementation of multi-tasking model built on encoder models - [Zero-shot
+multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb) - [Training
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-
+task-model/02_b_multitask_model_training_example.ipynb) - [Inference example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-
+model/02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https:
+//github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) 3. `GPT-2` - [Training GPT-2 model](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-
+training/03_gpt2_training.ipynb) 4. `Falcon 7B` - [Running Falcon 7b model]
 (https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
-05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
-## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
-Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
-install -r requirements ```
+05_falcon_7b.ipynb) 5. Quantized Llama2 models - [Run Llama2 chat on CPU]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+06_llama2_langchain_gglm_inference.ipynb) - [Run Llama2 QA on a custom pdf
+document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+04_llms/07_llama2_doc_qa.ipynb) ## Installation ### Install from PyPi ``` pip
+install nlp-models ``` ### Install from source ``` git clone git@github.com:
+minggnim/nlp-models.git pip install -r requirements ```
```

### Comparing `nlp-models-4.0.1/setup.cfg` & `nlp-models-4.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 4.0.1
+version = 4.1.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -35,11 +35,15 @@
 [options.packages.find]
 where = src
 
 [options.extras_require]
 full = 
 	tqdm
 
+[options.entry_points]
+console_scripts = 
+	llm_app = nlp_models.cmd.cli:cli
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `nlp-models-4.0.1/src/nlp_models/base/data.py` & `nlp-models-4.1.0/src/nlp_models/base/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/base/io.py` & `nlp-models-4.1.0/src/nlp_models/base/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/base/layers.py` & `nlp-models-4.1.0/src/nlp_models/base/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/base/metrics.py` & `nlp-models-4.1.0/src/nlp_models/base/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/base/utils.py` & `nlp-models-4.1.0/src/nlp_models/base/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/bert_classifier/bert.py` & `nlp-models-4.1.0/src/nlp_models/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/bert_classifier/predict.py` & `nlp-models-4.1.0/src/nlp_models/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/bert_classifier/train.py` & `nlp-models-4.1.0/src/nlp_models/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/llm/prompts.py` & `nlp-models-4.1.0/src/nlp_models/llm/prompts.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,7 +16,25 @@
 Human: {human_input}
 Assistant:"""
 
         self.chat_prompt = PromptTemplate(input_variables=["history", "human_input"], template=self.chat_template)
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.chat_prompt
+
+
+class QAPrompt:
+    def __init__(self) -> None:
+        self.qa_template = """Use the following pieces of information to answer the user's question.
+If you don't know the answer, just say that you don't know, don't try to make up an answer.
+
+Context: {context}
+Question: {question}
+
+Only return the helpful answer below and nothing else.
+Helpful answer:
+"""
+
+        self.qa_prompt = PromptTemplate(input_variables=['context', 'question'], template=self.qa_template)
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.qa_prompt
```

### Comparing `nlp-models-4.0.1/src/nlp_models/multi_task_model/mtl.py` & `nlp-models-4.1.0/src/nlp_models/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models/multi_task_model/trainer.py` & `nlp-models-4.1.0/src/nlp_models/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-4.0.1/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-4.1.0/src/nlp_models.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 4.0.1
+Version: 4.1.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -26,20 +26,27 @@
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 
 # NLP Models
 
 A repository for building transformer based nlp models
 
-## Run Llama2 Chat UI on CPU
+## Run Llama2 on consumer CPU
+
+### Run Chat UI on CPU
 ```
 cd pipelines/nlp_models/
 streamlit run app.py
 ```
 
+### Run Chat cmd line on CPU
+```
+llm_app chat -s 'hi there'
+```
+
 ## Models
 
 1. bert_classifier
    A wrapper package around BERT-based classification models
 
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_a_classification_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-finetuning/01_b_classification_inference_example.ipynb)
@@ -47,19 +54,21 @@
    An implementation of multi-tasking model built on encoder models
 
    - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb)
    - [Training example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_b_multitask_model_training_example.ipynb)
    - [Inference example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_c_multitask_model_inference_example.ipynb)
    - [Qqrant Vector DB](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/02_d_qdrant_vector_db.ipynb)
 
-## Other Example Notebooks
-
+3. `GPT-2`
 - [Training GPT-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-training/03_gpt2_training.ipynb)
-- [Running Falcon 4b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_4b.ipynb)
-- [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+4. `Falcon 7B`
+- [Running Falcon 7b model](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/05_falcon_7b.ipynb)
+5. Quantized Llama2 models
+- [Run Llama2 chat on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
+- [Run Llama2 QA on a custom pdf document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/07_llama2_doc_qa.ipynb)
 
 ## Installation
 
 ### Install from PyPi
 
 ```
 pip install nlp-models
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 4.0.1 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 4.1.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
@@ -14,32 +14,35 @@
 pypi.python.org/pypi/nlp-models/) [![Python package](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/python-package.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/python-package.yml) [![Dependency Review](https://github.com/
 minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/
 badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/
 workflows/dependency-review.yml) # NLP Models A repository for building
-transformer based nlp models ## Run Llama2 Chat UI on CPU ``` cd pipelines/
-nlp_models/ streamlit run app.py ``` ## Models 1. bert_classifier A wrapper
-package around BERT-based classification models - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-classification-
-finetuning/01_a_classification_model_training_example.ipynb) - [Inference
-example](https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
-classification-finetuning/01_b_classification_inference_example.ipynb) 2.
-multi_task_model An implementation of multi-tasking model built on encoder
-models - [Zero-shot multi-task model](https://github.com/minggnim/nlp-models/
-blob/master/notebooks/02_multi-task-model/
-02_a_multitask_model_zeroshot_learning.ipynb) - [Training example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_b_multitask_model_training_example.ipynb) - [Inference example](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https://
-github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
-02_d_qdrant_vector_db.ipynb) ## Other Example Notebooks - [Training GPT-
-2 model](https://github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-
-training/gpt-2-training/03_gpt2_training.ipynb) - [Running Falcon 4b model]
+transformer based nlp models ## Run Llama2 on consumer CPU ### Run Chat UI on
+CPU ``` cd pipelines/nlp_models/ streamlit run app.py ``` ### Run Chat cmd line
+on CPU ``` llm_app chat -s 'hi there' ``` ## Models 1. bert_classifier A
+wrapper package around BERT-based classification models - [Training example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/01_bert-
+classification-finetuning/01_a_classification_model_training_example.ipynb) -
+[Inference example](https://github.com/minggnim/nlp-models/blob/master/
+notebooks/01_bert-classification-finetuning/
+01_b_classification_inference_example.ipynb) 2. multi_task_model An
+implementation of multi-tasking model built on encoder models - [Zero-shot
+multi-task model](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+02_multi-task-model/02_a_multitask_model_zeroshot_learning.ipynb) - [Training
+example](https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-
+task-model/02_b_multitask_model_training_example.ipynb) - [Inference example]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-
+model/02_c_multitask_model_inference_example.ipynb) - [Qqrant Vector DB](https:
+//github.com/minggnim/nlp-models/blob/master/notebooks/02_multi-task-model/
+02_d_qdrant_vector_db.ipynb) 3. `GPT-2` - [Training GPT-2 model](https://
+github.com/minggnim/nlp-models/blob/master/notebooks/03_gpt-2-training/gpt-2-
+training/03_gpt2_training.ipynb) 4. `Falcon 7B` - [Running Falcon 7b model]
 (https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
-05_falcon_4b.ipynb) - [Run Llama2 chat on cpu](https://github.com/minggnim/nlp-
-models/blob/master/notebooks/04_llms/06_llama2_langchain_gglm_inference.ipynb)
-## Installation ### Install from PyPi ``` pip install nlp-models ``` ###
-Install from source ``` git clone git@github.com:minggnim/nlp-models.git pip
-install -r requirements ```
+05_falcon_7b.ipynb) 5. Quantized Llama2 models - [Run Llama2 chat on CPU]
+(https://github.com/minggnim/nlp-models/blob/master/notebooks/04_llms/
+06_llama2_langchain_gglm_inference.ipynb) - [Run Llama2 QA on a custom pdf
+document on CPU](https://github.com/minggnim/nlp-models/blob/master/notebooks/
+04_llms/07_llama2_doc_qa.ipynb) ## Installation ### Install from PyPi ``` pip
+install nlp-models ``` ### Install from source ``` git clone git@github.com:
+minggnim/nlp-models.git pip install -r requirements ```
```

### Comparing `nlp-models-4.0.1/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-4.1.0/src/nlp_models.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/nlp_models/__init__.py
 src/nlp_models.egg-info/PKG-INFO
 src/nlp_models.egg-info/SOURCES.txt
 src/nlp_models.egg-info/dependency_links.txt
+src/nlp_models.egg-info/entry_points.txt
 src/nlp_models.egg-info/requires.txt
 src/nlp_models.egg-info/top_level.txt
 src/nlp_models/base/__init__.py
 src/nlp_models/base/data.py
 src/nlp_models/base/io.py
 src/nlp_models/base/layers.py
 src/nlp_models/base/loss.py
 src/nlp_models/base/metrics.py
 src/nlp_models/base/utils.py
 src/nlp_models/bert_classifier/__init__.py
 src/nlp_models/bert_classifier/bert.py
 src/nlp_models/bert_classifier/predict.py
 src/nlp_models/bert_classifier/train.py
+src/nlp_models/cmd/__init__.py
+src/nlp_models/cmd/cli.py
 src/nlp_models/llm/__init__.py
+src/nlp_models/llm/apps.py
 src/nlp_models/llm/base.py
 src/nlp_models/llm/llms.py
 src/nlp_models/llm/prompts.py
+src/nlp_models/llm/vectordbs.py
 src/nlp_models/multi_task_model/__init__.py
 src/nlp_models/multi_task_model/mtl.py
 src/nlp_models/multi_task_model/trainer.py
```

