# Comparing `tmp/SNgramExtractor-0.0.5.tar.gz` & `tmp/SNgramExtractor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SNgramExtractor-0.0.5.tar", last modified: Sun Jan  1 17:45:10 2023, max compression
+gzip compressed data, was "dist/SNgramExtractor-0.0.6.tar", last modified: Sun Aug  6 13:59:09 2023, max compression
```

## Comparing `SNgramExtractor-0.0.5.tar` & `SNgramExtractor-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-01-01 17:45:10.000000 SNgramExtractor-0.0.5/
--rw-rw-r--   0 azim      (1000) azim      (1000)     4968 2023-01-01 17:45:10.000000 SNgramExtractor-0.0.5/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-01-01 17:45:10.000000 SNgramExtractor-0.0.5/setup.cfg
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-01-01 17:45:10.000000 SNgramExtractor-0.0.5/src/
--rw-rw-r--   0 azim      (1000) azim      (1000)     4161 2020-06-04 14:41:02.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.py
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-01-01 17:45:10.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/
--rw-r--r--   0 azim      (1000) azim      (1000)     4968 2023-01-01 17:45:09.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)       29 2023-01-01 17:45:09.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/requires.txt
--rw-r--r--   0 azim      (1000) azim      (1000)      274 2023-01-01 17:45:09.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/SOURCES.txt
--rw-r--r--   0 azim      (1000) azim      (1000)       16 2023-01-01 17:45:09.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/top_level.txt
--rw-r--r--   0 azim      (1000) azim      (1000)        1 2023-01-01 17:45:09.000000 SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/dependency_links.txt
--rw-r--r--   0 azim      (1000) azim      (1000)     4600 2023-01-01 17:43:49.000000 SNgramExtractor-0.0.5/README.rst
--rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 SNgramExtractor-0.0.5/LICENSE
--rw-r--r--   0 azim      (1000) azim      (1000)      767 2023-01-01 17:43:27.000000 SNgramExtractor-0.0.5/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:59:09.256487 SNgramExtractor-0.0.6/
+-rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 SNgramExtractor-0.0.6/LICENSE
+-rw-rw-r--   0 azim      (1000) azim      (1000)     5673 2023-08-06 13:59:09.260487 SNgramExtractor-0.0.6/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)     4620 2023-08-06 13:58:42.000000 SNgramExtractor-0.0.6/README.rst
+-rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-08-06 13:59:09.260487 SNgramExtractor-0.0.6/setup.cfg
+-rw-r--r--   0 azim      (1000) azim      (1000)      767 2023-08-06 13:57:19.000000 SNgramExtractor-0.0.6/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:59:09.248487 SNgramExtractor-0.0.6/src/
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:59:09.256487 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/
+-rw-r--r--   0 azim      (1000) azim      (1000)     5673 2023-08-06 13:59:09.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)      274 2023-08-06 13:59:09.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)        1 2023-08-06 13:59:09.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       29 2023-08-06 13:59:09.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/requires.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       16 2023-08-06 13:59:09.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.egg-info/top_level.txt
+-rw-rw-r--   0 azim      (1000) azim      (1000)     4161 2020-06-04 14:41:02.000000 SNgramExtractor-0.0.6/src/SNgramExtractor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SNgramExtractor-0.0.5/PKG-INFO` & `SNgramExtractor-0.0.6/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: SNgramExtractor
-Version: 0.0.5
-Summary: Implementation of syntactic n-grams (sn-gram) extraction
-Home-page: https://github.com/StatguyUser/SNgramExtractor
-Author: StatguyUser
-License: UNKNOWN
-Download-URL: https://github.com/StatguyUser/SNgramExtractor.git
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 What is it?
 ===========
 
-Companion library of machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
+Companion library of machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
 
 SNgramExtractor module helps extract Syntactic relations (SR tags) as elements of sn-grams. 
 
 We follow the path marked by the arrows in the dependencies and obtain sngrams.[1]
 
 The advantage of syntactic n-grams (SN-grams), i.e., n-grams that are constructed using paths in syntactic trees, is that they are less arbitrary than traditional n-grams. Thus, their number is less than the number of traditional n-grams. Besides, they can be interpreted as linguistic phenomenon, while traditional n-grams have no plausible linguistic interpretation they are merely statistical artifact. [1]
 
