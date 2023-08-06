# Comparing `tmp/signxml-3.2.0.tar.gz` & `tmp/signxml-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signxml-3.2.0.tar", last modified: Thu Apr 13 06:22:34 2023, max compression
+gzip compressed data, was "signxml-3.2.1.tar", last modified: Sun Aug  6 18:22:39 2023, max compression
```

## Comparing `signxml-3.2.0.tar` & `signxml-3.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983986 signxml-3.2.0/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11324 2021-10-07 21:38:03.000000 signxml-3.2.0/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       66 2022-12-16 21:17:49.000000 signxml-3.2.0/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      589 2022-12-16 21:17:49.000000 signxml-3.2.0/NOTICE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16566 2023-04-13 06:22:34.984188 signxml-3.2.0/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15648 2023-03-04 20:01:48.000000 signxml-3.2.0/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      288 2023-03-29 02:44:36.000000 signxml-3.2.0/pyproject.toml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      177 2023-04-13 06:22:34.984801 signxml-3.2.0/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1809 2023-04-13 06:21:28.000000 signxml-3.2.0/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.975156 signxml-3.2.0/signxml/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      612 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/__init__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.978272 signxml-3.2.0/signxml/__pyinstaller/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2022-08-21 15:15:01.000000 signxml-3.2.0/signxml/__pyinstaller/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      231 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/__pyinstaller/hook-signxml.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9569 2023-03-29 03:01:39.000000 signxml-3.2.0/signxml/algorithms.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      614 2022-08-24 04:57:56.000000 signxml-3.2.0/signxml/exceptions.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6722 2023-04-13 05:53:23.000000 signxml-3.2.0/signxml/processor.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2022-08-24 04:57:56.000000 signxml-3.2.0/signxml/py.typed
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.979439 signxml-3.2.0/signxml/schemas/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10293 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig-core-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      900 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig1-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4664 2021-10-07 21:38:03.000000 signxml-3.2.0/signxml/schemas/xmldsig11-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24308 2022-12-27 03:50:38.000000 signxml-3.2.0/signxml/signer.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.979817 signxml-3.2.0/signxml/util/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8963 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/util/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    31899 2023-04-13 05:53:23.000000 signxml-3.2.0/signxml/verifier.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.980562 signxml-3.2.0/signxml/xades/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1938 2022-12-16 21:17:49.000000 signxml-3.2.0/signxml/xades/__init__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983204 signxml-3.2.0/signxml/xades/schemas/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    21737 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24227 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201506.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24056 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201601.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2664 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201506.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3184 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201601.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      910 2022-11-07 16:31:27.000000 signxml-3.2.0/signxml/xades/schemas/XAdESv141.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    20109 2023-04-13 04:51:59.000000 signxml-3.2.0/signxml/xades/xades.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.977434 signxml-3.2.0/signxml.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16566 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      931 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       64 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/entry_points.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      123 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-04-13 06:22:34.000000 signxml-3.2.0/signxml.egg-info/top_level.txt
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-04-13 06:22:34.983594 signxml-3.2.0/test/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    38559 2023-04-13 05:53:18.000000 signxml-3.2.0/test/test.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.477310 signxml-3.2.1/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11324 2016-06-14 14:22:58.000000 signxml-3.2.1/LICENSE
+-rw-r--r--   0 kislyuk    (501) staff       (20)       66 2022-11-14 00:33:49.000000 signxml-3.2.1/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)      589 2022-11-13 06:37:55.000000 signxml-3.2.1/NOTICE
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-08-06 18:22:39.477431 signxml-3.2.1/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)    15648 2023-04-23 00:57:16.000000 signxml-3.2.1/README.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)      288 2023-04-08 16:53:45.000000 signxml-3.2.1/pyproject.toml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      177 2023-08-06 18:22:39.477816 signxml-3.2.1/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1842 2023-08-06 18:20:51.000000 signxml-3.2.1/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.451925 signxml-3.2.1/signxml/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      612 2022-11-27 19:29:34.000000 signxml-3.2.1/signxml/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.453698 signxml-3.2.1/signxml/__pyinstaller/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      224 2022-10-23 23:38:52.000000 signxml-3.2.1/signxml/__pyinstaller/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      231 2022-10-23 23:38:52.000000 signxml-3.2.1/signxml/__pyinstaller/hook-signxml.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     9569 2023-04-08 16:53:45.000000 signxml-3.2.1/signxml/algorithms.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      614 2022-10-23 23:38:52.000000 signxml-3.2.1/signxml/exceptions.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6722 2023-05-06 22:13:04.000000 signxml-3.2.1/signxml/processor.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-10-23 23:38:52.000000 signxml-3.2.1/signxml/py.typed
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.455104 signxml-3.2.1/signxml/schemas/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10293 2016-06-14 14:23:02.000000 signxml-3.2.1/signxml/schemas/xmldsig-core-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)      900 2016-06-14 14:23:02.000000 signxml-3.2.1/signxml/schemas/xmldsig1-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     4664 2016-06-14 14:23:02.000000 signxml-3.2.1/signxml/schemas/xmldsig11-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24273 2023-08-06 18:14:23.000000 signxml-3.2.1/signxml/signer.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.458731 signxml-3.2.1/signxml/util/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8963 2023-04-08 16:53:42.000000 signxml-3.2.1/signxml/util/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    31899 2023-05-06 22:13:04.000000 signxml-3.2.1/signxml/verifier.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.473755 signxml-3.2.1/signxml/xades/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1938 2022-11-27 20:16:00.000000 signxml-3.2.1/signxml/xades/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.476404 signxml-3.2.1/signxml/xades/schemas/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    21737 2022-10-29 20:33:16.000000 signxml-3.2.1/signxml/xades/schemas/XAdES.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24227 2022-10-29 20:33:33.000000 signxml-3.2.1/signxml/xades/schemas/XAdES01903v132-201506.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24056 2022-10-29 20:34:00.000000 signxml-3.2.1/signxml/xades/schemas/XAdES01903v132-201601.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2664 2022-10-29 20:34:18.000000 signxml-3.2.1/signxml/xades/schemas/XAdES01903v141-201506.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3184 2022-10-29 20:32:55.000000 signxml-3.2.1/signxml/xades/schemas/XAdES01903v141-201601.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)      910 2022-10-29 20:31:58.000000 signxml-3.2.1/signxml/xades/schemas/XAdESv141.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    20109 2023-04-08 16:53:45.000000 signxml-3.2.1/signxml/xades/xades.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.453375 signxml-3.2.1/signxml.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)      931 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       64 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/entry_points.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      123 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-08-06 18:22:39.000000 signxml-3.2.1/signxml.egg-info/top_level.txt
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-08-06 18:22:39.476735 signxml-3.2.1/test/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    38559 2023-05-06 22:13:04.000000 signxml-3.2.1/test/test.py
```

### Comparing `signxml-3.2.0/LICENSE` & `signxml-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/NOTICE` & `signxml-3.2.1/NOTICE`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/PKG-INFO` & `signxml-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.2.0
+Version: 3.2.1
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `signxml-3.2.0/README.rst` & `signxml-3.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/setup.py` & `signxml-3.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="signxml",
-    version="3.2.0",
+    version="3.2.1",
     url="https://github.com/kislyuk/signxml",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Python XML Signature and XAdES library",
     long_description=open("README.rst").read(),
     python_requires=">=3.7",
     install_requires=[
         # Dependencies are restricted by major version range according to semver.
         # By default, version minimums are set to be compatible with the oldest supported Ubuntu LTS (currently 18.04).
         "lxml >= 4.2.1, < 5",
         "cryptography >= 3.4.8",  # Set to the version in Ubuntu 22.04 due to features we need from cryptography 3.1
         "pyOpenSSL >= 17.5.0",
         "certifi >= 2018.1.18",
+        # "tsp-client >= 0.1.3",
     ],
     extras_require={
         "tests": [
             "ruff",
             "coverage",
             "build",
             "wheel",
```

### Comparing `signxml-3.2.0/signxml/__init__.py` & `signxml-3.2.1/signxml/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/algorithms.py` & `signxml-3.2.1/signxml/algorithms.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/exceptions.py` & `signxml-3.2.1/signxml/exceptions.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/processor.py` & `signxml-3.2.1/signxml/processor.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/schemas/xmldsig-core-schema.xsd` & `signxml-3.2.1/signxml/schemas/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/schemas/xmldsig1-schema.xsd` & `signxml-3.2.1/signxml/schemas/xmldsig1-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/schemas/xmldsig11-schema.xsd` & `signxml-3.2.1/signxml/schemas/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/signer.py` & `signxml-3.2.1/signxml/signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             sig_root.append(signing_settings.key_info)
 
     def _get_c14n_inputs_from_references(self, doc_root, references: List[SignatureReference]):
         c14n_inputs, new_references = [], []
         for reference in references:
             uri = reference.URI if reference.URI.startswith("#") else "#" + reference.URI
             c14n_inputs.append(self.get_root(self._resolve_reference(doc_root, {"URI": uri})))
-            new_references.append(SignatureReference(URI=uri, c14n_method=reference.c14n_method))
+            new_references.append(replace(reference, URI=uri))
         return c14n_inputs, new_references
 
     def _unpack(self, data, references: List[SignatureReference]):
         sig_root = Element(ds_tag("Signature"), nsmap=self.namespaces)
         if self.construction_method == SignatureConstructionMethod.enveloped:
             if isinstance(data, (str, bytes)):
                 raise InvalidInput("When using enveloped signature, **data** must be an XML element")
```

### Comparing `signxml-3.2.0/signxml/util/__init__.py` & `signxml-3.2.1/signxml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/verifier.py` & `signxml-3.2.1/signxml/verifier.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/__init__.py` & `signxml-3.2.1/signxml/xades/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdES.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdES.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201506.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdES01903v132-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdES01903v132-201601.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdES01903v132-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201506.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdES01903v141-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdES01903v141-201601.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdES01903v141-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/schemas/XAdESv141.xsd` & `signxml-3.2.1/signxml/xades/schemas/XAdESv141.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml/xades/xades.py` & `signxml-3.2.1/signxml/xades/xades.py`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/signxml.egg-info/PKG-INFO` & `signxml-3.2.1/signxml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.2.0
+Version: 3.2.1
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
```

### Comparing `signxml-3.2.0/signxml.egg-info/SOURCES.txt` & `signxml-3.2.1/signxml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signxml-3.2.0/test/test.py` & `signxml-3.2.1/test/test.py`

 * *Files identical despite different names*

