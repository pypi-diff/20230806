# Comparing `tmp/text2text-1.2.7.tar.gz` & `tmp/text2text-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.2.7.tar", last modified: Sun Jul  9 03:33:52 2023, max compression
+gzip compressed data, was "text2text-1.2.8.tar", last modified: Sat Aug  5 00:58:40 2023, max compression
```

## Comparing `text2text-1.2.7.tar` & `text2text-1.2.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.854973 text2text-1.2.7/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-07-09 03:20:10.000000 text2text-1.2.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    56465 2023-07-09 03:33:52.854973 text2text-1.2.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    55651 2023-07-09 03:32:54.000000 text2text-1.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 03:33:52.854973 text2text-1.2.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1283 2023-07-09 03:30:48.000000 text2text-1.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.848972 text2text-1.2.7/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      603 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.850972 text2text-1.2.7/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/indexer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.852973 text2text-1.2.7/text2text/langchain/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-09 03:21:56.000000 text2text-1.2.7/text2text/langchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/langchain/stfidf.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-09 03:21:32.000000 text2text-1.2.7/text2text/langchain/test_stfidf.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-09 03:21:49.000000 text2text-1.2.7/text2text/langchain/test_text2text_assistant.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/langchain/text2text_assistant.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.853973 text2text-1.2.7/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-07-09 03:21:25.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-07-09 03:20:10.000000 text2text-1.2.7/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:33:52.850972 text2text-1.2.7/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56465 2023-07-09 03:33:52.000000 text2text-1.2.7/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-07-09 03:33:52.000000 text2text-1.2.7/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 03:33:52.000000 text2text-1.2.7/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-09 03:33:52.000000 text2text-1.2.7/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-09 03:33:52.000000 text2text-1.2.7/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.657386 text2text-1.2.8/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-08-04 23:42:14.000000 text2text-1.2.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-08-05 00:58:40.656386 text2text-1.2.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    55862 2023-08-05 00:06:29.000000 text2text-1.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 00:58:40.657386 text2text-1.2.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1283 2023-08-05 00:55:46.000000 text2text-1.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.649385 text2text-1.2.8/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      603 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-08-05 00:00:07.000000 text2text-1.2.8/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.652385 text2text-1.2.8/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/indexer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.653385 text2text-1.2.8/text2text/langchain/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/langchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/langchain/stfidf.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/langchain/test_stfidf.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/langchain/test_text2text_assistant.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/langchain/text2text_assistant.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.655386 text2text-1.2.8/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-08-04 23:42:14.000000 text2text-1.2.8/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 00:58:40.651385 text2text-1.2.8/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-08-05 00:58:40.000000 text2text-1.2.8/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-08-05 00:58:40.000000 text2text-1.2.8/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 00:58:40.000000 text2text-1.2.8/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-05 00:58:40.000000 text2text-1.2.8/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-05 00:58:40.000000 text2text-1.2.8/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.2.7/LICENSE.txt` & `text2text-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/PKG-INFO` & `text2text-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.7
+Version: 1.2.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,15 @@
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
 ## Colab Notebooks
+* Assistant (free private chatGPT alternative) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K6Kk80w9vjFZ7PL9dPRgVuOPuaWcY4ae?usp=sharing)
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
```

### Comparing `text2text-1.2.7/README.md` & `text2text-1.2.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
 ## Colab Notebooks
+* Assistant (free private chatGPT alternative) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K6Kk80w9vjFZ7PL9dPRgVuOPuaWcY4ae?usp=sharing)
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
```

### Comparing `text2text-1.2.7/setup.py` & `text2text-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.2.7",
+  version="1.2.8",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.2.7/text2text/__init__.py` & `text2text-1.2.8/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/abstractor.py` & `text2text-1.2.8/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/answerer.py` & `text2text-1.2.8/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/assistant.py` & `text2text-1.2.8/text2text/assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pandas as pd
+import logging
 import text2text as t2t
-from transformers import AutoTokenizer
+from transformers import AutoTokenizer, logging
 from auto_gptq import AutoGPTQForCausalLM
 
+logging.set_verbosity(logging.CRITICAL)
+
 class Assistant(t2t.Transformer):
 
   def __init__(self, **kwargs):
