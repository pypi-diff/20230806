# Comparing `tmp/arab_transcription-1.0.0.tar.gz` & `tmp/arab_transcription-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arab_transcription-1.0.0.tar", last modified: Sat Jul 29 18:17:11 2023, max compression
+gzip compressed data, was "arab_transcription-1.0.1.tar", last modified: Sun Aug  6 17:32:32 2023, max compression
```

## Comparing `arab_transcription-1.0.0.tar` & `arab_transcription-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 18:17:11.117280 arab_transcription-1.0.0/
--rw-r--r--   0 mac        (501) staff       (20)     3493 2023-07-29 17:58:01.000000 arab_transcription-1.0.0/ArabText.py
--rw-r--r--   0 mac        (501) staff       (20)      220 2023-07-29 18:17:11.116675 arab_transcription-1.0.0/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     5062 2023-07-29 18:16:46.000000 arab_transcription-1.0.0/README.md
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 22:00:21.000000 arab_transcription-1.0.0/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 18:17:11.112829 arab_transcription-1.0.0/_types/
--rw-r--r--   0 mac        (501) staff       (20)       80 2023-03-08 20:49:17.000000 arab_transcription-1.0.0/_types/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1168 2023-03-08 20:49:17.000000 arab_transcription-1.0.0/_types/linked_queue.py
--rw-r--r--   0 mac        (501) staff       (20)     1855 2023-07-29 17:43:53.000000 arab_transcription-1.0.0/alphabet.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-29 18:17:11.115745 arab_transcription-1.0.0/arab_transcription.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      220 2023-07-29 18:17:10.000000 arab_transcription-1.0.0/arab_transcription.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      308 2023-07-29 18:17:11.000000 arab_transcription-1.0.0/arab_transcription.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-29 18:17:10.000000 arab_transcription-1.0.0/arab_transcription.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2023-07-29 18:17:10.000000 arab_transcription-1.0.0/arab_transcription.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)     2410 2023-05-15 17:01:37.000000 arab_transcription-1.0.0/mapping.py
--rw-r--r--   0 mac        (501) staff       (20)       51 2023-04-07 22:15:20.000000 arab_transcription-1.0.0/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-29 18:17:11.117442 arab_transcription-1.0.0/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      356 2023-07-29 18:09:08.000000 arab_transcription-1.0.0/setup.py
--rw-r--r--   0 mac        (501) staff       (20)     4908 2023-07-29 17:54:16.000000 arab_transcription-1.0.0/transliterator.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-06 17:32:32.446014 arab_transcription-1.0.1/
+-rw-r--r--   0 mac        (501) staff       (20)     3493 2023-07-29 17:58:01.000000 arab_transcription-1.0.1/ArabText.py
+-rw-r--r--   0 mac        (501) staff       (20)      220 2023-08-06 17:32:32.445552 arab_transcription-1.0.1/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     5062 2023-07-29 18:23:45.000000 arab_transcription-1.0.1/README.md
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 22:00:21.000000 arab_transcription-1.0.1/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-06 17:32:32.443035 arab_transcription-1.0.1/_types/
+-rw-r--r--   0 mac        (501) staff       (20)       80 2023-03-08 20:49:17.000000 arab_transcription-1.0.1/_types/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1168 2023-03-08 20:49:17.000000 arab_transcription-1.0.1/_types/linked_queue.py
+-rw-r--r--   0 mac        (501) staff       (20)     1855 2023-07-29 17:43:53.000000 arab_transcription-1.0.1/alphabet.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-08-06 17:32:32.444959 arab_transcription-1.0.1/arab_transcription.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      220 2023-08-06 17:32:32.000000 arab_transcription-1.0.1/arab_transcription.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      308 2023-08-06 17:32:32.000000 arab_transcription-1.0.1/arab_transcription.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-08-06 17:32:32.000000 arab_transcription-1.0.1/arab_transcription.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2023-08-06 17:32:32.000000 arab_transcription-1.0.1/arab_transcription.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)     2410 2023-05-15 17:01:37.000000 arab_transcription-1.0.1/mapping.py
+-rw-r--r--   0 mac        (501) staff       (20)       51 2023-04-07 22:15:20.000000 arab_transcription-1.0.1/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-08-06 17:32:32.446191 arab_transcription-1.0.1/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      356 2023-08-06 17:32:26.000000 arab_transcription-1.0.1/setup.py
+-rw-r--r--   0 mac        (501) staff       (20)     5058 2023-08-06 17:26:49.000000 arab_transcription-1.0.1/transliterator.py
```

### Comparing `arab_transcription-1.0.0/ArabText.py` & `arab_transcription-1.0.1/ArabText.py`

 * *Files identical despite different names*

### Comparing `arab_transcription-1.0.0/README.md` & `arab_transcription-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
 
 ## Usage
 
 **Python 3.9 or later required**
 
 ```bash
-pip install arab_transcription
+pip install arab-transcription
 ```
 
 ```bash
 python3 -m transliterator [-t arab_text] [-f arab_file]
 ```
 
 **Ex**.
