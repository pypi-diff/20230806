# Comparing `tmp/kuki-0.9.8.tar.gz` & `tmp/kuki-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.9.8.tar", last modified: Thu Jul 27 15:27:28 2023, max compression
+gzip compressed data, was "kuki-0.9.9.tar", last modified: Sun Jul 30 16:16:37 2023, max compression
```

## Comparing `kuki-0.9.8.tar` & `kuki-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.953883 kuki-0.9.8/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.8/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-27 15:27:28.953883 kuki-0.9.8/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      463 2023-07-25 13:52:37.000000 kuki-0.9.8/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.951882 kuki-0.9.8/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.8/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.8/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1375 2023-07-23 05:45:31.000000 kuki-0.9.8/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.8/kuki/ktrl.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.8/kuki/ktrl_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4768 2023-07-27 15:23:50.000000 kuki-0.9.8/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4087 2023-07-23 15:13:37.000000 kuki-0.9.8/kuki/package_util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.952883 kuki-0.9.8/kuki/q/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.8/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-26 16:08:04.000000 kuki-0.9.8/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-27 06:39:46.000000 kuki-0.9.8/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.8/kuki/q/ktrl.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1918 2023-07-27 07:07:32.000000 kuki-0.9.8/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.8/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.8/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    20344 2023-07-27 15:26:18.000000 kuki-0.9.8/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.8/kuki/util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.952883 kuki-0.9.8/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       15 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-27 15:27:28.000000 kuki-0.9.8/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      468 2023-07-27 15:27:28.953883 kuki-0.9.8/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.8/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-27 15:27:28.953883 kuki-0.9.8/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.8/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.8/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.8/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15975 2023-07-27 15:05:32.000000 kuki-0.9.8/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-30 16:16:37.171639 kuki-0.9.9/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.9/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-30 16:16:37.171639 kuki-0.9.9/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      463 2023-07-25 13:52:37.000000 kuki-0.9.9/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-30 16:16:37.169639 kuki-0.9.9/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.9/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1359 2023-07-28 01:44:19.000000 kuki-0.9.9/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1375 2023-07-23 05:45:31.000000 kuki-0.9.9/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.9/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.9/kuki/ktrl_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4768 2023-07-27 15:23:50.000000 kuki-0.9.9/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4101 2023-07-30 12:56:48.000000 kuki-0.9.9/kuki/package_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-30 16:16:37.170639 kuki-0.9.9/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.9/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-26 16:08:04.000000 kuki-0.9.9/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-27 06:39:46.000000 kuki-0.9.9/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.9/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1918 2023-07-27 07:07:32.000000 kuki-0.9.9/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.9/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.9/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    20382 2023-07-30 12:57:33.000000 kuki-0.9.9/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.9/kuki/util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-30 16:16:37.170639 kuki-0.9.9/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12048 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       15 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-30 16:16:37.000000 kuki-0.9.9/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      468 2023-07-30 16:16:37.171639 kuki-0.9.9/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.9/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-30 16:16:37.171639 kuki-0.9.9/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.9/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.9/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.9/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15975 2023-07-27 15:05:32.000000 kuki-0.9.9/test/test_kuki.py
```

### Comparing `kuki-0.9.8/LICENSE` & `kuki-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/PKG-INFO` & `kuki-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.8
+Version: 0.9.9
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kuki-0.9.8/kuki/kest.py` & `kuki-0.9.9/kuki/kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/ktrl.py` & `kuki-0.9.9/kuki/ktrl.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/ktrl_util.py` & `kuki-0.9.9/kuki/ktrl_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/kuki.py` & `kuki-0.9.9/kuki/kuki.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/package_util.py` & `kuki-0.9.9/kuki/package_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class Kuki(TypedDict):
     name: str
     version: str
     description: str
     author: str
     git: str
+    type: str
     dependencies: Dict[str, str]
 
 
 def generate_json(name: str, description="", author="", git="", package_type="q"):
     if package_config_path.exists():
         overwrite = input("kuki.json already exists, overwrite: (yes/No) ").strip()
         if not overwrite or not overwrite.lower() in ["yes"]:
```

### Comparing `kuki-0.9.8/kuki/q/cli.q` & `kuki-0.9.9/kuki/q/cli.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/q/kest.q` & `kuki-0.9.9/kuki/q/kest.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/q/kuki.q` & `kuki-0.9.9/kuki/q/kuki.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/q/log.q` & `kuki-0.9.9/kuki/q/log.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/q/path.q` & `kuki-0.9.9/kuki/q/path.q`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki/registry_util.py` & `kuki-0.9.9/kuki/registry_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
         "versions": {
             version: {
                 "_id": "{}@{}".format(pkg_name, version),
                 "name": pkg_name,
                 "description": kuki.get("package", ""),
                 "author": {"name": kuki.get("author", "unknown")},
                 "publisher": user,
+                "type": kuki["type"],
                 "version": version,
                 "readme": package_util.load_readme(),
                 "dependencies": kuki.get("dependencies", {}),
                 "dist": {
                     "shasum": shasum.hexdigest(),
                     "tarball": "{}{}/-/{}".format(registry, pkg_name, tar_name),
                 },
```

### Comparing `kuki-0.9.8/kuki/util.py` & `kuki-0.9.9/kuki/util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/kuki.egg-info/PKG-INFO` & `kuki-0.9.9/kuki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.9.8
+Version: 0.9.9
 Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
 Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `kuki-0.9.8/kuki.egg-info/SOURCES.txt` & `kuki-0.9.9/kuki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/test/test_kest.py` & `kuki-0.9.9/test/test_kest.py`

 * *Files identical despite different names*

### Comparing `kuki-0.9.8/test/test_kuki.py` & `kuki-0.9.9/test/test_kuki.py`

 * *Files identical despite different names*

