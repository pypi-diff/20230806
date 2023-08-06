# Comparing `tmp/BaselineRemoval-0.1.4.tar.gz` & `tmp/BaselineRemoval-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaselineRemoval-0.1.4.tar", last modified: Fri Feb 17 14:08:30 2023, max compression
+gzip compressed data, was "dist/BaselineRemoval-0.1.5.tar", last modified: Sun Aug  6 13:35:06 2023, max compression
```

## Comparing `BaselineRemoval-0.1.4.tar` & `BaselineRemoval-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-02-17 14:08:30.000000 BaselineRemoval-0.1.4/
--rw-rw-r--   0 azim      (1000) azim      (1000)     4779 2023-02-17 14:08:30.000000 BaselineRemoval-0.1.4/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-02-17 14:08:30.000000 BaselineRemoval-0.1.4/setup.cfg
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-02-17 14:08:30.000000 BaselineRemoval-0.1.4/src/
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-02-17 14:08:30.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/
--rw-r--r--   0 azim      (1000) azim      (1000)     4779 2023-02-17 14:08:29.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)       25 2023-02-17 14:08:29.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/requires.txt
--rw-r--r--   0 azim      (1000) azim      (1000)      274 2023-02-17 14:08:29.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/SOURCES.txt
--rw-r--r--   0 azim      (1000) azim      (1000)       16 2023-02-17 14:08:29.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/top_level.txt
--rw-r--r--   0 azim      (1000) azim      (1000)        1 2023-02-17 14:08:29.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/dependency_links.txt
--rw-r--r--   0 azim      (1000) azim      (1000)     7204 2023-02-17 14:06:32.000000 BaselineRemoval-0.1.4/src/BaselineRemoval.py
--rw-r--r--   0 azim      (1000) azim      (1000)     4302 2023-01-01 17:37:10.000000 BaselineRemoval-0.1.4/README.rst
--rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 BaselineRemoval-0.1.4/LICENSE
--rw-r--r--   0 azim      (1000) azim      (1000)      874 2023-02-17 14:05:42.000000 BaselineRemoval-0.1.4/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/
+-rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 BaselineRemoval-0.1.5/LICENSE
+-rw-rw-r--   0 azim      (1000) azim      (1000)     5556 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)     4322 2023-08-06 13:34:46.000000 BaselineRemoval-0.1.5/README.rst
+-rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/setup.cfg
+-rw-r--r--   0 azim      (1000) azim      (1000)      874 2023-08-06 12:09:18.000000 BaselineRemoval-0.1.5/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.792745 BaselineRemoval-0.1.5/src/
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.792745 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/
+-rw-r--r--   0 azim      (1000) azim      (1000)     5556 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)      274 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/SOURCES.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)        1 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/dependency_links.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       25 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/requires.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       16 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/top_level.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)     7204 2023-02-17 14:06:32.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BaselineRemoval-0.1.4/PKG-INFO` & `BaselineRemoval-0.1.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: BaselineRemoval
-Version: 0.1.4
-Summary: Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum
-Home-page: https://github.com/StatguyUser/BaselineRemoval
-Author: StatguyUser
-License: UNKNOWN
-Download-URL: https://github.com/StatguyUser/BaselineRemoval.git
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 What is it?
 ===========
 
-Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
+Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
 
   - **Modpoly** Modified multi-polynomial fit [1]. It has below 3 parameters.
   
   1) `degree`, it refers to polynomial degree, and default value is 2.
   
   2) `repitition`, it refers to how many iterations to run, and default value is 100.
   
