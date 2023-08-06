# Comparing `tmp/py-contract-ui-0.0.1.tar.gz` & `tmp/py-contract-ui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-contract-ui-0.0.1.tar", last modified: Sun Aug  6 12:47:59 2023, max compression
+gzip compressed data, was "py-contract-ui-0.0.2.tar", last modified: Sun Aug  6 13:36:33 2023, max compression
```

## Comparing `py-contract-ui-0.0.1.tar` & `py-contract-ui-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.491992 py-contract-ui-0.0.1/
--rw-r--r--   0 amjad      (501) staff       (20)     1061 2023-08-02 22:58:37.000000 py-contract-ui-0.0.1/LICENCE
--rw-r--r--   0 amjad      (501) staff       (20)       83 2023-08-03 00:58:59.000000 py-contract-ui-0.0.1/MANIFEST.in
--rw-r--r--   0 amjad      (501) staff       (20)     2600 2023-08-06 12:47:59.492091 py-contract-ui-0.0.1/PKG-INFO
--rw-r--r--   0 amjad      (501) staff       (20)     2110 2023-08-06 12:30:02.000000 py-contract-ui-0.0.1/README.md
--rw-r--r--   0 amjad      (501) staff       (20)      103 2023-08-02 22:56:05.000000 py-contract-ui-0.0.1/pyproject.toml
--rw-r--r--   0 amjad      (501) staff       (20)      765 2023-08-06 12:47:59.492367 py-contract-ui-0.0.1/setup.cfg
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.474682 py-contract-ui-0.0.1/src/
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.476002 py-contract-ui-0.0.1/src/py_contract_ui/
--rw-r--r--   0 amjad      (501) staff       (20)        0 2023-08-02 20:56:20.000000 py-contract-ui-0.0.1/src/py_contract_ui/__init__.py
--rw-r--r--   0 amjad      (501) staff       (20)     6279 2023-08-04 07:26:45.000000 py-contract-ui-0.0.1/src/py_contract_ui/generate_ui.py
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.484753 py-contract-ui-0.0.1/src/py_contract_ui/public/
--rw-r--r--   0 amjad      (501) staff       (20)   155850 2023-08-03 00:53:13.000000 py-contract-ui-0.0.1/src/py_contract_ui/public/bootstrap-5.0.2.min.css
--rw-r--r--   0 amjad      (501) staff       (20)   431289 2023-08-03 00:53:13.000000 py-contract-ui-0.0.1/src/py_contract_ui/public/bootstrap-5.0.2.min.css.map
--rw-r--r--   0 amjad      (501) staff       (20)  1412839 2023-08-03 00:53:13.000000 py-contract-ui-0.0.1/src/py_contract_ui/public/web3-1.7.3.min.js
--rw-r--r--   0 amjad      (501) staff       (20)  4292317 2023-08-03 00:53:13.000000 py-contract-ui-0.0.1/src/py_contract_ui/public/web3-1.7.3.min.js.map
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.491125 py-contract-ui-0.0.1/src/py_contract_ui/template/
--rw-r--r--   0 amjad      (501) staff       (20)        0 2023-08-02 21:18:31.000000 py-contract-ui-0.0.1/src/py_contract_ui/template/__init__.py
--rw-r--r--   0 amjad      (501) staff       (20)    43405 2023-08-02 21:18:17.000000 py-contract-ui-0.0.1/src/py_contract_ui/template/template.j2
-drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 12:47:59.477039 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/
--rw-r--r--   0 amjad      (501) staff       (20)     2600 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/PKG-INFO
--rw-r--r--   0 amjad      (501) staff       (20)      649 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/SOURCES.txt
--rw-r--r--   0 amjad      (501) staff       (20)        1 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/dependency_links.txt
--rw-r--r--   0 amjad      (501) staff       (20)       68 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/entry_points.txt
--rw-r--r--   0 amjad      (501) staff       (20)       33 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/requires.txt
--rw-r--r--   0 amjad      (501) staff       (20)       15 2023-08-06 12:47:59.000000 py-contract-ui-0.0.1/src/py_contract_ui.egg-info/top_level.txt
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.200250 py-contract-ui-0.0.2/
+-rw-r--r--   0 amjad      (501) staff       (20)     1061 2023-08-02 22:58:37.000000 py-contract-ui-0.0.2/LICENCE
+-rw-r--r--   0 amjad      (501) staff       (20)       83 2023-08-03 00:58:59.000000 py-contract-ui-0.0.2/MANIFEST.in
+-rw-r--r--   0 amjad      (501) staff       (20)     2600 2023-08-06 13:36:33.200323 py-contract-ui-0.0.2/PKG-INFO
+-rw-r--r--   0 amjad      (501) staff       (20)     2110 2023-08-06 12:30:02.000000 py-contract-ui-0.0.2/README.md
+-rw-r--r--   0 amjad      (501) staff       (20)      103 2023-08-02 22:56:05.000000 py-contract-ui-0.0.2/pyproject.toml
+-rw-r--r--   0 amjad      (501) staff       (20)      780 2023-08-06 13:36:33.200588 py-contract-ui-0.0.2/setup.cfg
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.183868 py-contract-ui-0.0.2/src/
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.185223 py-contract-ui-0.0.2/src/py_contract_ui/
+-rw-r--r--   0 amjad      (501) staff       (20)        0 2023-08-02 20:56:20.000000 py-contract-ui-0.0.2/src/py_contract_ui/__init__.py
+-rw-r--r--   0 amjad      (501) staff       (20)     6279 2023-08-04 07:26:45.000000 py-contract-ui-0.0.2/src/py_contract_ui/generate_ui.py
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.189714 py-contract-ui-0.0.2/src/py_contract_ui/public/
+-rw-r--r--   0 amjad      (501) staff       (20)   155850 2023-08-03 00:53:13.000000 py-contract-ui-0.0.2/src/py_contract_ui/public/bootstrap-5.0.2.min.css
+-rw-r--r--   0 amjad      (501) staff       (20)   431289 2023-08-03 00:53:13.000000 py-contract-ui-0.0.2/src/py_contract_ui/public/bootstrap-5.0.2.min.css.map
+-rw-r--r--   0 amjad      (501) staff       (20)  1412839 2023-08-03 00:53:13.000000 py-contract-ui-0.0.2/src/py_contract_ui/public/web3-1.7.3.min.js
+-rw-r--r--   0 amjad      (501) staff       (20)  4292317 2023-08-03 00:53:13.000000 py-contract-ui-0.0.2/src/py_contract_ui/public/web3-1.7.3.min.js.map
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.193619 py-contract-ui-0.0.2/src/py_contract_ui/template/
+-rw-r--r--   0 amjad      (501) staff       (20)        0 2023-08-02 21:18:31.000000 py-contract-ui-0.0.2/src/py_contract_ui/template/__init__.py
+-rw-r--r--   0 amjad      (501) staff       (20)    43405 2023-08-02 21:18:17.000000 py-contract-ui-0.0.2/src/py_contract_ui/template/template.j2
+drwxr-xr-x   0 amjad      (501) staff       (20)        0 2023-08-06 13:36:33.185986 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/
+-rw-r--r--   0 amjad      (501) staff       (20)     2600 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/PKG-INFO
+-rw-r--r--   0 amjad      (501) staff       (20)      649 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 amjad      (501) staff       (20)        1 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 amjad      (501) staff       (20)       68 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/entry_points.txt
+-rw-r--r--   0 amjad      (501) staff       (20)       47 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/requires.txt
+-rw-r--r--   0 amjad      (501) staff       (20)       15 2023-08-06 13:36:33.000000 py-contract-ui-0.0.2/src/py_contract_ui.egg-info/top_level.txt
```

### Comparing `py-contract-ui-0.0.1/LICENCE` & `py-contract-ui-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/PKG-INFO` & `py-contract-ui-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-contract-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: For converting Ethereum smart contract ABIs into interactive HTML user interface.
 Home-page: https://github.com/AMJADH195/py-contract-ui.git
 Author: Amjad
 Author-email: amjadh1996@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-contract-ui-0.0.1/README.md` & `py-contract-ui-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/setup.cfg` & `py-contract-ui-0.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-contract-ui
