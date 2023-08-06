# Comparing `tmp/pyPPG-1.0.3.tar.gz` & `tmp/pyPPG-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.3.tar", last modified: Mon Jul 31 07:41:09 2023, max compression
+gzip compressed data, was "pyPPG-1.0.4.tar", last modified: Sun Aug  6 09:52:11 2023, max compression
```

## Comparing `pyPPG-1.0.3.tar` & `pyPPG-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.200176 pyPPG-1.0.3/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.3/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      619 2023-07-31 07:41:09.200176 pyPPG-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.172618 pyPPG-1.0.3/pyPPG/
--rw-rw-rw-   0        0        0     3194 2023-07-26 11:45:26.000000 pyPPG-1.0.3/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0    19510 2023-07-31 07:08:30.000000 pyPPG-1.0.3/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     2204 2023-07-30 08:11:19.000000 pyPPG-1.0.3/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49745 2023-07-30 11:49:30.000000 pyPPG-1.0.3/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1845 2023-07-27 08:06:54.000000 pyPPG-1.0.3/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1906 2023-07-26 12:38:04.000000 pyPPG-1.0.3/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.3/pyPPG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.193787 pyPPG-1.0.3/pyPPG/pack_ppg/
--rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.3/pyPPG/pack_ppg/_ErrorHandler.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.3/pyPPG/pack_ppg/__init__.py
--rw-rw-rw-   0        0        0     4945 2023-07-23 15:56:13.000000 pyPPG-1.0.3/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.198837 pyPPG-1.0.3/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.3/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_biomarkers.py
--rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:41:09.192159 pyPPG-1.0.3/pyPPG.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-07-31 07:41:09.000000 pyPPG-1.0.3/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 07:41:09.200176 pyPPG-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-07-31 07:39:37.000000 pyPPG-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.355141 pyPPG-1.0.4/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4036 2023-08-06 09:52:11.355141 pyPPG-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3415 2023-07-27 14:35:58.000000 pyPPG-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.325381 pyPPG-1.0.4/pyPPG/
+-rw-rw-rw-   0        0        0     3195 2023-07-31 14:17:03.000000 pyPPG-1.0.4/pyPPG/Biomarkers.py
+-rw-rw-rw-   0        0        0     9414 2023-07-31 12:37:20.000000 pyPPG-1.0.4/pyPPG/DataHandling.py
+-rw-rw-rw-   0        0        0     2206 2023-08-06 08:07:59.000000 pyPPG-1.0.4/pyPPG/EXAMPLE.py
+-rw-rw-rw-   0        0        0    49740 2023-07-31 14:17:03.000000 pyPPG-1.0.4/pyPPG/FiducialPoints.py
+-rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.4/pyPPG/Preprocessing.py
+-rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.4/pyPPG/Statistics.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.4/pyPPG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.350090 pyPPG-1.0.4/pyPPG/pack_ppg/
+-rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.4/pyPPG/pack_ppg/_ErrorHandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.4/pyPPG/pack_ppg/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.4/pyPPG/ppgSQI.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.353590 pyPPG-1.0.4/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.4/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_biomarkers.py
+-rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_derivs_ratios.py
+-rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_derivs.py
+-rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_sig.py
+-rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_sig_ratios.py
+drwxrwxrwx   0        0        0        0 2023-08-06 09:52:11.348352 pyPPG-1.0.4/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0     4036 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-08-06 09:52:11.000000 pyPPG-1.0.4/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 09:52:11.355141 pyPPG-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-08-06 09:52:06.000000 pyPPG-1.0.4/setup.py
```

### Comparing `pyPPG-1.0.3/LICENSE.txt` & `pyPPG-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/README.md` & `pyPPG-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG/Biomarkers.py` & `pyPPG-1.0.4/pyPPG/Biomarkers.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     ###########################################################################
     ############################ Get PPG Biomarkers ###########################
     ###########################################################################
     def getBiomarkers (self):
         """
         This function returns the PPG biomarkers.
 
-        :return biomarkers: dictionary of biomarkers in different categories
+        :return: biomarkers dictionary of biomarkers in different categories:
             - PPG signal
             - Signal ratios
             - PPG derivatives
             - Derivatives ratios
         """
 
         s=self.s
