# Comparing `tmp/watertools-0.0.8.tar.gz` & `tmp/watertools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\watertools-0.0.8.tar", last modified: Sun Nov 17 21:51:31 2019, max compression
+gzip compressed data, was "dist\watertools-0.0.9.tar", last modified: Sun Nov 17 21:55:08 2019, max compression
```

## Comparing `watertools-0.0.8.tar` & `watertools-0.0.9.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/
--rw-rw-rw-   0        0        0      694 2019-11-17 21:51:31.000000 watertools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      103 2019-10-17 14:28:12.000000 watertools-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2019-11-17 21:51:31.000000 watertools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      824 2019-11-17 21:51:05.000000 watertools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/ALEXI/
--rw-rw-rw-   0        0        0    10979 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ALEXI/DataAccess.py
--rw-rw-rw-   0        0        0      960 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ALEXI/__init__.py
--rw-rw-rw-   0        0        0      793 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ALEXI/daily.py
--rw-rw-rw-   0        0        0     1398 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ALEXI/monthly.py
--rw-rw-rw-   0        0        0      796 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ALEXI/weekly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/ASCAT/
--rw-rw-rw-   0        0        0     6297 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ASCAT/DataAccess.py
--rw-rw-rw-   0        0        0      119 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ASCAT/__init__.py
--rw-rw-rw-   0        0        0      824 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ASCAT/daily.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/CFSR/
--rw-rw-rw-   0        0        0     8617 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CFSR/DataAccess_CFSR.py
--rw-rw-rw-   0        0        0     2687 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CFSR/Download_data_CFSR.py
--rw-rw-rw-   0        0        0     1056 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CFSR/__init__.py
--rw-rw-rw-   0        0        0     2559 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CFSR/daily.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/CHIRPS/
--rw-rw-rw-   0        0        0     6591 2019-11-17 18:04:19.000000 watertools-0.0.8/watertools/Collect/CHIRPS/DataAccess.py
--rw-rw-rw-   0        0        0      912 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CHIRPS/__init__.py
--rw-rw-rw-   0        0        0     1218 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CHIRPS/daily.py
--rw-rw-rw-   0        0        0     1046 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CHIRPS/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/CMRSET/
--rw-rw-rw-   0        0        0     5045 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CMRSET/DataAccess.py
--rw-rw-rw-   0        0        0      759 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CMRSET/__init__.py
--rw-rw-rw-   0        0        0      826 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/CMRSET/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/DEM/
--rw-rw-rw-   0        0        0    20103 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/DEM/DataAccess_Hydro.py
--rw-rw-rw-   0        0        0    11339 2019-11-11 13:48:07.000000 watertools-0.0.8/watertools/Collect/DEM/DataAccess_SRTM.py
--rw-rw-rw-   0        0        0     1993 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/DEM/HydroSHED.py
--rw-rw-rw-   0        0        0     2167 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/DEM/HydroSHED_Dir.py
--rw-rw-rw-   0        0        0     1765 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/DEM/SRTM.py
--rw-rw-rw-   0        0        0      568 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/DEM/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/ECMWF/
--rw-rw-rw-   0        0        0    14224 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ECMWF/DataAccess.py
--rw-rw-rw-   0        0        0     1910 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ECMWF/ECMWFdownload.py
--rw-rw-rw-   0        0        0     1074 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ECMWF/__init__.py
--rw-rw-rw-   0        0        0     1358 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ECMWF/daily.py
--rw-rw-rw-   0        0        0     1347 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ECMWF/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/ESACCI/
--rw-rw-rw-   0        0        0     1731 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ESACCI/DataAccess.py
--rw-rw-rw-   0        0        0     1594 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ESACCI/LU.py
--rw-rw-rw-   0        0        0      222 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ESACCI/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/ETmonitor/
--rw-rw-rw-   0        0        0     7467 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/DataAccess.py
--rw-rw-rw-   0        0        0      871 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/ET_monthly.py
--rw-rw-rw-   0        0        0      881 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/ETpot_monthly.py
--rw-rw-rw-   0        0        0      866 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/Ei_monthly.py
--rw-rw-rw-   0        0        0      868 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/Es_monthly.py
--rw-rw-rw-   0        0        0      854 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/Ew_monthly.py
--rw-rw-rw-   0        0        0      865 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/Tr_monthly.py
--rw-rw-rw-   0        0        0     1089 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/ETmonitor/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/FEWS/
--rw-rw-rw-   0        0        0      906 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/FEWS/ETpot_daily.py
--rw-rw-rw-   0        0        0      517 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/FEWS/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/GEOS/
--rw-rw-rw-   0        0        0     7670 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GEOS/DataAccess.py
--rw-rw-rw-   0        0        0      967 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GEOS/__init__.py
--rw-rw-rw-   0        0        0      887 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GEOS/daily.py
--rw-rw-rw-   0        0        0     1097 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GEOS/three_hourly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/GLDAS/
--rw-rw-rw-   0        0        0    31339 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/CLSM_DataAccess.py
--rw-rw-rw-   0        0        0     1032 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/CLSM_daily.py
--rw-rw-rw-   0        0        0     1070 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/CLSM_monthly.py
--rw-rw-rw-   0        0        0     1594 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/CLSM_three_hourly.py
--rw-rw-rw-   0        0        0    30335 2019-11-05 17:25:12.000000 watertools-0.0.8/watertools/Collect/GLDAS/DataAccess.py
--rw-rw-rw-   0        0        0    30301 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/NOAH_DataAccess.py
--rw-rw-rw-   0        0        0     1588 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/NOAH_daily.py
--rw-rw-rw-   0        0        0     1255 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/NOAH_monthly.py
--rw-rw-rw-   0        0        0     1854 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/NOAH_three_hourly.py
--rw-rw-rw-   0        0        0     2115 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/__init__.py
--rw-rw-rw-   0        0        0     1573 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/daily.py
--rw-rw-rw-   0        0        0     1245 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/monthly.py
--rw-rw-rw-   0        0        0     1844 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLDAS/three_hourly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/GLEAM/
--rw-rw-rw-   0        0        0     9602 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/DataAccess.py
--rw-rw-rw-   0        0        0      909 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/ET_daily.py
--rw-rw-rw-   0        0        0      891 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/ET_monthly.py
--rw-rw-rw-   0        0        0      922 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/ETpot_daily.py
--rw-rw-rw-   0        0        0      904 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/ETpot_monthly.py
--rw-rw-rw-   0        0        0      999 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GLEAM/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/GPM/
--rw-rw-rw-   0        0        0     6004 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GPM/DataAccess.py
--rw-rw-rw-   0        0        0      874 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GPM/__init__.py
--rw-rw-rw-   0        0        0      980 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GPM/daily.py
--rw-rw-rw-   0        0        0      997 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/GPM/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/Globcover/
--rw-rw-rw-   0        0        0     3104 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/Globcover/DataAccess.py
--rw-rw-rw-   0        0        0     1130 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/Globcover/Landuse.py
--rw-rw-rw-   0        0        0      490 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/Globcover/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/HiHydroSoil/
--rw-rw-rw-   0        0        0     5076 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/HiHydroSoil/DataAccess.py
--rw-rw-rw-   0        0        0      691 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/HiHydroSoil/ThetaSat_TopSoil.py
--rw-rw-rw-   0        0        0      697 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/HiHydroSoil/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/JRC/
--rw-rw-rw-   0        0        0     7770 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/JRC/DataAccess.py
--rw-rw-rw-   0        0        0      585 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/JRC/Occurrence.py
--rw-rw-rw-   0        0        0      566 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/JRC/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/L30/
--rw-rw-rw-   0        0        0     3658 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/L30/DataAccess.py
--rw-rw-rw-   0        0        0      819 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/L30/Harmonized.py
--rw-rw-rw-   0        0        0      326 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/L30/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MCD43/
--rw-rw-rw-   0        0        0      853 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MCD43/Albedo_daily.py
--rw-rw-rw-   0        0        0    15811 2019-11-17 17:12:50.000000 watertools-0.0.8/watertools/Collect/MCD43/DataAccess.py
--rw-rw-rw-   0        0        0      619 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MCD43/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MERRA/
--rw-rw-rw-   0        0        0    15607 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/DataAccess.py
--rw-rw-rw-   0        0        0     1140 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/__init__.py
--rw-rw-rw-   0        0        0      919 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/daily.py
--rw-rw-rw-   0        0        0      938 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/daily_MERRA2.py
--rw-rw-rw-   0        0        0     1158 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/hourly_MERRA2.py
--rw-rw-rw-   0        0        0     1121 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/three_hourly.py
--rw-rw-rw-   0        0        0      929 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MERRA/yearly_T_Amplitude.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD10/
--rw-rw-rw-   0        0        0    16313 2019-11-17 17:14:25.000000 watertools-0.0.8/watertools/Collect/MOD10/DataAccess.py
--rw-rw-rw-   0        0        0      818 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD10/SnowMask_8daily.py
--rw-rw-rw-   0        0        0      666 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD10/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD11/
--rw-rw-rw-   0        0        0    21206 2019-11-17 17:15:15.000000 watertools-0.0.8/watertools/Collect/MOD11/DataAccess.py
--rw-rw-rw-   0        0        0      863 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD11/LST_8daily.py
--rw-rw-rw-   0        0        0      858 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD11/LST_daily.py
--rw-rw-rw-   0        0        0      649 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD11/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD12/
--rw-rw-rw-   0        0        0    14605 2019-11-17 17:17:09.000000 watertools-0.0.8/watertools/Collect/MOD12/DataAccess.py
--rw-rw-rw-   0        0        0      889 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD12/LC_yearly.py
--rw-rw-rw-   0        0        0      716 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD12/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD13/
--rw-rw-rw-   0        0        0    16686 2019-11-17 17:16:53.000000 watertools-0.0.8/watertools/Collect/MOD13/DataAccess.py
--rw-rw-rw-   0        0        0      814 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD13/NDVI_16daily.py
--rw-rw-rw-   0        0        0      607 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD13/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD15/
--rw-rw-rw-   0        0        0    21444 2019-11-17 17:12:42.000000 watertools-0.0.8/watertools/Collect/MOD15/DataAccess.py
--rw-rw-rw-   0        0        0      861 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD15/FPAR_8daily.py
--rw-rw-rw-   0        0        0      859 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD15/LAI_8daily.py
--rw-rw-rw-   0        0        0      786 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD15/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD16/
--rw-rw-rw-   0        0        0    17937 2019-11-17 17:17:57.000000 watertools-0.0.8/watertools/Collect/MOD16/DataAccess.py
--rw-rw-rw-   0        0        0      974 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD16/ET_8daily.py
--rw-rw-rw-   0        0        0      848 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD16/ET_monthly.py
--rw-rw-rw-   0        0        0      650 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD16/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD17/
--rw-rw-rw-   0        0        0    16769 2019-11-17 17:18:36.000000 watertools-0.0.8/watertools/Collect/MOD17/DataAccessGPP.py
--rw-rw-rw-   0        0        0    15780 2019-11-17 17:19:11.000000 watertools-0.0.8/watertools/Collect/MOD17/DataAccessNPP.py
--rw-rw-rw-   0        0        0      822 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD17/GPP_8daily.py
--rw-rw-rw-   0        0        0      818 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD17/NPP_yearly.py
--rw-rw-rw-   0        0        0      779 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD17/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MOD9/
--rw-rw-rw-   0        0        0    15347 2019-11-17 17:13:30.000000 watertools-0.0.8/watertools/Collect/MOD9/DataAccess.py
--rw-rw-rw-   0        0        0      874 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD9/REF_daily.py
--rw-rw-rw-   0        0        0      599 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MOD9/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MSGCPP/
--rw-rw-rw-   0        0        0     3707 2019-11-03 19:00:39.000000 watertools-0.0.8/watertools/Collect/MSGCPP/DataAccess.py
--rw-rw-rw-   0        0        0      937 2019-10-31 07:49:40.000000 watertools-0.0.8/watertools/Collect/MSGCPP/SDS.py
--rw-rw-rw-   0        0        0      686 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MSGCPP/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MSWEP/
--rw-rw-rw-   0        0        0    10055 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MSWEP/DataAccess.py
--rw-rw-rw-   0        0        0      719 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MSWEP/__init__.py
--rw-rw-rw-   0        0        0      847 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MSWEP/daily.py
--rw-rw-rw-   0        0        0      848 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MSWEP/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MYD11/
--rw-rw-rw-   0        0        0    19339 2019-11-17 17:19:53.000000 watertools-0.0.8/watertools/Collect/MYD11/DataAccess.py
--rw-rw-rw-   0        0        0     1082 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MYD11/LST_daily.py
--rw-rw-rw-   0        0        0      587 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MYD11/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/MYD13/
--rw-rw-rw-   0        0        0    16792 2019-11-17 17:20:30.000000 watertools-0.0.8/watertools/Collect/MYD13/DataAccess.py
--rw-rw-rw-   0        0        0      814 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MYD13/NDVI_16daily.py
--rw-rw-rw-   0        0        0      607 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/MYD13/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/NLDAS/
--rw-rw-rw-   0        0        0    35162 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/DataAccess.py
--rw-rw-rw-   0        0        0    22946 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/FORA_DataAccess.py
--rw-rw-rw-   0        0        0     1346 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/FORA_daily.py
--rw-rw-rw-   0        0        0     1508 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/FORA_hourly.py
--rw-rw-rw-   0        0        0     1041 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/FORA_monthly.py
--rw-rw-rw-   0        0        0     1737 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/__init__.py
--rw-rw-rw-   0        0        0     1346 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/daily.py
--rw-rw-rw-   0        0        0     1456 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/hourly.py
--rw-rw-rw-   0        0        0     1041 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/NLDAS/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/PROBAV/
--rw-rw-rw-   0        0        0    14349 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/PROBAV/DataAccess.py
--rw-rw-rw-   0        0        0      666 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/PROBAV/__init__.py
--rw-rw-rw-   0        0        0      968 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/PROBAV/five_daily.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/RFE/
--rw-rw-rw-   0        0        0     5375 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/RFE/DataAccess.py
--rw-rw-rw-   0        0        0      857 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/RFE/__init__.py
--rw-rw-rw-   0        0        0      963 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/RFE/daily.py
--rw-rw-rw-   0        0        0     3493 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/RFE/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/S30/
--rw-rw-rw-   0        0        0     3551 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/S30/DataAccess.py
--rw-rw-rw-   0        0        0      819 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/S30/Harmonized.py
--rw-rw-rw-   0        0        0      326 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/S30/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/SEBS/
--rw-rw-rw-   0        0        0     5631 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SEBS/DataAccess.py
--rw-rw-rw-   0        0        0      745 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SEBS/__init__.py
--rw-rw-rw-   0        0        0      820 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SEBS/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/SSEBop/
--rw-rw-rw-   0        0        0    10921 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SSEBop/DataAccess.py
--rw-rw-rw-   0        0        0      886 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SSEBop/ET_monthly.py
--rw-rw-rw-   0        0        0      906 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SSEBop/ETpot_daily.py
--rw-rw-rw-   0        0        0      917 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SSEBop/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/SoilGrids/
--rw-rw-rw-   0        0        0     1783 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Absolute_Depth_To_Bedrock.py
--rw-rw-rw-   0        0        0     1953 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Bulk_Density.py
--rw-rw-rw-   0        0        0     2096 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Clay_Content.py
--rw-rw-rw-   0        0        0     2036 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Coarse_Fragment_Volumetric.py
--rw-rw-rw-   0        0        0     3047 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/DataAccess.py
--rw-rw-rw-   0        0        0     1749 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Depth_To_Bedrock.py
--rw-rw-rw-   0        0        0     2026 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Organic_Carbon_Content.py
--rw-rw-rw-   0        0        0     2019 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Organic_Carbon_Stock.py
--rw-rw-rw-   0        0        0     1829 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Predicted_Probability_Of_Occurrence.py
--rw-rw-rw-   0        0        0     2017 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Sand_Content.py
--rw-rw-rw-   0        0        0     2017 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Silt_Content.py
--rw-rw-rw-   0        0        0     1967 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/Soil_pH.py
--rw-rw-rw-   0        0        0     1143 2019-10-26 11:54:10.000000 watertools-0.0.8/watertools/Collect/SoilGrids/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/TRMM/
--rw-rw-rw-   0        0        0     6228 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TRMM/DataAccess.py
--rw-rw-rw-   0        0        0      813 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TRMM/__init__.py
--rw-rw-rw-   0        0        0      990 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TRMM/daily.py
--rw-rw-rw-   0        0        0     1007 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TRMM/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Collect/TWC/
--rw-rw-rw-   0        0        0     4285 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TWC/DataAccess.py
--rw-rw-rw-   0        0        0      527 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TWC/Gray_Water_Footprint.py
--rw-rw-rw-   0        0        0      970 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/TWC/__init__.py
--rw-rw-rw-   0        0        0     4162 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Collect/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Functions/
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Functions/Area_Conversions/
--rw-rw-rw-   0        0        0     3132 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Area_Conversions/Area_converter.py
--rw-rw-rw-   0        0        0     2248 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Area_Conversions/Boundaries.py
--rw-rw-rw-   0        0        0      257 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Area_Conversions/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Functions/Random/
--rw-rw-rw-   0        0        0      954 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Random/WaitbarConsole.py
--rw-rw-rw-   0        0        0      221 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Random/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/
--rw-rw-rw-   0        0        0     2794 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/Day_to_monthly_flux.py
--rw-rw-rw-   0        0        0     5069 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/Eightdaily_to_monthly_state.py
--rw-rw-rw-   0        0        0     2488 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/Monthly_to_yearly_flux.py
--rw-rw-rw-   0        0        0     5084 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/Sixteendaily_to_monthly_state.py
--rw-rw-rw-   0        0        0     5236 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/Weekly_to_monthly_flux.py
--rw-rw-rw-   0        0        0      416 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Time_Conversions/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Functions/Visualization/
--rw-rw-rw-   0        0        0     5032 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Visualization/Compare_Rasters_One_Point.py
--rw-rw-rw-   0        0        0     3540 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Visualization/Compare_Rasters_One_Polygon.py
--rw-rw-rw-   0        0        0      308 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/Visualization/__init__.py
--rw-rw-rw-   0        0        0      359 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Functions/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/General/
--rw-rw-rw-   0        0        0      317 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/General/__init__.py
--rw-rw-rw-   0        0        0    19798 2019-11-13 14:06:12.000000 watertools-0.0.8/watertools/General/data_conversions.py
--rw-rw-rw-   0        0        0    39673 2019-11-07 14:27:11.000000 watertools-0.0.8/watertools/General/raster_conversions.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Products/
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Products/ETens/
--rw-rw-rw-   0        0        0     9205 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETens/DataAccess.py
--rw-rw-rw-   0        0        0      582 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETens/__init__.py
--rw-rw-rw-   0        0        0     1563 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETens/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Products/ETref/
--rw-rw-rw-   0        0        0     5896 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/CalcETref.py
--rw-rw-rw-   0        0        0     1785 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/CollectDataETref.py
--rw-rw-rw-   0        0        0     7840 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/CollectLANDSAFETref.py
--rw-rw-rw-   0        0        0     6601 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/Interpolate_Meteo_ETref.py
--rw-rw-rw-   0        0        0     6368 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/SetVarETref.py
--rw-rw-rw-   0        0        0    15848 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/SlopeInfluence_ETref.py
--rw-rw-rw-   0        0        0     1492 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/__init__.py
--rw-rw-rw-   0        0        0     2403 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/daily.py
--rw-rw-rw-   0        0        0     3673 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/ETref/monthly.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools/Products/SoilGrids/
--rw-rw-rw-   0        0        0     1278 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/K_Sat.py
--rw-rw-rw-   0        0        0     4195 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/Theta_FC.py
--rw-rw-rw-   0        0        0     2962 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/Theta_Res.py
--rw-rw-rw-   0        0        0     3933 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/Theta_Sat.py
--rw-rw-rw-   0        0        0     3977 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/Theta_Sat2.py
--rw-rw-rw-   0        0        0     2974 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/Water_Holding_Capacity.py
--rw-rw-rw-   0        0        0      878 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/__init__.py
--rw-rw-rw-   0        0        0     2859 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/SoilGrids/n_van_genuchten.py
--rw-rw-rw-   0        0        0      756 2019-10-26 11:54:11.000000 watertools-0.0.8/watertools/Products/__init__.py
--rw-rw-rw-   0        0        0      452 2019-10-20 11:25:28.000000 watertools-0.0.8/watertools/WebAccounts.py
--rw-rw-rw-   0        0        0      201 2018-12-29 18:43:46.000000 watertools-0.0.8/watertools/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools.egg-info/
--rw-rw-rw-   0        0        0      694 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9150 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2019-11-17 21:51:31.000000 watertools-0.0.8/watertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/
+-rw-rw-rw-   0        0        0      694 2019-11-17 21:55:08.000000 watertools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2019-10-17 14:28:12.000000 watertools-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2019-11-17 21:55:08.000000 watertools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      824 2019-11-17 21:55:00.000000 watertools-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/ALEXI/
+-rw-rw-rw-   0        0        0    10979 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ALEXI/DataAccess.py
+-rw-rw-rw-   0        0        0      960 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ALEXI/__init__.py
+-rw-rw-rw-   0        0        0      793 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ALEXI/daily.py
+-rw-rw-rw-   0        0        0     1398 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ALEXI/monthly.py
+-rw-rw-rw-   0        0        0      796 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ALEXI/weekly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/ASCAT/
+-rw-rw-rw-   0        0        0     6297 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ASCAT/DataAccess.py
+-rw-rw-rw-   0        0        0      119 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ASCAT/__init__.py
+-rw-rw-rw-   0        0        0      824 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ASCAT/daily.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/CFSR/
+-rw-rw-rw-   0        0        0     8617 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CFSR/DataAccess_CFSR.py
+-rw-rw-rw-   0        0        0     2687 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CFSR/Download_data_CFSR.py
+-rw-rw-rw-   0        0        0     1056 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CFSR/__init__.py
+-rw-rw-rw-   0        0        0     2559 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CFSR/daily.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/CHIRPS/
+-rw-rw-rw-   0        0        0     6591 2019-11-17 18:04:19.000000 watertools-0.0.9/watertools/Collect/CHIRPS/DataAccess.py
+-rw-rw-rw-   0        0        0      912 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CHIRPS/__init__.py
+-rw-rw-rw-   0        0        0     1218 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CHIRPS/daily.py
+-rw-rw-rw-   0        0        0     1046 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CHIRPS/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/CMRSET/
+-rw-rw-rw-   0        0        0     5045 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CMRSET/DataAccess.py
+-rw-rw-rw-   0        0        0      759 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CMRSET/__init__.py
+-rw-rw-rw-   0        0        0      826 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/CMRSET/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/DEM/
+-rw-rw-rw-   0        0        0    20103 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/DEM/DataAccess_Hydro.py
+-rw-rw-rw-   0        0        0    11339 2019-11-11 13:48:07.000000 watertools-0.0.9/watertools/Collect/DEM/DataAccess_SRTM.py
+-rw-rw-rw-   0        0        0     1993 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/DEM/HydroSHED.py
+-rw-rw-rw-   0        0        0     2167 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/DEM/HydroSHED_Dir.py
+-rw-rw-rw-   0        0        0     1765 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/DEM/SRTM.py
+-rw-rw-rw-   0        0        0      568 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/DEM/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/ECMWF/
+-rw-rw-rw-   0        0        0    14224 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ECMWF/DataAccess.py
+-rw-rw-rw-   0        0        0     1910 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ECMWF/ECMWFdownload.py
+-rw-rw-rw-   0        0        0     1074 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ECMWF/__init__.py
+-rw-rw-rw-   0        0        0     1358 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ECMWF/daily.py
+-rw-rw-rw-   0        0        0     1347 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ECMWF/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/ESACCI/
+-rw-rw-rw-   0        0        0     1731 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ESACCI/DataAccess.py
+-rw-rw-rw-   0        0        0     1594 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ESACCI/LU.py
+-rw-rw-rw-   0        0        0      222 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ESACCI/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/ETmonitor/
+-rw-rw-rw-   0        0        0     7467 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/DataAccess.py
+-rw-rw-rw-   0        0        0      871 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/ET_monthly.py
+-rw-rw-rw-   0        0        0      881 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/ETpot_monthly.py
+-rw-rw-rw-   0        0        0      866 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/Ei_monthly.py
+-rw-rw-rw-   0        0        0      868 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/Es_monthly.py
+-rw-rw-rw-   0        0        0      854 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/Ew_monthly.py
+-rw-rw-rw-   0        0        0      865 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/Tr_monthly.py
+-rw-rw-rw-   0        0        0     1089 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/ETmonitor/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/FEWS/
+-rw-rw-rw-   0        0        0      906 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/FEWS/ETpot_daily.py
+-rw-rw-rw-   0        0        0      517 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/FEWS/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/GEOS/
+-rw-rw-rw-   0        0        0     7670 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GEOS/DataAccess.py
+-rw-rw-rw-   0        0        0      967 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GEOS/__init__.py
+-rw-rw-rw-   0        0        0      887 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GEOS/daily.py
+-rw-rw-rw-   0        0        0     1097 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GEOS/three_hourly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/GLDAS/
+-rw-rw-rw-   0        0        0    31339 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/CLSM_DataAccess.py
+-rw-rw-rw-   0        0        0     1032 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/CLSM_daily.py
+-rw-rw-rw-   0        0        0     1070 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/CLSM_monthly.py
+-rw-rw-rw-   0        0        0     1594 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/CLSM_three_hourly.py
+-rw-rw-rw-   0        0        0    30335 2019-11-05 17:25:12.000000 watertools-0.0.9/watertools/Collect/GLDAS/DataAccess.py
+-rw-rw-rw-   0        0        0    30301 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/NOAH_DataAccess.py
+-rw-rw-rw-   0        0        0     1588 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/NOAH_daily.py
+-rw-rw-rw-   0        0        0     1255 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/NOAH_monthly.py
+-rw-rw-rw-   0        0        0     1854 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/NOAH_three_hourly.py
+-rw-rw-rw-   0        0        0     2115 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/__init__.py
+-rw-rw-rw-   0        0        0     1573 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/daily.py
+-rw-rw-rw-   0        0        0     1245 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/monthly.py
+-rw-rw-rw-   0        0        0     1844 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLDAS/three_hourly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/GLEAM/
+-rw-rw-rw-   0        0        0     9602 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/DataAccess.py
+-rw-rw-rw-   0        0        0      909 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/ET_daily.py
+-rw-rw-rw-   0        0        0      891 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/ET_monthly.py
+-rw-rw-rw-   0        0        0      922 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/ETpot_daily.py
+-rw-rw-rw-   0        0        0      904 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/ETpot_monthly.py
+-rw-rw-rw-   0        0        0      999 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GLEAM/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/GPM/
+-rw-rw-rw-   0        0        0     6004 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GPM/DataAccess.py
+-rw-rw-rw-   0        0        0      874 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GPM/__init__.py
+-rw-rw-rw-   0        0        0      980 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GPM/daily.py
+-rw-rw-rw-   0        0        0      997 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/GPM/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/Globcover/
+-rw-rw-rw-   0        0        0     3104 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/Globcover/DataAccess.py
+-rw-rw-rw-   0        0        0     1130 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/Globcover/Landuse.py
+-rw-rw-rw-   0        0        0      490 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/Globcover/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/HiHydroSoil/
+-rw-rw-rw-   0        0        0     5076 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/HiHydroSoil/DataAccess.py
+-rw-rw-rw-   0        0        0      691 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/HiHydroSoil/ThetaSat_TopSoil.py
+-rw-rw-rw-   0        0        0      697 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/HiHydroSoil/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/JRC/
+-rw-rw-rw-   0        0        0     7770 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/JRC/DataAccess.py
+-rw-rw-rw-   0        0        0      585 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/JRC/Occurrence.py
+-rw-rw-rw-   0        0        0      566 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/JRC/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/L30/
+-rw-rw-rw-   0        0        0     3658 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/L30/DataAccess.py
+-rw-rw-rw-   0        0        0      819 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/L30/Harmonized.py
+-rw-rw-rw-   0        0        0      326 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/L30/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MCD43/
+-rw-rw-rw-   0        0        0      853 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MCD43/Albedo_daily.py
+-rw-rw-rw-   0        0        0    15811 2019-11-17 17:12:50.000000 watertools-0.0.9/watertools/Collect/MCD43/DataAccess.py
+-rw-rw-rw-   0        0        0      619 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MCD43/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MERRA/
+-rw-rw-rw-   0        0        0    15607 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/DataAccess.py
+-rw-rw-rw-   0        0        0     1140 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/__init__.py
+-rw-rw-rw-   0        0        0      919 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/daily.py
+-rw-rw-rw-   0        0        0      938 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/daily_MERRA2.py
+-rw-rw-rw-   0        0        0     1158 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/hourly_MERRA2.py
+-rw-rw-rw-   0        0        0     1121 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/three_hourly.py
+-rw-rw-rw-   0        0        0      929 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MERRA/yearly_T_Amplitude.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD10/
+-rw-rw-rw-   0        0        0    16313 2019-11-17 17:14:25.000000 watertools-0.0.9/watertools/Collect/MOD10/DataAccess.py
+-rw-rw-rw-   0        0        0      818 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD10/SnowMask_8daily.py
+-rw-rw-rw-   0        0        0      666 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD10/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD11/
+-rw-rw-rw-   0        0        0    21206 2019-11-17 17:15:15.000000 watertools-0.0.9/watertools/Collect/MOD11/DataAccess.py
+-rw-rw-rw-   0        0        0      863 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD11/LST_8daily.py
+-rw-rw-rw-   0        0        0      858 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD11/LST_daily.py
+-rw-rw-rw-   0        0        0      649 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD11/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD12/
+-rw-rw-rw-   0        0        0    14605 2019-11-17 17:17:09.000000 watertools-0.0.9/watertools/Collect/MOD12/DataAccess.py
+-rw-rw-rw-   0        0        0      889 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD12/LC_yearly.py
+-rw-rw-rw-   0        0        0      716 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD12/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD13/
+-rw-rw-rw-   0        0        0    16686 2019-11-17 17:16:53.000000 watertools-0.0.9/watertools/Collect/MOD13/DataAccess.py
+-rw-rw-rw-   0        0        0      814 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD13/NDVI_16daily.py
+-rw-rw-rw-   0        0        0      607 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD13/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD15/
+-rw-rw-rw-   0        0        0    21444 2019-11-17 17:12:42.000000 watertools-0.0.9/watertools/Collect/MOD15/DataAccess.py
+-rw-rw-rw-   0        0        0      861 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD15/FPAR_8daily.py
+-rw-rw-rw-   0        0        0      859 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD15/LAI_8daily.py
+-rw-rw-rw-   0        0        0      786 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD15/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD16/
+-rw-rw-rw-   0        0        0    17937 2019-11-17 17:17:57.000000 watertools-0.0.9/watertools/Collect/MOD16/DataAccess.py
+-rw-rw-rw-   0        0        0      974 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD16/ET_8daily.py
+-rw-rw-rw-   0        0        0      848 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD16/ET_monthly.py
+-rw-rw-rw-   0        0        0      650 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD16/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD17/
+-rw-rw-rw-   0        0        0    16769 2019-11-17 17:18:36.000000 watertools-0.0.9/watertools/Collect/MOD17/DataAccessGPP.py
+-rw-rw-rw-   0        0        0    15780 2019-11-17 17:19:11.000000 watertools-0.0.9/watertools/Collect/MOD17/DataAccessNPP.py
+-rw-rw-rw-   0        0        0      822 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD17/GPP_8daily.py
+-rw-rw-rw-   0        0        0      818 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD17/NPP_yearly.py
+-rw-rw-rw-   0        0        0      779 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD17/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MOD9/
+-rw-rw-rw-   0        0        0    15347 2019-11-17 17:13:30.000000 watertools-0.0.9/watertools/Collect/MOD9/DataAccess.py
+-rw-rw-rw-   0        0        0      874 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD9/REF_daily.py
+-rw-rw-rw-   0        0        0      599 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MOD9/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MSGCPP/
+-rw-rw-rw-   0        0        0     3707 2019-11-03 19:00:39.000000 watertools-0.0.9/watertools/Collect/MSGCPP/DataAccess.py
+-rw-rw-rw-   0        0        0      937 2019-10-31 07:49:40.000000 watertools-0.0.9/watertools/Collect/MSGCPP/SDS.py
+-rw-rw-rw-   0        0        0      686 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MSGCPP/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MSWEP/
+-rw-rw-rw-   0        0        0    10055 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MSWEP/DataAccess.py
+-rw-rw-rw-   0        0        0      719 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MSWEP/__init__.py
+-rw-rw-rw-   0        0        0      847 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MSWEP/daily.py
+-rw-rw-rw-   0        0        0      848 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MSWEP/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MYD11/
+-rw-rw-rw-   0        0        0    19339 2019-11-17 17:19:53.000000 watertools-0.0.9/watertools/Collect/MYD11/DataAccess.py
+-rw-rw-rw-   0        0        0     1082 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MYD11/LST_daily.py
+-rw-rw-rw-   0        0        0      587 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MYD11/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/MYD13/
+-rw-rw-rw-   0        0        0    16792 2019-11-17 17:20:30.000000 watertools-0.0.9/watertools/Collect/MYD13/DataAccess.py
+-rw-rw-rw-   0        0        0      814 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MYD13/NDVI_16daily.py
+-rw-rw-rw-   0        0        0      607 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/MYD13/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/NLDAS/
+-rw-rw-rw-   0        0        0    35162 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/DataAccess.py
+-rw-rw-rw-   0        0        0    22946 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/FORA_DataAccess.py
+-rw-rw-rw-   0        0        0     1346 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/FORA_daily.py
+-rw-rw-rw-   0        0        0     1508 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/FORA_hourly.py
+-rw-rw-rw-   0        0        0     1041 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/FORA_monthly.py
+-rw-rw-rw-   0        0        0     1737 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/__init__.py
+-rw-rw-rw-   0        0        0     1346 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/daily.py
+-rw-rw-rw-   0        0        0     1456 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/hourly.py
+-rw-rw-rw-   0        0        0     1041 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/NLDAS/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/PROBAV/
+-rw-rw-rw-   0        0        0    14349 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/PROBAV/DataAccess.py
+-rw-rw-rw-   0        0        0      666 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/PROBAV/__init__.py
+-rw-rw-rw-   0        0        0      968 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/PROBAV/five_daily.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/RFE/
+-rw-rw-rw-   0        0        0     5375 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/RFE/DataAccess.py
+-rw-rw-rw-   0        0        0      857 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/RFE/__init__.py
+-rw-rw-rw-   0        0        0      963 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/RFE/daily.py
+-rw-rw-rw-   0        0        0     3493 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/RFE/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/S30/
+-rw-rw-rw-   0        0        0     3551 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/S30/DataAccess.py
+-rw-rw-rw-   0        0        0      819 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/S30/Harmonized.py
+-rw-rw-rw-   0        0        0      326 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/S30/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/SEBS/
+-rw-rw-rw-   0        0        0     5631 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SEBS/DataAccess.py
+-rw-rw-rw-   0        0        0      745 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SEBS/__init__.py
+-rw-rw-rw-   0        0        0      820 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SEBS/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/SSEBop/
+-rw-rw-rw-   0        0        0    10921 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SSEBop/DataAccess.py
+-rw-rw-rw-   0        0        0      886 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SSEBop/ET_monthly.py
+-rw-rw-rw-   0        0        0      906 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SSEBop/ETpot_daily.py
+-rw-rw-rw-   0        0        0      917 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SSEBop/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/SoilGrids/
+-rw-rw-rw-   0        0        0     1783 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Absolute_Depth_To_Bedrock.py
+-rw-rw-rw-   0        0        0     1953 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Bulk_Density.py
+-rw-rw-rw-   0        0        0     2096 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Clay_Content.py
+-rw-rw-rw-   0        0        0     2036 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Coarse_Fragment_Volumetric.py
+-rw-rw-rw-   0        0        0     3047 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/DataAccess.py
+-rw-rw-rw-   0        0        0     1749 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Depth_To_Bedrock.py
+-rw-rw-rw-   0        0        0     2026 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Organic_Carbon_Content.py
+-rw-rw-rw-   0        0        0     2019 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Organic_Carbon_Stock.py
+-rw-rw-rw-   0        0        0     1829 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Predicted_Probability_Of_Occurrence.py
+-rw-rw-rw-   0        0        0     2017 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Sand_Content.py
+-rw-rw-rw-   0        0        0     2017 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Silt_Content.py
+-rw-rw-rw-   0        0        0     1967 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/Soil_pH.py
+-rw-rw-rw-   0        0        0     1143 2019-10-26 11:54:10.000000 watertools-0.0.9/watertools/Collect/SoilGrids/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/TRMM/
+-rw-rw-rw-   0        0        0     6228 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TRMM/DataAccess.py
+-rw-rw-rw-   0        0        0      813 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TRMM/__init__.py
+-rw-rw-rw-   0        0        0      990 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TRMM/daily.py
+-rw-rw-rw-   0        0        0     1007 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TRMM/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Collect/TWC/
+-rw-rw-rw-   0        0        0     4285 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TWC/DataAccess.py
+-rw-rw-rw-   0        0        0      527 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TWC/Gray_Water_Footprint.py
+-rw-rw-rw-   0        0        0      970 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/TWC/__init__.py
+-rw-rw-rw-   0        0        0     4162 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Collect/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Functions/
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Functions/Area_Conversions/
+-rw-rw-rw-   0        0        0     3132 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Area_Conversions/Area_converter.py
+-rw-rw-rw-   0        0        0     2248 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Area_Conversions/Boundaries.py
+-rw-rw-rw-   0        0        0      257 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Area_Conversions/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Functions/Random/
+-rw-rw-rw-   0        0        0      954 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Random/WaitbarConsole.py
+-rw-rw-rw-   0        0        0      221 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Random/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/
+-rw-rw-rw-   0        0        0     2794 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/Day_to_monthly_flux.py
+-rw-rw-rw-   0        0        0     5069 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/Eightdaily_to_monthly_state.py
+-rw-rw-rw-   0        0        0     2488 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/Monthly_to_yearly_flux.py
+-rw-rw-rw-   0        0        0     5084 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/Sixteendaily_to_monthly_state.py
+-rw-rw-rw-   0        0        0     5236 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/Weekly_to_monthly_flux.py
+-rw-rw-rw-   0        0        0      416 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Time_Conversions/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Functions/Visualization/
+-rw-rw-rw-   0        0        0     5032 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Visualization/Compare_Rasters_One_Point.py
+-rw-rw-rw-   0        0        0     3540 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Visualization/Compare_Rasters_One_Polygon.py
+-rw-rw-rw-   0        0        0      308 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/Visualization/__init__.py
+-rw-rw-rw-   0        0        0      359 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Functions/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/General/
+-rw-rw-rw-   0        0        0      317 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/General/__init__.py
+-rw-rw-rw-   0        0        0    19798 2019-11-13 14:06:12.000000 watertools-0.0.9/watertools/General/data_conversions.py
+-rw-rw-rw-   0        0        0    39673 2019-11-07 14:27:11.000000 watertools-0.0.9/watertools/General/raster_conversions.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Products/
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Products/ETens/
+-rw-rw-rw-   0        0        0     9205 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETens/DataAccess.py
+-rw-rw-rw-   0        0        0      582 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETens/__init__.py
+-rw-rw-rw-   0        0        0     1563 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETens/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Products/ETref/
+-rw-rw-rw-   0        0        0     5896 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/CalcETref.py
+-rw-rw-rw-   0        0        0     1785 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/CollectDataETref.py
+-rw-rw-rw-   0        0        0     7840 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/CollectLANDSAFETref.py
+-rw-rw-rw-   0        0        0     6601 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/Interpolate_Meteo_ETref.py
+-rw-rw-rw-   0        0        0     6368 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/SetVarETref.py
+-rw-rw-rw-   0        0        0    15848 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/SlopeInfluence_ETref.py
+-rw-rw-rw-   0        0        0     1492 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/__init__.py
+-rw-rw-rw-   0        0        0     2403 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/daily.py
+-rw-rw-rw-   0        0        0     3673 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/ETref/monthly.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools/Products/SoilGrids/
+-rw-rw-rw-   0        0        0     1278 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/K_Sat.py
+-rw-rw-rw-   0        0        0     4195 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/Theta_FC.py
+-rw-rw-rw-   0        0        0     2962 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/Theta_Res.py
+-rw-rw-rw-   0        0        0     3933 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/Theta_Sat.py
+-rw-rw-rw-   0        0        0     3977 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/Theta_Sat2.py
+-rw-rw-rw-   0        0        0     2974 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/Water_Holding_Capacity.py
+-rw-rw-rw-   0        0        0      878 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/__init__.py
+-rw-rw-rw-   0        0        0     2859 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/SoilGrids/n_van_genuchten.py
+-rw-rw-rw-   0        0        0      756 2019-10-26 11:54:11.000000 watertools-0.0.9/watertools/Products/__init__.py
+-rw-rw-rw-   0        0        0      452 2019-10-20 11:25:28.000000 watertools-0.0.9/watertools/WebAccounts.py
+-rw-rw-rw-   0        0        0      201 2018-12-29 18:43:46.000000 watertools-0.0.9/watertools/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools.egg-info/
+-rw-rw-rw-   0        0        0      694 2019-11-17 21:55:07.000000 watertools-0.0.9/watertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9150 2019-11-17 21:55:08.000000 watertools-0.0.9/watertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-11-17 21:55:07.000000 watertools-0.0.9/watertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2019-11-17 21:55:07.000000 watertools-0.0.9/watertools.egg-info/top_level.txt
```

### Comparing `watertools-0.0.8/PKG-INFO` & `watertools-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watertools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for data collecting and data processing of remote sensed data.
 Home-page: https://github.com/TimHessels/watertools
 Author: Tim Hessels
 Author-email: timhessels@hotmail.com
 License: UNKNOWN
 Description: # Water toolbox
