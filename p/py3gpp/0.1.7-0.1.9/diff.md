# Comparing `tmp/py3gpp-0.1.7.tar.gz` & `tmp/py3gpp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3gpp-0.1.7.tar", last modified: Fri Apr 28 07:09:56 2023, max compression
+gzip compressed data, was "py3gpp-0.1.9.tar", last modified: Sun Aug  6 16:58:08 2023, max compression
```

## Comparing `py3gpp-0.1.7.tar` & `py3gpp-0.1.9.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.764460 py3gpp-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 07:09:38.000000 py3gpp-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-28 07:09:56.764460 py3gpp-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-28 07:09:38.000000 py3gpp-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/CommonConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/DMRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/PDSCHConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/PDSCHPTRSConfigBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrCarrierConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrNumerologyConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHDMRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/configs/nrPDSCHPTRSConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrChannelEstimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrEqualizeMMSE.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrExtractResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrOFDMModulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCH.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPBCHPRBS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHPTRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPRBS.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrRateRecoverPolar.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrResourceGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSetResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSymbolDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrSymbolModulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-28 07:09:38.000000 py3gpp-0.1.7/py3gpp/nrTimingEstimate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.760460 py3gpp-0.1.7/py3gpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 07:09:56.000000 py3gpp-0.1.7/py3gpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 07:09:38.000000 py3gpp-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 07:09:56.764460 py3gpp-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 07:09:38.000000 py3gpp-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 07:09:56.764460 py3gpp-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHPTRS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrPDSCHPTRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-28 07:09:38.000000 py3gpp-0.1.7/tests/test_nrRateRecoverPolar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:58:08.083630 py3gpp-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-06 16:57:50.000000 py3gpp-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-06 16:58:08.083630 py3gpp-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-06 16:57:50.000000 py3gpp-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:58:08.079630 py3gpp-0.1.9/py3gpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:58:08.079630 py3gpp-0.1.9/py3gpp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/CommonConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/DMRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/PDSCHConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/PDSCHPTRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/nrCarrierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/nrNumerologyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/nrPDSCHConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/nrPDSCHDMRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/configs/nrPDSCHPTRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrChannelEstimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrDLSCHInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrEqualizeMMSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrExtractResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrOFDMDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrOFDMInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrOFDMModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPBCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPBCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPBCHPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPDSCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrResourceGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrSSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrSetResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrSymbolDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrSymbolModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-06 16:57:50.000000 py3gpp-0.1.9/py3gpp/nrTimingEstimate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:58:08.079630 py3gpp-0.1.9/py3gpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-06 16:58:08.000000 py3gpp-0.1.9/py3gpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-06 16:58:08.000000 py3gpp-0.1.9/py3gpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 16:58:08.000000 py3gpp-0.1.9/py3gpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 16:58:08.000000 py3gpp-0.1.9/py3gpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-06 16:58:08.000000 py3gpp-0.1.9/py3gpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-06 16:57:50.000000 py3gpp-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 16:58:08.083630 py3gpp-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 16:57:50.000000 py3gpp-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 16:58:08.083630 py3gpp-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrPDSCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-06 16:57:50.000000 py3gpp-0.1.9/tests/test_phase_compensation.py
```

### Comparing `py3gpp-0.1.7/LICENSE` & `py3gpp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/PKG-INFO` & `py3gpp-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.7
+Version: 0.1.9
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.7/README.md` & `py3gpp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/__init__.py` & `py3gpp-0.1.9/py3gpp/__init__.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/CommonConfig.py` & `py3gpp-0.1.9/py3gpp/configs/CommonConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/DMRSConfigBase.py` & `py3gpp-0.1.9/py3gpp/configs/DMRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/PDSCHConfigBase.py` & `py3gpp-0.1.9/py3gpp/configs/PDSCHConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/PDSCHPTRSConfigBase.py` & `py3gpp-0.1.9/py3gpp/configs/PDSCHPTRSConfigBase.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/nrCarrierConfig.py` & `py3gpp-0.1.9/py3gpp/configs/nrCarrierConfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .nrNumerologyConfig import nrNumerologyConfig
 
 class nrCarrierConfig(nrNumerologyConfig):
         def __init__(self, NCellID = 1, NSizeGrid = 52, NStartGrid = 0, NSlot = 0, NFrame = 0, SubcarrierSpacing = 15):
