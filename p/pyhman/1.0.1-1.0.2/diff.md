# Comparing `tmp/pyhman-1.0.1.tar.gz` & `tmp/pyhman-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhman-1.0.1.tar", last modified: Sun Aug  6 16:11:24 2023, max compression
+gzip compressed data, was "pyhman-1.0.2.tar", last modified: Sun Aug  6 16:15:30 2023, max compression
```

## Comparing `pyhman-1.0.1.tar` & `pyhman-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:11:24.134344 pyhman-1.0.1/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)    35149 2023-06-17 13:27:16.000000 pyhman-1.0.1/LICENSE
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      190 2023-08-06 16:11:24.134344 pyhman-1.0.1/PKG-INFO
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2551 2023-06-17 13:55:43.000000 pyhman-1.0.1/README.md
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:11:24.134344 pyhman-1.0.1/pyhman/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)        0 2023-06-17 09:51:56.000000 pyhman-1.0.1/pyhman/__init__.py
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     8415 2023-08-06 15:57:26.000000 pyhman-1.0.1/pyhman/hman.py
--rw-rw-r--   0 aightech  (1000) aightech  (1000)     2799 2023-06-17 11:43:16.000000 pyhman-1.0.1/pyhman/hmanserver.py
-drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:11:24.134344 pyhman-1.0.1/pyhman.egg-info/
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      190 2023-08-06 16:11:24.000000 pyhman-1.0.1/pyhman.egg-info/PKG-INFO
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      201 2023-08-06 16:11:24.000000 pyhman-1.0.1/pyhman.egg-info/SOURCES.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)        1 2023-08-06 16:11:24.000000 pyhman-1.0.1/pyhman.egg-info/dependency_links.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)        7 2023-08-06 16:11:24.000000 pyhman-1.0.1/pyhman.egg-info/top_level.txt
--rw-rw-r--   0 aightech  (1000) aightech  (1000)       38 2023-08-06 16:11:24.134344 pyhman-1.0.1/setup.cfg
--rw-rw-r--   0 aightech  (1000) aightech  (1000)      357 2023-08-06 16:02:19.000000 pyhman-1.0.1/setup.py
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:15:30.216760 pyhman-1.0.2/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)    35149 2023-06-17 13:27:16.000000 pyhman-1.0.2/LICENSE
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2791 2023-08-06 16:15:30.216760 pyhman-1.0.2/PKG-INFO
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2551 2023-06-17 13:55:43.000000 pyhman-1.0.2/README.md
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:15:30.216760 pyhman-1.0.2/pyhman/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)        0 2023-06-17 09:51:56.000000 pyhman-1.0.2/pyhman/__init__.py
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     8415 2023-08-06 15:57:26.000000 pyhman-1.0.2/pyhman/hman.py
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2799 2023-06-17 11:43:16.000000 pyhman-1.0.2/pyhman/hmanserver.py
+drwxrwxr-x   0 aightech  (1000) aightech  (1000)        0 2023-08-06 16:15:30.216760 pyhman-1.0.2/pyhman.egg-info/
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)     2791 2023-08-06 16:15:30.000000 pyhman-1.0.2/pyhman.egg-info/PKG-INFO
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)      201 2023-08-06 16:15:30.000000 pyhman-1.0.2/pyhman.egg-info/SOURCES.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)        1 2023-08-06 16:15:30.000000 pyhman-1.0.2/pyhman.egg-info/dependency_links.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)        7 2023-08-06 16:15:30.000000 pyhman-1.0.2/pyhman.egg-info/top_level.txt
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)       38 2023-08-06 16:15:30.216760 pyhman-1.0.2/setup.cfg
+-rw-rw-r--   0 aightech  (1000) aightech  (1000)      472 2023-08-06 16:15:25.000000 pyhman-1.0.2/setup.py
```

### Comparing `pyhman-1.0.1/LICENSE` & `pyhman-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhman-1.0.1/README.md` & `pyhman-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhman-1.0.1/pyhman/hman.py` & `pyhman-1.0.2/pyhman/hman.py`

 * *Files identical despite different names*

### Comparing `pyhman-1.0.1/pyhman/hmanserver.py` & `pyhman-1.0.2/pyhman/hmanserver.py`

 * *Files identical despite different names*

