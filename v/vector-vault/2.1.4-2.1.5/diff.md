# Comparing `tmp/vector_vault-2.1.4.tar.gz` & `tmp/vector_vault-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.1.4.tar", last modified: Sat Aug  5 16:44:22 2023, max compression
+gzip compressed data, was "vector_vault-2.1.5.tar", last modified: Sat Aug  5 19:07:22 2023, max compression
```

## Comparing `vector_vault-2.1.4.tar` & `vector_vault-2.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:44:22.117418 vector_vault-2.1.4/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    26593 2023-08-05 16:44:22.117287 vector_vault-2.1.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    25883 2023-08-01 07:40:15.000000 vector_vault-2.1.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-05 16:44:22.117457 vector_vault-2.1.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-08-05 16:44:08.000000 vector_vault-2.1.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:44:22.113283 vector_vault-2.1.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    26593 2023-08-05 16:44:22.000000 vector_vault-2.1.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-05 16:44:22.000000 vector_vault-2.1.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-05 16:44:22.000000 vector_vault-2.1.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-05 16:44:22.000000 vector_vault-2.1.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-05 16:44:22.000000 vector_vault-2.1.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 16:44:22.116923 vector_vault-2.1.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.4/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.4/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.4/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.4/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    36523 2023-08-05 16:44:01.000000 vector_vault-2.1.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.4/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 19:07:22.942671 vector_vault-2.1.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.1.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    26556 2023-08-05 19:07:22.942482 vector_vault-2.1.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    25883 2023-08-01 07:40:15.000000 vector_vault-2.1.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-08-05 19:07:22.942713 vector_vault-2.1.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1060 2023-08-05 19:07:15.000000 vector_vault-2.1.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 19:07:22.938416 vector_vault-2.1.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    26556 2023-08-05 19:07:22.000000 vector_vault-2.1.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2023-08-05 19:07:22.000000 vector_vault-2.1.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-08-05 19:07:22.000000 vector_vault-2.1.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-08-05 19:07:22.000000 vector_vault-2.1.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-08-05 19:07:22.000000 vector_vault-2.1.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-08-05 19:07:22.942111 vector_vault-2.1.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-06-09 19:04:41.000000 vector_vault-2.1.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13294 2023-07-16 01:36:29.000000 vector_vault-2.1.5/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-06-27 02:14:51.000000 vector_vault-2.1.5/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-07-18 22:45:16.000000 vector_vault-2.1.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.1.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.1.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2600 2023-07-18 22:45:26.000000 vector_vault-2.1.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16773 2023-07-21 20:42:10.000000 vector_vault-2.1.5/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    36524 2023-08-05 19:05:08.000000 vector_vault-2.1.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4084 2023-07-16 04:42:19.000000 vector_vault-2.1.5/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.1.5/vectorvault/wrap.py
```

### Comparing `vector_vault-2.1.4/LICENSE` & `vector_vault-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/PKG-INFO` & `vector_vault-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.1.4
+Version: 2.1.5
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -640,9 +638,7 @@
 Happy coding!
 <br>
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
 <br>
-
-
```

### Comparing `vector_vault-2.1.4/README.md` & `vector_vault-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/setup.py` & `vector_vault-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.1.4",
+    version="2.1.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.1.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.1.5/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.1.4
+Version: 2.1.5
 Summary: Vector Vault: Customize ChatGPT and unleash the full potential of generative AI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -640,9 +638,7 @@
 Happy coding!
 <br>
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
 <br>
-
-
```

### Comparing `vector_vault-2.1.4/vectorvault/ai.py` & `vector_vault-2.1.5/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/cloud_api.py` & `vector_vault-2.1.5/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/cloudmanager.py` & `vector_vault-2.1.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/creds.py` & `vector_vault-2.1.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/download.py` & `vector_vault-2.1.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/itemize.py` & `vector_vault-2.1.5/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/tools_gpt.py` & `vector_vault-2.1.5/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.1.4/vectorvault/vault.py` & `vector_vault-2.1.5/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
                             for text in context:
                                 input_ += text['data']
                         response = self.ai.llm_w_context(segment, input_, history, model=model, custom_prompt=custom_prompt)
                     else:
                         response = self.ai.llm(segment, history, model=model, custom_prompt=custom_prompt)
                     break
                 except Exception as e:
-                    exception += 1
+                    exceptions += 1
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     if exceptions >= 5:
                         print(f"API Failed too many times, exiting loop: {e}.")
                         break
                     time.sleep(5)
```

### Comparing `vector_vault-2.1.4/vectorvault/vecreq.py` & `vector_vault-2.1.5/vectorvault/vecreq.py`

 * *Files identical despite different names*

