# Comparing `tmp/reclist-2.0.1.tar.gz` & `tmp/reclist-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reclist-2.0.1.tar", last modified: Tue Jul 25 03:36:06 2023, max compression
+gzip compressed data, was "reclist-2.1.0.tar", last modified: Sun Aug  6 21:23:26 2023, max compression
```

## Comparing `reclist-2.0.1.tar` & `reclist-2.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      165 2023-02-28 04:47:32.000000 reclist-2.0.1/AUTHORS.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     3499 2023-02-28 04:47:32.000000 reclist-2.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       89 2023-02-28 04:47:32.000000 reclist-2.0.1/HISTORY.rst
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-07-14 01:35:32.000000 reclist-2.0.1/LICENSE
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      317 2023-07-25 03:35:16.000000 reclist-2.0.1/MANIFEST.in
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 03:36:06.209228 reclist-2.0.1/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    13598 2023-07-25 01:02:28.000000 reclist-2.0.1/README.rst
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      103 2023-07-25 03:36:04.000000 reclist-2.0.1/reclist/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      107 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/charts.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     2884 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/logs.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1612 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metadata.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist/metrics/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-02-28 04:47:32.000000 reclist-2.0.1/reclist/metrics/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     7003 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/distance_metrics.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     4855 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/hits.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1032 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/perturbation.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1567 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/metrics/price_homogeneity.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    11840 2023-07-24 17:02:51.000000 reclist-2.0.1/reclist/metrics/standard_metrics.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     9036 2023-07-24 17:02:51.000000 reclist-2.0.1/reclist/reclist.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     5106 2023-07-14 01:35:32.000000 reclist-2.0.1/reclist/similarity_models.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/reclist.egg-info/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/PKG-INFO
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      667 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/SOURCES.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/dependency_links.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-03-11 01:25:56.000000 reclist-2.0.1/reclist.egg-info/not-zip-safe
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      258 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/requires.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)        8 2023-07-25 03:36:06.000000 reclist-2.0.1/reclist.egg-info/top_level.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      204 2023-07-24 17:02:51.000000 reclist-2.0.1/requirements.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      159 2023-07-17 19:47:56.000000 reclist-2.0.1/requirements_dev.txt
--rw-rw-r--   0 vinid     (1000) vinid     (1000)      424 2023-07-25 03:36:06.209228 reclist-2.0.1/setup.cfg
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     1540 2023-07-25 03:36:04.000000 reclist-2.0.1/setup.py
-drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 03:36:06.209228 reclist-2.0.1/tests/
--rw-rw-r--   0 vinid     (1000) vinid     (1000)       37 2023-02-28 04:47:32.000000 reclist-2.0.1/tests/__init__.py
--rw-rw-r--   0 vinid     (1000) vinid     (1000)     2619 2023-07-17 19:47:56.000000 reclist-2.0.1/tests/test_reclist.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-08-06 21:23:26.120066 reclist-2.1.0/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      165 2023-02-28 04:47:32.000000 reclist-2.1.0/AUTHORS.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     3499 2023-02-28 04:47:32.000000 reclist-2.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       89 2023-02-28 04:47:32.000000 reclist-2.1.0/HISTORY.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-07-14 01:35:32.000000 reclist-2.1.0/LICENSE
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      317 2023-07-25 03:35:16.000000 reclist-2.1.0/MANIFEST.in
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    15800 2023-08-06 21:23:26.120066 reclist-2.1.0/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    15007 2023-08-06 21:19:04.000000 reclist-2.1.0/README.rst
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-08-06 21:23:26.120066 reclist-2.1.0/reclist/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      103 2023-08-06 21:21:41.000000 reclist-2.1.0/reclist/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      107 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/charts.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2884 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/logs.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1612 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/metadata.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-08-06 21:23:26.120066 reclist-2.1.0/reclist/metrics/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-02-28 04:47:32.000000 reclist-2.1.0/reclist/metrics/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     7003 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/metrics/distance_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     4855 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/metrics/hits.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1032 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/metrics/perturbation.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1567 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/metrics/price_homogeneity.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    12217 2023-08-06 21:19:04.000000 reclist-2.1.0/reclist/metrics/standard_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     9036 2023-07-24 17:02:51.000000 reclist-2.1.0/reclist/reclist.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     5106 2023-07-14 01:35:32.000000 reclist-2.1.0/reclist/similarity_models.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-08-06 21:23:26.120066 reclist-2.1.0/reclist.egg-info/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    15800 2023-08-06 21:23:26.000000 reclist-2.1.0/reclist.egg-info/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      667 2023-08-06 21:23:26.000000 reclist-2.1.0/reclist.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-08-06 21:23:26.000000 reclist-2.1.0/reclist.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-03-11 01:25:56.000000 reclist-2.1.0/reclist.egg-info/not-zip-safe
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      258 2023-08-06 21:23:26.000000 reclist-2.1.0/reclist.egg-info/requires.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        8 2023-08-06 21:23:26.000000 reclist-2.1.0/reclist.egg-info/top_level.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      204 2023-07-24 17:02:51.000000 reclist-2.1.0/requirements.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      159 2023-07-17 19:47:56.000000 reclist-2.1.0/requirements_dev.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      424 2023-08-06 21:23:26.120066 reclist-2.1.0/setup.cfg
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1540 2023-08-06 21:21:41.000000 reclist-2.1.0/setup.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-08-06 21:23:26.120066 reclist-2.1.0/tests/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       37 2023-02-28 04:47:32.000000 reclist-2.1.0/tests/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     3088 2023-08-06 21:19:04.000000 reclist-2.1.0/tests/test_reclist.py
```

### Comparing `reclist-2.0.1/CONTRIBUTING.rst` & `reclist-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/LICENSE` & `reclist-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/PKG-INFO` & `reclist-2.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: reclist
-Version: 2.0.1
-Summary: RecList
-Home-page: https://github.com/jacopotagliabue/reclist
-Author: RecList
-Author-email: 
-License: MIT license
-Keywords: reclist
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 =======
 RecList
 =======
 
 .. image:: images/reclist.png
         :width: 30%
         :alt: Rocket Emoji
