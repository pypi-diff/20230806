# Comparing `tmp/vector_vault-2.1.6.tar.gz` & `tmp/vector_vault-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.6.tar", last modified: Sun Aug  6 16:29:48 2023, max compression
+gzip compressed data, was "vector_vault-2.1.7.tar", last modified: Sun Aug  6 16:37:32 2023, max compression
```

## Comparing `vector_vault-2.1.6.tar` & `vector_vault-2.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:29:48.634502 vector_vault-2.1.6/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.6/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    26448 2023-08-06 16:29:48.634338 vector_vault-2.1.6/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    25775 2023-08-06 16:28:50.000000 vector_vault-2.1.6/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-06 16:29:48.634537 vector_vault-2.1.6/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-08-06 16:29:40.000000 vector_vault-2.1.6/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:29:48.630531 vector_vault-2.1.6/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    26448 2023-08-06 16:29:48.000000 vector_vault-2.1.6/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-06 16:29:48.000000 vector_vault-2.1.6/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-06 16:29:48.000000 vector_vault-2.1.6/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-06 16:29:48.000000 vector_vault-2.1.6/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-06 16:29:48.000000 vector_vault-2.1.6/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:29:48.633977 vector_vault-2.1.6/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.6/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.6/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.6/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.6/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.6/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.6/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.6/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.6/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36592 2023-08-06 16:27:34.000000 vector_vault-2.1.6/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.6/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.6/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.639297 vector_vault-2.1.7/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.7/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    26434 2023-08-06 16:37:32.639102 vector_vault-2.1.7/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    25775 2023-08-06 16:28:50.000000 vector_vault-2.1.7/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-06 16:37:32.639334 vector_vault-2.1.7/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1046 2023-08-06 16:37:02.000000 vector_vault-2.1.7/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.630103 vector_vault-2.1.7/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    26434 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-06 16:37:32.000000 vector_vault-2.1.7/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-06 16:37:32.638529 vector_vault-2.1.7/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.7/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13996 2023-08-06 16:37:28.000000 vector_vault-2.1.7/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.7/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.7/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.7/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.7/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.7/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.7/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36592 2023-08-06 16:27:34.000000 vector_vault-2.1.7/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.7/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.7/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.6/LICENSE` & `vector_vault-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/PKG-INFO` & `vector_vault-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.6
-Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
+Version: 2.1.7
+Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vector_vault-2.1.6/README.md` & `vector_vault-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/setup.py` & `vector_vault-2.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.6",
+    version="2.1.7",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
-    description="Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
+    description="Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
     classifiers=[
         "License :: Other/Proprietary License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `vector_vault-2.1.6/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.7/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.6
-Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
+Version: 2.1.7
+Summary: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vector_vault-2.1.6/vectorvault/ai.py` & `vector_vault-2.1.7/vectorvault/ai.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
     def llm(self, user_input: str = None, history: str = None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         '''
             If you pass in a custom_prompt with content already fully filled in, and no user_input, it will process your custom_prompt only without changing       
         '''
+        max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
+        max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
         if user_input:
             intokes = self.get_tokens(user_input)
             histokes = self.get_tokens(history) if history else 0
             if intokes + histokes > max_tokens:
                 tokes_left = max_tokens - intokes - histokes
                 if tokes_left < 0: # way too much input
@@ -66,14 +68,17 @@
         Additional Context: {context}
 
         Question: {content}
 
         (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
+        max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
+        max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
+
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
         promptokes = self.get_tokens(prompt_template)
 
         if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
@@ -111,14 +116,19 @@
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
         )
         return response['choices'][0]['message']['content']
 
 
     def llm_stream(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+        '''
+            Stream version of "llm"
+        '''
+        max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
+        max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
         intokes = self.get_tokens(user_input)
         histokes = self.get_tokens(history) if history else 0
         if intokes + histokes > max_tokens:
             tokes_left = max_tokens - intokes - histokes
             if tokes_left < 0: # way too much input
                 char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
@@ -171,14 +181,17 @@
         Additional Context: {context}
 
         Question: {content}
 
         (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:""" 
 
+        max_tokens = max_tokens * 4 if model == 'gpt-3.5-turbo-16k' else max_tokens
+        max_tokens = max_tokens * 8 if model == 'gpt-4-32k' else max_tokens
+
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
         promptokes = self.get_tokens(prompt_template)
 
         if (intokes + contokes + histokes + promptokes) > max_tokens * .9:
```

### Comparing `vector_vault-2.1.6/vectorvault/cloud_api.py` & `vector_vault-2.1.7/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/cloudmanager.py` & `vector_vault-2.1.7/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/creds.py` & `vector_vault-2.1.7/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/download.py` & `vector_vault-2.1.7/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/itemize.py` & `vector_vault-2.1.7/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/tools_gpt.py` & `vector_vault-2.1.7/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/vault.py` & `vector_vault-2.1.7/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.6/vectorvault/vecreq.py` & `vector_vault-2.1.7/vectorvault/vecreq.py`

 * *Files identical despite different names*

