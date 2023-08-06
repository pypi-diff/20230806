# Comparing `tmp/bandolier-0.0.7.tar.gz` & `tmp/bandolier-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandolier-0.0.7.tar", last modified: Sun Aug  6 07:36:17 2023, max compression
+gzip compressed data, was "bandolier-0.0.8.tar", last modified: Sun Aug  6 07:40:11 2023, max compression
```

## Comparing `bandolier-0.0.7.tar` & `bandolier-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:36:17.961189 bandolier-0.0.7/
--rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.0.7/LICENSE
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:36:17.961046 bandolier-0.0.7/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.0.7/README.md
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:36:17.959913 bandolier-0.0.7/bandolier/
--rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.0.7/bandolier/__init__.py
--rw-r--r--   0 jlb        (501) staff       (20)     4152 2023-08-04 08:58:41.000000 bandolier-0.0.7/bandolier/bandolier.py
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:36:17.960841 bandolier-0.0.7/bandolier.egg-info/
--rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:36:17.000000 bandolier-0.0.7/bandolier.egg-info/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 07:36:17.000000 bandolier-0.0.7/bandolier.egg-info/SOURCES.txt
--rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 07:36:17.000000 bandolier-0.0.7/bandolier.egg-info/dependency_links.txt
--rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 07:36:17.000000 bandolier-0.0.7/bandolier.egg-info/requires.txt
--rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 07:36:17.000000 bandolier-0.0.7/bandolier.egg-info/top_level.txt
--rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 07:36:17.961237 bandolier-0.0.7/setup.cfg
--rw-r--r--   0 jlb        (501) staff       (20)     1278 2023-08-06 07:36:12.000000 bandolier-0.0.7/setup.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.042694 bandolier-0.0.8/
+-rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.0.8/LICENSE
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:40:11.042511 bandolier-0.0.8/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)     3135 2023-08-06 07:20:08.000000 bandolier-0.0.8/README.md
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.041447 bandolier-0.0.8/bandolier/
+-rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.0.8/bandolier/__init__.py
+-rw-r--r--   0 jlb        (501) staff       (20)     4152 2023-08-04 08:58:41.000000 bandolier-0.0.8/bandolier/bandolier.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 07:40:11.042212 bandolier-0.0.8/bandolier.egg-info/
+-rw-r--r--   0 jlb        (501) staff       (20)     3802 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/SOURCES.txt
+-rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/dependency_links.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/requires.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 07:40:11.000000 bandolier-0.0.8/bandolier.egg-info/top_level.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 07:40:11.042748 bandolier-0.0.8/setup.cfg
+-rw-r--r--   0 jlb        (501) staff       (20)     1370 2023-08-06 07:40:08.000000 bandolier-0.0.8/setup.py
```

### Comparing `bandolier-0.0.7/LICENSE` & `bandolier-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.7/PKG-INFO` & `bandolier-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.7
+Version: 0.0.8
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.7/README.md` & `bandolier-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.7/bandolier/bandolier.py` & `bandolier-0.0.8/bandolier/bandolier.py`

 * *Files identical despite different names*

### Comparing `bandolier-0.0.7/bandolier.egg-info/PKG-INFO` & `bandolier-0.0.8/bandolier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.0.7
+Version: 0.0.8
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bandolier-0.0.7/setup.py` & `bandolier-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,34 +3,43 @@
 readme = ""
 with open("README.md") as f:
     readme = f.read()
     readme = readme.split("\n")
     readme = [line for line in readme if "<img" not in line]
     readme = "\n".join(readme)
 
-with open("requirements.txt", "r") as f:
-    requirements = f.read().splitlines()
+# with open("requirements.txt", "r") as f:
+#    requirements = f.read().splitlines()
 
-with open("requirements-dev.txt", "r") as f:
-    requirements_dev = f.read().splitlines()
+# with open("requirements-dev.txt", "r") as f:
+#    requirements_dev = f.read().splitlines()
 
 setup(
     name="bandolier",
-    version="0.0.7",
+    version="0.0.8",
     description="A helper for OpenAI functions",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/johnnysands/bandolier",
     author="Johnny Sands",
     author_email="johnnysands@users.noreply.github.com",
     license="MIT",
     packages=["bandolier"],
-    install_requires=requirements,
-    extras_require={"dev": requirements_dev},
-    package_data={"": ["requirements.txt"]},
+    install_requires=[
+        "openai",
+        "python-box",
+        "tiktoken",
+    ],
+    # dev requirements
+    extras_require={
+        "dev": [
+            "pytest",
+            "twine",
+        ],
+    },
     readme="README.md",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
```

