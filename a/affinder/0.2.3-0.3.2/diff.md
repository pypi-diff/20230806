# Comparing `tmp/affinder-0.2.3.tar.gz` & `tmp/affinder-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affinder-0.2.3.tar", last modified: Fri Apr  8 01:03:19 2022, max compression
+gzip compressed data, was "affinder-0.3.2.tar", last modified: Sun Aug  6 14:47:34 2023, max compression
```

## Comparing `affinder-0.2.3.tar` & `affinder-0.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.604431 affinder-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.596431 affinder-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-04-08 01:03:02.000000 affinder-0.2.3/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-04-08 01:03:02.000000 affinder-0.2.3/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-04-08 01:03:02.000000 affinder-0.2.3/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-04-08 01:03:02.000000 affinder-0.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-04-08 01:03:02.000000 affinder-0.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/.napari/
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-04-08 01:03:02.000000 affinder-0.2.3/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-04-08 01:03:02.000000 affinder-0.2.3/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-04-08 01:03:02.000000 affinder-0.2.3/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-08 01:03:02.000000 affinder-0.2.3/.yapfignore
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-04-08 01:03:02.000000 affinder-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-08 01:03:02.000000 affinder-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-04-08 01:03:19.604431 affinder-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-04-08 01:03:02.000000 affinder-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7505 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     9707 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/replace_description_text.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-04-08 01:03:02.000000 affinder-0.2.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-04-08 01:03:02.000000 affinder-0.2.3/examples/basic-example.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-04-08 01:03:02.000000 affinder-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-04-08 01:03:19.604431 affinder-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-04-08 01:03:02.000000 affinder-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.596431 affinder-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/src/affinder/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/src/affinder/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/src/affinder/_tests/labels0.zarr/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/labels0.zarr/.zarray
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/labels0.zarr/0.0
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/src/affinder/_tests/labels1.zarr/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/labels1.zarr/.zarray
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/labels1.zarr/0.0
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/_tests/test_affinder.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-08 01:03:18.000000 affinder-0.2.3/src/affinder/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6205 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/affinder.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-08 01:03:02.000000 affinder-0.2.3/src/affinder/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 01:03:19.600431 affinder-0.2.3/src/affinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2022-04-08 01:03:18.000000 affinder-0.2.3/src/affinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-04-08 01:03:19.000000 affinder-0.2.3/src/affinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 01:03:18.000000 affinder-0.2.3/src/affinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-08 01:03:19.000000 affinder-0.2.3/src/affinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-04-08 01:03:19.000000 affinder-0.2.3/src/affinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-08 01:03:19.000000 affinder-0.2.3/src/affinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-04-08 01:03:02.000000 affinder-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.213172 affinder-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.213172 affinder-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-06 14:47:17.000000 affinder-0.3.2/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-06 14:47:17.000000 affinder-0.3.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-06 14:47:17.000000 affinder-0.3.2/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-06 14:47:17.000000 affinder-0.3.2/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-06 14:47:17.000000 affinder-0.3.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.213172 affinder-0.3.2/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-08-06 14:47:17.000000 affinder-0.3.2/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-06 14:47:17.000000 affinder-0.3.2/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-06 14:47:17.000000 affinder-0.3.2/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-06 14:47:17.000000 affinder-0.3.2/.yapfignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-06 14:47:17.000000 affinder-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-06 14:47:17.000000 affinder-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-06 14:47:34.217172 affinder-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-06 14:47:17.000000 affinder-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.213172 affinder-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/replace_description_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-06 14:47:17.000000 affinder-0.3.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-06 14:47:17.000000 affinder-0.3.2/examples/basic-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-06 14:47:17.000000 affinder-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-06 14:47:34.217172 affinder-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-06 14:47:17.000000 affinder-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.213172 affinder-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/src/affinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/src/affinder/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/src/affinder/_tests/labels0.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/labels0.zarr/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/labels0.zarr/0.0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/src/affinder/_tests/labels1.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/labels1.zarr/.zarray
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/labels1.zarr/0.0
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/_tests/test_affinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/affinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-06 14:47:17.000000 affinder-0.3.2/src/affinder/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:47:34.217172 affinder-0.3.2/src/affinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 14:47:34.000000 affinder-0.3.2/src/affinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-06 14:47:17.000000 affinder-0.3.2/tox.ini
```

### Comparing `affinder-0.2.3/.github/workflows/build-docs.yml` & `affinder-0.3.2/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/.github/workflows/deploy-docs.yml` & `affinder-0.3.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/.github/workflows/plugin_preview.yml` & `affinder-0.3.2/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/.github/workflows/test_and_deploy.yml` & `affinder-0.3.2/.github/workflows/test_and_deploy.yml`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9]
+        python-version: ['3.9', '3.10']
 
     steps:
-      - uses: actions/checkout@v2
-
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       # these libraries enable testing on Qt on linux
       - uses: tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
@@ -46,46 +45,46 @@
       # note: if you need dependencies from conda, considering using
       # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
       # and
       # tox-conda: https://github.com/tox-dev/tox-conda
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools tox tox-gh-actions
+          python -m pip install setuptools tox tox-gh-actions
           python -m pip install .[testing]
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v3
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your 
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools setuptools_scm wheel twine
+          pip install -U setuptools setuptools_scm wheel twine build
       - name: Build and publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
         run: |
           git tag
-          python setup.py sdist bdist_wheel
+          python -m build .
           twine upload dist/*
```

