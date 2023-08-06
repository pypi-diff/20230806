# Comparing `tmp/HawaData-0.9.2.tar.gz` & `tmp/HawaData-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.9.2.tar", last modified: Sun Aug  6 09:45:42 2023, max compression
+gzip compressed data, was "HawaData-0.9.3.tar", last modified: Sun Aug  6 11:10:49 2023, max compression
```

## Comparing `HawaData-0.9.2.tar` & `HawaData-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.688098 HawaData-0.9.2/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.672208 HawaData-0.9.2/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3606 2023-08-06 09:45:42.000000 HawaData-0.9.2/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-08-06 09:45:42.000000 HawaData-0.9.2/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-08-06 09:45:42.000000 HawaData-0.9.2/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-08-06 09:45:42.000000 HawaData-0.9.2/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3606 2023-08-06 09:45:42.687806 HawaData-0.9.2/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.9.2/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.672742 HawaData-0.9.2/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.9.2/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.676169 HawaData-0.9.2/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.9.2/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.9.2/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.9.2/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      142 2023-08-01 09:59:51.000000 HawaData-0.9.2/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.9.2/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.679512 HawaData-0.9.2/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.9.2/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    17368 2023-07-27 05:22:54.000000 HawaData-0.9.2/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6517 2023-07-27 05:22:54.000000 HawaData-0.9.2/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.9.2/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.9.2/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.684829 HawaData-0.9.2/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.9.2/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.9.2/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.9.2/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.9.2/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.9.2/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.9.2/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1181 2023-08-01 09:59:51.000000 HawaData-0.9.2/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.686518 HawaData-0.9.2/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.9.2/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    29047 2023-08-06 09:44:56.000000 HawaData-0.9.2/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.9.2/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-08-06 09:45:42.688183 HawaData-0.9.2/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.9.2/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 09:45:42.687212 HawaData-0.9.2/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.9.2/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.139787 HawaData-0.9.3/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.125337 HawaData-0.9.3/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3622 2023-08-06 11:10:49.000000 HawaData-0.9.3/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-08-06 11:10:49.000000 HawaData-0.9.3/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-08-06 11:10:49.000000 HawaData-0.9.3/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-08-06 11:10:49.000000 HawaData-0.9.3/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3622 2023-08-06 11:10:49.139377 HawaData-0.9.3/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.9.3/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.125855 HawaData-0.9.3/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.9.3/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.128857 HawaData-0.9.3/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.9.3/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.9.3/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.9.3/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      142 2023-08-01 09:59:51.000000 HawaData-0.9.3/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.9.3/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.131830 HawaData-0.9.3/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.9.3/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    17368 2023-07-27 05:22:54.000000 HawaData-0.9.3/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6517 2023-07-27 05:22:54.000000 HawaData-0.9.3/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.9.3/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.9.3/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.136053 HawaData-0.9.3/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.9.3/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.9.3/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.9.3/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.9.3/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.9.3/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.9.3/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1181 2023-08-01 09:59:51.000000 HawaData-0.9.3/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.137688 HawaData-0.9.3/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.9.3/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    29123 2023-08-06 11:10:07.000000 HawaData-0.9.3/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.9.3/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-08-06 11:10:49.139921 HawaData-0.9.3/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.9.3/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-08-06 11:10:49.138510 HawaData-0.9.3/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.9.3/test/test_query.py
```

### Comparing `HawaData-0.9.2/HawaData.egg-info/PKG-INFO` & `HawaData-0.9.3/HawaData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -123,7 +123,8 @@
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
 - 0.9.0 use less item codes to upper
 - 0.9.1 add no answers error
 - 0.9.2 fix when without gender
+- 0.9.3 fix nan
```

### Comparing `HawaData-0.9.2/HawaData.egg-info/SOURCES.txt` & `HawaData-0.9.3/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/PKG-INFO` & `HawaData-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.9.2
+Version: 0.9.3
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -123,7 +123,8 @@
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
 - 0.9.0 use less item codes to upper
 - 0.9.1 add no answers error
 - 0.9.2 fix when without gender
+- 0.9.3 fix nan
```

### Comparing `HawaData-0.9.2/README.md` & `HawaData-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/base/db.py` & `HawaData-0.9.3/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/base/decos.py` & `HawaData-0.9.3/hawa/base/decos.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/base/init.py` & `HawaData-0.9.3/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/common/data.py` & `HawaData-0.9.3/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/common/query.py` & `HawaData-0.9.3/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/common/utils.py` & `HawaData-0.9.3/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/config.py` & `HawaData-0.9.3/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/data/klass.py` & `HawaData-0.9.3/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/data/province.py` & `HawaData-0.9.3/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/data/school.py` & `HawaData-0.9.3/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/data/student.py` & `HawaData-0.9.3/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/hawa/paper/health.py` & `HawaData-0.9.3/hawa/paper/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,14 +470,16 @@
         base = data.to_dict(orient='records')
         middle = {d[first_col]: d[second_col] / 100 for d in base}
         reverse_middle = {v: k for k, v in middle.items()}
         res = [(self._retain_prec(k), reverse_middle[k]) for k in sorted(reverse_middle.keys(), reverse=True)]
         return res
 
     def count_cond(self, a: float, b: float, target: str = ''):
+        a = 0 if math.isnan(a) else a
+        b = 0 if math.isnan(b) else b
         if a == b:
             condition = f'等于{target}' if target else '等于'
         elif a - b >= 5:
             condition = f'明显高于{target}' if target else '明显高于'
         elif abs(a - b) < 5:
             condition = f'与{target}的差异不明显' if target else '差异不明显于'
         elif a - b <= -5:
```

### Comparing `HawaData-0.9.2/hawa/paper/mht.py` & `HawaData-0.9.3/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/setup.py` & `HawaData-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.9.2/test/test_query.py` & `HawaData-0.9.3/test/test_query.py`

 * *Files identical despite different names*