@@ -211,15 +188,15 @@
             from random import randint
 
             return { "luck_number": randint(0, 100) }
 
 
 Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
 and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
-RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see *dummy.py* for an example with different input types).
 
 Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
 (name of the suite, name of the model, run timestamp):
 
 .. code-block::
 
     .reclist/
@@ -239,18 +216,59 @@
 
 * tests and metrics to be used on your own datasets and models;
 
 * automated storage of results, with versioning, both in a local folder or on S3;
 
 * flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
 
-* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see below);
 
 * reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
 
+Using Third-Party Tracking Tools
+--------------------------------
+
+*RecList* supports streaming the results of your tests directly to your cloud platform of choice, both as metrics and charts.
+
+If you have the `Python client installed <https://docs.neptune.ai/about/api/>`__, you can use the
+Neptune logger by simply specifying it at init time, and either passing *NEPTUNE_KEY* and *NEPTUNE_PROJECT_NAME* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.NEPTUNE,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+If you have the `Python client installed <https://pypi.org/project/comet-ml/>`__, you can use the
+Comet logger by simply specifying it at init time, and either passing *COMET_KEY*, *COMET_PROJECT_NAME*, *COMET_WORKSPACE* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.COMET,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+
+If you wish to add a new platform, you can do so by simply implementing a new class inheriting from RecLogger.
 
 Acknowledgments
 ---------------
 
 The original authors are:
 
 * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
@@ -293,17 +311,7 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (2021-11-16)
-------------------
-
-* First release on PyPI.
```

### Comparing `reclist-2.0.1/README.rst` & `reclist-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: reclist
+Version: 2.1.0
+Summary: RecList
+Home-page: https://github.com/jacopotagliabue/reclist
+Author: RecList
+Author-email: 
+License: MIT license
+Keywords: reclist
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 =======
 RecList
 =======
 
 .. image:: images/reclist.png
         :width: 30%
         :alt: Rocket Emoji
@@ -188,15 +211,15 @@
             from random import randint
 
             return { "luck_number": randint(0, 100) }
 
 
 Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
 and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
-RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see *dummy.py* for an example with different input types).
 
 Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
 (name of the suite, name of the model, run timestamp):
 
 .. code-block::
 
     .reclist/
