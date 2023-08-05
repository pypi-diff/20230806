# Comparing `tmp/happytransformer-2.4.1.tar.gz` & `tmp/happytransformer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/happytransformer-2.4.1.tar", last modified: Sun Feb  6 05:50:07 2022, max compression
+gzip compressed data, was "happytransformer-3.0.0.tar", last modified: Sat Aug  5 22:49:04 2023, max compression
```

## Comparing `happytransformer-2.4.1.tar` & `happytransformer-3.0.0.tar`

### file list

```diff
@@ -1,65 +1,28 @@
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/
--rw-r--r--   0 ericfillion   (501) staff       (20)     4583 2022-02-06 05:50:07.000000 happytransformer-2.4.1/PKG-INFO
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/
--rw-r--r--   0 ericfillion   (501) staff       (20)     2605 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_token_classification.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/sp/
--rw-r--r--   0 ericfillion   (501) staff       (20)      129 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/sp/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      239 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/sp/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      406 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/sp/trainer.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     3080 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_transformer.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/toc/
--rw-r--r--   0 ericfillion   (501) staff       (20)      134 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/toc/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)       59 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/toc/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      403 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/toc/trainer.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      122 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/cuda_detect.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     5372 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_text_classification.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     4420 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_text_to_text.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     1310 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/__init__.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/qa/
--rw-r--r--   0 ericfillion   (501) staff       (20)      129 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/qa/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      756 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/qa/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)    10378 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/qa/trainer.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/tc/
--rw-r--r--   0 ericfillion   (501) staff       (20)      129 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/tc/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      758 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/tc/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     8192 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/tc/trainer.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/gen/
--rw-r--r--   0 ericfillion   (501) staff       (20)      134 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/gen/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      905 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/gen/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     5896 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/gen/trainer.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/wp/
--rw-r--r--   0 ericfillion   (501) staff       (20)      130 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/wp/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      939 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/wp/default_args.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     6594 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/wp/trainer.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     2793 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/fine_tuning_util.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     6278 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_question_answering.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/adaptors/
--rw-r--r--   0 ericfillion   (501) staff       (20)      355 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/adaptors/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      302 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/adaptors/adaptor.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      565 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/adaptors/berts.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     2091 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_next_sentence.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     6599 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_generation.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     4265 2022-02-06 05:47:30.000000 happytransformer-2.4.1/happytransformer/happy_trainer.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer/tt/
--rw-r--r--   0 ericfillion   (501) staff       (20)       60 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/tt/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     7338 2022-02-06 05:47:30.000000 happytransformer-2.4.1/happytransformer/tt/trainer.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     3924 2022-02-06 05:01:25.000000 happytransformer-2.4.1/happytransformer/happy_word_prediction.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/tests/
--rw-r--r--   0 ericfillion   (501) staff       (20)     4352 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_tc.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      962 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_ns.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     4845 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_wp.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     4490 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_tt.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     1049 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_toc.py
--rw-r--r--   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/__init__.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     7204 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_gen.py
--rw-r--r--   0 ericfillion   (501) staff       (20)      828 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/shared_tests.py
--rw-r--r--   0 ericfillion   (501) staff       (20)     3917 2022-02-06 05:01:25.000000 happytransformer-2.4.1/tests/test_qa.py
-drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/
--rw-r--r--   0 ericfillion   (501) staff       (20)     4583 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/PKG-INFO
--rw-r--r--   0 ericfillion   (501) staff       (20)     1627 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/SOURCES.txt
--rw-r--r--   0 ericfillion   (501) staff       (20)      120 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/requires.txt
--rw-r--r--   0 ericfillion   (501) staff       (20)       23 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/top_level.txt
--rw-r--r--   0 ericfillion   (501) staff       (20)        1 2022-02-06 05:50:07.000000 happytransformer-2.4.1/happytransformer.egg-info/dependency_links.txt
--rw-r--r--   0 ericfillion   (501) staff       (20)     3092 2022-02-06 05:01:25.000000 happytransformer-2.4.1/README.md
--rw-r--r--   0 ericfillion   (501) staff       (20)     1561 2022-02-06 05:48:48.000000 happytransformer-2.4.1/setup.py
--rw-r--r--   0 ericfillion   (501) staff       (20)       79 2022-02-06 05:50:07.000000 happytransformer-2.4.1/setup.cfg
+drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2023-08-05 22:49:04.090412 happytransformer-3.0.0/
+-rw-r--r--   0 ericfillion   (501) staff       (20)    11342 2022-05-27 21:22:04.000000 happytransformer-3.0.0/LICENSE
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4003 2023-08-05 22:49:04.090496 happytransformer-3.0.0/PKG-INFO
+-rw-r--r--   0 ericfillion   (501) staff       (20)     3082 2023-08-05 22:42:03.000000 happytransformer-3.0.0/README.md
+drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2023-08-05 22:49:04.089184 happytransformer-3.0.0/happytransformer/
+-rw-r--r--   0 ericfillion   (501) staff       (20)      762 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/__init__.py
+drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2023-08-05 22:49:04.090296 happytransformer-3.0.0/happytransformer/adaptors/
+-rw-r--r--   0 ericfillion   (501) staff       (20)      355 2022-05-27 21:22:04.000000 happytransformer-3.0.0/happytransformer/adaptors/__init__.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)      201 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/adaptors/adaptor.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)      563 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/adaptors/berts.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     2222 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/args.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     5487 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/fine_tuning_util.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4225 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_generation.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     1950 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_next_sentence.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     5516 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_question_answering.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4176 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_text_classification.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4128 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_text_to_text.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     2146 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_token_classification.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)    13772 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_transformer.py
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4029 2023-08-05 22:42:04.000000 happytransformer-3.0.0/happytransformer/happy_word_prediction.py
+drwxr-xr-x   0 ericfillion   (501) staff       (20)        0 2023-08-05 22:49:04.089763 happytransformer-3.0.0/happytransformer.egg-info/
+-rw-r--r--   0 ericfillion   (501) staff       (20)     4003 2023-08-05 22:49:04.000000 happytransformer-3.0.0/happytransformer.egg-info/PKG-INFO
+-rw-r--r--   0 ericfillion   (501) staff       (20)      770 2023-08-05 22:49:04.000000 happytransformer-3.0.0/happytransformer.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfillion   (501) staff       (20)        1 2023-08-05 22:49:04.000000 happytransformer-3.0.0/happytransformer.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfillion   (501) staff       (20)      194 2023-08-05 22:49:04.000000 happytransformer-3.0.0/happytransformer.egg-info/requires.txt
+-rw-r--r--   0 ericfillion   (501) staff       (20)       17 2023-08-05 22:49:04.000000 happytransformer-3.0.0/happytransformer.egg-info/top_level.txt
+-rw-r--r--   0 ericfillion   (501) staff       (20)       79 2023-08-05 22:49:04.090770 happytransformer-3.0.0/setup.cfg
+-rw-r--r--   0 ericfillion   (501) staff       (20)     1652 2023-08-05 22:42:04.000000 happytransformer-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `happytransformer-2.4.1/PKG-INFO` & `happytransformer-3.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 Metadata-Version: 2.1
 Name: happytransformer
-Version: 2.4.1
-Summary: Happy Transformer is an API built on top of Hugging Face's Transformer library that makes it easy to utilize state-of-the-art NLP models.
+Version: 3.0.0
+Summary: Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference.
 Home-page: https://github.com/EricFillion/happy-transformer
 Author: The Happy Transformer Development Team
 Author-email: happytransformer@gmail.com
 License: Apache 2.0
-Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 
-        [![Downloads](https://pepy.tech/badge/happytransformer)](https://pepy.tech/project/happytransformer)
-        [![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://happytransformer.com)
-        ![PyPI](https://img.shields.io/pypi/v/happytransformer)
-        [![](https://github.com/EricFillion/happy-transformer/workflows/build/badge.svg)](https://github.com/EricFillion/happy-transformer/actions)
-        
-        # Happy Transformer 
-        **Documentation and news: [happytransformer.com](http://happytransformer.com)**
-        
-        New Course: Create a text generation web app. Also learn how to fine-tune GPT-Neo [link](https://www.udemy.com/course/nlp-text-generation-python-web-app/?couponCode=LAUNCH)
-        
-        
-        Join our Discord server: [![Support Server](https://img.shields.io/discord/839263772312862740.svg?label=Discord&logo=Discord&colorB=7289da&style=?style=flat-square&logo=appveyor)](https://discord.gg/psVwe3wfTb)
-        
-        
-        
-        ![HappyTransformer](logo.png)
-        
-        Happy Transformer is an package built on top of [Hugging Face's transformer library](https://huggingface.co/transformers/) that makes it easy to utilize state-of-the-art NLP models. 
-        
-        ## Features 
-          
-        | Public Methods                     | Basic Usage  | Training   |
-        |------------------------------------|--------------|------------|
-        | Text Generation                    | ✔            | ✔          |
-        | Text Classification                | ✔            | ✔          | 
-        | Word Prediction                    | ✔            | ✔          |
-        | Question Answering                 | ✔            | ✔          | 
-        | Text-to-Text                       | ✔            | ✔          | 
-        | Next Sentence Prediction           | ✔            |            | 
-        | Token Classification               | ✔            |            | 
-        
-        ## Quick Start
-        ```sh
-        pip install happytransformer
-        ```
-        
-        ```python
-        
-        from happytransformer import HappyWordPrediction
-        #--------------------------------------#
-        happy_wp = HappyWordPrediction()  # default uses distilbert-base-uncased
-        result = happy_wp.predict_mask("I think therefore I [MASK]")
-        print(result)  # [WordPredictionResult(token='am', score=0.10172799974679947)]
-        print(result[0].token)  # am
-        ```
-        
-        ## Maintainers
-        - [Eric Fillion](https://github.com/ericfillion)  Lead Maintainer
-        - [Ted Brownlow](https://github.com/ted537) Maintainer
-        
-        ## Tutorials 
-        [Text generation with training (GPT-Neo)](https://youtu.be/GzHJ3NUVtV4)
-        
-        [Text classification (training)](https://www.vennify.ai/train-text-classification-transformers/) 
-        
-        [Text classification (hate speech detection)](https://youtu.be/jti2sPQYzeQ) 
-        
-        [Text classification (sentiment analysis)](https://youtu.be/Ew72EAgM7FM)
-        
-        [Word prediction with training (DistilBERT, RoBERTa)](https://youtu.be/AWe0PHsPc_M)
-        
-        [Top T5 Models ](https://www.vennify.ai/top-t5-transformer-models/)
-        
-        [Grammar Correction](https://www.vennify.ai/grammar-correction-python/)
-        
-        [Fine-tune a Grammar Correction Model](https://www.vennify.ai/fine-tune-grammar-correction/)
-        
-Keywords: bert,roberta,xlnet,transformer,happy,HappyTransformer,classification,nlp,nlu,natural,language,processing,understanding
+Keywords: bert,roberta,ai,transformer,happy,HappyTransformer,classification,nlp,nlu,natural,language,processing,understanding
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 
+[![Downloads](https://pepy.tech/badge/happytransformer)](https://pepy.tech/project/happytransformer)
+[![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://happytransformer.com)
+![PyPI](https://img.shields.io/pypi/v/happytransformer)
+[![](https://github.com/EricFillion/happy-transformer/workflows/build/badge.svg)](https://github.com/EricFillion/happy-transformer/actions)
+
+# Happy Transformer 
+**Documentation and news: [happytransformer.com](http://happytransformer.com)**
+
+
+
+Join our Discord server: [![Support Server](https://img.shields.io/discord/839263772312862740.svg?label=Discord&logo=Discord&colorB=7289da&style=?style=flat-square&logo=appveyor)](https://discord.gg/psVwe3wfTb)
+
+
+
+![HappyTransformer](logo.png)
+
+Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference. 
+
+## 3.0.0 
+1. Deepspeed for training 
+2. Apple's MPS for training and inference 
+3. WandB to track training runs 
+4. Data supplied for training is automatically split into portions for training and evaluating
+5. Push models directly to Hugging Face's Model Hub
+
+Read about the full 3.0.0 update including breaking changes [here](https://happytransformer.com/news/). 
+
+
+## Tasks 
+  
+| Tasks                    | Inference | Training   |
+|--------------------------|-----------|------------|
+| Text Generation          | ✔         | ✔          |
+| Text Classification      | ✔         | ✔          | 
+| Word Prediction          | ✔         | ✔          |
+| Question Answering       | ✔         | ✔          | 
+| Text-to-Text             | ✔         | ✔          | 
+| Next Sentence Prediction | ✔         |            | 
+| Token Classification     | ✔         |            | 
+
+## Quick Start
+```sh
+pip install happytransformer
+```
+
+```python
+
+from happytransformer import HappyWordPrediction
+#--------------------------------------#
+happy_wp = HappyWordPrediction()  # default uses distilbert-base-uncased
+result = happy_wp.predict_mask("I think therefore I [MASK]")
+print(result)  # [WordPredictionResult(token='am', score=0.10172799974679947)]
+print(result[0].token)  # am
+```
+
+## Maintainers
+- [Eric Fillion](https://github.com/ericfillion)  Lead Maintainer
+- [Ted Brownlow](https://github.com/ted537) Maintainer
+
+
+## Tutorials 
+[Text generation with training (GPT-Neo)](https://youtu.be/GzHJ3NUVtV4)
+
+[Text classification (training)](https://www.vennify.ai/train-text-classification-transformers/) 
+
+[Text classification (hate speech detection)](https://youtu.be/jti2sPQYzeQ) 
+
+[Text classification (sentiment analysis)](https://youtu.be/Ew72EAgM7FM)
+
+[Word prediction with training (DistilBERT, RoBERTa)](https://youtu.be/AWe0PHsPc_M)
+
+[Top T5 Models ](https://www.vennify.ai/top-t5-transformer-models/)
+
+[Grammar Correction](https://www.vennify.ai/grammar-correction-python/)
+
+[Fine-tune a Grammar Correction Model](https://www.vennify.ai/fine-tune-grammar-correction/)
+
+
```

