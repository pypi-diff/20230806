# Comparing `tmp/apollo11log-0.1.0.tar.gz` & `tmp/apollo11log-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo11log-0.1.0.tar", max compression
+gzip compressed data, was "apollo11log-0.1.1.tar", max compression
```

## Comparing `apollo11log-0.1.0.tar` & `apollo11log-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-06 00:41:21.535969 apollo11log-0.1.0/README.md
--rw-r--r--   0        0        0      995 2023-08-06 00:40:17.649475 apollo11log-0.1.0/apollo11log/__main__.py
--rw-r--r--   0        0        0   818263 2023-08-06 00:30:42.777437 apollo11log-0.1.0/apollo11log/log.txt
--rw-r--r--   0        0        0      421 2023-08-06 00:48:05.526757 apollo11log-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      647 2023-08-06 00:48:10.226594 apollo11log-0.1.0/setup.py
--rw-r--r--   0        0        0      396 2023-08-06 00:48:10.226799 apollo11log-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      763 2023-08-06 00:50:06.136189 apollo11log-0.1.1/README.md
+-rw-r--r--   0        0        0      995 2023-08-06 00:40:17.649475 apollo11log-0.1.1/apollo11log/__main__.py
+-rw-r--r--   0        0        0   818263 2023-08-06 00:30:42.777437 apollo11log-0.1.1/apollo11log/log.txt
+-rw-r--r--   0        0        0      454 2023-08-06 00:50:25.148989 apollo11log-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1485 2023-08-06 00:50:56.190277 apollo11log-0.1.1/setup.py
+-rw-r--r--   0        0        0     1192 2023-08-06 00:50:56.190550 apollo11log-0.1.1/PKG-INFO
```

### Comparing `apollo11log-0.1.0/apollo11log/__main__.py` & `apollo11log-0.1.1/apollo11log/__main__.py`

 * *Files identical despite different names*

### Comparing `apollo11log-0.1.0/apollo11log/log.txt` & `apollo11log-0.1.1/apollo11log/log.txt`

 * *Files identical despite different names*

