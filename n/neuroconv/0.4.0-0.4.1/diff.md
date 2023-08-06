# Comparing `tmp/neuroconv-0.4.0.tar.gz` & `tmp/neuroconv-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroconv-0.4.0.tar", last modified: Sun Jul 23 19:19:38 2023, max compression
+gzip compressed data, was "neuroconv-0.4.1.tar", last modified: Sun Aug  6 19:19:17 2023, max compression
```

## Comparing `neuroconv-0.4.0.tar` & `neuroconv-0.4.1.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.665921 neuroconv-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-23 19:19:32.000000 neuroconv-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-23 19:19:38.665921 neuroconv-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-23 19:19:32.000000 neuroconv-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-23 19:19:32.000000 neuroconv-0.4.0/base_gin_test_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-23 19:19:32.000000 neuroconv-0.4.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-23 19:19:32.000000 neuroconv-0.4.0/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-23 19:19:32.000000 neuroconv-0.4.0/make_environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-23 19:19:32.000000 neuroconv-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:19:38.665921 neuroconv-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-23 19:19:32.000000 neuroconv-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.633921 neuroconv-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.637920 neuroconv-0.4.0/src/neuroconv/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/basedatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/baseextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/basetemporalalignmentinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/audio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/miniscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/miniscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/miniscope/miniscopedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/video_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21369 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/alphaomega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/alphaomega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/biocam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/biocam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/edf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/edf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/intan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/intan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.645921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/kilosort/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/kilosort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/maxwell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/maxwell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mcsraw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mcsraw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mearec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mearec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuralynx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuralynx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/phy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/phy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/plexon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/plexon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.649921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spike2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spike2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/tdt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/tdt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/abf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/abf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/brukertiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/brukertiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/caiman/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/cnmfe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/cnmfe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/cnmfe/cnmfedatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.653921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/extract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeimagingdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sbx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/scanimage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/scanimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/suite2p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/tiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/tiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/csv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/csv/csvtimeintertervalsinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.657921 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/excel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/excel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/datainterfaces/text/timeintervalsinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/nwbconverter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.661921 neuroconv-0.4.0/src/neuroconv/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/schemas/base_metadata_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/schemas/metadata_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/schemas/source_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/schemas/time_series_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/schemas/yaml_conversion_specification_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.661921 neuroconv-0.4.0/src/neuroconv/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.661921 neuroconv-0.4.0/src/neuroconv/tools/audio/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/audio/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/data_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/figshare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/hdmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.661921 neuroconv-0.4.0/src/neuroconv/tools/neo/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/neo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/neo/neo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/nwb_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/path_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/processes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.661921 neuroconv-0.4.0/src/neuroconv/tools/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/roiextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    46767 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/roiextractors/roiextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/signal_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.665921 neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69197 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/spikeinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.665921 neuroconv-0.4.0/src/neuroconv/tools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt
--rw-r--r--   0 runner    (1001) docker     (123)    33413 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/data_interface_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/mock_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/mock_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/testing/mock_ttl_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.665921 neuroconv-0.4.0/src/neuroconv/tools/yaml_conversion_specification/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/yaml_conversion_specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.665921 neuroconv-0.4.0/src/neuroconv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-23 19:19:32.000000 neuroconv-0.4.0/src/neuroconv/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:19:38.641921 neuroconv-0.4.0/src/neuroconv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 19:19:38.000000 neuroconv-0.4.0/src/neuroconv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.193287 neuroconv-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-06 19:19:12.000000 neuroconv-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-06 19:19:17.193287 neuroconv-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-08-06 19:19:12.000000 neuroconv-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-06 19:19:12.000000 neuroconv-0.4.1/base_gin_test_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-06 19:19:12.000000 neuroconv-0.4.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-06 19:19:12.000000 neuroconv-0.4.1/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-06 19:19:12.000000 neuroconv-0.4.1/make_environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-06 19:19:12.000000 neuroconv-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 19:19:17.193287 neuroconv-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-06 19:19:12.000000 neuroconv-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.173287 neuroconv-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/basedatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/baseextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/basetemporalalignmentinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/miniscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/miniscope/miniscopedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/video_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21369 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/alphaomega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/alphaomega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/biocam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/biocam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/cellexplorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/cellexplorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23974 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/edf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/edf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/intan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/intan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/kilosort/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/kilosort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/maxwell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mcsraw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mcsraw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mearec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mearec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuralynx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuralynx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.181287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/phy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/phy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/plexon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/plexon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spike2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spike2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikegadgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikegadgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/tdt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/tdt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/abf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/abf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/brukertiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/brukertiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/caiman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/cnmfe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/cnmfe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/cnmfe/cnmfedatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/micromanagertiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/micromanagertiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeimagingdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sbx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/scanimage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/scanimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.185287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/tiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/tiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/csv/csvtimeintertervalsinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/excel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/datainterfaces/text/timeintervalsinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/nwbconverter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/schemas/base_metadata_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/schemas/metadata_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/schemas/source_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/schemas/time_series_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/schemas/yaml_conversion_specification_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/tools/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/audio/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/data_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/figshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/hdmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/tools/neo/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/neo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/neo/neo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/nwb_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/path_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/processes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/tools/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/roiextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46773 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/roiextractors/roiextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/signal_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.189287 neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69197 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/spikeinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.193287 neuroconv-0.4.1/src/neuroconv/tools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    33413 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/data_interface_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/mock_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/mock_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/testing/mock_ttl_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.193287 neuroconv-0.4.1/src/neuroconv/tools/yaml_conversion_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/yaml_conversion_specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.193287 neuroconv-0.4.1/src/neuroconv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-06 19:19:12.000000 neuroconv-0.4.1/src/neuroconv/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 19:19:17.177287 neuroconv-0.4.1/src/neuroconv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-06 19:19:17.000000 neuroconv-0.4.1/src/neuroconv.egg-info/top_level.txt
```

### Comparing `neuroconv-0.4.0/PKG-INFO` & `neuroconv-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 Metadata-Version: 2.1
 Name: neuroconv
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert data from proprietary formats to NWB format.
 Home-page: https://github.com/catalystneuro/neuroconv
 Author: Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer, and Ben Dichter.
 Author-email: ben.dichter@catalystneuro.com
 License: BSD-3-Clause
 Keywords: nwb
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: full
 Provides-Extra: ophys