### Comparing `happytransformer-2.4.1/happytransformer/happy_token_classification.py` & `happytransformer-3.0.0/happytransformer/happy_token_classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-from typing import List, Optional
 from dataclasses import dataclass
+from typing import List, Union
 
-from transformers import TokenClassificationPipeline, AutoModelForTokenClassification
+from transformers import AutoModelForTokenClassification, TokenClassificationPipeline
 
-from happytransformer.happy_transformer import HappyTransformer
-from happytransformer.toc.trainer import TOCTrainer
-from happytransformer.cuda_detect import detect_cuda_device_number
 from happytransformer.adaptors import get_adaptor
-from happytransformer.toc import  ARGS_TOC_TRAIN, ARGS_TOC_EVAl, ARGS_TOC_TEST
-
+from happytransformer.happy_transformer import HappyTransformer
 
 @dataclass
 class TokenClassificationResult:
     word: str
     score: float
     entity: str
     index: int
     start: int
     end: int
 
 
 class HappyTokenClassification(HappyTransformer):
-    """
-    A user facing class for token classification
-    """
     def __init__(
-        self, model_type: str = "BERT", model_name: str = "dslim/bert-base-NER", load_path: str = "", use_auth_token: str = None):
+        self, model_type: str = "BERT", model_name: str = "dslim/bert-base-NER", load_path: str = "", use_auth_token: Union[bool, str] = None, trust_remote_code: bool =False):
 
         self.adaptor = get_adaptor(model_type)
