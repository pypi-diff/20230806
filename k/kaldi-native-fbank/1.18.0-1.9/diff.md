# Comparing `tmp/kaldi-native-fbank-1.18.0.tar.gz` & `tmp/kaldi-native-fbank-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaldi-native-fbank-1.18.0.tar", last modified: Sun Aug  6 08:33:59 2023, max compression
+gzip compressed data, was "kaldi-native-fbank-1.9.tar", last modified: Thu Jan  5 03:30:38 2023, max compression
```

## Comparing `kaldi-native-fbank-1.18.0.tar` & `kaldi-native-fbank-1.9.tar`

### file list

```diff
@@ -1,83 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.287465 kaldi-native-fbank-1.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-06 08:33:59.287465 kaldi-native-fbank-1.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.275466 kaldi-native-fbank-1.18.0/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.275466 kaldi-native-fbank-1.18.0/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.275466 kaldi-native-fbank-1.18.0/cmake/Modules/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/Modules/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/Modules/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.275466 kaldi-native-fbank-1.18.0/cmake/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/cmake/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/cmake/__pycache__/cmake_extension.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/cmake_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/cmake/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.275466 kaldi-native-fbank-1.18.0/kaldi-native-fbank/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.279466 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-fbank.h
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-functions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-window.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-window.h
--rw-r--r--   0 runner    (1001) docker     (123)    80227 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/fftsg.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/generate-whisper-melbank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/log.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/log.h
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/mel-computations.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/mel-computations.h
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/online-feature.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/online-feature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/rfft.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/rfft.h
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-log.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-online-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-online-feature.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-rfft.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/whisper-feature.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/whisper-feature.h
--rw-r--r--   0 runner    (1001) docker     (123)   206745 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/whisper-mel-bank.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.279466 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.283465 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-fbank.h
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-window.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-window.h
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/kaldi-native-fbank.cc
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/kaldi-native-fbank.h
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/mel-computations.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/mel-computations.h
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/online-feature.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/online-feature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/rfft.cc
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/rfft.h
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.283465 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/kaldi_native_fbank/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/kaldi_native_fbank/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.283465 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5202 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_fbank_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      718 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_feature_window_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2787 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_frame_extraction_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_mel_bank_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_online_fbank.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1304 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_online_whisper_fbank.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_rfft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 08:33:59.287465 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-06 08:33:59.000000 kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 08:33:59.287465 kaldi-native-fbank-1.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-06 08:23:20.000000 kaldi-native-fbank-1.18.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.645781 kaldi-native-fbank-1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-01-05 03:30:38.641781 kaldi-native-fbank-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.633781 kaldi-native-fbank-1.9/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.633781 kaldi-native-fbank-1.9/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.633781 kaldi-native-fbank-1.9/cmake/Modules/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/Modules/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/Modules/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.633781 kaldi-native-fbank-1.9/cmake/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-01-05 03:30:37.000000 kaldi-native-fbank-1.9/cmake/__pycache__/cmake_extension.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/cmake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/cmake/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.633781 kaldi-native-fbank-1.9/kaldi-native-fbank/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.637781 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-fbank.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-functions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-window.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-window.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80007 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/fftsg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/log.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/mel-computations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/mel-computations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/online-feature.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/online-feature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/rfft.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/rfft.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-log.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-online-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-online-feature.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-rfft.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.637781 kaldi-native-fbank-1.9/kaldi-native-fbank/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.641781 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-fbank.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-window.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-window.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/kaldi-native-fbank.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/kaldi-native-fbank.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/mel-computations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/mel-computations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/online-feature.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/online-feature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.641781 kaldi-native-fbank-1.9/kaldi-native-fbank/python/kaldi_native_fbank/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/kaldi_native_fbank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.641781 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5202 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_fbank_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2787 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_frame_extraction_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2214 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_mel_bank_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_online_fbank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 03:30:38.641781 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-05 03:30:38.000000 kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 03:30:38.645781 kaldi-native-fbank-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-01-05 03:30:27.000000 kaldi-native-fbank-1.9/setup.py
```

### Comparing `kaldi-native-fbank-1.18.0/LICENSE` & `kaldi-native-fbank-1.9/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 
+                                 Legal Notices
+
+   NOTE (this is not from the Apache License): The copyright model is that
+   authors (or their employers, if noted in individual files) own their
+   individual contributions. The authors' contributions can be discerned
+   from the git history.
+
+ -------------------------------------------------------------------------
+
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
```

### Comparing `kaldi-native-fbank-1.18.0/README.md` & `kaldi-native-fbank-1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 # Introduction
 
 Kaldi-compatible online fbank feature extractor without external dependencies.
 
-Tested on the following architectures and operating systems:
-
-  - Linux
-  - macOS
-  - Windows
-  - Android
-  - x86
-  - arm
-  - aarch64
-
 # Usage
 
-See the following CMake-based speech recognition (i.e., text-to-speech) projects
-for its usage:
+See the following CMake-based projects for its usage:
 
 - <https://github.com/k2-fsa/sherpa-ncnn>
   - Specifically, please have a look at <https://github.com/k2-fsa/sherpa-ncnn/blob/master/sherpa-ncnn/csrc/features.h>
 - <https://github.com/k2-fsa/sherpa-onnx>
 
-They use `kaldi-native-fbank` to compute fbank features for **real-time**
-speech recognition.
+They use kaldi-native-fbank to compute fbank features for speech recognition.
 
 # Python APIs
 
 First, please install `kaldi-native-fbank` by
 
 ```bash
 git clone https://github.com/csukuangfj/kaldi-native-fbank
```

### Comparing `kaldi-native-fbank-1.18.0/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `kaldi-native-fbank-1.9/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/cmake/Modules/FetchContent.cmake` & `kaldi-native-fbank-1.9/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/cmake/__pycache__/cmake_extension.cpython-310.pyc` & `kaldi-native-fbank-1.9/cmake/__pycache__/cmake_extension.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Aug  6 08:23:20 2023 UTC, .py size: 3964 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,222 +1,223 @@
-00000000: 6f0d 0d0a 0000 0000 7858 cf64 7c0f 0000  o.......xX.d|...
+00000000: 550d 0d0a 0000 0000 5344 b663 7c0f 0000  U.......SD.c|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6401 6c07 5a07 6400 6403 6c08  ..d.d.l.Z.d.d.l.
 00000070: 6d09 5a09 0100 6404 6405 8400 5a0a 6406  m.Z...d.d...Z.d.
-00000080: 6407 8400 5a0b 6408 6409 8400 5a0c 7a10  d...Z.d.d...Z.z.
+00000080: 6407 8400 5a0b 6408 6409 8400 5a0c 7a20  d...Z.d.d...Z.z 
 00000090: 6400 640a 6c0d 6d0e 5a0f 0100 4700 640b  d.d.l.m.Z...G.d.
