# Comparing `tmp/storage-local-0.1.8.tar.gz` & `tmp/storage-local-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-local-0.1.8.tar", last modified: Fri Sep  8 14:23:15 2023, max compression
+gzip compressed data, was "storage-local-0.1.9.tar", last modified: Fri Sep  8 15:55:12 2023, max compression
```

## Comparing `storage-local-0.1.8.tar` & `storage-local-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:23:15.684387 storage-local-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-08 14:23:15.684387 storage-local-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-08 14:22:48.000000 storage-local-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:23:15.684387 storage-local-0.1.8/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-09-08 14:22:48.000000 storage-local-0.1.8/circles_local_aws_s3_storage_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-08 14:22:48.000000 storage-local-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 14:23:15.684387 storage-local-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-09-08 14:22:48.000000 storage-local-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:23:15.684387 storage-local-0.1.8/storage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-08 14:23:15.000000 storage-local-0.1.8/storage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-09-08 14:23:15.000000 storage-local-0.1.8/storage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 14:23:15.000000 storage-local-0.1.8/storage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-08 14:23:15.000000 storage-local-0.1.8/storage_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 14:23:15.684387 storage-local-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 14:22:48.000000 storage-local-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-09-08 14:22:48.000000 storage-local-0.1.8/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-09-08 14:22:48.000000 storage-local-0.1.8/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 15:55:12.664296 storage-local-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-08 15:55:12.664296 storage-local-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-08 15:54:48.000000 storage-local-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 15:55:12.664296 storage-local-0.1.9/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-09-08 15:54:48.000000 storage-local-0.1.9/circles_local_aws_s3_storage_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-08 15:54:48.000000 storage-local-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 15:55:12.664296 storage-local-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2023-09-08 15:54:48.000000 storage-local-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 15:55:12.664296 storage-local-0.1.9/storage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-09-08 15:55:12.000000 storage-local-0.1.9/storage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2023-09-08 15:55:12.000000 storage-local-0.1.9/storage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 15:55:12.000000 storage-local-0.1.9/storage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-08 15:55:12.000000 storage-local-0.1.9/storage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 15:55:12.664296 storage-local-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 15:54:48.000000 storage-local-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-09-08 15:54:48.000000 storage-local-0.1.9/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-09-08 15:54:48.000000 storage-local-0.1.9/tests/test_circles_storage.py
```

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/AWSStorage.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,29 @@
         aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY")
         self.client = boto3.client('s3',
                                    aws_access_key_id=aws_access_key_id,
                                    aws_secret_access_key=aws_secret_access_key)
 
     # uploads file to S3
 
-    def upload_file(self, local_path, filename, remote_path, created_user_id):
+    def upload_file(self, local_path, filename, remote_path, created_user_id, url = None):
         read_binary = 'rb'
         with open(local_path, read_binary) as file_obj:
             file_contents = file_obj.read()
 
         # Upload the file to S3 with the CRC32 checksum
         response = self.client.put_object(
             Bucket=self.bucket_name,
             Key=remote_path+filename,
             Body=file_contents,
             ChecksumAlgorithm='crc32'
         )
         if 'ETag' in response:
             id = self.database.uploadToDatabase(
-                remote_path, filename, self.region, created_user_id, constants.STORAGE_TYPE_ID, constants.FILE_TYPE_ID, constants.EXTENSION_ID)  # Constants needs to be replaced by parameter
+                remote_path, filename, self.region, created_user_id, constants.STORAGE_TYPE_ID, constants.FILE_TYPE_ID, constants.EXTENSION_ID, url)  # Constants needs to be replaced by parameter
             return id
         return None
 
     # download a file from s3 to local_path
     def download_file(self, remote_path, local_path):
         print(self.bucket_name,remote_path,local_path)
         self.client.download_file(self.bucket_name, remote_path, local_path)
```

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/CirclesStorage.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/CirclesStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,11 +148,11 @@
             # Set decode_content value to True, otherwise the downloaded image file's size will be zero.
             response.raw.decode_content = True
 
             # Open a local file with wb ( write binary ) permission.
             with open(local_file_name, 'wb') as f:
                 shutil.copyfileobj(response.raw, f)
             
-            self.s3.upload_file(local_file_name, local_file_name, remote_file_path, profile_id)
+            self.s3.upload_file(local_file_name, local_file_name, remote_file_path, profile_id, image_url)
             self.lgrins.end(object={'Image successfully downloaded: ' : local_file_name})
         else:
             self.lgrins.error('Image couldn\'t be retrieved')
```

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/FileTypeDB.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/StorageDB.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             password=os.getenv("RDS_PASSWORD"),
             database=os.getenv("RDS_DB_NAME")
         )
         self.cursor = self.mydb.cursor(buffered=True)
 
-    def uploadToDatabase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
+    def uploadToDatabase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id, url = None) -> int:
         add_storage = ("INSERT INTO storage.storage_view "
-                       "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) "
-                       "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
-        storage_data = (file_path, filename, region, created_user_id,
+                       "(path, filename, region, url, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) "
+                       "VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s)")
+        storage_data = (file_path, filename, region, url, created_user_id,
                         created_user_id, storage_type_id, file_type_id, extension_id)
         self.cursor.execute(add_storage, storage_data)
         self.mydb.commit()
         select_stmt = "SELECT LAST_INSERT_ID()"
         self.cursor.execute(select_stmt)
         last_insert_id = self.cursor.fetchone()[0]
         return int(last_insert_id)
```

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/StorageInterface.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.1.8/circles_local_aws_s3_storage_python/constants.py` & `storage-local-0.1.9/circles_local_aws_s3_storage_python/constants.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.1.8/setup.py` & `storage-local-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='storage-local',
-    version='0.1.8', # https://pypi.org/project/storage-local/
+    version='0.1.9', # https://pypi.org/project/storage-local/
     author="Circles",
     author_email="info@circle.zone",
     description="PyPI Package for Circles Storage functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

### Comparing `storage-local-0.1.8/storage_local.egg-info/SOURCES.txt` & `storage-local-0.1.9/storage_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storage-local-0.1.8/tests/test_S3.py` & `storage-local-0.1.9/tests/test_S3.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.1.8/tests/test_circles_storage.py` & `storage-local-0.1.9/tests/test_circles_storage.py`

 * *Files identical despite different names*

