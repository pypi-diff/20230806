# Comparing `tmp/pyPPG-1.0.4.tar.gz` & `tmp/pyPPG-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.4.tar", last modified: Sun Aug  6 09:52:11 2023, max compression
+gzip compressed data, was "pyPPG-1.0.5.tar", last modified: Sun Aug  6 10:13:16 2023, max compression
```

## Comparing `pyPPG-1.0.4.tar` & `pyPPG-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.355141 pyPPG-1.0.4/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4036 2023-08-06 09:52:11.355141 pyPPG-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.325381 pyPPG-1.0.4/pyPPG/
--rw-rw-rw-   0        0        0     3195 2023-07-31 14:17:03.000000 pyPPG-1.0.4/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0     9414 2023-07-31 12:37:20.000000 pyPPG-1.0.4/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     2206 2023-08-06 08:07:59.000000 pyPPG-1.0.4/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49740 2023-07-31 14:17:03.000000 pyPPG-1.0.4/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.4/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.4/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.4/pyPPG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.350090 pyPPG-1.0.4/pyPPG/pack_ppg/
--rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.4/pyPPG/pack_ppg/_ErrorHandler.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.4/pyPPG/pack_ppg/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.4/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.353590 pyPPG-1.0.4/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.4/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_biomarkers.py
--rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.348352 pyPPG-1.0.4/pyPPG.egg-info/
--rw-rw-rw-   0        0        0     4036 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 09:52:11.355141 pyPPG-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-08-06 09:52:06.000000 pyPPG-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.383415 pyPPG-1.0.5/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4069 2023-08-06 10:13:16.383415 pyPPG-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3448 2023-08-06 10:11:22.000000 pyPPG-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.369561 pyPPG-1.0.5/pyPPG/
+-rw-rw-rw-   0        0        0     3195 2023-07-31 14:17:03.000000 pyPPG-1.0.5/pyPPG/Biomarkers.py
+-rw-rw-rw-   0        0        0     9414 2023-07-31 12:37:20.000000 pyPPG-1.0.5/pyPPG/DataHandling.py
+-rw-rw-rw-   0        0        0     2206 2023-08-06 08:07:59.000000 pyPPG-1.0.5/pyPPG/EXAMPLE.py
+-rw-rw-rw-   0        0        0    49740 2023-07-31 14:17:03.000000 pyPPG-1.0.5/pyPPG/FiducialPoints.py
+-rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.5/pyPPG/Preprocessing.py
+-rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.5/pyPPG/Statistics.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.5/pyPPG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.379084 pyPPG-1.0.5/pyPPG/pack_ppg/
+-rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.5/pyPPG/pack_ppg/_ErrorHandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.5/pyPPG/pack_ppg/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.5/pyPPG/ppgSQI.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.382359 pyPPG-1.0.5/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.5/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_biomarkers.py
+-rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_derivs_ratios.py
+-rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_derivs.py
+-rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_sig.py
+-rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_sig_ratios.py
+drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.378141 pyPPG-1.0.5/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0     4069 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 10:13:16.384016 pyPPG-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-08-06 10:11:45.000000 pyPPG-1.0.5/setup.py
```

### Comparing `pyPPG-1.0.4/LICENSE.txt` & `pyPPG-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/PKG-INFO` & `pyPPG-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.4
+Version: 1.0.5
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -29,26 +29,28 @@
 2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
 3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
 5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
-![img.png](figs/pyPPG_pipeline.svg).
+![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
-![alt text](figs/PPG_sample.svg)
+![](figs/PPG_sample.svg)
 
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
+pip project: https://pypi.org/project/pyPPG/
+
 ## Requirements
 ### Python Requirements:
 
 Python >= 3.10
 
 scipy == 1.9.1
```

### Comparing `pyPPG-1.0.4/README.md` & `pyPPG-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
 3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
 5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
-![img.png](figs/pyPPG_pipeline.svg).
+![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
-![alt text](figs/PPG_sample.svg)
+![](figs/PPG_sample.svg)
 
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
+pip project: https://pypi.org/project/pyPPG/
+
 ## Requirements
 ### Python Requirements:
 
 Python >= 3.10
 
 scipy == 1.9.1
```

### Comparing `pyPPG-1.0.4/pyPPG/Biomarkers.py` & `pyPPG-1.0.5/pyPPG/Biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/DataHandling.py` & `pyPPG-1.0.5/pyPPG/DataHandling.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/EXAMPLE.py` & `pyPPG-1.0.5/pyPPG/EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/FiducialPoints.py` & `pyPPG-1.0.5/pyPPG/FiducialPoints.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/Preprocessing.py` & `pyPPG-1.0.5/pyPPG/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/Statistics.py` & `pyPPG-1.0.5/pyPPG/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppgSQI.py` & `pyPPG-1.0.5/pyPPG/ppgSQI.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppg_bm/get_biomarkers.py` & `pyPPG-1.0.5/pyPPG/ppg_bm/get_biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_derivs_ratios.py` & `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_derivs_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_derivs.py` & `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_derivs.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_sig.py` & `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_sig.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_sig_ratios.py` & `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_sig_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.4/pyPPG.egg-info/PKG-INFO` & `pyPPG-1.0.5/pyPPG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.4
+Version: 1.0.5
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -29,26 +29,28 @@
 2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
 3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
 5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
-![img.png](figs/pyPPG_pipeline.svg).
+![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
-![alt text](figs/PPG_sample.svg)
+![](figs/PPG_sample.svg)
 
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
+pip project: https://pypi.org/project/pyPPG/
+
 ## Requirements
 ### Python Requirements:
 
 Python >= 3.10
 
 scipy == 1.9.1
```

### Comparing `pyPPG-1.0.4/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.5/pyPPG.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,16 +19,8 @@
 pyPPG/pack_ppg/_ErrorHandler.py
 pyPPG/pack_ppg/__init__.py
 pyPPG/ppg_bm/__init__.py
 pyPPG/ppg_bm/get_biomarkers.py
 pyPPG/ppg_bm/get_bm_derivs_ratios.py
 pyPPG/ppg_bm/get_bm_ppg_derivs.py
 pyPPG/ppg_bm/get_bm_ppg_sig.py
-pyPPG/ppg_bm/get_bm_sig_ratios.py
-pyPPG/pack_ppg/_ErrorHandler.py
-pyPPG/pack_ppg/__init__.py
-pyPPG/ppg_bm/__init__.py
-pyPPG/ppg_bm/get_biomarkers.py
-pyPPG/ppg_bm/get_bm_derivs_ratios.py
-pyPPG/ppg_bm/get_bm_ppg_derivs.py
-pyPPG/ppg_bm/get_bm_ppg_sig.py
 pyPPG/ppg_bm/get_bm_sig_ratios.py
```

### Comparing `pyPPG-1.0.4/setup.py` & `pyPPG-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyPPG',
-    version='1.0.4',
+    version='1.0.5',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
```

