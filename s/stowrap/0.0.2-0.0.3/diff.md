# Comparing `tmp/stowrap-0.0.2.tar.gz` & `tmp/stowrap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stowrap-0.0.2.tar", last modified: Sun Aug  6 12:57:49 2023, max compression
+gzip compressed data, was "stowrap-0.0.3.tar", last modified: Sun Aug  6 14:18:25 2023, max compression
```

## Comparing `stowrap-0.0.2.tar` & `stowrap-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 12:57:40.000000 stowrap-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 12:57:49.083281 stowrap-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-06 12:57:40.000000 stowrap-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 12:57:49.083281 stowrap-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-06 12:57:40.000000 stowrap-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.079281 stowrap-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.079281 stowrap-0.0.2/src/stowrap/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-06 12:57:40.000000 stowrap-0.0.2/src/stowrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-06 12:57:40.000000 stowrap-0.0.2/src/stowrap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/src/stowrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 12:57:49.000000 stowrap-0.0.2/src/stowrap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 12:57:49.083281 stowrap-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-06 12:57:40.000000 stowrap-0.0.2/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 14:18:16.000000 stowrap-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-06 14:18:25.636995 stowrap-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-06 14:18:16.000000 stowrap-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 14:18:25.636995 stowrap-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-06 14:18:16.000000 stowrap-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.632995 stowrap-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/src/stowrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-06 14:18:16.000000 stowrap-0.0.3/src/stowrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-06 14:18:16.000000 stowrap-0.0.3/src/stowrap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/src/stowrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-06 14:18:16.000000 stowrap-0.0.3/tests/test_upload.py
```

### Comparing `stowrap-0.0.2/LICENSE` & `stowrap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stowrap-0.0.2/PKG-INFO` & `stowrap-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stowrap
-Version: 0.0.2
+Version: 0.0.3
 Summary: stowrap: Python Storage Service Wrapper.
 Home-page: https://github.com/yokoe/stowrap
 Download-URL: https://github.com/yokoe/stowrap
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
@@ -29,9 +29,10 @@
 
 c = stowrap.Client("s3")
 
 ```
 
 ### Upload a file
 ```
-c.upload("my-bucket", "/path/to/local/file", "dstfile.txt")
+result = c.upload("my-bucket", "/path/to/local/file", "dstfile.txt")
+print(result.url)
 ```
```

### Comparing `stowrap-0.0.2/setup.py` & `stowrap-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "stowrap: Python Storage Service Wrapper."
 NAME = "stowrap"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/stowrap"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 PYTHON_REQUIRES = ">=3.9"
 INSTALL_REQUIRES = [
     "gcshus",
     "boto3",
 ]
 PACKAGES = ["stowrap"]
 PACKAGE_DIR = {"": "src"}
```

### Comparing `stowrap-0.0.2/src/stowrap.egg-info/PKG-INFO` & `stowrap-0.0.3/src/stowrap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stowrap
-Version: 0.0.2
+Version: 0.0.3
 Summary: stowrap: Python Storage Service Wrapper.
 Home-page: https://github.com/yokoe/stowrap
 Download-URL: https://github.com/yokoe/stowrap
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
@@ -29,9 +29,10 @@
 
 c = stowrap.Client("s3")
 
 ```
 
 ### Upload a file
 ```
-c.upload("my-bucket", "/path/to/local/file", "dstfile.txt")
+result = c.upload("my-bucket", "/path/to/local/file", "dstfile.txt")
+print(result.url)
 ```
```

### Comparing `stowrap-0.0.2/tests/test_upload.py` & `stowrap-0.0.3/tests/test_upload.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,23 +5,29 @@
 from datetime import datetime
 import os
 
 load_dotenv()
 
 
 class TestUpload(unittest.TestCase):
-    def upload_test_file(self, service, bucket, filename):
+    def upload_test_file(self, service, bucket, filename) -> stowrap.UploadResult:
         with tempfile.TemporaryDirectory() as tempdir:
             testfile = os.path.join(tempdir, "test.txt")
             with open(testfile, "w") as f:
                 f.write(datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
-            stowrap.Client(service).upload(bucket, testfile, filename)
+            return stowrap.Client(service).upload(bucket, testfile, filename)
 
     def test_gcs_upload(self):
-        self.upload_test_file("gcs", os.environ["TEST_GCS_BUCKET"], "test.txt")
+        result = self.upload_test_file("gcs", os.environ["TEST_GCS_BUCKET"], "test.txt")
+        self.assertTrue(result.url.startswith("https://storage.googleapis.com/"))
 
     def test_s3_upload(self):
-        self.upload_test_file("s3", os.environ["TEST_S3_BUCKET"], "test.txt")
+        bucket = os.environ["TEST_S3_BUCKET"]
+        result = self.upload_test_file("s3", bucket, "test.txt")
+        self.assertTrue(
+            result.url.startswith(f"https://{bucket}.s3.amazonaws.com/"),
+            f"url is {result.url}",
+        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