-000000a0: 640c 8400 640c 650f 8303 5a0e 5700 6e0b  d...d.e...Z.W.n.
-000000b0: 0400 6510 794b 0100 0100 0100 6401 5a0e  ..e.yK......d.Z.
-000000c0: 5900 6e01 7700 640d 6507 6a11 6602 640e  Y.n.w.d.e.j.f.d.
-000000d0: 640f 8404 5a12 4700 6410 6411 8400 6411  d...Z.G.d.d...d.
-000000e0: 6509 8303 5a13 6401 5300 2912 e900 0000  e...Z.d.S.).....
-000000f0: 004e 2901 da04 5061 7468 2901 da09 6275  .N)...Path)...bu
-00000100: 696c 645f 6578 7463 0000 0000 0000 0000  ild_extc........
-00000110: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00000120: 7316 0000 0074 006a 01a0 0264 0164 00a1  s....t.j...d.d..
-00000130: 027d 007c 0064 0075 0153 0029 024e da1e  .}.|.d.u.S.).N..
-00000140: 4b41 4c44 495f 4e41 5449 5645 5f46 4241  KALDI_NATIVE_FBA
-00000150: 4e4b 5f49 535f 464f 525f 5059 5049 2903  NK_IS_FOR_PYPI).
-00000160: da02 6f73 da07 656e 7669 726f 6eda 0367  ..os..environ..g
-00000170: 6574 2901 da03 616e 73a9 0072 0900 0000  et)...ans..r....
-00000180: fa50 2f68 6f6d 652f 7275 6e6e 6572 2f77  .P/home/runner/w
-00000190: 6f72 6b2f 6b61 6c64 692d 6e61 7469 7665  ork/kaldi-native
-000001a0: 2d66 6261 6e6b 2f6b 616c 6469 2d6e 6174  -fbank/kaldi-nat
-000001b0: 6976 652d 6662 616e 6b2f 636d 616b 652f  ive-fbank/cmake/
-000001c0: 636d 616b 655f 6578 7465 6e73 696f 6e2e  cmake_extension.
-000001d0: 7079 da0b 6973 5f66 6f72 5f70 7970 690e  py..is_for_pypi.
-000001e0: 0000 0073 0400 0000 0e01 0801 720b 0000  ...s........r...
-000001f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000200: 0000 0200 0000 4300 0000 f30c 0000 0074  ......C........t
-00000210: 00a0 01a1 0064 016b 0253 0029 024e da06  .....d.k.S.).N..
-00000220: 4461 7277 696e a902 da08 706c 6174 666f  Darwin....platfo
-00000230: 726d da06 7379 7374 656d 7209 0000 0072  rm..systemr....r
-00000240: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
-00000250: 6973 5f6d 6163 6f73 1300 0000 f302 0000  is_macos........
-00000260: 000c 0172 1100 0000 6300 0000 0000 0000  ...r....c.......
-00000270: 0000 0000 0000 0000 0002 0000 0043 0000  .............C..
-00000280: 0072 0c00 0000 2902 4eda 0757 696e 646f  .r....).N..Windo
-00000290: 7773 720e 0000 0072 0900 0000 7209 0000  wsr....r....r...
-000002a0: 0072 0900 0000 720a 0000 00da 0a69 735f  .r....r......is_
-000002b0: 7769 6e64 6f77 7317 0000 0072 1200 0000  windows....r....
-000002c0: 7214 0000 0029 01da 0b62 6469 7374 5f77  r....)...bdist_w
-000002d0: 6865 656c 6300 0000 0000 0000 0000 0000  heelc...........
-000002e0: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
-000002f0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-00000300: 5a03 6403 5300 2904 7215 0000 0063 0100  Z.d.S.).r....c..
-00000310: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00000320: 0000 4300 0000 732a 0000 0074 00a0 017c  ..C...s*...t...|
-00000330: 00a1 0101 0074 0283 0072 1074 0383 0073  .....t...r.t...s
-00000340: 1064 017c 005f 0464 0053 0064 027c 005f  .d.|._.d.S.d.|._
-00000350: 0464 0053 0029 034e 5446 2905 da0c 5f62  .d.S.).NTF)..._b
-00000360: 6469 7374 5f77 6865 656c da10 6669 6e61  dist_wheel..fina
-00000370: 6c69 7a65 5f6f 7074 696f 6e73 720b 0000  lize_optionsr...
-00000380: 0072 1100 0000 da0c 726f 6f74 5f69 735f  .r......root_is_
-00000390: 7075 7265 2901 da04 7365 6c66 7209 0000  pure)...selfr...
-000003a0: 0072 0900 0000 720a 0000 0072 1700 0000  .r....r....r....
-000003b0: 1f00 0000 7308 0000 000a 010c 030a 010a  ....s...........
-000003c0: 047a 1c62 6469 7374 5f77 6865 656c 2e66  .z.bdist_wheel.f
-000003d0: 696e 616c 697a 655f 6f70 7469 6f6e 734e  inalize_optionsN
-000003e0: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000003f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000400: 6e61 6d65 5f5f 7217 0000 0072 0900 0000  name__r....r....
-00000410: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00000420: 1500 0000 1e00 0000 7304 0000 0008 000c  ........s.......
-00000430: 0172 1500 0000 da06 7265 7475 726e 6301  .r......returnc.
-00000440: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00000450: 0000 004f 0000 0073 2600 0000 6401 7c02  ...O...s&...d.|.
-00000460: 6402 3c00 6700 7d03 7400 6a01 7c00 7c03  d.<.g.}.t.j.|.|.
-00000470: 6702 7c01 a201 5200 6900 7c02 a401 8e01  g.|...R.i.|.....
-00000480: 5300 2903 4e7a 0363 2b2b da08 6c61 6e67  S.).Nz.c++..lang
-00000490: 7561 6765 2902 da0a 7365 7475 7074 6f6f  uage)...setuptoo
-000004a0: 6c73 da09 4578 7465 6e73 696f 6e29 04da  ls..Extension)..
-000004b0: 046e 616d 65da 0461 7267 73da 066b 7761  .name..args..kwa
-000004c0: 7267 73da 0773 6f75 7263 6573 7209 0000  rgs..sourcesr...
-000004d0: 0072 0900 0000 720a 0000 00da 0f63 6d61  .r....r......cma
-000004e0: 6b65 5f65 7874 656e 7369 6f6e 2f00 0000  ke_extension/...
-000004f0: 7306 0000 0008 0104 011a 0172 2500 0000  s..........r%...
-00000500: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000510: 0003 0000 0040 0000 0073 1e00 0000 6500  .....@...s....e.
-00000520: 5a01 6400 5a02 6401 6503 6a04 6a05 6602  Z.d.Z.d.e.j.j.f.
-00000530: 6402 6403 8404 5a06 6404 5300 2905 da0e  d.d...Z.d.S.)...
-00000540: 4275 696c 6445 7874 656e 7369 6f6e da03  BuildExtension..
-00000550: 6578 7463 0200 0000 0000 0000 0000 0000  extc............
-00000560: 0a00 0000 0900 0000 4300 0000 73b4 0100  ........C...s...
-00000570: 0074 006a 017c 006a 0264 0164 028d 0201  .t.j.|.j.d.d....
-00000580: 0074 006a 017c 006a 0364 0164 028d 0201  .t.j.|.j.d.d....
-00000590: 0074 047c 006a 0383 01a0 05a1 0064 031b  .t.|.j.......d..
-000005a0: 007d 0274 0474 0683 016a 076a 07a0 05a1  .}.t.t...j.j....
-000005b0: 007d 0374 006a 08a0 0964 0464 05a1 027d  .}.t.j...d.d...}
-000005c0: 0474 006a 08a0 0964 0664 05a1 027d 0574  .t.j...d.d...}.t
-000005d0: 006a 08a0 0964 0764 05a1 027d 067c 0464  .j...d.d...}.|.d
-000005e0: 056b 0272 3c64 087d 0464 097c 029b 0064  .k.r<d.}.d.|...d
-000005f0: 0a9d 037d 077c 0764 0b37 007d 0764 0c7c  ...}.|.d.7.}.d.|
-00000600: 0476 0172 5a74 0a64 0d74 0b6a 0c9b 009d  .v.rZt.d.t.j....
-00000610: 0283 0101 007c 0464 0e74 0b6a 0c9b 009d  .....|.d.t.j....
-00000620: 0237 007d 047c 047c 0737 007d 0474 0d83  .7.}.|.|.7.}.t..
-00000630: 0072 a464 0f7c 049b 0064 107c 006a 029b  .r.d.|...d.|.j..
-00000640: 0064 117c 039b 0064 127c 006a 029b 0064  .d.|...d.|.j...d
-00000650: 139d 097d 0874 0a64 147c 089b 009d 0283  ...}.t.d.|......
-00000660: 0101 0074 00a0 0e64 157c 049b 0064 107c  ...t...d.|...d.|
-00000670: 006a 029b 0064 117c 039b 009d 06a1 017d  .j...d.|.......}
-00000680: 097c 0964 166b 0372 9074 0f64 1783 0182  .|.d.k.r.t.d....
-00000690: 0174 00a0 0e64 187c 006a 029b 0064 199d  .t...d.|.j...d..
-000006a0: 03a1 017d 097c 0964 166b 0372 a274 0f64  ...}.|.d.k.r.t.d
-000006b0: 1a83 0182 0164 0053 007c 0564 056b 0272  .....d.S.|.d.k.r
-000006c0: b47c 0664 056b 0272 b474 0a64 1b83 0101  .|.d.k.r.t.d....
-000006d0: 0074 0a64 1c83 0101 0064 1d7c 006a 029b  .t.d.....d.|.j..
-000006e0: 0064 1e7c 049b 0064 0a7c 039b 0064 1f7c  .d.|...d.|...d.|
-000006f0: 059b 0064 209d 097d 0874 0a64 147c 089b  ...d ..}.t.d.|..
-00000700: 009d 0283 0101 0074 00a0 0e7c 08a1 017d  .......t...|...}
-00000710: 097c 0964 166b 0372 d874 0f64 2183 0182  .|.d.k.r.t.d!...
-00000720: 0164 0053 0029 224e 5429 01da 0865 7869  .d.S.)"NT)...exi
-00000730: 7374 5f6f 6bda 126b 616c 6469 5f6e 6174  st_ok..kaldi_nat
-00000740: 6976 655f 6662 616e 6bda 1d4b 414c 4449  ive_fbank..KALDI
-00000750: 5f4e 4154 4956 455f 4642 414e 4b5f 434d  _NATIVE_FBANK_CM
-00000760: 414b 455f 4152 4753 da00 da1c 4b41 4c44  AKE_ARGS....KALD
-00000770: 495f 4e41 5449 5645 5f46 4241 4e4b 5f4d  I_NATIVE_FBANK_M
-00000780: 414b 455f 4152 4753 da09 4d41 4b45 464c  AKE_ARGS..MAKEFL
-00000790: 4147 537a 1a2d 4443 4d41 4b45 5f42 5549  AGSz.-DCMAKE_BUI
-000007a0: 4c44 5f54 5950 453d 5265 6c65 6173 657a  LD_TYPE=Releasez
-000007b0: 1820 2d44 434d 414b 455f 494e 5354 414c  . -DCMAKE_INSTAL
-000007c0: 4c5f 5052 4546 4958 3dfa 0120 7a26 202d  L_PREFIX=.. z& -
-000007d0: 444b 414c 4449 5f4e 4154 4956 455f 4642  DKALDI_NATIVE_FB
-000007e0: 414e 4b5f 4255 494c 445f 5445 5354 533d  ANK_BUILD_TESTS=
-000007f0: 4f46 4620 da11 5059 5448 4f4e 5f45 5845  OFF ..PYTHON_EXE
-00000800: 4355 5441 424c 457a 1d53 6574 7469 6e67  CUTABLEz.Setting
-00000810: 2050 5954 484f 4e5f 4558 4543 5554 4142   PYTHON_EXECUTAB
-00000820: 4c45 2074 6f20 7a15 202d 4450 5954 484f  LE to z. -DPYTHO
-00000830: 4e5f 4558 4543 5554 4142 4c45 3d7a 170a  N_EXECUTABLE=z..
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 636d 616b 6520 7a04 202d 4220 7a04 202d  cmake z. -B z. -
-00000860: 5320 7a1f 0a20 2020 2020 2020 2020 2020  S z..           
-00000870: 2020 2020 2063 6d61 6b65 202d 2d62 7569       cmake --bui
-00000880: 6c64 207a 3520 2d2d 7461 7267 6574 2069  ld z5 --target i
-00000890: 6e73 7461 6c6c 202d 2d63 6f6e 6669 6720  nstall --config 
-000008a0: 5265 6c65 6173 6520 2d2d 202d 6d0a 2020  Release -- -m.  
-000008b0: 2020 2020 2020 2020 2020 7a12 6275 696c            z.buil
-000008c0: 6420 636f 6d6d 616e 6420 6973 3a0a 7a06  d command is:.z.
-000008d0: 636d 616b 6520 7201 0000 007a 2646 6169  cmake r....z&Fai
-000008e0: 6c65 6420 746f 2063 6f6e 6669 6775 7265  led to configure
-000008f0: 206b 616c 6469 5f6e 6174 6976 655f 6662   kaldi_native_fb
-00000900: 616e 6b7a 0e63 6d61 6b65 202d 2d62 7569  ankz.cmake --bui
-00000910: 6c64 207a 2820 2d2d 7461 7267 6574 2069  ld z( --target i
-00000920: 6e73 7461 6c6c 202d 2d63 6f6e 6669 6720  nstall --config 
-00000930: 5265 6c65 6173 6520 2d2d 202d 6d7a 2446  Release -- -mz$F
-00000940: 6169 6c65 6420 746f 2069 6e73 7461 6c6c  ailed to install
-00000950: 206b 616c 6469 5f6e 6174 6976 655f 6662   kaldi_native_fb
-00000960: 616e 6b7a 1a46 6f72 2066 6173 7420 636f  ankz.For fast co
-00000970: 6d70 696c 6174 696f 6e2c 2072 756e 3a7a  mpilation, run:z
-00000980: 4165 7870 6f72 7420 4b41 4c44 495f 4e41  Aexport KALDI_NA
-00000990: 5449 5645 5f46 4241 4e4b 5f4d 414b 455f  TIVE_FBANK_MAKE_
-000009a0: 4152 4753 3d22 2d6a 223b 2070 7974 686f  ARGS="-j"; pytho
-000009b0: 6e20 7365 7475 702e 7079 2069 6e73 7461  n setup.py insta
-000009c0: 6c6c 7a14 0a20 2020 2020 2020 2020 2020  llz..           
-000009d0: 2020 2020 2063 6420 7a18 0a0a 2020 2020       cd z...    
-000009e0: 2020 2020 2020 2020 2020 2020 636d 616b              cmak
-000009f0: 6520 7a17 0a0a 2020 2020 2020 2020 2020  e z...          
-00000a00: 2020 2020 2020 6d61 6b65 207a 1520 696e        make z. in
-00000a10: 7374 616c 6c0a 2020 2020 2020 2020 2020  stall.          
-00000a20: 2020 7abc 0a42 7569 6c64 206b 616c 6469    z..Build kaldi
-00000a30: 2d6e 6174 6976 652d 6662 616e 6b20 6661  -native-fbank fa
-00000a40: 696c 6564 2e20 506c 6561 7365 2063 6865  iled. Please che
-00000a50: 636b 2074 6865 2065 7272 6f72 206d 6573  ck the error mes
-00000a60: 7361 6765 2e0a 596f 7520 6361 6e20 6173  sage..You can as
-00000a70: 6b20 666f 7220 6865 6c70 2062 7920 6372  k for help by cr
-00000a80: 6561 7469 6e67 2061 6e20 6973 7375 6520  eating an issue 
-00000a90: 6f6e 2047 6974 4875 622e 0a0a 436c 6963  on GitHub...Clic
-00000aa0: 6b3a 0a09 6874 7470 733a 2f2f 6769 7468  k:..https://gith
-00000ab0: 7562 2e63 6f6d 2f63 7375 6b75 616e 6766  ub.com/csukuangf
-00000ac0: 6a2f 6b61 6c64 692d 6e61 7469 7665 2d66  j/kaldi-native-f
-00000ad0: 6261 6e6b 2f69 7373 7565 732f 6e65 770a  bank/issues/new.
-00000ae0: 2910 7205 0000 00da 086d 616b 6564 6972  ).r......makedir
-00000af0: 73da 0a62 7569 6c64 5f74 656d 70da 0962  s..build_temp..b
-00000b00: 7569 6c64 5f6c 6962 7202 0000 00da 0772  uild_libr......r
-00000b10: 6573 6f6c 7665 da08 5f5f 6669 6c65 5f5f  esolve..__file__
-00000b20: da06 7061 7265 6e74 7206 0000 0072 0700  ..parentr....r..
-00000b30: 0000 da05 7072 696e 74da 0373 7973 da0a  ....print..sys..
-00000b40: 6578 6563 7574 6162 6c65 7214 0000 0072  executabler....r
-00000b50: 1000 0000 da09 4578 6365 7074 696f 6e29  ......Exception)
-00000b60: 0a72 1900 0000 7227 0000 00da 0b69 6e73  .r....r'.....ins
-00000b70: 7461 6c6c 5f64 6972 da16 6b61 6c64 695f  tall_dir..kaldi_
-00000b80: 6e61 7469 7665 5f66 6261 6e6b 5f64 6972  native_fbank_dir
-00000b90: da0a 636d 616b 655f 6172 6773 da09 6d61  ..cmake_args..ma
-00000ba0: 6b65 5f61 7267 73da 1073 7973 7465 6d5f  ke_args..system_
-00000bb0: 6d61 6b65 5f61 7267 73da 1065 7874 7261  make_args..extra
-00000bc0: 5f63 6d61 6b65 5f61 7267 73da 0962 7569  _cmake_args..bui
-00000bd0: 6c64 5f63 6d64 da03 7265 7472 0900 0000  ld_cmd..retr....
-00000be0: 7209 0000 0072 0a00 0000 da0f 6275 696c  r....r......buil
-00000bf0: 645f 6578 7465 6e73 696f 6e36 0000 0073  d_extension6...s
-00000c00: 7400 0000 1002 1003 1202 1002 0e02 0e01  t...............
-00000c10: 0e01 0802 0401 0c02 0801 0802 1001 1001  ................
-00000c20: 0802 0602 0201 0201 04ff 0401 04ff 0201  ................
-00000c30: 04ff 0402 08fe 0e04 0401 1601 04ff 0803  ................
-00000c40: 0801 0402 0c01 04ff 0803 0801 04ff 1003  ................
-00000c50: 0801 0201 0201 04ff 0204 0401 04ff 0203  ................
-00000c60: 04fd 0203 04fd 0205 08fb 0e07 0a02 0801  ................
-00000c70: 0201 0201 04ff 04ff 7a1e 4275 696c 6445  ........z.BuildE
-00000c80: 7874 656e 7369 6f6e 2e62 7569 6c64 5f65  xtension.build_e
-00000c90: 7874 656e 7369 6f6e 4e29 0772 1a00 0000  xtensionN).r....
-00000ca0: 721b 0000 0072 1c00 0000 721f 0000 00da  r....r....r.....
-00000cb0: 0965 7874 656e 7369 6f6e 7220 0000 0072  .extensionr ...r
-00000cc0: 4200 0000 7209 0000 0072 0900 0000 7209  B...r....r....r.
-00000cd0: 0000 0072 0a00 0000 7226 0000 0035 0000  ...r....r&...5..
-00000ce0: 0073 0400 0000 0800 1601 7226 0000 0029  .s........r&...)
-00000cf0: 14da 0467 6c6f 6272 0500 0000 720f 0000  ...globr....r...
-00000d00: 00da 0673 6875 7469 6c72 3700 0000 da07  ...shutilr7.....
-00000d10: 7061 7468 6c69 6272 0200 0000 721f 0000  pathlibr....r...
-00000d20: 00da 1c73 6574 7570 746f 6f6c 732e 636f  ...setuptools.co
-00000d30: 6d6d 616e 642e 6275 696c 645f 6578 7472  mmand.build_extr
-00000d40: 0300 0000 720b 0000 0072 1100 0000 7214  ....r....r....r.
-00000d50: 0000 00da 1177 6865 656c 2e62 6469 7374  .....wheel.bdist
-00000d60: 5f77 6865 656c 7215 0000 0072 1600 0000  _wheelr....r....
-00000d70: da0b 496d 706f 7274 4572 726f 7272 2000  ..ImportErrorr .
-00000d80: 0000 7225 0000 0072 2600 0000 7209 0000  ..r%...r&...r...
-00000d90: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000da0: da08 3c6d 6f64 756c 653e 0100 0000 7326  ..<module>....s&
-00000db0: 0000 0008 0208 0108 0108 0108 010c 0108  ................
-00000dc0: 020c 0108 0308 0508 0402 040c 0114 020c  ................
-00000dd0: 0d08 0102 ff10 0414 06                   .........
+000000a0: 640c 8400 640c 650f 8303 5a0e 5700 6e18  d...d.e...Z.W.n.
+000000b0: 0400 6510 6b0a 7298 0100 0100 0100 6401  ..e.k.r.......d.
+000000c0: 5a0e 5900 6e02 5800 6507 6a11 640d 9c01  Z.Y.n.X.e.j.d...
+000000d0: 640e 640f 8404 5a12 4700 6410 6411 8400  d.d...Z.G.d.d...
+000000e0: 6411 6509 8303 5a13 6401 5300 2912 e900  d.e...Z.d.S.)...
+000000f0: 0000 004e 2901 da04 5061 7468 2901 da09  ...N)...Path)...
+00000100: 6275 696c 645f 6578 7463 0000 0000 0000  build_extc......
+00000110: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000120: 0000 7316 0000 0074 006a 01a0 0264 0164  ..s....t.j...d.d
+00000130: 00a1 027d 007c 0064 006b 0953 0029 024e  ...}.|.d.k.S.).N
+00000140: 5a1e 4b41 4c44 495f 4e41 5449 5645 5f46  Z.KALDI_NATIVE_F
+00000150: 4241 4e4b 5f49 535f 464f 525f 5059 5049  BANK_IS_FOR_PYPI
+00000160: 2903 da02 6f73 da07 656e 7669 726f 6eda  )...os..environ.
+00000170: 0367 6574 2901 5a03 616e 73a9 0072 0700  .get).Z.ans..r..
+00000180: 0000 fa50 2f68 6f6d 652f 7275 6e6e 6572  ...P/home/runner
+00000190: 2f77 6f72 6b2f 6b61 6c64 692d 6e61 7469  /work/kaldi-nati
+000001a0: 7665 2d66 6261 6e6b 2f6b 616c 6469 2d6e  ve-fbank/kaldi-n
+000001b0: 6174 6976 652d 6662 616e 6b2f 636d 616b  ative-fbank/cmak
+000001c0: 652f 636d 616b 655f 6578 7465 6e73 696f  e/cmake_extensio
+000001d0: 6e2e 7079 da0b 6973 5f66 6f72 5f70 7970  n.py..is_for_pyp
+000001e0: 690e 0000 0073 0400 0000 0001 0e01 7209  i....s........r.
+000001f0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000200: 0000 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+00000210: 0074 00a0 01a1 0064 016b 0253 0029 024e  .t.....d.k.S.).N
+00000220: da06 4461 7277 696e a902 da08 706c 6174  ..Darwin....plat
+00000230: 666f 726d da06 7379 7374 656d 7207 0000  form..systemr...
+00000240: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000250: da08 6973 5f6d 6163 6f73 1300 0000 7302  ..is_macos....s.
+00000260: 0000 0000 0172 0e00 0000 6300 0000 0000  .....r....c.....
+00000270: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00000280: 0000 0073 0c00 0000 7400 a001 a100 6401  ...s....t.....d.
+00000290: 6b02 5300 2902 4eda 0757 696e 646f 7773  k.S.).N..Windows
+000002a0: 720b 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
+000002b0: 0700 0000 7208 0000 00da 0a69 735f 7769  ....r......is_wi
+000002c0: 6e64 6f77 7317 0000 0073 0200 0000 0001  ndows....s......
+000002d0: 7210 0000 0029 01da 0b62 6469 7374 5f77  r....)...bdist_w
+000002e0: 6865 656c 6300 0000 0000 0000 0000 0000  heelc...........
+000002f0: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
+00000300: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00000310: 5a03 6403 5300 2904 7211 0000 0063 0100  Z.d.S.).r....c..
+00000320: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000330: 0000 4300 0000 7328 0000 0074 00a0 017c  ..C...s(...t...|
+00000340: 00a1 0101 0074 0283 0072 1e74 0383 0073  .....t...r.t...s
+00000350: 1e64 017c 005f 046e 0664 027c 005f 0464  .d.|._.n.d.|._.d
+00000360: 0053 0029 034e 5446 2905 da0c 5f62 6469  .S.).NTF)..._bdi
+00000370: 7374 5f77 6865 656c da10 6669 6e61 6c69  st_wheel..finali
+00000380: 7a65 5f6f 7074 696f 6e73 7209 0000 0072  ze_optionsr....r
+00000390: 0e00 0000 5a0c 726f 6f74 5f69 735f 7075  ....Z.root_is_pu
+000003a0: 7265 2901 da04 7365 6c66 7207 0000 0072  re)...selfr....r
+000003b0: 0700 0000 7208 0000 0072 1300 0000 1f00  ....r....r......
+000003c0: 0000 7308 0000 0000 010a 030c 0108 047a  ..s............z
+000003d0: 1c62 6469 7374 5f77 6865 656c 2e66 696e  .bdist_wheel.fin
+000003e0: 616c 697a 655f 6f70 7469 6f6e 734e 2904  alize_optionsN).
+000003f0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000400: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000410: 6d65 5f5f 7213 0000 0072 0700 0000 7207  me__r....r....r.
+00000420: 0000 0072 0700 0000 7208 0000 0072 1100  ...r....r....r..
+00000430: 0000 1e00 0000 7302 0000 0008 0172 1100  ......s......r..
+00000440: 0000 2901 da06 7265 7475 726e 6301 0000  ..)...returnc...
+00000450: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000460: 004f 0000 0073 2000 0000 6401 7c02 6402  .O...s ...d.|.d.
+00000470: 3c00 6700 7d03 7400 6a01 7c00 7c03 6602  <.g.}.t.j.|.|.f.
+00000480: 7c01 9e02 7c02 8e01 5300 2903 4e7a 0363  |...|...S.).Nz.c
+00000490: 2b2b da08 6c61 6e67 7561 6765 2902 da0a  ++..language)...
+000004a0: 7365 7475 7074 6f6f 6c73 da09 4578 7465  setuptools..Exte
+000004b0: 6e73 696f 6e29 04da 046e 616d 65da 0461  nsion)...name..a
+000004c0: 7267 73da 066b 7761 7267 73da 0773 6f75  rgs..kwargs..sou
+000004d0: 7263 6573 7207 0000 0072 0700 0000 7208  rcesr....r....r.
+000004e0: 0000 00da 0f63 6d61 6b65 5f65 7874 656e  .....cmake_exten
+000004f0: 7369 6f6e 2f00 0000 7306 0000 0000 0108  sion/...s.......
+00000500: 0104 0172 2000 0000 6300 0000 0000 0000  ...r ...c.......
+00000510: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000520: 0073 1e00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
+00000530: 6a04 6a05 6401 9c01 6402 6403 8404 5a06  j.j.d...d.d...Z.
+00000540: 6404 5300 2905 da0e 4275 696c 6445 7874  d.S.)...BuildExt
+00000550: 656e 7369 6f6e 2901 da03 6578 7463 0200  ension)...extc..
+00000560: 0000 0000 0000 0000 0000 0a00 0000 0900  ................
+00000570: 0000 4300 0000 73be 0100 0074 006a 017c  ..C...s....t.j.|
+00000580: 006a 0264 0164 028d 0201 0074 006a 017c  .j.d.d.....t.j.|
+00000590: 006a 0364 0164 028d 0201 0074 047c 006a  .j.d.d.....t.|.j
+000005a0: 0383 01a0 05a1 0064 031b 007d 0274 0474  .......d...}.t.t
+000005b0: 0683 016a 076a 07a0 05a1 007d 0374 006a  ...j.j.....}.t.j
+000005c0: 08a0 0964 0464 05a1 027d 0474 006a 08a0  ...d.d...}.t.j..
+000005d0: 0964 0664 05a1 027d 0574 006a 08a0 0964  .d.d...}.t.j...d
+000005e0: 0764 05a1 027d 067c 0464 056b 0272 7864  .d...}.|.d.k.rxd
+000005f0: 087d 0464 097c 029b 0064 0a9d 037d 077c  .}.d.|...d...}.|
+00000600: 0764 0b37 007d 0764 0c7c 046b 0772 b474  .d.7.}.d.|.k.r.t
+00000610: 0a64 0d74 0b6a 0c9b 009d 0283 0101 007c  .d.t.j.........|
+00000620: 0464 0e74 0b6a 0c9b 009d 0237 007d 047c  .d.t.j.....7.}.|
+00000630: 047c 0737 007d 0474 0d83 0090 0172 4c64  .|.7.}.t.....rLd
+00000640: 0f7c 049b 0064 107c 006a 029b 0064 117c  .|...d.|.j...d.|
+00000650: 039b 0064 127c 006a 029b 0064 139d 097d  ...d.|.j...d...}
+00000660: 0874 0a64 147c 089b 009d 0283 0101 0074  .t.d.|.........t
+00000670: 00a0 0e64 157c 049b 0064 107c 006a 029b  ...d.|...d.|.j..
+00000680: 0064 117c 039b 009d 06a1 017d 097c 0964  .d.|.......}.|.d
+00000690: 166b 0390 0172 2474 0f64 1783 0182 0174  .k...r$t.d.....t
+000006a0: 00a0 0e64 187c 006a 029b 0064 199d 03a1  ...d.|.j...d....
+000006b0: 017d 097c 0964 166b 0390 0172 ba74 0f64  .}.|.d.k...r.t.d
+000006c0: 1a83 0182 016e 6e7c 0564 056b 0290 0172  .....nn|.d.k...r
+000006d0: 707c 0664 056b 0290 0172 7074 0a64 1b83  p|.d.k...rpt.d..
+000006e0: 0101 0074 0a64 1c83 0101 0064 1d7c 006a  ...t.d.....d.|.j
+000006f0: 029b 0064 1e7c 049b 0064 0a7c 039b 0064  ...d.|...d.|...d
+00000700: 1f7c 059b 0064 209d 097d 0874 0a64 147c  .|...d ..}.t.d.|
+00000710: 089b 009d 0283 0101 0074 00a0 0e7c 08a1  .........t...|..
+00000720: 017d 097c 0964 166b 0390 0172 ba74 0f64  .}.|.d.k...r.t.d
+00000730: 2183 0182 0164 0053 0029 224e 5429 01da  !....d.S.)"NT)..
+00000740: 0865 7869 7374 5f6f 6bda 126b 616c 6469  .exist_ok..kaldi
+00000750: 5f6e 6174 6976 655f 6662 616e 6b5a 1d4b  _native_fbankZ.K
+00000760: 414c 4449 5f4e 4154 4956 455f 4642 414e  ALDI_NATIVE_FBAN
+00000770: 4b5f 434d 414b 455f 4152 4753 da00 5a1c  K_CMAKE_ARGS..Z.
+00000780: 4b41 4c44 495f 4e41 5449 5645 5f46 4241  KALDI_NATIVE_FBA
+00000790: 4e4b 5f4d 414b 455f 4152 4753 5a09 4d41  NK_MAKE_ARGSZ.MA
+000007a0: 4b45 464c 4147 537a 1a2d 4443 4d41 4b45  KEFLAGSz.-DCMAKE
+000007b0: 5f42 5549 4c44 5f54 5950 453d 5265 6c65  _BUILD_TYPE=Rele
+000007c0: 6173 657a 1820 2d44 434d 414b 455f 494e  asez. -DCMAKE_IN
+000007d0: 5354 414c 4c5f 5052 4546 4958 3dfa 0120  STALL_PREFIX=.. 
+000007e0: 7a26 202d 444b 414c 4449 5f4e 4154 4956  z& -DKALDI_NATIV
+000007f0: 455f 4642 414e 4b5f 4255 494c 445f 5445  E_FBANK_BUILD_TE
+00000800: 5354 533d 4f46 4620 5a11 5059 5448 4f4e  STS=OFF Z.PYTHON
+00000810: 5f45 5845 4355 5441 424c 457a 1d53 6574  _EXECUTABLEz.Set
+00000820: 7469 6e67 2050 5954 484f 4e5f 4558 4543  ting PYTHON_EXEC
+00000830: 5554 4142 4c45 2074 6f20 7a15 202d 4450  UTABLE to z. -DP
+00000840: 5954 484f 4e5f 4558 4543 5554 4142 4c45  YTHON_EXECUTABLE
+00000850: 3d7a 170a 2020 2020 2020 2020 2020 2020  =z..            
+00000860: 2020 2020 636d 616b 6520 7a04 202d 4220      cmake z. -B 
+00000870: 7a04 202d 5320 7a1f 0a20 2020 2020 2020  z. -S z..       
+00000880: 2020 2020 2020 2020 2063 6d61 6b65 202d           cmake -
+00000890: 2d62 7569 6c64 207a 3520 2d2d 7461 7267  -build z5 --targ
+000008a0: 6574 2069 6e73 7461 6c6c 202d 2d63 6f6e  et install --con
+000008b0: 6669 6720 5265 6c65 6173 6520 2d2d 202d  fig Release -- -
+000008c0: 6d0a 2020 2020 2020 2020 2020 2020 7a12  m.            z.
+000008d0: 6275 696c 6420 636f 6d6d 616e 6420 6973  build command is
+000008e0: 3a0a 7a06 636d 616b 6520 7201 0000 007a  :.z.cmake r....z
+000008f0: 2646 6169 6c65 6420 746f 2063 6f6e 6669  &Failed to confi
+00000900: 6775 7265 206b 616c 6469 5f6e 6174 6976  gure kaldi_nativ
+00000910: 655f 6662 616e 6b7a 0e63 6d61 6b65 202d  e_fbankz.cmake -
+00000920: 2d62 7569 6c64 207a 2820 2d2d 7461 7267  -build z( --targ
+00000930: 6574 2069 6e73 7461 6c6c 202d 2d63 6f6e  et install --con
+00000940: 6669 6720 5265 6c65 6173 6520 2d2d 202d  fig Release -- -
+00000950: 6d7a 2446 6169 6c65 6420 746f 2069 6e73  mz$Failed to ins
+00000960: 7461 6c6c 206b 616c 6469 5f6e 6174 6976  tall kaldi_nativ
+00000970: 655f 6662 616e 6b7a 1a46 6f72 2066 6173  e_fbankz.For fas
+00000980: 7420 636f 6d70 696c 6174 696f 6e2c 2072  t compilation, r
+00000990: 756e 3a7a 4165 7870 6f72 7420 4b41 4c44  un:zAexport KALD
+000009a0: 495f 4e41 5449 5645 5f46 4241 4e4b 5f4d  I_NATIVE_FBANK_M
+000009b0: 414b 455f 4152 4753 3d22 2d6a 223b 2070  AKE_ARGS="-j"; p
+000009c0: 7974 686f 6e20 7365 7475 702e 7079 2069  ython setup.py i
+000009d0: 6e73 7461 6c6c 7a14 0a20 2020 2020 2020  nstallz..       
+000009e0: 2020 2020 2020 2020 2063 6420 7a18 0a0a           cd z...
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 636d 616b 6520 7a17 0a0a 2020 2020 2020  cmake z...      
+00000a10: 2020 2020 2020 2020 2020 6d61 6b65 207a            make z
+00000a20: 1520 696e 7374 616c 6c0a 2020 2020 2020  . install.      
+00000a30: 2020 2020 2020 7abc 0a42 7569 6c64 206b        z..Build k
+00000a40: 616c 6469 2d6e 6174 6976 652d 6662 616e  aldi-native-fban
+00000a50: 6b20 6661 696c 6564 2e20 506c 6561 7365  k failed. Please
+00000a60: 2063 6865 636b 2074 6865 2065 7272 6f72   check the error
+00000a70: 206d 6573 7361 6765 2e0a 596f 7520 6361   message..You ca
+00000a80: 6e20 6173 6b20 666f 7220 6865 6c70 2062  n ask for help b
+00000a90: 7920 6372 6561 7469 6e67 2061 6e20 6973  y creating an is
+00000aa0: 7375 6520 6f6e 2047 6974 4875 622e 0a0a  sue on GitHub...
+00000ab0: 436c 6963 6b3a 0a09 6874 7470 733a 2f2f  Click:..https://
+00000ac0: 6769 7468 7562 2e63 6f6d 2f63 7375 6b75  github.com/csuku
+00000ad0: 616e 6766 6a2f 6b61 6c64 692d 6e61 7469  angfj/kaldi-nati
+00000ae0: 7665 2d66 6261 6e6b 2f69 7373 7565 732f  ve-fbank/issues/
+00000af0: 6e65 770a 2910 7204 0000 00da 086d 616b  new.).r......mak
+00000b00: 6564 6972 73da 0a62 7569 6c64 5f74 656d  edirs..build_tem
+00000b10: 705a 0962 7569 6c64 5f6c 6962 7202 0000  pZ.build_libr...
+00000b20: 00da 0772 6573 6f6c 7665 da08 5f5f 6669  ...resolve..__fi
+00000b30: 6c65 5f5f da06 7061 7265 6e74 7205 0000  le__..parentr...
+00000b40: 0072 0600 0000 da05 7072 696e 74da 0373  .r......print..s
+00000b50: 7973 da0a 6578 6563 7574 6162 6c65 7210  ys..executabler.
+00000b60: 0000 0072 0d00 0000 da09 4578 6365 7074  ...r......Except
+00000b70: 696f 6e29 0a72 1400 0000 7222 0000 00da  ion).r....r"....
+00000b80: 0b69 6e73 7461 6c6c 5f64 6972 5a16 6b61  .install_dirZ.ka
+00000b90: 6c64 695f 6e61 7469 7665 5f66 6261 6e6b  ldi_native_fbank
+00000ba0: 5f64 6972 5a0a 636d 616b 655f 6172 6773  _dirZ.cmake_args
+00000bb0: 5a09 6d61 6b65 5f61 7267 735a 1073 7973  Z.make_argsZ.sys
+00000bc0: 7465 6d5f 6d61 6b65 5f61 7267 735a 1065  tem_make_argsZ.e
+00000bd0: 7874 7261 5f63 6d61 6b65 5f61 7267 735a  xtra_cmake_argsZ
+00000be0: 0962 7569 6c64 5f63 6d64 da03 7265 7472  .build_cmd..retr
+00000bf0: 0700 0000 7207 0000 0072 0800 0000 da0f  ....r....r......
+00000c00: 6275 696c 645f 6578 7465 6e73 696f 6e36  build_extension6
+00000c10: 0000 0073 7000 0000 0002 1003 1002 1202  ...sp...........
+00000c20: 1002 0e01 0e01 0e02 0801 0402 0c01 0802  ................
+00000c30: 0801 1001 1002 0802 0801 0201 02ff 0401  ................
+00000c40: 04ff 0401 02ff 0401 04ff 0804 0e01 0401  ................
+00000c50: 16ff 0403 0a01 0802 0401 0cff 0403 0a01  ................
+00000c60: 0a02 1401 0801 0201 02ff 0404 0201 04ff  ................
+00000c70: 0403 02fd 0403 02fd 0405 02fb 0807 0e02  ................
+00000c80: 0a01 0a01 0201 02ff 7a1e 4275 696c 6445  ........z.BuildE
+00000c90: 7874 656e 7369 6f6e 2e62 7569 6c64 5f65  xtension.build_e
+00000ca0: 7874 656e 7369 6f6e 4e29 0772 1500 0000  xtensionN).r....
+00000cb0: 7216 0000 0072 1700 0000 721a 0000 00da  r....r....r.....
+00000cc0: 0965 7874 656e 7369 6f6e 721b 0000 0072  .extensionr....r
+00000cd0: 3200 0000 7207 0000 0072 0700 0000 7207  2...r....r....r.
+00000ce0: 0000 0072 0800 0000 7221 0000 0035 0000  ...r....r!...5..
+00000cf0: 0073 0200 0000 0801 7221 0000 0029 14da  .s......r!...)..
+00000d00: 0467 6c6f 6272 0400 0000 720c 0000 00da  .globr....r.....
+00000d10: 0673 6875 7469 6c72 2d00 0000 da07 7061  .shutilr-.....pa
+00000d20: 7468 6c69 6272 0200 0000 721a 0000 005a  thlibr....r....Z
+00000d30: 1c73 6574 7570 746f 6f6c 732e 636f 6d6d  .setuptools.comm
+00000d40: 616e 642e 6275 696c 645f 6578 7472 0300  and.build_extr..
+00000d50: 0000 7209 0000 0072 0e00 0000 7210 0000  ..r....r....r...
+00000d60: 005a 1177 6865 656c 2e62 6469 7374 5f77  .Z.wheel.bdist_w
+00000d70: 6865 656c 7211 0000 0072 1200 0000 da0b  heelr....r......
+00000d80: 496d 706f 7274 4572 726f 7272 1b00 0000  ImportErrorr....
+00000d90: 7220 0000 0072 2100 0000 7207 0000 0072  r ...r!...r....r
+00000da0: 0700 0000 7207 0000 0072 0800 0000 da08  ....r....r......
+00000db0: 3c6d 6f64 756c 653e 0300 0000 7322 0000  <module>....s"..
+00000dc0: 0008 0108 0108 0108 0108 010c 0208 010c  ................
+00000dd0: 0308 0508 0408 0402 010c 0214 0d0e 010a  ................
+00000de0: 0310 06                                  ...
```

### Comparing `kaldi-native-fbank-1.18.0/cmake/cmake_extension.py` & `kaldi-native-fbank-1.9/cmake/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/cmake/googletest.cmake` & `kaldi-native-fbank-1.9/cmake/googletest.cmake`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 function(download_googltest)
   if(CMAKE_VERSION VERSION_LESS 3.11)
     list(APPEND CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/cmake/Modules)
   endif()
 
   include(FetchContent)
 
-  set(googletest_URL  "https://github.com/google/googletest/archive/refs/tags/v1.13.0.tar.gz")
-  set(googletest_URL2 "https://huggingface.co/csukuangfj/k2-cmake-deps/resolve/main/googletest-1.13.0.tar.gz")
-  set(googletest_HASH "SHA256=ad7fdba11ea011c1d925b3289cf4af2c66a352e18d4c7264392fead75e919363")
-
-  # If you don't have access to the Internet,
-  # please pre-download googletest
-  set(possible_file_locations
-    $ENV{HOME}/Downloads/googletest-1.13.0.tar.gz
-    ${PROJECT_SOURCE_DIR}/googletest-1.13.0.tar.gz
-    ${PROJECT_BINARY_DIR}/googletest-1.13.0.tar.gz
-    /tmp/googletest-1.13.0.tar.gz
-    /star-fj/fangjun/download/github/googletest-1.13.0.tar.gz
-  )
-
-  foreach(f IN LISTS possible_file_locations)
-    if(EXISTS ${f})
-      set(googletest_URL  "${f}")
-      file(TO_CMAKE_PATH "${googletest_URL}" googletest_URL)
-      set(googletest_URL2)
-      break()
-    endif()
-  endforeach()
+  set(googletest_URL  "https://github.com/google/googletest/archive/release-1.10.0.tar.gz")
+  set(googletest_HASH "SHA256=9dc9157a9a1551ec7a7e43daea9a694a0bb5fb8bec81235d8a1e6ef64c716dcb")
 
   set(BUILD_GMOCK ON CACHE BOOL "" FORCE)
   set(INSTALL_GTEST OFF CACHE BOOL "" FORCE)
   set(gtest_disable_pthreads ON CACHE BOOL "" FORCE)
   set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
 
   FetchContent_Declare(googletest
-    URL
-      ${googletest_URL}
-      ${googletest_URL2}
+    URL               ${googletest_URL}
     URL_HASH          ${googletest_HASH}
   )
 
   FetchContent_GetProperties(googletest)
   if(NOT googletest_POPULATED)
     message(STATUS "Downloading googletest from ${googletest_URL}")
     FetchContent_Populate(googletest)
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/CMakeLists.txt` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
   feature-fbank.cc
   feature-functions.cc
   feature-window.cc
   fftsg.c
   mel-computations.cc
   online-feature.cc
   rfft.cc