```

### Comparing `watertools-0.0.8/setup.py` & `watertools-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="watertools",
-    version="0.0.8",
+    version="0.0.9",
     author="Tim Hessels",
     author_email="timhessels@hotmail.com",
     description="Tools for data collecting and data processing of remote sensed data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TimHessels/watertools",
     packages=setuptools.find_packages(),
```

### Comparing `watertools-0.0.8/watertools/Collect/ALEXI/DataAccess.py` & `watertools-0.0.9/watertools/Collect/ALEXI/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ALEXI/__init__.py` & `watertools-0.0.9/watertools/Collect/ALEXI/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ALEXI/daily.py` & `watertools-0.0.9/watertools/Collect/ALEXI/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ALEXI/monthly.py` & `watertools-0.0.9/watertools/Collect/ALEXI/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ALEXI/weekly.py` & `watertools-0.0.9/watertools/Collect/ALEXI/weekly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ASCAT/DataAccess.py` & `watertools-0.0.9/watertools/Collect/ASCAT/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ASCAT/daily.py` & `watertools-0.0.9/watertools/Collect/ASCAT/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CFSR/DataAccess_CFSR.py` & `watertools-0.0.9/watertools/Collect/CFSR/DataAccess_CFSR.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CFSR/Download_data_CFSR.py` & `watertools-0.0.9/watertools/Collect/CFSR/Download_data_CFSR.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CFSR/__init__.py` & `watertools-0.0.9/watertools/Collect/CFSR/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CFSR/daily.py` & `watertools-0.0.9/watertools/Collect/CFSR/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CHIRPS/DataAccess.py` & `watertools-0.0.9/watertools/Collect/CHIRPS/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CHIRPS/__init__.py` & `watertools-0.0.9/watertools/Collect/CHIRPS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CHIRPS/daily.py` & `watertools-0.0.9/watertools/Collect/CHIRPS/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CHIRPS/monthly.py` & `watertools-0.0.9/watertools/Collect/CHIRPS/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CMRSET/DataAccess.py` & `watertools-0.0.9/watertools/Collect/CMRSET/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CMRSET/__init__.py` & `watertools-0.0.9/watertools/Collect/CMRSET/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/CMRSET/monthly.py` & `watertools-0.0.9/watertools/Collect/CMRSET/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/DataAccess_Hydro.py` & `watertools-0.0.9/watertools/Collect/DEM/DataAccess_Hydro.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/DataAccess_SRTM.py` & `watertools-0.0.9/watertools/Collect/DEM/DataAccess_SRTM.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/HydroSHED.py` & `watertools-0.0.9/watertools/Collect/DEM/HydroSHED.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/HydroSHED_Dir.py` & `watertools-0.0.9/watertools/Collect/DEM/HydroSHED_Dir.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/SRTM.py` & `watertools-0.0.9/watertools/Collect/DEM/SRTM.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/DEM/__init__.py` & `watertools-0.0.9/watertools/Collect/DEM/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ECMWF/DataAccess.py` & `watertools-0.0.9/watertools/Collect/ECMWF/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ECMWF/ECMWFdownload.py` & `watertools-0.0.9/watertools/Collect/ECMWF/ECMWFdownload.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ECMWF/__init__.py` & `watertools-0.0.9/watertools/Collect/ECMWF/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ECMWF/daily.py` & `watertools-0.0.9/watertools/Collect/ECMWF/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ECMWF/monthly.py` & `watertools-0.0.9/watertools/Collect/ECMWF/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ESACCI/DataAccess.py` & `watertools-0.0.9/watertools/Collect/ESACCI/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ESACCI/LU.py` & `watertools-0.0.9/watertools/Collect/ESACCI/LU.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/DataAccess.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/ET_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/ET_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/ETpot_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/ETpot_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/Ei_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/Ei_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/Es_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/Es_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/Ew_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/Ew_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/Tr_monthly.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/Tr_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/ETmonitor/__init__.py` & `watertools-0.0.9/watertools/Collect/ETmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/FEWS/ETpot_daily.py` & `watertools-0.0.9/watertools/Collect/FEWS/ETpot_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/FEWS/__init__.py` & `watertools-0.0.9/watertools/Collect/FEWS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GEOS/DataAccess.py` & `watertools-0.0.9/watertools/Collect/GEOS/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GEOS/__init__.py` & `watertools-0.0.9/watertools/Collect/GEOS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GEOS/daily.py` & `watertools-0.0.9/watertools/Collect/GEOS/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GEOS/three_hourly.py` & `watertools-0.0.9/watertools/Collect/GEOS/three_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/CLSM_DataAccess.py` & `watertools-0.0.9/watertools/Collect/GLDAS/CLSM_DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/CLSM_daily.py` & `watertools-0.0.9/watertools/Collect/GLDAS/CLSM_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/CLSM_monthly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/CLSM_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/CLSM_three_hourly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/CLSM_three_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/DataAccess.py` & `watertools-0.0.9/watertools/Collect/GLDAS/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/NOAH_DataAccess.py` & `watertools-0.0.9/watertools/Collect/GLDAS/NOAH_DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/NOAH_daily.py` & `watertools-0.0.9/watertools/Collect/GLDAS/NOAH_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/NOAH_monthly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/NOAH_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/NOAH_three_hourly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/NOAH_three_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/__init__.py` & `watertools-0.0.9/watertools/Collect/GLDAS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/daily.py` & `watertools-0.0.9/watertools/Collect/GLDAS/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/monthly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLDAS/three_hourly.py` & `watertools-0.0.9/watertools/Collect/GLDAS/three_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/DataAccess.py` & `watertools-0.0.9/watertools/Collect/GLEAM/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/ET_daily.py` & `watertools-0.0.9/watertools/Collect/GLEAM/ET_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/ET_monthly.py` & `watertools-0.0.9/watertools/Collect/GLEAM/ET_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/ETpot_daily.py` & `watertools-0.0.9/watertools/Collect/GLEAM/ETpot_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/ETpot_monthly.py` & `watertools-0.0.9/watertools/Collect/GLEAM/ETpot_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GLEAM/__init__.py` & `watertools-0.0.9/watertools/Collect/GLEAM/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GPM/DataAccess.py` & `watertools-0.0.9/watertools/Collect/GPM/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GPM/__init__.py` & `watertools-0.0.9/watertools/Collect/GPM/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GPM/daily.py` & `watertools-0.0.9/watertools/Collect/GPM/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/GPM/monthly.py` & `watertools-0.0.9/watertools/Collect/GPM/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/Globcover/DataAccess.py` & `watertools-0.0.9/watertools/Collect/Globcover/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/Globcover/Landuse.py` & `watertools-0.0.9/watertools/Collect/Globcover/Landuse.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/HiHydroSoil/DataAccess.py` & `watertools-0.0.9/watertools/Collect/HiHydroSoil/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/HiHydroSoil/ThetaSat_TopSoil.py` & `watertools-0.0.9/watertools/Collect/HiHydroSoil/ThetaSat_TopSoil.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/HiHydroSoil/__init__.py` & `watertools-0.0.9/watertools/Collect/HiHydroSoil/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/JRC/DataAccess.py` & `watertools-0.0.9/watertools/Collect/JRC/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/JRC/Occurrence.py` & `watertools-0.0.9/watertools/Collect/JRC/Occurrence.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/JRC/__init__.py` & `watertools-0.0.9/watertools/Collect/JRC/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/L30/DataAccess.py` & `watertools-0.0.9/watertools/Collect/L30/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/L30/Harmonized.py` & `watertools-0.0.9/watertools/Collect/L30/Harmonized.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MCD43/Albedo_daily.py` & `watertools-0.0.9/watertools/Collect/MCD43/Albedo_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MCD43/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MCD43/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MCD43/__init__.py` & `watertools-0.0.9/watertools/Collect/MCD43/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MERRA/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/__init__.py` & `watertools-0.0.9/watertools/Collect/MERRA/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/daily.py` & `watertools-0.0.9/watertools/Collect/MERRA/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/daily_MERRA2.py` & `watertools-0.0.9/watertools/Collect/MERRA/daily_MERRA2.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/hourly_MERRA2.py` & `watertools-0.0.9/watertools/Collect/MERRA/hourly_MERRA2.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/three_hourly.py` & `watertools-0.0.9/watertools/Collect/MERRA/three_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MERRA/yearly_T_Amplitude.py` & `watertools-0.0.9/watertools/Collect/MERRA/yearly_T_Amplitude.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD10/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD10/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD10/SnowMask_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD10/SnowMask_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD10/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD10/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD11/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD11/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD11/LST_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD11/LST_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD11/LST_daily.py` & `watertools-0.0.9/watertools/Collect/MOD11/LST_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD11/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD11/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD12/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD12/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD12/LC_yearly.py` & `watertools-0.0.9/watertools/Collect/MOD12/LC_yearly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD12/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD12/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD13/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD13/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD13/NDVI_16daily.py` & `watertools-0.0.9/watertools/Collect/MOD13/NDVI_16daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD13/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD13/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD15/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD15/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD15/FPAR_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD15/FPAR_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD15/LAI_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD15/LAI_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD15/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD15/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD16/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD16/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD16/ET_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD16/ET_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD16/ET_monthly.py` & `watertools-0.0.9/watertools/Collect/MOD16/ET_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD16/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD16/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD17/DataAccessGPP.py` & `watertools-0.0.9/watertools/Collect/MOD17/DataAccessGPP.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD17/DataAccessNPP.py` & `watertools-0.0.9/watertools/Collect/MOD17/DataAccessNPP.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD17/GPP_8daily.py` & `watertools-0.0.9/watertools/Collect/MOD17/GPP_8daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD17/NPP_yearly.py` & `watertools-0.0.9/watertools/Collect/MOD17/NPP_yearly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD17/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD17/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD9/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MOD9/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD9/REF_daily.py` & `watertools-0.0.9/watertools/Collect/MOD9/REF_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MOD9/__init__.py` & `watertools-0.0.9/watertools/Collect/MOD9/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSGCPP/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MSGCPP/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSGCPP/SDS.py` & `watertools-0.0.9/watertools/Collect/MSGCPP/SDS.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSGCPP/__init__.py` & `watertools-0.0.9/watertools/Collect/MSGCPP/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSWEP/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MSWEP/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSWEP/__init__.py` & `watertools-0.0.9/watertools/Collect/MSWEP/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSWEP/daily.py` & `watertools-0.0.9/watertools/Collect/MSWEP/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MSWEP/monthly.py` & `watertools-0.0.9/watertools/Collect/MSWEP/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD11/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MYD11/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD11/LST_daily.py` & `watertools-0.0.9/watertools/Collect/MYD11/LST_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD11/__init__.py` & `watertools-0.0.9/watertools/Collect/MYD11/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD13/DataAccess.py` & `watertools-0.0.9/watertools/Collect/MYD13/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD13/NDVI_16daily.py` & `watertools-0.0.9/watertools/Collect/MYD13/NDVI_16daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/MYD13/__init__.py` & `watertools-0.0.9/watertools/Collect/MYD13/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/DataAccess.py` & `watertools-0.0.9/watertools/Collect/NLDAS/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/FORA_DataAccess.py` & `watertools-0.0.9/watertools/Collect/NLDAS/FORA_DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/FORA_daily.py` & `watertools-0.0.9/watertools/Collect/NLDAS/FORA_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/FORA_hourly.py` & `watertools-0.0.9/watertools/Collect/NLDAS/FORA_hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/FORA_monthly.py` & `watertools-0.0.9/watertools/Collect/NLDAS/FORA_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/__init__.py` & `watertools-0.0.9/watertools/Collect/NLDAS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/daily.py` & `watertools-0.0.9/watertools/Collect/NLDAS/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/hourly.py` & `watertools-0.0.9/watertools/Collect/NLDAS/hourly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/NLDAS/monthly.py` & `watertools-0.0.9/watertools/Collect/NLDAS/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/PROBAV/DataAccess.py` & `watertools-0.0.9/watertools/Collect/PROBAV/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/PROBAV/__init__.py` & `watertools-0.0.9/watertools/Collect/PROBAV/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/PROBAV/five_daily.py` & `watertools-0.0.9/watertools/Collect/PROBAV/five_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/RFE/DataAccess.py` & `watertools-0.0.9/watertools/Collect/RFE/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/RFE/__init__.py` & `watertools-0.0.9/watertools/Collect/RFE/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/RFE/daily.py` & `watertools-0.0.9/watertools/Collect/RFE/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/RFE/monthly.py` & `watertools-0.0.9/watertools/Collect/RFE/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/S30/DataAccess.py` & `watertools-0.0.9/watertools/Collect/S30/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/S30/Harmonized.py` & `watertools-0.0.9/watertools/Collect/S30/Harmonized.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SEBS/DataAccess.py` & `watertools-0.0.9/watertools/Collect/SEBS/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SEBS/__init__.py` & `watertools-0.0.9/watertools/Collect/SEBS/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SEBS/monthly.py` & `watertools-0.0.9/watertools/Collect/SEBS/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SSEBop/DataAccess.py` & `watertools-0.0.9/watertools/Collect/SSEBop/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SSEBop/ET_monthly.py` & `watertools-0.0.9/watertools/Collect/SSEBop/ET_monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SSEBop/ETpot_daily.py` & `watertools-0.0.9/watertools/Collect/SSEBop/ETpot_daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SSEBop/__init__.py` & `watertools-0.0.9/watertools/Collect/SSEBop/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Absolute_Depth_To_Bedrock.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Absolute_Depth_To_Bedrock.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Bulk_Density.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Bulk_Density.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Clay_Content.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Clay_Content.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Coarse_Fragment_Volumetric.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Coarse_Fragment_Volumetric.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/DataAccess.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Depth_To_Bedrock.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Depth_To_Bedrock.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Organic_Carbon_Content.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Organic_Carbon_Content.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Organic_Carbon_Stock.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Organic_Carbon_Stock.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Predicted_Probability_Of_Occurrence.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Predicted_Probability_Of_Occurrence.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Sand_Content.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Sand_Content.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Silt_Content.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Silt_Content.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/Soil_pH.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/Soil_pH.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/SoilGrids/__init__.py` & `watertools-0.0.9/watertools/Collect/SoilGrids/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TRMM/DataAccess.py` & `watertools-0.0.9/watertools/Collect/TRMM/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TRMM/__init__.py` & `watertools-0.0.9/watertools/Collect/TRMM/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TRMM/daily.py` & `watertools-0.0.9/watertools/Collect/TRMM/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TRMM/monthly.py` & `watertools-0.0.9/watertools/Collect/TRMM/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TWC/DataAccess.py` & `watertools-0.0.9/watertools/Collect/TWC/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TWC/Gray_Water_Footprint.py` & `watertools-0.0.9/watertools/Collect/TWC/Gray_Water_Footprint.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/TWC/__init__.py` & `watertools-0.0.9/watertools/Collect/TWC/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Collect/__init__.py` & `watertools-0.0.9/watertools/Collect/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Area_Conversions/Area_converter.py` & `watertools-0.0.9/watertools/Functions/Area_Conversions/Area_converter.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Area_Conversions/Boundaries.py` & `watertools-0.0.9/watertools/Functions/Area_Conversions/Boundaries.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Random/WaitbarConsole.py` & `watertools-0.0.9/watertools/Functions/Random/WaitbarConsole.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Time_Conversions/Day_to_monthly_flux.py` & `watertools-0.0.9/watertools/Functions/Time_Conversions/Day_to_monthly_flux.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Time_Conversions/Eightdaily_to_monthly_state.py` & `watertools-0.0.9/watertools/Functions/Time_Conversions/Eightdaily_to_monthly_state.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Time_Conversions/Monthly_to_yearly_flux.py` & `watertools-0.0.9/watertools/Functions/Time_Conversions/Monthly_to_yearly_flux.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Time_Conversions/Sixteendaily_to_monthly_state.py` & `watertools-0.0.9/watertools/Functions/Time_Conversions/Sixteendaily_to_monthly_state.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Time_Conversions/Weekly_to_monthly_flux.py` & `watertools-0.0.9/watertools/Functions/Time_Conversions/Weekly_to_monthly_flux.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Visualization/Compare_Rasters_One_Point.py` & `watertools-0.0.9/watertools/Functions/Visualization/Compare_Rasters_One_Point.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Functions/Visualization/Compare_Rasters_One_Polygon.py` & `watertools-0.0.9/watertools/Functions/Visualization/Compare_Rasters_One_Polygon.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/General/data_conversions.py` & `watertools-0.0.9/watertools/General/data_conversions.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/General/raster_conversions.py` & `watertools-0.0.9/watertools/General/raster_conversions.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETens/DataAccess.py` & `watertools-0.0.9/watertools/Products/ETens/DataAccess.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETens/__init__.py` & `watertools-0.0.9/watertools/Products/ETens/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETens/monthly.py` & `watertools-0.0.9/watertools/Products/ETens/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/CalcETref.py` & `watertools-0.0.9/watertools/Products/ETref/CalcETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/CollectDataETref.py` & `watertools-0.0.9/watertools/Products/ETref/CollectDataETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/CollectLANDSAFETref.py` & `watertools-0.0.9/watertools/Products/ETref/CollectLANDSAFETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/Interpolate_Meteo_ETref.py` & `watertools-0.0.9/watertools/Products/ETref/Interpolate_Meteo_ETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/SetVarETref.py` & `watertools-0.0.9/watertools/Products/ETref/SetVarETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/SlopeInfluence_ETref.py` & `watertools-0.0.9/watertools/Products/ETref/SlopeInfluence_ETref.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/__init__.py` & `watertools-0.0.9/watertools/Products/ETref/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/daily.py` & `watertools-0.0.9/watertools/Products/ETref/daily.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/ETref/monthly.py` & `watertools-0.0.9/watertools/Products/ETref/monthly.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/K_Sat.py` & `watertools-0.0.9/watertools/Products/SoilGrids/K_Sat.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/Theta_FC.py` & `watertools-0.0.9/watertools/Products/SoilGrids/Theta_FC.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/Theta_Res.py` & `watertools-0.0.9/watertools/Products/SoilGrids/Theta_Res.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/Theta_Sat.py` & `watertools-0.0.9/watertools/Products/SoilGrids/Theta_Sat.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/Theta_Sat2.py` & `watertools-0.0.9/watertools/Products/SoilGrids/Theta_Sat2.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/Water_Holding_Capacity.py` & `watertools-0.0.9/watertools/Products/SoilGrids/Water_Holding_Capacity.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/__init__.py` & `watertools-0.0.9/watertools/Products/SoilGrids/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/SoilGrids/n_van_genuchten.py` & `watertools-0.0.9/watertools/Products/SoilGrids/n_van_genuchten.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools/Products/__init__.py` & `watertools-0.0.9/watertools/Products/__init__.py`

 * *Files identical despite different names*

### Comparing `watertools-0.0.8/watertools.egg-info/PKG-INFO` & `watertools-0.0.9/watertools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watertools
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for data collecting and data processing of remote sensed data.
 Home-page: https://github.com/TimHessels/watertools
 Author: Tim Hessels
 Author-email: timhessels@hotmail.com
 License: UNKNOWN
 Description: # Water toolbox
```

### Comparing `watertools-0.0.8/watertools.egg-info/SOURCES.txt` & `watertools-0.0.9/watertools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