+        model_class = AutoModelForTokenClassification
 
-        if load_path != "":
-            model = AutoModelForTokenClassification.from_pretrained(load_path)
-        else:
-            model = AutoModelForTokenClassification.from_pretrained(model_name, use_auth_token=use_auth_token)
-
+        super().__init__(model_type, model_name, model_class, use_auth_token=use_auth_token, load_path=load_path, trust_remote_code=trust_remote_code)
 
-        super().__init__(model_type, model_name, model, use_auth_token=use_auth_token, load_path=load_path)
+        self._type = "tok"
 
-        device_number = detect_cuda_device_number()
-
-        self._pipeline = TokenClassificationPipeline(model=self.model, tokenizer=self.tokenizer, device=device_number)
-
-        self._trainer = TOCTrainer(self.model, model_type, self.tokenizer, self._device, self.logger)
+        self._pipeline_class = TokenClassificationPipeline
 
     def classify_token(self, text: str) -> List[TokenClassificationResult]:
         """
         :param text: Text that contains tokens to be classified
         :return:
         """
+
+        # loads pipeline if it hasn't been loaded already.
+        self._load_pipeline()
+
         if not isinstance(text, str):
             raise ValueError('the "text" argument must be a single string')
         results = self._pipeline(text)
 
         return [
             TokenClassificationResult(
                 word=answer["word"],
@@ -61,15 +51,15 @@
                 start=answer["start"],
                 end=answer["end"],
             )
             for answer in results
         ]
 
 
-    def train(self, input_filepath, args=ARGS_TOC_TRAIN):
+    def train(self, input_filepath, args=None, eval_filepath: str = ""):
         raise NotImplementedError("train() is currently not available")
 
-    def eval(self, input_filepath, args=ARGS_TOC_EVAl):
+    def eval(self, input_filepath, args=None):
         raise NotImplementedError("eval() is currently not available")
 
-    def test(self, input_filepath, args=ARGS_TOC_TEST):
+    def test(self, input_filepath, args=None):
         raise NotImplementedError("test() is currently not available")
```

### Comparing `happytransformer-2.4.1/happytransformer/happy_text_to_text.py` & `happytransformer-3.0.0/happytransformer/happy_generation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,110 @@
-"""
-Contains a class called HappyTextToText which performs text to text generation
-"""
 from dataclasses import dataclass
+from typing import List, Union
 
-from transformers import Text2TextGenerationPipeline, AutoModelForSeq2SeqLM
+from datasets import Dataset
+from transformers import AutoModelForCausalLM, default_data_collator, TextGenerationPipeline
 
-from happytransformer.happy_transformer import HappyTransformer
-from happytransformer.tt.trainer import TTTrainer
-from happytransformer.cuda_detect import detect_cuda_device_number
 from happytransformer.adaptors import get_adaptor
-from happytransformer.tt.trainer import TTTrainArgs, TTEvalArgs, TTTestArgs
-
-
-@dataclass
-class TextToTextResult:
-    """
-    Returned when HappyTextToText.generate() is called
-    """
-    text: str
+from happytransformer.args import GENEvalArgs, GENTrainArgs
+from happytransformer.fine_tuning_util import csv_tok_text_gen_mlm, EvalResult, tok_text_gen_mlm
+from happytransformer.happy_transformer import HappyTransformer
 
 @dataclass
-class TTSettings:
-    """
-    Used to adjust the text generation algorithm that's used when
-    HappyTextToText.generate() is called 
-
-    """
+class GENSettings:
     min_length: int = 10
     max_length: int = 50
     do_sample: bool = False
     early_stopping: bool = False
     num_beams: int = 1
     temperature: float = 1
     top_k: int = 50
     no_repeat_ngram_size: int = 0
     top_p: float = 1
+    bad_words: List[str] = None
 
+@dataclass
+class GenerationResult:
+    text: str
 
-class HappyTextToText(HappyTransformer):
-    """
-    A user facing class for text to text generation
-    """
-    def __init__(self, model_type: str = "T5", model_name: str = "t5-small", load_path: str = "", use_auth_token: str = None):
+
+class HappyGeneration(HappyTransformer):
+    def __init__(self, model_type: str = "GPT2", model_name: str = "gpt2", 
+                 load_path: str = "", use_auth_token:  Union[bool, str]  = None, trust_remote_code: bool =False):
 
         self.adaptor = get_adaptor(model_type)
+        model_class = AutoModelForCausalLM
 
-        if load_path != "":
-            model = AutoModelForSeq2SeqLM.from_pretrained(load_path)
-        else:
-            model = AutoModelForSeq2SeqLM.from_pretrained(model_name, use_auth_token=use_auth_token)
+        super().__init__(model_type, model_name, model_class,  use_auth_token=use_auth_token, load_path=load_path, trust_remote_code=trust_remote_code)
 
+        self._data_collator = default_data_collator
 
-        super().__init__(model_type, model_name, model, use_auth_token=use_auth_token, load_path=load_path)
+        self._t_data_file_type = ["text", "csv"]
 
-        device_number = detect_cuda_device_number()
+        self._type = "gen"
 
-        self._pipeline = Text2TextGenerationPipeline(model=self.model,
-                                                     tokenizer=self.tokenizer, device=device_number)
+        self._pipeline_class = TextGenerationPipeline
 
