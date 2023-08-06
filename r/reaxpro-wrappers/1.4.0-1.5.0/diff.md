# Comparing `tmp/reaxpro-wrappers-1.4.0.tar.gz` & `tmp/reaxpro-wrappers-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.4.0.tar", last modified: Fri Aug  4 08:48:53 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.5.0.tar", last modified: Sun Aug  6 14:42:43 2023, max compression
```

## Comparing `reaxpro-wrappers-1.4.0.tar` & `reaxpro-wrappers-1.5.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.006883 reaxpro-wrappers-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-04 08:48:53.006883 reaxpro-wrappers-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.994882 reaxpro-wrappers-1.4.0/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.994882 reaxpro-wrappers-1.4.0/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/co_pt111_meso.json
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/energy_landscape.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/ams/pesexploration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/models/multiscale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/multiscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20608 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/multiscale/co_pt111_meso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:52.998882 reaxpro-wrappers-1.4.0/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49172 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    78524 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.002883 reaxpro-wrappers-1.4.0/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.006883 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-04 08:48:52.000000 reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-04 08:48:53.006883 reaxpro-wrappers-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-04 08:48:32.000000 reaxpro-wrappers-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:48:53.006883 reaxpro-wrappers-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-08-04 08:48:33.000000 reaxpro-wrappers-1.4.0/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-04 08:48:33.000000 reaxpro-wrappers-1.4.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-04 08:48:33.000000 reaxpro-wrappers-1.4.0/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-04 08:48:33.000000 reaxpro-wrappers-1.4.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.125607 reaxpro-wrappers-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-06 14:42:43.125607 reaxpro-wrappers-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.117607 reaxpro-wrappers-1.5.0/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.117607 reaxpro-wrappers-1.5.0/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.117607 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/co_pt111_meso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/energy_landscape.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/ams/pesexploration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.117607 reaxpro-wrappers-1.5.0/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.117607 reaxpro-wrappers-1.5.0/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/multiscale/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/multiscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20608 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/multiscale/co_pt111_meso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49172 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78572 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.121607 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-06 14:42:43.000000 reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-06 14:42:43.125607 reaxpro-wrappers-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-06 14:42:26.000000 reaxpro-wrappers-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:42:43.125607 reaxpro-wrappers-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-08-06 14:42:27.000000 reaxpro-wrappers-1.5.0/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-06 14:42:27.000000 reaxpro-wrappers-1.5.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-08-06 14:42:27.000000 reaxpro-wrappers-1.5.0/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-06 14:42:27.000000 reaxpro-wrappers-1.5.0/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.4.0/LICENSE` & `reaxpro-wrappers-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/PKG-INFO` & `reaxpro-wrappers-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.4.0
+Version: 1.5.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.4.0/README.md` & `reaxpro-wrappers-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.5.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/ams/co_pt111_meso.json` & `reaxpro-wrappers-1.5.0/osp/dictionaries/ams/co_pt111_meso.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.5.0/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.5.0/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/CO_ads+Pt111.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.5.0/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.5.0/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/models/multiscale/co_pt111_meso.py` & `reaxpro-wrappers-1.5.0/osp/models/multiscale/co_pt111_meso.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/models/settings/general.py` & `reaxpro-wrappers-1.5.0/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/models/utils/general.py` & `reaxpro-wrappers-1.5.0/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.5.0/osp/models/zacros/co_pyzacros.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.5.0/osp/tools/graph_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/tools/io_functions.py` & `reaxpro-wrappers-1.5.0/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.5.0/osp/tools/mapping_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
         if search_landscape:
             plams_molecule = map_PLAMSLandscape(search_landscape[0])
 
         else:
             plams_molecule = map_PLAMSMolecule(root_cuds_object)
 
-        plams_settings = map_PLAMSSettings(self.workdir, root_cuds_object)
+        path = os.path.join(self.workdir, self.jobname)
+        plams_settings = map_PLAMSSettings(path, root_cuds_object)
 
         return (plams_molecule, plams_settings)
 
     elif engine == "Zacros":
 
         software = emmo.Zacros()
         root_cuds_object.add(software, rel=emmo.hasModellingSoftware)
```

### Comparing `reaxpro-wrappers-1.4.0/osp/tools/set_functions.py` & `reaxpro-wrappers-1.5.0/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.5.0/osp/wrappers/simams/simams_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 """Describe AMS Session class."""
 from osp.core.session import SimWrapperSession
 from osp.core.cuds import Cuds
 from osp.tools.graph_functions import graph_wrapper_dependencies
 from osp.tools.mapping_functions import map_function, map_results
-from scm.plams import init as PlamsInit
+from scm.plams import init, config
 from scm.plams import MultiJob, AMSJob
-import tempfile
-import os
+from uuid import uuid4
 # from osp.core.utils import pretty_print
 
 
 class SimamsSession(SimWrapperSession):
     """Describe AMS Session class."""
 
     def __init__(self, engine=None, **kwargs):
         """Initialise SimamsSession."""
         if engine is None:
-            path = tempfile.mkdtemp()
-            folder = "plams_workdir"
-            jobname = "plamsjob"
-            PlamsInit(path=path, folder = folder)
-            self.workdir = os.path.join(path, folder, jobname)
-            self.engine = MultiJob(name=jobname)
+            init()
+            self.workdir = config.get("default_jobmanager").workdir
+            self.jobname = str(uuid4())
+            self.engine = MultiJob(name=self.jobname)
         super().__init__(engine)
 
     def __str__(self):
         """To overwrite the private str method. Not advised, but here it is."""
         # TODO: Define the output of str(SomeSimulationSession())
         return "Some Wrapper Session"
```

### Comparing `reaxpro-wrappers-1.4.0/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.5.0/osp/wrappers/simzacros/simzacros_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.4.0
+Version: 1.5.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.4.0/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.5.0/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/setup.cfg` & `reaxpro-wrappers-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.4.0
+version = v1.5.0
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.4.0/setup.py` & `reaxpro-wrappers-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.5.0/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/tests/test_examples.py` & `reaxpro-wrappers-1.5.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.5.0/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.4.0/tests/test_tools.py` & `reaxpro-wrappers-1.5.0/tests/test_tools.py`

 * *Files identical despite different names*

