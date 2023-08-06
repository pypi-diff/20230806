# Comparing `tmp/storage-local-0.0.8.tar.gz` & `tmp/storage-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-local-0.0.8.tar", last modified: Mon Jul 31 11:08:53 2023, max compression
+gzip compressed data, was "storage-local-0.0.9.tar", last modified: Sun Aug  6 17:31:37 2023, max compression
```

## Comparing `storage-local-0.0.8.tar` & `storage-local-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 11:08:53.535877 storage-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-31 11:08:31.000000 storage-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 11:08:31.000000 storage-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:08:53.535877 storage-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-31 11:08:31.000000 storage-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/storage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-06 17:31:37.346613 storage-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 17:31:12.000000 storage-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-06 17:31:12.000000 storage-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:31:37.346613 storage-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-06 17:31:12.000000 storage-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/storage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/test_circles_storage.py
```

### Comparing `storage-local-0.0.8/circles_local_aws_s3_storage_python/AWSStorage.py` & `storage-local-0.0.9/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-
 import os
 import boto3
 
 from circles_local_aws_s3_storage_python.StorageInterface import StorageInterface
 from circles_local_aws_s3_storage_python.StorageDB import StorageDB
+from circles_local_aws_s3_storage_python import constants
 
-debug = False
 class AwsS3Storage(StorageInterface):
-    
 
     def __init__(self, bucket_name, region):
-        if (debug): print("Initializing AwsS3Storage bucket_name="+str(bucket_name)+' region='+str(region))
         self.region = region
         self.bucket_name = bucket_name
         self.database = StorageDB()
-        if (debug): print("AWS_ACCESS_KEY_ID: " +os.getenv("AWS_ACCESS_KEY_ID"))
-        if (debug): print("AWS_SECRET_ACCESS_KEY: " +os.getenv("AWS_SECRET_ACCESS_KEY"))
         self.client = boto3.client('s3',
                                    aws_access_key_id=os.getenv(
                                        "AWS_ACCESS_KEY_ID"),
                                    aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"))
 
     # uploads file to S3
 
@@ -32,16 +27,16 @@
         response = self.client.put_object(
             Bucket=self.bucket_name,
             Key=remote_path+filename,
             Body=file_contents,
             ChecksumAlgorithm='crc32'
         )
         if 'ETag' in response:
-            id = self.database.uploadToDataBase(
-                remote_path, filename, self.region, created_user_id, 1, 1, 1)  # One's needs to be replaced by parameter
+            id = self.database.uploadToDatabase(
+                remote_path, filename, self.region, created_user_id, constants.STORAGE_TYPE_ID, constants.FILE_TYPE_ID, constants.EXTENSION_ID)  # Constants needs to be replaced by parameter
             return id
         return None
 
     # download a file from s3 to local_path
     def download_file(self, remote_path, local_path):
         self.client.download_file(self.bucket_name, remote_path, local_path)
```

### Comparing `storage-local-0.0.8/circles_local_aws_s3_storage_python/FileTypeDB.py` & `storage-local-0.0.9/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageDB.py` & `storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     def __init__(self) -> None:
         self.mydb = mysql.connector.connect(
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             passwd=os.getenv("RDS_PASSWORD"),
             database=os.getenv("RDS_DB_NAME")
         )
-        self.cursor = self.mydb.cursor()
+        self.cursor = self.mydb.cursor(buffered=True)
 
-    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, file_extension_id) -> int:
+    def uploadToDatabase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
         add_storage = ("INSERT INTO storage.storage_table "
                        "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) "
                        "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
         storage_data = (file_path, filename, region, created_user_id,
-                        created_user_id, storage_type_id, file_type_id, file_extension_id)
+                        created_user_id, storage_type_id, file_type_id, extension_id)
         self.cursor.execute(add_storage, storage_data)
         self.mydb.commit()
         select_stmt = "SELECT LAST_INSERT_ID()"
         self.cursor.execute(select_stmt)
         last_insert_id = self.cursor.fetchone()[0]
         return int(last_insert_id)
```

### Comparing `storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageInterface.py` & `storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.8/storage_local.egg-info/SOURCES.txt` & `storage-local-0.0.9/storage_local.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 circles_local_aws_s3_storage_python/AWSStorage.py
 circles_local_aws_s3_storage_python/CirclesStorage.py
 circles_local_aws_s3_storage_python/FileTypeDB.py
 circles_local_aws_s3_storage_python/StorageDB.py
 circles_local_aws_s3_storage_python/StorageInterface.py
 circles_local_aws_s3_storage_python/__init__.py
+circles_local_aws_s3_storage_python/constants.py
 storage_local.egg-info/PKG-INFO
 storage_local.egg-info/SOURCES.txt
 storage_local.egg-info/dependency_links.txt
 storage_local.egg-info/top_level.txt
 tests/__init__.py
 tests/test_S3.py
 tests/test_circles_storage.py
```

### Comparing `storage-local-0.0.8/tests/test_S3.py` & `storage-local-0.0.9/tests/test_S3.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,58 +4,48 @@
 import unittest
 from dotenv.main import load_dotenv
 
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 from circles_local_aws_s3_storage_python.StorageDB import StorageDB
 load_dotenv()
 
-# TODO: Get the debug from Environment using our method in Python util/SDK
-debug=False
+
+PROFILE_ID = 1
+
 
 class s3_test(unittest.TestCase):
+
     def setUp(self) -> None:
-        # TODO: Write to Logger with Storge_Testing Component Id
-        if (debug): print('Bucket=', end='')
-        if (debug): print(os.getenv("BUCKET_NAME"))
-        if (debug): print('Region=',  end='')
-        if (debug): print(os.getenv("REGION"))
-        if (debug): print(os.getenv("BUCKET_NAME"))
         self.s3_resource = boto3.resource('s3')
         self.awsS3 = AwsS3Storage(
             os.getenv("BUCKET_NAME"), os.getenv("REGION"))
         self.test_file_contents = b'this it a file test!'
         self.database = StorageDB()
 
     def test_upload(self):
         cwd = os.getcwd()
-        # TODO: Use consts
         filepath = os.path.join(cwd, 'tests/test.txt')
-        # TODO: Use consts
         functionId = self.awsS3.upload_file(
-            filepath, 'test.txt', 'python/', 1)
+            filepath, 'test.txt', 'python/', PROFILE_ID)
         s3_object = self.s3_resource.Object(
             os.getenv("BUCKET_NAME"), 'python/test.txt')
         s3_file_contents = s3_object.get()['Body'].read()
         self.assertEqual(s3_file_contents, self.test_file_contents)
         actualId = self.database.getLastId()
         self.assertEqual(functionId, actualId)
 
     def test_download(self):
-        # As I'm not sure setUp was running and we need to run test_upload() before running test_download()
-        self.setUp()
-        self.test_upload()
-        
         cwd = os.getcwd()
         self.awsS3.download_file(
             'python/test.txt', cwd+'/test.txt')
         assert os.path.isfile(
             cwd+'/test.txt')
 
     def test_logical_delete(self):
-        self.awsS3.delete_file('python\\', 'test.txt', 1)
+        self.awsS3.delete_file('python/', 'test.txt', PROFILE_ID)
         result = self.database.getEndTimeStampFromDB(
-            'python\\', 'test.txt', os.getenv("REGION"))
+            'python/', 'test.txt', os.getenv("REGION"))
         self.assertIsNotNone(result[0])
 
 
 if __name__ == '__main__':
     unittest.main()
```