+            super().__init__()
             self._NCellID = NCellID
             self._NSizeGrid = NSizeGrid
             self._NStartGrid = NStartGrid
             self._NSlot = NSlot
             self._NFrame = NFrame
             self.SubcarrierSpacing = SubcarrierSpacing
```

### Comparing `py3gpp-0.1.7/py3gpp/configs/nrNumerologyConfig.py` & `py3gpp-0.1.9/py3gpp/configs/nrNumerologyConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/nrPDSCHConfig.py` & `py3gpp-0.1.9/py3gpp/configs/nrPDSCHConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/configs/nrPDSCHDMRSConfig.py` & `py3gpp-0.1.9/py3gpp/configs/nrPDSCHDMRSConfig.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/helper.py` & `py3gpp-0.1.9/py3gpp/helper.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrBCHDecode.py` & `py3gpp-0.1.9/py3gpp/nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrCRCEncode.py` & `py3gpp-0.1.9/py3gpp/nrCRCEncode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrChannelEstimate.py` & `py3gpp-0.1.9/py3gpp/nrChannelEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrOFDMDemodulate.py` & `py3gpp-0.1.9/py3gpp/nrOFDMDemodulate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from py3gpp.nrOFDMInfo import nrOFDMInfo
+from py3gpp.configs.nrCarrierConfig import nrCarrierConfig
 
 # TODO: implement CyclicPrefixFraction
 def nrOFDMDemodulate(
     carrier=None,
     waveform=None,
     nrb=None,
     scs=None,
@@ -23,46 +24,64 @@
             return
         if scs == None:
             print("Error: scs is needed without carrierConfig!")
             return
         if initialNSlot == None:
             print("Error: initialNSlot is needed without carrierConfig!")
             return
+        carrier = nrCarrierConfig(1, NSizeGrid = nrb, NStartGrid = 0, SubcarrierSpacing = scs, NSlot = initialNSlot)
     else:
         nrb = carrier.NSizeGrid
         scs = carrier.SubcarrierSpacing
-        initialNSlot = 0
+        initialNSlot = 0 if initialNSlot is None else initialNSlot
+        
     if Nfft == None:
         if SampleRate == None:
             Nfft = nrOFDMInfo(nrb=nrb, scs=scs)["Nfft"]
             SampleRate = int(Nfft * scs * 1000)
         else:
             Nfft = int(SampleRate // scs // 1000)
     mu = (scs // 15) - 1
     if CyclicPrefix == "normal":
         N_cp1 = int(((144) * 2 ** (-mu) + 16) * (SampleRate / 30720000))
         N_cp2 = int((144 * 2 ** (-mu)) * (SampleRate / 30720000))
     else:
         N_cp1 = int((512 * 2 ** (-mu)) * (SampleRate / 30720000))
         N_cp2 = N_cp1
+    N_cp = np.zeros(carrier.SymbolsPerSlot, dtype=int)
+    for i in range(len(N_cp)):
+        N_cp[i] = N_cp1 if i == 0 or i == 7 * 2 ** (mu) else N_cp2
 
     idx = 0
-    slot = 0
+    sym_pos_in_slot = initialNSlot
     grid = np.zeros((nrb * 12, 0), "complex")
-    while idx + Nfft < waveform.shape[0]:
-        if slot == 0 or slot == 7 * 2 ** (mu):
-            cp = N_cp1
-        else:
-            cp = N_cp2
-        slot = (slot + 1) % (7 * 2 ** (mu))
-        cp_advance = int(CyclicPrefixFraction * cp)
+
+    sample_pos_in_slot = 0
+    for i in range(initialNSlot):
+        sample_pos_in_slot += Nfft + N_cp[i]
+
+    symbols_per_slot = carrier.SymbolsPerSlot
+    while idx + Nfft <= waveform.shape[0]:
+        sym_pos_in_slot = sym_pos_in_slot % symbols_per_slot
+        cp_advance = int(CyclicPrefixFraction * N_cp[sym_pos_in_slot])
         idx += cp_advance
         symbol_t = waveform[idx:][:Nfft]
         symbol_f = np.fft.fftshift(np.fft.fft(symbol_t))
 
-        symbol_f *= np.exp(1j*2*np.pi*(cp - cp_advance)/Nfft*np.arange(len(symbol_f)))
-        symbol_f *= np.exp(1j*np.pi*(cp - cp_advance))
+        symbol_f *= np.exp(1j*2*np.pi*(N_cp[sym_pos_in_slot] - cp_advance)/Nfft*np.arange(len(symbol_f)))
+        symbol_f *= np.exp(1j*np.pi*(N_cp[sym_pos_in_slot] - cp_advance))
 
         symbol_f = symbol_f[Nfft // 2 - nrb * 12 // 2 : Nfft // 2 + nrb * 12 // 2]
+
+        # phase compensation according to TS 38.211 section 5.4
+        if sym_pos_in_slot == 0:
+            sample_pos_in_slot = 0
+        sample_pos_in_slot += N_cp[sym_pos_in_slot]
+        # print(f'symbol {sym_pos_in_slot}, pos {sample_pos_in_slot}, CP {N_cp[sym_pos_in_slot]}, pos {idx - cp_advance}')
+        symbol_f *= np.exp(1j * 2 * np.pi * CarrierFrequency / SampleRate * sample_pos_in_slot)
+        sample_pos_in_slot += Nfft
+
         grid = np.concatenate((grid, np.expand_dims(symbol_f, 1)), axis=1)
-        idx += Nfft + (cp - cp_advance)
+        idx += Nfft + (N_cp[sym_pos_in_slot] - cp_advance)
+        # print(f'slot {slot}, cp_len {N_cp}')
+        sym_pos_in_slot = sym_pos_in_slot + 1
     return grid
```

### Comparing `py3gpp-0.1.7/py3gpp/nrPBCH.py` & `py3gpp-0.1.9/py3gpp/nrPBCH.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrPBCHDMRSIndices.py` & `py3gpp-0.1.9/py3gpp/nrPBCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrPDSCHDMRS.py` & `py3gpp-0.1.9/py3gpp/nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrPDSCHDMRSIndices.py` & `py3gpp-0.1.9/py3gpp/nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrPDSCHPTRS.py` & `py3gpp-0.1.9/py3gpp/nrPDSCHPTRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrPDSCHPTRSIndices.py` & `py3gpp-0.1.9/py3gpp/nrPDSCHPTRSIndices.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from py3gpp.nrPDSCHPTRS import PDSCHPTRSSyms
 from py3gpp.configs.nrPDSCHConfig import nrPDSCHConfig
 from py3gpp.configs.nrCarrierConfig import nrCarrierConfig
 
 def nrPDSCHPTRSIndices(carrier: nrCarrierConfig, cfg: nrPDSCHConfig):
     if cfg.EnablePTRS == 0:
-        return []
+        return np.array([])
 
     frame_begin = cfg.NRBSize * min(cfg.PRBSet)
     frame_end = cfg.NRBSize * (max(cfg.PRBSet)+1)
     frame_size = cfg.NRBSize * cfg.NSizeBWP
 
     # Align with frequency offset based on DMRS type
     if cfg.DMRS.DMRSConfigurationType == 1:
@@ -30,15 +30,15 @@
     kRBref *= cfg.NRBSize
 
     # Move to BWP offset and the rest frequency offsets
     ptrs_begin = frame_begin + kREref + kRBref
 
     # Calculate PTRS positions in every occupied symbol. Frequency position,
     # for every 2 or 4 RBs
-    occupied_res = np.array(list(range(ptrs_begin, frame_end, (cfg.PTRS.FrequencyDensity*12))))
+    occupied_res = np.array(list(range(ptrs_begin, frame_end, (cfg.PTRS.FrequencyDensity*cfg.NRBSize))))
 
     # Calculates occupied symbols numbers. Time positions
     occupied_syms = PDSCHPTRSSyms(carrier, cfg)
 
     # Move PTRS indices to occupied symbols
     ptrs_indices = np.array([occupied_res+(sym*frame_size) for sym in occupied_syms])
     if len(ptrs_indices) > 0:
```

### Comparing `py3gpp-0.1.7/py3gpp/nrPolarDecode.py` & `py3gpp-0.1.9/py3gpp/nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrRateRecoverPolar.py` & `py3gpp-0.1.9/py3gpp/nrRateRecoverPolar.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrSSS.py` & `py3gpp-0.1.9/py3gpp/nrSSS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrSymbolDemodulate.py` & `py3gpp-0.1.9/py3gpp/nrSymbolDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/py3gpp/nrSymbolModulate.py` & `py3gpp-0.1.9/py3gpp/nrSymbolModulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 # 38.211 5.1 Modulation mapper
 
 import numpy as np
 
 def nrSymbolModulate(databits, modulation):
     int_modtype = modulation.lower()
 
-    assert int_modtype in ['bpsk_pi2', 'bpsk', 'qpsk', 'qam16', 'qam64', 'qam256'], "modulation type is incorrect"
+    assert int_modtype in ["pi/2-bpsk", "bpsk", "qpsk", "16qam", "64qam", "256qam"], "modulation type is incorrect"
     assert len(databits) > 0, "length of databits must be greater 0"
 
-    if int_modtype == 'bpsk':
+    if int_modtype == "bpsk":
         res_arr = np.zeros(len(databits), dtype=(complex))
         for idx, sample in enumerate(databits):
             res_arr[idx] = (1-2*sample) + 1j*(1-2*sample)
         res_arr = [x/np.sqrt(2) for x in res_arr]
 
-    elif int_modtype == 'bpsk_pi2':
+    elif int_modtype == "pi/2-bpsk":
         res_arr = np.zeros(len(databits), dtype=(complex))
         for idx, sample in enumerate(databits):
             if idx%2:
                 res_arr[idx] = (2*sample-1) + 1j*(1-2*sample)
             else:
                 res_arr[idx] = (1-2*sample) + 1j*(1-2*sample)
         res_arr = [x/np.sqrt(2) for x in res_arr]
 
-    elif int_modtype == 'qpsk':
+    elif int_modtype == "qpsk":
         assert not (len(databits) % 2), "length of databits must be multiple of 2"
         res_arr = np.zeros((len(databits)//2), dtype=(complex))
         chunks = np.array_split(databits, len(databits)//2)
         for idx, sample in enumerate(chunks):
             res_arr[idx] = (1-2*sample[0]) + 1j*(1-2*sample[1])
         res_arr = [x/np.sqrt(2) for x in res_arr]
 
-    elif int_modtype == 'qam16':
+    elif int_modtype == "16qam":
         assert not (len(databits) % 4), "length of databits must be multiple of 4"
         res_arr = np.zeros((len(databits)//4), dtype=(complex))
         chunks = np.array_split(databits, len(databits)//4)
         for idx, sample in enumerate(chunks):
             res_arr[idx] = ( (1-2*sample[0]) * (2-(1-2*sample[2])) ) + 1j*( (1-2*sample[1]) * (2-(1-2*sample[3])) )
         res_arr = [x/np.sqrt(10) for x in res_arr]
 
-    elif int_modtype == 'qam64':
+    elif int_modtype == "64qam":
         assert not (len(databits) % 6), "length of databits must be multiple of 6"
         res_arr = np.zeros((len(databits)//6), dtype=(complex))
         chunks = np.array_split(databits, len(databits)//6)
         for idx, sample in enumerate(chunks):
             res_arr[idx] = ( (1-2*sample[0]) * (4-(1-2*sample[2]) * (2-(1-2*sample[4]))) ) + 1j*( (1-2*sample[1]) * (4-(1-2*sample[3]) * (2-(1-2*sample[5]))) )
         res_arr = [x/np.sqrt(42) for x in res_arr]
 
-    elif int_modtype == 'qam256':
+    elif int_modtype == "256qam":
         assert not (len(databits) % 8), "length of databits must be multiple of 8"
         res_arr = np.zeros((len(databits)//8), dtype=(complex))
         chunks = np.array_split(databits, len(databits)//8)
         for idx, sample in enumerate(chunks):
             res_arr[idx] = ( (1-2*sample[0]) * (8-(1-2*sample[2]) * (4-(1-2*sample[4]) * (2-(1-2*sample[6])))) ) + 1j*( (1-2*sample[1]) * (8-(1-2*sample[3]) * (4-(1-2*sample[5]) * (2-(1-2*sample[7])))) )
         res_arr = [x/np.sqrt(170) for x in res_arr]
```

### Comparing `py3gpp-0.1.7/py3gpp/nrTimingEstimate.py` & `py3gpp-0.1.9/py3gpp/nrTimingEstimate.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     scs=None,
     initialNSlot=None,
     refInd=None,
     refSym=None,
     CyclicPrefix="normal",
     Nfft=None,
     SampleRate=None,
+    CarrierFrequency=None
 ):
     refWaveform, _ = nrOFDMModulate(
-        grid=refGrid, scs=scs, initialNSlot=initialNSlot, SampleRate=SampleRate, Nfft=Nfft, carrier=carrier
+        grid=refGrid, scs=scs, initialNSlot=initialNSlot, SampleRate=SampleRate, Nfft=Nfft,
+        carrier=carrier, CarrierFrequency=CarrierFrequency
     )
     xcorr = scipy.signal.correlate(waveform, refWaveform, "valid")
     index = np.argmax(np.abs(xcorr))
     return index
```

### Comparing `py3gpp-0.1.7/py3gpp.egg-info/PKG-INFO` & `py3gpp-0.1.9/py3gpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.7
+Version: 0.1.9
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.7/py3gpp.egg-info/SOURCES.txt` & `py3gpp-0.1.9/py3gpp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 setup.py
 py3gpp/__init__.py
 py3gpp/helper.py
 py3gpp/nrBCHDecode.py
 py3gpp/nrCRCDecode.py
 py3gpp/nrCRCEncode.py
 py3gpp/nrChannelEstimate.py
+py3gpp/nrDLSCHInfo.py
 py3gpp/nrEqualizeMMSE.py
 py3gpp/nrExtractResources.py
 py3gpp/nrOFDMDemodulate.py
 py3gpp/nrOFDMInfo.py
 py3gpp/nrOFDMModulate.py
 py3gpp/nrPBCH.py
 py3gpp/nrPBCHDMRS.py
 py3gpp/nrPBCHDMRSIndices.py
 py3gpp/nrPBCHIndices.py
 py3gpp/nrPBCHPRBS.py
+py3gpp/nrPDSCH.py
 py3gpp/nrPDSCHDMRS.py
 py3gpp/nrPDSCHDMRSIndices.py
 py3gpp/nrPDSCHPTRS.py
 py3gpp/nrPDSCHPTRSIndices.py
 py3gpp/nrPRBS.py
 py3gpp/nrPSS.py
 py3gpp/nrPSSIndices.py
@@ -48,12 +50,14 @@
 py3gpp/configs/nrNumerologyConfig.py
 py3gpp/configs/nrPDSCHConfig.py
 py3gpp/configs/nrPDSCHDMRSConfig.py
 py3gpp/configs/nrPDSCHPTRSConfig.py
 tests/test_nrBCHDecode.py
 tests/test_nrCRCDecode.py
 tests/test_nrCRCEncode.py
+tests/test_nrPDSCH.py
 tests/test_nrPDSCHDMRS.py
 tests/test_nrPDSCHDMRSIndices.py
 tests/test_nrPDSCHPTRS.py
 tests/test_nrPDSCHPTRSIndices.py
-tests/test_nrRateRecoverPolar.py
+tests/test_nrRateRecoverPolar.py
+tests/test_phase_compensation.py
```

### Comparing `py3gpp-0.1.7/pyproject.toml` & `py3gpp-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.7"
+version = "0.1.9"
 authors = [
     {name = "Benjamin Menküc", email = "benjamin@menkuec.de"},
 ]
 description = "Functions for 5G NR signal processing"
 name = "py3gpp"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `py3gpp-0.1.7/tests/test_nrBCHDecode.py` & `py3gpp-0.1.9/tests/test_nrBCHDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrCRCDecode.py` & `py3gpp-0.1.9/tests/test_nrCRCDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrPDSCHDMRS.py` & `py3gpp-0.1.9/tests/test_nrPDSCHDMRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrPDSCHDMRSIndices.py` & `py3gpp-0.1.9/tests/test_nrPDSCHDMRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrPDSCHPTRS.py` & `py3gpp-0.1.9/tests/test_nrPDSCHPTRS.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrPDSCHPTRSIndices.py` & `py3gpp-0.1.9/tests/test_nrPDSCHPTRSIndices.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.7/tests/test_nrRateRecoverPolar.py` & `py3gpp-0.1.9/tests/test_nrRateRecoverPolar.py`

 * *Files identical despite different names*

