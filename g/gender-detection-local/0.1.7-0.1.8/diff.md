# Comparing `tmp/gender-detection-local-0.1.7.tar.gz` & `tmp/gender-detection-local-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-detection-local-0.1.7.tar", last modified: Wed Aug  2 15:20:51 2023, max compression
+gzip compressed data, was "gender-detection-local-0.1.8.tar", last modified: Sun Aug  6 08:11:50 2023, max compression
```

## Comparing `gender-detection-local-0.1.7.tar` & `gender-detection-local-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/CirclesGenderDetectionPython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-02 15:20:37.000000 gender-detection-local-0.1.7/CirclesGenderDetectionPython/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/gender_detection_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:20:51.000000 gender-detection-local-0.1.7/gender_detection_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:20:51.305804 gender-detection-local-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 15:20:38.000000 gender-detection-local-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:11:50.344446 gender-detection-local-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:11:50.340446 gender-detection-local-0.1.8/CirclesGenderDetectionPython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:11:34.000000 gender-detection-local-0.1.8/CirclesGenderDetectionPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7030816 2023-08-06 08:11:34.000000 gender-detection-local-0.1.8/CirclesGenderDetectionPython/gender_detection
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-08-06 08:11:34.000000 gender-detection-local-0.1.8/CirclesGenderDetectionPython/gender_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-06 08:11:34.000000 gender-detection-local-0.1.8/CirclesGenderDetectionPython/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 08:11:50.340446 gender-detection-local-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-06 08:11:35.000000 gender-detection-local-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:11:50.340446 gender-detection-local-0.1.8/gender_detection_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 08:11:50.000000 gender-detection-local-0.1.8/gender_detection_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-06 08:11:50.000000 gender-detection-local-0.1.8/gender_detection_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:11:50.000000 gender-detection-local-0.1.8/gender_detection_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-06 08:11:50.000000 gender-detection-local-0.1.8/gender_detection_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-06 08:11:35.000000 gender-detection-local-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 08:11:50.344446 gender-detection-local-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-06 08:11:35.000000 gender-detection-local-0.1.8/setup.py
```

### Comparing `gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection` & `gender-detection-local-0.1.8/CirclesGenderDetectionPython/gender_detection`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.7/CirclesGenderDetectionPython/gender_detection.py` & `gender-detection-local-0.1.8/CirclesGenderDetectionPython/gender_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         # Apply data augmentation
         if rand() < 0.5:
             image = flip_left_right(image)
 
         model = load_model(model_path)
         prediction = model.predict(expand_dims(image, axis=0))[0]
-        self.lgrins.info("Prediction Confidence (>0.5 Male,<=0.5 Female)",prediction)
+        self.lgrins.info("Prediction Confidence (>0.5 Male,<=0.5 Female): "+prediction)
         if prediction > 0.5:
             #print("Male")
             self.lgrins.stop()
             return "Male"
         else:
             #print("Female")
             self.lgrins.stop()
```

### Comparing `gender-detection-local-0.1.7/README.md` & `gender-detection-local-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gender-detection-local-0.1.7/setup.py` & `gender-detection-local-0.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
      name='gender-detection-local',  
-     version='0.1.7',
+     version='0.1.8',
      author="Circles",
      author_email="info@circles.zone",
      description="PyPI Package for gender detection",
      long_description="This is a package for running gender detection and predicting gender",
      long_description_content_type="text/markdown",
      url="https://github.com/circles-zone/gender-detection-local-python-package",
      packages=setuptools.find_packages(),
```

