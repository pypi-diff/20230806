# Comparing `tmp/xgrads-0.2.3.tar.gz` & `tmp/xgrads-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgrads-0.2.3.tar", last modified: Sun Apr 23 11:33:43 2023, max compression
+gzip compressed data, was "xgrads-0.2.4.tar", last modified: Sun Aug  6 15:52:05 2023, max compression
```

## Comparing `xgrads-0.2.3.tar` & `xgrads-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:33:43.340118 xgrads-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-23 11:33:29.000000 xgrads-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-23 11:33:43.340118 xgrads-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-23 11:33:29.000000 xgrads-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:33:43.340118 xgrads-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-23 11:33:29.000000 xgrads-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:33:43.336118 xgrads-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-23 11:33:29.000000 xgrads-0.2.3/tests/test_CtlDescriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-23 11:33:29.000000 xgrads-0.2.3/tests/test_openDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-23 11:33:29.000000 xgrads-0.2.3/tests/test_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-23 11:33:29.000000 xgrads-0.2.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:33:43.336118 xgrads-0.2.3/xgrads/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 11:33:29.000000 xgrads-0.2.3/xgrads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36105 2023-04-23 11:33:29.000000 xgrads-0.2.3/xgrads/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18211 2023-04-23 11:33:29.000000 xgrads-0.2.3/xgrads/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-04-23 11:33:29.000000 xgrads-0.2.3/xgrads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:33:43.340118 xgrads-0.2.3/xgrads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-23 11:33:43.000000 xgrads-0.2.3/xgrads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-23 11:33:43.000000 xgrads-0.2.3/xgrads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:33:43.000000 xgrads-0.2.3/xgrads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 11:33:43.000000 xgrads-0.2.3/xgrads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 11:33:43.000000 xgrads-0.2.3/xgrads.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:52:05.230341 xgrads-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 15:51:53.000000 xgrads-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-08-06 15:52:05.230341 xgrads-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-08-06 15:51:53.000000 xgrads-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 15:52:05.230341 xgrads-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-06 15:51:53.000000 xgrads-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:52:05.226341 xgrads-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-08-06 15:51:53.000000 xgrads-0.2.4/tests/test_CtlDescriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-06 15:51:53.000000 xgrads-0.2.4/tests/test_openDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-06 15:51:53.000000 xgrads-0.2.4/tests/test_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-06 15:51:53.000000 xgrads-0.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:52:05.230341 xgrads-0.2.4/xgrads/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-06 15:51:53.000000 xgrads-0.2.4/xgrads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39806 2023-08-06 15:51:53.000000 xgrads-0.2.4/xgrads/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-08-06 15:51:53.000000 xgrads-0.2.4/xgrads/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18794 2023-08-06 15:51:53.000000 xgrads-0.2.4/xgrads/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 15:52:05.230341 xgrads-0.2.4/xgrads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-08-06 15:52:05.000000 xgrads-0.2.4/xgrads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-06 15:52:05.000000 xgrads-0.2.4/xgrads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 15:52:05.000000 xgrads-0.2.4/xgrads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 15:52:05.000000 xgrads-0.2.4/xgrads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 15:52:05.000000 xgrads-0.2.4/xgrads.egg-info/top_level.txt
```

### Comparing `xgrads-0.2.3/PKG-INFO` & `xgrads-0.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,104 @@
-Metadata-Version: 2.1
-Name: xgrads
-Version: 0.2.3
-Summary: Parse and read ctl file commonly used by GrADS.
-Home-page: https://github.com/miniufo/xgrads
-Author: miniufo
-Author-email: miniufo@163.com
-License: MIT
-Keywords: grads opengrads xarray dask
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# xgrads
-
-[![DOI](https://zenodo.org/badge/244529165.svg)](https://zenodo.org/badge/latestdoi/244529165)
-![GitHub](https://img.shields.io/github/license/miniufo/xgrads)
-[![Documentation Status](https://readthedocs.org/projects/xgrads/badge/?version=latest)](https://xgrads.readthedocs.io/en/latest/?badge=latest)
-
-
-![3D plot](https://raw.githubusercontent.com/miniufo/xgrads/master/pics/3D.png)
-
-
-## 1. Introduction
-The Grid Analysis and Display System ([GrADS](http://cola.gmu.edu/grads/) or [OpenGrADS](http://www.opengrads.org/)) is a widely used software for easy access, manipulation, and visualization of earth science data.  It uses a [descriptor (or control) file with a suffix `.ctl`](http://cola.gmu.edu/grads/gadoc/descriptorfile.html) to  describe a raw binary 4D dataset.  The `ctl` file is similar to the header information of a [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html) file, containing all the information about dimensions, attributes, and variables except for the variable data.
-
-This python package [`xgrads`](https://github.com/miniufo/xgrads) is designed for parse and read the `.ctl` file commonly used by [GrADS](http://cola.gmu.edu/grads/).  Right now it can parse various kinds of `.ctl` files.  However, only the commonly used raw binary 4D datasets can be read using [`dask`](https://dask.org/) and return as a [`xarray.Dataset`](http://xarray.pydata.org/en/stable/)  Other types of binary data, like `dtype` is `station` or`grib`, may be supported in the future.
-
----
-## 2. How to install
-**Requirements**
-`xgrads` is developed under the environment with `xarray` (=version 0.15.0), `dask` (=version 2.11.0), `numpy` (=version 1.15.4), `cartopy` (=version 0.17.0), and `pyproj` (=version 1.9.6).  Older versions of these packages are not well tested.
-
-**Install via pip**
-```
-pip install xgrads
-```
-
-**Install from github**
-```
-git clone https://github.com/miniufo/xgrads.git
-cd xgrads
-python setup.py install
-```
-
-
----
-## 3. Examples
-### 3.1 Parse a `.ctl` file
-Parsing a `.ctl` file is pretty simple using the following code:
-```python
-from xgrads import CtlDescriptor
-
-ctl = CtlDescriptor(file='test.ctl')
-
-# print all the info in ctl file
-print(ctl)
-```
-
-If you have already load the ASCII content in the `.ctl` file, you can do it as:
-```python
-content = \
-    "dset ^binary.dat\n" \
-    "* this is a comment line\n" \
-    "title 10-deg resolution model\n" \
-    "undef -9.99e8\n" \
-    "xdef 36 linear   0 10\n" \
-    "ydef 19 linear -90 10\n" \
-    "zdef  1 linear   0  1\n" \
-    "tdef  1 linear 00z01Jan2000 1dy\n" \
-    "vars  1\n" \
-    "test  1 99 test variable\n" \
-    "endvars\n"
-
-ctl = CtlDescriptor(content=content)
-
-# print all the info
-print(ctl)
-```
----
-
-### 3.2 Read binary data into a `xarray.Dataset`
-Reading a `.ctl` related binary data file is also pretty simple using the following code:
-```python
-from xgrads import open_CtlDataset
-
-dset = open_CtlDataset('test.ctl')
-
-# print all the info in ctl file
-print(dset)
-```
-
-Then you have the `dset` as a `xarray.Dataset`.  This is similar to [`xarray.open_dataset`](http://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html) that use [`dask`](https://dask.org/) to chunk (buffer) parts of the whole dataset in physical memory if the whole dataset is too large to fit in.
-
-If there are many `.ctl` files in a folder, we can also open all of them in a single call of `open_mfdataset` as:
-```python
-from xgrads import open_mfDataset
-
-dset = open_mfDataset('./folder/*.ctl')
-
-# print all the info in ctl file
-print(dset)
-```
-assuming that every `.ctl` file has similar data structure except the time step is different.  This is similar to [`xarray.open_mfdataset`](http://xarray.pydata.org/en/v0.12.3/generated/xarray.open_mfdataset.html).
-
----
-
-### 3.3 Convert a GrADS dataset to a NetCDF dataset
-With the above functionality, it is easy to convert a `.ctl` ([GrADS](http://cola.gmu.edu/grads/)) dataset to a `.nc` ([NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html)) dataset:
-```python
-from xgrads import open_CtlDataset
-
-open_CtlDataset('input.ctl').to_netcdf('output.nc')
-```
+# xgrads
+
+[![DOI](https://zenodo.org/badge/244529165.svg)](https://zenodo.org/badge/latestdoi/244529165)
+![GitHub](https://img.shields.io/github/license/miniufo/xgrads)
+[![Documentation Status](https://readthedocs.org/projects/xgrads/badge/?version=latest)](https://xgrads.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/xgrads.svg)](https://badge.fury.io/py/xgrads)
+![Workflow](https://github.com/miniufo/xgrads/actions/workflows/python-publish.yml/badge.svg)
+[![pytest](https://github.com/miniufo/xgrads/actions/workflows/tests.yml/badge.svg)](https://github.com/miniufo/xgrads/actions/workflows/tests.yml)
+[![Build Status](https://app.travis-ci.com/miniufo/xgrads.svg?branch=master)](https://app.travis-ci.com/miniufo/xgrads)
+
+![3D plot](https://raw.githubusercontent.com/miniufo/xgrads/master/pics/3D.png)
+
+
+## 1. Introduction
+The Grid Analysis and Display System ([GrADS](http://cola.gmu.edu/grads/) or [OpenGrADS](http://www.opengrads.org/)) is a widely used software for easy access, manipulation, and visualization of earth science data.  It uses a [descriptor (or control) file with a suffix `.ctl`](http://cola.gmu.edu/grads/gadoc/descriptorfile.html) to  describe a raw binary 4D dataset.  The `ctl` file is similar to the header information of a [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html) file, containing all the information about dimensions, attributes, and variables except for the variable data.
+
+This python package [`xgrads`](https://github.com/miniufo/xgrads) is designed for parse and read the `.ctl` file commonly used by [GrADS](http://cola.gmu.edu/grads/).  Right now it can parse various kinds of `.ctl` files.  However, only the commonly used raw binary 4D datasets can be read using [`dask`](https://dask.org/) and return as a [`xarray.Dataset`](http://xarray.pydata.org/en/stable/)  Other types of binary data, like `dtype` is `station` or`grib`, may be supported in the future.
+
+---
+## 2. How to install
+**Requirements**
+`xgrads` is developed under the environment with `xarray` (=version 0.15.0), `dask` (=version 2.11.0), `numpy` (=version 1.15.4), `cartopy` (=version 0.17.0), and `pyproj` (=version 1.9.6).  Older versions of these packages are not well tested.
+
+**Install via pip**
+```
+pip install xgrads
+```
+
+**Install from github**
+```
+git clone https://github.com/miniufo/xgrads.git
+cd xgrads
+python setup.py install
+```
+
+
+---
+## 3. Examples
+### 3.1 Parse a `.ctl` file
+Parsing a `.ctl` file is pretty simple using the following code:
+```python
+from xgrads import CtlDescriptor
+
+ctl = CtlDescriptor(file='test.ctl')
+
+# print all the info in ctl file
+print(ctl)
+```
+
+If you have already load the ASCII content in the `.ctl` file, you can do it as:
+```python
+content = \
+    "dset ^binary.dat\n" \
+    "* this is a comment line\n" \
+    "title 10-deg resolution model\n" \
+    "undef -9.99e8\n" \
+    "xdef 36 linear   0 10\n" \
+    "ydef 19 linear -90 10\n" \
+    "zdef  1 linear   0  1\n" \
+    "tdef  1 linear 00z01Jan2000 1dy\n" \
+    "vars  1\n" \
+    "test  1 99 test variable\n" \
+    "endvars\n"
+
+ctl = CtlDescriptor(content=content)
+
+# print all the info
+print(ctl)
+```
+---
+
+### 3.2 Read binary data into a `xarray.Dataset`
+Reading a `.ctl` related binary data file is also pretty simple using the following code:
+```python
+from xgrads import open_CtlDataset
+
+dset = open_CtlDataset('test.ctl')
+
+# print all the info in ctl file
+print(dset)
+```
+
+Then you have the `dset` as a `xarray.Dataset`.  This is similar to [`xarray.open_dataset`](http://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html) that use [`dask`](https://dask.org/) to chunk (buffer) parts of the whole dataset in physical memory if the whole dataset is too large to fit in.
+
+If there are many `.ctl` files in a folder, we can also open all of them in a single call of `open_mfdataset` as:
+```python
+from xgrads import open_mfDataset
+
+dset = open_mfDataset('./folder/*.ctl')
+
+# print all the info in ctl file
+print(dset)
+```
+assuming that every `.ctl` file has similar data structure except the time step is different.  This is similar to [`xarray.open_mfdataset`](http://xarray.pydata.org/en/v0.12.3/generated/xarray.open_mfdataset.html).
+
+---
+
+### 3.3 Convert a GrADS dataset to a NetCDF dataset
+With the above functionality, it is easy to convert a `.ctl` ([GrADS](http://cola.gmu.edu/grads/)) dataset to a `.nc` ([NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html)) dataset:
+```python
+from xgrads import open_CtlDataset
+
+open_CtlDataset('input.ctl').to_netcdf('output.nc')
+```
```

### Comparing `xgrads-0.2.3/xgrads/core.py` & `xgrads-0.2.4/xgrads/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1051 +1,1130 @@
-# -*- coding: utf-8 -*-
-"""
-Created on 2020.03.02
-
-@author: MiniUFO
-Copyright 2018. All rights reserved. Use is subject to license terms.
-"""
-import os, sys, re
-import numpy as np
-from datetime import datetime
-from numpy import datetime64, timedelta64
-
-
-"""
-Core classes are defined below
-"""
-class CtlDescriptor(object):
-    """A class for a ctl file
-    
-    This class represents a descriptor file like the .ctl file for GrADS.
-    It generally includes a multi-dimensional dataset on the Earth.
-    
-    Attributes
-    ----------
-        dsetPath: str
-            dataset file
-        descPath: str
-            descriptor file
-        indxPath: str
-            index file (for GRIB file)
-        stnmPath: str
-            station map file (for station file)
-        
-        pdef: PDEF
-            projection-definition
-        tdef: Coordinate
-            time coordinate definition
-        zdef: Coordinate
-            z-coordinate definition
-        ydef: Coordinate
-            y-coordinate definition
-        xdef: Coordinate
-            x-coordinate definition
-        vdef: list of CtlVar
-            variables definition
-        
-        comments: list of str
-            list of global string comments
-        
-        zrev: bool
-            z-dimension reverse (i.e., from north to south)
-        yrev: bool
-            y-dimension reverse (i.e., from upper to lower levels)
-        
-        hasData: bool
-            whether the corresponding binary data file exist
-        vcount: int
-            variable count
-        
-        dtype: numpy.dtype
-            data type
-        periodicX: bool
-            whether xdef is periodic
-        
-        cal365Days: bool
-            whether the calendar is always 365 days (no leap year)
-        template: bool
-            whether it is a template for multiple binary files
-        sequential: bool
-            whether it is a sequential file (Fortran style)
-        byteOrder: str
-            byte order, ['little', 'big'] for little-endian or big-endian
-        storage: str
-            storage type, '99' or '-1,20' or others
-        
-        totalZCount: int
-            total number of horizontal slice
-        zRecLength: int
-            record length of a single horizontal slice
-        tRecLength: int
-            record length of a single time (including all variables)
-    """
-    def __init__(self, encoding='GBK', **kwargs):
-        """Constructor
-
-        One of the keyword argument `file` or `content` should be specified.
-        
-        Parameters
-        ----------
-        encoding: {'GBK', 'UTF-8'}, optional
-            Encoding for the ctl file contents.
-        file: str
-            The ctl path/file name.
-        content: str
-            A string representation for the ctl file contents.
-
-        Returns
-        -------
-        CtlDescriptor
-            An object represents the ctl file
-        """
-        self.vcount = 0
-        
-        self.pdef = None
-        self.tdef = None
-        self.zdef = None
-        self.ydef = None
-        self.xdef = None
-        self.vdef = None
-        self.comments = {}
-        
-        self.dsetPath = ''
-        self.descPath = ''
-        self.indxPath = ''
-        self.stnmPath = ''
-        self.storage  = ''
-        self.dtype    = ''
-        self.title    = ''
-        self.incre    = ''
-        
-        self.zrev     = False
-        self.yrev     = False
-        self.hasData  = False
-        
-        self.periodicX   = False
-        self.cal365Days  = False
-        self.template    = False
-        self.sequential  = False
-        
-        self.totalZCount = 0
-        self.zRecLength  = 0
-        self.tRecLength  = 0
-        self.byteOrder   = sys.byteorder
-        
-        if kwargs.get('file'):
-            abspath = kwargs['file']
-            
-            if not '/' in abspath: # thanks to Baofeng Jiao from IAP
-                abspath = './' + abspath
-            
-            if os.path.getsize(abspath) / (1024.0*1024.0) > 2:
-                raise Exception('ctl file is too large (> 2 MB)')
-            
-            with open(abspath, 'r', encoding=encoding) as f:
-                fileContent = f.readlines()
-        
-        elif kwargs.get('content'):
-            abspath = None
-            fileContent = kwargs['content'].splitlines()
-        else:
-            raise Exception('invalid key word '+
-                            '(file='' or content='' is allowed)')
-        
-        for i, line in enumerate(fileContent):
-            llower = line.lower()
-            if (llower.startswith('dset') or
-                llower.startswith('index') or
-                llower.startswith('stnmap')
-               ) and abspath is not None and '^' in line:
-                dirname = os.path.dirname(abspath)
-                if dirname[-1] != '/':
-                    fileContent[i] = line.replace('^',
-                                       os.path.dirname(abspath) + '/')
-                else:
-                    fileContent[i] = line.replace('^',
-                                       os.path.dirname(abspath))
-        
-        self.descPath=abspath
-        self.parse(fileContent)
-    
-    def parse(self, fileContent):
-        """Parse file content as a multi-line str"""
-        dpath_str = None
-        
-        for oneline in fileContent:
-            if   oneline.lower().startswith('dset'):
-                dpath_str = oneline.split()[1]
-            elif oneline.lower().startswith('index'):
-                self._processIndex(oneline)
-            elif oneline.lower().startswith('stnmap'):
-                self._processStnmap(oneline)
-            elif oneline.lower().startswith('dtype'):
-                self.dtype = oneline[5:].strip()
-            elif oneline.lower().startswith('pdef'):
-                self._processPDEF(oneline)
-            elif oneline.lower().startswith('title'):
-                self.title = oneline.split()[1].strip()
-            elif oneline.lower().startswith('undef'):
-                self.undef = float(oneline.split()[1].strip())
-            elif oneline.lower().startswith('options'):
-                self._processOptions(oneline)
-            elif oneline.lower().startswith('byteswapped'):
-                self.byteOrder  = 'big' \
-                    if sys.byteorder == 'little' else 'little'
-            elif oneline.lower().startswith('xdef'):
-                self._processXDef(oneline, fileContent)
-            elif oneline.lower().startswith('ydef'):
-                self._processYDef(oneline,fileContent)
-            elif oneline.lower().startswith('zdef'):
-                self._processZDef(oneline, fileContent)
-            elif oneline.lower().startswith('tdef'):
-                self._processTDef(oneline)
-            elif oneline.lower().startswith('vars'):
-                self._processVars(oneline, fileContent)
-            elif oneline.lower().startswith('@ global string comment'):
-                self._processGlobalComments(oneline)
-            elif oneline.startswith('*') or oneline.strip() == '':
-                continue
-        
-        if dpath_str == None:
-            raise Exception('no valid dset is parsed')
-        
-        if self.template:
-            self._processDSets(dpath_str)
-        else:
-            self._processDSet(dpath_str)
-        
-        if self.yrev:
-            self.ydef.samples = np.flip(self.ydef.samples)
-        
-        if self.zrev:
-            self.zdef = np.flip(self.zdef)
-    
-    def _processDSets(self, dpath_str):
-        strPos = dpath_str.find('%')
-        
-        if strPos == -1:
-            raise Exception('template is used in ctl but no % in dset')
-        
-        endPos = len(dpath_str) - dpath_str[::-1].find('.') - 1
-        # endPos = len(dpath_str) if endPos == -1 else endPos
-        
-        template = dpath_str[strPos:endPos]
-        
-        tokens = [self._get_template_format('%'+token)
-                  for token in filter(lambda x: x != '', template.split('%'))]
-        # tokens = []
-        # for token in filter(lambda x: x != '', template.split('%')):
-        #     tokens.append(self._get_template_format('%' + token))
-        fmt = ''.join(tokens)
-        
-        fileList = []
-        
-        times = self.tdef.samples
-        base  = self._get_field(times[0])
-        for l in range(len(times)):
-            part = times[l].item().strftime(fmt)
-            
-            fname = dpath_str[:strPos] + part + dpath_str[endPos:]
-            fname = self._replace_forecast_template(fname, l, base)
-            
-            # remove duplicated file
-            if fname not in fileList:
-                fileList.append(fname)
-        
-        self.dsetPath = np.array(fileList)
-        
-        has = True
-        for file in fileList:
-            if not os.path.exists(file):
-                has = False
-                break
-
-        self.hasData = has
-        
-    def _processDSet(self, dpath_str):
-        self.dsetPath = dpath_str
-        self.hasData  = os.path.exists(self.dsetPath)
-    
-    def _processIndex(self, oneline):
-        self.indxPath = oneline.split()[1]
-    
-    def _processStnmap(self, oneline):
-        self.stnmPath = oneline.split()[1]
-    
-    def _processPDEF(self, oneline):
-        self.pdef = PDEF(oneline)
-    
-    def _processOptions(self, oneline):
-        lineLower = oneline.lower()
-        
-        if 'yrev'             in lineLower: self.yrev       = True
-        if 'zrev'             in lineLower: self.zrev       = True
-        if 'template'         in lineLower: self.template   = True
-        if 'sequential'       in lineLower: self.sequential = True
-        if '365_day_calendar' in lineLower: self.cal365Days = True
-        if 'big_endian'       in lineLower: self.byteOrder  = 'big'
-        if 'byteswapped'      in lineLower: self.byteOrder  = \
-            'big' if sys.byteorder == 'little' else 'little'
-    
-    def _processXDef(self, oneline, fileContent):
-        tokens = oneline.lower().split()
-        xnum   = int(tokens[1])
-        
-        if   tokens[2] == 'linear': xlnr = True
-        elif tokens[2] == 'levels': xlnr = False
-        else: raise Exception('invalid type for xdef (linear or levels): ' +
-                              tokens[2])
-
-        if xlnr:
-            start, intv = float(tokens[3]), float(tokens[4])
-            self.xdef = Coordinate('xdef', np.linspace(start,
-                                                       start + intv * (xnum-1),
-                                                       xnum, dtype=np.float32))
-        else:
-            values = [float(i) for i in tokens[3:]]
-            count  = len(values)
-            index  = fileContent.index(oneline) + 1
-            
-            while count < xnum:
-                split = fileContent[index].split()
-                values += [float(v) for v in split]
-                count  += len(split)
-                index  += 1
-            
-            if count != xnum:
-                raise Exception('not parse xdef correctly')
-            
-            self.xdef = Coordinate('xdef', np.array(values))
-
-        self.periodicX = self.xdef.isPeriodic(360)
-
-    def _processYDef(self, oneline, fileContent):
-        tokens = oneline.lower().split()
-        ynum   = int(tokens[1])
-        
-        if   tokens[2] == 'linear': ylnr = True
-        elif tokens[2] == 'levels': ylnr = False
-        else: raise Exception('invalid type for ydef (linear or levels): ' +
-                              tokens[2])
-        
-        if ylnr:
-            start, intv = float(tokens[3]), float(tokens[4])
-            self.ydef = Coordinate('ydef', np.linspace(start,
-                                                       start + intv * (ynum-1),
-                                                       ynum, dtype=np.float32))
-        else:
-            values = [float(i) for i in tokens[3:]]
-            count  = len(values)
-            index  = fileContent.index(oneline) + 1
-            
-            while count < ynum:
-                split = fileContent[index].split()
-                values += [float(v) for v in split]
-                count  += len(split)
-                index  += 1
-            
-            if count != ynum:
-                raise Exception(('not parse ydef correctly, count={0} '+
-                                 'while ynum={1}').format(count, ynum))
-            
-            self.ydef = Coordinate('ydef', np.array(values))
-    
-    def _processZDef(self, oneline, fileContent):
-        tokens = oneline.lower().split()
-        znum   = int(tokens[1])
-        
-        if   tokens[2] == 'linear': zlnr = True
-        elif tokens[2] == 'levels': zlnr = False
-        else: raise Exception('invalid type for zdef (linear or levels): ' +
-                              tokens[2])
-        
-        if zlnr:
-            start, intv = float(tokens[3]), float(tokens[4])
-            self.zdef = Coordinate('zdef', np.linspace(start,
-                                                       start + intv * (znum-1),
-                                                       znum, dtype=np.float32))
-            
-        else:
-            values = [float(i) for i in tokens[3:]]
-            count  = len(values)
-            index  = fileContent.index(oneline) + 1
-            
-            while count < znum:
-                split = fileContent[index].split()
-                values += [float(v) for v in split]
-                count  += len(split)
-                index  += 1
-            
-            if count != znum:
-                raise Exception('not parse zdef correctly')
-            
-            self.zdef = Coordinate('zdef', np.array(values))
-
-    def _processTDef(self, oneline):
-        tokens = oneline.lower().split()
-        tnum   = int(tokens[1])
-
-        if tokens[2]!='linear':
-            raise Exception('nonlinear tdef is not supported')
-
-        times = self._times_to_array(tokens[3], tokens[4], tnum)
-        
-        self.incre = GrADS_increment_to_timedelta64(tokens[4])
-        self.tdef  = Coordinate('tdef', times)
-    
-    def _processVars(self, oneline, fileContent):
-        if (self.dtype != 'station' and 
-            not all([self.tdef, self.zdef, self.ydef, self.xdef])):
-            raise Exception('vdef should be after x, y, z and t definitions')
-        
-        t = self.tdef.length()
-        
-        if self.dtype != 'station':
-            y = self.ydef.length() if self.pdef is None else self.pdef.jsize
-            x = self.xdef.length() if self.pdef is None else self.pdef.isize
-        
-            self.zRecLength = x * y * 4
-            
-            # add two bytes at the beginning and the end
-            if self.sequential:
-                self.zRecLength += 8
-        
-        tokens = oneline.split()
-        vnum   = int(tokens[1])
-        start  = fileContent.index(oneline) + 1
-        
-        if vnum < 1:
-            raise Exception('there should be at least one CtlVar')
-        
-        self.vcount = vnum
-        self.vdef   = [None] * vnum
-        
-        v = CtlVar(fileContent[start])
-        v.index =0
-        v.strPos=0
-        v.tcount=t
-        
-        if self.dtype != 'station':
-            v.ycount=y
-            v.xcount=x
-        
-        self.totalZCount += v.zcount
-        self.storage      = v.storage
-        self.vdef[0]      = v
-        
-        type1 = type2 = type3 = False
-        
-        for i in range(1, vnum):
-            v  = CtlVar(fileContent[start+i])
-            vs = self.vdef[i-1]
-            
-            v.index  = i
-            v.undef  = self.undef
-            v.tcount = t
-            
-            if self.dtype != 'station':
-                v.ycount = y
-                v.xcount = x
-            
-            # if v.storage in ['99', '0']:
-            if v.storage in ['99', '0', '00', '000', '1', '11', '111']:
-                v.strPos = vs.zcount * self.zRecLength + vs.strPos
-                type1 = True
-            elif v.storage == '-1,20':
-                v.strPos = vs.zcount * self.zRecLength * t + vs.strPos
-                type2 = True
-            else:
-                type3 = True
-            
-            if not type3 and type1 == type2:
-                raise Exception('storage type should be the same')
-            
-            self.totalZCount += v.zcount
-            self.vdef[i] = v
-        
-        self.tRecLength = self.zRecLength * self.totalZCount
-        
-        if fileContent[start + vnum].strip().lower() != 'endvars':
-            raise Exception('endvars is expected')
-    
-    def _processGlobalComments(self, oneline):
-        cnt = oneline[24:].strip().split('=')
-        
-        self.comments[cnt[0].strip()] = cnt[1].strip()
-
-    def _get_template_format(self, part):
-        """Get time format string
-        
-        See the following URL for reference:
-        http://cola.gmu.edu/grads/gadoc/templates.html
-        
-        %x1   1 digit decade
-        %x3   3 digit decade
-        %y2   2 digit year
-        %y4   4 digit year
-        %m1   1 or 2 digit month
-        %m2   2 digit month (leading zero if needed)
-        %mc   3 character month abbreviation
-        %d1   1 or 2 digit day
-        %d2   2 digit day (leading zero if needed)
-        %h1   1 or 2 digit hour
-        %h2   2 digit hour
-        %h3   3 digit hour (e.g., 120 or 012)
-        %n2   2 digit minute; leading zero if needed
-        %f2   2 digit forecast hour; leading zero if needed; more digits added
-              for hours >99; hour values increase indefinitely
-        %f3   3 digit forecast hour; leading zeros if needed; more digits added
-              for hours >999; hour values increase indefinitely
-        %fn2  2 digit forecast minute; leading zero if needed; more digits added
-              for minutes > 99; minute values increase indefinitely (2.0.a9+)
-        %fhn  forecast time expressed in hours and minutes (hhnn) where minute
-              value (nn) is always <=59 and hour value (hh) increases indefinitely.
-              If hh or nn are <=9, they are padded with a 0, so they are always at
-              least 2 digits; more digits added for hours >99. (2.0.a9+)
-        %fdhn forecast time expressed in days, hours, and minutes (ddhhnn) where
-              minute value (nn) is always <=59, hour value (hh) is always <=23 and
-              day value (dd) increases indefinitely. If dd, hh, or nn are <=9, they
-              are padded with a 0 so they are always at least 2 digits; more digits
-              added for days >99. (2.0.a9+)
-        %j3   3 digit julian day (day of year) (2.0.a7+)
-        %t1   1 or 2 digit time index (file names contain number sequences that
-              begin with 1 or 01) (2.0.a7+)
-        %t2   2 digit time index (file names contain number sequences that begin
-              with 01) (2.0.a7+)
-        %t3   3 digit time index (file names contain number sequences that begin
-              with 001) (2.0.a7+)
-        %t4   4 digit time index (file names contain number sequences that begin
-              with 0001) (2.0.a8+)
-        %t5   5 digit time index (file names contain number sequences that begin
-              with 00001) (2.0.a8+)
-        %t6   6 digit time index (file names contain number sequences that begin
-              with 000001) (2.0.a8+)
-        %tm1  1 or 2 digit time index (file names contain number sequences that
-              begin with 0 or 00) (2.0.a7+)
-        %tm2  2 digit time index (file names contain number sequences that begin
-              with 00) (2.0.a7+)
-        %tm3  3 digit time index (file names contain number sequences that begin
-              with 000) (2.0.a7+)
-        %tm4  4 digit time index (file names contain number sequences that begin
-              with 0000) (2.0.a8+)
-        %tm5  5 digit time index (file names contain number sequences that begin
-              with 00000) (2.0.a8+)
-        %tm6  6 digit time index (file names contain number sequences that begin
-              with 000000) (2.0.a8+)
-    
-        Parameters
-        ----------
-        part : str
-            A string in the above format started with %.
-    
-        Returns
-        -------
-        str
-            The format in python datetime
-        """
-        if   part == '%y2':
-            return '%y'
-        elif part == '%y4':
-            return '%Y'
-        elif part == '%m1':
-            return '%m'
-        elif part == '%m2':
-            return '%m'
-        elif part == '%mc':
-            return '%b'
-        elif part == '%d1':
-            return '%d'
-        elif part == '%d2':
-            return '%d'
-        elif part == '%h1':
-            return '%H'
-        elif part == '%h2':
-            return '%H'
-        elif part == '%n2':
-            return '%M'
-        elif part in ['%f3', '%f2', '%fn2', '%fhn', '%fdhn']:
-            # this is not supported by strftime()
-            return '_miniufo_' + part[1:]
-        else:
-            raise Exception('unsupported format: ' + part)
-    
-    def _replace_forecast_template(self, fname, l, base):
-        """Replace forecast str %f as a template in dset
-    
-        Parameters
-        ----------
-        fname: str
-            A given string of binary file.
-        l: int
-            Index of file in a template.
-        base: numpy.datetime64
-            Base time.
-    
-        Returns
-        -------
-        str
-            A string after replacing the %f template.
-        """
-        amount = l * self.incre
-        
-        days = base[..., 2]
-        hour = base[..., 3]
-        mins = base[..., 4]
-        
-        if fname.find('_miniufo_f3') != -1:
-            dt = (amount.astype("timedelta64[h]") + hour).astype(int)
-            fname = fname.replace('_miniufo_f3', '{0:03d}'.format(dt))
-        
-        if fname.find('_miniufo_f2') != -1:
-            dt = (amount.astype("timedelta64[h]") + hour).astype(int)
-            fname = fname.replace('_miniufo_f2', '{0:02d}'.format(dt))
-        
-        if fname.find('_miniufo_fn2') != -1:
-            dt = (amount.astype("timedelta64[m]") + mins).astype(int)
-            fname = fname.replace('_miniufo_fn2', '{0:02d}'.format(dt))
-        
-        if fname.find('_miniufo_fhn') != -1:
-            dt_h = (amount.astype("timedelta64[h]") + hour).astype(int)
-            dt_m = (amount.astype("timedelta64[m]") + mins).astype(int) % 60
-            fname = fname.replace('_miniufo_fhn',
-                                  '{0:02d}'.format(dt_h)+'{0:02d}'.format(dt_m))
-        
-        if fname.find('_miniufo_fdhn') != -1:
-            dt_d = (amount.astype("timedelta64[D]") + days).astype(int)
-            dt_h = (amount.astype("timedelta64[h]") + hour).astype(int) % 24
-            dt_m = (amount.astype("timedelta64[m]") + mins).astype(int) % 60
-            fname = fname.replace('_miniufo_fdhn',
-                                  '{0:02d}'.format(dt_d)+
-                                  '{0:02d}'.format(dt_h)+
-                                  '{0:02d}'.format(dt_m))
-        
-        return fname
-
-    def _get_field(self, datetime64):
-        """Get fields of a datetime64
-        
-        Convert array of datetime64 to a calendar array of
-        [year, month, day, hour, minute, seconds, microsecond]
-        with these quantites indexed on the last axis.
-    
-        Parameters
-        ----------
-        datetime64: datetime64 array (...)
-            numpy.ndarray of datetimes of arbitrary shape
-    
-        Returns
-        -------
-        cal: uint32 array (..., 7)
-            calendar array with last axis representing year, month, day, hour,
-            minute, second, microsecond
-        """
-        # allocate output 
-        out = np.empty(datetime64.shape + (7,), dtype="u4")
-        
-        # decompose calendar floors
-        Y, M, D, h, m, s = [datetime64.astype(f'M8[{x}]') for x in 'YMDhms']
-        
-        out[..., 0] = Y + 1970 # Gregorian Year
-        out[..., 1] = (M - Y) + 1 # month
-        out[..., 2] = (D - M) + 1 # dat
-        out[..., 3] = (datetime64 - D).astype('m8[h]' ) # hour
-        out[..., 4] = (datetime64 - h).astype('m8[m]' ) # minute
-        out[..., 5] = (datetime64 - m).astype('m8[s]' ) # second
-        out[..., 6] = (datetime64 - s).astype('m8[us]') # microsecond
-        
-        return out
-
-
-    def _times_to_array(self, strTime, incre, tnum):
-        """Change format of time
-        
-        Convert GrADS time string of strart time and increment
-        to an array of numpy.datetime64.
-        
-        Parameters
-        ----------
-        strTime : str
-            Grads start time e.g., 00:00z01Jan2000.
-        incre : str
-            Grads time increment in str format e.g., 1dy.
-        tnum : int
-            Grads time increment in str format e.g., 1dy.
-        
-        Returns
-        -------
-        numpy array of datetime64
-            Times in datetime64 format
-        """
-        if 'mo' in incre:
-            start = GrADStime_to_datetime(strTime)
-            
-            lst = []
-            for l in range(tnum):
-                y, m = start.year, start.month
-                y, m = y+int((m+l-1)/12), int((m+l-1)%12)+1
-                lst.append(start.replace(year=y, month=m))
-            
-            return np.asarray(lst, dtype='datetime64[s]')
-            
-        elif 'yr' in incre:
-            start = GrADStime_to_datetime(strTime)
-            
-            lst = []
-            for l in range(tnum):
-                y = start.year + l
-                lst.append(start.replace(year=y))
-            
-            return np.asarray(lst, dtype='datetime64[s]')
-        
-        else:
-            start = GrADStime_to_datetime64(strTime)
-            intv  = GrADS_increment_to_timedelta64(incre)
-
-            if self.cal365Days:
-
-                lst = []
-                while len(lst) < tnum:
-                    isfeb29 = (start.item().day == 29) and (start.item().month == 2)
-                    if not isfeb29:
-                        lst.append(start)
-                    start += intv
-
-                return np.asarray(lst)
-
-            else:
-
-                return np.arange(start, start + intv * tnum, intv)
-
-    def __repr__(self):
-        """Print this class as a string"""
-        vdef = np.array(self.vdef)
-        pdef = self.pdef.proj if self.pdef is not None else ''
-        
-        return \
-            '   dsetPath: ' + str(self.dsetPath)  + '\n'\
-            '   descPath: ' + str(self.descPath)  + '\n'\
-            '   indxPath: ' + str(self.indxPath)  + '\n'\
-            '   stnmPath: ' + str(self.stnmPath)  + '\n'\
-            '      title: ' + str(self.title)     + '\n'\
-            '      undef: ' + str(self.undef)     + '\n'\
-            '       zrev: ' + str(self.zrev)      + '\n'\
-            '       yrev: ' + str(self.yrev)      + '\n'\
-            '      dtype: ' + str(self.dtype)     + '\n'\
-            '   template: ' + str(self.template)  + '\n'\
-            '  periodicX: ' + str(self.periodicX) + '\n'\
-            ' cal365Days: ' + str(self.cal365Days)+ '\n'\
-            ' sequential: ' + str(self.sequential)+ '\n'\
-            '  byteOrder: ' + str(self.byteOrder) + '\n'\
-            '       xdef: ' + str(self.xdef)      + '\n'\
-            '       ydef: ' + str(self.ydef)      + '\n'\
-            '       zdef: ' + str(self.zdef)      + '\n'\
-            '       tdef: ' + str(self.tdef)      + '\n'\
-            '       pdef: ' + str(pdef)           + '\n'\
-            '       vdef: ' + str(vdef)
-
-
-
-class PDEF(object):
-    """PDEF class
-    
-    Parse necessary info in PDEF.
-    
-    Reference: http://cola.gmu.edu/grads/gadoc/pdef.html
-    
-    Attributes
-    ----------
-        isize: int
-            size of native grid in x direction
-        jsize: int
-            size of native grid in y direction
-        proj: str
-            type of projection
-        lonref: str
-            reference longitude
-    """
-    def __init__(self, oneline):
-        """Constructor
-        
-        Parameters
-        ----------
-        oneline: str
-            The ASCII line of PDEF in ctl file.
-        """
-        lineLower = oneline.lower()
-        
-        if 'nps' in lineLower or 'sps' in lineLower:
-            token = lineLower.split()
-            
-            if len(token) != 8:
-                raise Exception('not enough tokens for PDEF, ' +
-                                'expected 8 but found ' + str(len(token)))
-            
-            self.isize   = int  (token[1]) # size of native grid in x direction
-            self.jsize   = int  (token[2]) # size of native grid in y direction
-            self.proj    =      (token[3]) # type of projection
-            self.ipole   = int  (token[4]) # i-coord of pole ref to ll corner
-            self.jpole   = int  (token[5]) # j-coord of pole ref to ll corner
-            self.lonref  = float(token[6]) # reference longitude
-            self.gridinc = float(token[7]) # distance between gripoints in km
-            
-        elif 'lccr' in lineLower or 'lcc' in lineLower:
-            token = lineLower.split()
-            
-            if len(token) != 13:
-                raise Exception('not enough tokens for PDEF, ' +
-                                'expected 13 but found ' + str(len(token)))
-            
-            self.isize   = int  (token[1]) # size of native grid in x direction
-            self.jsize   = int  (token[2]) # size of native grid in y direction
-            self.proj    =      (token[3]) # type of projection
-            self.latref  = float(token[4]) # ref latitude
-            self.lonref  = float(token[5]) # ref longitude (E>0, W<0)
-            self.iref    = float(token[6]) # i of ref point
-            self.jref    = float(token[7]) # j of ref point
-            self.Struelat= float(token[8]) # S true lat
-            self.Ntruelat= float(token[9]) # N true lat
-            self.slon    = float(token[10]) # standard longitude
-            self.dx      = float(token[11]) # grid X increment in meters
-            self.dy      = float(token[12]) # grid Y increment in meters
-        
-        else:
-            raise Exception('not currently supported PDEF\n' + oneline)
-
-    def __repr__(self):
-        """Print this class as a string"""
-        return '\n'.join(['%s: %s' % item for item in self.__dict__.items()])
-    
-
-
-class Coordinate(object):
-    """Discrete sampled coordinate
-    
-    This is a simple wrapper for np.array for a coordinate.
-    
-    Attributes
-    ----------
-        isLinear: bool
-            Steps are even or uneven
-        isIncre: int
-            Is increasing or decreasing
-        name: str
-            The name of the coordinate
-        samples: str
-            Discretized coordinate samples
-        delSamples: str
-            Finite difference between samples
-    """
-    def __init__(self, name, samples):
-        """Constructor
-        
-        Parameters
-        ----------
-        name : str
-            The name of the coordinate.
-        samples : np.array
-            1D array for the discrete coordinate.
-        """
-        self.isLinear   = True
-        self.isIncre    = True
-        self.name       = name
-        self.samples    = samples
-        self.delSamples = None
-        
-        self.max = np.max(self.samples)
-        self.min = np.min(self.samples)
-        
-        if len(samples) > 1:
-            self.delSamples = np.diff(self.samples)
-            
-            if self.samples[-1] < self.samples[0]:
-                self.isIncre=False
-        else:
-            self.delSamples = np.array([1])
-    
-    def length(self):
-        return len(self.samples)
-    
-    def isPeriodic(self,period):
-        # not physically but generally true
-        if not self.isLinear: return False
-        
-        delta = self.delSamples[0]
-        start = self.samples[-1] + delta - period
-        
-        if(abs((start - self.samples[0]) / delta > 1e-4)):
-            return False
-        
-        return True
-    
-    def __str__(self):
-        """Print this class as a string"""
-        return str(self.samples)
-
-
-
-class CtlVar(object):
-    """A simple variable class used in .ctl file
-    
-    Attributes
-    ----------
-        tcount: int
-            T grid points
-        zcount: int
-            Z grid points
-        ycount: int
-            Y grid points
-        xcount: int
-            X grid points
-        undef: float
-            Undefined values
-        dependZ: bool
-            Whether the var depends on z
-        unit: str
-            Unit of the variable
-        name: str
-            Name of the variable
-        comment: str
-            A short comment
-        index: str
-            Index of this variable
-        strPos: str
-            Start position (in bytes) of this variable in the binary file
-    """
-    __reBlank = re.compile(r'[\s\t]+')
-    __reUnits = re.compile(r'\([^\(\)]+?\)')
-    
-    
-    def __init__(self, oneLineStr):
-        self.tcount = 0
-        self.zcount = 0
-        self.ycount = 0
-        self.xcount = 0
-        self.undef  = np.nan
-        self.dependZ= True # whether the var depends on z
-        
-        self.unit   = ''
-        self.name   = ''
-        self.comment= ''
-        
-        self.index  = 0
-        self.strPos = 0
-        
-        if len(CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3))== 3:
-            self.name, self.zcount, self.storage = \
-                CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3)
-            self.comment = self.name
-        else:
-            self.name, self.zcount, self.storage, self.comment = \
-                CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3)
-        
-        self.zcount = int(self.zcount)
-        
-        findMatch = CtlVar.__reUnits.findall(self.comment)
-        
-        if findMatch:
-            self.unit    = findMatch[-1]
-            self.comment = self.comment[:self.comment.index(self.unit)].strip()
-        else:
-            self.unit = ''
-
-        if self.zcount == 0:
-            self.zcount = 1
-            self.dependZ= False
-    
-    def __str__(self):
-        """
-        Print this class as a string.
-        """
-        return '\n'.join(('%8s: %s' % item for item in self.__dict__.items()))
-    
-    def __repr__(self):
-        """
-        Print this class as a string.
-        """
-        return 'CtlVar: {0:8s} in shape (t={1:d}, z={2:d}, y={3:d}, x={4:d})'\
-                .format(self.name,
-                        self.tcount, self.zcount,
-                        self.ycount, self.xcount)
-
-
-
-"""
-Some useful functions defined here
-"""
-def GrADStime_to_datetime(gradsTime):
-    """Convert GrADS time string e.g., 00:00z01Jan2000 to datetime
-    
-    Parameters
-    ----------
-    gradsTime: str
-        Grads time in str format e.g., 00:00z01Jan2000.
-    
-    Returns
-    -------
-    datetime
-        GrADS time in datetime format
-    """
-    lens = len(gradsTime)
-    
-    if   lens==15 or lens==14:
-        time = datetime.strptime(gradsTime, "%H:%Mz%d%b%Y")
-    elif lens==12 or lens==11:
-        time = datetime.strptime(gradsTime, "%Hz%d%b%Y"   )
-    elif lens== 9 or lens== 8:
-        time = datetime.strptime(gradsTime, "%d%b%Y"      )
-    elif lens== 7:
-        time = datetime.strptime(gradsTime, "%b%Y"        )
-    else:
-        raise Exception('invalid length of GrADS date/time string')
-    
-    return time
-
-
-def GrADStime_to_datetime64(gradsTime):
-    """Convert GrADS time string e.g., 00:00z01Jan2000 to numpy.datetime64
-    
-    Parameters
-    ----------
-    gradsTime : str
-        Grads time in str format e.g., 00:00z01Jan2000.
-    
-    Returns
-    -------
-    datetime64
-        GrADS time in datetime64 format
-    """
-    time = GrADStime_to_datetime(gradsTime)
-    
-    return datetime64(time.strftime('%Y-%m-%dT%H:%M:%S'))
-
-
-def GrADS_increment_to_timedelta64(incre):
-    """Convert GrADS time increment string to numpy.timedelta64
-    
-    Parameters
-    ----------
-    incre: str
-        Grads time increment in str format e.g., 1dy.
-    
-    Returns
-    -------
-    timedelta64
-        GrADS time in datetime64 format
-    """
-    unit   = incre[-2:]
-    amount = incre[:-2]
-
-    unitDict = {
-        'se': 's',
-        'mn': 'm',
-        'hr': 'h',
-        'dy': 'D',
-        'mo': 'M',
-        'yr': 'Y'}
-
-    return timedelta64(int(amount), unitDict[unit])
-
-
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on 2020.03.02
+
+@author: MiniUFO
+Copyright 2018. All rights reserved. Use is subject to license terms.
+"""
+import os, sys, re
+import numpy as np
+from datetime import datetime
+from numpy import datetime64, timedelta64
+
+
+"""
+Core classes are defined below
+"""
+class CtlDescriptor(object):
+    """A class for a ctl file
+    
+    This class represents a descriptor file like the .ctl file for GrADS.
+    It generally includes a multi-dimensional dataset on the Earth.
+    
+    Attributes
+    ----------
+    dsetPath: str
+        dataset file
+    descPath: str
+        descriptor file
+    indxPath: str
+        index file (for GRIB file)
+    stnmPath: str
+        station map file (for station file)
+    
+    pdef: PDEF
+        Projection-definition
+    tdef: Coordinate
+        time coordinate definition
+    zdef: Coordinate
+        z-coordinate definition
+    ydef: Coordinate
+        y-coordinate definition
+    xdef: Coordinate
+        x-coordinate definition
+    vdef: list of CtlVar
+        Variables definition
+    edef: list of str
+        Ensemble definition
+    
+    comments: list of str
+        list of global string comments
+    
+    zrev: bool
+        z-dimension reverse (i.e., from north to south)
+    yrev: bool
+        y-dimension reverse (i.e., from upper to lower levels)
+    
+    hasData: bool
+        whether the corresponding binary data file exist
+    vcount: int
+        variable count
+    
+    dtype: numpy.dtype
+        data type
+    periodicX: bool
+        whether xdef is periodic
+    
+    cal365Days: bool
+        whether the calendar is always 365 days (no leap year)
+    template: bool
+        whether it is a template for multiple binary files
+    sequential: bool
+        whether it is a sequential file (Fortran style)
+    byteOrder: str
+        byte order, ['little', 'big'] for little-endian or big-endian
+    storage: str
+        storage type, '99' or '-1,20' or others
+    
+    totalZCount: int
+        total number of horizontal slice
+    zRecLength: int
+        record length of a single horizontal slice
+    tRecLength: int
+        record length of a single time (including all variables)
+    """
+    def __init__(self, encoding='GBK', **kwargs):
+        """Constructor
+
+        One of the keyword argument `file` or `content` should be specified.
+        
+        Parameters
+        ----------
+        encoding: {'GBK', 'UTF-8'}, optional
+            Encoding for the ctl file contents.
+        file: str
+            The ctl path/file name.
+        content: str
+            A string representation for the ctl file contents.
+
+        Returns
+        -------
+        CtlDescriptor
+            An object represents the ctl file
+        """
+        self.vcount = 0
+        
+        self.pdef = None
+        self.tdef = None
+        self.zdef = None
+        self.ydef = None
+        self.xdef = None
+        self.vdef = None
+        self.edef = None
+        self.comments = {}
+        
+        self.dsetPath = ''
+        self.descPath = ''
+        self.indxPath = ''
+        self.stnmPath = ''
+        self.storage  = ''
+        self.dtype    = ''
+        self.title    = ''
+        self.incre    = ''
+        
+        self.zrev     = False
+        self.yrev     = False
+        self.hasData  = False
+        
+        self.periodicX   = False
+        self.cal365Days  = False
+        self.template    = False
+        self.sequential  = False
+        
+        self.totalZCount = 0
+        self.zRecLength  = 0
+        self.tRecLength  = 0
+        self.byteOrder   = sys.byteorder
+        
+        if kwargs.get('file'):
+            abspath = kwargs['file']
+            
+            if not '/' in abspath: # thanks to Baofeng Jiao from IAP
+                abspath = './' + abspath
+            
+            if os.path.getsize(abspath) / (1024.0*1024.0) > 2:
+                raise Exception('ctl file is too large (> 2 MB)')
+            
+            with open(abspath, 'r', encoding=encoding) as f:
+                fileContent = f.readlines()
+        
+        elif kwargs.get('content'):
+            abspath = None
+            fileContent = kwargs['content'].splitlines()
+        else:
+            raise Exception('invalid key word '+
+                            '(file='' or content='' is allowed)')
+        
+        for i, line in enumerate(fileContent):
+            llower = line.lower()
+            if (llower.startswith('dset') or
+                llower.startswith('index') or
+                llower.startswith('stnmap')
+               ) and abspath is not None and '^' in line:
+                dirname = os.path.dirname(abspath)
+                if dirname[-1] != '/':
+                    fileContent[i] = line.replace('^',
+                                       os.path.dirname(abspath) + '/')
+                else:
+                    fileContent[i] = line.replace('^',
+                                       os.path.dirname(abspath))
+        
+        self.descPath=abspath
+        self.parse(fileContent)
+    
+    def parse(self, fileContent):
+        """Parse file content as a multi-line str"""
+        dpath_str = None
+        
+        for oneline in fileContent:
+            if   oneline.lower().startswith('dset'):
+                dpath_str = oneline.split()[1]
+            elif oneline.lower().startswith('index'):
+                self._processIndex(oneline)
+            elif oneline.lower().startswith('stnmap'):
+                self._processStnmap(oneline)
+            elif oneline.lower().startswith('dtype'):
+                self.dtype = oneline[5:].strip()
+            elif oneline.lower().startswith('pdef'):
+                self._processPDEF(oneline)
+            elif oneline.lower().startswith('title'):
+                self.title = oneline.split()[1].strip()
+            elif oneline.lower().startswith('undef'):
+                self.undef = float(oneline.split()[1].strip())
+            elif oneline.lower().startswith('options'):
+                self._processOptions(oneline)
+            elif oneline.lower().startswith('byteswapped'):
+                self.byteOrder  = 'big' \
+                    if sys.byteorder == 'little' else 'little'
+            elif oneline.lower().startswith('xdef'):
+                self._processXDef(oneline, fileContent)
+            elif oneline.lower().startswith('ydef'):
+                self._processYDef(oneline,fileContent)
+            elif oneline.lower().startswith('zdef'):
+                self._processZDef(oneline, fileContent)
+            elif oneline.lower().startswith('tdef'):
+                self._processTDef(oneline)
+            elif oneline.lower().startswith('edef'):
+                self._processEDef(oneline, fileContent)
+            elif oneline.lower().startswith('vars'):
+                self._processVars(oneline, fileContent)
+            elif oneline.lower().startswith('@ global string comment'):
+                self._processGlobalComments(oneline)
+            elif oneline.startswith('*') or oneline.strip() == '':
+                continue
+        
+        if dpath_str == None:
+            raise Exception('no valid dset is parsed')
+        
+        if self.template:
+            self._processDSets(dpath_str)
+        else:
+            self._processDSet(dpath_str)
+        
+        if self.yrev:
+            self.ydef.samples = np.flip(self.ydef.samples)
+        
+        if self.zrev:
+            self.zdef = np.flip(self.zdef)
+        
+        if self.edef:
+            strPos = 0
+            for i, e in enumerate(self.edef):
+                self.edef[i] = self.edef[i]._replace(strPos=strPos)
+                strPos += e.tcount * self.tRecLength
+    
+    def _processDSets(self, dpath_str):
+        strPos = dpath_str.find('%')
+        
+        if strPos == -1:
+            raise Exception('template is used in ctl but no % in dset')
+        
+        endPos = len(dpath_str) - dpath_str[::-1].find('.') - 1
+        # endPos = len(dpath_str) if endPos == -1 else endPos
+        
+        template = dpath_str[strPos:endPos]
+        
+        tokens = [self._get_template_format('%'+token)
+                  for token in filter(lambda x: x != '', template.split('%'))]
+        # tokens = []
+        # for token in filter(lambda x: x != '', template.split('%')):
+        #     tokens.append(self._get_template_format('%' + token))
+        fmt = ''.join(tokens)
+        
+        fileList = []
+        
+        times = self.tdef.samples
+        base  = self._get_field(times[0])
+        for l in range(len(times)):
+            part = times[l].item().strftime(fmt)
+            
+            fname = dpath_str[:strPos] + part + dpath_str[endPos:]
+            fname = self._replace_forecast_template(fname, l, base)
+            
+            # remove duplicated file
+            if fname not in fileList:
+                fileList.append(fname)
+        
+        self.dsetPath = np.array(fileList)
+        
+        has = True
+        for file in fileList:
+            if not os.path.exists(file):
+                has = False
+                break
+
+        self.hasData = has
+        
+    def _processDSet(self, dpath_str):
+        self.dsetPath = dpath_str
+        self.hasData  = os.path.exists(self.dsetPath)
+    
+    def _processIndex(self, oneline):
+        self.indxPath = oneline.split()[1]
+    
+    def _processStnmap(self, oneline):
+        self.stnmPath = oneline.split()[1]
+    
+    def _processPDEF(self, oneline):
+        self.pdef = PDEF(oneline)
+    
+    def _processOptions(self, oneline):
+        lineLower = oneline.lower()
+        
+        if 'yrev'             in lineLower: self.yrev       = True
+        if 'zrev'             in lineLower: self.zrev       = True
+        if 'template'         in lineLower: self.template   = True
+        if 'sequential'       in lineLower: self.sequential = True
+        if '365_day_calendar' in lineLower: self.cal365Days = True
+        if 'big_endian'       in lineLower: self.byteOrder  = 'big'
+        if 'byteswapped'      in lineLower: self.byteOrder  = \
+            'big' if sys.byteorder == 'little' else 'little'
+    
+    def _processXDef(self, oneline, fileContent):
+        tokens = oneline.lower().split()
+        xnum   = int(tokens[1])
+        
+        if   tokens[2] == 'linear': xlnr = True
+        elif tokens[2] == 'levels': xlnr = False
+        else: raise Exception('invalid type for xdef (linear or levels): ' +
+                              tokens[2])
+
+        if xlnr:
+            start, intv = float(tokens[3]), float(tokens[4])
+            self.xdef = Coordinate('xdef', np.linspace(start,
+                                                       start + intv * (xnum-1),
+                                                       xnum, dtype=np.float32))
+        else:
+            values = [float(i) for i in tokens[3:]]
+            count  = len(values)
+            index  = fileContent.index(oneline) + 1
+            
+            while count < xnum:
+                split = fileContent[index].split()
+                values += [float(v) for v in split]
+                count  += len(split)
+                index  += 1
+            
+            if count != xnum:
+                raise Exception('not parse xdef correctly')
+            
+            self.xdef = Coordinate('xdef', np.array(values))
+
+        self.periodicX = self.xdef.isPeriodic(360)
+
+    def _processYDef(self, oneline, fileContent):
+        tokens = oneline.lower().split()
+        ynum   = int(tokens[1])
+        
+        if   tokens[2] == 'linear': ylnr = True
+        elif tokens[2] == 'levels': ylnr = False
+        else: raise Exception('invalid type for ydef (linear or levels): ' +
+                              tokens[2])
+        
+        if ylnr:
+            start, intv = float(tokens[3]), float(tokens[4])
+            self.ydef = Coordinate('ydef', np.linspace(start,
+                                                       start + intv * (ynum-1),
+                                                       ynum, dtype=np.float32))
+        else:
+            values = [float(i) for i in tokens[3:]]
+            count  = len(values)
+            index  = fileContent.index(oneline) + 1
+            
+            while count < ynum:
+                split = fileContent[index].split()
+                values += [float(v) for v in split]
+                count  += len(split)
+                index  += 1
+            
+            if count != ynum:
+                raise Exception(('not parse ydef correctly, count={0} '+
+                                 'while ynum={1}').format(count, ynum))
+            
+            self.ydef = Coordinate('ydef', np.array(values))
+    
+    def _processZDef(self, oneline, fileContent):
+        tokens = oneline.lower().split()
+        znum   = int(tokens[1])
+        
+        if   tokens[2] == 'linear': zlnr = True
+        elif tokens[2] == 'levels': zlnr = False
+        else: raise Exception('invalid type for zdef (linear or levels): ' +
+                              tokens[2])
+        
+        if zlnr:
+            start, intv = float(tokens[3]), float(tokens[4])
+            self.zdef = Coordinate('zdef', np.linspace(start,
+                                                       start + intv * (znum-1),
+                                                       znum, dtype=np.float32))
+            
+        else:
+            values = [float(i) for i in tokens[3:]]
+            count  = len(values)
+            index  = fileContent.index(oneline) + 1
+            
+            while count < znum:
+                split = fileContent[index].split()
+                values += [float(v) for v in split]
+                count  += len(split)
+                index  += 1
+            
+            if count != znum:
+                raise Exception('zdef not parsed correctly')
+            
+            self.zdef = Coordinate('zdef', np.array(values))
+
+    def _processTDef(self, oneline):
+        tokens = oneline.lower().split()
+        tnum   = int(tokens[1])
+
+        if tokens[2]!='linear':
+            raise Exception('nonlinear tdef is not supported')
+
+        times = self._times_to_array(tokens[3], tokens[4], tnum)
+        
+        self.incre = GrADS_increment_to_timedelta64(tokens[4])
+        self.tdef  = Coordinate('tdef', times)
+
+    def _processEDef(self, oneline, fileContent):
+        if not self.tdef:
+            raise Exception('edef should be after tdef')
+        
+        from collections import namedtuple
+        
+        Ensemble = namedtuple('Ensemble', ['name', 'tcount', 'tstart',
+                                           'codes', 'strPos'])
+        
+        tokens = oneline.lower().split()
+        enum   = int(tokens[1])
+        tdef   = self.tdef
+        index  = fileContent.index(oneline) + 1
+        
+        if len(tokens) > 2:
+            if tokens[2].lower() == 'names':
+                NAMES = True
+            else:
+                raise Exception(f'Expected str \'NAMEs\', but found {tokens[2]}')
+            
+            if NAMES:
+                enames = [i for i in tokens[3:]]
+                count  = len(enames)
+                
+                while count < enum:
+                    split = fileContent[index].split()
+                    enames += [v for v in split]
+                    count  += len(split)
+                    index  += 1
+                
+                if count != enum:
+                    raise Exception((f'edef not parsed correctly, count={count} '+
+                                     'while enum={enum}'))
+                
+                self.edef = [Ensemble(name, tdef.length(), tdef.samples[0], None, 0)
+                             for name in enames]
+        else:
+            tmp = []
+            for i in range(enum):
+                eline = fileContent[index + i].strip()
+                
+                if eline.lower() == 'endedef':
+                    raise Exception(f'not enough ensembles, need {enum}')
+                
+                tkns  = eline.split()
+                
+                name = tkns[0]
+                tcnt = int(tkns[1])
+                tstr = GrADStime_to_datetime(tkns[2])
+                code = None
+                
+                if len(tkns) >3:
+                    code = tkns[3]
+                    
+                if tcnt > tdef.length():
+                    raise Exception('Tcount in EDEF must be less than or equal' +
+                                    'to the Tcount in TDEF')
+                
+                tmp.append(Ensemble(name, tcnt, tstr, code, 0))
+            
+            self.edef = tmp
+    
+    def _processVars(self, oneline, fileContent):
+        if (self.dtype != 'station' and 
+            not all([self.tdef, self.zdef, self.ydef, self.xdef])):
+            raise Exception('vdef should be after x, y, z and t definitions')
+        
+        t = self.tdef.length()
+        
+        if self.dtype != 'station':
+            y = self.ydef.length() if self.pdef is None else self.pdef.jsize
+            x = self.xdef.length() if self.pdef is None else self.pdef.isize
+        
+            self.zRecLength = x * y * 4
+            
+            # add two bytes at the beginning and the end
+            if self.sequential:
+                self.zRecLength += 8
+        
+        tokens = oneline.split()
+        vnum   = int(tokens[1])
+        start  = fileContent.index(oneline) + 1
+        
+        if vnum < 1:
+            raise Exception('there should be at least one CtlVar')
+        
+        self.vcount = vnum
+        self.vdef   = [None] * vnum
+        
+        v = CtlVar(fileContent[start])
+        v.index =0
+        v.strPos=0
+        v.tcount=t
+        
+        if self.dtype != 'station':
+            v.ycount=y
+            v.xcount=x
+        
+        self.totalZCount += v.zcount
+        self.storage      = v.storage
+        self.vdef[0]      = v
+        
+        type1 = type2 = type3 = False
+        
+        for i in range(1, vnum):
+            v  = CtlVar(fileContent[start+i])
+            vs = self.vdef[i-1]
+            
+            v.index  = i
+            v.undef  = self.undef
+            v.tcount = t
+            
+            if self.dtype != 'station':
+                v.ycount = y
+                v.xcount = x
+            
+            # if v.storage in ['99', '0']:
+            if v.storage in ['99', '0', '00', '000', '1', '11', '111']:
+                v.strPos = vs.zcount * self.zRecLength + vs.strPos
+                type1 = True
+            elif v.storage == '-1,20':
+                v.strPos = vs.zcount * self.zRecLength * t + vs.strPos
+                type2 = True
+            else:
+                type3 = True
+            
+            if not type3 and type1 == type2:
+                raise Exception('storage type should be the same')
+            
+            self.totalZCount += v.zcount
+            self.vdef[i] = v
+        
+        self.tRecLength = self.zRecLength * self.totalZCount
+        
+        if fileContent[start + vnum].strip().lower() != 'endvars':
+            raise Exception('endvars is expected')
+    
+    def _processGlobalComments(self, oneline):
+        cnt = oneline[24:].strip().split('=')
+        
+        self.comments[cnt[0].strip()] = cnt[1].strip()
+
+    def _get_template_format(self, part):
+        """Get time format string
+        
+        See the following URL for reference:
+        http://cola.gmu.edu/grads/gadoc/templates.html
+        
+        %x1   1 digit decade
+        %x3   3 digit decade
+        %y2   2 digit year
+        %y4   4 digit year
+        %m1   1 or 2 digit month
+        %m2   2 digit month (leading zero if needed)
+        %mc   3 character month abbreviation
+        %d1   1 or 2 digit day
+        %d2   2 digit day (leading zero if needed)
+        %h1   1 or 2 digit hour
+        %h2   2 digit hour
+        %h3   3 digit hour (e.g., 120 or 012)
+        %n2   2 digit minute; leading zero if needed
+        %f2   2 digit forecast hour; leading zero if needed; more digits added
+              for hours >99; hour values increase indefinitely
+        %f3   3 digit forecast hour; leading zeros if needed; more digits added
+              for hours >999; hour values increase indefinitely
+        %fn2  2 digit forecast minute; leading zero if needed; more digits added
+              for minutes > 99; minute values increase indefinitely (2.0.a9+)
+        %fhn  forecast time expressed in hours and minutes (hhnn) where minute
+              value (nn) is always <=59 and hour value (hh) increases indefinitely.
+              If hh or nn are <=9, they are padded with a 0, so they are always at
+              least 2 digits; more digits added for hours >99. (2.0.a9+)
+        %fdhn forecast time expressed in days, hours, and minutes (ddhhnn) where
+              minute value (nn) is always <=59, hour value (hh) is always <=23 and
+              day value (dd) increases indefinitely. If dd, hh, or nn are <=9, they
+              are padded with a 0 so they are always at least 2 digits; more digits
+              added for days >99. (2.0.a9+)
+        %j3   3 digit julian day (day of year) (2.0.a7+)
+        %t1   1 or 2 digit time index (file names contain number sequences that
+              begin with 1 or 01) (2.0.a7+)
+        %t2   2 digit time index (file names contain number sequences that begin
+              with 01) (2.0.a7+)
+        %t3   3 digit time index (file names contain number sequences that begin
+              with 001) (2.0.a7+)
+        %t4   4 digit time index (file names contain number sequences that begin
+              with 0001) (2.0.a8+)
+        %t5   5 digit time index (file names contain number sequences that begin
+              with 00001) (2.0.a8+)
+        %t6   6 digit time index (file names contain number sequences that begin
+              with 000001) (2.0.a8+)
+        %tm1  1 or 2 digit time index (file names contain number sequences that
+              begin with 0 or 00) (2.0.a7+)
+        %tm2  2 digit time index (file names contain number sequences that begin
+              with 00) (2.0.a7+)
+        %tm3  3 digit time index (file names contain number sequences that begin
+              with 000) (2.0.a7+)
+        %tm4  4 digit time index (file names contain number sequences that begin
+              with 0000) (2.0.a8+)
+        %tm5  5 digit time index (file names contain number sequences that begin
+              with 00000) (2.0.a8+)
+        %tm6  6 digit time index (file names contain number sequences that begin
+              with 000000) (2.0.a8+)
+    
+        Parameters
+        ----------
+        part : str
+            A string in the above format started with %.
+    
+        Returns
+        -------
+        str
+            The format in python datetime
+        """
+        if   part == '%y2':
+            return '%y'
+        elif part == '%y4':
+            return '%Y'
+        elif part == '%m1':
+            return '%m'
+        elif part == '%m2':
+            return '%m'
+        elif part == '%mc':
+            return '%b'
+        elif part == '%d1':
+            return '%d'
+        elif part == '%d2':
+            return '%d'
+        elif part == '%h1':
+            return '%H'
+        elif part == '%h2':
+            return '%H'
+        elif part == '%n2':
+            return '%M'
+        elif part in ['%f3', '%f2', '%fn2', '%fhn', '%fdhn']:
+            # this is not supported by strftime()
+            return '_miniufo_' + part[1:]
+        else:
+            raise Exception('unsupported format: ' + part)
+    
+    def _replace_forecast_template(self, fname, l, base):
+        """Replace forecast str %f as a template in dset
+    
+        Parameters
+        ----------
+        fname: str
+            A given string of binary file.
+        l: int
+            Index of file in a template.
+        base: numpy.datetime64
+            Base time.
+    
+        Returns
+        -------
+        str
+            A string after replacing the %f template.
+        """
+        amount = l * self.incre
+        
+        days = base[..., 2]
+        hour = base[..., 3]
+        mins = base[..., 4]
+        
+        if fname.find('_miniufo_f3') != -1:
+            dt = (amount.astype("timedelta64[h]") + hour).astype(int)
+            fname = fname.replace('_miniufo_f3', '{0:03d}'.format(dt))
+        
+        if fname.find('_miniufo_f2') != -1:
+            dt = (amount.astype("timedelta64[h]") + hour).astype(int)
+            fname = fname.replace('_miniufo_f2', '{0:02d}'.format(dt))
+        
+        if fname.find('_miniufo_fn2') != -1:
+            dt = (amount.astype("timedelta64[m]") + mins).astype(int)
+            fname = fname.replace('_miniufo_fn2', '{0:02d}'.format(dt))
+        
+        if fname.find('_miniufo_fhn') != -1:
+            dt_h = (amount.astype("timedelta64[h]") + hour).astype(int)
+            dt_m = (amount.astype("timedelta64[m]") + mins).astype(int) % 60
+            fname = fname.replace('_miniufo_fhn',
+                                  '{0:02d}'.format(dt_h)+'{0:02d}'.format(dt_m))
+        
+        if fname.find('_miniufo_fdhn') != -1:
+            dt_d = (amount.astype("timedelta64[D]") + days).astype(int)
+            dt_h = (amount.astype("timedelta64[h]") + hour).astype(int) % 24
+            dt_m = (amount.astype("timedelta64[m]") + mins).astype(int) % 60
+            fname = fname.replace('_miniufo_fdhn',
+                                  '{0:02d}'.format(dt_d)+
+                                  '{0:02d}'.format(dt_h)+
+                                  '{0:02d}'.format(dt_m))
+        
+        return fname
+
+    def _get_field(self, datetime64):
+        """Get fields of a datetime64
+        
+        Convert array of datetime64 to a calendar array of
+        [year, month, day, hour, minute, seconds, microsecond]
+        with these quantites indexed on the last axis.
+    
+        Parameters
+        ----------
+        datetime64: datetime64 array (...)
+            numpy.ndarray of datetimes of arbitrary shape
+    
+        Returns
+        -------
+        cal: uint32 array (..., 7)
+            calendar array with last axis representing year, month, day, hour,
+            minute, second, microsecond
+        """
+        # allocate output 
+        out = np.empty(datetime64.shape + (7,), dtype="u4")
+        
+        # decompose calendar floors
+        Y, M, D, h, m, s = [datetime64.astype(f'M8[{x}]') for x in 'YMDhms']
+        
+        out[..., 0] = Y + 1970 # Gregorian Year
+        out[..., 1] = (M - Y) + 1 # month
+        out[..., 2] = (D - M) + 1 # dat
+        out[..., 3] = (datetime64 - D).astype('m8[h]' ) # hour
+        out[..., 4] = (datetime64 - h).astype('m8[m]' ) # minute
+        out[..., 5] = (datetime64 - m).astype('m8[s]' ) # second
+        out[..., 6] = (datetime64 - s).astype('m8[us]') # microsecond
+        
+        return out
+
+
+    def _times_to_array(self, strTime, incre, tnum):
+        """Change format of time
+        
+        Convert GrADS time string of strart time and increment
+        to an array of numpy.datetime64.
+        
+        Parameters
+        ----------
+        strTime : str
+            Grads start time e.g., 00:00z01Jan2000.
+        incre : str
+            Grads time increment in str format e.g., 1dy.
+        tnum : int
+            Grads time increment in str format e.g., 1dy.
+        
+        Returns
+        -------
+        numpy array of datetime64
+            Times in datetime64 format
+        """
+        if 'mo' in incre:
+            start = GrADStime_to_datetime(strTime)
+            
+            lst = []
+            for l in range(tnum):
+                y, m = start.year, start.month
+                y, m = y+int((m+l-1)/12), int((m+l-1)%12)+1
+                lst.append(start.replace(year=y, month=m))
+            
+            return np.asarray(lst, dtype='datetime64[s]')
+            
+        elif 'yr' in incre:
+            start = GrADStime_to_datetime(strTime)
+            
+            lst = []
+            for l in range(tnum):
+                y = start.year + l
+                lst.append(start.replace(year=y))
+            
+            return np.asarray(lst, dtype='datetime64[s]')
+        
+        else:
+            start = GrADStime_to_datetime64(strTime)
+            intv  = GrADS_increment_to_timedelta64(incre)
+
+            if self.cal365Days:
+
+                lst = []
+                while len(lst) < tnum:
+                    isfeb29 = (start.item().day == 29) and (start.item().month == 2)
+                    if not isfeb29:
+                        lst.append(start)
+                    start += intv
+
+                return np.asarray(lst)
+
+            else:
+
+                return np.arange(start, start + intv * tnum, intv)
+
+    def __repr__(self):
+        """Print this class as a string"""
+        vdef = np.array(self.vdef)
+        pdef = self.pdef.proj if self.pdef is not None else ''
+        
+        if self.edef is not None:
+            edef = [f'Ensem: {e.name}, {e.tcount}, {e.tstart}, {e.codes}, {e.strPos}'
+                    for e in self.edef]
+        else:
+            edef = 'None'
+        
+        return \
+            '   dsetPath: ' + str(self.dsetPath)  + '\n'\
+            '   descPath: ' + str(self.descPath)  + '\n'\
+            '   indxPath: ' + str(self.indxPath)  + '\n'\
+            '   stnmPath: ' + str(self.stnmPath)  + '\n'\
+            '      title: ' + str(self.title)     + '\n'\
+            '      undef: ' + str(self.undef)     + '\n'\
+            '       zrev: ' + str(self.zrev)      + '\n'\
+            '       yrev: ' + str(self.yrev)      + '\n'\
+            '      dtype: ' + str(self.dtype)     + '\n'\
+            '   template: ' + str(self.template)  + '\n'\
+            '  periodicX: ' + str(self.periodicX) + '\n'\
+            ' cal365Days: ' + str(self.cal365Days)+ '\n'\
+            ' sequential: ' + str(self.sequential)+ '\n'\
+            '  byteOrder: ' + str(self.byteOrder) + '\n'\
+            '       xdef: ' + str(self.xdef)      + '\n'\
+            '       ydef: ' + str(self.ydef)      + '\n'\
+            '       zdef: ' + str(self.zdef)      + '\n'\
+            '       tdef: ' + str(self.tdef)      + '\n'\
+            '       edef: ' + str(edef)           + '\n'\
+            '       pdef: ' + str(pdef)           + '\n'\
+            '       vdef: ' + str(vdef)
+
+
+
+class PDEF(object):
+    """PDEF class
+    
+    Parse necessary info in PDEF.
+    
+    Reference: http://cola.gmu.edu/grads/gadoc/pdef.html
+    
+    Attributes
+    ----------
+    isize: int
+        size of native grid in x direction
+    jsize: int
+        size of native grid in y direction
+    proj: str
+        type of projection
+    lonref: str
+        reference longitude
+    """
+    def __init__(self, oneline):
+        """Constructor
+        
+        Parameters
+        ----------
+        oneline: str
+            The ASCII line of PDEF in ctl file.
+        """
+        lineLower = oneline.lower()
+        
+        if 'nps' in lineLower or 'sps' in lineLower:
+            token = lineLower.split()
+            
+            if len(token) != 8:
+                raise Exception('not enough tokens for PDEF, ' +
+                                'expected 8 but found ' + str(len(token)))
+            
+            self.isize   = int  (token[1]) # size of native grid in x direction
+            self.jsize   = int  (token[2]) # size of native grid in y direction
+            self.proj    =      (token[3]) # type of projection
+            self.ipole   = int  (token[4]) # i-coord of pole ref to ll corner
+            self.jpole   = int  (token[5]) # j-coord of pole ref to ll corner
+            self.lonref  = float(token[6]) # reference longitude
+            self.gridinc = float(token[7]) # distance between gripoints in km
+            
+        elif 'lccr' in lineLower or 'lcc' in lineLower:
+            token = lineLower.split()
+            
+            if len(token) != 13:
+                raise Exception('not enough tokens for PDEF, ' +
+                                'expected 13 but found ' + str(len(token)))
+            
+            self.isize   = int  (token[1]) # size of native grid in x direction
+            self.jsize   = int  (token[2]) # size of native grid in y direction
+            self.proj    =      (token[3]) # type of projection
+            self.latref  = float(token[4]) # ref latitude
+            self.lonref  = float(token[5]) # ref longitude (E>0, W<0)
+            self.iref    = float(token[6]) # i of ref point
+            self.jref    = float(token[7]) # j of ref point
+            self.Struelat= float(token[8]) # S true lat
+            self.Ntruelat= float(token[9]) # N true lat
+            self.slon    = float(token[10]) # standard longitude
+            self.dx      = float(token[11]) # grid X increment in meters
+            self.dy      = float(token[12]) # grid Y increment in meters
+        
+        else:
+            raise Exception('not currently supported PDEF\n' + oneline)
+
+    def __repr__(self):
+        """Print this class as a string"""
+        return '\n'.join(['%s: %s' % item for item in self.__dict__.items()])
+    
+
+
+class Coordinate(object):
+    """Discrete sampled coordinate
+    
+    This is a simple wrapper for np.array for a coordinate.
+    
+    Attributes
+    ----------
+    isLinear: bool
+        Steps are even or uneven
+    isIncre: int
+        Is increasing or decreasing
+    name: str
+        The name of the coordinate
+    samples: str
+        Discretized coordinate samples
+    delSamples: str
+        Finite difference between samples
+    """
+    def __init__(self, name, samples):
+        """Constructor
+        
+        Parameters
+        ----------
+        name : str
+            The name of the coordinate.
+        samples : np.array
+            1D array for the discrete coordinate.
+        """
+        self.isLinear   = True
+        self.isIncre    = True
+        self.name       = name
+        self.samples    = samples
+        self.delSamples = None
+        
+        self.max = np.max(self.samples)
+        self.min = np.min(self.samples)
+        
+        if len(samples) > 1:
+            self.delSamples = np.diff(self.samples)
+            
+            if self.samples[-1] < self.samples[0]:
+                self.isIncre=False
+        else:
+            self.delSamples = np.array([1])
+    
+    def length(self):
+        return len(self.samples)
+    
+    def isPeriodic(self,period):
+        # not physically but generally true
+        if not self.isLinear: return False
+        
+        delta = self.delSamples[0]
+        start = self.samples[-1] + delta - period
+        
+        if(abs((start - self.samples[0]) / delta > 1e-4)):
+            return False
+        
+        return True
+    
+    def __str__(self):
+        """Print this class as a string"""
+        return str(self.samples)
+
+
+
+class CtlVar(object):
+    """A simple variable class used in .ctl file
+    
+    Attributes
+    ----------
+    tcount: int
+        T grid points
+    zcount: int
+        Z grid points
+    ycount: int
+        Y grid points
+    xcount: int
+        X grid points
+    undef: float
+        Undefined values
+    dependZ: bool
+        Whether the var depends on z
+    unit: str
+        Unit of the variable
+    name: str
+        Name of the variable
+    comment: str
+        A short comment
+    index: str
+        Index of this variable
+    strPos: str
+        Start position (in bytes) of this variable in the binary file
+    """
+    __reBlank = re.compile(r'[\s\t]+')
+    __reUnits = re.compile(r'\([^\(\)]+?\)')
+    
+    
+    def __init__(self, oneLineStr):
+        self.tcount = 0
+        self.zcount = 0
+        self.ycount = 0
+        self.xcount = 0
+        self.undef  = np.nan
+        self.dependZ= True # whether the var depends on z
+        
+        self.unit   = ''
+        self.name   = ''
+        self.comment= ''
+        
+        self.index  = 0
+        self.strPos = 0
+        
+        if len(CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3))== 3:
+            self.name, self.zcount, self.storage = \
+                CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3)
+            self.comment = self.name
+        else:
+            self.name, self.zcount, self.storage, self.comment = \
+                CtlVar.__reBlank.split(oneLineStr.strip(), maxsplit=3)
+        
+        self.zcount = int(self.zcount)
+        
+        findMatch = CtlVar.__reUnits.findall(self.comment)
+        
+        if findMatch:
+            self.unit    = findMatch[-1]
+            self.comment = self.comment[:self.comment.index(self.unit)].strip()
+        else:
+            self.unit = ''
+
+        if self.zcount == 0:
+            self.zcount = 1
+            self.dependZ= False
+    
+    def __str__(self):
+        """
+        Print this class as a string.
+        """
+        return '\n'.join(('%8s: %s' % item for item in self.__dict__.items()))
+    
+    def __repr__(self):
+        """
+        Print this class as a string.
+        """
+        return 'CtlVar: {0:8s} in shape (t={1:d}, z={2:d}, y={3:d}, x={4:d})'\
+                .format(self.name,
+                        self.tcount, self.zcount,
+                        self.ycount, self.xcount)
+
+
+"""
+Some useful functions defined here
+"""
+def GrADStime_to_datetime(gradsTime):
+    """Convert GrADS time string e.g., 00:00z01Jan2000 to datetime
+    
+    Parameters
+    ----------
+    gradsTime: str
+        Grads time in str format e.g., 00:00z01Jan2000.
+    
+    Returns
+    -------
+    datetime
+        GrADS time in datetime format
+    """
+    lens = len(gradsTime)
+    
+    if   lens==15 or lens==14:
+        time = datetime.strptime(gradsTime, "%H:%Mz%d%b%Y")
+    elif lens==12 or lens==11:
+        time = datetime.strptime(gradsTime, "%Hz%d%b%Y"   )
+    elif lens== 9 or lens== 8:
+        time = datetime.strptime(gradsTime, "%d%b%Y"      )
+    elif lens== 7:
+        time = datetime.strptime(gradsTime, "%b%Y"        )
+    else:
+        raise Exception('invalid length of GrADS date/time string')
+    
+    return time
+
+
+def GrADStime_to_datetime64(gradsTime):
+    """Convert GrADS time string e.g., 00:00z01Jan2000 to numpy.datetime64
+    
+    Parameters
+    ----------
+    gradsTime : str
+        Grads time in str format e.g., 00:00z01Jan2000.
+    
+    Returns
+    -------
+    datetime64
+        GrADS time in datetime64 format
+    """
+    time = GrADStime_to_datetime(gradsTime)
+    
+    return datetime64(time.strftime('%Y-%m-%dT%H:%M:%S'))
+
+
+def GrADS_increment_to_timedelta64(incre):
+    """Convert GrADS time increment string to numpy.timedelta64
+    
+    Parameters
+    ----------
+    incre: str
+        Grads time increment in str format e.g., 1dy.
+    
+    Returns
+    -------
+    timedelta64
+        GrADS time in datetime64 format
+    """
+    unit   = incre[-2:]
+    amount = incre[:-2]
+
+    unitDict = {
+        'se': 's',
+        'mn': 'm',
+        'hr': 'h',
+        'dy': 'D',
+        'mo': 'M',
+        'yr': 'Y'}
+
+    return timedelta64(int(amount), unitDict[unit])
+
+
+
+
```

### Comparing `xgrads-0.2.3/xgrads/io.py` & `xgrads-0.2.4/xgrads/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,551 +1,629 @@
-# -*- coding: utf-8 -*-
-"""
-Created on 2020.04.11
-
-@author: MiniUFO
-Copyright 2018. All rights reserved. Use is subject to license terms.
-"""
-import os
-import numpy as np
-import xarray as xr
-import dask.array as dsa
-from dask.base import tokenize
-from glob import glob
-from pathlib import Path
-from .core import CtlDescriptor
-from functools import reduce
-
-"""
-IO related functions here
-"""
-def open_mfdataset(paths, parallel=False, encoding='GBK'):
-    """Open multiple ctl files as a single dataset
-    
-    This is similar to `xarray.open_mfdataset()` that can simutaneously open
-    a series of ctl files that are in similar spatial ranges but of different
-    temporal ranges.
-
-    Parameters
-    ----------
-    paths: str or sequence
-        Either a string glob in the form ``"path/to/my/files/*.ctl"`` or an
-        explicit list of files to open. Paths can be given as strings or as
-        pathlib Paths.
-    parallel: bool, optional
-        If True, the open and preprocess steps of this function will be
-        performed in parallel using ``dask.delayed``. Default is False.
-    encoding: str
-        Encoding for the ctl file content e.g., ['GBK', 'UTF-8'].
-
-    Returns
-    -------
-    re: xarray.Dataset
-        A dataset.
-
-    Notes
-    -----
-    ``open_mfdataset`` opens files with read-only access. When you modify values
-    of a Dataset, even one linked to files on disk, only the in-memory copy you
-    are manipulating in xarray is modified: the original file on disk is never
-    touched.
-    """
-    if isinstance(paths, str):
-        paths = sorted(glob(paths))
-    else:
-        paths = [str(p) if isinstance(p, Path) else p for p in paths]
-
-    if not paths:
-        raise OSError("no files to open")
-
-    if parallel:
-        import dask
-
-        # wrap the open_dataset
-        open_ = dask.delayed(open_CtlDataset)
-    else:
-        open_ = open_CtlDataset
-
-    datasets = [open_(p, encoding=encoding) for p in paths]
-
-    if parallel:
-        # calling compute here will return the datasets/file_objs lists,
-        # the underlying datasets will still be stored as dask arrays
-        datasets = dask.compute(datasets)
-
-        return xr.concat(datasets[0], dim='time')
-
-    combined = xr.concat(datasets, dim='time')
-
-    return combined
-
-
-def open_CtlDataset(desfile, returnctl=False, encoding='GBK'):
-    """Open a single ctl dataset
-    
-    Open a 4D dataset with a descriptor file end with .ctl and
-    return a xarray.Dataset.  This also uses the dask to chunk
-    very large dataset, which is similar to the xarray.open_dataset.
-
-    Parameters
-    ----------
-    desfile: string
-        Path to the descriptor file end with .ctl or .cts
-    returnctl: bool
-        Return dset and ctl as a tuple
-
-    Returns
-    -------
-    dset: xarray.Dataset
-        Dataset object containing all coordinates and variables.
-    ctl: xgrads.CtlDescriptor
-        Ctl descriptor file if returnctl == True.
-    """
-    if isinstance(desfile, str):
-        if not desfile.endswith('.ctl'):
-            raise Exception('unsupported file, suffix should be .ctl')
-
-        ctl = CtlDescriptor(encoding=encoding, file=desfile)
-    elif isinstance(desfile, CtlDescriptor):
-        ctl = desfile
-    else:
-        raise Exception('unsupported type of input ('+str(type(desfile))+'), ' +
-                        '[CtlDescriptor or str] are allowed')
-
-    if ctl.template:
-        tcount = len(ctl.tdef.samples) # number of total time count
-        tcPerf = []                    # number of time count per file
-        
-        has_missing = False
-        for file in ctl.dsetPath:
-            if os.path.exists(file):
-                fsize = os.path.getsize(file)
-    
-                if fsize % ctl.tRecLength != 0:
-                    raise Exception('incomplete file for ' + file +
-                                    ' (not multiple of ' + str(ctl.tRecLength) +
-                                    ' bytes)')
-    
-                tcPerf.append(fsize // ctl.tRecLength)
-            else:
-                print(' warning: ' + file + ' is missing...')
-                has_missing = True
-        
-        if has_missing:
-            raise Exception('there are missing binary files')
-
-        total_size = sum(tcPerf)
-
-        if total_size < tcount:
-            raise Exception('no enough files for ' + str(tcount) +
-                            ' time records')
-
-        # get time record number in each file
-        rem = tcount
-        idx = 0
-        for i, num in enumerate(tcPerf):
-            rem -= num
-            if rem <= 0:
-                idx = i
-                break
-
-        tcPerf_m      = tcPerf[:idx+1]
-        tcPerf_m[idx] = tcPerf[idx   ] + rem
-
-        # print(ctl.dsetPath)
-        # print(tcPerf)
-        # print(tcPerf_m)
-
-        binData = __read_template_as_dask(ctl, tcPerf_m)
-
-    else:
-        expect = ctl.tRecLength * ctl.tdef.length()
-        actual = os.path.getsize(ctl.dsetPath)
-
-        if expect != actual:
-            print('WARNING: expected binary file size: {0}, actual size: {1}'
-                            .format(expect, actual))
-
-        binData = __read_as_dask(ctl)
-
-    variables = []
-
-    if ctl.pdef is None:
-        for m, v in enumerate(ctl.vdef):
-            if v.dependZ:
-                da = xr.DataArray(name=v.name, data=binData[m],
-                                  dims=['time', 'lev', 'lat', 'lon'],
-                                  coords={'time': ctl.tdef.samples[:],
-                                          'lev' : ctl.zdef.samples[:v.zcount],
-                                          'lat' : ctl.ydef.samples[:],
-                                          'lon' : ctl.xdef.samples[:]},
-                                  attrs={'comment': v.comment,
-                                         'storage': v.storage})
-            else:
-                t, z, y, x = binData[m].shape
-                da = xr.DataArray(name=v.name,
-                                  data=binData[m].reshape((t,y,x)),
-                                  dims=['time', 'lat', 'lon'],
-                                  coords={'time': ctl.tdef.samples[:],
-                                          'lat' : ctl.ydef.samples[:],
-                                          'lon' : ctl.xdef.samples[:]},
-                                  attrs={'comment': v.comment,
-                                         'storage': v.storage})
-            variables.append(da)
-
-    else:
-        PDEF = ctl.pdef
-
-        if PDEF.proj in ['lcc', 'lccr']:
-            ycoord = np.linspace(0, (PDEF.jsize-1) * PDEF.dx, PDEF.jsize)
-            xcoord = np.linspace(0, (PDEF.isize-1) * PDEF.dy, PDEF.isize)
-
-        elif PDEF.proj in ['sps', 'nps']:
-            inc = PDEF.gridinc * 1000 # change unit from km to m
-            ycoord = np.linspace(-(PDEF.jpole), (PDEF.jsize-PDEF.jpole),
-                                   PDEF.jsize) * inc
-            xcoord = np.linspace(-(PDEF.ipole), (PDEF.isize-PDEF.ipole),
-                                   PDEF.isize) * inc
-
-        for m, v in enumerate(ctl.vdef):
-            if v.dependZ:
-                da = xr.DataArray(name=v.name, data=binData[m],
-                                  dims=['time', 'lev', 'y', 'x'],
-                                  coords={'time': ctl.tdef.samples[:],
-                                          'lev' : ctl.zdef.samples[:v.zcount],
-                                          'y' : ycoord,
-                                          'x' : xcoord},
-                                  attrs={'comment': v.comment,
-                                         'storage': v.storage})
-            else:
-                t, z, y, x = binData[m].shape
-                da = xr.DataArray(name=v.name,
-                                  data=binData[m].reshape((t,y,x)),
-                                  dims=['time', 'y', 'x'],
-                                  coords={'time': ctl.tdef.samples[:],
-                                          'y' : ycoord,
-                                          'x' : xcoord},
-                                  attrs={'comment': v.comment,
-                                         'storage': v.storage})
-
-            variables.append(da)
-
-#    variables = {v.name: (['time','lev','lat','lon'], binData[m])
-#                 for m,v in enumerate(ctl.vdef)}
-
-    dset = xr.merge(variables)
-
-    dset.attrs['title'] = ctl.title
-    dset.attrs['undef'] = ctl.undef
-    dset.attrs['pdef' ] = 'None'
-
-    if ctl.pdef:
-        dset.attrs['pdef' ] = ctl.pdef.proj
-
-    if returnctl:
-        return dset, ctl
-    else:
-        return dset
-
-
-
-"""
-Helper (private) methods are defined below
-"""
-def __read_as_dask(dd):
-    """Read binary data and return as a dask array
-
-    Parameters
-    ----------
-    dd: CtlDescriptor
-        A CtlDescriptor
-
-    Returns
-    -------
-    re: dask.array
-        Data viewed as `dask.array`.
-    """
-    if dd.pdef is None:
-        t, y, x = dd.tdef.length(), dd.ydef.length(), dd.xdef.length()
-    else:
-        t, y, x = dd.tdef.length(), dd.pdef.jsize, dd.pdef.isize
-
-    totalNum = sum([reduce(lambda x, y:
-                    x*y, (t,v.zcount,y,x)) for v in dd.vdef])
-
-    if dd.sequential:
-        sequentialSize = x * y + 2
-    else:
-        sequentialSize = -1
-
-    # print(totalNum * 4.0 / 1024.0 / 1024.0)
-
-    binData = []
-
-    dtype   = '<f4' if dd.byteOrder == 'little' else '>f4'
-
-    for m, v in enumerate(dd.vdef):
-        name = '@miniufo_' + tokenize(v, m)
-
-        if totalNum < (100 * 100 * 100 * 10): # about 40 MB, chunk all
-            # print('small')
-            chunk = (t, v.zcount, y, x)
-            shape = (t, v.zcount, y, x)
-
-            dsk = {(name, 0, 0, 0, 0):
-                   (__read_var, dd.dsetPath, v, dd.tRecLength,
-                    None, None, dtype, sequentialSize)}
-
-            binData.append(dsa.Array(dsk, name, chunk,
-                                     dtype=dtype, shape=shape))
-
-        elif totalNum > (200 * 100 * 100 * 100): # about 800 MB, chunk 2D slice
-            # print('large')
-            chunk = (1, 1, y, x)
-            shape = (t, v.zcount, y, x)
-
-            dsk = {(name, l, k, 0, 0):
-                   (__read_var, dd.dsetPath, v, dd.tRecLength,
-                    l, k, dtype, sequentialSize)
-                   for l in range(t)
-                   for k in range(v.zcount)}
-
-            binData.append(dsa.Array(dsk, name, chunk,
-                                     dtype=dtype, shape=shape))
-
-        else: # in between, chunk 3D slice
-            # print('between')
-            chunk = (1, v.zcount, y, x)
-            shape = (t, v.zcount, y, x)
-
-            dsk = {(name, l, 0, 0, 0):
-                   (__read_var, dd.dsetPath, v, dd.tRecLength,
-                    l, None, dtype, sequentialSize)
-                   for l in range(t)}
-
-            binData.append(dsa.Array(dsk, name, chunk,
-                                     dtype=dtype, shape=shape))
-
-    return binData
-
-
-def __read_template_as_dask(dd, tcPerf):
-    """Read template binary data and return as a dask array
-
-    Parameters
-    ----------
-    dd: CtlDescriptor
-        A CtlDescriptor
-    tcPerf: list of int
-        Number of time count per file
-
-    Returns
-    -------
-    re: list of dask.array
-        Data viewed as `dask.array`.
-    """
-    if dd.pdef is None:
-        t, y, x = dd.tdef.length(), dd.ydef.length(), dd.xdef.length()
-    else:
-        t, y, x = dd.tdef.length(), dd.pdef.jsize, dd.pdef.isize
-
-    totalNum = sum([reduce(lambda x, y:
-                    x*y, (tcPerf[0],v.zcount,y,x)) for v in dd.vdef])
-
-    if dd.sequential:
-        sequentialSize = x * y + 2
-    else:
-        sequentialSize = -1
-
-    # print(totalNum * 4.0 / 1024.0 / 1024.0)
-
-    binData = []
-
-    dtype   = '<f4' if dd.byteOrder == 'little' else '>f4'
-
-    for m, v in enumerate(dd.vdef):
-        name = '@miniufo_' + tokenize(v, m)
-
-        if totalNum > (200 * 100 * 100 * 100): # about 800 MB, chunk 2D slice
-            # print('large')
-            chunk = (1, 1, y, x)
-            shape = (t, v.zcount, y, x)
-
-            dsk = {(name, l + sum(tcPerf[:m]), k, 0, 0):
-                   (__read_var, f, v, dd.tRecLength,
-                    l, k, dtype, sequentialSize)
-                   for m, f in enumerate(dd.dsetPath[:len(tcPerf)])
-                   for l in range(tcPerf[m])
-                   for k in range(v.zcount)}
-
-            binData.append(dsa.Array(dsk, name, chunk,
-                                     dtype=dtype, shape=shape))
-
-        else: # in between, chunk 3D slice
-            # print('between')
-            chunk = (1, v.zcount, y, x)
-            shape = (t, v.zcount, y, x)
-
-            dsk = {(name, l + sum(tcPerf[:m]), 0, 0, 0):
-                   (__read_var, f, v, dd.tRecLength,
-                    l, None, dtype, sequentialSize)
-                   for m, f in enumerate(dd.dsetPath[:len(tcPerf)])
-                   for l in range(tcPerf[m])}
-
-            binData.append(dsa.Array(dsk, name, chunk,
-                                     dtype=dtype, shape=shape))
-
-    return binData
-
-
-def __read_var(file, var, tstride, tstep, zstep, dtype, sequentialSize=-1):
-    """Read a variable given the trange
-
-    Parameters
-    ----------
-    file: str
-        A file from which data are read.
-    var: CtlVar
-        A variable that need to be read.
-    tstride: int
-        Stride of a single time record.
-    tstep: int
-        T-step to be read, started from 0.  If None, read all t-steps
-    zstep: int
-        Z-step to be read, started from 0.  If None, read all z-steps
-    sequentialSize: int
-        Size of the sequential block (= y * x).  Default of -1 means
-        non-sequential storage.
-
-    Returns
-    -------
-    re: numpy.ndarray
-        Binary data.
-    """
-    # print(var.name+' '+str(tstep)+' '+str(zstep)+' '+str(var.strPos))
-
-    if var.storage == '-1,20':
-        if tstep is None and zstep is None:
-            shape = (var.tcount, var.zcount, var.ycount, var.xcount)
-            if sequentialSize != -1:
-                seqShp = (var.tcount, var.zcount, sequentialSize)
-            else:
-                seqShp = shape
-            pos   = var.strPos
-            return __read_continuous(file, pos, shape, dtype,
-                                     sequentialShape=seqShp)
-
-        elif zstep is None and tstep is not None:
-            shape = (1, var.zcount, var.ycount, var.xcount)
-            if sequentialSize != -1:
-                seqShp = (1, var.zcount, sequentialSize)
-            else:
-                seqShp = shape
-            pos   = var.strPos
-            return __read_continuous(file, pos, shape, dtype,
-                                     sequentialShape=seqShp)
-
-        elif tstep is None and zstep is not None:
-            raise Exception('not implemented in -1,20')
-
-        else:
-            shape = (1, 1, var.ycount, var.xcount)
-            zstri = var.ycount * var.xcount * 4
-            if sequentialSize != -1:
-                seqShp = (1, 1, sequentialSize)
-                zstri += 8
-            else:
-                seqShp = shape
-            pos   = var.strPos + zstri * zstep
-            return __read_continuous(file, pos, shape, dtype,
-                                     sequentialShape=seqShp)
-
-    elif var.storage in ['99', '0', '00', '000', '1', '11', '111']:
-    # elif var.storage == '99' or var.storage == '0':
-        if tstep is None and zstep is None:
-            shape = (1, var.zcount, var.ycount, var.xcount)
-            if sequentialSize != -1:
-                seqShp = (1, var.zcount, sequentialSize)
-            else:
-                seqShp = shape
-            pos   = var.strPos
-            data  = []
-
-            for l in range(var.tcount):
-                data.append(__read_continuous(file, pos, shape, dtype,
-                                              sequentialShape=seqShp))
-                pos += tstride
-
-            return np.concatenate(data)
-
-        elif zstep is None and tstep is not None:
-            shape = (1, var.zcount, var.ycount, var.xcount)
-            if sequentialSize != -1:
-                seqShp = (1, var.zcount, sequentialSize)
-            else:
-                seqShp = shape
-            pos   = var.strPos + tstride * tstep
-            data = __read_continuous(file, pos, shape, dtype,
-                                     sequentialShape=seqShp)
-
-            return data
-
-        elif tstep is None and zstep is not None:
-            raise Exception('not implemented in 0,99')
-
-        else:
-            shape = (1, 1, var.ycount, var.xcount)
-            zstri = var.ycount * var.xcount * 4
-            if sequentialSize != -1:
-                seqShp = (1, 1, sequentialSize)
-                zstri += 8
-            else:
-                seqShp = shape
-            pos   = var.strPos + tstride * tstep + zstri * zstep
-            return __read_continuous(file, pos, shape, dtype,
-                                     sequentialShape=seqShp)
-
-    else:
-        raise Exception('invalid storage ' + var.storage +
-                        ', only "99" or "-1,20" are supported')
-
-
-def __read_continuous(file, offset=0, shape=None, dtype='<f4',
-                      use_mmap=True, sequentialShape=None):
-    """
-    Read a block of continuous data into the memory.
-
-    Parameters
-    ----------
-    file  : str
-        A file from which data are read.
-    offset: int
-        An offset where the read is started.
-    shape : tuple
-        A tuple indicate shape of the Array returned.
-    sequentialShape : tuple
-        If in Fortran-sequential storage, provide a shape including the
-        beginning and the end numbers.
-
-    Returns
-    -------
-    re: numpy.ndarray
-        Binary data.
-    """
-    with open(file, 'rb') as f:
-        if use_mmap:
-            data = np.memmap(f, dtype=dtype, mode='r', offset=offset,
-                             shape=sequentialShape, order='C')
-        else:
-            number_of_values = reduce(lambda x, y: x*y, sequentialShape)
-
-            f.seek(offset)
-            data = np.fromfile(f, dtype=dtype, count=number_of_values)
-
-    if sequentialShape != shape:
-        data = data.reshape((shape[0],shape[1],-1))[:,:,1:-1]
-
-    data = data.reshape(shape, order='C')
-
-    data.shape = shape
-
-    return data
+# -*- coding: utf-8 -*-
+"""
+Created on 2020.04.11
+
+@author: MiniUFO
+Copyright 2018. All rights reserved. Use is subject to license terms.
+"""
+import os
+import numpy as np
+import xarray as xr
+import dask.array as dsa
+from dask.base import tokenize
+from glob import glob
+from pathlib import Path
+from .core import CtlDescriptor
+from functools import reduce
+
+"""
+IO related functions here
+"""
+def open_mfdataset(paths, parallel=False, encoding='GBK'):
+    """Open multiple ctl files as a single dataset
+    
+    This is similar to `xarray.open_mfdataset()` that can simutaneously open
+    a series of ctl files that are in similar spatial ranges but of different
+    temporal ranges.
+
+    Parameters
+    ----------
+    paths: str or sequence
+        Either a string glob in the form ``"path/to/my/files/*.ctl"`` or an
+        explicit list of files to open. Paths can be given as strings or as
+        pathlib Paths.
+    parallel: bool, optional
+        If True, the open and preprocess steps of this function will be
+        performed in parallel using ``dask.delayed``. Default is False.
+    encoding: str
+        Encoding for the ctl file content e.g., ['GBK', 'UTF-8'].
+
+    Returns
+    -------
+    re: xarray.Dataset
+        A dataset.
+
+    Notes
+    -----
+    ``open_mfdataset`` opens files with read-only access. When you modify values
+    of a Dataset, even one linked to files on disk, only the in-memory copy you
+    are manipulating in xarray is modified: the original file on disk is never
+    touched.
+    """
+    if isinstance(paths, str):
+        paths = sorted(glob(paths))
+    else:
+        paths = [str(p) if isinstance(p, Path) else p for p in paths]
+
+    if not paths:
+        raise OSError("no files to open")
+
+    if parallel:
+        import dask
+
+        # wrap the open_dataset
+        open_ = dask.delayed(open_CtlDataset)
+    else:
+        open_ = open_CtlDataset
+
+    datasets = [open_(p, encoding=encoding) for p in paths]
+
+    if parallel:
+        # calling compute here will return the datasets/file_objs lists,
+        # the underlying datasets will still be stored as dask arrays
+        datasets = dask.compute(datasets)
+
+        return xr.concat(datasets[0], dim='time')
+
+    combined = xr.concat(datasets, dim='time')
+
+    return combined
+
+
+def open_CtlDataset(desfile, returnctl=False, encoding='GBK'):
+    """Open a single ctl dataset
+    
+    Open a 4D dataset with a descriptor file end with .ctl and
+    return a xarray.Dataset.  This also uses the dask to chunk
+    very large dataset, which is similar to the xarray.open_dataset.
+
+    Parameters
+    ----------
+    desfile: string
+        Path to the descriptor file end with .ctl or .cts
+    returnctl: bool
+        Return dset and ctl as a tuple
+
+    Returns
+    -------
+    dset: xarray.Dataset
+        Dataset object containing all coordinates and variables.
+    ctl: xgrads.CtlDescriptor
+        Ctl descriptor file if returnctl == True.
+    """
+    if isinstance(desfile, str):
+        if not desfile.endswith('.ctl'):
+            raise Exception('unsupported file, suffix should be .ctl')
+
+        ctl = CtlDescriptor(encoding=encoding, file=desfile)
+    elif isinstance(desfile, CtlDescriptor):
+        ctl = desfile
+    else:
+        raise Exception('unsupported type of input ('+str(type(desfile))+'), ' +
+                        '[CtlDescriptor or str] are allowed')
+
+    if ctl.template:
+        if ctl.edef:
+            raise Exception('template and EDEF are not simultaneously supported yet')
+        
+        tcount = len(ctl.tdef.samples) # number of total time count
+        tcPerf = []                    # number of time count per file
+        
+        has_missing = False
+        for file in ctl.dsetPath:
+            if os.path.exists(file):
+                fsize = os.path.getsize(file)
+    
+                if fsize % ctl.tRecLength != 0:
+                    raise Exception('incomplete file for ' + file +
+                                    ' (not multiple of ' + str(ctl.tRecLength) +
+                                    ' bytes)')
+    
+                tcPerf.append(fsize // ctl.tRecLength)
+            else:
+                print(' warning: ' + file + ' is missing...')
+                has_missing = True
+        
+        if has_missing:
+            raise Exception('there are missing binary files')
+
+        total_size = sum(tcPerf)
+
+        if total_size < tcount:
+            raise Exception('no enough files for ' + str(tcount) +
+                            ' time records')
+
+        # get time record number in each file
+        rem = tcount
+        idx = 0
+        for i, num in enumerate(tcPerf):
+            rem -= num
+            if rem <= 0:
+                idx = i
+                break
+
+        tcPerf_m      = tcPerf[:idx+1]
+        tcPerf_m[idx] = tcPerf[idx   ] + rem
+
+        # print(ctl.dsetPath)
+        # print(tcPerf)
+        # print(tcPerf_m)
+
+        binData = __read_template_as_dask(ctl, tcPerf_m)
+
+    else:
+        if ctl.edef == None:
+            expect = ctl.tRecLength * ctl.tdef.length()
+        else:
+            expect = 0
+            for ens in ctl.edef:
+                expect += ens.tcount * ctl.tRecLength
+        
+        actual = os.path.getsize(ctl.dsetPath)
+
+        if expect != actual:
+            print('WARNING: expected binary file size: {0}, actual size: {1}'
+                            .format(expect, actual))
+
+        binData = __read_as_dask(ctl)
+
+    variables = []
+
+    if ctl.pdef is None:
+        for m, v in enumerate(ctl.vdef):
+            if v.dependZ:
+                if ctl.edef:
+                    data = binData[m]
+                    dims = ['ens', 'time', 'lev', 'lat', 'lon']
+                    coords = {'ens' : [ens.name for ens in ctl.edef],
+                              'time': ctl.tdef.samples[:],
+                              'lev' : ctl.zdef.samples[:v.zcount],
+                              'lat' : ctl.ydef.samples[:],
+                              'lon' : ctl.xdef.samples[:]}
+                else:
+                    data = binData[m]
+                    dims = ['time', 'lev', 'lat', 'lon']
+                    coords = {'time': ctl.tdef.samples[:],
+                              'lev' : ctl.zdef.samples[:v.zcount],
+                              'lat' : ctl.ydef.samples[:],
+                              'lon' : ctl.xdef.samples[:]}
+            else:
+                if ctl.edef:
+                    e, t, z, y, x = binData[m].shape
+                    data = binData[m].reshape((e,t,y,x))
+                    dims = ['ens', 'time', 'lat', 'lon']
+                    coords = {'ens' : [ens.name for ens in ctl.edef],
+                              'time': ctl.tdef.samples[:],
+                              'lat' : ctl.ydef.samples[:],
+                              'lon' : ctl.xdef.samples[:]}
+                else:
+                    t, z, y, x = binData[m].shape
+                    data = binData[m].reshape((t,y,x))
+                    dims = ['time', 'lat', 'lon']
+                    coords = {'time': ctl.tdef.samples[:],
+                              'lat' : ctl.ydef.samples[:],
+                              'lon' : ctl.xdef.samples[:]}
+            
+            da = xr.DataArray(name=v.name, data=data, dims=dims, coords=coords,
+                              attrs={'comment': v.comment,
+                                     'storage': v.storage})
+            variables.append(da)
+
+    else:
+        PDEF = ctl.pdef
+
+        if PDEF.proj in ['lcc', 'lccr']:
+            ycoord = np.linspace(0, (PDEF.jsize-1) * PDEF.dx, PDEF.jsize)
+            xcoord = np.linspace(0, (PDEF.isize-1) * PDEF.dy, PDEF.isize)
+
+        elif PDEF.proj in ['sps', 'nps']:
+            inc = PDEF.gridinc * 1000 # change unit from km to m
+            ycoord = np.linspace(-(PDEF.jpole), (PDEF.jsize-PDEF.jpole),
+                                   PDEF.jsize) * inc
+            xcoord = np.linspace(-(PDEF.ipole), (PDEF.isize-PDEF.ipole),
+                                   PDEF.isize) * inc
+
+        for m, v in enumerate(ctl.vdef):
+            if v.dependZ:
+                if ctl.edef:
+                    data = binData[m]
+                    dims = ['ens', 'time', 'lev', 'y', 'x']
+                    coords = {'ens' : [ens.name for ens in ctl.edef],
+                              'time': ctl.tdef.samples[:],
+                              'lev' : ctl.zdef.samples[:v.zcount],
+                              'y'   : ycoord,
+                              'x'   : xcoord}
+                else:
+                    data = binData[m]
+                    dims = ['time', 'lev', 'y', 'x']
+                    coords = {'time': ctl.tdef.samples[:],
+                              'lev' : ctl.zdef.samples[:v.zcount],
+                              'y' : ycoord,
+                              'x' : xcoord}
+            else:
+                if ctl.edef:
+                    e, t, z, y, x = binData[m].shape
+                    data = binData[m].reshape((e,t,y,x))
+                    dims = ['ens', 'time', 'y', 'x']
+                    coords = {'ens' : [ens.name for ens in ctl.edef],
+                              'time': ctl.tdef.samples[:],
+                              'y' : ycoord,
+                              'x' : xcoord}
+                else:
+                    t, z, y, x = binData[m].shape
+                    data = binData[m].reshape((t,y,x))
+                    dims = ['time', 'y', 'x']
+                    coords = {'time': ctl.tdef.samples[:],
+                              'y' : ycoord,
+                              'x' : xcoord}
+
+            da = xr.DataArray(name=v.name, data=data, dims=dims, coords=coords,
+                              attrs={'comment': v.comment,
+                                     'storage': v.storage})
+            variables.append(da)
+
+#    variables = {v.name: (['time','lev','lat','lon'], binData[m])
+#                 for m,v in enumerate(ctl.vdef)}
+
+    dset = xr.merge(variables)
+
+    dset.attrs['title'] = ctl.title
+    dset.attrs['undef'] = ctl.undef
+    dset.attrs['pdef' ] = 'None'
+
+    if ctl.pdef:
+        dset.attrs['pdef' ] = ctl.pdef.proj
+
+    if returnctl:
+        return dset, ctl
+    else:
+        return dset
+
+
+
+"""
+Helper (private) methods are defined below
+"""
+def __read_as_dask(dd):
+    """Read binary data and return as a dask array
+
+    Parameters
+    ----------
+    dd: CtlDescriptor
+        A CtlDescriptor
+
+    Returns
+    -------
+    re: dask.array
+        Data viewed as `dask.array`.
+    """
+    if dd.pdef is None:
+        t, y, x = dd.tdef.length(), dd.ydef.length(), dd.xdef.length()
+    else:
+        t, y, x = dd.tdef.length(), dd.pdef.jsize, dd.pdef.isize
+
+    totalNum = sum([reduce(lambda x, y:
+                    x*y, (t,v.zcount,y,x)) for v in dd.vdef])
+
+    if dd.sequential:
+        sequentialSize = x * y + 2
+    else:
+        sequentialSize = -1
+
+    # print(totalNum * 4.0 / 1024.0 / 1024.0)
+
+    binData = []
+
+    dtype   = '<f4' if dd.byteOrder == 'little' else '>f4'
+
+    for m, v in enumerate(dd.vdef):
+        name = '@miniufo_' + tokenize(v, m)
+
+        if totalNum < (100 * 100 * 100 * 10): # about 40 MB, chunk all
+            # print('small')
+            if dd.edef == None:
+                chunk = (t, v.zcount, y, x)
+                shape = (t, v.zcount, y, x)
+    
+                dsk = {(name, 0, 0, 0, 0):
+                       (__read_var, dd.dsetPath, v, 0, dd.tRecLength,
+                        None, None, dtype, sequentialSize)}
+            else:
+                e = len(dd.edef)
+                chunk = (1, t, v.zcount, y, x)
+                shape = (e, t, v.zcount, y, x)
+    
+                dsk = {(name, n, 0, 0, 0, 0):
+                       (__read_var, dd.dsetPath, v, ens.strPos, dd.tRecLength,
+                        None, None, dtype, sequentialSize)
+                       for n, ens in enumerate(dd.edef)}
+
+            binData.append(dsa.Array(dsk, name, chunk,
+                                     dtype=dtype, shape=shape))
+
+        elif totalNum > (200 * 100 * 100 * 100): # about 800 MB, chunk 2D slice
+            # print('large')
+            if dd.edef == None:
+                chunk = (1, 1, y, x)
+                shape = (t, v.zcount, y, x)
+
+                dsk = {(name, l, k, 0, 0):
+                       (__read_var, dd.dsetPath, v, 0, dd.tRecLength,
+                        l, k, dtype, sequentialSize)
+                       for l in range(t)
+                       for k in range(v.zcount)}
+            else:
+                e = len(dd.edef)
+                chunk = (1, 1, 1, y, x)
+                shape = (e, t, v.zcount, y, x)
+
+                dsk = {(name, n, l, k, 0, 0):
+                       (__read_var, dd.dsetPath, v, ens.strPos, dd.tRecLength,
+                        l, k, dtype, sequentialSize)
+                       for n, ens in enumerate(dd.edef)
+                       for l in range(t)
+                       for k in range(v.zcount)}
+
+            binData.append(dsa.Array(dsk, name, chunk,
+                                     dtype=dtype, shape=shape))
+
+
+        else: # in between, chunk 3D slice
+            # print('between')
+            if dd.edef == None:
+                chunk = (1, v.zcount, y, x)
+                shape = (t, v.zcount, y, x)
+    
+                dsk = {(name, l, 0, 0, 0):
+                       (__read_var, dd.dsetPath, v, 0, dd.tRecLength,
+                        l, None, dtype, sequentialSize)
+                       for l in range(t)}
+            else:
+                e = len(dd.edef)
+                chunk = (1, 1, v.zcount, y, x)
+                shape = (e, t, v.zcount, y, x)
+    
+                dsk = {(name, n, l, 0, 0, 0):
+                       (__read_var, dd.dsetPath, v, ens.strPos, dd.tRecLength,
+                        l, None, dtype, sequentialSize)
+                       for n, ens in enumerate(dd.edef)
+                       for l in range(t)}
+
+            binData.append(dsa.Array(dsk, name, chunk,
+                                     dtype=dtype, shape=shape))
+
+    return binData
+
+
+def __read_template_as_dask(dd, tcPerf):
+    """Read template binary data and return as a dask array
+
+    Parameters
+    ----------
+    dd: CtlDescriptor
+        A CtlDescriptor
+    tcPerf: list of int
+        Number of time count per file
+
+    Returns
+    -------
+    re: list of dask.array
+        Data viewed as `dask.array`.
+    """
+    if dd.pdef is None:
+        t, y, x = dd.tdef.length(), dd.ydef.length(), dd.xdef.length()
+    else:
+        t, y, x = dd.tdef.length(), dd.pdef.jsize, dd.pdef.isize
+
+    totalNum = sum([reduce(lambda x, y:
+                    x*y, (tcPerf[0],v.zcount,y,x)) for v in dd.vdef])
+
+    if dd.sequential:
+        sequentialSize = x * y + 2
+    else:
+        sequentialSize = -1
+
+    # print(totalNum * 4.0 / 1024.0 / 1024.0)
+
+    binData = []
+
+    dtype   = '<f4' if dd.byteOrder == 'little' else '>f4'
+
+    for m, v in enumerate(dd.vdef):
+        name = '@miniufo_' + tokenize(v, m)
+
+        if totalNum > (200 * 100 * 100 * 100): # about 800 MB, chunk 2D slice
+            # print('large')
+            chunk = (1, 1, y, x)
+            shape = (t, v.zcount, y, x)
+
+            dsk = {(name, l + sum(tcPerf[:m]), k, 0, 0):
+                   (__read_var, f, v, 0, dd.tRecLength,
+                    l, k, dtype, sequentialSize)
+                   for m, f in enumerate(dd.dsetPath[:len(tcPerf)])
+                   for l in range(tcPerf[m])
+                   for k in range(v.zcount)}
+
+            binData.append(dsa.Array(dsk, name, chunk,
+                                     dtype=dtype, shape=shape))
+
+        else: # in between, chunk 3D slice
+            # print('between')
+            chunk = (1, v.zcount, y, x)
+            shape = (t, v.zcount, y, x)
+
+            dsk = {(name, l + sum(tcPerf[:m]), 0, 0, 0):
+                   (__read_var, f, v, 0, dd.tRecLength,
+                    l, None, dtype, sequentialSize)
+                   for m, f in enumerate(dd.dsetPath[:len(tcPerf)])
+                   for l in range(tcPerf[m])}
+
+            binData.append(dsa.Array(dsk, name, chunk,
+                                     dtype=dtype, shape=shape))
+
+    return binData
+
+
+def __read_var(file, var, epos, tstride, tstep, zstep, dtype, sequentialSize=-1):
+    """Read a variable given the trange
+
+    Parameters
+    ----------
+    file: str
+        A file from which data are read.
+    var: CtlVar
+        A variable that need to be read.
+    epos: int
+        Position of the ensemble dimension
+    tstride: int
+        Stride of a single time record.
+    tstep: int
+        T-step to be read, started from 0.  If None, read all t-steps
+    zstep: int
+        Z-step to be read, started from 0.  If None, read all z-steps
+    sequentialSize: int
+        Size of the sequential block (= y * x).  Default of -1 means
+        non-sequential storage.
+
+    Returns
+    -------
+    re: numpy.ndarray
+        Binary data.
+    """
+    # print(var.name+' '+str(tstep)+' '+str(zstep)+' '+str(var.strPos))
+
+    if var.storage == '-1,20':
+        if tstep is None and zstep is None:
+            shape = (var.tcount, var.zcount, var.ycount, var.xcount)
+            if sequentialSize != -1:
+                seqShp = (var.tcount, var.zcount, sequentialSize)
+            else:
+                seqShp = shape
+            pos   = var.strPos + epos
+            return __read_continuous(file, pos, shape, dtype,
+                                     sequentialShape=seqShp)
+
+        elif zstep is None and tstep is not None:
+            shape = (1, var.zcount, var.ycount, var.xcount)
+            if sequentialSize != -1:
+                seqShp = (1, var.zcount, sequentialSize)
+            else:
+                seqShp = shape
+            pos   = var.strPos + epos
+            return __read_continuous(file, pos, shape, dtype,
+                                     sequentialShape=seqShp)
+
+        elif tstep is None and zstep is not None:
+            raise Exception('not implemented in -1,20')
+
+        else:
+            shape = (1, 1, var.ycount, var.xcount)
+            zstri = var.ycount * var.xcount * 4
+            if sequentialSize != -1:
+                seqShp = (1, 1, sequentialSize)
+                zstri += 8
+            else:
+                seqShp = shape
+            pos   = var.strPos + zstri * zstep + epos
+            return __read_continuous(file, pos, shape, dtype,
+                                     sequentialShape=seqShp)
+
+    elif var.storage in ['99', '0', '00', '000', '1', '11', '111']:
+    # elif var.storage == '99' or var.storage == '0':
+        if tstep is None and zstep is None:
+            shape = (1, var.zcount, var.ycount, var.xcount)
+            if sequentialSize != -1:
+                seqShp = (1, var.zcount, sequentialSize)
+            else:
+                seqShp = shape
+            pos   = var.strPos + epos
+            data  = []
+
+            for l in range(var.tcount):
+                data.append(__read_continuous(file, pos, shape, dtype,
+                                              sequentialShape=seqShp))
+                pos += tstride
+
+            return np.concatenate(data)
+
+        elif zstep is None and tstep is not None:
+            shape = (1, var.zcount, var.ycount, var.xcount)
+            if sequentialSize != -1:
+                seqShp = (1, var.zcount, sequentialSize)
+            else:
+                seqShp = shape
+            pos   = var.strPos + tstride * tstep + epos
+            data = __read_continuous(file, pos, shape, dtype,
+                                     sequentialShape=seqShp)
+
+            return data
+
+        elif tstep is None and zstep is not None:
+            raise Exception('not implemented in 0,99')
+
+        else:
+            shape = (1, 1, var.ycount, var.xcount)
+            zstri = var.ycount * var.xcount * 4
+            if sequentialSize != -1:
+                seqShp = (1, 1, sequentialSize)
+                zstri += 8
+            else:
+                seqShp = shape
+            pos   = var.strPos + tstride * tstep + zstri * zstep + epos
+            return __read_continuous(file, pos, shape, dtype,
+                                     sequentialShape=seqShp)
+
+    else:
+        raise Exception('invalid storage ' + var.storage +
+                        ', only "99" or "-1,20" are supported')
+
+
+def __read_continuous(file, offset=0, shape=None, dtype='<f4',
+                      use_mmap=True, sequentialShape=None):
+    """
+    Read a block of continuous data into the memory.
+
+    Parameters
+    ----------
+    file  : str
+        A file from which data are read.
+    offset: int
+        An offset where the read is started.
+    shape : tuple
+        A tuple indicate shape of the Array returned.
+    sequentialShape : tuple
+        If in Fortran-sequential storage, provide a shape including the
+        beginning and the end numbers.
+
+    Returns
+    -------
+    re: numpy.ndarray
+        Binary data.
+    """
+    with open(file, 'rb') as f:
+        if use_mmap:
+            data = np.memmap(f, dtype=dtype, mode='r', offset=offset,
+                             shape=sequentialShape, order='C')
+        else:
+            number_of_values = reduce(lambda x, y: x*y, sequentialShape)
+
+            f.seek(offset)
+            data = np.fromfile(f, dtype=dtype, count=number_of_values)
+
+    if sequentialShape != shape:
+        data = data.reshape((shape[0],shape[1],-1))[:,:,1:-1]
+
+    data = data.reshape(shape, order='C')
+
+    data.shape = shape
+
+    return data
```

### Comparing `xgrads-0.2.3/xgrads.egg-info/PKG-INFO` & `xgrads-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,118 @@
 Metadata-Version: 2.1
 Name: xgrads
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse and read ctl file commonly used by GrADS.
 Home-page: https://github.com/miniufo/xgrads
 Author: miniufo
 Author-email: miniufo@163.com
 License: MIT
 Keywords: grads opengrads xarray dask
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# xgrads
-
-[![DOI](https://zenodo.org/badge/244529165.svg)](https://zenodo.org/badge/latestdoi/244529165)
-![GitHub](https://img.shields.io/github/license/miniufo/xgrads)
-[![Documentation Status](https://readthedocs.org/projects/xgrads/badge/?version=latest)](https://xgrads.readthedocs.io/en/latest/?badge=latest)
-
-
-![3D plot](https://raw.githubusercontent.com/miniufo/xgrads/master/pics/3D.png)
-
-
-## 1. Introduction
-The Grid Analysis and Display System ([GrADS](http://cola.gmu.edu/grads/) or [OpenGrADS](http://www.opengrads.org/)) is a widely used software for easy access, manipulation, and visualization of earth science data.  It uses a [descriptor (or control) file with a suffix `.ctl`](http://cola.gmu.edu/grads/gadoc/descriptorfile.html) to  describe a raw binary 4D dataset.  The `ctl` file is similar to the header information of a [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html) file, containing all the information about dimensions, attributes, and variables except for the variable data.
-
-This python package [`xgrads`](https://github.com/miniufo/xgrads) is designed for parse and read the `.ctl` file commonly used by [GrADS](http://cola.gmu.edu/grads/).  Right now it can parse various kinds of `.ctl` files.  However, only the commonly used raw binary 4D datasets can be read using [`dask`](https://dask.org/) and return as a [`xarray.Dataset`](http://xarray.pydata.org/en/stable/)  Other types of binary data, like `dtype` is `station` or`grib`, may be supported in the future.
-
----
-## 2. How to install
-**Requirements**
-`xgrads` is developed under the environment with `xarray` (=version 0.15.0), `dask` (=version 2.11.0), `numpy` (=version 1.15.4), `cartopy` (=version 0.17.0), and `pyproj` (=version 1.9.6).  Older versions of these packages are not well tested.
-
-**Install via pip**
-```
-pip install xgrads
-```
-
-**Install from github**
-```
-git clone https://github.com/miniufo/xgrads.git
-cd xgrads
-python setup.py install
-```
-
-
----
-## 3. Examples
-### 3.1 Parse a `.ctl` file
-Parsing a `.ctl` file is pretty simple using the following code:
-```python
-from xgrads import CtlDescriptor
-
-ctl = CtlDescriptor(file='test.ctl')
-
-# print all the info in ctl file
-print(ctl)
-```
-
-If you have already load the ASCII content in the `.ctl` file, you can do it as:
-```python
-content = \
-    "dset ^binary.dat\n" \
-    "* this is a comment line\n" \
-    "title 10-deg resolution model\n" \
-    "undef -9.99e8\n" \
-    "xdef 36 linear   0 10\n" \
-    "ydef 19 linear -90 10\n" \
-    "zdef  1 linear   0  1\n" \
-    "tdef  1 linear 00z01Jan2000 1dy\n" \
-    "vars  1\n" \
-    "test  1 99 test variable\n" \
-    "endvars\n"
-
-ctl = CtlDescriptor(content=content)
-
-# print all the info
-print(ctl)
-```
----
-
-### 3.2 Read binary data into a `xarray.Dataset`
-Reading a `.ctl` related binary data file is also pretty simple using the following code:
-```python
-from xgrads import open_CtlDataset
-
-dset = open_CtlDataset('test.ctl')
-
-# print all the info in ctl file
-print(dset)
-```
-
-Then you have the `dset` as a `xarray.Dataset`.  This is similar to [`xarray.open_dataset`](http://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html) that use [`dask`](https://dask.org/) to chunk (buffer) parts of the whole dataset in physical memory if the whole dataset is too large to fit in.
-
-If there are many `.ctl` files in a folder, we can also open all of them in a single call of `open_mfdataset` as:
-```python
-from xgrads import open_mfDataset
-
-dset = open_mfDataset('./folder/*.ctl')
-
-# print all the info in ctl file
-print(dset)
-```
-assuming that every `.ctl` file has similar data structure except the time step is different.  This is similar to [`xarray.open_mfdataset`](http://xarray.pydata.org/en/v0.12.3/generated/xarray.open_mfdataset.html).
-
----
-
-### 3.3 Convert a GrADS dataset to a NetCDF dataset
-With the above functionality, it is easy to convert a `.ctl` ([GrADS](http://cola.gmu.edu/grads/)) dataset to a `.nc` ([NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html)) dataset:
-```python
-from xgrads import open_CtlDataset
-
-open_CtlDataset('input.ctl').to_netcdf('output.nc')
-```
+# xgrads
+
+[![DOI](https://zenodo.org/badge/244529165.svg)](https://zenodo.org/badge/latestdoi/244529165)
+![GitHub](https://img.shields.io/github/license/miniufo/xgrads)
+[![Documentation Status](https://readthedocs.org/projects/xgrads/badge/?version=latest)](https://xgrads.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/xgrads.svg)](https://badge.fury.io/py/xgrads)
+![Workflow](https://github.com/miniufo/xgrads/actions/workflows/python-publish.yml/badge.svg)
+[![pytest](https://github.com/miniufo/xgrads/actions/workflows/tests.yml/badge.svg)](https://github.com/miniufo/xgrads/actions/workflows/tests.yml)
+[![Build Status](https://app.travis-ci.com/miniufo/xgrads.svg?branch=master)](https://app.travis-ci.com/miniufo/xgrads)
+
+![3D plot](https://raw.githubusercontent.com/miniufo/xgrads/master/pics/3D.png)
+
+
+## 1. Introduction
+The Grid Analysis and Display System ([GrADS](http://cola.gmu.edu/grads/) or [OpenGrADS](http://www.opengrads.org/)) is a widely used software for easy access, manipulation, and visualization of earth science data.  It uses a [descriptor (or control) file with a suffix `.ctl`](http://cola.gmu.edu/grads/gadoc/descriptorfile.html) to  describe a raw binary 4D dataset.  The `ctl` file is similar to the header information of a [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html) file, containing all the information about dimensions, attributes, and variables except for the variable data.
+
+This python package [`xgrads`](https://github.com/miniufo/xgrads) is designed for parse and read the `.ctl` file commonly used by [GrADS](http://cola.gmu.edu/grads/).  Right now it can parse various kinds of `.ctl` files.  However, only the commonly used raw binary 4D datasets can be read using [`dask`](https://dask.org/) and return as a [`xarray.Dataset`](http://xarray.pydata.org/en/stable/)  Other types of binary data, like `dtype` is `station` or`grib`, may be supported in the future.
+
+---
+## 2. How to install
+**Requirements**
+`xgrads` is developed under the environment with `xarray` (=version 0.15.0), `dask` (=version 2.11.0), `numpy` (=version 1.15.4), `cartopy` (=version 0.17.0), and `pyproj` (=version 1.9.6).  Older versions of these packages are not well tested.
+
+**Install via pip**
+```
+pip install xgrads
+```
+
+**Install from github**
+```
+git clone https://github.com/miniufo/xgrads.git
+cd xgrads
+python setup.py install
+```
+
+
+---
+## 3. Examples
+### 3.1 Parse a `.ctl` file
+Parsing a `.ctl` file is pretty simple using the following code:
+```python
+from xgrads import CtlDescriptor
+
+ctl = CtlDescriptor(file='test.ctl')
+
+# print all the info in ctl file
+print(ctl)
+```
+
+If you have already load the ASCII content in the `.ctl` file, you can do it as:
+```python
+content = \
+    "dset ^binary.dat\n" \
+    "* this is a comment line\n" \
+    "title 10-deg resolution model\n" \
+    "undef -9.99e8\n" \
+    "xdef 36 linear   0 10\n" \
+    "ydef 19 linear -90 10\n" \
+    "zdef  1 linear   0  1\n" \
+    "tdef  1 linear 00z01Jan2000 1dy\n" \
+    "vars  1\n" \
+    "test  1 99 test variable\n" \
+    "endvars\n"
+
+ctl = CtlDescriptor(content=content)
+
+# print all the info
+print(ctl)
+```
+---
+
+### 3.2 Read binary data into a `xarray.Dataset`
+Reading a `.ctl` related binary data file is also pretty simple using the following code:
+```python
+from xgrads import open_CtlDataset
+
+dset = open_CtlDataset('test.ctl')
+
+# print all the info in ctl file
+print(dset)
+```
+
+Then you have the `dset` as a `xarray.Dataset`.  This is similar to [`xarray.open_dataset`](http://xarray.pydata.org/en/stable/generated/xarray.open_dataset.html) that use [`dask`](https://dask.org/) to chunk (buffer) parts of the whole dataset in physical memory if the whole dataset is too large to fit in.
+
+If there are many `.ctl` files in a folder, we can also open all of them in a single call of `open_mfdataset` as:
+```python
+from xgrads import open_mfDataset
+
+dset = open_mfDataset('./folder/*.ctl')
+
+# print all the info in ctl file
+print(dset)
+```
+assuming that every `.ctl` file has similar data structure except the time step is different.  This is similar to [`xarray.open_mfdataset`](http://xarray.pydata.org/en/v0.12.3/generated/xarray.open_mfdataset.html).
+
+---
+
+### 3.3 Convert a GrADS dataset to a NetCDF dataset
+With the above functionality, it is easy to convert a `.ctl` ([GrADS](http://cola.gmu.edu/grads/)) dataset to a `.nc` ([NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/file_structure_and_performance.html)) dataset:
+```python
+from xgrads import open_CtlDataset
+
+open_CtlDataset('input.ctl').to_netcdf('output.nc')
+```
```