@@ -76,15 +64,15 @@
 ================
 
 `pip install SNgramExtractor`
 
 How to cite?
 ================
 
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
+Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
 
 Dependencies
 ============
 
  - [spacy](https://spacy.io/)
  - [spacy model en_core_web_sm](https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.2.0/en_core_web_sm-2.2.0.tar.gz)
 
@@ -93,9 +81,7 @@
 
 1. [Syntactic Dependency-Based N-grams as Classification Features](http://www.icsd.aegean.gr/lecturers/stamatatos/papers/MICAI2012.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
 2. [Syntactic N-grams as Machine Learning Features for Natural Language Processing](http://www.cic.ipn.mx/~sidorov/Synt_n_grams_ESWA_FINAL.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
 3. [Dependency-Based Open Information Extraction](http://www.anthology.aclweb.org/W/W12/W12-0702.pdf) by Pablo Gamallo, Marcos Garcia and Santiago Fernandez-Lanza
 4. [Query Understanding Enhanced By Hierarchical Parsing Structures](https://groups.csail.mit.edu/sls/publications/2013/Liu_ASRU_2013.pdf) by Jingjing Liu, Panupong Pasupat, Yining Wang, Scott Cyphers, and Jim Glass
 5. [Dependency Structure Trees in Syntax Based Machine Translation](http://www.cs.cmu.edu/~vamshi/publications/DependencyMT_report.pdf) by Vamshi Ambati
 6. [Question Answering Passage Retrieval Using Dependency Relations](https://www.comp.nus.edu.sg/~kanmy/papers/f66-cui.pdf) by Hang Cui, Renxu Sun, Keya Li, Min-Yen Kan and Tat-Seng Chua
-
-
```

### Comparing `SNgramExtractor-0.0.5/src/SNgramExtractor.py` & `SNgramExtractor-0.0.6/src/SNgramExtractor.py`

 * *Files identical despite different names*

### Comparing `SNgramExtractor-0.0.5/src/SNgramExtractor.egg-info/PKG-INFO` & `SNgramExtractor-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,98 @@
 Metadata-Version: 2.1
 Name: SNgramExtractor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of syntactic n-grams (sn-gram) extraction
 Home-page: https://github.com/StatguyUser/SNgramExtractor
 Author: StatguyUser
 License: UNKNOWN
 Download-URL: https://github.com/StatguyUser/SNgramExtractor.git
+Description: What is it?
+        ===========
+        
+        Companion library of machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
+        
+        SNgramExtractor module helps extract Syntactic relations (SR tags) as elements of sn-grams. 
+        
+        We follow the path marked by the arrows in the dependencies and obtain sngrams.[1]
+        
+        The advantage of syntactic n-grams (SN-grams), i.e., n-grams that are constructed using paths in syntactic trees, is that they are less arbitrary than traditional n-grams. Thus, their number is less than the number of traditional n-grams. Besides, they can be interpreted as linguistic phenomenon, while traditional n-grams have no plausible linguistic interpretation they are merely statistical artifact. [1]
+        
+        SN-gram has usability across many natural language processing application areas, such as classification tasks in machine learning[2], information extraction[3], query understanding[4], machine translation[5], question answering systems[6]
+        
+        Input parameters
+        ================
+        
+          - **text** input text as a single sentence.
+          - **meta_tag** Resultant bigram and trigram should be concatenated with part of speech tag('pos') or dependency tag('dep') or original SN-gram('original')
+          - **trigram_flag** if we need to include trigrams derived from SN-grams as well ('yes') or not ('no'). Default is 'yes'
+          - **nlp_model** Specify the spacy language model you want to use. Default is spacy English language model en_core_web_sm. This is useful for being able to use languages other than english.
+        
+        Output
+        ================
+        
+        Dictionary object with key value pairs for bigram and trigram derived from SN-gram.
+        
+          - **SNBigram** dictionary key for bigram derived from SN-gram
+          - **SNTrigram** dictionary key for trigram derived from SN-gram
+        
+        How to use is it?
+        =================
+        
+        ```python
+        
+        from SNgramExtractor import SNgramExtractor
+        
+        text='Economic news have little effect on financial markets.'    
+        SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=None)
+        output=SNgram_obj.get_SNgram()
+        print(text)
+        print('SNGram bigram:',output['SNBigram'])
+        print('SNGram trigram:',output['SNTrigram'])
+        
+        print('-----------------------------------')
+        text='every cloud has a silver lining'
+        SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=None)
+        output=SNgram_obj.get_SNgram()
+        print(text)
+        print('SNGram bigram:',output['SNBigram'])
+        print('SNGram trigram:',output['SNTrigram'])
+        
+        print('-----------------------------------')
+        nlp_french = spacy.load('fr_core_news_sm')
+        text='Je voudrais réserver un hôtel à Rennes.'
+        SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=nlp_french)
+        output=SNgram_obj.get_SNgram()    
+        print(text)
+        print('SNGram bigram:',output['SNBigram'])
+        print('SNGram trigram:',output['SNTrigram'])
+        
+        ```
+        
+        Where to get it?
+        ================
+        
+        `pip install SNgramExtractor`
+        
+        How to cite?
+        ================
+        
+        Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
+        
+        Dependencies
+        ============
+        
+         - [spacy](https://spacy.io/)
+         - [spacy model en_core_web_sm](https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.2.0/en_core_web_sm-2.2.0.tar.gz)
+        
+        References
+        ============
+        
+        1. [Syntactic Dependency-Based N-grams as Classification Features](http://www.icsd.aegean.gr/lecturers/stamatatos/papers/MICAI2012.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
+        2. [Syntactic N-grams as Machine Learning Features for Natural Language Processing](http://www.cic.ipn.mx/~sidorov/Synt_n_grams_ESWA_FINAL.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
+        3. [Dependency-Based Open Information Extraction](http://www.anthology.aclweb.org/W/W12/W12-0702.pdf) by Pablo Gamallo, Marcos Garcia and Santiago Fernandez-Lanza
+        4. [Query Understanding Enhanced By Hierarchical Parsing Structures](https://groups.csail.mit.edu/sls/publications/2013/Liu_ASRU_2013.pdf) by Jingjing Liu, Panupong Pasupat, Yining Wang, Scott Cyphers, and Jim Glass
+        5. [Dependency Structure Trees in Syntax Based Machine Translation](http://www.cs.cmu.edu/~vamshi/publications/DependencyMT_report.pdf) by Vamshi Ambati
+        6. [Question Answering Passage Retrieval Using Dependency Relations](https://www.comp.nus.edu.sg/~kanmy/papers/f66-cui.pdf) by Hang Cui, Renxu Sun, Keya Li, Min-Yen Kan and Tat-Seng Chua
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-What is it?
-===========
-
-Companion library of machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html)
-
-SNgramExtractor module helps extract Syntactic relations (SR tags) as elements of sn-grams. 
-
-We follow the path marked by the arrows in the dependencies and obtain sngrams.[1]
-
-The advantage of syntactic n-grams (SN-grams), i.e., n-grams that are constructed using paths in syntactic trees, is that they are less arbitrary than traditional n-grams. Thus, their number is less than the number of traditional n-grams. Besides, they can be interpreted as linguistic phenomenon, while traditional n-grams have no plausible linguistic interpretation they are merely statistical artifact. [1]
-
-SN-gram has usability across many natural language processing application areas, such as classification tasks in machine learning[2], information extraction[3], query understanding[4], machine translation[5], question answering systems[6]
-
-Input parameters
-================
-
-  - **text** input text as a single sentence.
-  - **meta_tag** Resultant bigram and trigram should be concatenated with part of speech tag('pos') or dependency tag('dep') or original SN-gram('original')
-  - **trigram_flag** if we need to include trigrams derived from SN-grams as well ('yes') or not ('no'). Default is 'yes'
-  - **nlp_model** Specify the spacy language model you want to use. Default is spacy English language model en_core_web_sm. This is useful for being able to use languages other than english.
-
-Output
-================
-
-Dictionary object with key value pairs for bigram and trigram derived from SN-gram.
-
-  - **SNBigram** dictionary key for bigram derived from SN-gram
-  - **SNTrigram** dictionary key for trigram derived from SN-gram
-
-How to use is it?
-=================
-
-```python
-
-from SNgramExtractor import SNgramExtractor
-
-text='Economic news have little effect on financial markets.'    
-SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=None)
-output=SNgram_obj.get_SNgram()
-print(text)
-print('SNGram bigram:',output['SNBigram'])
-print('SNGram trigram:',output['SNTrigram'])
-
-print('-----------------------------------')
-text='every cloud has a silver lining'
-SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=None)
-output=SNgram_obj.get_SNgram()
-print(text)
-print('SNGram bigram:',output['SNBigram'])
-print('SNGram trigram:',output['SNTrigram'])
-
-print('-----------------------------------')
-nlp_french = spacy.load('fr_core_news_sm')
-text='Je voudrais réserver un hôtel à Rennes.'
-SNgram_obj=SNgramExtractor(text,meta_tag='original',trigram_flag='yes',nlp_model=nlp_french)
-output=SNgram_obj.get_SNgram()    
-print(text)
-print('SNGram bigram:',output['SNBigram'])
-print('SNGram trigram:',output['SNTrigram'])
-
-```
-
-Where to get it?
-================
-
-`pip install SNgramExtractor`
-
-How to cite?
-================
-
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
-
-Dependencies
-============
-
- - [spacy](https://spacy.io/)
- - [spacy model en_core_web_sm](https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.2.0/en_core_web_sm-2.2.0.tar.gz)
-
-References
-============
-
-1. [Syntactic Dependency-Based N-grams as Classification Features](http://www.icsd.aegean.gr/lecturers/stamatatos/papers/MICAI2012.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
-2. [Syntactic N-grams as Machine Learning Features for Natural Language Processing](http://www.cic.ipn.mx/~sidorov/Synt_n_grams_ESWA_FINAL.pdf) by Grigori Sidorov , Francisco Velasquez, Efstathios Stamatatos, Alexander Gelbukh and Liliana Chanona-Hernández
-3. [Dependency-Based Open Information Extraction](http://www.anthology.aclweb.org/W/W12/W12-0702.pdf) by Pablo Gamallo, Marcos Garcia and Santiago Fernandez-Lanza
-4. [Query Understanding Enhanced By Hierarchical Parsing Structures](https://groups.csail.mit.edu/sls/publications/2013/Liu_ASRU_2013.pdf) by Jingjing Liu, Panupong Pasupat, Yining Wang, Scott Cyphers, and Jim Glass
-5. [Dependency Structure Trees in Syntax Based Machine Translation](http://www.cs.cmu.edu/~vamshi/publications/DependencyMT_report.pdf) by Vamshi Ambati
-6. [Question Answering Passage Retrieval Using Dependency Relations](https://www.comp.nus.edu.sg/~kanmy/papers/f66-cui.pdf) by Hang Cui, Renxu Sun, Keya Li, Min-Yen Kan and Tat-Seng Chua
-
-
```

### Comparing `SNgramExtractor-0.0.5/LICENSE` & `SNgramExtractor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SNgramExtractor-0.0.5/setup.py` & `SNgramExtractor-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     with open('README.rst', encoding='utf-8') as f:
         long_description = f.read()
 
 
 setup(
     name='SNgramExtractor',
-    version='0.0.5',
+    version='0.0.6',
     description='Implementation of syntactic n-grams (sn-gram) extraction',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='StatguyUser',
     url='https://github.com/StatguyUser/SNgramExtractor',
     install_requires=['spacy','spacy[en_core_news_md]'],
     download_url='https://github.com/StatguyUser/SNgramExtractor.git',
```