-version = 0.0.1
+version = 0.0.2
 author = Amjad
 author_email = amjadh1996@gmail.com
 description = For converting Ethereum smart contract ABIs into interactive HTML user interface.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AMJADH195/py-contract-ui.git
 classifiers = 
@@ -15,14 +15,15 @@
 [options]
 packages = find:
 python_requires = >=3.11
 include_package_data = True
 install_requires = 
 	uvicorn>=0.23.2
 	fastapi>=0.100.1
+	Jinja2>=3.1.2
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	contract-ui-gen = py_contract_ui.generate_ui:main
```

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/generate_ui.py` & `py-contract-ui-0.0.2/src/py_contract_ui/generate_ui.py`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/public/bootstrap-5.0.2.min.css` & `py-contract-ui-0.0.2/src/py_contract_ui/public/bootstrap-5.0.2.min.css`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/public/bootstrap-5.0.2.min.css.map` & `py-contract-ui-0.0.2/src/py_contract_ui/public/bootstrap-5.0.2.min.css.map`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/public/web3-1.7.3.min.js` & `py-contract-ui-0.0.2/src/py_contract_ui/public/web3-1.7.3.min.js`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/public/web3-1.7.3.min.js.map` & `py-contract-ui-0.0.2/src/py_contract_ui/public/web3-1.7.3.min.js.map`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui/template/template.j2` & `py-contract-ui-0.0.2/src/py_contract_ui/template/template.j2`

 * *Files identical despite different names*

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui.egg-info/PKG-INFO` & `py-contract-ui-0.0.2/src/py_contract_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-contract-ui
-Version: 0.0.1
+Version: 0.0.2
 Summary: For converting Ethereum smart contract ABIs into interactive HTML user interface.
 Home-page: https://github.com/AMJADH195/py-contract-ui.git
 Author: Amjad
 Author-email: amjadh1996@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `py-contract-ui-0.0.1/src/py_contract_ui.egg-info/SOURCES.txt` & `py-contract-ui-0.0.2/src/py_contract_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

