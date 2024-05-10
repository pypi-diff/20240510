# Comparing `tmp/eurmlsdk-0.0.77.tar.gz` & `tmp/eurmlsdk-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.77.tar", last modified: Wed May  8 11:20:58 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.78.tar", last modified: Fri May 10 09:56:03 2024, max compression
```

## Comparing `eurmlsdk-0.0.77.tar` & `eurmlsdk-0.0.78.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-08 11:20:58.336289 eurmlsdk-0.0.77/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.0.77/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.0.77/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      383 2024-05-08 11:20:58.336289 eurmlsdk-0.0.77/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.0.77/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-08 11:20:58.336289 eurmlsdk-0.0.77/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       31 2024-05-07 11:07:27.000000 eurmlsdk-0.0.77/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     3255 2024-05-08 10:45:05.000000 eurmlsdk-0.0.77/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)    10466 2024-05-07 10:55:35.000000 eurmlsdk-0.0.77/eurmlsdk/base_class.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4654 2024-05-08 11:17:33.000000 eurmlsdk-0.0.77/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-08 11:20:58.336289 eurmlsdk-0.0.77/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      383 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      321 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       46 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-08 11:20:58.000000 eurmlsdk-0.0.77/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-08 11:20:58.336289 eurmlsdk-0.0.77/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      735 2024-05-08 11:18:55.000000 eurmlsdk-0.0.77/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.949207 eurmlsdk-0.0.78/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3255 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5427 2024-05-10 09:55:14.000000 eurmlsdk-0.0.78/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       65 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      765 2024-05-10 09:55:31.000000 eurmlsdk-0.0.78/setup.py
```

### Comparing `eurmlsdk-0.0.77/eurmlsdk/__main__.py` & `eurmlsdk-0.0.78/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.77/eurmlsdk/base_class.py` & `eurmlsdk-0.0.78/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.77/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.78/eurmlsdk/eur_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,37 @@
         except TimeoutError as err:
             print("Connection Timeout Error: ", err)
             exit(1)
         except Exception as err:
             print("Error: %s" % err)
             exit(1)
 
+    def uploadToRemote(self, ssh_client, local_path, remote_path):
+        print("Uploading model {} to {}".format(local_path, remote_path))
+        sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
+        sftp_progress_bar.put(local_path, remote_path)
+        print("Model upload successful")
+
     def uploadModel(self, ssh_client, local_path, remote_path):
         try:
-            print("Uploading model {} to {}".format(local_path, remote_path))
             sftp = ssh_client.open_sftp()
-            sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
-            sftp_progress_bar.put(local_path, remote_path)
-            print("Model upload successful")
+            sftp.chdir("/home/embeduradmin/")
+            sftp.stat(remote_path)
+            print('Model File {} already exists'.format(remote_path.split("/")[-1]))
+            upload = input('Do you want to upload it again (y/n)? ')
+            while upload.lower() != 'y' and upload.lower() != 'n':
+                print("Your response ('{}') was not one of the expected responses: y, n".format(upload))
+                upload = input('Do you want to upload it again (y/n)? ')
+            if upload == 'y':
+                self.uploadToRemote(ssh_client, local_path, remote_path)
+            sftp.close()
+        except IOError:
+            self.uploadToRemote(ssh_client, local_path, remote_path)
             sftp.close()
+            exit(1)
         except Exception as err:
             print("Error uploading the model file: ", err)
             exit(1)
 
     def execute_script(self, ssh_client, script_path, modelFile):
         try:
             print("Starting script execution...")
```

### Comparing `eurmlsdk-0.0.77/setup.py` & `eurmlsdk-0.0.78/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.77',
+    version='0.0.78',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
         'paramiko',
+        'tensorflow==2.13.1',
         'tqdm',
         'ultralytics'
     ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
```