-  whisper-feature.cc
 )
 
 if(KALDI_NATIVE_FBANK_ENABLE_CHECK)
   list(APPEND sources log.cc)
 endif()
 
 add_library(kaldi-native-fbank-core ${sources})
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-fbank.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-fbank.cc`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,15 @@
  * limitations under the License.
  */
 
 // This file is copied/modified from kaldi/src/feat/feature-fbank.cc
 //
 #include "kaldi-native-fbank/csrc/feature-fbank.h"
 
-#include <algorithm>
 #include <cmath>
-#include <limits>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-functions.h"
 
 namespace knf {
 
 static void Sqrt(float *in_out, int32_t n) {
   for (int32_t i = 0; i != n; ++i) {
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-fbank.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-fbank.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 // This file is copied/modified from kaldi/src/feat/feature-fbank.h
 
 #ifndef KALDI_NATIVE_FBANK_CSRC_FEATURE_FBANK_H_
 #define KALDI_NATIVE_FBANK_CSRC_FEATURE_FBANK_H_
 
 #include <map>
-#include <string>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-window.h"
 #include "kaldi-native-fbank/csrc/mel-computations.h"
 #include "kaldi-native-fbank/csrc/rfft.h"
 
 namespace knf {
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-functions.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-functions.cc`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-functions.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-functions.h`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
  * distributed under the License is distributed on an "AS IS" BASIS,
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 // This file is copied/modified from kaldi/src/feat/feature-functions.h
-#ifndef KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H_
-#define KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H_
+#ifndef KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H
+#define KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H
 
 #include <vector>
 namespace knf {
 
 // ComputePowerSpectrum converts a complex FFT (as produced by the FFT
 // functions in csrc/rfft.h), and converts it into
 // a power spectrum.  If the complex FFT is a vector of size n (representing
@@ -31,8 +31,8 @@
 // energies of the fft bins from zero to the Nyquist frequency.  Contents of the
 // remaining (n/2) - 1 elements are undefined at output.
 
 void ComputePowerSpectrum(std::vector<float> *complex_fft);
 
 }  // namespace knf
 
-#endif  // KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H_
+#endif  // KALDI_NATIVE_FBANK_CSRC_FEATURE_FUNCTIONS_H
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-window.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-window.cc`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 //
 // Copyright (c)  2022  Xiaomi Corporation (authors: Fangjun Kuang)
 
 // This file is copied/modified from kaldi/src/feat/feature-window.cc
 
 #include "kaldi-native-fbank/csrc/feature-window.h"
 