### Comparing `affinder-0.2.3/.gitignore` & `affinder-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/.napari/DESCRIPTION.md` & `affinder-0.3.2/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/.style.yapf` & `affinder-0.3.2/.style.yapf`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/LICENSE` & `affinder-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/PKG-INFO` & `affinder-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: affinder
-Version: 0.2.3
+Version: 0.3.2
 Summary: Quickly find the affine matrix mapping one image to another using manual correspondence points annotation
 Home-page: https://github.com/jni/affinder
 Author: Juan Nunez-Iglesias
 Author-email: juan.nunez-iglesias@monash.edu
 License: BSD-3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # affinder
 
@@ -78,9 +76,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/jni/affinder/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `affinder-0.2.3/README.md` & `affinder-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/docs/Makefile` & `affinder-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/docs/conf.py` & `affinder-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/docs/index.rst` & `affinder-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/docs/make.bat` & `affinder-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/docs/replace_description_text.py` & `affinder-0.3.2/docs/replace_description_text.py`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/examples/basic-example.py` & `affinder-0.3.2/examples/basic-example.py`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/setup.cfg` & `affinder-0.3.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Framework :: napari
 	Topic :: Software Development :: Testing
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	License :: OSI Approved :: BSD License
 
 [options]
 package_dir = 
 	=src
 include_package_data = True
 packages = find:
 setup_requires = setuptools_scm
 install_requires = 
-	napari>=0.4.12
+	napari>=0.4.17
 	npe2>=0.1.2
 	numpy
 	scikit-image
 	magicgui>=0.3.7
 	toolz
-python_requires = >=3.7
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = affinder=affinder.main:main
 napari.manifest = 
@@ -47,15 +46,17 @@
 [options.extras_require]
 testing = 
 	coverage
 	pytest
 	pytest-cov
 	pytest-qt
 	scikit-image[data]
-	napari[pyqt5]
+	napari[pyqt5]!=0.4.18
+	pygments!=2.16
+	zarr
 docs = 
 	furo
 	myst-parser
 
 [options.package_data]
 affinder = napari.yaml
```

### Comparing `affinder-0.2.3/src/affinder/_tests/labels0.zarr/0.0` & `affinder-0.3.2/src/affinder/_tests/labels0.zarr/0.0`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/src/affinder/_tests/labels1.zarr/0.0` & `affinder-0.3.2/src/affinder/_tests/labels1.zarr/0.0`

 * *Files identical despite different names*

### Comparing `affinder-0.2.3/src/affinder/_tests/test_affinder.py` & `affinder-0.3.2/src/affinder/_tests/test_affinder.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,7 +79,22 @@
 
     actual_affine = np.asarray(l1.affine)
     expected_affine = np.array([[0.48155037, 0.85804854, 5.43577937],
                                 [-0.88088632, 0.49188026, 328.20642821],
                                 [0., 0., 1.]])
 
     np.testing.assert_allclose(actual_affine, expected_affine)