@@ -216,18 +239,59 @@
 
 * tests and metrics to be used on your own datasets and models;
 
 * automated storage of results, with versioning, both in a local folder or on S3;
 
 * flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
 
-* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see below);
 
 * reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
 
+Using Third-Party Tracking Tools
+--------------------------------
+
+*RecList* supports streaming the results of your tests directly to your cloud platform of choice, both as metrics and charts.
+
+If you have the `Python client installed <https://docs.neptune.ai/about/api/>`__, you can use the
+Neptune logger by simply specifying it at init time, and either passing *NEPTUNE_KEY* and *NEPTUNE_PROJECT_NAME* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.NEPTUNE,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+If you have the `Python client installed <https://pypi.org/project/comet-ml/>`__, you can use the
+Comet logger by simply specifying it at init time, and either passing *COMET_KEY*, *COMET_PROJECT_NAME*, *COMET_WORKSPACE* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.COMET,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+
+If you wish to add a new platform, you can do so by simply implementing a new class inheriting from RecLogger.
 
 Acknowledgments
 ---------------
 
 The original authors are:
 
 * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
@@ -270,7 +334,17 @@
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-11-16)
+------------------
+
+* First release on PyPI.
```

### Comparing `reclist-2.0.1/reclist/logs.py` & `reclist-2.1.0/reclist/logs.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metadata.py` & `reclist-2.1.0/reclist/metadata.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metrics/distance_metrics.py` & `reclist-2.1.0/reclist/metrics/distance_metrics.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metrics/hits.py` & `reclist-2.1.0/reclist/metrics/hits.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metrics/perturbation.py` & `reclist-2.1.0/reclist/metrics/perturbation.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metrics/price_homogeneity.py` & `reclist-2.1.0/reclist/metrics/price_homogeneity.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/metrics/standard_metrics.py` & `reclist-2.1.0/reclist/metrics/standard_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,24 @@
     >>> y_pred = pd.DataFrame([[1, 2, 4], [3, 6, 2]])
     >>> y_test = pd.DataFrame([[5, 1, 0], [6, 2, 3]])
     >>> hits_at_k(y_pred, y_test, k=2)
     array([[0, 1, 0],
            [2, 0, 1]])
 
     """
-
     hits = hits_at_k(y_pred, y_test, k)                     # N x M x k
-    ranks = hits * np.arange(1, k + 1, 1)[None, None, :]    # N x M x k
-    ranks = ranks.max(axis=2)                               # N x M
+    # TODO: hits_at_k can be modified to return df with last dim=k instead of preds shape
+    rank_overlap = min(k, hits.shape[-1])
+    ranks = hits * np.arange(1, rank_overlap + 1, 1)[None, None, :]    # N x M x k
+    # set to float
+    ranks = ranks.astype(float)
+    # set non-hits to infinity
+    ranks[ranks==0] = np.inf
+    # get highest rank; if no hit, rank is infinite
+    ranks = ranks.min(axis=2)                               # N x M
     return ranks
 
 
 def misses_at_k(
     y_pred: pd.DataFrame,
     y_test: pd.DataFrame,
     k: int
@@ -235,15 +241,16 @@
     >>> y_pred = pd.DataFrame([[2, 1, 4], [3, 6, 2]])
     >>> y_test = pd.DataFrame([[5, 1, 0], [2, 1, 0]])
     >>> rr_at_k(y_pred, y_test, k=2)
     array([0.5, 0.0])
     """
     
     ranks = ranks_at_k(y_pred, y_test, k).astype(np.float64)  # N x M