```

#### html2text {}

```diff
@@ -46,15 +46,15 @@
 |4|damma____|u____________|
 |5|kasra____|i____________|
 |6|shadda___|(double)_____|
 |7|sukÅ«n_|'____________|
 The long vowels are indicated byÂ *Ä*,Â *Ä«*Â andÂ *Å«*, and
 theÂ *maddah*Â may also be used to lengthen a vowel. TheÂ *shadda*Â is
 indicated by the doubling of a letter ## Usage **Python 3.9 or later required**
-```bash pip install arab_transcription ``` ```bash python3 -m transliterator [-
+```bash pip install arab-transcription ``` ```bash python3 -m transliterator [-
 t arab_text] [-f arab_file] ``` **Ex**. ```bash python3 -m transliterator -
 t "ÙÙÙÙÙÙØ¯Ù Ø¢ØªÙÙÙÙÙØ§ ÙÙÙØ³ÙÙ Ø§ÙÙÙÙØªÙØ§Ø¨Ù
 ÙÙÙÙÙÙÙÙÙÙÙØ§ ÙÙÙ Ø¨ÙØ¹ÙØ¯ÙÙÙ Ø¨ÙØ§ÙØ±ÙÙØ³ÙÙÙ Û
 ÙÙØ¢ØªÙÙÙÙÙØ§ Ø¹ÙÙØ³ÙÙ Ø§Ø¨ÙÙÙ ÙÙØ±ÙÙÙÙÙ
 Ø§ÙÙØ¨ÙÙÙÙÙÙØ§ØªÙ ÙÙØ£ÙÙÙÙØ¯ÙÙÙØ§ÙÙ Ø¨ÙØ±ÙÙØ­Ù
 Ø§ÙÙÙÙØ¯ÙØ³Ù Û Ø£ÙÙÙÙÙÙÙÙÙÙØ§ Ø¬ÙØ§Ø¡ÙÙÙÙÙ
 Ø±ÙØ³ÙÙÙÙ Ø¨ÙÙÙØ§ ÙÙØ§ ØªÙÙÙÙÙÙÙ° Ø£ÙÙÙÙØ³ÙÙÙÙÙ
```

### Comparing `arab_transcription-1.0.0/_types/linked_queue.py` & `arab_transcription-1.0.1/_types/linked_queue.py`

 * *Files identical despite different names*

### Comparing `arab_transcription-1.0.0/alphabet.py` & `arab_transcription-1.0.1/alphabet.py`

 * *Files identical despite different names*

### Comparing `arab_transcription-1.0.0/mapping.py` & `arab_transcription-1.0.1/mapping.py`

 * *Files identical despite different names*

### Comparing `arab_transcription-1.0.0/transliterator.py` & `arab_transcription-1.0.1/transliterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 
 def normalize(text):
     # some text may have shadda coming after a vowel whic in this case
     # will fail the script, so were swapping
     text = list(text)
     for i, c in enumerate(text):
-        if c == alphabet.SHADDA and (text[i-1] in alphabet.VOWELS):
-            text[i], text[i-1] = text[i-1], text[i]
+        if c == alphabet.SHADDA:
+            if (text[i-1] in alphabet.VOWELS):
+                text[i], text[i-1] = text[i-1], text[i]
+            elif (text[i-1] == alphabet.LAM) and not (text[i+1] in alphabet.VOWELS):
+                text.insert(i+1, alphabet.FATHA)
     return text
 
 
 class ArabTransliterator:
 
     def __init__(self):
         self.table = _mapping
```