-#include <algorithm>
 #include <cmath>
-#include <limits>
 #include <vector>
 
 #ifndef M_2PI
 #define M_2PI 6.283185307179586476925286766559005
 #endif
 
 namespace knf {
@@ -26,34 +24,26 @@
     : window_(opts.WindowSize()) {
   int32_t frame_length = opts.WindowSize();
   KNF_CHECK_GT(frame_length, 0);
 
   float *window_data = window_.data();
 
   double a = M_2PI / (frame_length - 1);
-  if (opts.window_type == "hann") {
-    // see https://pytorch.org/docs/stable/generated/torch.hann_window.html
-    // We assume periodic is true
-    a = M_2PI / frame_length;
-  }
-
   for (int32_t i = 0; i < frame_length; i++) {
     double i_fl = static_cast<double>(i);
     if (opts.window_type == "hanning") {
       window_data[i] = 0.5 - 0.5 * cos(a * i_fl);
     } else if (opts.window_type == "sine") {
       // when you are checking ws wikipedia, please
       // note that 0.5 * a = M_PI/(frame_length-1)
       window_data[i] = sin(0.5 * a * i_fl);
     } else if (opts.window_type == "hamming") {
       window_data[i] = 0.54 - 0.46 * cos(a * i_fl);
-    } else if (opts.window_type == "hann") {
-      window_data[i] = 0.50 - 0.50 * cos(a * i_fl);
-    } else if (opts.window_type == "povey") {
-      // like hamming but goes to zero at edges.
+    } else if (opts.window_type ==
+               "povey") {  // like hamming but goes to zero at edges.
       window_data[i] = pow(0.5 - 0.5 * cos(a * i_fl), 0.85);
     } else if (opts.window_type == "rectangular") {
       window_data[i] = 1.0;
     } else if (opts.window_type == "blackman") {
       window_data[i] = opts.blackman_coeff - 0.5 * cos(a * i_fl) +
                        (0.5 - opts.blackman_coeff) * cos(2 * a * i_fl);
     } else {
@@ -219,14 +209,17 @@
 }
 
 void ProcessWindow(const FrameExtractionOptions &opts,
                    const FeatureWindowFunction &window_function, float *window,
                    float *log_energy_pre_window /*= nullptr*/) {
   int32_t frame_length = opts.WindowSize();
 
+  // TODO(fangjun): Remove dither
+  KNF_CHECK_EQ(opts.dither, 0);
+
   if (opts.remove_dc_offset) {
     RemoveDcOffset(window, frame_length);
   }
 
   if (log_energy_pre_window != NULL) {
     float energy = std::max<float>(InnerProduct(window, window, frame_length),
                                    std::numeric_limits<float>::epsilon());
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/feature-window.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/feature-window.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // kaldi-native-fbank/csrc/feature-window.h
 //
 // Copyright (c)  2022  Xiaomi Corporation (authors: Fangjun Kuang)
 
 // This file is copied/modified from kaldi/src/feat/feature-window.h
 
-#ifndef KALDI_NATIVE_FBANK_CSRC_FEATURE_WINDOW_H_
-#define KALDI_NATIVE_FBANK_CSRC_FEATURE_WINDOW_H_
+#ifndef KALDI_NATIVE_FEAT_CSRC_FEATURE_WINDOW_H_
+#define KALDI_NATIVE_FEAT_CSRC_FEATURE_WINDOW_H_
 
 #include <sstream>
 #include <string>
 #include <vector>
 
 #include "kaldi-native-fbank/csrc/log.h"
 
@@ -31,25 +31,29 @@
   float samp_freq = 16000;
   float frame_shift_ms = 10.0f;   // in milliseconds.
   float frame_length_ms = 25.0f;  // in milliseconds.
   float dither = 1.0f;            // Amount of dithering, 0.0 means no dither.
   float preemph_coeff = 0.97f;    // Preemphasis coefficient.
   bool remove_dc_offset = true;   // Subtract mean of wave before FFT.
   std::string window_type = "povey";  // e.g. Hamming window
-  // May be "hamming", "rectangular", "povey", "hanning", "hann", "sine",
-  // "blackman".
+  // May be "hamming", "rectangular", "povey", "hanning", "sine", "blackman"
   // "povey" is a window I made to be similar to Hamming but to go to zero at
   // the edges, it's pow((0.5 - 0.5*cos(n/N*2*pi)), 0.85) I just don't think the
   // Hamming window makes sense as a windowing function.
   bool round_to_power_of_two = true;
   float blackman_coeff = 0.42f;
   bool snip_edges = true;
   // bool allow_downsample = false;
   // bool allow_upsample = false;
 
+  // Used for streaming feature extraction. It indicates the number
+  // of feature frames to keep in the recycling vector. -1 means to
+  // keep all feature frames.
+  int32_t max_feature_vectors = -1;
+
   int32_t WindowShift() const {
     return static_cast<int32_t>(samp_freq * 0.001f * frame_shift_ms);
   }
   int32_t WindowSize() const {
     return static_cast<int32_t>(samp_freq * 0.001f * frame_length_ms);
   }
   int32_t PaddedWindowSize() const {
@@ -67,14 +71,15 @@
     KNF_PRINT(remove_dc_offset);
     KNF_PRINT(window_type);
     KNF_PRINT(round_to_power_of_two);
     KNF_PRINT(blackman_coeff);
     KNF_PRINT(snip_edges);
     // KNF_PRINT(allow_downsample);
     // KNF_PRINT(allow_upsample);
+    KNF_PRINT(max_feature_vectors);
 #undef KNF_PRINT
     return os.str();
   }
 };
 
 std::ostream &operator<<(std::ostream &os, const FrameExtractionOptions &opts);
 
@@ -84,15 +89,14 @@
   explicit FeatureWindowFunction(const FrameExtractionOptions &opts);
   /**
    * @param wave Pointer to a 1-D array of shape [window_size].
    *             It is modified in-place: wave[i] = wave[i] * window_[i].
    * @param
    */
   void Apply(float *wave) const;
-  const std::vector<float> &GetWindow() const { return window_; }
 
  private:
   std::vector<float> window_;  // of size opts.WindowSize()
 };
 
 int64_t FirstSampleOfFrame(int32_t frame, const FrameExtractionOptions &opts);
 
@@ -103,15 +107,15 @@
 
       @param [in] num_samples  The number of samples in the wave file.
       @param [in] opts     The frame-extraction options class
 
       @param [in] flush   True if we are asserting that this number of samples
    is 'all there is', false if we expecting more data to possibly come in.  This
    only makes a difference to the answer
-   if opts.snip_edges== false.  For offline feature extraction you always want
+   if opts.snips_edges== false.  For offline feature extraction you always want
    flush == true.  In an online-decoding context, once you know (or decide) that
    no more data is coming in, you'd call it with flush == true at the end to
    flush out any remaining data.
 */
 int32_t NumFrames(int64_t num_samples, const FrameExtractionOptions &opts,
                   bool flush = true);
 
@@ -167,8 +171,8 @@
                    float *log_energy_pre_window = nullptr);
 
 // Compute the inner product of two vectors
 float InnerProduct(const float *a, const float *b, int32_t n);
 
 }  // namespace knf
 
-#endif  // KALDI_NATIVE_FBANK_CSRC_FEATURE_WINDOW_H_
+#endif  // KALDI_NATIVE_FEAT_CSRC_FEATURE_WINDOW_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/fftsg.c` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/fftsg.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 /* This file is copied from
- *
  * https://www.kurims.kyoto-u.ac.jp/~ooura/fft.html
- *
- * Copyright Takuya OOURA, 1996-2001
- *
- * You may use, copy, modify and distribute this code for any
- * purpose (include commercial use) and without fee. Please refer to
- * this package when you modify this code.
  */
 /*
 Fast Fourier/Cosine/Sine Transform
     dimension   :one
     data length :power of 2
     decimation  :frequency
     radix       :split-radix
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/log.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/log.cc`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,34 @@
  * Refer to
  * https://github.com/kaldi-asr/kaldi/blob/master/src/base/kaldi-error.cc
  */
 
 #include "kaldi-native-fbank/csrc/log.h"
 
 #ifdef KNF_HAVE_EXECINFO_H
-#include <execinfo.h>  // To get stack trace in error messages.
+#include <execinfo.h> // To get stack trace in error messages.
 #ifdef KNF_HAVE_CXXABI_H
-#include <cxxabi.h>  // For name demangling.
+#include <cxxabi.h> // For name demangling.
 // Useful to decode the stack trace, but only used if we have execinfo.h
-#endif  // KNF_HAVE_CXXABI_H
-#endif  // KNF_HAVE_EXECINFO_H
+#endif // KNF_HAVE_CXXABI_H
+#endif // KNF_HAVE_EXECINFO_H
 
 #include <stdlib.h>
 
 #include <ctime>
 #include <iomanip>
 #include <string>
 
 namespace knf {
 
 std::string GetDateTimeStr() {
   std::ostringstream os;
   std::time_t t = std::time(nullptr);
   std::tm tm = *std::localtime(&t);
-  os << std::put_time(&tm, "%F %T");  // yyyy-mm-dd hh:mm:ss
+  os << std::put_time(&tm, "%F %T"); // yyyy-mm-dd hh:mm:ss
   return os.str();
 }
 
 static bool LocateSymbolRange(const std::string &trace_name, std::size_t *begin,
                               std::size_t *end) {
   // Find the first '_' with leading ' ' or '('.
   *begin = std::string::npos;
@@ -68,15 +68,15 @@
   return *end != std::string::npos;
 }
 
 #ifdef KNF_HAVE_EXECINFO_H
 static std::string Demangle(const std::string &trace_name) {
 #ifndef KNF_HAVE_CXXABI_H
   return trace_name;
-#else   // KNF_HAVE_CXXABI_H
+#else  // KNF_HAVE_CXXABI_H
   // Try demangle the symbol. We are trying to support the following formats
   // produced by different platforms:
   //
   // Linux:
   //   ./kaldi-error-test(_ZN5kaldi13UnitTestErrorEv+0xb) [0x804965d]
   //
   // Mac:
@@ -93,50 +93,51 @@
   char *demangled_name = abi::__cxa_demangle(symbol.c_str(), 0, 0, &status);
   if (status == 0 && demangled_name != nullptr) {
     symbol = demangled_name;
     free(demangled_name);
   }
   return trace_name.substr(0, begin) + symbol +
          trace_name.substr(end, std::string::npos);
-#endif  // KNF_HAVE_CXXABI_H
+#endif // KNF_HAVE_CXXABI_H
 }
-#endif  // KNF_HAVE_EXECINFO_H
+#endif // KNF_HAVE_EXECINFO_H
 
 std::string GetStackTrace() {
   std::string ans;
 #ifdef KNF_HAVE_EXECINFO_H
   constexpr const std::size_t kMaxTraceSize = 50;
-  constexpr const std::size_t kMaxTracePrint = 50;  // Must be even.
-                                                    // Buffer for the trace.
+  constexpr const std::size_t kMaxTracePrint = 50; // Must be even.
+                                                   // Buffer for the trace.
   void *trace[kMaxTraceSize];
   // Get the trace.
   std::size_t size = backtrace(trace, kMaxTraceSize);
   // Get the trace symbols.
   char **trace_symbol = backtrace_symbols(trace, size);
-  if (trace_symbol == nullptr) return ans;
+  if (trace_symbol == nullptr)
+    return ans;
 
   // Compose a human-readable backtrace string.
   ans += "[ Stack-Trace: ]\n";
   if (size <= kMaxTracePrint) {
     for (std::size_t i = 0; i < size; ++i) {
       ans += Demangle(trace_symbol[i]) + "\n";
     }
-  } else {  // Print out first+last (e.g.) 5.
+  } else { // Print out first+last (e.g.) 5.
     for (std::size_t i = 0; i < kMaxTracePrint / 2; ++i) {
       ans += Demangle(trace_symbol[i]) + "\n";
     }
     ans += ".\n.\n.\n";
     for (std::size_t i = size - kMaxTracePrint / 2; i < size; ++i) {
       ans += Demangle(trace_symbol[i]) + "\n";
     }
     if (size == kMaxTraceSize)
-      ans += ".\n.\n.\n";  // Stack was too long, probably a bug.
+      ans += ".\n.\n.\n"; // Stack was too long, probably a bug.
   }
 
   // We must free the array of pointers allocated by backtrace_symbols(),
   // but not the strings themselves.
   free(trace_symbol);
-#endif  // KNF_HAVE_EXECINFO_H
+#endif // KNF_HAVE_EXECINFO_H
   return ans;
 }
 
-}  // namespace knf
+} // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/log.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/log.h`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/mel-computations.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/mel-computations.cc`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 // This file is copied/modified from kaldi/src/feat/mel-computations.cc
 
 #include "kaldi-native-fbank/csrc/mel-computations.h"
 
 #include <algorithm>
 #include <sstream>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-window.h"
 
 namespace knf {
 
 std::ostream &operator<<(std::ostream &os, const MelBanksOptions &opts) {
   os << opts.ToString();
@@ -153,28 +152,30 @@
        vtln_high <= 0.0f || vtln_high >= high_freq || vtln_high <= vtln_low)) {
     KNF_LOG(FATAL) << "Bad values in options: vtln-low " << vtln_low
                    << " and vtln-high " << vtln_high << ", versus "
                    << "low-freq " << low_freq << " and high-freq " << high_freq;
   }
 
   bins_.resize(num_bins);