-        self._trainer = TTTrainer(self.model, model_type, self.tokenizer, self._device, self.logger)
+    def load_model(self):
+        pass
 
 
     def __assert_default_text_is_val(self, text):
-        """
-        Ensures the input's text input is valid.
-        Raises a Value Error if the text input is not valid.
-        :param text: The value the user inputs for the "text" parameter
-        """
-
         if not isinstance(text, str):
             raise ValueError("The text input must be a string")
         if not text:
             raise ValueError("The text input must have at least one character")
 
 
-    def generate_text(self, text: str,
-                      args: TTSettings = TTSettings()) -> TextToTextResult:
-        """
-        :param text: starting text that the model uses as a prompt to continue it.
-        :param args: A TTSettings object
-        :return: A TextToTextResult() object
-        """
+    def generate_text(self, text: str, args: GENSettings=GENSettings()) -> GenerationResult:
+
+        # loads pipeline if it hasn't been loaded already.
+        self._load_pipeline()
+
         self.__assert_default_text_is_val(text)
+        input_ids = self.tokenizer.encode(text, return_tensors="pt")
+        adjusted_min_length = args.min_length + len(input_ids[0])
+        adjusted_max_length = args.max_length + len(input_ids[0])
+        if args.bad_words:
+            bad_words_ids = [self.tokenizer(" "+phrase.strip()).input_ids for phrase in args.bad_words]
+        else:
+            bad_words_ids = None
 
