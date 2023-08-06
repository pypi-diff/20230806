# Comparing `tmp/osm-fieldwork-0.3.3.tar.gz` & `tmp/osm-fieldwork-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.3.3.tar", last modified: Tue Jul 25 20:55:00 2023, max compression
+gzip compressed data, was "osm-fieldwork-0.3.4.tar", last modified: Sun Aug  6 19:57:32 2023, max compression
```

## Comparing `osm-fieldwork-0.3.3.tar` & `osm-fieldwork-0.3.4.tar`

### file list

```diff
@@ -1,96 +1,98 @@
--rw-r--r--   0        0        0    34625 2023-07-25 20:54:52.845209 osm-fieldwork-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     8656 2023-07-25 20:54:52.845209 osm-fieldwork-0.3.3/README.md
--rwxr-xr-x   0        0        0    13130 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5099 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     4400 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4205 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    27539 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/OdkCentral.py
--rw-r--r--   0        0        0        0 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0     9940 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0     9941 2023-07-25 20:54:52.849209 osm-fieldwork-0.3.3/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      504 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      349 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      240 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      678 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      119 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      412 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      137 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      495 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0       94 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0      106 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0      104 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0      107 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0        0 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/taginfo-db.db
--rw-r--r--   0        0        0      245 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4745 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      348 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      170 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      140 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     7378 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/filter_data.py
--rwxr-xr-x   0        0        0    16103 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0      442 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/main.py
--rwxr-xr-x   0        0        0    21353 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/make_data_extract.py
--rw-r--r--   0        0        0     3896 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/models.yaml
--rwxr-xr-x   0        0        0     5284 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4224 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0     5235 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk2osm.py
--rwxr-xr-x   0        0        0    15611 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0    21645 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5336 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    13082 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     8003 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     3757 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0       81 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/.~lock.test.xls#
--rw-r--r--   0        0        0     3795 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0      830 2023-07-25 20:54:52.853209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2023-07-25 20:54:52.857209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2023-07-25 20:54:52.861209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0    69120 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    22528 2023-07-25 20:54:52.869209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0   115963 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   265216 2023-07-25 20:54:52.873209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/test.xls
--rw-r--r--   0        0        0   353280 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/thamel.xls
--rw-r--r--   0        0        0   118272 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     3726 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     2106 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       32 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/.flake8
--rw-r--r--   0        0        0      574 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/Test.yaml
--rw-r--r--   0        0        0     2713 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test.csv
--rwxr-xr-x   0        0        0     3817 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_conflation.py
--rwxr-xr-x   0        0        0     2427 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_convert.py
--rwxr-xr-x   0        0        0     2076 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_csv.py
--rwxr-xr-x   0        0        0     3473 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_osm.py
--rwxr-xr-x   0        0        0     2992 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_uriparser.py
--rwxr-xr-x   0        0        0     1697 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/test_yaml.py
--rw-r--r--   0        0        0    12719 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/Salida.geojson
--rw-r--r--   0        0        0     5601 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/odk_pois.osm
--rw-r--r--   0        0        0   129410 2023-07-25 20:54:52.877209 osm-fieldwork-0.3.3/tests/testdata/osm_buildings.geojson
--rw-r--r--   0        0        0     9343 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34625 2023-08-06 19:57:23.991866 osm-fieldwork-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0     8656 2023-08-06 19:57:23.991866 osm-fieldwork-0.3.4/README.md
+-rwxr-xr-x   0        0        0    13130 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5099 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     4400 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4205 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    31363 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/OdkCentral.py
+-rw-r--r--   0        0        0        0 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0     9940 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0     9801 2023-08-06 19:57:23.999867 osm-fieldwork-0.3.4/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      504 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      349 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      240 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      741 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      119 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      412 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      137 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      495 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0      180 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/highways.yaml
+-rw-r--r--   0        0        0       94 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0      106 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0      104 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0      107 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0        0 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/taginfo-db.db
+-rw-r--r--   0        0        0      245 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4745 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      348 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      170 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      140 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     7532 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/filter_data.py
+-rwxr-xr-x   0        0        0    14233 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0      442 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/main.py
+-rwxr-xr-x   0        0        0    21750 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/make_data_extract.py
+-rw-r--r--   0        0        0     3896 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/models.yaml
+-rwxr-xr-x   0        0        0     5284 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4215 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0     5235 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/odk2osm.py
+-rwxr-xr-x   0        0        0    18014 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0    21591 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5336 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    13335 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     8003 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     3420 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3795 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0      830 2023-08-06 19:57:24.003867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2023-08-06 19:57:24.007867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2023-08-06 19:57:24.007867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0    69120 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    40448 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/highways.xls
+-rw-r--r--   0        0        0    22528 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2023-08-06 19:57:24.019867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   265216 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/test.xls
+-rw-r--r--   0        0        0   353280 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/thamel.xls
+-rw-r--r--   0        0        0   118272 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2023-08-06 19:57:24.023867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     4069 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     2163 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/.flake8
+-rw-r--r--   0        0        0      574 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/Test.yaml
+-rw-r--r--   0        0        0     2713 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test.csv
+-rwxr-xr-x   0        0        0     3823 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_conflation.py
+-rwxr-xr-x   0        0        0     2900 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_convert.py
+-rwxr-xr-x   0        0        0     2076 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_csv.py
+-rwxr-xr-x   0        0        0     3473 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_osm.py
+-rwxr-xr-x   0        0        0     2992 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_uriparser.py
+-rwxr-xr-x   0        0        0     2260 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/test_yaml.py
+-rw-r--r--   0        0        0    12719 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/testdata/Salida.geojson
+-rw-r--r--   0        0        0     5601 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/testdata/odk_pois.osm
+-rw-r--r--   0        0        0   129410 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/testdata/osm_buildings.geojson
+-rw-r--r--   0        0        0   246174 2023-08-06 19:57:24.027867 osm-fieldwork-0.3.4/tests/testdata/testcamps.json
+-rw-r--r--   0        0        0     9343 1970-01-01 00:00:00.000000 osm-fieldwork-0.3.4/PKG-INFO
```

### Comparing `osm-fieldwork-0.3.3/LICENSE.md` & `osm-fieldwork-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/README.md` & `osm-fieldwork-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.3.4/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.3.4/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.3.4/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.3.4/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.3.4/osm_fieldwork/OdkCentral.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,51 @@
 from requests.auth import HTTPBasicAuth
 import json
 import zlib
 from datetime import datetime
 from base64 import b64encode
 import segno
 import zlib
+import re
+from shapely.geometry import Point
+from geojson import Feature, FeatureCollection, dump
+from cpuinfo import get_cpu_info
+from time import sleep
+from codetiming import Timer
+import concurrent.futures
+
 
 # Set log level for urllib
 log_level = os.getenv("LOG_LEVEL", default="INFO")
 logging.getLogger("urllib3").setLevel(log_level)
 
 log = logging.getLogger(__name__)
 
+def downloadThread(
+        project_id: int,
+        xforms: list,
+):
+    """Download a list of submissions from ODK Central"""
+    timer = Timer(text="downloadThread() took {seconds:.0f}s")
+    timer.start()
+    data = list()
+    # log.debug(f"downloadThread() called! {len(xforms)} xforms")
+    for task in xforms:
+        form = OdkForm()
+        submissions = form.getSubmissions(project_id, task['xmlFormId'], 0, False, True)
+        subs = form.listSubmissions(project_id, task['xmlFormId'])
+        if type(subs) == dict:
+            log.error(f"{subs['message']}, {subs['code']} ")
+            continue
+        # log.debug(f"There are {len(subs)} submissions for {task['xmlFormId']}")
+        if len(subs) > 0:
+            data += subs
+    # log.debug(f"There are {len(xforms)} Xforms, and {len(submissions)} submissions total")
+    timer.stop()
+    return data
 
 class OdkCentral(object):
     def __init__(self,
                  url: str = None,
                  user: str = None,
                  passwd: str = None
                  ):
@@ -68,15 +98,15 @@
             "form_update_mode": "match_exactly",
             "autosend": "wifi_and_cellular",
         }
         # If there is a config file with authentication setting, use that
         # so we don't have to supply this all the time. This is only used
         # when odk_client is used, and no parameters are passed in.
         if not self.url:
-            log.debug("Configuring ODKCentral from file .odkcentral")
+            # log.debug("Configuring ODKCentral from file .odkcentral")
             home = os.getenv("HOME")
             config = ".odkcentral"
             filespec = home + "/" + config
             if os.path.exists(filespec):
                 file = open(filespec, "r")
                 for line in file:
                     # Support embedded comments
@@ -92,26 +122,29 @@
                         self.passwd = tmp[1].strip("\n")
             else:
                 log.warning(f"Authentication settings missing from {filespec}")
         else:
             log.debug(f"ODKCentral configuration parsed: {self.url}")
         # Base URL for the REST API
         self.version = "v1"
-        log.debug(f"Using {self.version} API")
+        # log.debug(f"Using {self.version} API")
         self.base = self.url + "/" + self.version + "/"
 
         # Authentication data
         self.auth = HTTPBasicAuth(self.user, self.passwd)
 
         # Use a persistant connect, better for multiple requests
         self.session = requests.Session()
 
         # These are just cached data from the queries
         self.projects = dict()
-        self.users = None
+        self.users = list()
+        # The number of threads is based on the CPU cores
+        info = get_cpu_info()
+        self.cores = info['count']
 
     def authenticate(self,
                      url:str = None,
                      user:str = None,
                      passwd:str = None
                      ):
         """Setup authenticate to an ODK Central server"""
@@ -244,16 +277,16 @@
 
 
 class OdkProject(OdkCentral):
     """Class to manipulate a project on an ODK Central server"""
 
     def __init__(self, url=None, user=None, passwd=None):
         super().__init__(url, user, passwd)
-        self.forms = None
-        self.submissions = None
+        self.forms = list()
+        self.submissions = list()
         self.data = None
         self.appusers = None
         self.id = None
 
     def getData(self,
                 keyword: str
                 ):
@@ -264,14 +297,57 @@
                   ):
         """Fetch a list of forms in a project on an ODK Central server."""
         url = f"{self.base}projects/{xform}/forms"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
         self.forms = result.json()
         return self.forms
 
+
+    def getAllSubmissions(self,
+                          project_id: int,
+                          xforms: list = None
+                        ):
+        """Fetch a list of submissions in a project on an ODK Central server."""
+        timer = Timer(text="getAllSubmissions() took {seconds:.0f}s")
+        timer.start()
+        if not xforms:
+            xforms = self.listForms(project_id)
+        chunk = round(len(xforms) / self.cores) if round(len(xforms) / self.cores) > 0 else 1        
+        last_slice = len(xforms) if len(xforms) % chunk == 0 else len(xforms) - 1
+        cycle = range(0, (last_slice + chunk) +1, chunk)
+        future = None
+        result = None
+        previous = 0
+        newdata = list()
+
+        # single threaded for easier debugging
+        # for current in cycle:
+        #     if previous == current:
+        #         continue
+        #     result = downloadThread(project_id, xforms[previous:current])
+        #     previous = current
+        #     newdata += result
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.cores) as executor:
+            futures = list()
+            for current in cycle:
+                if previous == current:
+                    continue
+                result = executor.submit(downloadThread, project_id, xforms[previous:current])
+                previous = current
+                futures.append(result)
+            for future in concurrent.futures.as_completed(futures):
+                log.debug(f"Waiting for thread to complete..")
+                data = future.result(timeout=10)
+                if len(data) > 0:
+                    newdata += data
+        timer.stop()
+        return newdata
+
+
     def listAppUsers(self,
                      projectId: int
                      ):
         """Fetch a list of app users for a project from an ODK Central server."""
         url = f"{self.base}projects/{projectId}/app-users"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
         self.appusers = result.json()
@@ -290,14 +366,24 @@
                    ):
         """Get all the details for a project on an ODK Central server"""
         url = f"{self.base}projects/{projectId}"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
         self.data = result.json()
         return self.data
 
+    def getFullDetails(self,
+                   projectId: int
+                   ):
+        """Get extended details for a project on an ODK Central server"""
+        url = f"{self.base}projects/{projectId}"
+        self.session.headers.update({"X-Extended-Metadata": "true"})
+        result = self.session.get(url, auth=self.auth, verify=self.verify)
+        self.data = result.json()
+        return self.data
+
     def dump(self):
         """Dump internal data structures, for debugging purposes only"""
         super().dump()
         if self.forms:
             print("There are %d forms in this project" % len(self.forms))
             for data in self.forms:
                 print(
@@ -356,23 +442,35 @@
                    ):
         """Get all the details for a form on an ODK Central server"""
         url = f"{self.base}projects/{projectId}/forms/{xform}"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
         self.data = result.json()
         return result
 
+    def getFullDetails(self,
+                       projectId: int,
+                       xform: str):
+        url = f"{self.base}projects/{projectId}/forms/{xform}"
+        self.session.headers.update({"X-Extended-Metadata": "true"})
+        result = self.session.get(url, auth=self.auth, verify=self.verify)
+        self.data = result.json()
+        return result
+
     def listSubmissions(self,
-                        projectId,
+                        projectId: int,
                         xform: str
                         ):
         """Fetch a list of submission instances for a given form."""
-        url = f"{self.base}projects/{projectId}/forms/{xform}/submissions"
+        url = f"{self.base}projects/{projectId}/forms/{xform}.svc/Submissions"
         result = self.session.get(url, auth=self.auth, verify=self.verify)
-        self.submissions = result.json()
-        return self.submissions
+        if result.ok:
+            self.submissions = result.json()
+            return self.submissions['value']
+        else:
+            return list()
 
     def listAssignments(self,
                         projectId: int,
                         xform: str
                         ):
         """List the Role & Actor assignments for users on a project"""
         url = f"{self.base}projects/{projectId}/forms/{xform}/assignments"
@@ -389,38 +487,39 @@
         """Fetch a CSV file of the submissions without media to a survey form."""
         headers = {"Content-Type": "application/json"}
         now = datetime.now()
         timestamp = f"{now.year}_{now.hour}_{now.minute}"
         
         if json:
             url = self.base + f"projects/{projectId}/forms/{xform}.svc/Submissions"
-            filespec = f"/tmp/{xform}_{timestamp}.json"
+            filespec = f"{xform}_{timestamp}.json"
         else:
             url = self.base + f"projects/{projectId}/forms/{xform}/submissions"
-            filespec = f"/tmp/{xform}_{timestamp}.csv"
+            filespec = f"{xform}_{timestamp}.csv"
 
         if submission_id:
             url = url + f"('{submission_id}')"
 
+        # log.debug(f'Getting submissions for {projectId}, Form {xform}')
         result = self.session.get(url, auth=self.auth, headers=headers, verify=self.verify)
         if result.status_code == 200:
             if disk:
                 # id = self.forms[0]['xmlFormId']
                 try:
                     file = open(filespec, "xb")
                     file.write(result.content)
                 except FileExistsError:
                     file = open(filespec, "wb")
                     file.write(result.content)
                 log.info("Wrote output file %s" % filespec)
                 file.close()
             return result.content
         else:
-            log.error(f'Submissions for {projectId}, Form {xform}' + "doesn't exist")
-            return None
+            log.error(f'Submissions for {projectId}, Form {xform}' + " doesn't exist")
+            return list()
 
     def getSubmissionMedia(self,
                            projectId: int,
                            xform: str
                            ):
         """Fetch a ZIP file of the submissions with media to a survey form."""
         url = self.base + f"projects/{projectId}/forms/{xform}/submissions.csv.zip"
@@ -552,15 +651,14 @@
         """Delete a form from an ODK Central server"""
         # FIXME: If your goal is to prevent it from showing up on survey clients like ODK Collect, consider
         # setting its state to closing or closed
         if self.draft:
             url = f"{self.base}projects/{projectId}/forms/{xform}/draft"
         else:
             url = f"{self.base}projects/{projectId}/forms/{xform}"
-        print(url)
         result = self.session.delete(url, auth=self.auth, verify=self.verify)
         return result
 
     def publishForm(self,
                     projectId: int,
                     xform: str
                     ):
@@ -580,15 +678,15 @@
             log.info(f"Published {xform} on Central.")
         return result.status_code
 
     def dump(self):
         """Dump internal data structures, for debugging purposes only"""
         # super().dump()
         entries = len(self.media)