@@ -85,15 +73,15 @@
 Where to get it?
 ================
 
 `pip install BaselineRemoval`
 
 How to cite?
 ============
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
+Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
 
 Dependencies
 ============
 
  - [numpy](https://www.numpy.org/])
 
  - [scikit-learn](https://scikit-learn.org/)
@@ -102,9 +90,7 @@
 
 References
 ============
 
 1. [Automated Method for Subtraction of Fluorescence from Biological Raman Spectra](https://www.researchgate.net/publication/8974238_Automated_Method_for_Subtraction_of_Fluorescence_from_Biological_Raman_Spectra) by Lieber & Mahadevan-Jansen (2003)
 2. [Automated Autofluorescence Background Subtraction Algorithm for Biomedical Raman Spectroscopy](https://www.researchgate.net/publication/5818031_Automated_Autofluorescence_Background_Subtraction_Algorithm_for_Biomedical_Raman_Spectroscopy) by Zhao, Jianhua, Lui, Harvey, McLean, David I., Zeng, Haishan (2007)
 3. [Baseline correction using adaptive iteratively reweighted penalized least squares](https://pubs.rsc.org/is/content/articlelanding/2010/an/b922045c#!divAbstract) by Zhi-Min Zhang, Shan Chena and Yi-Zeng Liang (2010)
-
-
```

### Comparing `BaselineRemoval-0.1.4/src/BaselineRemoval.egg-info/PKG-INFO` & `BaselineRemoval-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,107 @@
 Metadata-Version: 2.1
 Name: BaselineRemoval
-Version: 0.1.4
+Version: 0.1.5
 Summary: Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum
 Home-page: https://github.com/StatguyUser/BaselineRemoval
 Author: StatguyUser
 License: UNKNOWN
 Download-URL: https://github.com/StatguyUser/BaselineRemoval.git
+Description: What is it?
+        ===========
+        
+        Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
+        
+          - **Modpoly** Modified multi-polynomial fit [1]. It has below 3 parameters.
+          
+          1) `degree`, it refers to polynomial degree, and default value is 2.
+          
+          2) `repitition`, it refers to how many iterations to run, and default value is 100.
+          
+          3) `gradient`, it refers to gradient for polynomial loss, default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
+          
+          - **IModPoly** Improved ModPoly[2], which addresses noise issue in ModPoly. It has below 3 parameters.
+          
+          1) `degree`, it refers to polynomial degree, and default value is 2.
+          
+          2) `repitition`, it refers to how many iterations to run, and default value is 100.
+          
+          3) `gradient`, it refers to gradient for polynomial loss, and default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
+          
+          - **ZhangFit** Zhang fit[3], which doesn’t require any user intervention and prior information, such as detected peaks. It has below 3 parameters.
+          
+          1) `lambda_`, it can be adjusted by user. The larger lambda is,  the smoother the resulting background. Default value is 100.
+          
+          2) `porder` refers to adaptive iteratively reweighted penalized least squares for baseline fitting. Default value is 1.
+          
+          3) `repitition` is how many iterations to run, and default value is 15.
+        
+        We can use the python library to process spectral data through either of the techniques ModPoly, IModPoly or Zhang fit algorithm for baseline subtraction. The functions will return baseline-subtracted spectrum.
+        
+        How to use it?
+        =================
+        
+        ```python
+        
+        from BaselineRemoval import BaselineRemoval
+        
+        input_array=[10,20,1.5,5,2,9,99,25,47]
+        
+        polynomial_degree=2 #only needed for Modpoly and IModPoly algorithm
+        
+        baseObj=BaselineRemoval(input_array)
+        
+        Modpoly_output=baseObj.ModPoly(polynomial_degree)
+        
+        Imodpoly_output=baseObj.IModPoly(polynomial_degree)
+        
+        Zhangfit_output=baseObj.ZhangFit()
+        
+        print('Original input:',input_array)
+        
+        print('Modpoly base corrected values:',Modpoly_output)
+        
+        print('IModPoly base corrected values:',Imodpoly_output)
+        
+        print('ZhangFit base corrected values:',Zhangfit_output)
+        
+        Original input: [10, 20, 1.5, 5, 2, 9, 99, 25, 47]
+        
+        Modpoly base corrected values: [-1.98455800e-04  1.61793368e+01  1.08455179e+00  5.21544654e+00
+          7.20210508e-02  2.15427531e+00  8.44622093e+01 -4.17691125e-03
+          8.75511661e+00]
+        
+        IModPoly base corrected values: [-0.84912125 15.13786196 -0.11351367  3.89675187 -1.33134142  0.70220645
+         82.99739548 -1.44577432  7.37269705]
+        
+        ZhangFit base corrected values: [ 8.49924691e+00  1.84994576e+01 -3.31739230e-04  3.49854060e+00
+          4.97412948e-01  7.49628529e+00  9.74951576e+01  2.34940300e+01
+          4.54929023e+01
+        
+        ```
+        Where to get it?
+        ================
+        
+        `pip install BaselineRemoval`
+        
+        How to cite?
+        ============
+        Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
+        
+        Dependencies
+        ============
+        
+         - [numpy](https://www.numpy.org/])
+        
+         - [scikit-learn](https://scikit-learn.org/)
+        
+         - [scipy](https://www.scipy.org/)
+        
+        References
+        ============
+        
+        1. [Automated Method for Subtraction of Fluorescence from Biological Raman Spectra](https://www.researchgate.net/publication/8974238_Automated_Method_for_Subtraction_of_Fluorescence_from_Biological_Raman_Spectra) by Lieber & Mahadevan-Jansen (2003)
+        2. [Automated Autofluorescence Background Subtraction Algorithm for Biomedical Raman Spectroscopy](https://www.researchgate.net/publication/5818031_Automated_Autofluorescence_Background_Subtraction_Algorithm_for_Biomedical_Raman_Spectroscopy) by Zhao, Jianhua, Lui, Harvey, McLean, David I., Zeng, Haishan (2007)
+        3. [Baseline correction using adaptive iteratively reweighted penalized least squares](https://pubs.rsc.org/is/content/articlelanding/2010/an/b922045c#!divAbstract) by Zhi-Min Zhang, Shan Chena and Yi-Zeng Liang (2010)
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-What is it?
-===========
-
-Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
-
-  - **Modpoly** Modified multi-polynomial fit [1]. It has below 3 parameters.
-  
-  1) `degree`, it refers to polynomial degree, and default value is 2.
-  
-  2) `repitition`, it refers to how many iterations to run, and default value is 100.
-  
-  3) `gradient`, it refers to gradient for polynomial loss, default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
-  
-  - **IModPoly** Improved ModPoly[2], which addresses noise issue in ModPoly. It has below 3 parameters.
-  
-  1) `degree`, it refers to polynomial degree, and default value is 2.
-  
-  2) `repitition`, it refers to how many iterations to run, and default value is 100.
-  
-  3) `gradient`, it refers to gradient for polynomial loss, and default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
-  
-  - **ZhangFit** Zhang fit[3], which doesn’t require any user intervention and prior information, such as detected peaks. It has below 3 parameters.
-  
-  1) `lambda_`, it can be adjusted by user. The larger lambda is,  the smoother the resulting background. Default value is 100.
-  
-  2) `porder` refers to adaptive iteratively reweighted penalized least squares for baseline fitting. Default value is 1.
-  
-  3) `repitition` is how many iterations to run, and default value is 15.
-
-We can use the python library to process spectral data through either of the techniques ModPoly, IModPoly or Zhang fit algorithm for baseline subtraction. The functions will return baseline-subtracted spectrum.
-
-How to use it?
-=================
-
-```python
-
-from BaselineRemoval import BaselineRemoval
-
-input_array=[10,20,1.5,5,2,9,99,25,47]
-
-polynomial_degree=2 #only needed for Modpoly and IModPoly algorithm
-
-baseObj=BaselineRemoval(input_array)
-
-Modpoly_output=baseObj.ModPoly(polynomial_degree)
-
-Imodpoly_output=baseObj.IModPoly(polynomial_degree)
-
-Zhangfit_output=baseObj.ZhangFit()
-
-print('Original input:',input_array)
-
-print('Modpoly base corrected values:',Modpoly_output)
-
-print('IModPoly base corrected values:',Imodpoly_output)
-
-print('ZhangFit base corrected values:',Zhangfit_output)
-
-Original input: [10, 20, 1.5, 5, 2, 9, 99, 25, 47]
-
-Modpoly base corrected values: [-1.98455800e-04  1.61793368e+01  1.08455179e+00  5.21544654e+00
-  7.20210508e-02  2.15427531e+00  8.44622093e+01 -4.17691125e-03
-  8.75511661e+00]
-
-IModPoly base corrected values: [-0.84912125 15.13786196 -0.11351367  3.89675187 -1.33134142  0.70220645
- 82.99739548 -1.44577432  7.37269705]
-
-ZhangFit base corrected values: [ 8.49924691e+00  1.84994576e+01 -3.31739230e-04  3.49854060e+00
-  4.97412948e-01  7.49628529e+00  9.74951576e+01  2.34940300e+01
-  4.54929023e+01
-
-```
-Where to get it?
-================
-
-`pip install BaselineRemoval`
-
-How to cite?
-============
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
-
-Dependencies
-============
-
- - [numpy](https://www.numpy.org/])
-
- - [scikit-learn](https://scikit-learn.org/)
-
- - [scipy](https://www.scipy.org/)
-
-References
-============
-
-1. [Automated Method for Subtraction of Fluorescence from Biological Raman Spectra](https://www.researchgate.net/publication/8974238_Automated_Method_for_Subtraction_of_Fluorescence_from_Biological_Raman_Spectra) by Lieber & Mahadevan-Jansen (2003)
-2. [Automated Autofluorescence Background Subtraction Algorithm for Biomedical Raman Spectroscopy](https://www.researchgate.net/publication/5818031_Automated_Autofluorescence_Background_Subtraction_Algorithm_for_Biomedical_Raman_Spectroscopy) by Zhao, Jianhua, Lui, Harvey, McLean, David I., Zeng, Haishan (2007)
-3. [Baseline correction using adaptive iteratively reweighted penalized least squares](https://pubs.rsc.org/is/content/articlelanding/2010/an/b922045c#!divAbstract) by Zhi-Min Zhang, Shan Chena and Yi-Zeng Liang (2010)
-
-
```

### Comparing `BaselineRemoval-0.1.4/src/BaselineRemoval.py` & `BaselineRemoval-0.1.5/src/BaselineRemoval.py`

 * *Files identical despite different names*

### Comparing `BaselineRemoval-0.1.4/README.rst` & `BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,107 @@
-What is it?
-===========
-
-Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
-
-  - **Modpoly** Modified multi-polynomial fit [1]. It has below 3 parameters.
-  
-  1) `degree`, it refers to polynomial degree, and default value is 2.
-  
-  2) `repitition`, it refers to how many iterations to run, and default value is 100.
-  
-  3) `gradient`, it refers to gradient for polynomial loss, default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
-  
-  - **IModPoly** Improved ModPoly[2], which addresses noise issue in ModPoly. It has below 3 parameters.
-  
-  1) `degree`, it refers to polynomial degree, and default value is 2.
-  
-  2) `repitition`, it refers to how many iterations to run, and default value is 100.
-  
-  3) `gradient`, it refers to gradient for polynomial loss, and default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
-  
-  - **ZhangFit** Zhang fit[3], which doesn’t require any user intervention and prior information, such as detected peaks. It has below 3 parameters.
-  
-  1) `lambda_`, it can be adjusted by user. The larger lambda is,  the smoother the resulting background. Default value is 100.
-  
-  2) `porder` refers to adaptive iteratively reweighted penalized least squares for baseline fitting. Default value is 1.
-  
-  3) `repitition` is how many iterations to run, and default value is 15.
-
-We can use the python library to process spectral data through either of the techniques ModPoly, IModPoly or Zhang fit algorithm for baseline subtraction. The functions will return baseline-subtracted spectrum.
-
-How to use it?
-=================
-
-```python
-
-from BaselineRemoval import BaselineRemoval
-
-input_array=[10,20,1.5,5,2,9,99,25,47]
-
-polynomial_degree=2 #only needed for Modpoly and IModPoly algorithm
-
-baseObj=BaselineRemoval(input_array)
-
-Modpoly_output=baseObj.ModPoly(polynomial_degree)
-
-Imodpoly_output=baseObj.IModPoly(polynomial_degree)
-
-Zhangfit_output=baseObj.ZhangFit()
-
-print('Original input:',input_array)
-
-print('Modpoly base corrected values:',Modpoly_output)
-
-print('IModPoly base corrected values:',Imodpoly_output)
-
-print('ZhangFit base corrected values:',Zhangfit_output)
-
-Original input: [10, 20, 1.5, 5, 2, 9, 99, 25, 47]
-
-Modpoly base corrected values: [-1.98455800e-04  1.61793368e+01  1.08455179e+00  5.21544654e+00
-  7.20210508e-02  2.15427531e+00  8.44622093e+01 -4.17691125e-03
-  8.75511661e+00]
-
-IModPoly base corrected values: [-0.84912125 15.13786196 -0.11351367  3.89675187 -1.33134142  0.70220645
- 82.99739548 -1.44577432  7.37269705]
-
-ZhangFit base corrected values: [ 8.49924691e+00  1.84994576e+01 -3.31739230e-04  3.49854060e+00
-  4.97412948e-01  7.49628529e+00  9.74951576e+01  2.34940300e+01
-  4.54929023e+01
-
-```
-Where to get it?
-================
-
-`pip install BaselineRemoval`
-
-How to cite?
-============
-Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models A Second Course for Data Scientists
-
-Dependencies
-============
-
- - [numpy](https://www.numpy.org/])
-
- - [scikit-learn](https://scikit-learn.org/)
-
- - [scipy](https://www.scipy.org/)
-
-References
-============
-
-1. [Automated Method for Subtraction of Fluorescence from Biological Raman Spectra](https://www.researchgate.net/publication/8974238_Automated_Method_for_Subtraction_of_Fluorescence_from_Biological_Raman_Spectra) by Lieber & Mahadevan-Jansen (2003)
-2. [Automated Autofluorescence Background Subtraction Algorithm for Biomedical Raman Spectroscopy](https://www.researchgate.net/publication/5818031_Automated_Autofluorescence_Background_Subtraction_Algorithm_for_Biomedical_Raman_Spectroscopy) by Zhao, Jianhua, Lui, Harvey, McLean, David I., Zeng, Haishan (2007)
-3. [Baseline correction using adaptive iteratively reweighted penalized least squares](https://pubs.rsc.org/is/content/articlelanding/2010/an/b922045c#!divAbstract) by Zhi-Min Zhang, Shan Chena and Yi-Zeng Liang (2010)
+Metadata-Version: 2.1
+Name: BaselineRemoval
+Version: 0.1.5
+Summary: Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum
+Home-page: https://github.com/StatguyUser/BaselineRemoval
+Author: StatguyUser
+License: UNKNOWN
+Download-URL: https://github.com/StatguyUser/BaselineRemoval.git
+Description: What is it?
+        ===========
+        
+        Companion python library for the machine learning book [Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists](https://statguyuser.github.io/feature-engg-selection-for-explainable-models.github.io/index.html). It is used for baseline correction. It has below 3 methods for baseline removal from spectra.
+        
+          - **Modpoly** Modified multi-polynomial fit [1]. It has below 3 parameters.
+          
+          1) `degree`, it refers to polynomial degree, and default value is 2.
+          
+          2) `repitition`, it refers to how many iterations to run, and default value is 100.
+          
+          3) `gradient`, it refers to gradient for polynomial loss, default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
+          
+          - **IModPoly** Improved ModPoly[2], which addresses noise issue in ModPoly. It has below 3 parameters.
+          
+          1) `degree`, it refers to polynomial degree, and default value is 2.
+          
+          2) `repitition`, it refers to how many iterations to run, and default value is 100.
+          
+          3) `gradient`, it refers to gradient for polynomial loss, and default is 0.001. It measures incremental gain over each iteration. If gain in any iteration is less than this, further improvement will stop.
+          
+          - **ZhangFit** Zhang fit[3], which doesn’t require any user intervention and prior information, such as detected peaks. It has below 3 parameters.
+          
+          1) `lambda_`, it can be adjusted by user. The larger lambda is,  the smoother the resulting background. Default value is 100.
+          
+          2) `porder` refers to adaptive iteratively reweighted penalized least squares for baseline fitting. Default value is 1.
+          
+          3) `repitition` is how many iterations to run, and default value is 15.
+        
+        We can use the python library to process spectral data through either of the techniques ModPoly, IModPoly or Zhang fit algorithm for baseline subtraction. The functions will return baseline-subtracted spectrum.
+        
+        How to use it?
+        =================
+        
+        ```python
+        
+        from BaselineRemoval import BaselineRemoval
+        
+        input_array=[10,20,1.5,5,2,9,99,25,47]
+        
+        polynomial_degree=2 #only needed for Modpoly and IModPoly algorithm
+        
+        baseObj=BaselineRemoval(input_array)
+        
+        Modpoly_output=baseObj.ModPoly(polynomial_degree)
+        
+        Imodpoly_output=baseObj.IModPoly(polynomial_degree)
+        
+        Zhangfit_output=baseObj.ZhangFit()
+        
+        print('Original input:',input_array)
+        
+        print('Modpoly base corrected values:',Modpoly_output)
+        
+        print('IModPoly base corrected values:',Imodpoly_output)
+        
+        print('ZhangFit base corrected values:',Zhangfit_output)
+        
+        Original input: [10, 20, 1.5, 5, 2, 9, 99, 25, 47]
+        
+        Modpoly base corrected values: [-1.98455800e-04  1.61793368e+01  1.08455179e+00  5.21544654e+00
+          7.20210508e-02  2.15427531e+00  8.44622093e+01 -4.17691125e-03
+          8.75511661e+00]
+        
+        IModPoly base corrected values: [-0.84912125 15.13786196 -0.11351367  3.89675187 -1.33134142  0.70220645
+         82.99739548 -1.44577432  7.37269705]
+        
+        ZhangFit base corrected values: [ 8.49924691e+00  1.84994576e+01 -3.31739230e-04  3.49854060e+00
+          4.97412948e-01  7.49628529e+00  9.74951576e+01  2.34940300e+01
+          4.54929023e+01
+        
+        ```
+        Where to get it?
+        ================
+        
+        `pip install BaselineRemoval`
+        
+        How to cite?
+        ============
+        Md Azimul Haque (2022). Feature Engineering & Selection for Explainable Models: A Second Course for Data Scientists. Lulu Press, Inc.
+        
+        Dependencies
+        ============
+        
+         - [numpy](https://www.numpy.org/])
+        
+         - [scikit-learn](https://scikit-learn.org/)
+        
+         - [scipy](https://www.scipy.org/)
+        
+        References
+        ============
+        
+        1. [Automated Method for Subtraction of Fluorescence from Biological Raman Spectra](https://www.researchgate.net/publication/8974238_Automated_Method_for_Subtraction_of_Fluorescence_from_Biological_Raman_Spectra) by Lieber & Mahadevan-Jansen (2003)
+        2. [Automated Autofluorescence Background Subtraction Algorithm for Biomedical Raman Spectroscopy](https://www.researchgate.net/publication/5818031_Automated_Autofluorescence_Background_Subtraction_Algorithm_for_Biomedical_Raman_Spectroscopy) by Zhao, Jianhua, Lui, Harvey, McLean, David I., Zeng, Haishan (2007)
+        3. [Baseline correction using adaptive iteratively reweighted penalized least squares](https://pubs.rsc.org/is/content/articlelanding/2010/an/b922045c#!divAbstract) by Zhi-Min Zhang, Shan Chena and Yi-Zeng Liang (2010)
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `BaselineRemoval-0.1.4/LICENSE` & `BaselineRemoval-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BaselineRemoval-0.1.4/setup.py` & `BaselineRemoval-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     with open('README.rst', encoding='utf-8') as f:
         long_description = f.read()
 
 
 setup(
     name='BaselineRemoval',
-    version='0.1.4',
+    version='0.1.5',
     description='Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='StatguyUser',
     url='https://github.com/StatguyUser/BaselineRemoval',
     install_requires=['numpy','scikit-learn','scipy'],
     download_url='https://github.com/StatguyUser/BaselineRemoval.git',
```