-        output = self._pipeline(text, min_length=args.min_length,
-                                max_length=args.max_length,
+        output = self._pipeline(text, min_length=adjusted_min_length,
+                                return_full_text=False,
+                                max_length=adjusted_max_length,
                                 do_sample=args.do_sample,
                                 early_stopping=args.early_stopping,
                                 num_beams=args.num_beams,
                                 temperature=args.temperature,
                                 top_k=args.top_k,
                                 no_repeat_ngram_size=args.no_repeat_ngram_size,
                                 top_p=args.top_p,
+                                bad_words_ids=bad_words_ids
                                 )
-        return TextToTextResult(text=output[0]['generated_text'])
+        return GenerationResult(text=output[0]['generated_text'])
+
+
+    def __post_process_generated_text(self, result, text):
+        return result[len(text):]
 
-    def train(self, input_filepath, args=TTTrainArgs()):
-        """
-        Trains the text-to-text model
-        input_filepath: a string that contains the location of a csv file
-        for training. Contains the following header values: text_1, text_2
-        args: A TTTrainArgs() object
-        return: None
-        """
-        self._trainer.train(input_filepath=input_filepath, dataclass_args=args)
-
-    def eval(self, input_filepath, args=TTEvalArgs()):
-        """
-        Evaluated the text-to-text model
-
-        input_filepath: a string that contains the location of a csv file
-        for training. Contains the following header values: text_1, text_2
-
-        args: A TTEvalArgs() object
-        return: an EvalResult() object
-        """
 
-        result = self._trainer.eval(input_filepath=input_filepath, dataclass_args=args)
-        return result
+    def train(self, input_filepath: str,  args: GENTrainArgs =GENTrainArgs(), eval_filepath: str =""):
+        super(HappyGeneration, self).train(input_filepath, args, eval_filepath)
 
+    def eval(self, input_filepath: str, args: GENEvalArgs =GENEvalArgs()) -> EvalResult:
+        return super(HappyGeneration, self).eval(input_filepath, args)
 
-    def test(self, input_filepath, args=TTTestArgs):
+    def test(self, input_filepath, args=None):
         raise NotImplementedError("test() is currently not available")
+
+    def _tok_function(self, raw_dataset: Dataset, args: Union[GENTrainArgs, GENEvalArgs], file_type: str) -> Dataset:
+
+        if file_type == "text":
+            return tok_text_gen_mlm(tokenizer=self.tokenizer, dataset=raw_dataset,  args=args,
+                                           mlm=False)
+        else:
+            return csv_tok_text_gen_mlm(tokenizer=self.tokenizer, dataset=raw_dataset, args=args,
+                                        mlm=False,
+                                        )
+
+
```

### Comparing `happytransformer-2.4.1/happytransformer/__init__.py` & `happytransformer-3.0.0/happytransformer/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,16 @@
 from happytransformer.happy_word_prediction import HappyWordPrediction
 from happytransformer.happy_text_classification import HappyTextClassification
 from happytransformer.happy_next_sentence import HappyNextSentence
 from happytransformer.happy_token_classification import HappyTokenClassification
 from happytransformer.happy_generation import HappyGeneration, GENSettings
 from happytransformer.happy_text_to_text import HappyTextToText, TTSettings
 
-from happytransformer.gen.default_args import ARGS_GEN_TRAIN, ARGS_GEN_EVAl
-from happytransformer.qa.default_args import ARGS_QA_TRAIN, ARGS_QA_EVAl, ARGS_QA_TEST
-from happytransformer.tc.default_args import ARGS_TC_TRAIN, ARGS_TC_EVAL, ARGS_TC_TEST
-from happytransformer.wp.default_args import ARGS_WP_TRAIN, ARGS_WP_EVAl
-
-from happytransformer.gen.trainer import GENTrainArgs, GENEvalArgs
-from happytransformer.qa.trainer import QATestArgs, QAEvalArgs, QATrainArgs
-from happytransformer.tc.trainer import TCTrainArgs, TCEvalArgs, TCTestArgs
-from happytransformer.wp.trainer import WPTrainArgs, WPEvalArgs
-from happytransformer.tt.trainer import TTTrainArgs, TTEvalArgs
-
-
-from happytransformer.happy_generation import (
-    HappyGeneration, GENSettings
+from happytransformer.args import (
+    GENTrainArgs, GENEvalArgs,
+    QATestArgs, QAEvalArgs, QATrainArgs,
+    TCTrainArgs, TCEvalArgs, TCTestArgs,
+    WPTrainArgs, WPEvalArgs,
+    TTTrainArgs, TTEvalArgs
 )
 
 name = "happytransformer"
```

### Comparing `happytransformer-2.4.1/happytransformer/happy_question_answering.py` & `happytransformer-3.0.0/happytransformer/happy_question_answering.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,144 @@
-"""
-Contains the HappyQuestionAnswering class.
-
-"""
-from typing import List
+import csv
 from dataclasses import dataclass
-from transformers import QuestionAnsweringPipeline, AutoModelForQuestionAnswering
+from typing import List, Union
 
-from happytransformer.happy_transformer import HappyTransformer
-from happytransformer.qa.trainer import QATrainer, QATrainArgs, QAEvalArgs, QATestArgs
-from happytransformer.happy_trainer import EvalResult
-from happytransformer.qa import ARGS_QA_TRAIN, ARGS_QA_EVAl, ARGS_QA_TEST
+from datasets import Dataset
+from transformers import AutoModelForQuestionAnswering, DataCollatorWithPadding, QuestionAnsweringPipeline
+from tqdm import tqdm
 
-from happytransformer.cuda_detect import detect_cuda_device_number
 from happytransformer.adaptors import get_adaptor
-from happytransformer.fine_tuning_util import create_args_dataclass
+from happytransformer.args import QAEvalArgs, QATestArgs, QATrainArgs
+from happytransformer.fine_tuning_util import EvalResult
+from happytransformer.happy_transformer import HappyTransformer
 
 @dataclass
 class QuestionAnsweringResult:
     answer: str
     score: float
     start: int
     end: int
 
 
 class HappyQuestionAnswering(HappyTransformer):
-    """
-    This class is a user facing class that allows users to solve question answering problems using
-    a transformer QA models. These models are able to answer a question given context for the
-    question by selecting a span within the context that answers the question.
-
-    The purpose of this class is to be lightweight and easy
-    to understand and to offload complex tasks to
-    other classes.
-    """
     def __init__(self, model_type="DISTILBERT",
                  model_name="distilbert-base-cased-distilled-squad", 
                  load_path: str = "",
-                 use_auth_token: str = None):
+                 use_auth_token: Union[bool, str] = None,
+                 trust_remote_code: bool=False
+                 ):
         
         self.adaptor = get_adaptor(model_type)
+        model_class = AutoModelForQuestionAnswering
 
-        if load_path != "":
-            model = AutoModelForQuestionAnswering.from_pretrained(load_path)
-        else:
-            model = AutoModelForQuestionAnswering.from_pretrained(model_name, use_auth_token=use_auth_token)
+        super().__init__(model_type, model_name, model_class,  use_auth_token=use_auth_token, load_path=load_path, trust_remote_code=trust_remote_code)
 
-        super().__init__(model_type, model_name, model, use_auth_token=use_auth_token, load_path=load_path)
-        device_number = detect_cuda_device_number()
+        self._pipeline_class = QuestionAnsweringPipeline
 
-        self._pipeline = QuestionAnsweringPipeline(model=self.model, tokenizer=self.tokenizer, device=device_number)
+        self._data_collator = DataCollatorWithPadding(self.tokenizer)
 
-        self._trainer = QATrainer(self.model, model_type, self.tokenizer, self._device, self.logger)
+        self._t_data_file_type = ["csv"]
+
+        self._type = "qa"
 
     def answer_question(self, context: str, question: str, top_k: int = 1) \
             -> List[QuestionAnsweringResult]:
-        """
-        Find the answers to a question.
-        The answer MUST be contained somewhere within the context for this to work.
-        top_k describes the number of answers to return.
-        """
 
-        pipeline_output = self._pipeline(context=context, question=question, topk=top_k)
+        # loads pipeline if it hasn't been loaded already.
+        self._load_pipeline()
+
+        pipeline_output = self._pipeline(context=context, question=question, top_k=top_k)
         # transformers returns a single dictionary when top_k ==1.
         # Our convention however is to have constant output format
         answers = [pipeline_output] if top_k == 1 else pipeline_output
 
         return [
             QuestionAnsweringResult(
                 answer=answer["answer"],
                 score=answer["score"],
                 start=answer["start"],
                 end=answer["end"],)
             for answer in answers
         ]
 
-    def train(self, input_filepath, args=QATrainArgs()):
-        """
-        Trains the question answering model
-
-        input_filepath: a string that contains the location of a csv file
-        for training. Contains the following header values: context,
-        question, answer_text, answer_start
-
-        args: Either a QATrainArgs() object or a dictionary that contains all of the same keys as ARGS_QA_TRAIN
-
-        return: None
-        """
-
-        if type(args) == dict:
-            method_dataclass_args = create_args_dataclass(default_dic_args=ARGS_QA_TRAIN,
-                                                                input_dic_args=args,
-                                                                method_dataclass_args=QATrainArgs)
-        elif type(args) == QATrainArgs:
-            method_dataclass_args = args
-        else:
-            raise ValueError("Invalid args type. Use a QATrainArgs object or a dictionary")
-
-
-        self._trainer.train(input_filepath=input_filepath, dataclass_args=method_dataclass_args)
+    def train(self, input_filepath, args: QATrainArgs =QATrainArgs(), eval_filepath: str = ""):
+        super(HappyQuestionAnswering, self).train(input_filepath, args, eval_filepath)
 
     def eval(self, input_filepath, args=QAEvalArgs()) -> EvalResult:
-        """
-        Trains the question answering model
-
-        input_filepath: a string that contains the location of a csv file
-        for training. Contains the following header values:
-        context, question, answer_text, answer_start
 
-        args: Either a QAEvalArgs() object or a dictionary that contains all of the same keys as ARGS_QA_EVAl
+        return super(HappyQuestionAnswering, self).eval(input_filepath, args)
 
-        return: A dictionary that contains a key called "eval_loss"
 
-        """
+    def test(self, input_filepath, args=QATestArgs()):
         if type(args) == dict:
-            method_dataclass_args = create_args_dataclass(default_dic_args=ARGS_QA_EVAl,
-                                                                input_dic_args=args,
-                                                                method_dataclass_args=QAEvalArgs)
-        elif type(args) == QAEvalArgs:
-            method_dataclass_args = args
-        else:
-            raise ValueError("Invalid args type. Use a QAEvalArgs object or a dictionary")
+            raise ValueError( "As of version 2.5.0 dictionary inputs are not acceptable. Please provide a QATestArgs. ")
 
-        return self._trainer.eval(input_filepath=input_filepath, dataclass_args=method_dataclass_args)
+        contexts, questions = self._get_data(input_filepath, test_data=True)
 
+        return [
+            self.answer_question(context, question)[0]
+            for context, question in
+            tqdm(zip(contexts, questions))
+        ]
 
-    def test(self, input_filepath, args=QATestArgs()):
-        """
-        Tests the question answering model. Used to obtain results
-
-        input_filepath: a string that contains the location of a csv file
-        for training. Contains the following header values:
-        context, question
-
-        args: Either a QATestArgs() object or a dictionary that contains all of the same keys as ARGS_QA_TEST
-
-        return: A list of dictionaries. Each dictionary
-        contains the keys: "score", "start", "end" and "answer"
-        """
-        if type(args) == dict:
-            method_dataclass_args = create_args_dataclass(default_dic_args=ARGS_QA_TEST,
-                                                                input_dic_args=args,
-                                                                method_dataclass_args=QATestArgs)
-        elif type(args) == QATestArgs:
-            method_dataclass_args = args
-        else:
-            raise ValueError("Invalid args type. Use a QATestArgs object or a dictionary")
-
+    def _tok_function(self, raw_dataset, args: QATrainArgs, file_type: str) -> Dataset:
 
-        return self._trainer.test(input_filepath=input_filepath, solve=self.answer_question, dataclass_args=method_dataclass_args)
+        def __preprocess_function(case):
+            case["answer_start"] = int(case['answer_start'])
+            gold_text = case['answer_text']
+            start_idx = case['answer_start']
+            end_idx = start_idx + len(gold_text)
+
+            # todo (maybe): strip answer['text'] (remove white space from start and end)
+            # sometimes squad answers are off by a character or two – fix this
+            if case["context"][start_idx:end_idx] == gold_text:
+                case['answer_end'] = end_idx
+            elif case["context"][start_idx - 1:end_idx - 1] == gold_text:
+                case["context"]['answer_start'] = start_idx - 1
+                case["context"]['answer_end'] = end_idx - 1
+            elif case[start_idx - 2:end_idx - 2] == gold_text:
+                case["context"]['answer_start'] = start_idx - 2
+                case["context"]['answer_end'] = end_idx - 2
+
+            encodings = self.tokenizer(case["context"], case["question"], truncation=True, padding=True)
+
+            start_position = encodings.char_to_token(case['answer_start'])
+            end_position =  encodings.char_to_token(case['answer_end'] - 1)
+            if start_position is None:
+                start_position = self.tokenizer.model_max_length
+            if end_position is None:
+                end_position = self.tokenizer.model_max_length
+
+            encodings.update({'start_positions': start_position, 'end_positions': end_position})
+
+            return encodings
+
+
+        tok_dataset = raw_dataset.map(
+            __preprocess_function,
+            batched=False,
+            remove_columns=["context", "question", "answer_text", "answer_start"],
+            desc="Tokenizing data"
+        )
+
+        return tok_dataset
+
+    @staticmethod
+    def _get_data(filepath, test_data=False):
+        contexts = []
+        questions = []
+        answers = []
+        with open(filepath, newline='', encoding="utf-8") as csv_file:
+            reader = csv.DictReader(csv_file)
+            for row in reader:
+                contexts.append(row['context'])
+                questions.append(row['question'])
+                if not test_data:
+                    answer = {}
+                    answer["answer_text"] = row['answer_text']
+                    answer["answer_start"] = int(row['answer_start'])
+                    answers.append(answer)
+        csv_file.close()
+
+        if not test_data:
+            return contexts, questions, answers
+        return contexts, questions
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `happytransformer-2.4.1/happytransformer/adaptors/berts.py` & `happytransformer-3.0.0/happytransformer/adaptors/berts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from .adaptor import Adaptor
 
-
-
 class RobertaAdaptor(Adaptor):
 
     @staticmethod
     def preprocess_mask_text(text: str) -> str:
         return text.replace('[MASK]', '<mask>')
 
     @staticmethod
```

### Comparing `happytransformer-2.4.1/happytransformer/happy_word_prediction.py` & `happytransformer-3.0.0/happytransformer/happy_word_prediction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-from typing import List, Optional
 from dataclasses import dataclass
+from datasets import Dataset
+from typing import List, Optional, Union
 
-from transformers import FillMaskPipeline, AutoModelForMaskedLM, PretrainedConfig
+from transformers import AutoModelForMaskedLM, DataCollatorForLanguageModeling, FillMaskPipeline
 
-from happytransformer.happy_transformer import HappyTransformer
-from happytransformer.wp.trainer import WPTrainer, WPTrainArgs, WPEvalArgs
-from happytransformer.cuda_detect import detect_cuda_device_number
 from happytransformer.adaptors import get_adaptor
-from happytransformer.wp import ARGS_WP_TRAIN, ARGS_WP_EVAl, ARGS_WP_TEST
-from happytransformer.happy_trainer import EvalResult
-from happytransformer.fine_tuning_util import create_args_dataclass
+from happytransformer.args import WPEvalArgs, WPTrainArgs
+from happytransformer.fine_tuning_util import EvalResult, tok_text_gen_mlm, csv_tok_text_gen_mlm
+from happytransformer.happy_transformer import HappyTransformer
+
 
 @dataclass
 class WordPredictionResult:
     token: str
     score: float
 
 class HappyWordPrediction(HappyTransformer):
     """
     A user facing class for text classification
     """
     def __init__(
             self, model_type: str = "DISTILBERT", model_name: str = "distilbert-base-uncased",
-            load_path: str ="", use_auth_token: str = None):
-
+            load_path: str ="", use_auth_token: Union[bool, str] = None, trust_remote_code: bool =False):
 
         self.adaptor = get_adaptor(model_type)