-        print("Form has %d attachements" % entries)
+        print("Form has %d attachments" % entries)
         for form in self.media:
             if "name" in form:
                 print("Name: %s" % form["name"])
 
 
 class OdkAppUser(OdkCentral):
     def __init__(self, url=None, user=None, passwd=None):
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.3.4/osm_fieldwork/basemapper.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/convert.py` & `osm-fieldwork-0.3.4/osm_fieldwork/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,27 +77,27 @@
         else:
             self.multiple = list()
 
     def privateData(self,
                     keyword: str
                     ):
         """See is a keyword is in the private data category"""
-        return keyword in self.private
+        return keyword.lower() in self.private
 
     def convertData(self,
                     keyword: str
                     ):
         """See is a keyword is in the convert data category"""
-        return keyword in self.convert
+        return keyword.lower() in self.convert
 
     def ignoreData(self,
                    keyword: str
                    ):
         """See is a keyword is in the convert data category"""
-        return keyword in self.ignore
+        return keyword.lower() in self.ignore
 
     def getKeyword(self,
                    value: str
                    ):
         """Get the value for a keyword from the yaml file"""
         key = self.yaml.yaml(value)
         if type(key) == bool:
@@ -117,61 +117,52 @@
             return None
 
     def convertEntry(self,
                      tag: str,
                      value: str
                      ):
         """Convert a tag and value from the ODK represention to an OSM one"""
-        #all = list()
+        all = list()
 
         # If it's not in any conversion data, pass it through unchanged.
-        if tag in self.ignore:
+        if tag.lower() in self.ignore:
             # logging.debug(f"FIXME: Ignoring {tag}")
             return None
+        low = tag.lower()
         if (
-            tag not in self.convert
-            and tag not in self.ignore
-            and tag not in self.private
+            low not in self.convert
+            and low not in self.ignore
+            and low not in self.private
         ):
             return {tag: value}
 
-        newtag = None
-        newval = None
+        newtag = tag.lower()
+        newval = value
         # If the tag is in the config file, convert it.
-        if self.convertData(tag):
-            newtag = self.convertTag(tag)
+        if self.convertData(newtag):
+            newtag = self.convertTag(newtag)
             if newtag != tag:
                 logging.debug(f"Converted Tag for entry {tag} to {newtag}")
 
-        if newtag is None:
-            newtag = tag
         # Truncate the elevation, as it's really long
         if newtag == "ele":
             value = value[:7]
         newval = self.convertValue(newtag, value)
-        if newval != value:
-            logging.debug("Converted Value for entry '%s' to '%s'" % (value, newval))
-            for i in newval:
-                key = list(i.keys())[0]
-                newtag = key
-                newval = i[key]
-                #all.append({newtag: newval})
-        #else:
-        #    all.append({newtag: newval})
-
-        # if newtag not in self.tags:
-        #     tmp = { newtag: None }
-        #     key = list()
-        #     all.append(tmp)
-        # else:
-        #     val = self.tags[newtag]
-        #     key = list(val.keys())[0]
-        #     logging.debug("Converted Value for entry %s to %s" % (tag, value))
-        #     # all = self.Value(tag, value)
-        return {newtag: newval}
+        logging.debug("Converted Value for entry '%s' to '%s'" % (value, newval))
+        # there can be multiple new tag/value pairs for some values from ODK
+        if type(newval) == str:
+            all.append({newtag: newval})
+        elif type(newval) == list:
+            for entry in newval:
+                if type(entry) == str:
+                    all.append({newtag: newval})
+                elif type(entry) == dict:
+                    for k, v in entry.items():
+                        all.append({k: v})
+        return all
 
     def convertValue(self,
                      tag: str,
                      value: str
                      ):
         """Convert a single tag value"""
         all = list()
@@ -204,31 +195,32 @@
                 all.append(entry)
         return all
 
     def convertTag(self,
                    tag: str
                    ):
         """Convert a single tag"""
-        if tag in self.convert:
-            newtag = self.convert[tag]
+        low = tag.lower()
+        if low in self.convert:
+            newtag = self.convert[low]
             if type(newtag) is str:
                 logging.debug("\tTag '%s' converted to '%s'" % (tag, newtag))
                 tmp = newtag.split("=")
                 if len(tmp) > 1:
                     newtag = tmp[0]
             elif type(newtag) is list:
                 logging.error("FIXME: list()")
                 # epdb.st()
-                return tag
+                return low
             elif type(newtag) is dict:
                 # logging.error("FIXME: dict()")
-                return tag
-            return newtag
+                return low
+            return newtag.lower()
         else:
-            return tag
+            return low
 
     def dump(self):
         """Dump the contents of the yaml file"""
         print("YAML file: %s" % self.filespec)
         print("Convert section")
         for key, val in self.convert.items():
             if type(val) is list:
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.3.4/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.3.4/osm_fieldwork/data_models/category.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 - natural:
   - nature.xls
 
 # historic is an official OSM tag
 - historic:
   - historical.xls
 
+# highway is an official OSM tag
+- highways:
+  - highways.xls
+
 - waterpoints:
   - waterpoints.xls
 
 - buildings:
   - buildings.xls
 
 - cemeteries:
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.3.4/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.3.4/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.3.4/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.3.4/osm_fieldwork/filter_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,24 @@
             self.parse(filespec)
 
     def parse(self,
               filespec: str
               ):
         """Read in the XLSForm and extract the data we want"""
         entries = pd.read_excel(filespec, sheet_name=[0, 1, 2])
-        
         title = entries[2]['form_title'].to_list()[0]
         extract = ""
         for entry in entries[0]['type']:
             if str(entry) == 'nan':
                 continue
             if entry[:20] == "select_one_from_file":
                 extract = entry[21:]
-        log.info(f"Got data extract filename: \"{extract}\", title: \"{title}\"")
+                log.info(f"Got data extract filename: \"{extract}\", title: \"{title}\"")
+            else:
+                extract = "none"
         total = len(entries[1]['list_name'])
         index = 1
         while index < total:
             key = entries[1]['list_name'][index]
             if key == 'model' or str(key) == "nan":
                 index += 1
                 continue
@@ -99,14 +100,15 @@
             self.keep.extend(self.yaml['keep'])
 
         return title, extract
 
     def cleanData(self,
                   data
                   ):
+        """Filter out any data not in the data_model"""
         tmpfile = data
         if type(data) == str:
             outfile = open(f"new-{data}", "x")
             infile = open(tmpfile, "r")
             indata = geojson.load(infile)
         elif type(data) == bytes:
             indata = eval(data.decode())
@@ -118,14 +120,15 @@
             "version",
             "changeset",
             )
         collection = list()
         for feature in indata['features']:
             properties = dict()
             for key, value in feature['properties'].items():
+                # log.debug(f"{key} = {value}")
                 if key in self.keep:
                     if key == 'tags':
                         for k, v in value.items():
                             if k[:4] == "name":
                                 properties['title'] = value[k]
                                 properties['label'] = value[k]
                             else:
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.3.4/osm_fieldwork/json2osm.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from osm_fieldwork.osmfile import OsmFile
 from osm_fieldwork.xlsforms import xlsforms_path
 from geojson import Point, Feature, FeatureCollection, dump
 from pathlib import Path
 #import pandas as pd
 import math
 import re
+import flatdict
 
 
 # set log level for urlib
 log = logging.getLogger(__name__)
 
 class JsonDump(Convert):
     """A class to parse the JSON files from ODK Central or odk2geojson"""
@@ -86,18 +87,24 @@
                  ):
         """Write a feature to an OSM XML output file"""
         out = ""
         if "id" in feature["tags"]:
             feature["id"] = feature["tags"]["id"]
         if "lat" not in feature["attrs"] or "lon" not in feature["attrs"]:
             return None
+        if 'user' in feature['tags'] and 'user' not in feature["attrs"]:
+            feature["attrs"]['user'] = feature['tags']['user']
+            del feature['tags']['user']
+        if 'uid' in feature['tags'] and 'uid' not in ["attrs"]:
+            feature["attrs"]['uid'] = feature['tags']['uid']
+            del feature['tags']['uid']
         if "refs" not in feature:
-            out += self.osm.createNode(feature)
+            out += self.osm.createNode(feature, True)
         else:
-            out += self.osm.createWay(feature)
+            out += self.osm.createWay(feature, True)
         self.osm.write(out)
 
     def finishOSM(self):
         """Write the OSM XML file footer and close it"""
         self.osm.footer()
 
     def createGeoJson(self, file="tmp.geojson"):