+Provides-Extra: brukertiff
 Provides-Extra: scanimage
-Provides-Extra: sima
-Provides-Extra: micromanagertiff
-Provides-Extra: sbx
-Provides-Extra: hdf5
-Provides-Extra: extract
 Provides-Extra: suite2p
-Provides-Extra: miniscope
-Provides-Extra: tiff
 Provides-Extra: caiman
+Provides-Extra: hdf5
+Provides-Extra: extract
 Provides-Extra: cnmfe
-Provides-Extra: brukertiff
+Provides-Extra: sima
+Provides-Extra: sbx
+Provides-Extra: tiff
+Provides-Extra: miniscope
+Provides-Extra: micromanagertiff
 Provides-Extra: ecephys
-Provides-Extra: mcsraw
+Provides-Extra: spike2
 Provides-Extra: tdt
-Provides-Extra: neuralynx
-Provides-Extra: cellexplorer
-Provides-Extra: alphaomega
+Provides-Extra: spikeglx
+Provides-Extra: maxwell
 Provides-Extra: blackrock
 Provides-Extra: edf
-Provides-Extra: spikeinterface
-Provides-Extra: maxwell
 Provides-Extra: intan
-Provides-Extra: neuroscope
 Provides-Extra: spikegadgets
-Provides-Extra: axona
-Provides-Extra: spikeglx
-Provides-Extra: spike2
 Provides-Extra: biocam
+Provides-Extra: plexon
+Provides-Extra: spikeinterface
 Provides-Extra: phy
-Provides-Extra: mearec
+Provides-Extra: alphaomega
 Provides-Extra: kilosort
+Provides-Extra: mearec
+Provides-Extra: neuralynx
+Provides-Extra: cellexplorer
 Provides-Extra: openephys
-Provides-Extra: plexon
+Provides-Extra: axona
+Provides-Extra: mcsraw
+Provides-Extra: neuroscope
 Provides-Extra: icephys
 Provides-Extra: abf
-Provides-Extra: video
-Provides-Extra: behavior
-Provides-Extra: sleap
 Provides-Extra: deeplabcut
+Provides-Extra: behavior
+Provides-Extra: video
 Provides-Extra: audio
-Provides-Extra: csv
+Provides-Extra: sleap
 Provides-Extra: excel
 Provides-Extra: text