+        model_class = AutoModelForMaskedLM
 
-        if load_path != "":
-            model = AutoModelForMaskedLM.from_pretrained(load_path)
-        else:
-            model = AutoModelForMaskedLM.from_pretrained(model_name, use_auth_token=use_auth_token)
 
-        super().__init__(model_type, model_name, model, load_path=load_path, use_auth_token=use_auth_token)
+        super().__init__(model_type, model_name, model_class, load_path=load_path, use_auth_token=use_auth_token, trust_remote_code=trust_remote_code)
 
-        device_number = detect_cuda_device_number()
 
-        self._pipeline = FillMaskPipeline(model=self.model, tokenizer=self.tokenizer, device=device_number)
+        self._pipeline_class = FillMaskPipeline
 
-        self._trainer = WPTrainer(self.model, model_type, self.tokenizer, self._device, self.logger)
+        # mlm_probability is modified to the train args value within HappyTransformer._run_eval() and HappyTransformer._run_eval()
+        self._data_collator = DataCollatorForLanguageModeling(tokenizer=self.tokenizer,
+                                                        mlm_probability=0.1)
+        self._t_data_file_type = ["text", "csv"]
+        self._type = "wp"
 
     def predict_mask(self, text: str, targets: Optional[List[str]] = None, top_k: int = 1) -> List[WordPredictionResult]:
         """
         Predict [MASK] tokens in a string.
         targets limit possible guesses if supplied.
         top_k describes number of targets to return*
         *top_k does not apply if targets is supplied
         """
+
+        # loads pipeline if it hasn't been loaded already.
+        self._load_pipeline()
+
+
         if not isinstance(text, str):
             raise ValueError('the "text" argument must be a single string')
 
         text_for_pipeline = self.adaptor.preprocess_mask_text(text)
         answers = self._pipeline(
             text_for_pipeline, 
             targets=targets, top_k=top_k
@@ -61,35 +64,37 @@
             WordPredictionResult(
                 token=fix_token(answer["token_str"]), 
                 score=answer["score"]
             )
             for answer in answers
         ]
 
-    def train(self, input_filepath, args=ARGS_WP_TRAIN):
-        if type(args) == dict:
-            method_dataclass_args = create_args_dataclass(default_dic_args=ARGS_WP_TRAIN,
-                                                         input_dic_args=args,
-                                                         method_dataclass_args=WPTrainArgs)
-        elif type(args) == WPTrainArgs:
-            method_dataclass_args = args
-        else:
-            raise ValueError("Invalid args type. Use a WPTrainArgs object or a dictionary")
-
-        self._trainer.train(input_filepath=input_filepath, dataclass_args=method_dataclass_args)
+    def train(self, input_filepath: str,  args: WPTrainArgs =WPTrainArgs(), eval_filepath: str = ""):
+        super(HappyWordPrediction, self).train(input_filepath, args, eval_filepath)
 
-    def eval(self, input_filepath, args=ARGS_WP_EVAl) -> EvalResult:
-        if type(args) == dict:
+    def eval(self, input_filepath, args: WPEvalArgs = WPEvalArgs()) -> EvalResult:
+        return super(HappyWordPrediction, self).eval(input_filepath, args)
 