@@ -124,76 +131,34 @@
                 props = {**item["tags"], **item["private"]}
             else:
                 props = item["tags"]
             features.append(Feature(geometry=poi, properties=props))
         collection = FeatureCollection(features)
         dump(collection, self.json)
 
-    def getAllTags(self,
-                   data
-                   ):
-        all_tags = dict()
-        tags = dict()
-        if type(data) == dict:
-            for k, v in data.items():
-                if type(v) == dict:
-                    # log.debug(f"Processing tag {k} = {v}")
-                    for k1, v1 in v.items():
-                        # log.debug(f"Processing sub tag {k} = {v}")
-                        # tags.update(self.getAllTags(v))
-                        if type(v1) == dict:
-                            for i, j in v1.items():
-                                if type(j) == dict:
-                                    # FIXME: this should handle more than one
-                                    # but so far I've only it to be accuracy, no other
-                                    # tags
-                                    k2 = list(j.keys())[0]
-                                    tags[k2] = list(j.values())[0]
-                                else:
-                                    tags[i] = j
-                        else:
-                            tags[k1] = v1
-                        # log.debug(f"TAGS: {tags}")
-                else:
-                    if v:
-                        # if k in self.saved:
-                        #     if str(v) == 'nan' or len(v) == 0:
-                        #         log.debug(f"FIXME: {k} {v}")
-                        #         val = self.saved[k]
-                        #         if val and len(v) == 0:
-                        #             log.warning(f"Using last saved value for \"{k}\"! Now \"{val}\"" )
-                        #             value = val
-                        #         else:
-                        #             self.saved[k] = value
-                        #             log.debug(f"Updating last saved value for \"{k}\" with \"{value}\"")
-                        if type(v) != str:
-                            tags[k] = str(v)
-                        else:
-                            tags[k] = escape(v)
-                all_tags.update(tags)
-        return all_tags
-
     def parse(self,
-              filespec: str,
+              filespec: str = None,
               data: str = None
               ):
         """Parse the JSON file from ODK Central and convert it to a data structure"""
         all_tags = list()
         if not data:
             file = open(filespec, "r")
             infile = Path(filespec)
             if infile.suffix == ".geojson":
                 reader = geojson.load(file)
             elif infile.suffix == ".json":
                 reader = json.load(file)
             else:
                 log.error("Need to specify a JSON or GeoJson file!")
                 return all_tags
-        else:
+        elif type(data) == str:
             reader = geojson.loads(data)
+        elif type(data) == list:
+            reader = data
         
         total = list()
         # JSON files from Central use value as the keyword, whereas
         # GeoJSON uses features for the same thing.
         if 'value' in reader:
             data = reader['value']
         elif 'features' in reader:
@@ -201,57 +166,51 @@
         else:
             data = reader
         for row in data:
             # log.info(f"ROW: {row}")
             tags = dict()
             if 'geometry' in row:
                 tags['geometry'] = row['geometry']
+            else:
+                pat = re.compile("[-0-9.]*, [0-9.-]*, [0-9.]*")
+                gps = re.findall(pat, str(row))
+                # If geopoint warmup is used, there will be two matches, we only
+                # want the second one, which is the location.
+                for coords in gps:
+                    tags['geometry'] = coords
             if 'properties' in row:
                 indata = row['properties'] # A GeoJson formatted file
             else:
                 indata = row    # A JOSM file from ODK Central
-            for keyword, value in indata.items():
-                # There's many extraneous fields in the input file which we don't need.
-                base = keyword.lower()
-                if (
-                    base is None
-                    or value is None
-                    or len(value) == 0
-                ):
+
+            # flatten all the groups into a single data structure
+            flattened = flatdict.FlatDict(row)
+            for k, v in flattened.items():
+                last = k.rfind(':') + 1
+                key = k[last:]
+                # log.debug(f"Processing tag {key} = {v}")
+                # names and comments may have spaces, otherwise
+                # it's from a select_multiple
+                pat = re.compile("name[:a-z]*")
+                names = re.findall(pat, key)
+                if len(names) > 0:
+                    for name in names:
+                        tags[name] = v
                     continue
-                if keyword is None or len(keyword) == 0:
+                if key == 'comment':
+                    tags[key] = v
+                # a JSON file from ODK Central always uses coordinates as
+                # the keyword
+                if key == 'coordinates':
+                    if type(v) == list:
+                        lat = v[1]
+                        lon = v[0]
+                        tags['geometry'] = f"{lat} {lon}"
                     continue
-                if type(value) == str:
-                    if keyword not in self.ignore:
-                        continue
-                    items = self.convertEntry(keyword, value)
-                    if items is not None and tags is not None:
-                        tags.update(items)
-                    else:
-                        continue
-                else:
-                    alltags = self.getAllTags(value)
-                    for k, v in alltags.items():
-                        if v:
-                            items = dict()
-                            if type(v) == dict:
-                                v1 = alltags[k]
-                                if len(v1) > 1:
-                                    log.warning("Got more than 1 result! {v1}")
-                                    v2 = v1[v1.keys()]
-                                    items = self.convertEntry(k, v2)
-                            else:
-                                items = self.convertEntry(k, v)
-                                #    for entry in items:
-                                #        for k, v in entry.items():
-                                #            tags[k] = v
-                                #    else:
-                                #tags[k1] = v1
-                        if items is not None:
-                            tags.update(items)
+                tags[key] = v
             total.append(tags)
         return total
 
     def createEntry(self,
                     entry: dict
                     ):
         """Create the feature data structure"""
@@ -302,40 +261,44 @@
                 elif type(value) == list:
                     lat = float(value[1])
                     lon = float(value[0])
                 attrs["lat"] = lat
                 attrs["lon"] = lon
                 # log.debug(f"ATTRS: {attrs}")
 
-            if key is not None and len(key) > 0 and key in attributes:
-                attrs[key] = value
-                log.debug("Adding attribute %s with value %s" % (key, value))
-            else:
-                if key in self.multiple:
-                    for item in value:
-                        if key in item:
-                            for entry in item[key].split():
-                                vals = self.getValues(key)
-                                if entry in vals:
-                                    if vals[entry].find("="):
-                                        tmp = vals[entry].split("=")
-                                        tags[tmp[0]] = tmp[1]
-                                else:
-                                    tags[entry] = "yes"
-                    continue
+            # Some tags are actually attributes
+            # print(f"FIXME: {key} {key in attributes}")
+            # if key in self.multiple:
+            #     for item in value:
+            #         if key in item:
+            #             for entry in item[key].split():
+            #                 vals = self.getValues(key)
+            #                 if entry in vals:
+            #                     if vals[entry].find("="):
+            #                         tmp = vals[entry].split("=")
+            #                         tags[tmp[0]] = tmp[1]
+            #                 else:
+            #                     tags[entry] = "yes"
+            #     continue
+
+            if value is not None and value != "no" and value != "unknown":
+                if key == "track" or key == "geoline":
+                    refs.append(tag)
+                    log.debug("Adding reference %s" % tag)
+                elif len(str(value)) > 0:
+                    if self.privateData(key):
+                        priv[key] = value
+                    else:
+                        item = self.convertEntry(key, value)
+                        if item is not None and type(item) == dict:
+                            tags.update(item)
+                        elif type(item) == list:
+                            for entry in item:
+                                tags.update(entry)
 
-                if value is not None and value != "no" and value != "unknown":
-                    if key == "track" or key == "geoline":
-                        refs.append(tag)
-                        log.debug("Adding reference %s" % tag)
-                    elif len(str(value)) > 0:
-                        if self.privateData(key):
-                            priv[key] = value
-                        else:
-                            tags[key] = value
             if len(tags) > 0:
                 if 'geometry' in tags:
                     del tags['geometry']
                 feature["attrs"] = attrs
                 feature["tags"] = tags
             if len(refs) > 0:
                 feature["refs"] = refs
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.3.4/osm_fieldwork/make_data_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             elif table == "ways_poly":
                 tables.append("polygon")
             elif table == "ways_line":
                 tables.append("line")
             elif table == "relations":
                 tables.append("line")
         features["geometryType"] = tables
-        if not poly:
+        if not poly and category != 'highways':
             features["centroid"] = "true"
         return json.dumps(features)
 
     def createSQL(self,
                   category: str,
                   polygon: bool = False
                   ):
@@ -200,15 +200,15 @@
 
         sql = list()
         # The database tables to query
         tables = data['from']
         for table in tables:
             query = "SELECT "
             select = data['select']