+
+
+def test_ensure_different_layers(make_napari_viewer):
+    viewer = make_napari_viewer()
+    image0 = np.random.random((50, 50))
+    image1 = np.random.random((30, 30))
+    image2 = np.random.random((40, 40))
+    for image in [image0, image1, image2]:
+        viewer.add_image(image)
+    qtwidget, widget = viewer.window.add_plugin_dock_widget(
+            'affinder', 'Start affinder'
+            )
+    assert widget.reference.value != widget.moving.value
+    widget.reference.value = widget.moving.value
+    assert widget.reference.value != widget.moving.value
```

### Comparing `affinder-0.2.3/src/affinder/affinder.py` & `affinder-0.3.2/src/affinder/affinder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from typing import Optional
 
 from enum import Enum
 import pathlib
 import toolz as tz
 from magicgui import magicgui, magic_factory
 import numpy as np
@@ -21,15 +22,18 @@
 def reset_view(viewer: 'napari.Viewer', layer: 'napari.layers.Layer'):
     if viewer.dims.ndisplay != 2:
         return
     extent = layer.extent.world[:, viewer.dims.displayed]
     size = extent[1] - extent[0]
     center = extent[0] + size/2
     viewer.camera.center = center
-    viewer.camera.zoom = np.min(viewer._canvas_size) / np.max(size)
+    with warnings.catch_warnings():
+        warnings.simplefilter('ignore')
+        canvas_size = viewer._canvas_size
+    viewer.camera.zoom = np.min(canvas_size) / np.max(size)
 
 
 @tz.curry
 def next_layer_callback(
         value,  # we ignore the arguments returned with the event -- we will
         *args,  # instead introspect the layer data and selection state
         viewer,
@@ -78,15 +82,50 @@
 @magicgui
 def close_affinder(layers, callback):
     for layer in layers:
         layer.events.data.disconnect(callback)
         layer.mode = 'pan_zoom'
 
 
+def _update_unique_choices(widget, choice_name):
+    """Update the selected choice in a ComboBox widget to be unique.
+
+    When `choice_name` is selected by another widget, and the choice in
+    `widget` needs to be different, this callback can be called to update the
+    choice in `widget`.
+    """
+    if not isinstance(choice_name, str):
+        # in some circumstances, widget.changed.connect passes the choice
+        # name to the callback, and in other cases it's the actual choice
+        # value. Here we coerce it to always be the name but that's an
+        # arbitrary choice.
+        choice_name = choice_name.name
+    choices = widget.choices
+    choice_names = [value.name for value in choices]
+    index = choice_names.index(choice_name)
+    value = widget.choices[index]
+    if widget.value is value:
+        next_index = (index+1) % len(choices)
+        with widget.changed.blocked():
+            widget.value = widget.choices[next_index]
+
+
+def _on_affinder_main_init(widget):
+    """Make sure that the reference and moving image are not the same."""
+    widget.reference.changed.connect(
+            lambda v: _update_unique_choices(widget.moving, v)
+            )
+    widget.moving.changed.connect(
+            lambda v: _update_unique_choices(widget.reference, v)
+            )
+    _update_unique_choices(widget.moving, widget.reference.current_choice)
+
+
 @magic_factory(
+        widget_init=_on_affinder_main_init,
         call_button='Start',
         layout='vertical',
         output={'mode': 'w'},
         viewer={'visible': False, 'label': ' '},
         )
 def start_affinder(
         viewer: 'napari.viewer.Viewer',
```

### Comparing `affinder-0.2.3/src/affinder.egg-info/PKG-INFO` & `affinder-0.3.2/src/affinder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: affinder
-Version: 0.2.3
+Version: 0.3.2
 Summary: Quickly find the affine matrix mapping one image to another using manual correspondence points annotation
 Home-page: https://github.com/jni/affinder
 Author: Juan Nunez-Iglesias
 Author-email: juan.nunez-iglesias@monash.edu
 License: BSD-3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 # affinder
 
@@ -78,9 +76,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [file an issue]: https://github.com/jni/affinder/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `affinder-0.2.3/src/affinder.egg-info/SOURCES.txt` & `affinder-0.3.2/src/affinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