-            method_dataclass_args = create_args_dataclass(default_dic_args=ARGS_WP_EVAl,
-                                                         input_dic_args=args,
-                                                         method_dataclass_args=WPEvalArgs)
-        elif type(args) == WPEvalArgs:
-            method_dataclass_args = args
-        else:
-            raise ValueError("Invalid args type. Use a ARGS_WP_EVAl object or a dictionary")
 
-        return self._trainer.eval(input_filepath=input_filepath, dataclass_args=method_dataclass_args)
+    def test(self, input_filepath, args=None):
+        raise NotImplementedError("test() is currently not available")
 
+    def _tok_function(self, raw_dataset, args: Union[WPTrainArgs, WPEvalArgs], file_type: str) -> Dataset:
 
-    def test(self, input_filepath, args=ARGS_WP_TEST):
-        raise NotImplementedError("test() is currently not available")
+        if file_type == "text":
+            if not args.line_by_line:
+                return tok_text_gen_mlm(tokenizer=self.tokenizer, dataset=raw_dataset, args=args,
+                                        mlm=True)
+            else:
+                def tokenize_function(example):
+                    return self.tokenizer(example["text"],
+                                     add_special_tokens=True, truncation=True)
+
+                tokenized_dataset = raw_dataset.map(tokenize_function, batched=True,
+                                                remove_columns=["text"])
+                return tokenized_dataset
+        else:
+            return csv_tok_text_gen_mlm(tokenizer=self.tokenizer,
+                                        dataset=raw_dataset,
+                                        args=args,
+                                        mlm=True
+                                        )
```

### Comparing `happytransformer-2.4.1/happytransformer.egg-info/PKG-INFO` & `happytransformer-3.0.0/happytransformer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,99 @@
 Metadata-Version: 2.1
 Name: happytransformer
-Version: 2.4.1
-Summary: Happy Transformer is an API built on top of Hugging Face's Transformer library that makes it easy to utilize state-of-the-art NLP models.
+Version: 3.0.0
+Summary: Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference.
 Home-page: https://github.com/EricFillion/happy-transformer
 Author: The Happy Transformer Development Team
 Author-email: happytransformer@gmail.com
 License: Apache 2.0