```

### Comparing `pyPPG-1.0.3/pyPPG/EXAMPLE.py` & `pyPPG-1.0.4/pyPPG/EXAMPLE.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ###########################################################################
 def example_code(filtering=True,correct=True,savefig=True):
     '''
     This is an example code for PPG analysis. The main parts:
         1) Loading a raw PPG signal: various file formats such as .mat, .csv, .txt, or .edf.
         2) Get Fiducial points: extract the fiducial points of PPG, PPG', PPG'' and PPG'" signals
         3) Plot Fiducials Points
-        4) Get Biomarkers: extract 74 PPG biomarkers in four categories
+        4) Get Biomarkers: extract 74 PPG biomarkers in four categories:
             - PPG signal
             - Signal ratios
             - PPG derivatives
             - Derivatives ratios
         5) Get Statistics: summary of the 74 PPG biomarkers
         6) Save data: save the extracted Fiducial points, Biomarkers, and Statistics into .csv file
 
@@ -58,8 +58,8 @@
     print('Program finished')
 
 
 
 ###########################################################################
 ############################## RUN EXAMPLE CODE ###########################
 ###########################################################################
-example_code()
+#example_code()
```

### Comparing `pyPPG-1.0.3/pyPPG/FiducialPoints.py` & `pyPPG-1.0.4/pyPPG/FiducialPoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,15 +709,15 @@
     ###########################################################################
     ####################### Setup up the beat detector ########################
     ###########################################################################
     def setup_up_abdp_algorithm(self):
         """
         This function setups the filter parameters of the algorithm
 
-        :return: filter parameters of the algorithm, DotMap.
+        :return: filter parameters of the algorithm, DotMap
 
         """
         # plausible HR limits
         up=DotMap()
         up.fl = 30               #lower bound for HR
         up.fh = 200              #upper bound for HR
         up.fl_hz = up.fl/60
@@ -747,15 +747,15 @@
         :param up: setup up parameters of the algorithm
         :type up: DotMap
         :param peaks: peaks of the signal
         :type peaks: 1-d array
         :param med_hr: median heart rate
         :type med_hr: float
 
-        :return: onsets, 1-d array.
+        :return: onsets, 1-d array
 
         """
 
         Y1=self.Bandpass(sig, fs, 0.9*up.fl_hz, 3*up.fh_hz)
         temp_oi0=find_peaks(-Y1,distance=med_hr*0.3)[0]
 
         null_indexes = np.where(temp_oi0<peaks[0])
@@ -796,15 +796,15 @@
         Dicrotic Notch function estimate the location of dicrotic notch in between the systolic and diastolic peak
 
         :param peaks: peaks of the signal
         :type peaks: 1-d array
         :param onsets: onsets of the signal
         :type onsets: list
 
-        :return: location of dicrotic notches, 1-d array.
+        :return: location of dicrotic notches, 1-d array
         """
 
         ## The 2nd derivative and Hamming low pass filter is calculated.
         dxx = np.diff(np.diff(self.filt_sig))
         fs = self.fs
 
         # Make filter
@@ -883,15 +883,15 @@
         :param onsets: onsets of the signal
         :type onsets: list
         :param dicroticnotches: dicrotic notches of the signal
         :type dicroticnotches: list
         :param e_point: e-points of the signal
         :type e_point: pd.Series
 
-        :return diastolicpeak: location of dicrotic notches, 1-d array.
+        :return: diastolicpeak location of dicrotic notches, 1-d array
         """
 
         nan_v = np.empty(len(dicroticnotch))
         nan_v[:] = np.NaN
         diastolicpeak = nan_v
 
         for i in range(0,len(dicroticnotch)):
@@ -1153,15 +1153,15 @@
     def CorrectFiducialPoints(self,fiducials: pd.DataFrame):
         """Correct the Fiducial Points
 
             :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
             :type fiducials: DataFrame
 
             :return:
-                - fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
+                - fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
         """
 
         for i in range(0,len(fiducials.on)):
 
             # Correct onset
             try:
                 win_onr = self.fs * 0.005
```

### Comparing `pyPPG-1.0.3/pyPPG/Preprocessing.py` & `pyPPG-1.0.4/pyPPG/Preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     '''The function calculates the preprocessed PPG, PPG', PPG", and PPG'".
 
     :param s: a struct of PPG signal:
         - s.v: a vector of PPG values
         - s.fs: the sampling frequency of the PPG in Hz
     :type s: DotMap
 
