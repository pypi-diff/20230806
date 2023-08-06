# Comparing `tmp/dispCal-0.1.8.tar.gz` & `tmp/dispCal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispCal-0.1.8.tar", last modified: Fri Aug 12 08:02:47 2022, max compression
+gzip compressed data, was "dispCal-0.1.9.tar", last modified: Sat Nov  5 06:38:14 2022, max compression
```

## Comparing `dispCal-0.1.8.tar` & `dispCal-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-08-12 08:02:47.892994 dispCal-0.1.8/
--rw-r--r--   0 jiangyiran   (501) staff       (20)     1074 2022-05-26 09:43:42.000000 dispCal-0.1.8/LICENSE
--rw-r--r--   0 jiangyiran   (501) staff       (20)      482 2022-08-12 08:02:47.892881 dispCal-0.1.8/PKG-INFO
--rw-r--r--   0 jiangyiran   (501) staff       (20)     3011 2022-05-29 03:36:19.000000 dispCal-0.1.8/README.md
-drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-08-12 08:02:47.892115 dispCal-0.1.8/dispCal.egg-info/
--rw-r--r--   0 jiangyiran   (501) staff       (20)      482 2022-08-12 08:02:47.000000 dispCal-0.1.8/dispCal.egg-info/PKG-INFO
--rw-r--r--   0 jiangyiran   (501) staff       (20)      235 2022-08-12 08:02:47.000000 dispCal-0.1.8/dispCal.egg-info/SOURCES.txt
--rw-r--r--   0 jiangyiran   (501) staff       (20)        1 2022-08-12 08:02:47.000000 dispCal-0.1.8/dispCal.egg-info/dependency_links.txt
--rw-r--r--   0 jiangyiran   (501) staff       (20)       15 2022-08-12 08:02:47.000000 dispCal-0.1.8/dispCal.egg-info/top_level.txt
--rw-r--r--   0 jiangyiran   (501) staff       (20)       99 2022-05-26 09:45:00.000000 dispCal-0.1.8/pyproject.toml
--rw-r--r--   0 jiangyiran   (501) staff       (20)       38 2022-08-12 08:02:47.893032 dispCal-0.1.8/setup.cfg
--rw-r--r--   0 jiangyiran   (501) staff       (20)      966 2022-08-12 08:02:41.000000 dispCal-0.1.8/setup.py
-drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-08-12 08:02:47.892733 dispCal-0.1.8/src/
--rw-r--r--   0 jiangyiran   (501) staff       (20)       40 2022-05-26 09:10:46.000000 dispCal-0.1.8/src/__init__.py
--rw-r--r--   0 jiangyiran   (501) staff       (20)    51366 2022-08-12 08:00:58.000000 dispCal-0.1.8/src/cyDisp.pyx
--rw-r--r--   0 jiangyiran   (501) staff       (20)     1762 2022-05-30 02:03:52.000000 dispCal-0.1.8/src/disp.py
--rw-r--r--   0 jiangyiran   (501) staff       (20)    51365 2022-08-12 03:28:04.000000 dispCal-0.1.8/src/dispV2.py
--rw-r--r--   0 jiangyiran   (501) staff       (20)      720 2022-05-26 08:10:52.000000 dispCal-0.1.8/src/setup.py
+drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-11-05 06:38:14.629431 dispCal-0.1.9/
+-rw-r--r--   0 jiangyiran   (501) staff       (20)     1074 2022-05-26 09:43:42.000000 dispCal-0.1.9/LICENSE
+-rw-r--r--   0 jiangyiran   (501) staff       (20)      482 2022-11-05 06:38:14.629224 dispCal-0.1.9/PKG-INFO
+-rw-r--r--   0 jiangyiran   (501) staff       (20)     3011 2022-05-29 03:36:19.000000 dispCal-0.1.9/README.md
+drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-11-05 06:38:14.626656 dispCal-0.1.9/dispCal.egg-info/
+-rw-r--r--   0 jiangyiran   (501) staff       (20)      482 2022-11-05 06:38:14.000000 dispCal-0.1.9/dispCal.egg-info/PKG-INFO
+-rw-r--r--   0 jiangyiran   (501) staff       (20)      235 2022-11-05 06:38:14.000000 dispCal-0.1.9/dispCal.egg-info/SOURCES.txt
+-rw-r--r--   0 jiangyiran   (501) staff       (20)        1 2022-11-05 06:38:14.000000 dispCal-0.1.9/dispCal.egg-info/dependency_links.txt
+-rw-r--r--   0 jiangyiran   (501) staff       (20)       15 2022-11-05 06:38:14.000000 dispCal-0.1.9/dispCal.egg-info/top_level.txt
+-rw-r--r--   0 jiangyiran   (501) staff       (20)       99 2022-05-26 09:45:00.000000 dispCal-0.1.9/pyproject.toml
+-rw-r--r--   0 jiangyiran   (501) staff       (20)       38 2022-11-05 06:38:14.629483 dispCal-0.1.9/setup.cfg
+-rw-r--r--   0 jiangyiran   (501) staff       (20)      966 2022-11-05 06:33:51.000000 dispCal-0.1.9/setup.py
+drwxr-xr-x   0 jiangyiran   (501) staff       (20)        0 2022-11-05 06:38:14.628846 dispCal-0.1.9/src/
+-rw-r--r--   0 jiangyiran   (501) staff       (20)       40 2022-05-26 09:10:46.000000 dispCal-0.1.9/src/__init__.py
+-rw-r--r--   0 jiangyiran   (501) staff       (20)    51370 2022-11-05 06:33:15.000000 dispCal-0.1.9/src/cyDisp.pyx
+-rw-r--r--   0 jiangyiran   (501) staff       (20)     1762 2022-05-30 02:03:52.000000 dispCal-0.1.9/src/disp.py
+-rw-r--r--   0 jiangyiran   (501) staff       (20)    51365 2022-08-12 03:28:04.000000 dispCal-0.1.9/src/dispV2.py
+-rw-r--r--   0 jiangyiran   (501) staff       (20)      720 2022-05-26 08:10:52.000000 dispCal-0.1.9/src/setup.py
```

### Comparing `dispCal-0.1.8/LICENSE` & `dispCal-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dispCal-0.1.8/README.md` & `dispCal-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dispCal-0.1.8/setup.py` & `dispCal-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from distutils.extension import Extension  
 # 必须部分
 from Cython.Distutils import build_ext 
 
 
 setup(
     name='dispCal',
-    version='0.1.8',
+    version='0.1.9',
     description='Calculate Surface Wave Dispersion',
     author='baogege(Jiang Yiran)',
     author_email="baogege@pku.edu.cn",
     url="https://github.com/baogegeJiang/dispCal",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
```

### Comparing `dispCal-0.1.8/src/cyDisp.pyx` & `dispCal-0.1.9/src/dispV2.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,15 +952,15 @@
             tmp = E11
         if E21>tmp:
             tmp = E21
         if E31>tmp:
             tmp = E31
         if E41>tmp:
             tmp = E41
-        if tmp<0.000000000001:
+        if tmp<0.00000000001:
             tmp=1
         E0 = E01/tmp
         E1 = E11/tmp
         E2 = E21/tmp
         E3 = E31/tmp
         E4 = E41/tmp
         #e[:]=ee[:]
```

### Comparing `dispCal-0.1.8/src/disp.py` & `dispCal-0.1.9/src/disp.py`

 * *Files identical despite different names*

### Comparing `dispCal-0.1.8/src/dispV2.py` & `dispCal-0.1.9/src/cyDisp.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if x>0.0:
         return 1
     else:
         return -1
 cdef double del1st
 cdef int jsol
 cdef int index
-cdef double a[500],b[500],d[500],rho[200],X[20],Y[20]
+cdef double a[1000],b[1000],d[1000],rho[1000],X[20],Y[20]
 #cdef double xka,xkb,wvnop,wvnom,rb,ra,t,gammk,gamm1,rho1,e1,e2,xmu,q,y,z,cosq,sinq,fac,e01,e20,xnor,ynor,wvno2,dpth,p,znul,plmn
 #cdef int   i0
 cdef double E0,E1,E2,E3,E4
 cdef double E01,E11,E21,E31,E41
 cdef double ca01,ca02,ca03,ca04,ca00
 cdef double ca11,ca12,ca13,ca14,ca10
 cdef double ca21,ca22,ca23,ca24,ca20
@@ -952,15 +952,15 @@
             tmp = E11
         if E21>tmp:
             tmp = E21
         if E31>tmp:
             tmp = E31
         if E41>tmp:
             tmp = E41
-        if tmp<0.00000000001:
+        if tmp<0.000000000001:
             tmp=1
         E0 = E01/tmp
         E1 = E11/tmp
         E2 = E21/tmp
         E3 = E31/tmp
         E4 = E41/tmp
         #e[:]=ee[:]
```

### Comparing `dispCal-0.1.8/src/setup.py` & `dispCal-0.1.9/src/setup.py`

 * *Files identical despite different names*