-Description: [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 
-        [![Downloads](https://pepy.tech/badge/happytransformer)](https://pepy.tech/project/happytransformer)
-        [![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://happytransformer.com)
-        ![PyPI](https://img.shields.io/pypi/v/happytransformer)
-        [![](https://github.com/EricFillion/happy-transformer/workflows/build/badge.svg)](https://github.com/EricFillion/happy-transformer/actions)
-        
-        # Happy Transformer 
-        **Documentation and news: [happytransformer.com](http://happytransformer.com)**
-        
-        New Course: Create a text generation web app. Also learn how to fine-tune GPT-Neo [link](https://www.udemy.com/course/nlp-text-generation-python-web-app/?couponCode=LAUNCH)
-        
-        
-        Join our Discord server: [![Support Server](https://img.shields.io/discord/839263772312862740.svg?label=Discord&logo=Discord&colorB=7289da&style=?style=flat-square&logo=appveyor)](https://discord.gg/psVwe3wfTb)
-        
-        
-        
-        ![HappyTransformer](logo.png)
-        
-        Happy Transformer is an package built on top of [Hugging Face's transformer library](https://huggingface.co/transformers/) that makes it easy to utilize state-of-the-art NLP models. 
-        
-        ## Features 
-          
-        | Public Methods                     | Basic Usage  | Training   |
-        |------------------------------------|--------------|------------|
-        | Text Generation                    | ✔            | ✔          |
-        | Text Classification                | ✔            | ✔          | 
-        | Word Prediction                    | ✔            | ✔          |
-        | Question Answering                 | ✔            | ✔          | 
-        | Text-to-Text                       | ✔            | ✔          | 
-        | Next Sentence Prediction           | ✔            |            | 
-        | Token Classification               | ✔            |            | 
-        
-        ## Quick Start
-        ```sh
-        pip install happytransformer
-        ```
-        
-        ```python
-        
-        from happytransformer import HappyWordPrediction
-        #--------------------------------------#
-        happy_wp = HappyWordPrediction()  # default uses distilbert-base-uncased
-        result = happy_wp.predict_mask("I think therefore I [MASK]")
-        print(result)  # [WordPredictionResult(token='am', score=0.10172799974679947)]
-        print(result[0].token)  # am
-        ```
-        
-        ## Maintainers
-        - [Eric Fillion](https://github.com/ericfillion)  Lead Maintainer
-        - [Ted Brownlow](https://github.com/ted537) Maintainer
-        
-        ## Tutorials 
-        [Text generation with training (GPT-Neo)](https://youtu.be/GzHJ3NUVtV4)
-        
-        [Text classification (training)](https://www.vennify.ai/train-text-classification-transformers/) 
-        
-        [Text classification (hate speech detection)](https://youtu.be/jti2sPQYzeQ) 
-        
-        [Text classification (sentiment analysis)](https://youtu.be/Ew72EAgM7FM)
-        
-        [Word prediction with training (DistilBERT, RoBERTa)](https://youtu.be/AWe0PHsPc_M)
-        
-        [Top T5 Models ](https://www.vennify.ai/top-t5-transformer-models/)
-        
-        [Grammar Correction](https://www.vennify.ai/grammar-correction-python/)
-        
-        [Fine-tune a Grammar Correction Model](https://www.vennify.ai/fine-tune-grammar-correction/)
-        
-Keywords: bert,roberta,xlnet,transformer,happy,HappyTransformer,classification,nlp,nlu,natural,language,processing,understanding
+Keywords: bert,roberta,ai,transformer,happy,HappyTransformer,classification,nlp,nlu,natural,language,processing,understanding
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 
+[![Downloads](https://pepy.tech/badge/happytransformer)](https://pepy.tech/project/happytransformer)
+[![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://happytransformer.com)
+![PyPI](https://img.shields.io/pypi/v/happytransformer)
+[![](https://github.com/EricFillion/happy-transformer/workflows/build/badge.svg)](https://github.com/EricFillion/happy-transformer/actions)
+
+# Happy Transformer 
+**Documentation and news: [happytransformer.com](http://happytransformer.com)**
+
+
+
+Join our Discord server: [![Support Server](https://img.shields.io/discord/839263772312862740.svg?label=Discord&logo=Discord&colorB=7289da&style=?style=flat-square&logo=appveyor)](https://discord.gg/psVwe3wfTb)
+
+
+
+![HappyTransformer](logo.png)
+
+Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference. 
+
+## 3.0.0 
+1. Deepspeed for training 
+2. Apple's MPS for training and inference 
+3. WandB to track training runs 
+4. Data supplied for training is automatically split into portions for training and evaluating
+5. Push models directly to Hugging Face's Model Hub
+
+Read about the full 3.0.0 update including breaking changes [here](https://happytransformer.com/news/). 
+
+
+## Tasks 
+  
+| Tasks                    | Inference | Training   |
+|--------------------------|-----------|------------|
+| Text Generation          | ✔         | ✔          |
+| Text Classification      | ✔         | ✔          | 
+| Word Prediction          | ✔         | ✔          |
+| Question Answering       | ✔         | ✔          | 
+| Text-to-Text             | ✔         | ✔          | 
+| Next Sentence Prediction | ✔         |            | 
+| Token Classification     | ✔         |            | 
+
+## Quick Start
+```sh
+pip install happytransformer
+```
+
+```python
+
+from happytransformer import HappyWordPrediction
+#--------------------------------------#
+happy_wp = HappyWordPrediction()  # default uses distilbert-base-uncased
+result = happy_wp.predict_mask("I think therefore I [MASK]")
+print(result)  # [WordPredictionResult(token='am', score=0.10172799974679947)]
+print(result[0].token)  # am
+```
+
+## Maintainers
+- [Eric Fillion](https://github.com/ericfillion)  Lead Maintainer
+- [Ted Brownlow](https://github.com/ted537) Maintainer
+
+
+## Tutorials 
+[Text generation with training (GPT-Neo)](https://youtu.be/GzHJ3NUVtV4)
+
+[Text classification (training)](https://www.vennify.ai/train-text-classification-transformers/) 
+
+[Text classification (hate speech detection)](https://youtu.be/jti2sPQYzeQ) 
+
+[Text classification (sentiment analysis)](https://youtu.be/Ew72EAgM7FM)
+
+[Word prediction with training (DistilBERT, RoBERTa)](https://youtu.be/AWe0PHsPc_M)
+
+[Top T5 Models ](https://www.vennify.ai/top-t5-transformer-models/)
+
+[Grammar Correction](https://www.vennify.ai/grammar-correction-python/)
+
+[Fine-tune a Grammar Correction Model](https://www.vennify.ai/fine-tune-grammar-correction/)
+
+
```

### Comparing `happytransformer-2.4.1/README.md` & `happytransformer-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,45 @@
 [![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](http://happytransformer.com)
 ![PyPI](https://img.shields.io/pypi/v/happytransformer)
 [![](https://github.com/EricFillion/happy-transformer/workflows/build/badge.svg)](https://github.com/EricFillion/happy-transformer/actions)
 
 # Happy Transformer 
 **Documentation and news: [happytransformer.com](http://happytransformer.com)**
 
-New Course: Create a text generation web app. Also learn how to fine-tune GPT-Neo [link](https://www.udemy.com/course/nlp-text-generation-python-web-app/?couponCode=LAUNCH)
 
 
 Join our Discord server: [![Support Server](https://img.shields.io/discord/839263772312862740.svg?label=Discord&logo=Discord&colorB=7289da&style=?style=flat-square&logo=appveyor)](https://discord.gg/psVwe3wfTb)
 
 
 
 ![HappyTransformer](logo.png)
 
-Happy Transformer is an package built on top of [Hugging Face's transformer library](https://huggingface.co/transformers/) that makes it easy to utilize state-of-the-art NLP models. 
+Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference. 
 
-## Features 
+## 3.0.0 
+1. Deepspeed for training 
+2. Apple's MPS for training and inference 
+3. WandB to track training runs 
+4. Data supplied for training is automatically split into portions for training and evaluating
+5. Push models directly to Hugging Face's Model Hub
+
+Read about the full 3.0.0 update including breaking changes [here](https://happytransformer.com/news/). 
+
+
+## Tasks 
   
-| Public Methods                     | Basic Usage  | Training   |
-|------------------------------------|--------------|------------|
-| Text Generation                    | ✔            | ✔          |
-| Text Classification                | ✔            | ✔          | 
-| Word Prediction                    | ✔            | ✔          |
-| Question Answering                 | ✔            | ✔          | 
-| Text-to-Text                       | ✔            | ✔          | 
-| Next Sentence Prediction           | ✔            |            | 
-| Token Classification               | ✔            |            | 
+| Tasks                    | Inference | Training   |
+|--------------------------|-----------|------------|
+| Text Generation          | ✔         | ✔          |
+| Text Classification      | ✔         | ✔          | 
+| Word Prediction          | ✔         | ✔          |
+| Question Answering       | ✔         | ✔          | 
+| Text-to-Text             | ✔         | ✔          | 
+| Next Sentence Prediction | ✔         |            | 
+| Token Classification     | ✔         |            | 
 
 ## Quick Start
 ```sh
 pip install happytransformer
 ```
 
 ```python
@@ -45,14 +54,15 @@
 print(result[0].token)  # am
 ```
 
 ## Maintainers
 - [Eric Fillion](https://github.com/ericfillion)  Lead Maintainer
 - [Ted Brownlow](https://github.com/ted537) Maintainer
 
+
 ## Tutorials 
 [Text generation with training (GPT-Neo)](https://youtu.be/GzHJ3NUVtV4)
 
 [Text classification (training)](https://www.vennify.ai/train-text-classification-transformers/) 
 
 [Text classification (hate speech detection)](https://youtu.be/jti2sPQYzeQ)
```

### Comparing `happytransformer-2.4.1/setup.py` & `happytransformer-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 import pathlib
 
 current_location = pathlib.Path(__file__).parent
 readme = (current_location / "README.md").read_text()
 
 setup(
     name = 'happytransformer',
-    packages = find_packages(),
-    version = '2.4.1',
+    packages = find_packages(exclude=("tests",)),
+    version = '3.0.0',
     license='Apache 2.0',
-    description = "Happy Transformer is an API built on top of Hugging Face's Transformer library that makes it easy to utilize state-of-the-art NLP models.",
+    description = "Happy Transformer makes it easy to fine-tune NLP Transformer models and use them for inference.",
     long_description= readme,
     long_description_content_type='text/markdown',
     author = "The Happy Transformer Development Team",
     author_email = 'happytransformer@gmail.com',
     url = 'https://github.com/EricFillion/happy-transformer',
-    keywords = ['bert', 'roberta', 'xlnet', "transformer", "happy", "HappyTransformer",  "classification",  "nlp", "nlu", "natural", "language", "processing", "understanding"],
+    keywords = ['bert', 'roberta', 'ai', "transformer", "happy", "HappyTransformer",  "classification",  "nlp", "nlu", "natural", "language", "processing", "understanding"],
 
     install_requires=[
             'torch>=1.0',
             'tqdm>=4.43',
-            'transformers>=4.4.0',
-            'datasets>=1.6.0',
+            'transformers>=4.30.1,<5.0.0',
+            'datasets>=2.13.1,<3.0.0',
             'dataclasses; python_version < "3.7"',
             'sentencepiece',
-            'protobuf'
-
+            'protobuf',
+            'accelerate>=0.20.1,<1.0.0',
+            'tokenizers>=0.13.3,<1.0.0',
+            'wandb'
     ],
     classifiers=[
         'Intended Audience :: Developers',
         "Intended Audience :: Science/Research",
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

