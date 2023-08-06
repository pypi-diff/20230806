# Comparing `tmp/JanexPT-0.0.2.tar.gz` & `tmp/JanexPT-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanexPT-0.0.2.tar", last modified: Sun Aug  6 12:42:31 2023, max compression
+gzip compressed data, was "JanexPT-0.0.3.tar", last modified: Sun Aug  6 12:48:56 2023, max compression
```

## Comparing `JanexPT-0.0.2.tar` & `JanexPT-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT/
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT/JanexSub/
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.2/JanexPT/JanexSub/JanexSub.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.2/JanexPT/JanexSub/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 15:15:17.000000 JanexPT-0.0.2/JanexPT/__init__.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-05 15:58:06.000000 JanexPT-0.0.2/JanexPT/chat.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     3754 2023-08-05 16:12:24.000000 JanexPT-0.0.2/JanexPT/main.py
--rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-06 12:38:40.000000 JanexPT-0.0.2/JanexPT/train.py
-drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:42:31.604591 JanexPT-0.0.2/JanexPT.egg-info/
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/SOURCES.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/dependency_links.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/requires.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-06 12:42:31.000000 JanexPT-0.0.2/JanexPT.egg-info/top_level.txt
--rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-05 14:49:33.000000 JanexPT-0.0.2/LICENSE
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:42:31.604591 JanexPT-0.0.2/PKG-INFO
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1500 2023-08-05 16:10:30.000000 JanexPT-0.0.2/README.md
--rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-06 12:42:31.604591 JanexPT-0.0.2/setup.cfg
--rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-06 12:42:24.000000 JanexPT-0.0.2/setup.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:48:56.064851 JanexPT-0.0.3/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:48:56.064851 JanexPT-0.0.3/JanexPT/
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:48:56.064851 JanexPT-0.0.3/JanexPT/JanexSub/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.3/JanexPT/JanexSub/JanexSub.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        0 2023-08-05 14:49:33.000000 JanexPT-0.0.3/JanexPT/JanexSub/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-05 15:15:17.000000 JanexPT-0.0.3/JanexPT/__init__.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      252 2023-08-05 15:58:06.000000 JanexPT-0.0.3/JanexPT/chat.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     3998 2023-08-06 12:48:21.000000 JanexPT-0.0.3/JanexPT/main.py
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     4414 2023-08-06 12:38:40.000000 JanexPT-0.0.3/JanexPT/train.py
+drwxr-xr-x   0 cipher    (1000) cipher    (1000)        0 2023-08-06 12:48:56.064851 JanexPT-0.0.3/JanexPT.egg-info/
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:48:56.000000 JanexPT-0.0.3/JanexPT.egg-info/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)      307 2023-08-06 12:48:56.000000 JanexPT-0.0.3/JanexPT.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        1 2023-08-06 12:48:56.000000 JanexPT-0.0.3/JanexPT.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       20 2023-08-06 12:48:56.000000 JanexPT-0.0.3/JanexPT.egg-info/requires.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)        8 2023-08-06 12:48:56.000000 JanexPT-0.0.3/JanexPT.egg-info/top_level.txt
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     2930 2023-08-05 14:49:33.000000 JanexPT-0.0.3/LICENSE
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1892 2023-08-06 12:48:56.064851 JanexPT-0.0.3/PKG-INFO
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1500 2023-08-05 16:10:30.000000 JanexPT-0.0.3/README.md
+-rw-r--r--   0 cipher    (1000) cipher    (1000)       38 2023-08-06 12:48:56.064851 JanexPT-0.0.3/setup.cfg
+-rw-r--r--   0 cipher    (1000) cipher    (1000)     1312 2023-08-06 12:48:52.000000 JanexPT-0.0.3/setup.py
```

### Comparing `JanexPT-0.0.2/JanexPT/main.py` & `JanexPT-0.0.3/JanexPT/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,22 @@
 import random
 import json
 
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset, DataLoader
 
+IM = IntentMatcher("intents.json", "thesaurus.json")
+
+def tokenize(sentence):
+    input_string = sentence
+    return IM.tokenize(input_string)
 
 def stem(word):
-    return stemmer.stem(word.lower())
+    return IM.stem(word.lower())
 
 def bag_of_words(tokenized_sentence, words):
     # stem each word
     sentence_words = [stem(word) for word in tokenized_sentence]
     # initialize bag with 0 for each word
     bag = np.zeros(len(words), dtype=np.float32)
     for idx, w in enumerate(words):
@@ -64,15 +69,19 @@
         return self.n_samples
 
 class JanexPT:
     def __init__(self, intents_file_path, thesaurus_file_path, UIName):
         self.intents_file_path = intents_file_path
         self.thesaurus_file_path = thesaurus_file_path
         self.FILE = "data.pth"
-        self.data = torch.load(self.FILE)
+        try:
+            self.data = torch.load(self.FILE)
+        except:
+            self.trainpt()
+            self.data = torch.load(self.FILE)
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.input_size = self.data["input_size"]
         self.hidden_size = self.data["hidden_size"]
         self.output_size = self.data["output_size"]
         self.all_words = self.data['all_words']
         self.tags = self.data['tags']
         self.model_state = self.data["model_state"]
```

### Comparing `JanexPT-0.0.2/JanexPT/train.py` & `JanexPT-0.0.3/JanexPT/train.py`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.2/JanexPT.egg-info/PKG-INFO` & `JanexPT-0.0.3/JanexPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.2/LICENSE` & `JanexPT-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.2/PKG-INFO` & `JanexPT-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JanexPT
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/Cipher58/Janex-Pytorch
 Download-URL: https://github.com/Cipher58/Janex-Pytorch
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `JanexPT-0.0.2/README.md` & `JanexPT-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `JanexPT-0.0.2/setup.py` & `JanexPT-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="JanexPT",
 
     # version of the module
-    version="0.0.2",
+    version="0.0.3",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Janex-Pytorch',
 
     # your Email address
```