-    reciprocal_ranks = np.reciprocal(ranks, out=ranks, where=ranks > 0)  # N x M
+    reciprocal_ranks = np.reciprocal(ranks, out=ranks,)       # N x M
+    # reciprocal_ranks = np.reciprocal(ranks, out=ranks, where=ranks > 0)  # N x M
     return reciprocal_ranks.max(axis=1)  # N
 
 
 def mrr_at_k(
     y_pred: pd.DataFrame, 
     y_test: pd.DataFrame, 
     k: int
```

### Comparing `reclist-2.0.1/reclist/reclist.py` & `reclist-2.1.0/reclist/reclist.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist/similarity_models.py` & `reclist-2.1.0/reclist/similarity_models.py`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/reclist.egg-info/PKG-INFO` & `reclist-2.1.0/reclist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reclist
-Version: 2.0.1
+Version: 2.1.0
 Summary: RecList
 Home-page: https://github.com/jacopotagliabue/reclist
 Author: RecList
 Author-email: 
 License: MIT license
 Keywords: reclist
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -211,15 +211,15 @@
             from random import randint
 
             return { "luck_number": randint(0, 100) }
 
 
 Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
 and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
-RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see *dummy.py* for an example with different input types).
 
 Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
 (name of the suite, name of the model, run timestamp):
 
 .. code-block::
 
     .reclist/
@@ -239,18 +239,59 @@
 
 * tests and metrics to be used on your own datasets and models;
 
 * automated storage of results, with versioning, both in a local folder or on S3;
 
 * flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
 
-* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see below);
 
 * reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
 
+Using Third-Party Tracking Tools
+--------------------------------
+
+*RecList* supports streaming the results of your tests directly to your cloud platform of choice, both as metrics and charts.
+
+If you have the `Python client installed <https://docs.neptune.ai/about/api/>`__, you can use the
+Neptune logger by simply specifying it at init time, and either passing *NEPTUNE_KEY* and *NEPTUNE_PROJECT_NAME* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.NEPTUNE,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+If you have the `Python client installed <https://pypi.org/project/comet-ml/>`__, you can use the
+Comet logger by simply specifying it at init time, and either passing *COMET_KEY*, *COMET_PROJECT_NAME*, *COMET_WORKSPACE* as kwargs, or setting them as environment variables.
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.COMET,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model
+    )
+
+    cdf(verbose=True)
+
+
+If you wish to add a new platform, you can do so by simply implementing a new class inheriting from RecLogger.
 
 Acknowledgments
 ---------------
 
 The original authors are:
 
 * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
```

### Comparing `reclist-2.0.1/reclist.egg-info/SOURCES.txt` & `reclist-2.1.0/reclist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reclist-2.0.1/setup.py` & `reclist-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,13 +51,13 @@
     keywords="reclist",
     name="reclist",
     packages=find_packages(include=["reclist", "reclist.*"]),
     test_suite="tests",
     tests_require=test_requirements,
 
     url='https://github.com/jacopotagliabue/reclist',
-    version='2.0.1',
+    version='2.1.0',
     zip_safe=False,
     extras_require={
         "dev": style_packages + ["pre-commit==2.20.0"],
     },
 )
```

### Comparing `reclist-2.0.1/tests/test_reclist.py` & `reclist-2.1.0/tests/test_reclist.py`

 * *Files 26% similar despite different names*

```diff
@@ -77,22 +77,40 @@
         [[0, 2, 14, 32, None],
          [1, 8,  7, None, None]]
     )
     df_e = pd.DataFrame(
         [[10, 12, 14, None, None, None], 
          [22, 8, 64, 13, 1, 0]]
     )
+    df_f = pd.DataFrame(
+        [[10, 12, 14, None, None, None], 
+         [22, 1, 64, 13, 1, 0]]
+    )
+
+    df_g = pd.DataFrame(
+        [[10, 12, 14, None, None, None], 
+         [22, 17, 64, 13, 1, 0]]
+    )
     # df_f = pd.DataFrame(
     #     [[2, 3], 
     #      [0, 1]]
     #     )
     
     # basic tests
     assert mrr_at_k(df_b, df_a, 1) == 1
     assert mrr_at_k(df_c, df_a, 2) == 0.25
     assert mrr_at_k(df_c, df_a, 1) == 0
 
     # multi target tests
     assert mrr_at_k(df_e, df_d, 2) == 1/4
     assert mrr_at_k(df_e, df_d, 3) == pytest.approx(5/12)
     assert mrr_at_k(df_e, df_d, 6) == pytest.approx(5/12)
+
+    # k larger than pred size
+    assert mrr_at_k(df_e, df_d, 20) == pytest.approx(5/12)
+    
+    # repeated prediction that is a hit
+    assert mrr_at_k(df_f, df_d, 6) == pytest.approx(5/12)
+
+    assert mrr_at_k(df_g, df_d, 6) == pytest.approx(4/15)
+
```