+  center_freqs_.resize(num_bins);
 
   for (int32_t bin = 0; bin < num_bins; ++bin) {
     float left_mel = mel_low_freq + bin * mel_freq_delta,
           center_mel = mel_low_freq + (bin + 1) * mel_freq_delta,
           right_mel = mel_low_freq + (bin + 2) * mel_freq_delta;
 
     if (vtln_warp_factor != 1.0f) {
       left_mel = VtlnWarpMelFreq(vtln_low, vtln_high, low_freq, high_freq,
                                  vtln_warp_factor, left_mel);
       center_mel = VtlnWarpMelFreq(vtln_low, vtln_high, low_freq, high_freq,
                                    vtln_warp_factor, center_mel);
       right_mel = VtlnWarpMelFreq(vtln_low, vtln_high, low_freq, high_freq,
                                   vtln_warp_factor, right_mel);
     }
+    center_freqs_[bin] = InverseMelScale(center_mel);
 
     // this_bin will be a vector of coefficients that is only
     // nonzero where this mel bin is active.
     std::vector<float> this_bin(num_fft_bins);
 
     int32_t first_index = -1, last_index = -1;
     for (int32_t i = 0; i < num_fft_bins; ++i) {
@@ -214,40 +215,14 @@
       for (auto k : bins_[i].second) os << k << ", ";
       os << "\n";
     }
     KNF_LOG(INFO) << os.str();
   }
 }
 