-            if polygon:
+            if polygon or category == "highways":
                 centroid = "geom"
             else:
                 centroid = "ST_Centroid(geom)"
             # if tags exists, then only return those fields
             if 'tags' in select:
                 for tag in select['tags']:
                     query += f" {select[tag]} AS {tag}, "
@@ -238,20 +238,23 @@
                    ):
         # sql = f"DROP VIEW IF EXISTS ways_view;CREATE TEMP VIEW ways_view AS SELECT * FROM ways_poly WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         sql = f"DROP VIEW IF EXISTS ways_view;CREATE VIEW ways_view AS SELECT * FROM ways_poly WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         self.dbcursor.execute(sql)
         # sql = f"DROP VIEW IF EXISTS nodes_view;CREATE TEMP VIEW nodes_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         sql = f"DROP VIEW IF EXISTS nodes_view;CREATE VIEW nodes_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         self.dbcursor.execute(sql)
-
+        sql = f"DROP VIEW IF EXISTS lines_view;CREATE VIEW lines_view AS SELECT * FROM ways_line WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
+        self.dbcursor.execute(sql)
         sql = f"DROP VIEW IF EXISTS relations_view;CREATE TEMP VIEW relations_view AS SELECT * FROM nodes WHERE ST_CONTAINS(ST_GeomFromEWKT('SRID=4326;{ewkt.wkt}'), geom)"
         # self.dbcursor.execute(sql)
 
         if query.find(" ways_poly ") > 0:
             query = query.replace("ways_poly", "ways_view")
+        if query.find(" ways_line ") > 0:
+            query = query.replace("ways_line", "lines_view")
         elif query.find(" nodes ") > 0:
             query = query.replace("nodes", "nodes_view")
         features = list()
         log.debug(query)
         self.dbcursor.execute(query)
         result = self.dbcursor.fetchall()
         log.info("Query returned %d records" % len(result))
@@ -549,36 +552,36 @@
             if match:
                 tmp = match.group().split("/")
         outfile = tmp[3]
     else:
         outfile = args.geojson.lower()
 
     xlsfile = choices[args.category]
-    if args.postgres:
+    if args.postgres is not None:
         log.info("Using a Postgres database for the data source")
         pg = PostgresClient(args.dbhost, args.dbname)
-        if args.geojson:
+        if args.geojson is not None:
             extract = args.geojson
         else:
             infile = FilterData(xlsfile)
             extract = infile.metadata[1]
         pg.getFeatures(args.boundary, extract, args.polygon, args.category, xlsfile)
         log.info(f"Created {outfile} for {args.category}")
         # pg.cleanup(outfile)
-    elif args.overpass:
+    elif args.overpass is not None:
         log.info("Using Overpass Turbo for the data source")
         op = OverpassClient(outfile)
         clip = open(args.boundary, "r")
         geom = geojson.load(clip)
         #op.getFeatures(args.boundary, args.geojson, args.category)
         op.getFeatures(geom, args.geojson, xlsfile, args.category)
-    elif args.infile:
+    elif args.infile is not None:
         f = FileClient(args.infile)
         f.getFeatures(args.boundary, args.geojson, args.category)
         log.info("Using file %s for the data source" % args.infile)
     else:
         log.error("You need to supply either --overpass or --postgres")
 
-        # logging.info("Wrote output data file to: %s" % outfile)
+    # logging.info("Wrote output data file to: %s" % outfile)
 
 if __name__ == "__main__":
     main()
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/models.yaml` & `osm-fieldwork-0.3.4/osm_fieldwork/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.3.4/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.3.4/osm_fieldwork/odk2geojson.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,20 +28,21 @@
 from datetime import datetime
 from osm_fieldwork.ODKInstance import ODKInstance
 import geojson
 import json
 from geojson import Feature, FeatureCollection, dump
 from shapely.geometry import Point
 from datetime import datetime
+import flatdict
 
 
 # Instantiate logger
 log = logging.getLogger(__name__)
 
-def moon():
+def main():
     parser = argparse.ArgumentParser(
         description="Convert ODK XML instance file to GeoJson"
     )
     parser.add_argument("-v", "--verbose", nargs="?", const="0", help="verbose output")
     parser.add_argument("-i", "--instance", required=True, help="The instance file(s) from ODK Collect")
     parser.add_argument("-o","--outfile", default='tmp.geojson', help='The output file for JOSM')
     args = parser.parse_args()
@@ -85,34 +86,39 @@
         tags = dict()
         #odkxml = ODKInstance()
         #data = odkxml.parse(filespec=xml)
         file = open(xml, "r")
         # Instances are small, read the whole file
         data = file.read(os.path.getsize(xml))
         doc = xmltodict.parse(data)
-        # This is pretty ugly. We know that somewhere in the lower level
-        # dicts there are GPS coordinates, which luckily are easy to
-        # find and should always be a unique field in a feature. While
-        # is ugly, it's also way more efficient than looping through
-        # levels to find that one value. Plus htis doesn't care what the
-        # key is.
-        pat = re.compile("[0-9.]* [0-9.-]* [0-9.]* [0-9.]*")
-        data = json.dumps(doc)
-        gps = re.findall(pat, str(data))
-        for coords in gps:
-            tmp = coords.split(' ')
-            lat = float(tmp[0])
-            lon = float(tmp[1])                
-            poi = Point(lon, lat)
-        features.append(Feature(geometry=poi, properties=doc['data']))
+
+        flattened = flatdict.FlatDict(doc['data'])
+        poi = Point()
+        feature = dict()
+        for key, value in flattened.items():
+            if key[0] == '@' or value is None:
+                continue
+            last = key.rfind(':') + 1
+            key = key[last:]
+            pat = re.compile("[0-9.]* [0-9.-]* [0-9.]* [0-9.]*")
+            gps = re.findall(pat, value)
+            if len(gps) > 0:
+                tmp = gps[0].split(' ')
+                lat = float(tmp[0])
+                lon = float(tmp[1])
+                poi = Point(lon, lat)
+            else:
+                feature[key] = value
+        features.append(Feature(geometry=poi, properties=feature))
     collection = FeatureCollection(features)
 
     now = datetime.now()
     timestamp = f"_{now.year}_{now.month}-{now.day}-{now.hour}-{now.minute}"
     outfile = args.instance.replace("*", "") + timestamp + ".geojson"