-    model_name_or_path = kwargs.get("model_name_or_path", "TheBloke/vicuna-13b-v1.3-GPTQ")
-    model_basename = kwargs.get("model_basename", "vicuna-13b-v1.3-GPTQ-4bit-128g.no-act.order")
+    model_name_or_path = kwargs.get("model_name_or_path", "TheBloke/vicuna-13B-v1.5-16K-GPTQ")
 
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, use_fast=True)
 
     self.__class__.model = AutoGPTQForCausalLM.from_quantized(model_name_or_path,
-      model_basename=model_basename,
       use_safetensors=True,
       trust_remote_code=False,
       device="cuda:0",
       use_triton=False,
       quantize_config=None
     )
 
@@ -27,17 +28,17 @@
       df["input_line"] = self._translate_lines(df["input_line"].tolist(), src_lang, 'en')
     if retriever:
       k = kwargs.get('k', 1)
       df["knowledge"] = retriever.retrieve(df["input_line"].str.lower().tolist(), k=k)
       df["input_line"] = df["knowledge"].apply(' '.join) + " - " + df["input_line"]
     df["input_line"] = "USER: " + df["input_line"] + "\nASSISTANT:"
     temperature = kwargs.get('temperature', 0.7)
-    top_p = kwargs.get('top_p', 0.9)
+    top_p = kwargs.get('top_p', 0.95)
     top_k = kwargs.get('top_k', 0)
-    repetition_penalty = kwargs.get('repetition_penalty', 1.1)
+    repetition_penalty = kwargs.get('repetition_penalty', 1.15)
     max_new_tokens = kwargs.get('max_new_tokens', 512)
     tok = self.__class__.tokenizer
     m = self.__class__.model
 
     input_ids = tok(df["input_line"].tolist(), return_tensors="pt", padding=True).input_ids
     input_ids = input_ids.to(m.device)
     generate_kwargs = dict(
```

### Comparing `text2text-1.2.7/text2text/biunilm/loader_utils.py` & `text2text-1.2.8/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/biunilm/seq2seq_loader.py` & `text2text-1.2.8/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/bm25er.py` & `text2text-1.2.8/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/counter.py` & `text2text-1.2.8/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/fitter.py` & `text2text-1.2.8/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/handler.py` & `text2text-1.2.8/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/identifier.py` & `text2text-1.2.8/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/indexer.py` & `text2text-1.2.8/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/langchain/stfidf.py` & `text2text-1.2.8/text2text/langchain/stfidf.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/langchain/test_stfidf.py` & `text2text-1.2.8/text2text/langchain/test_stfidf.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/langchain/text2text_assistant.py` & `text2text-1.2.8/text2text/langchain/text2text_assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/measurer.py` & `text2text-1.2.8/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.2.8/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.2.8/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.2.8/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.2.8/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.2.8/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/questioner.py` & `text2text-1.2.8/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/server.py` & `text2text-1.2.8/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/summarizer.py` & `text2text-1.2.8/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/tfidfer.py` & `text2text-1.2.8/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/tokenizer.py` & `text2text-1.2.8/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/transformer.py` & `text2text-1.2.8/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/translator.py` & `text2text-1.2.8/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text/vectorizer.py` & `text2text-1.2.8/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.2.7/text2text.egg-info/PKG-INFO` & `text2text-1.2.8/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.2.7
+Version: 1.2.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,15 @@
 * [Citation](https://github.com/artitw/text2text#citation)
 * [Contributing](https://github.com/artitw/text2text#contributing)
 * [Code of Conduct](https://github.com/artitw/text2text#code-of-conduct)
 
 </details>
 
 ## Colab Notebooks
+* Assistant (free private chatGPT alternative) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1K6Kk80w9vjFZ7PL9dPRgVuOPuaWcY4ae?usp=sharing)
 * Assistant with knowledge base [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 * STF-IDF multilingual search [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 * All examples [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR)
 
 ## How Crosslingual Models Work (click to watch)
 [![Crosslingual Models](http://img.youtube.com/vi/caZLVcJqsqo/0.jpg)](https://youtu.be/caZLVcJqsqo "Cross-Lingual Models")
```

### Comparing `text2text-1.2.7/text2text.egg-info/SOURCES.txt` & `text2text-1.2.8/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

