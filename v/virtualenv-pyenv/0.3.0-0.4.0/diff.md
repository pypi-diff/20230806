# Comparing `tmp/virtualenv_pyenv-0.3.0.tar.gz` & `tmp/virtualenv-pyenv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualenv_pyenv-0.3.0.tar", max compression
+gzip compressed data, was "virtualenv-pyenv-0.4.0.tar", last modified: Sun Aug  6 09:35:04 2023, max compression
```

## Comparing `virtualenv_pyenv-0.3.0.tar` & `virtualenv-pyenv-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,20 @@
--rw-r--r--   0        0        0     1099 2023-07-14 09:50:32.674448 virtualenv_pyenv-0.3.0/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-13 14:26:07.450787 virtualenv_pyenv-0.3.0/README.md
--rw-r--r--   0        0        0     1555 2023-07-13 14:58:13.210574 virtualenv_pyenv-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-13 14:58:20.454688 virtualenv_pyenv-0.3.0/src/_virtualenv_pyenv/__init__.py
--rw-r--r--   0        0        0     4669 2023-07-10 10:33:32.312416 virtualenv_pyenv-0.3.0/src/_virtualenv_pyenv/discovery.py
--rw-r--r--   0        0        0     5021 1970-01-01 00:00:00.000000 virtualenv_pyenv-0.3.0/PKG-INFO
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/
+-rw-rw-r--   0 def       (1000) def       (1000)     1099 2023-07-14 09:50:32.000000 virtualenv-pyenv-0.4.0/LICENSE
+-rw-rw-r--   0 def       (1000) def       (1000)     8711 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     6333 2023-08-04 14:04:19.000000 virtualenv-pyenv-0.4.0/README.md
+-rw-rw-r--   0 def       (1000) def       (1000)     2309 2023-08-03 10:12:30.000000 virtualenv-pyenv-0.4.0/pyproject.toml
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/src/
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/src/_virtualenv_pyenv/
+-rw-rw-r--   0 def       (1000) def       (1000)       22 2023-08-06 09:34:04.000000 virtualenv-pyenv-0.4.0/src/_virtualenv_pyenv/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     6646 2023-08-03 10:11:28.000000 virtualenv-pyenv-0.4.0/src/_virtualenv_pyenv/discovery.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/
+-rw-rw-r--   0 def       (1000) def       (1000)     8711 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)      430 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/SOURCES.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/dependency_links.txt
+-rw-rw-r--   0 def       (1000) def       (1000)      240 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/entry_points.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       35 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/requires.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       18 2023-08-06 09:35:04.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/top_level.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-08-06 09:34:20.000000 virtualenv-pyenv-0.4.0/src/virtualenv_pyenv.egg-info/zip-safe
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-06 09:35:04.159952 virtualenv-pyenv-0.4.0/tests/
+-rw-rw-r--   0 def       (1000) def       (1000)    11122 2023-08-04 14:09:11.000000 virtualenv-pyenv-0.4.0/tests/test_discovery.py
```

### Comparing `virtualenv_pyenv-0.3.0/LICENSE` & `virtualenv-pyenv-0.4.0/LICENSE`

 * *Files identical despite different names*