+Provides-Extra: csv
 License-File: license.txt
 
 [![PyPI version](https://badge.fury.io/py/neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg)
 ![Full Tests](https://github.com/catalystneuro/neuroconv/actions/workflows/testing.yml/badge.svg)
 ![Auto-release](https://github.com/catalystneuro/neuroconv/actions/workflows/auto-publish.yml/badge.svg)
 [![codecov](https://codecov.io/github/catalystneuro/neuroconv/coverage.svg?branch=main)](https://codecov.io/github/catalystneuro/neuroconv?branch=main)
 [![documentation](https://readthedocs.org/projects/neuroconv/badge/?version=main)](https://neuroconv.readthedocs.io/en/main/)
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: neuroconv Version: 0.4.0 Summary: Convert data from
+Metadata-Version: 2.1 Name: neuroconv Version: 0.4.1 Summary: Convert data from
 proprietary formats to NWB format. Home-page: https://github.com/catalystneuro/
 neuroconv Author: Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer,
 and Ben Dichter. Author-email: ben.dichter@catalystneuro.com License: BSD-3-
 Clause Keywords: nwb Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: test Provides-Extra: docs Provides-Extra: full
-Provides-Extra: ophys Provides-Extra: scanimage Provides-Extra: sima Provides-
-Extra: micromanagertiff Provides-Extra: sbx Provides-Extra: hdf5 Provides-
-Extra: extract Provides-Extra: suite2p Provides-Extra: miniscope Provides-
-Extra: tiff Provides-Extra: caiman Provides-Extra: cnmfe Provides-Extra:
-brukertiff Provides-Extra: ecephys Provides-Extra: mcsraw Provides-Extra: tdt
+Provides-Extra: ophys Provides-Extra: brukertiff Provides-Extra: scanimage
+Provides-Extra: suite2p Provides-Extra: caiman Provides-Extra: hdf5 Provides-
+Extra: extract Provides-Extra: cnmfe Provides-Extra: sima Provides-Extra: sbx
+Provides-Extra: tiff Provides-Extra: miniscope Provides-Extra: micromanagertiff
+Provides-Extra: ecephys Provides-Extra: spike2 Provides-Extra: tdt Provides-
+Extra: spikeglx Provides-Extra: maxwell Provides-Extra: blackrock Provides-
+Extra: edf Provides-Extra: intan Provides-Extra: spikegadgets Provides-Extra:
+biocam Provides-Extra: plexon Provides-Extra: spikeinterface Provides-Extra:
+phy Provides-Extra: alphaomega Provides-Extra: kilosort Provides-Extra: mearec
 Provides-Extra: neuralynx Provides-Extra: cellexplorer Provides-Extra:
-alphaomega Provides-Extra: blackrock Provides-Extra: edf Provides-Extra:
-spikeinterface Provides-Extra: maxwell Provides-Extra: intan Provides-Extra:
-neuroscope Provides-Extra: spikegadgets Provides-Extra: axona Provides-Extra:
-spikeglx Provides-Extra: spike2 Provides-Extra: biocam Provides-Extra: phy
-Provides-Extra: mearec Provides-Extra: kilosort Provides-Extra: openephys
-Provides-Extra: plexon Provides-Extra: icephys Provides-Extra: abf Provides-
-Extra: video Provides-Extra: behavior Provides-Extra: sleap Provides-Extra:
-deeplabcut Provides-Extra: audio Provides-Extra: csv Provides-Extra: excel
-Provides-Extra: text License-File: license.txt [![PyPI version](https://
-badge.fury.io/py/neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg) ![Full
-Tests](https://github.com/catalystneuro/neuroconv/actions/workflows/
-testing.yml/badge.svg) ![Auto-release](https://github.com/catalystneuro/
-neuroconv/actions/workflows/auto-publish.yml/badge.svg) [![codecov](https://
-codecov.io/github/catalystneuro/neuroconv/coverage.svg?branch=main)](https://
-codecov.io/github/catalystneuro/neuroconv?branch=main) [![documentation](https:
-//readthedocs.org/projects/neuroconv/badge/?version=main)](https://
-neuroconv.readthedocs.io/en/main/) [![License](https://img.shields.io/pypi/l/
-neuroconv.svg)](https://github.com/catalystneuro/neuroconv/license.txt)
+openephys Provides-Extra: axona Provides-Extra: mcsraw Provides-Extra:
+neuroscope Provides-Extra: icephys Provides-Extra: abf Provides-Extra:
+deeplabcut Provides-Extra: behavior Provides-Extra: video Provides-Extra: audio
+Provides-Extra: sleap Provides-Extra: excel Provides-Extra: text Provides-
+Extra: csv License-File: license.txt [![PyPI version](https://badge.fury.io/py/
+neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg) ![Full Tests](https://
+github.com/catalystneuro/neuroconv/actions/workflows/testing.yml/badge.svg) !
+[Auto-release](https://github.com/catalystneuro/neuroconv/actions/workflows/
+auto-publish.yml/badge.svg) [![codecov](https://codecov.io/github/
+catalystneuro/neuroconv/coverage.svg?branch=main)](https://codecov.io/github/
+catalystneuro/neuroconv?branch=main) [![documentation](https://readthedocs.org/
+projects/neuroconv/badge/?version=main)](https://neuroconv.readthedocs.io/en/
+main/) [![License](https://img.shields.io/pypi/l/neuroconv.svg)](https://
+github.com/catalystneuro/neuroconv/license.txt)
                                [NeuroConv logo]
           **** Automatically convert neurophysiology data to NWB ****
                          Explore_our_documentation_Â»
  ## Table of Contents - [About](#about) - [Installation](#installation) -
 [Documentation](#documentation) - [License](#license) ## About NeuroConv is a
 Python package for converting neurophysiology data in a variety of proprietary
 formats to the [Neurodata Without Borders (NWB)](http://nwb.org) standard.
```

### Comparing `neuroconv-0.4.0/README.md` & `neuroconv-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/license.txt` & `neuroconv-0.4.1/license.txt`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/pyproject.toml` & `neuroconv-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/setup.py` & `neuroconv-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 gin_config_file_base = Path("./base_gin_test_config.json")
 gin_config_file_local = Path("./tests/test_on_data/gin_test_config.json")
 if not gin_config_file_local.exists():
     copy(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="neuroconv",
-    version="0.4.0",
+    version="0.4.1",
     description="Convert data from proprietary formats to NWB format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer, and Ben Dichter.",
     author_email="ben.dichter@catalystneuro.com",
     url="https://github.com/catalystneuro/neuroconv",
     keywords="nwb",
```

### Comparing `neuroconv-0.4.0/src/neuroconv/basedatainterface.py` & `neuroconv-0.4.1/src/neuroconv/basedatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/baseextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/baseextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/basetemporalalignmentinterface.py` & `neuroconv-0.4.1/src/neuroconv/basetemporalalignmentinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/__init__.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/audio/audiointerface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/deeplabcut/deeplabcutdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/miniscope/miniscopedatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/miniscope/miniscopedatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/sleap_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/sleap/sleapdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/video_utils.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/video_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/behavior/video/videodatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/alphaomega/alphaomegadatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/axona_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/axona/axonadatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/baselfpextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/baserecordingextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/basesortingextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/biocam/biocamdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/blackrockdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/blackrock/header_tools.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/cellexplorer/cellexplorerdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/edf/edfdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/intan/intandatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/kilosort/kilosortdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/maxwell/maxonedatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mcsraw/mcsrawdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/mearec/mearecdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuralynx/neuralynxdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscope_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/neuroscope/neuroscopedatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephysbinarydatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephysdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephyslegacydatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/openephys/openephyssortingdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/phy/phydatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/plexon/plexondatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spike2/spike2datainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikegadgets/spikegadgetsdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglx_utils.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxconverter.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/spikeglx/spikeglxnidqinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ecephys/tdt/tdtdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/abf/abfdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/icephys/baseicephysinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def get_metadata(self) -> dict:
         from ...tools.neo import get_number_of_electrodes
 
         metadata = super().get_metadata()
         metadata["Icephys"] = dict(
             Device=[dict(name="DeviceIcephys", description="no description")],
-            Electrode=[
+            Electrodes=[
                 dict(name=f"electrode-{i}", description="no description", device="DeviceIcephys")
                 for i in range(get_number_of_electrodes(self.readers_list[0]))
             ],
         )
         return metadata
 
     def get_original_timestamps(self) -> np.ndarray:
```

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/baseimagingextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/basesegmentationextractorinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/brukertiff/brukertiffdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/caiman/caimandatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/extract/extractdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/hdf5/hdf5datainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/micromanagertiff/micromanagertiffdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeconverter.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeconverter.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeimagingdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/miniscope/miniscopeimagingdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sbx/sbxdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/scanimage/scanimageimaginginterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/sima/simadatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/suite2p/suite2pdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/ophys/tiff/tiffdatainterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/text/excel/exceltimeintervalsinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/datainterfaces/text/timeintervalsinterface.py` & `neuroconv-0.4.1/src/neuroconv/datainterfaces/text/timeintervalsinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/nwbconverter.py` & `neuroconv-0.4.1/src/neuroconv/nwbconverter.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/schemas/base_metadata_schema.json` & `neuroconv-0.4.1/src/neuroconv/schemas/base_metadata_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/schemas/metadata_schema.json` & `neuroconv-0.4.1/src/neuroconv/schemas/metadata_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/schemas/source_schema.json` & `neuroconv-0.4.1/src/neuroconv/schemas/source_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/schemas/time_series_schema.json` & `neuroconv-0.4.1/src/neuroconv/schemas/time_series_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/schemas/yaml_conversion_specification_schema.json` & `neuroconv-0.4.1/src/neuroconv/schemas/yaml_conversion_specification_schema.json`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/audio/audio.py` & `neuroconv-0.4.1/src/neuroconv/tools/audio/audio.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/data_transfers.py` & `neuroconv-0.4.1/src/neuroconv/tools/data_transfers.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/figshare.py` & `neuroconv-0.4.1/src/neuroconv/tools/figshare.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/hdmf.py` & `neuroconv-0.4.1/src/neuroconv/tools/hdmf.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/importing.py` & `neuroconv-0.4.1/src/neuroconv/tools/importing.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/neo/neo.py` & `neuroconv-0.4.1/src/neuroconv/tools/neo/neo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import distutils.version
 import uuid
 import warnings
+from copy import deepcopy
 from pathlib import Path
 from typing import Optional, Tuple
 
 import neo.io.baseio
 import numpy as np
 import pynwb
 from hdmf.backends.hdf5 import H5DataIO
@@ -176,32 +177,34 @@
             description="no description",
             device_name=[i.name for i in nwbfile.devices.values()][0],
         )
         for elec_id in range(get_number_of_electrodes(neo_reader))
     ]
 
     if "Electrodes" not in metadata["Icephys"] or len(metadata["Icephys"]["Electrodes"]) == 0:
-        metadata["Icephys"]["Electrodes"] = defaults
+        metadata["Icephys"]["Electrodes"] = deepcopy(defaults)
 
     assert all(
         [isinstance(x, dict) for x in metadata["Icephys"]["Electrodes"]]
     ), "Expected metadata['Icephys']['Electrodes'] to be a list of dictionaries!"
 
     # Create Icephys electrode from metadata
     for elec in metadata["Icephys"]["Electrodes"]:
         if elec.get("name", defaults[0]["name"]) not in nwbfile.icephys_electrodes:
-            device_name = elec.get("device_name", defaults[0]["device_name"])
+            device_name = elec.pop("device_name", None) or elec.pop("device", defaults[0]["device_name"])
+            # elec.pop("device_name", 0)
             if device_name not in nwbfile.devices:
                 new_device_metadata = dict(Ecephys=dict(Device=[dict(name=device_name)]))
                 add_device_from_metadata(nwbfile, modality="Icephys", metadata=new_device_metadata)
                 warnings.warn(
                     f"Device '{device_name}' not detected in "
                     "attempted link to icephys electrode! Automatically generating."
                 )
-            electrode_kwargs = dict(
+            electrode_kwargs = elec
+            electrode_kwargs.update(
                 name=elec.get("name", defaults[0]["name"]),
                 description=elec.get("description", defaults[0]["description"]),
                 device=nwbfile.devices[device_name],
             )
             nwbfile.create_icephys_electrode(**electrode_kwargs)
```

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/nwb_helpers.py` & `neuroconv-0.4.1/src/neuroconv/tools/nwb_helpers.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/path_expansion.py` & `neuroconv-0.4.1/src/neuroconv/tools/path_expansion.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,31 +60,33 @@
         ...                 file_path="sub-{subject_id}/sub-{subject_id}_ses-{session_id}"
         ...             )
         ...         )
         ...     )
         ... )
         """
 
-        session_keys = {"session_start_time", "session_id", "subject_id"}
+        non_standard_super = "extras"
+        standard_metadata = {"session_id": "NWBFile", "session_start_time": "NWBFile", "subject_id": "Subject"}
 
         out = DeepDict()
         for interface, source_data in source_data_spec.items():
             for path_type in ("file_path", "folder_path"):
-                if path_type in source_data:
-                    for path, metadata in self.extract_metadata(source_data["base_directory"], source_data[path_type]):
-                        key = tuple((k, v) for k, v in sorted(metadata.items()) if k in session_keys)
-                        out[key]["source_data"][interface][path_type] = os.path.join(
-                            source_data["base_directory"], path
-                        )  # return the absolute path
-                        if "session_id" in metadata:
-                            out[key]["metadata"]["NWBFile"]["session_id"] = metadata["session_id"]
-                        if "session_start_time" in metadata:
-                            out[key]["metadata"]["NWBFile"]["session_start_time"] = metadata["session_start_time"]
-                        if "subject_id" in metadata:
-                            out[key]["metadata"]["Subject"]["subject_id"] = metadata["subject_id"]
+                if path_type not in source_data:
+                    continue
+
+                for path, metadata in self.extract_metadata(source_data["base_directory"], source_data[path_type]):
+                    key = tuple((k, v) for k, v in sorted(metadata.items()))
+                    out[key]["source_data"][interface][path_type] = os.path.join(
+                        source_data["base_directory"], path
+                    )  # return the absolute path
+
+                    for meta_key, meta_val in metadata.items():
+                        super_key = standard_metadata.get(meta_key, non_standard_super)
+                        out[key]["metadata"][super_key][meta_key] = meta_val
+
         return list(dict(out).values())
 
 
 class LocalPathExpander(AbstractPathExpander):
     def list_directory(self, base_directory: DirectoryPath) -> Iterable[FilePath]:
         base_directory = Path(base_directory)
         assert base_directory.is_dir(), f"The specified 'base_directory' ({base_directory}) is not a directory!"
```

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/processes.py` & `neuroconv-0.4.1/src/neuroconv/tools/processes.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py` & `neuroconv-0.4.1/src/neuroconv/tools/roiextractors/imagingextractordatachunkiterator.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/roiextractors/roiextractors.py` & `neuroconv-0.4.1/src/neuroconv/tools/roiextractors/roiextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,17 +815,17 @@
 
     # Get traces from the segmentation extractor
     traces_to_add = segmentation_extractor.get_traces_dict()
 
     # Filter empty data
     traces_to_add = {trace_name: trace for trace_name, trace in traces_to_add.items() if trace is not None}
     # Filter all zero data
-    traces_to_add = {
-        trace_name: trace for trace_name, trace in traces_to_add.items() if any(x != 0 for x in np.ravel(trace))
-    }
+    # traces_to_add = {
+    #     trace_name: trace for trace_name, trace in traces_to_add.items() if any(x != 0 for x in np.ravel(trace))
+    # }
 
     # Early return if there is nothing to add
     if not traces_to_add:
         return nwbfile
 
     # Create a reference for ROIs from the plane segmentation
     roi_table_region = _create_roi_table_region(
```

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/signal_processing.py` & `neuroconv-0.4.1/src/neuroconv/tools/signal_processing.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/spikeinterface.py` & `neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/spikeinterface.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py` & `neuroconv-0.4.1/src/neuroconv/tools/spikeinterface/spikeinterfacerecordingdatachunkiterator.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt` & `neuroconv-0.4.1/src/neuroconv/tools/testing/_path_expander_demo_ibl_filepaths.txt`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/testing/data_interface_mixins.py` & `neuroconv-0.4.1/src/neuroconv/tools/testing/data_interface_mixins.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/testing/mock_files.py` & `neuroconv-0.4.1/src/neuroconv/tools/testing/mock_files.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/testing/mock_interfaces.py` & `neuroconv-0.4.1/src/neuroconv/tools/testing/mock_interfaces.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/testing/mock_ttl_signals.py` & `neuroconv-0.4.1/src/neuroconv/tools/testing/mock_ttl_signals.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/text.py` & `neuroconv-0.4.1/src/neuroconv/tools/text.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py` & `neuroconv-0.4.1/src/neuroconv/tools/yaml_conversion_specification/yaml_conversion_specification.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/utils/__init__.py` & `neuroconv-0.4.1/src/neuroconv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/utils/checks.py` & `neuroconv-0.4.1/src/neuroconv/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/utils/dict.py` & `neuroconv-0.4.1/src/neuroconv/utils/dict.py`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv/utils/json_schema.py` & `neuroconv-0.4.1/src/neuroconv/utils/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,18 +263,18 @@
     if "allow_extra" in docval:
         schema["additionalProperties"] = docval["allow_extra"]
     return schema
 
 
 def get_metadata_schema_for_icephys():
     schema = get_base_schema(tag="Icephys")
-    schema["required"] = ["Device", "Electrode"]
+    schema["required"] = ["Device", "Electrodes"]
     schema["properties"] = dict(
         Device=dict(type="array", minItems=1, items={"$ref": "#/properties/Icephys/properties/definitions/Device"}),
-        Electrode=dict(
+        Electrodes=dict(
             type="array",
             minItems=1,
             items={"$ref": "#/properties/Icephys/properties/definitions/Electrode"},
         ),
         Sessions=dict(
             type="array",
             minItems=1,
```

### Comparing `neuroconv-0.4.0/src/neuroconv.egg-info/PKG-INFO` & `neuroconv-0.4.1/src/neuroconv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 Metadata-Version: 2.1
 Name: neuroconv
-Version: 0.4.0
+Version: 0.4.1
 Summary: Convert data from proprietary formats to NWB format.
 Home-page: https://github.com/catalystneuro/neuroconv
 Author: Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer, and Ben Dichter.
 Author-email: ben.dichter@catalystneuro.com
 License: BSD-3-Clause
 Keywords: nwb
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: full
 Provides-Extra: ophys
+Provides-Extra: brukertiff
 Provides-Extra: scanimage
-Provides-Extra: sima
-Provides-Extra: micromanagertiff
-Provides-Extra: sbx
-Provides-Extra: hdf5
-Provides-Extra: extract
 Provides-Extra: suite2p
-Provides-Extra: miniscope
-Provides-Extra: tiff
 Provides-Extra: caiman
+Provides-Extra: hdf5
+Provides-Extra: extract
 Provides-Extra: cnmfe
-Provides-Extra: brukertiff
+Provides-Extra: sima
+Provides-Extra: sbx
+Provides-Extra: tiff
+Provides-Extra: miniscope
+Provides-Extra: micromanagertiff
 Provides-Extra: ecephys
-Provides-Extra: mcsraw
+Provides-Extra: spike2
 Provides-Extra: tdt
-Provides-Extra: neuralynx
-Provides-Extra: cellexplorer
-Provides-Extra: alphaomega
+Provides-Extra: spikeglx
+Provides-Extra: maxwell
 Provides-Extra: blackrock
 Provides-Extra: edf
-Provides-Extra: spikeinterface
-Provides-Extra: maxwell
 Provides-Extra: intan
-Provides-Extra: neuroscope
 Provides-Extra: spikegadgets
-Provides-Extra: axona
-Provides-Extra: spikeglx
-Provides-Extra: spike2
 Provides-Extra: biocam
+Provides-Extra: plexon
+Provides-Extra: spikeinterface
 Provides-Extra: phy
-Provides-Extra: mearec
+Provides-Extra: alphaomega
 Provides-Extra: kilosort
+Provides-Extra: mearec
+Provides-Extra: neuralynx
+Provides-Extra: cellexplorer
 Provides-Extra: openephys
-Provides-Extra: plexon
+Provides-Extra: axona
+Provides-Extra: mcsraw
+Provides-Extra: neuroscope
 Provides-Extra: icephys
 Provides-Extra: abf
-Provides-Extra: video
-Provides-Extra: behavior
-Provides-Extra: sleap
 Provides-Extra: deeplabcut
+Provides-Extra: behavior
+Provides-Extra: video
 Provides-Extra: audio
-Provides-Extra: csv
+Provides-Extra: sleap
 Provides-Extra: excel
 Provides-Extra: text
+Provides-Extra: csv
 License-File: license.txt
 
 [![PyPI version](https://badge.fury.io/py/neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg)
 ![Full Tests](https://github.com/catalystneuro/neuroconv/actions/workflows/testing.yml/badge.svg)
 ![Auto-release](https://github.com/catalystneuro/neuroconv/actions/workflows/auto-publish.yml/badge.svg)
 [![codecov](https://codecov.io/github/catalystneuro/neuroconv/coverage.svg?branch=main)](https://codecov.io/github/catalystneuro/neuroconv?branch=main)
 [![documentation](https://readthedocs.org/projects/neuroconv/badge/?version=main)](https://neuroconv.readthedocs.io/en/main/)
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: neuroconv Version: 0.4.0 Summary: Convert data from
+Metadata-Version: 2.1 Name: neuroconv Version: 0.4.1 Summary: Convert data from
 proprietary formats to NWB format. Home-page: https://github.com/catalystneuro/
 neuroconv Author: Cody Baker, Szonja Weigl, Heberto Mayorquin, Luiz Tauffer,
 and Ben Dichter. Author-email: ben.dichter@catalystneuro.com License: BSD-3-
 Clause Keywords: nwb Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Provides-Extra: test Provides-Extra: docs Provides-Extra: full
-Provides-Extra: ophys Provides-Extra: scanimage Provides-Extra: sima Provides-
-Extra: micromanagertiff Provides-Extra: sbx Provides-Extra: hdf5 Provides-
-Extra: extract Provides-Extra: suite2p Provides-Extra: miniscope Provides-
-Extra: tiff Provides-Extra: caiman Provides-Extra: cnmfe Provides-Extra:
-brukertiff Provides-Extra: ecephys Provides-Extra: mcsraw Provides-Extra: tdt
+Provides-Extra: ophys Provides-Extra: brukertiff Provides-Extra: scanimage
+Provides-Extra: suite2p Provides-Extra: caiman Provides-Extra: hdf5 Provides-
+Extra: extract Provides-Extra: cnmfe Provides-Extra: sima Provides-Extra: sbx
+Provides-Extra: tiff Provides-Extra: miniscope Provides-Extra: micromanagertiff
+Provides-Extra: ecephys Provides-Extra: spike2 Provides-Extra: tdt Provides-
+Extra: spikeglx Provides-Extra: maxwell Provides-Extra: blackrock Provides-
+Extra: edf Provides-Extra: intan Provides-Extra: spikegadgets Provides-Extra:
+biocam Provides-Extra: plexon Provides-Extra: spikeinterface Provides-Extra:
+phy Provides-Extra: alphaomega Provides-Extra: kilosort Provides-Extra: mearec
 Provides-Extra: neuralynx Provides-Extra: cellexplorer Provides-Extra:
-alphaomega Provides-Extra: blackrock Provides-Extra: edf Provides-Extra:
-spikeinterface Provides-Extra: maxwell Provides-Extra: intan Provides-Extra:
-neuroscope Provides-Extra: spikegadgets Provides-Extra: axona Provides-Extra:
-spikeglx Provides-Extra: spike2 Provides-Extra: biocam Provides-Extra: phy
-Provides-Extra: mearec Provides-Extra: kilosort Provides-Extra: openephys
-Provides-Extra: plexon Provides-Extra: icephys Provides-Extra: abf Provides-
-Extra: video Provides-Extra: behavior Provides-Extra: sleap Provides-Extra:
-deeplabcut Provides-Extra: audio Provides-Extra: csv Provides-Extra: excel
-Provides-Extra: text License-File: license.txt [![PyPI version](https://
-badge.fury.io/py/neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg) ![Full
-Tests](https://github.com/catalystneuro/neuroconv/actions/workflows/
-testing.yml/badge.svg) ![Auto-release](https://github.com/catalystneuro/
-neuroconv/actions/workflows/auto-publish.yml/badge.svg) [![codecov](https://
-codecov.io/github/catalystneuro/neuroconv/coverage.svg?branch=main)](https://
-codecov.io/github/catalystneuro/neuroconv?branch=main) [![documentation](https:
-//readthedocs.org/projects/neuroconv/badge/?version=main)](https://
-neuroconv.readthedocs.io/en/main/) [![License](https://img.shields.io/pypi/l/
-neuroconv.svg)](https://github.com/catalystneuro/neuroconv/license.txt)
+openephys Provides-Extra: axona Provides-Extra: mcsraw Provides-Extra:
+neuroscope Provides-Extra: icephys Provides-Extra: abf Provides-Extra:
+deeplabcut Provides-Extra: behavior Provides-Extra: video Provides-Extra: audio
+Provides-Extra: sleap Provides-Extra: excel Provides-Extra: text Provides-
+Extra: csv License-File: license.txt [![PyPI version](https://badge.fury.io/py/
+neuroconv.svg)](https://badge.fury.io/py/neuroconv.svg) ![Full Tests](https://
+github.com/catalystneuro/neuroconv/actions/workflows/testing.yml/badge.svg) !
+[Auto-release](https://github.com/catalystneuro/neuroconv/actions/workflows/
+auto-publish.yml/badge.svg) [![codecov](https://codecov.io/github/
+catalystneuro/neuroconv/coverage.svg?branch=main)](https://codecov.io/github/
+catalystneuro/neuroconv?branch=main) [![documentation](https://readthedocs.org/
+projects/neuroconv/badge/?version=main)](https://neuroconv.readthedocs.io/en/
+main/) [![License](https://img.shields.io/pypi/l/neuroconv.svg)](https://
+github.com/catalystneuro/neuroconv/license.txt)
                                [NeuroConv logo]
           **** Automatically convert neurophysiology data to NWB ****
                          Explore_our_documentation_Â»
  ## Table of Contents - [About](#about) - [Installation](#installation) -
 [Documentation](#documentation) - [License](#license) ## About NeuroConv is a
 Python package for converting neurophysiology data in a variety of proprietary
 formats to the [Neurodata Without Borders (NWB)](http://nwb.org) standard.
```

### Comparing `neuroconv-0.4.0/src/neuroconv.egg-info/SOURCES.txt` & `neuroconv-0.4.1/src/neuroconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroconv-0.4.0/src/neuroconv.egg-info/requires.txt` & `neuroconv-0.4.1/src/neuroconv.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 ndx-sound>=0.2.0
 
 [axona]
 spikeinterface>=0.98.2
 packaging<22.0
 
 [behavior]
+dlc2nwb>=0.3
+tables
 opencv-python-headless>=4.5.1.48
 ndx-miniscope>=0.5.1
 natsort>=8.3.1
+ndx-sound>=0.2.0
 sleap-io>=0.0.2
 av>=10.0.0
-dlc2nwb>=0.3
-tables
-ndx-sound>=0.2.0
 
 [behavior:sys_platform == "darwin"]
 opencv-python-headless<4.7.0.72,>=4.5.1.48
 
 [behavior:sys_platform == "darwin" and python_version >= "3.11"]
 opencv-python-headless<4.7,>=4.5.1.48
 
@@ -82,23 +82,23 @@
 sphinx-toggleprompt==0.2.0
 sphinx-copybutton==0.5.0
 roiextractors
 
 [ecephys]
 spikeinterface>=0.98.2
 packaging<22.0
-natsort>=7.1.1
-hdf5storage>=0.1.18
-pymatreader>=0.0.32
 pyedflib>=0.1.30
-spikeextractors
 pyintan>=0.3.0
-lxml>=4.6.5
+spikeextractors
 MEArec>=1.8.0
+natsort>=7.1.1
+hdf5storage>=0.1.18
+pymatreader>=0.0.32
 pyopenephys>=1.1.2
+lxml>=4.6.5
 
 [ecephys:python_version <= "3.9"]
 sonpy>=1.7.1
 
 [ecephys:python_version >= "3.11"]
 numpy<1.25.0
 
@@ -115,38 +115,38 @@
 xlrd
 
 [extract]
 roiextractors>=0.5.3
 
 [full]
 roiextractors>=0.5.3
-scanimage-tiff-reader>=1.4.1
 tifffile>=2023.3.21
+scanimage-tiff-reader>=1.4.1
+tiffile>=2018.10.18
 ndx-miniscope>=0.5.1
 natsort>=8.3.1
-tiffile>=2018.10.18
 spikeinterface>=0.98.2
 packaging<22.0
-natsort>=7.1.1
-hdf5storage>=0.1.18
-pymatreader>=0.0.32
 pyedflib>=0.1.30
-spikeextractors
 pyintan>=0.3.0
-lxml>=4.6.5
+spikeextractors
 MEArec>=1.8.0
+natsort>=7.1.1
+hdf5storage>=0.1.18
+pymatreader>=0.0.32
 pyopenephys>=1.1.2
+lxml>=4.6.5
 neo>=0.9.0
 ndx-dandi-icephys>=0.4.0
-opencv-python-headless>=4.5.1.48
-sleap-io>=0.0.2
-av>=10.0.0
 dlc2nwb>=0.3
 tables
+opencv-python-headless>=4.5.1.48
 ndx-sound>=0.2.0
+sleap-io>=0.0.2
+av>=10.0.0
 openpyxl
 xlrd
 
 [full:python_version <= "3.9"]
 sonpy>=1.7.1
 
 [full:python_version >= "3.11"]
@@ -209,19 +209,19 @@
 [openephys]
 spikeinterface>=0.98.2
 packaging<22.0
 pyopenephys>=1.1.2
 
 [ophys]
 roiextractors>=0.5.3
-scanimage-tiff-reader>=1.4.1
 tifffile>=2023.3.21
+scanimage-tiff-reader>=1.4.1
+tiffile>=2018.10.18
 ndx-miniscope>=0.5.1
 natsort>=8.3.1
-tiffile>=2018.10.18
 
 [phy]
 spikeinterface>=0.98.2
 packaging<22.0
 
 [plexon]
 spikeinterface>=0.98.2
```