-    json = open(outfile, 'w')
-    dump(collection, json)
+    outfile = outfile.replace(' ', '')
+    fout = open(outfile, 'w')
+    dump(collection, fout)
 
     print(f"Wrote output file {outfile}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/odk2osm.py` & `osm-fieldwork-0.3.4/osm_fieldwork/odk2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.3.4/osm_fieldwork/odk_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 
 import logging
 import argparse
 import sys
 import os
 import json
 from osm_fieldwork.OdkCentral import OdkCentral, OdkProject, OdkForm, OdkAppUser
+from osm_fieldwork.json2osm import JsonDump
 from pathlib import Path
+from sys import argv
+from geojson import Feature, FeatureCollection, dump
+from datetime import datetime
+from codetiming import Timer
+
 
 # Set log level
 log_level = os.getenv("LOG_LEVEL", default="INFO")
 logging.getLogger("urllib3").setLevel(log_level)
 
 log = logging.getLogger(__name__)
 
@@ -67,15 +73,15 @@
     parser.add_argument(
         "-s", "--server", choices=["projects", "users", "delete"], help="project operations"
     )
     # This is for project specific requests
     parser.add_argument(
         "-p",
         "--project",
-        choices=["forms", "app-users", "assignments", "delete"],
+        choices=["forms", "app-users", "assignments", "delete", "submissions"],
         help="project operations",
     )
     parser.add_argument("-i", "--id", type=int, help="Project ID nunmber")
     parser.add_argument("-f", "--form", help="XForm name")
     parser.add_argument("-u", "--uuid", help="Submission UUID, needed to download the data")
     # This is for form specific requests
     parser.add_argument("-x", "--xform",
@@ -125,14 +131,18 @@
     # parser.add_argument("-d", "--download", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Download files from ODK Central")
     # parser.add_argument("-u", "--upload", choices=['xml', 'xlsx', 'attach', 'submit', 'zip'], help="Upload files to ODK Central")
 
     # Any files we want to use are specified on the command line with an argument.
     # Multiple files are stored in a list.
     args, unknown = parser.parse_known_args()
 
+    if len(argv) <= 1:
+        parser.print_help()
+        quit()
+
     # Get any files for upload or download
     files = list()
     if unknown is not None:
         files = unknown
 
     # if verbose, dump to the terminal.
     if args.verbose is not None:
@@ -143,21 +153,29 @@
         ch.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         ch.setFormatter(formatter)
         root.addHandler(ch)
 
+    timer = Timer(text="odk_client() took {seconds:.0f}s")
+    timer.start()
     # Commands to the ODK Central server, which gets data that applies
     # to all projects on the server.
     if args.server:
         central = OdkCentral()
         # central.authenticate()
         if args.server == "projects":
             projects = central.listProjects()
+            if not projects:
+                projects = list()
+            elif 'message' in projects:
+                log.error(f"{projects['message']}, {projects['code']} ")
+                quit()
+
             print("There are %d projects on this ODK Central server" % len(projects))
             ordered = sorted(projects, key=lambda item: item.get("id"))
             for project in ordered:
                 print("\t%s: %s" % (project["id"], project["name"]))
         elif args.server == "users":
             users = central.listUsers()
             logging.info("There are %d users on this ODK Central server" % len(users))
@@ -182,22 +200,49 @@
             forms = project.listForms(args.id)
             if type(forms) == dict:
                 log.error(f"{forms['message']}, {forms['code']} ")
                 quit()
             if type(forms) != list:
                 log.error(forms['message'])
                 quit()
-                ordered = sorted(forms, key=lambda item: item.get("xmlFormId"))
-                for form in ordered:
-                    print("\t%r: %r" % (form["xmlFormId"], form["name"]))
-                    # if args.project == "submissions":
-                    #     submit = project.listSubmissions(args.id, args.form)
-                    #     # ordered = sorted(submit, key=lambda item: item.get('xmlFormId'))
-                    #     for data in submit:
-                    #         print("\t%s by user %s" % (data['instanceId'], data['submitterId']))
+            ordered = sorted(forms, key=lambda item: item.get("xmlFormId"))
+            for form in ordered:
+                print("\t%r: %r" % (form["xmlFormId"], form["name"]))
+
+        elif args.project == "submissions":
+            submissions = project.getAllSubmissions(args.id)
+            jsonin = JsonDump()
+            now = datetime.now().strftime("%Y-%m-%dT%TZ")
+            outfile = f"{args.project}_{now}"
+            jsonin.createOSM(f"{outfile}.osm")
+            # jsonin.createGeoJson(f"{outfile}.geojson")
+            data = jsonin.parse(data=submissions)
+            log.debug(f"There are a total of {len(submissions)} submissions")
+            for entry in data:
+                feature = jsonin.createEntry(entry)
+                # Sometimes bad entries, usually from debugging XForm design, sneak in
+                if len(feature) == 0:
+                    continue
+                if "lat" not in feature["attrs"]:
+                    if 'geometry' in feature['tags']:
+                        if type(feature['tags']['geometry']) == str:
+                            coords = list(feature['tags']['geometry'])
+                            # del feature['tags']['geometry']
+                    elif 'coordinates' in feature['tags']:
+                        coords = feature['tags']['coordinates']
+                        feature['attrs'] = {'lat': coords[1], 'lon': coords[0]}
+                    else:
+                        log.warning("Bad record! %r" % feature)
+                        continue
+                jsonin.writeOSM(feature)
+                log.info(f"Wrote {outfile}.osm")
+                # This GeoJson file has all the data values
+                # jsonin.writeGeoJson(feature)
+                #log.info(f"Wrote {outfile}.geojson")
+
         elif args.project == "app-users":
             users = project.listAppUsers(args.id)
             logging.info("There are %d app users on this ODK Central server" % len(users))
             ordered = sorted(users, key=lambda item: item.get("id"))
             for user in ordered:
                 print("\t%r: %s (%s)" % (user["id"], user["displayName"], user["token"]))
         elif args.project == "delete":
@@ -245,54 +290,70 @@
                     file = open(file, "xb")
                 except FileExistsError:
                     file = open(file, "wb")
                     file.write(data)
                     file.close()
         elif args.xform == "assignments":
             assign = form.listAssignments(args.id, args.form)
+            if type(assign) == dict:
+                log.error(f"{assign['message']}, {assign['code']} ")
+                quit()
             logging.info(
                 "There are %d assignments  on this ODK Central server" % len(assign)
             )
             # ordered = sorted(assign, key=lambda item: item.get('id'))
             for role in assign:
                 print("\t%r" % role)
+
         elif args.xform == "submissions":
             submissions = form.listSubmissions(args.id, args.form)
             if not submissions:
                 submissions = list()
-            elif type(submissions) == dict:
+            elif 'message' in submissions:
                 log.error(f"{submissions['message']}, {submissions['code']} ")
-            else:
-                logging.info(
-                    "There are %d submissions for XForm %s" % (len(submissions), args.form)
+                quit()
+
+            logging.info(
+                "There are %d submissions for XForm %s" % (len(submissions), args.form)
                 )
             for file in submissions:
                 # form.submissions.append(file)
-                print("%s: %s" % (file["instanceId"], file["createdAt"]))
+                print("%s: %s" % (file['meta']['instanceID'], file["end"]))
 
         elif args.xform == "csv":
             submissions = form.getSubmissions(args.id, args.form, True, False)
+            if type(submissions) == dict:
+                log.error(f"{submissions['message']}, {submissions['code']} ")
             logging.info(
                 "There are %d submissions for XForm %s" % (len(submissions), args.form)
             )
             for file in submissions:
                 form.submissions.append(file)
-                print("%s: %s" % (file["instanceId"], file["createdAt"]))
+                print("%s: %s" % (file['meta']['instanceID'], file["end"]))
 
         elif args.xform == "json":
             submissions = form.getSubmissions(args.id, args.form, False, True, True)
+            if type(submissions) == dict:
+                log.error(f"{submissions['message']}, {submissions['code']} ")
+                quit()
+            else:
+                if submissions is None:
+                    submissions = list()
             logging.info(
                 "There are %d submissions for XForm %s" % (len(submissions), args.form)
             )
             for file in submissions:
                 form.submissions.append(file)
                 #print("%s: %s" % (file["instanceId"], file["createdAt"]))
 
         elif args.xform == "attachments":
             attachments = form.listMedia(args.id, args.form)
+            if type(attachments) == dict:
+                log.error(f"{attachments['message']}, {attachments['code']} ")
+                quit()
             logging.info(
                 "There are %d attachments for XForm %s" % (len(attachments), args.form)
             )
             for file in attachments:
                 print("\t%s exists ? %s" % (file["name"], file["exists"]))
 
         elif args.xform == "create":
@@ -364,10 +425,11 @@
                     # name = "%s-%s" % (project['name'], user['displayName'])
                     name = "%s-%s" % (args.form, user["displayName"])
                     result = appuser.getQRCode(args.id, user["token"], name)
             elif args.bulk == "update":
                 users = central.listAppUsers(args.id)
                 for user in users:
                     result = appuser.updateRole(args.id, args.form, role, user["id"])
+    timer.stop()
 
 if __name__ == "__main__":
     main()
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.3.4/osm_fieldwork/odk_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 
 import argparse
 import logging
 import sys
 import os
 from sys import argv
-from osgeo import ogr
 from osm_fieldwork.osmfile import OsmFile
 from geojson import Point, Feature, FeatureCollection, dump, Polygon
 import geojson
 import psycopg2
 from shapely.geometry import shape, Polygon, mapping
 import shapely
 from shapely import wkt
@@ -339,16 +338,18 @@
         # Use fuzzy string matching to handle minor issues in the name column,
         # which is often used to match an amenity.
         if len(self.data) == 0:
             self.postgres[0].dbcursor.execute("CREATE EXTENSION IF NOT EXISTS fuzzystrmatch")
         log.debug(f"OdkMerge::conflateData() called! {len(odkdata)} features")
 
         # A chunk is a group of threads
-        chunk =  round(len(odkdata)/cores)
-        cycle = range(0, len(odkdata), chunk)
+        chunk = round(len(odkdata) / cores)
+
+        # cycle = range(0, len(odkdata), chunk)
+
         # Chop the data into a subset for each thread
         newdata = list()
         future = None
         result = None
         index = 0
         with concurrent.futures.ThreadPoolExecutor(max_workers=cores) as executor:
             i = 0
@@ -457,24 +458,22 @@
         quit()
     else:
         osmdata = unknown[0]
         source = unknown[1]
 
     # if verbose, dump to the terminal.
     if args.verbose:
-        root = logging.getLogger()
         log.setLevel(logging.DEBUG)
-
         ch = logging.StreamHandler(sys.stdout)
         ch.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             "%(threadName)10s - %(name)s - %(levelname)s - %(message)s"
         )
         ch.setFormatter(formatter)
-        root.addHandler(ch)
+        log.addHandler(ch)
 
     if args.outfile:
         outfile = args.outfile
     else:
         outfile = os.path.basename(osmdata.replace('.osm', '-foo.osm'))
 
     # This is the existing OSM data, a database or a file
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.3.4/osm_fieldwork/osm2favorities.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.3.4/osm_fieldwork/osmfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,17 +120,17 @@
         if "version" not in way["attrs"]:
             attrs["version"] = 1
         else:
             attrs["version"] = way["attrs"]["version"] + 1
         attrs["timestamp"] = datetime.now().strftime("%Y-%m-%dT%TZ")
         # If the resulting file is publicly accessible without authentication, The GDPR applies
         # and the identifying fields should not be included
-        if "uid" in way and attrs["uid"] is not None:
+        if "uid" in way["attrs"]:
             attrs["uid"] = way["attrs"]["uid"]
-        if "user" in way and attrs["user"] is not None:
+        if "user" in way["attrs"]:
             attrs["user"] = way["attrs"]["user"]
 
         # Make all the nodes first. The data in the track has 4 fields. The first two
         # are the lat/lon, then the altitude, and finally the GPS accuracy.
         # newrefs = list()
         node = dict()
         node["attrs"] = dict()
@@ -227,18 +227,18 @@
         else:
             attrs["version"] = int(node['attrs']["version"]) + 1
         attrs["lat"] = node["attrs"]["lat"]
         attrs["lon"] = node["attrs"]["lon"]
         attrs["timestamp"] = datetime.now().strftime("%Y-%m-%dT%TZ")
         # If the resulting file is publicly accessible without authentication, THE GDPR applies
         # and the identifying fields should not be included
-        if "uid" in node and attrs["uid"] is not None:
-            attrs["uid"] = node["uid"]
-        if "user" in node and attrs["ser"] is not None:
-            attrs["user"] = node["user"]
+        if "uid" in node['attrs']:
+            attrs["uid"] = node['attrs']["uid"]
+        if "user" in node['attrs']:
+            attrs["user"] = node['attrs']["user"]
 
         # Processs atrributes
         line = ""
         osm = ""
         for ref, value in attrs.items():
             line += "%s=%r " % (ref, str(value))
         osm += "  <node " + line
@@ -288,23 +288,32 @@
         with open(osmfile, "r") as file:
             xml = file.read(size)  # Instances are small, read the whole file
             doc = xmltodict.parse(xml)
             if "osm" not in doc:
                 logging.warning("No data in this instance")
                 return False
             field = doc["osm"]
+
+            if "node" not in field:
+                logging.warning("No nodes in this instance")
+                return False
+
         if type(field["node"]) == dict:
             attrs = dict()
             tags = dict()
             for k, v in field["node"].items():
                 if k[0] == '@':
                     attrs[k[1:]] = v
                 else:
-                    for pair in field["node"]['tag']:
-                        tags[pair['@k']] = pair['@v']
+                    if type(field["node"]['tag']) == dict:
+                        tags[field["node"]['tag']["@k"]] = field["node"]['tag']["@v"].strip()
+                    else:
+                        for pair in field['node']['tag']:
+                            tags[pair['@k']] = pair['@v']
+
             node = {"attrs": attrs, "tags": tags}
             self.data[node["attrs"]["id"]] = node
         else:
             for node in field["node"]:
                 attrs = {
                     "id": int(node["@id"]),
                     "lat": node["@lat"][:10],
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.3.4/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.3.4/osm_fieldwork/xforms.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,22 @@
 # raw data.
 
 # ODK allows a colon in a selection name, but does not for the
 # variable name that later gets used as a tag. When using existing OSM
 # data we need to handle converting the tag name back to the colon
 # version for OSM.
 convert:
-  # From the Saint Lucia XForm
-  - _record_your_current_location_altitude: ele
-  - Record_your_current_location-Longitude: lon
-  - Record_your_current_location-Latitide: lat
-  # Other forms
   - camptype: tourism
   - openfire: leisure=firepit
   - latitude: lat
   - longitude: lon
   - altitude: ele
   - submitterid: uid
-  - submitterId: uid
   - submittername: user
-  - submitterName: user
   - submissiondate: timestamp
-  - submissionDate: timestamp
   - comment: note
   - view: viewpoint
   - cell: cellular
   - Monday: Mo
   - Tuesday: Tu
   - Wednesday: We
   - Thursday: Th
@@ -53,15 +45,14 @@
   - power_type: power_source
   - provider: operator:type
   - operator_type: operator:type
   - cemetery_services:
       - cemetery: amenity=grave_yard
       - cremation: amenity=crematorium
   - xid: id
-  - camptype: tourism
   - food: amenity
   - brewery: craft=brewery
   - housing: building
   - xlocation: geometry
   - coordinates: geometry
   - healthcare_type: healthcare
   - building_material: building:material
@@ -104,25 +95,25 @@
   - district
   - elev
   - area
   - geological_site
   - lateral_material
   - lateral_system
   - access_roof
+  - updatedat
 
 # All of these tags are in the CSV file, and can be ignored
 ignore:
   - __id
   - model
   - type
   - features
   - accuracy
   - meta
   - __system
-  - attachmentsExpected
   - status
   - reviewState
   - formVersion
   - edits
   - attachmentsexpected
   - attachmentspresent
   - reviewstate
@@ -131,20 +122,18 @@
   - deviceid
   - deviceId
   - key
   - start
   - end
   - today
   - status
-  - instanceid
   - audio
   - image
   - phonenumber
   - detail
-  - what_are_you_mapping
   - highway_type
   - waterpoint_img
   - enum_name
   - username
   - model
   - email
   - category
@@ -152,14 +141,14 @@
   - formversion
   - building_menu
   - food_menu
   - medical_menu
   - retail_menu
   - government_menu
   - note
-  - instanceID
+  - instanceid
 
 multiple:
   - healthcare
   - amenity_type
   - specialty
```

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/test.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/test.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/thamel.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/thamel.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.3.4/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.3.4/osm_fieldwork/yamlfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,37 +39,48 @@
         self.file = open(data, "rb").read()
         self.yaml = yaml.load(self.file, Loader=yaml.Loader)
         #else:
         #    self.yaml = yaml.load(str(data), Loader=yaml.Loader)
 
     def privateData(self, keyword: str):
         """See if a keyword is in the private data category"""
-        return keyword in self.yaml["private"]
+        for value in self.yaml["private"]:
+            if keyword.lower() in value:
+                return True
+        return False
 
     def ignoreData(self, keyword: str):
         """See if a keyword is in the ignore data category"""
-        return keyword in self.yaml["ignore"]
-
-    def tagsData(self, keyword: str):
-        """See if a keyword is in the tags completness section"""
-        return keyword in self.yaml["tags"]
+        for value in self.yaml["ignore"]:
+            if keyword.lower() in value:
+                return True
+        return False
+
+    def convertData(self, keyword: str):
+        """See if a keyword is in the convert data category"""
+        for value in self.yaml["convert"]:
+            if keyword.lower() in value:
+                return True
+        return False
 
     def hasList(self, keyword: str):
         for tags in self.yaml["tags"]:
             for tag in tags:
                 if tag == keyword:
                     return tag
             logging.debug(type(tags))
 
     def dump(self):
         """Dump the contents of the yaml file"""
         if self.filespec:
             print("YAML file: %s" % self.filespec)
-        for item in self.yaml:
-            print(f"{item}")
+        for key, values in self.yaml.items():
+            print(f"Key is:{key}")
+            for k in values:
+                print(f"\t{k}")
 
     def write(self, table: list, where: list):
         tab = "    "
         yaml = ["select:", f"{tab}\"osm_id\": id", f"{tab}tags:"]
         for item in where:
             yaml.append(f"{tab}{tab}- {item}")
         yaml.append("from:")
```

### Comparing `osm-fieldwork-0.3.3/pyproject.toml` & `osm-fieldwork-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "requests>=2.28.2",
     "segno>=1.5.2",
     "xmltodict>=0.13.0",
     "shapely>=1.8.5",
     "overpy>=0.6",
     "thefuzz>=0.19.0",
     "haversine>=2.8.0",
+    "flatdict>=4.0.1",
+    "ogr>=0.44.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = "GPL-3.0-only"
 keywords = [
     "fmtm",
     "odk",
@@ -34,15 +36,15 @@
 ]
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
 ]
-version = "0.3.3"
+version = "0.3.4"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://github.com/hotosm/osm-fieldwork/wiki"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.optional-dependencies]
@@ -72,23 +74,23 @@
 
 [tool.pdm.dev-dependencies]
 test = [
     "pytest>=7.2.1",
 ]
 
 [tool.pytest.ini_options]
-addopts = "-ra -q"
+addopts = "-ra -q -p no:warnings"
 testpaths = [
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.3"
+version = "0.3.4"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 
 [build-system]
```

### Comparing `osm-fieldwork-0.3.3/tests/Test.yaml` & `osm-fieldwork-0.3.4/tests/Test.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/test.csv` & `osm-fieldwork-0.3.4/tests/test.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/test_conflation.py` & `osm-fieldwork-0.3.4/tests/test_conflation.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """This tests conflating against the GeoJson data extract file"""
     passes = 0
     osm = OsmFile()
     osmdata = osm.loadFile(args.odk)
     odk = OdkMerge(args.osm)
     # Although the code is multi-threaded, we can call the function that
     # does all the work directly without threading. Easier to debug this qay.
-    data = conflateThread(osmdata, odk)
+    data = conflateThread(osmdata, odk, 0)
     # There are 8 features in the test data
     if len(data) == 8:
         passes += 1
     # The first feature is a match, so has the OSM ID, the second
     # feature doesn't match, so negative ID
     if data[0]['attrs']['id'] > 0 and data[1]['attrs']['id'] < 0:
         passes += 1
@@ -61,15 +61,15 @@
 
 def test_db():
     """This test against a local database. If there is no postgres, then
     none of the tests get run."""
     passes = 0
     # this database always exists on this developer's machine
     odk = OdkMerge("PG:colorado", args.boundary)
-    if odk.dbcursor is not None:
+    if odk.postgres is not None:
         passes += 1
     else:
         return
     # We also want to trap a bad database name
     # odk = OdkMerge("PG:foobar")
     # if odk.dbcursor is None:
     #     passes += 1
@@ -85,15 +85,15 @@
     keys = list(osmdata.keys())
     if osmdata[keys[6]]['attrs']['id'] > 0 and osmdata[keys[0]]['attrs']['id'] < 0:
         passes += 1
 
     odk = OdkMerge(args.database, args.boundary)
     # Although the code is multi-threaded, we can call the function that
     # does all the work directly without threading. Easier to debug this way.
-    data = conflateThread(osmdata, odk)
+    data = conflateThread(osmdata, odk, 0)
     if len(data[6]['attrs']) > 0 and data[6]['attrs']['id'] > 0 and data[0]['attrs']['id'] < 0:
         passes += 1
     assert(passes == 4)
 
 if __name__ == "__main__":
     print("--- test_file() ---")
     test_file()
```

### Comparing `osm-fieldwork-0.3.3/tests/test_convert.py` & `osm-fieldwork-0.3.4/tests/test_yaml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 #!/usr/bin/python3
 
-# Copyright (c) 2021, 2022, 2023 Humanitarian OpenStreetMap Team
+# Copyright (c) 2022, 2023 Humanitarian OpenStreetMap Team
 #
-# This file is part of Osm-Fieldwork.
+# This file is part of osm_fieldwork.
 #
-#     Osm-Fieldwork is free software: you can redistribute it and/or modify
+#     Underpass is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     Underpass is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
-#     along with Osm-Fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
+#     along with osm_fieldwork.  If not, see <https:#www.gnu.org/licenses/>.
 #
 
-import os
-import sys
 import argparse
+import sys
+import os
 from osm_fieldwork.xlsforms import xlsforms_path
-from osm_fieldwork.convert import Convert
+from osm_fieldwork.yamlfile import YamlFile
 
-parser = argparse.ArgumentParser(
-    description="Read and convert a CSV file from ODK Central"
+parser = argparse.ArgumentParser(description="Read and parse a YAML file")
+parser.add_argument(
+    "--infile", help="The YAML input file"
 )
-parser.add_argument("--infile", default="tests/test.csv", help="The CSV input file")
 args = parser.parse_args()
 
 path = xlsforms_path.replace("/xlsforms", "")
-csv = Convert(f"{path}/xforms.yaml")
+infile = f"{path}/xforms.yaml"
+data = YamlFile(infile)
+# data.dump()
+
+def test_load():
+    """See if the file got loaded"""
+    hits = 0
+    if len(data.yaml.keys()) > 0:
+        hits = 1
+    if len(data.yaml['convert']) > 0:
+        hits += 1
+    if len(data.yaml['ignore']) > 0:
+        hits += 1
+    if len(data.yaml['private']) > 0:
+        hits += 1
+    assert hits == 4
+
+def test_good():
+    hits = 0
+    if data.convertData('amenity'):
+        hits += 1
+    if data.convertData('foobar') == False:
+        hits += 1
+    assert hits == 2
+
+def test_private():
+    hits = 0
+    if data.privateData('income'):
+        hits += 1
+    if data.privateData('foobar') == False:
+        hits += 1
+    assert hits == 2
+
+def test_ignore():
+    hits = 0
+    if data.ignoreData('model'):
+        hits += 1
+    if data.ignoreData('foobar') == False:
+        hits += 1
+    assert hits == 2
+
+# def test_bool_bad():
+#     assert "bad keyword" data.yaml['convert'] is not True
+
 
-def test_get_keyword():
-    """Convert a feature"""
-    if "sac_scale" in csv.yaml.yaml["tags"]:
-        assert 0
-    else:
-        assert 1
-
-
-def test_no_keyword():
-    """Convert a feature that doesn't exist"""
-    if "sac_scale" in csv.yaml.yaml["convert"]:
-        csv.getKeyword("doesn't exist")
-        assert 0
-    else:
-        assert 1
-
-
-# def test_convert_list():
-#     """Convert a list of features"""
-#     features = list()
-#     features.append("firepit")
-#     features.append("parking")
-#     features.append("viewpoint")
-#     result = csv.convertList(features)
-#     assert result[0]['leisure'] == "firepit" and result[1]['amenity'] == "parking" and result[2]['tourism'] == "viewpoint"
-
-# def test_bool_keyword():
-#     """Convert a feature"""
-#     result = csv.getKeyword("bear box")
-#     assert result == "bear box"
-
-
-def test_convert_tag():
-    tmp1 = csv.convertTag("altitude")
-    tmp2 = csv.convertTag("foobar")
-    assert tmp1 == "ele" and tmp2 == "foobar"
+# def test_value():
+#     assert "caravans" == "tourism"
 
 
-# Run standalone for easier debugging when not under pytest
 if __name__ == "__main__":
-    test_get_keyword()
-    test_no_keyword()
-    #    test_convert_list()
-    #    test_bool_keyword()
-    test_convert_tag()
+    test_load()
+    test_good()
+    test_private()
+    test_ignore()
```

### Comparing `osm-fieldwork-0.3.3/tests/test_csv.py` & `osm-fieldwork-0.3.4/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/test_osm.py` & `osm-fieldwork-0.3.4/tests/test_osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/test_uriparser.py` & `osm-fieldwork-0.3.4/tests/test_uriparser.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/testdata/Salida.geojson` & `osm-fieldwork-0.3.4/tests/testdata/Salida.geojson`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/testdata/odk_pois.osm` & `osm-fieldwork-0.3.4/tests/testdata/odk_pois.osm`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/tests/testdata/osm_buildings.geojson` & `osm-fieldwork-0.3.4/tests/testdata/osm_buildings.geojson`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.3.3/PKG-INFO` & `osm-fieldwork-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.3.3
+Version: 0.3.4
 Summary: Convert CSV files from ODK Central to OSM format.
 License: GPL-3.0-only
 Keywords: fmtm,odk,hot,openstreetmap,opendatakit
 Author-email: Rob Savoye <rob.savoye@hotosm.org>
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

