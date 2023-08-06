# Comparing `tmp/rethge_torch-0.0.1.tar.gz` & `tmp/rethge_torch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rethge_torch-0.0.1.tar", last modified: Sun Aug  6 08:48:26 2023, max compression
+gzip compressed data, was "rethge_torch-0.0.2.tar", last modified: Sun Aug  6 12:15:45 2023, max compression
```

## Comparing `rethge_torch-0.0.1.tar` & `rethge_torch-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 08:48:26.973686 rethge_torch-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-08-06 07:05:45.000000 rethge_torch-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1078 2023-08-06 08:48:26.974686 rethge_torch-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-08-06 08:46:52.000000 rethge_torch-0.0.1/README.md
--rw-rw-rw-   0        0        0      440 2023-08-06 08:37:43.000000 rethge_torch-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-08-06 08:48:26.976695 rethge_torch-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 08:48:26.963686 rethge_torch-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 08:48:26.970687 rethge_torch-0.0.1/src/rethge_torch/
--rw-rw-rw-   0        0        0        0 2023-08-06 07:08:14.000000 rethge_torch-0.0.1/src/rethge_torch/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-06 07:08:25.000000 rethge_torch-0.0.1/src/rethge_torch/main.py
--rw-rw-rw-   0        0        0    14062 2023-08-06 08:15:01.000000 rethge_torch-0.0.1/src/rethge_torch/rethge_components.py
--rw-rw-rw-   0        0        0    41610 2023-08-06 08:11:50.000000 rethge_torch-0.0.1/src/rethge_torch/rethge_torch.py
--rw-rw-rw-   0        0        0     5891 2023-08-06 08:13:47.000000 rethge_torch-0.0.1/src/rethge_torch/rethge_train_with_track.py
-drwxrwxrwx   0        0        0        0 2023-08-06 08:48:26.973686 rethge_torch-0.0.1/src/rethge_torch.egg-info/
--rw-rw-rw-   0        0        0     1078 2023-08-06 08:48:26.000000 rethge_torch-0.0.1/src/rethge_torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-08-06 08:48:26.000000 rethge_torch-0.0.1/src/rethge_torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 08:48:26.000000 rethge_torch-0.0.1/src/rethge_torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-06 08:48:26.000000 rethge_torch-0.0.1/src/rethge_torch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 12:15:45.299586 rethge_torch-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-08-06 07:05:45.000000 rethge_torch-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1078 2023-08-06 12:15:45.299586 rethge_torch-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-08-06 08:46:52.000000 rethge_torch-0.0.2/README.md
+-rw-rw-rw-   0        0        0      440 2023-08-06 08:37:43.000000 rethge_torch-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-08-06 12:15:45.300577 rethge_torch-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 12:15:45.285566 rethge_torch-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 12:15:45.295578 rethge_torch-0.0.2/src/rethge_torch/
+-rw-rw-rw-   0        0        0        0 2023-08-06 07:08:14.000000 rethge_torch-0.0.2/src/rethge_torch/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 07:08:14.000000 rethge_torch-0.0.2/src/rethge_torch/main.py
+-rw-rw-rw-   0        0        0    41610 2023-08-06 08:11:50.000000 rethge_torch-0.0.2/src/rethge_torch/rethge.py
+-rw-rw-rw-   0        0        0    14062 2023-08-06 08:15:01.000000 rethge_torch-0.0.2/src/rethge_torch/rethge_components.py
+-rw-rw-rw-   0        0        0     5891 2023-08-06 08:13:47.000000 rethge_torch-0.0.2/src/rethge_torch/rethge_train_with_track.py
+drwxrwxrwx   0        0        0        0 2023-08-06 12:15:45.298580 rethge_torch-0.0.2/src/rethge_torch.egg-info/
+-rw-rw-rw-   0        0        0     1078 2023-08-06 12:15:45.000000 rethge_torch-0.0.2/src/rethge_torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-08-06 12:15:45.000000 rethge_torch-0.0.2/src/rethge_torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 12:15:45.000000 rethge_torch-0.0.2/src/rethge_torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-06 12:15:45.000000 rethge_torch-0.0.2/src/rethge_torch.egg-info/top_level.txt
```

### Comparing `rethge_torch-0.0.1/PKG-INFO` & `rethge_torch-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rethge_torch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package that contains help functions to convenient pytorch using. including plot, model train & evaluate, results analysis and more...
 Home-page: https://github.com/ReThGe/rethge_torch
 Author: ReThGe
 Author-email: YanShumai8274@163.com
 Project-URL: Bug Tracker, https://github.com/ReThGe/rethge_torch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rethge_torch-0.0.1/setup.cfg` & `rethge_torch-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6574 6867 655f 746f 7263 680d   = rethge_torch.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
 00000030: 0d0a 6175 7468 6f72 203d 2052 6554 6847  ..author = ReThG
 00000040: 650d 0a61 7574 686f 725f 656d 6169 6c20  e..author_email 
 00000050: 3d20 5961 6e53 6875 6d61 6938 3237 3440  = YanShumai8274@
 00000060: 3136 332e 636f 6d0d 0a64 6573 6372 6970  163.com..descrip
 00000070: 7469 6f6e 203d 2041 2073 6d61 6c6c 2070  tion = A small p
 00000080: 6163 6b61 6765 2074 6861 7420 636f 6e74  ackage that cont
 00000090: 6169 6e73 2068 656c 7020 6675 6e63 7469  ains help functi
```

### Comparing `rethge_torch-0.0.1/src/rethge_torch/rethge_components.py` & `rethge_torch-0.0.2/src/rethge_torch/rethge_components.py`

 * *Files identical despite different names*

### Comparing `rethge_torch-0.0.1/src/rethge_torch/rethge_torch.py` & `rethge_torch-0.0.2/src/rethge_torch/rethge.py`

 * *Files identical despite different names*

### Comparing `rethge_torch-0.0.1/src/rethge_torch/rethge_train_with_track.py` & `rethge_torch-0.0.2/src/rethge_torch/rethge_train_with_track.py`

 * *Files identical despite different names*

### Comparing `rethge_torch-0.0.1/src/rethge_torch.egg-info/PKG-INFO` & `rethge_torch-0.0.2/src/rethge_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rethge-torch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package that contains help functions to convenient pytorch using. including plot, model train & evaluate, results analysis and more...
 Home-page: https://github.com/ReThGe/rethge_torch
 Author: ReThGe
 Author-email: YanShumai8274@163.com
 Project-URL: Bug Tracker, https://github.com/ReThGe/rethge_torch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

