# Comparing `tmp/cjptools-0.1.8.tar.gz` & `tmp/cjptools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjptools-0.1.8.tar", last modified: Sun Aug  6 06:59:58 2023, max compression
+gzip compressed data, was "cjptools-0.1.9.tar", last modified: Sun Aug  6 07:02:55 2023, max compression
```

## Comparing `cjptools-0.1.8.tar` & `cjptools-0.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.610340 cjptools-0.1.8/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      276 2023-08-06 06:59:58.610340 cjptools-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.565284 cjptools-0.1.8/cjptools/
--rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.8/cjptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.573316 cjptools-0.1.8/cjptools/dptools/
--rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.8/cjptools/dptools/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.8/cjptools/dptools/rdpAccount.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.590516 cjptools-0.1.8/cjptools/interfaces/
--rw-rw-rw-   0        0        0       19 2023-08-06 05:58:36.000000 cjptools-0.1.8/cjptools/interfaces/__init__.py
--rw-rw-rw-   0        0        0     4000 2023-08-06 06:59:42.000000 cjptools-0.1.8/cjptools/interfaces/data.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.597401 cjptools-0.1.8/cjptools/printModules/
--rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.8/cjptools/printModules/__init__.py
--rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.8/cjptools/printModules/absPrinter.py
--rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.8/cjptools/printModules/printerCompose.py
--rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.8/cjptools/printModules/printers.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.606341 cjptools-0.1.8/cjptools/utils/
--rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.8/cjptools/utils/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.8/cjptools/utils/check.py
--rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.8/cjptools/utils/gpu_mem_track.py
--rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.8/cjptools/utils/modelsize_estimate.py
--rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.8/cjptools/utils/path.py
--rw-rw-rw-   0        0        0      336 2023-08-03 07:47:46.000000 cjptools-0.1.8/cjptools/utils/reflect.py
--rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.8/cjptools/utils/rnd.py
--rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.8/cjptools/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-08-06 06:59:58.569316 cjptools-0.1.8/cjptools.egg-info/
--rw-rw-rw-   0        0        0      276 2023-08-06 06:59:58.000000 cjptools-0.1.8/cjptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-08-06 06:59:58.000000 cjptools-0.1.8/cjptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 06:59:58.000000 cjptools-0.1.8/cjptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-06 06:59:58.000000 cjptools-0.1.8/cjptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-06 06:59:58.610340 cjptools-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-08-06 06:59:34.000000 cjptools-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.070054 cjptools-0.1.9/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-08-06 07:02:55.070054 cjptools-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.041701 cjptools-0.1.9/cjptools/
+-rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.9/cjptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.049696 cjptools-0.1.9/cjptools/dptools/
+-rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.9/cjptools/dptools/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.9/cjptools/dptools/rdpAccount.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.053668 cjptools-0.1.9/cjptools/interfaces/
+-rw-rw-rw-   0        0        0       19 2023-08-06 05:58:36.000000 cjptools-0.1.9/cjptools/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3997 2023-08-06 07:01:47.000000 cjptools-0.1.9/cjptools/interfaces/data.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.057667 cjptools-0.1.9/cjptools/printModules/
+-rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.9/cjptools/printModules/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.9/cjptools/printModules/absPrinter.py
+-rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.9/cjptools/printModules/printerCompose.py
+-rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.9/cjptools/printModules/printers.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.070054 cjptools-0.1.9/cjptools/utils/
+-rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.9/cjptools/utils/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.9/cjptools/utils/check.py
+-rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.9/cjptools/utils/gpu_mem_track.py
+-rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.9/cjptools/utils/modelsize_estimate.py
+-rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.9/cjptools/utils/path.py
+-rw-rw-rw-   0        0        0      336 2023-08-03 07:47:46.000000 cjptools-0.1.9/cjptools/utils/reflect.py
+-rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.9/cjptools/utils/rnd.py
+-rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.9/cjptools/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-08-06 07:02:55.045697 cjptools-0.1.9/cjptools.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-08-06 07:02:54.000000 cjptools-0.1.9/cjptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-08-06 07:02:55.000000 cjptools-0.1.9/cjptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 07:02:54.000000 cjptools-0.1.9/cjptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 07:02:54.000000 cjptools-0.1.9/cjptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 07:02:55.070054 cjptools-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-08-06 07:01:51.000000 cjptools-0.1.9/setup.py
```

### Comparing `cjptools-0.1.8/LICENSE` & `cjptools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/dptools/rdpAccount.py` & `cjptools-0.1.9/cjptools/dptools/rdpAccount.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/interfaces/data.py` & `cjptools-0.1.9/cjptools/interfaces/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,31 +61,31 @@
 
     def __str__(self):
         res = ""
         if self.localTrains:
             res += "\n====================本地训练数据集===================="
             for (i, dataloader) in enumerate(self.localTrains):
                 if dataloader:
-                    res += f"\n> [本地训练数据集 {i}]："
+                    res += f"\n> [本地训练数据集 {i}]\n"
                     res += display_data_details(dataloader)
                 else:
                     res += f"\n> [warning] 本地训练数据集 {i} 不存在！"
         if self.localVals:
             res += "\n====================本地验证数据集===================="
             for (i, dataloader) in enumerate(self.localVals):
                 if dataloader:
-                    res += f"\n> [本地验证数据集 {i}]："
+                    res += f"\n> [本地验证数据集 {i}]\n"
                     res += display_data_details(dataloader)
                 else:
                     res += f"\n> [warning] 本地验证数据集 {i} 不存在！"
         if self.localTests:
             res += "\n====================本地测试数据集===================="
             for (i, dataloader) in enumerate(self.localTests):
                 if dataloader:
-                    res += f"\n> [本地测试数据集 {i}]："
+                    res += f"\n> [本地测试数据集 {i}]\n"
                     res += display_data_details(dataloader)
                 else:
                     res += f"\n> [warning] 本地测试数据集 {i} 不存在！"
         if self.globalTrain:
             res += "\n====================全局训练数据集====================\n"
             res += display_data_details(self.globalTrain)
         if self.globalVal:
```

### Comparing `cjptools-0.1.8/cjptools/printModules/printers.py` & `cjptools-0.1.9/cjptools/printModules/printers.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/utils/gpu_mem_track.py` & `cjptools-0.1.9/cjptools/utils/gpu_mem_track.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/utils/modelsize_estimate.py` & `cjptools-0.1.9/cjptools/utils/modelsize_estimate.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/utils/path.py` & `cjptools-0.1.9/cjptools/utils/path.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools/utils/rnd.py` & `cjptools-0.1.9/cjptools/utils/rnd.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/cjptools.egg-info/SOURCES.txt` & `cjptools-0.1.9/cjptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.8/setup.py` & `cjptools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="cjptools",
-    version="0.1.8",
+    version="0.1.9",
     keywords=("database", "localServer"),
     description="My Personal Toolkit",
     long_description="My Personal Toolkit",
     license="MIT Licence",
     author="Cai Jianping",
     author_email="jpingcai@163.com",
```