-MelBanks::MelBanks(const float *weights, int32_t num_rows, int32_t num_cols) {
-  bins_.resize(num_rows);
-  for (int32_t bin = 0; bin < num_rows; ++bin) {
-    const float *this_bin = weights + bin * num_cols;
-
-    int32_t first_index = -1, last_index = -1;
-
-    for (int32_t i = 0; i < num_cols; ++i) {
-      if (this_bin[i] == 0) {
-        continue;
-      }
-      if (first_index == -1) first_index = i;
-      last_index = i;
-    }
-
-    KNF_CHECK(first_index != -1 && last_index >= first_index &&
-              "You have an incorrect weight matrix.");
-
-    bins_[bin].first = first_index;
-    int32_t size = last_index + 1 - first_index;
-
-    bins_[bin].second.insert(bins_[bin].second.end(), this_bin + first_index,
-                             this_bin + first_index + size);
-  }
-}
-
 // "power_spectrum" contains fft energies.
 void MelBanks::Compute(const float *power_spectrum,
                        float *mel_energies_out) const {
   int32_t num_bins = bins_.size();
 
   for (int32_t i = 0; i < num_bins; i++) {
     int32_t offset = bins_[i].first;
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/mel-computations.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/mel-computations.h`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,14 @@
  */
 // This file is copied/modified from kaldi/src/feat/mel-computations.h
 #ifndef KALDI_NATIVE_FBANK_CSRC_MEL_COMPUTATIONS_H_
 #define KALDI_NATIVE_FBANK_CSRC_MEL_COMPUTATIONS_H_
 
 #include <cmath>
 #include <string>
-#include <utility>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-window.h"
 
 namespace knf {
 
 struct MelBanksOptions {
   int32_t num_bins = 25;  // e.g. 25; number of triangular bins
@@ -85,30 +83,28 @@
                                float low_freq, float high_freq,
                                float vtln_warp_factor, float mel_freq);
 
   // TODO(fangjun): Remove vtln_warp_factor
   MelBanks(const MelBanksOptions &opts,
            const FrameExtractionOptions &frame_opts, float vtln_warp_factor);
 
-  // Initialize with a 2-d weights matrix
-  // @param weights Pointer to the start address of the matrix
-  // @param num_rows It equls to number of mel bins
-  // @param num_cols It equals to (number of fft bins)/2+1
-  MelBanks(const float *weights, int32_t num_rows, int32_t num_cols);
-
   /// Compute Mel energies (note: not log energies).
   /// At input, "fft_energies" contains the FFT energies (not log).
   ///
   /// @param fft_energies 1-D array of size num_fft_bins/2+1
   /// @param mel_energies_out  1-D array of size num_mel_bins
   void Compute(const float *fft_energies, float *mel_energies_out) const;
 
   int32_t NumBins() const { return bins_.size(); }
 
  private:
+  // center frequencies of bins, numbered from 0 ... num_bins-1.
+  // Needed by GetCenterFreqs().
+  std::vector<float> center_freqs_;
+
   // the "bins_" vector is a vector, one for each bin, of a pair:
   // (the first nonzero fft-bin), (the vector of weights).
   std::vector<std::pair<int32_t, std::vector<float>>> bins_;
 
   // TODO(fangjun): Remove debug_ and htk_mode_
   bool debug_;
   bool htk_mode_;
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/online-feature.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/online-feature.cc`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,14 @@
  */
 
 // The content in this file is copied/modified from
 // This file is copied/modified from kaldi/src/feat/online-feature.cc
 
 #include "kaldi-native-fbank/csrc/online-feature.h"
 
-#include <algorithm>
-#include <utility>
-#include <vector>
-
 #include "kaldi-native-fbank/csrc/feature-window.h"
 #include "kaldi-native-fbank/csrc/log.h"
 
 namespace knf {
 
 RecyclingVector::RecyclingVector(int32_t items_to_hold)
     : items_to_hold_(items_to_hold == 0 ? -1 : items_to_hold),
@@ -56,29 +52,28 @@
   items_.push_back(std::move(item));
 }
 
 int32_t RecyclingVector::Size() const {
   return first_available_index_ + static_cast<int32_t>(items_.size());
 }
 
-// discard the first n frames
-void RecyclingVector::Pop(int32_t n) {
-  for (int32_t i = 0; i < n && !items_.empty(); ++i) {
-    items_.pop_front();
-    ++first_available_index_;
-  }
-}
-
 template <class C>
 OnlineGenericBaseFeature<C>::OnlineGenericBaseFeature(
     const typename C::Options &opts)
     : computer_(opts),
       window_function_(computer_.GetFrameOptions()),
+      features_(opts.frame_opts.max_feature_vectors),
       input_finished_(false),
-      waveform_offset_(0) {}
+      waveform_offset_(0) {
+  // RE the following assert: search for ONLINE_IVECTOR_LIMIT in
+  // online-ivector-feature.cc.
+  // Casting to uint32, an unsigned type, means that -1 would be treated
+  // as `very large`.
+  KNF_CHECK(static_cast<uint32_t>(opts.frame_opts.max_feature_vectors) > 200);
+}
 
 template <class C>
 void OnlineGenericBaseFeature<C>::AcceptWaveform(float sampling_rate,
                                                  const float *waveform,
                                                  int32_t n) {
   if (n == 0) {
     return;  // Nothing to do.
@@ -158,10 +153,9 @@
 
       waveform_remainder_.swap(new_remainder);
     }
   }
 }
 
 template class OnlineGenericBaseFeature<FbankComputer>;
-template class OnlineGenericBaseFeature<WhisperFeatureComputer>;
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/online-feature.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/online-feature.h`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,16 @@
 // The content in this file is copied/modified from
 // This file is copied/modified from kaldi/src/feat/online-feature.h
 #ifndef KALDI_NATIVE_FBANK_CSRC_ONLINE_FEATURE_H_
 #define KALDI_NATIVE_FBANK_CSRC_ONLINE_FEATURE_H_
 
 #include <cstdint>
 #include <deque>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-fbank.h"
-#include "kaldi-native-fbank/csrc/whisper-feature.h"
 
 namespace knf {
 
 /// This class serves as a storage for feature vectors with an option to limit
 /// the memory usage by removing old elements. The deleted frames indices are
 /// "remembered" so that regardless of the MAX_ITEMS setting, the user always
 /// provides the indices as if no deletion was being performed.
@@ -53,17 +51,14 @@
   void PushBack(std::vector<float> item);
 
   /// This method returns the size as if no "recycling" had happened,
   /// i.e. equivalent to the number of times the PushBack method has been
   /// called.
   int32_t Size() const;
 
-  // discard the first n frames
-  void Pop(int32_t n);
-
  private:
   std::deque<std::vector<float>> items_;
   int32_t items_to_hold_;
   int32_t first_available_index_;
 };
 
 /// This is a templated class for online feature extraction;
@@ -103,17 +98,14 @@
 
   // InputFinished() tells the class you won't be providing any
   // more waveform.  This will help flush out the last frame or two
   // of features, in the case where snip-edges == false; it also
   // affects the return value of IsLastFrame().
   void InputFinished();
 
-  // discard the first n frames
-  void Pop(int32_t n) { features_.Pop(n); }
-
  private:
   // This function computes any additional feature frames that it is possible to
   // compute from 'waveform_remainder_', which at this point may contain more
   // than just a remainder-sized quantity (because AcceptWaveform() appends to
   // waveform_remainder_ before calling this function).  It adds these feature
   // frames to features_, and shifts off any now-unneeded samples of input from
   // waveform_remainder_ while incrementing waveform_offset_ by the same amount.
@@ -139,12 +131,11 @@
   // after extracting all the whole frames we can (whatever length of feature
   // will be required for the next phase of computation).
   // It is a 1-D tensor
   std::vector<float> waveform_remainder_;
 };
 
 using OnlineFbank = OnlineGenericBaseFeature<FbankComputer>;
-using OnlineWhisperFbank = OnlineGenericBaseFeature<WhisperFeatureComputer>;
 
 }  // namespace knf
 
 #endif  // KALDI_NATIVE_FBANK_CSRC_ONLINE_FEATURE_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/rfft.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/rfft.cc`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,27 @@
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include "kaldi-native-fbank/csrc/rfft.h"
 
-#include <algorithm>
 #include <cmath>
 #include <vector>
 
 #include "kaldi-native-fbank/csrc/log.h"
 
 // see fftsg.c
 #ifdef __cplusplus
 extern "C" void rdft(int n, int isgn, double *a, int *ip, double *w);
 #else
 void rdft(int n, int isgn, double *a, int *ip, double *w);
 #endif
 
 namespace knf {
-
 class Rfft::RfftImpl {
  public:
   explicit RfftImpl(int32_t n) : n_(n), ip_(2 + std::sqrt(n / 2)), w_(n / 2) {
     KNF_CHECK_EQ(n & (n - 1), 0);
   }
 
   void Compute(float *in_out) {
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/rfft.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/rfft.h`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-log.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-log.cc`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,14 @@
  */
 
 #include "gtest/gtest.h"
 #include "kaldi-native-fbank/csrc/log.h"
 
 namespace knf {
 
-#if KNF_ENABLE_CHECK
-
 TEST(Log, TestLog) {
   KNF_LOG(TRACE) << "this is a trace message";
   KNF_LOG(DEBUG) << "this is a debug message";
   KNF_LOG(INFO) << "this is an info message";
   KNF_LOG(WARNING) << "this is a warning message";
   KNF_LOG(ERROR) << "this is an error message";
 
@@ -64,10 +62,8 @@
   KNF_DCHECK_GE(2, 1) << "ok";
 
 #if !defined(NDEBUG)
   ASSERT_THROW(KNF_CHECK_EQ(2, 1) << "bad things happened", std::runtime_error);
 #endif
 }
 
-#endif
-
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-online-fbank.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-online-fbank.cc`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-online-feature.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-online-feature.cc`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/csrc/test-rfft.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/csrc/test-rfft.cc`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/CMakeLists.txt` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 pybind11_add_module(_kaldi_native_fbank
   feature-fbank.cc
   feature-window.cc
   kaldi-native-fbank.cc
   mel-computations.cc
   online-feature.cc
-  rfft.cc
   utils.cc
 )
 
 if(APPLE)
   execute_process(
     COMMAND "${PYTHON_EXECUTABLE}" -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
     OUTPUT_STRIP_TRAILING_WHITESPACE
@@ -19,11 +18,16 @@
 endif()
 
 if(NOT WIN32)
   target_link_libraries(_kaldi_native_fbank PRIVATE "-Wl,-rpath,${kaldi_native_fbank_rpath_origin}/kaldi_native_fbank/lib")
 endif()
 
 target_link_libraries(_kaldi_native_fbank PRIVATE kaldi-native-fbank-core)
+if(UNIX AND NOT APPLE)
+  target_link_libraries(_kaldi_native_fbank PUBLIC ${PYTHON_LIBRARY})
+elseif(WIN32)
+  target_link_libraries(_kaldi_native_fbank PUBLIC ${PYTHON_LIBRARIES})
+endif()
 
 install(TARGETS _kaldi_native_fbank
   DESTINATION ../
 )
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-fbank.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-fbank.cc`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #include <string>
 
 #include "kaldi-native-fbank/csrc/feature-fbank.h"
 #include "kaldi-native-fbank/python/csrc/utils.h"
 
 namespace knf {
 
-static void PybindFbankOptions(py::module &m) {  // NOLINT
+static void PybindFbankOptions(py::module &m) {
   using PyClass = FbankOptions;
   py::class_<PyClass>(m, "FbankOptions")
       .def(py::init<>())
       .def_readwrite("frame_opts", &PyClass::frame_opts)
       .def_readwrite("mel_opts", &PyClass::mel_opts)
       .def_readwrite("use_energy", &PyClass::use_energy)
       .def_readwrite("energy_floor", &PyClass::energy_floor)
@@ -46,12 +46,10 @@
           "from_dict",
           [](py::dict dict) -> PyClass { return FbankOptionsFromDict(dict); })
       .def(py::pickle(
           [](const PyClass &self) -> py::dict { return AsDict(self); },
           [](py::dict dict) -> PyClass { return FbankOptionsFromDict(dict); }));
 }
 
-void PybindFeatureFbank(py::module &m) {  // NOLINT
-  PybindFbankOptions(m);
-}
+void PybindFeatureFbank(py::module &m) { PybindFbankOptions(m); }
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-fbank.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-fbank.h`

 * *Files 12% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 #ifndef KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_FBANK_H_
 #define KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_FBANK_H_
 
 #include "kaldi-native-fbank/python/csrc/kaldi-native-fbank.h"
 
 namespace knf {
 
-void PybindFeatureFbank(py::module &m);  // NOLINT
+void PybindFeatureFbank(py::module &m);
 
 }  // namespace knf
 
 #endif  // KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_FBANK_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-window.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-window.cc`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,35 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include "kaldi-native-fbank/python/csrc/feature-window.h"
 
 #include <string>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/feature-window.h"
 #include "kaldi-native-fbank/python/csrc/utils.h"
 
 namespace knf {
 
-static void PybindFrameExtractionOptions(py::module &m) {  // NOLINT
+static void PybindFrameExtractionOptions(py::module &m) {
   using PyClass = FrameExtractionOptions;
   py::class_<PyClass>(m, "FrameExtractionOptions")
       .def(py::init<>())
       .def_readwrite("samp_freq", &PyClass::samp_freq)
       .def_readwrite("frame_shift_ms", &PyClass::frame_shift_ms)
       .def_readwrite("frame_length_ms", &PyClass::frame_length_ms)
       .def_readwrite("dither", &PyClass::dither)
       .def_readwrite("preemph_coeff", &PyClass::preemph_coeff)
       .def_readwrite("remove_dc_offset", &PyClass::remove_dc_offset)
       .def_readwrite("window_type", &PyClass::window_type)
       .def_readwrite("round_to_power_of_two", &PyClass::round_to_power_of_two)
       .def_readwrite("blackman_coeff", &PyClass::blackman_coeff)
       .def_readwrite("snip_edges", &PyClass::snip_edges)
+      .def_readwrite("max_feature_vectors", &PyClass::max_feature_vectors)
       .def("as_dict",
            [](const PyClass &self) -> py::dict { return AsDict(self); })
       .def_static("from_dict",
                   [](py::dict dict) -> PyClass {
                     return FrameExtractionOptionsFromDict(dict);
                   })
 #if 0
@@ -55,26 +55,11 @@
            [](const PyClass &self) -> std::string { return self.ToString(); })
       .def(py::pickle(
           [](const PyClass &self) -> py::dict { return AsDict(self); },
           [](py::dict dict) -> PyClass {
             return FrameExtractionOptionsFromDict(dict);
           }));
 }
-static void PybindFeatureWindowFunction(py::module *m) {
-  using PyClass = FeatureWindowFunction;
-  py::class_<PyClass>(*m, "FeatureWindowFunction")
-      .def(py::init<const FrameExtractionOptions &>(), py::arg("opts"))
-      .def("apply",
-           [](const PyClass &self,
-              std::vector<float> &wave) -> std::vector<float> {
-             self.Apply(wave.data());
-             return wave;
-           })
-      .def_property_readonly("window", &PyClass::GetWindow);
-}
 
-void PybindFeatureWindow(py::module &m) {  // NOLINT
-  PybindFrameExtractionOptions(m);
-  PybindFeatureWindowFunction(&m);
-}
+void PybindFeatureWindow(py::module &m) { PybindFrameExtractionOptions(m); }
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/feature-window.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/feature-window.h`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 #ifndef KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_WINDOW_H_
 #define KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_WINDOW_H_
 
 #include "kaldi-native-fbank/python/csrc/kaldi-native-fbank.h"
 
 namespace knf {
 
-void PybindFeatureWindow(py::module &m);  // NOLINT
+void PybindFeatureWindow(py::module &m);
 
 }  // namespace knf
 
 #endif  // KALDI_NATIVE_FBANK_PYTHON_CSRC_FEATURE_WINDOW_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/kaldi-native-fbank.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/kaldi-native-fbank.cc`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,20 @@
 
 #include "kaldi-native-fbank/python/csrc/kaldi-native-fbank.h"
 
 #include "kaldi-native-fbank/python/csrc/feature-fbank.h"
 #include "kaldi-native-fbank/python/csrc/feature-window.h"
 #include "kaldi-native-fbank/python/csrc/mel-computations.h"
 #include "kaldi-native-fbank/python/csrc/online-feature.h"
-#include "kaldi-native-fbank/python/csrc/rfft.h"
 
 namespace knf {
 
 PYBIND11_MODULE(_kaldi_native_fbank, m) {
   m.doc() = "Python wrapper for kaldi native fbank";
   PybindFeatureWindow(m);
   PybindMelComputations(m);
   PybindFeatureFbank(m);
-  PybindRfft(m);
 
   PybindOnlineFeature(m);
 }
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/kaldi-native-fbank.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/kaldi-native-fbank.h`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/mel-computations.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/mel-computations.cc`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #include <string>
 
 #include "kaldi-native-fbank/csrc/mel-computations.h"
 #include "kaldi-native-fbank/python/csrc/utils.h"
 
 namespace knf {
 
-static void PybindMelBanksOptions(py::module &m) {  // NOLINT
+static void PybindMelBanksOptions(py::module &m) {
   using PyClass = MelBanksOptions;
   py::class_<PyClass>(m, "MelBanksOptions")
       .def(py::init<>())
       .def_readwrite("num_bins", &PyClass::num_bins)
       .def_readwrite("low_freq", &PyClass::low_freq)
       .def_readwrite("high_freq", &PyClass::high_freq)
       .def_readwrite("vtln_low", &PyClass::vtln_low)
@@ -47,12 +47,10 @@
       .def(py::pickle(
           [](const PyClass &self) -> py::dict { return AsDict(self); },
           [](py::dict dict) -> PyClass {
             return MelBanksOptionsFromDict(dict);
           }));
 }
 
-void PybindMelComputations(py::module &m) {  // NOLINT
-  PybindMelBanksOptions(m);
-}
+void PybindMelComputations(py::module &m) { PybindMelBanksOptions(m); }
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/mel-computations.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/mel-computations.h`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 #ifndef KALDI_NATIVE_FBANK_PYTHON_CSRC_MEL_COMPUTATIONS_H_
 #define KALDI_NATIVE_FBANK_PYTHON_CSRC_MEL_COMPUTATIONS_H_
 
 #include "kaldi-native-fbank/python/csrc/kaldi-native-fbank.h"
 
 namespace knf {
 
-void PybindMelComputations(py::module &m);  // NOLINT
+void PybindMelComputations(py::module &m);
 
 }  // namespace knf
 
 #endif  // KALDI_NATIVE_FBANK_PYTHON_CSRC_MEL_COMPUTATIONS_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/online-feature.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/online-feature.cc`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,20 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  */
 
 #include "kaldi-native-fbank/python/csrc/online-feature.h"
 
 #include <string>
-#include <vector>
 
 #include "kaldi-native-fbank/csrc/online-feature.h"
 namespace knf {
 
 template <typename C>
-void PybindOnlineFeatureTpl(py::module &m,  // NOLINT
-                            const std::string &class_name,
+void PybindOnlineFeatureTpl(py::module &m, const std::string &class_name,
                             const std::string &class_help_doc = "") {
   using PyClass = OnlineGenericBaseFeature<C>;
   using Options = typename C::Options;
   py::class_<PyClass>(m, class_name.c_str(), class_help_doc.c_str())
       .def(py::init<const Options &>(), py::arg("opts"))
       .def_property_readonly("dim", &PyClass::Dim)
       .def_property_readonly("frame_shift_in_seconds",
@@ -57,13 +55,12 @@
                                 waveform.size());
           },
           py::arg("sampling_rate"), py::arg("waveform"),
           py::call_guard<py::gil_scoped_release>())
       .def("input_finished", &PyClass::InputFinished);
 }
 
-void PybindOnlineFeature(py::module &m) {  // NOLINT
+void PybindOnlineFeature(py::module &m) {
   PybindOnlineFeatureTpl<FbankComputer>(m, "OnlineFbank");
-  PybindOnlineFeatureTpl<WhisperFeatureComputer>(m, "OnlineWhisperFbank");
 }
 
 }  // namespace knf
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/online-feature.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/online-feature.h`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 #ifndef KALDI_NATIVE_FBANK_PYTHON_CSRC_ONLINE_FEATURE_H_
 #define KALDI_NATIVE_FBANK_PYTHON_CSRC_ONLINE_FEATURE_H_
 
 #include "kaldi-native-fbank/python/csrc/kaldi-native-fbank.h"
 
 namespace knf {
 
-void PybindOnlineFeature(py::module &m);  // NOLINT
+void PybindOnlineFeature(py::module &m);
 
 }  // namespace knf
 
 #endif  // KALDI_NATIVE_FBANK_PYTHON_CSRC_ONLINE_FEATURE_H_
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/utils.cc` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/utils.cc`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
   FROM_DICT(float_, dither);
   FROM_DICT(float_, preemph_coeff);
   FROM_DICT(bool_, remove_dc_offset);
   FROM_DICT(str, window_type);
   FROM_DICT(bool_, round_to_power_of_two);
   FROM_DICT(float_, blackman_coeff);
   FROM_DICT(bool_, snip_edges);
+  FROM_DICT(int_, max_feature_vectors);
 
   return opts;
 }
 
 py::dict AsDict(const FrameExtractionOptions &opts) {
   py::dict dict;
 
@@ -57,14 +58,15 @@
   AS_DICT(dither);
   AS_DICT(preemph_coeff);
   AS_DICT(remove_dc_offset);
   AS_DICT(window_type);
   AS_DICT(round_to_power_of_two);
   AS_DICT(blackman_coeff);
   AS_DICT(snip_edges);
+  AS_DICT(max_feature_vectors);
 
   return dict;
 }
 
 MelBanksOptions MelBanksOptionsFromDict(py::dict dict) {
   MelBanksOptions opts;
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/csrc/utils.h` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/CMakeLists.txt` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,17 @@
   set_property(TEST ${name}
     PROPERTY ENVIRONMENT "PYTHONPATH=${kaldi_native_fbank_path}:$<TARGET_FILE_DIR:_kaldi_native_fbank>:$ENV{PYTHONPATH}"
   )
 endfunction()
 
 # please sort the files in alphabetic order
 set(py_test_files
-  test_fbank_options.py
-  test_feature_window_function.py
   test_frame_extraction_options.py
   test_mel_bank_options.py
-  test_online_whisper_fbank.py
-  test_rfft.py
+  test_fbank_options.py
 )
 
 if(KALDI_NATIVE_FBANK_BUILD_TESTS)
   foreach(source IN LISTS py_test_files)
     kaldi_native_fbank_add_py_test(${source})
   endforeach()
 endif()
```

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_fbank_options.py` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_fbank_options.py`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_frame_extraction_options.py` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_frame_extraction_options.py`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_mel_bank_options.py` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_mel_bank_options.py`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi-native-fbank/python/tests/test_online_fbank.py` & `kaldi-native-fbank-1.9/kaldi-native-fbank/python/tests/test_online_fbank.py`

 * *Files identical despite different names*

### Comparing `kaldi-native-fbank-1.18.0/kaldi_native_fbank.egg-info/SOURCES.txt` & `kaldi-native-fbank-1.9/kaldi_native_fbank.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-cmake/__init__.py
 cmake/cmake_extension.py
 cmake/googletest.cmake
 cmake/pybind11.cmake
 cmake/Modules/FetchContent.cmake
 cmake/Modules/README.md
 cmake/Modules/FetchContent/CMakeLists.cmake.in
-cmake/__pycache__/__init__.cpython-310.pyc
-cmake/__pycache__/cmake_extension.cpython-310.pyc
+cmake/__pycache__/cmake_extension.cpython-38.pyc
 kaldi-native-fbank/CMakeLists.txt
 kaldi-native-fbank/csrc/CMakeLists.txt
 kaldi-native-fbank/csrc/feature-fbank.cc
 kaldi-native-fbank/csrc/feature-fbank.h
 kaldi-native-fbank/csrc/feature-functions.cc
 kaldi-native-fbank/csrc/feature-functions.h
 kaldi-native-fbank/csrc/feature-window.cc
 kaldi-native-fbank/csrc/feature-window.h
 kaldi-native-fbank/csrc/fftsg.c
-kaldi-native-fbank/csrc/generate-whisper-melbank.py
 kaldi-native-fbank/csrc/log.cc
 kaldi-native-fbank/csrc/log.h
 kaldi-native-fbank/csrc/mel-computations.cc
 kaldi-native-fbank/csrc/mel-computations.h
 kaldi-native-fbank/csrc/online-feature.cc
 kaldi-native-fbank/csrc/online-feature.h
 kaldi-native-fbank/csrc/rfft.cc
 kaldi-native-fbank/csrc/rfft.h
 kaldi-native-fbank/csrc/test-log.cc
 kaldi-native-fbank/csrc/test-online-fbank.cc
 kaldi-native-fbank/csrc/test-online-feature.cc
 kaldi-native-fbank/csrc/test-rfft.cc
-kaldi-native-fbank/csrc/whisper-feature.cc
-kaldi-native-fbank/csrc/whisper-feature.h
-kaldi-native-fbank/csrc/whisper-mel-bank.h
 kaldi-native-fbank/python/CMakeLists.txt
 kaldi-native-fbank/python/csrc/CMakeLists.txt
 kaldi-native-fbank/python/csrc/feature-fbank.cc
 kaldi-native-fbank/python/csrc/feature-fbank.h
 kaldi-native-fbank/python/csrc/feature-window.cc
 kaldi-native-fbank/python/csrc/feature-window.h
 kaldi-native-fbank/python/csrc/kaldi-native-fbank.cc
 kaldi-native-fbank/python/csrc/kaldi-native-fbank.h
 kaldi-native-fbank/python/csrc/mel-computations.cc
 kaldi-native-fbank/python/csrc/mel-computations.h
 kaldi-native-fbank/python/csrc/online-feature.cc
 kaldi-native-fbank/python/csrc/online-feature.h
-kaldi-native-fbank/python/csrc/rfft.cc
-kaldi-native-fbank/python/csrc/rfft.h
 kaldi-native-fbank/python/csrc/utils.cc
 kaldi-native-fbank/python/csrc/utils.h
 kaldi-native-fbank/python/kaldi_native_fbank/__init__.py
 kaldi-native-fbank/python/tests/CMakeLists.txt
 kaldi-native-fbank/python/tests/test_fbank_options.py
-kaldi-native-fbank/python/tests/test_feature_window_function.py
 kaldi-native-fbank/python/tests/test_frame_extraction_options.py
 kaldi-native-fbank/python/tests/test_mel_bank_options.py
 kaldi-native-fbank/python/tests/test_online_fbank.py
-kaldi-native-fbank/python/tests/test_online_whisper_fbank.py
-kaldi-native-fbank/python/tests/test_rfft.py
 kaldi_native_fbank.egg-info/PKG-INFO
 kaldi_native_fbank.egg-info/SOURCES.txt
 kaldi_native_fbank.egg-info/dependency_links.txt
 kaldi_native_fbank.egg-info/not-zip-safe
 kaldi_native_fbank.egg-info/top_level.txt
```

### Comparing `kaldi-native-fbank-1.18.0/setup.py` & `kaldi-native-fbank-1.9/setup.py`

 * *Files identical despite different names*