-    :return filt_sig, filt_d1, filt_d2, filt_d3: preprocessed PPG, PPG', PPG", and PPG'"
+    :return: filt_sig, filt_d1, filt_d2, filt_d3: preprocessed PPG, PPG', PPG", and PPG'"
     '''
 
     ## PPG filtering
     if filtering:
         fL = 0.5
         fH = 12
         order = 4
```

### Comparing `pyPPG-1.0.3/pyPPG/Statistics.py` & `pyPPG-1.0.4/pyPPG/Statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :param peaks: 1-d array, peaks of the signal
     :type peaks: Series
     :param onsets: 1-d array, onsets of the signal
     :type onsets: Series
     :param ppg_biomarkers: dictionary of the PPG biomarkers
     :type ppg_biomarkers: dict
 
-    :return df_windows: data frame with summary of PPG features
+    :return: df_windows: data frame with summary of PPG features
     """
 
     BM_keys = list(ppg_biomarkers.keys())
     ppg_statistics={}
     for j in range (0, len(BM_keys)):
         df_features=ppg_biomarkers[BM_keys[j]]
```

### Comparing `pyPPG-1.0.3/pyPPG/ppgSQI.py` & `pyPPG-1.0.4/pyPPG/ppgSQI.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def ppgSQI(ppg, fs, ann_ppg):
     '''
     PPG Signal Quality Index based on beat template correlation.
 
     :param ppg: PPG data
     :param fs: Samples frequency
     :param ann_ppg: PPG annotation time(samples)
-    :return psqi: PPG SQI
+    :return: psqi: PPG Signal Quality Index
 
     Reference
     ---------
     Li, Qiao, and Gari D. Clifford. "Dynamic time warping and machine learning for signal quality assessment of pulsatile signals."
     Physiological measurement 33.9 (2012): 1491.
 
     Author:
```

### Comparing `pyPPG-1.0.3/pyPPG/ppg_bm/get_biomarkers.py` & `pyPPG-1.0.4/pyPPG/ppg_bm/get_biomarkers.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_derivs_ratios.py` & `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_derivs_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_derivs.py` & `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_derivs.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_ppg_sig.py` & `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_ppg_sig.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG/ppg_bm/get_bm_sig_ratios.py` & `pyPPG-1.0.4/pyPPG/ppg_bm/get_bm_sig_ratios.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.3/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.4/pyPPG.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,16 @@
 pyPPG/pack_ppg/_ErrorHandler.py
 pyPPG/pack_ppg/__init__.py
 pyPPG/ppg_bm/__init__.py
 pyPPG/ppg_bm/get_biomarkers.py
 pyPPG/ppg_bm/get_bm_derivs_ratios.py
 pyPPG/ppg_bm/get_bm_ppg_derivs.py
 pyPPG/ppg_bm/get_bm_ppg_sig.py
+pyPPG/ppg_bm/get_bm_sig_ratios.py
+pyPPG/pack_ppg/_ErrorHandler.py
+pyPPG/pack_ppg/__init__.py
+pyPPG/ppg_bm/__init__.py
+pyPPG/ppg_bm/get_biomarkers.py
+pyPPG/ppg_bm/get_bm_derivs_ratios.py
+pyPPG/ppg_bm/get_bm_ppg_derivs.py
+pyPPG/ppg_bm/get_bm_ppg_sig.py
 pyPPG/ppg_bm/get_bm_sig_ratios.py
```

### Comparing `pyPPG-1.0.3/setup.py` & `pyPPG-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup, find_packages
+import io
+
+with io.open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name='pyPPG',
-    version='1.0.3',
+    version='1.0.4',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
-    long_description=0,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
```

